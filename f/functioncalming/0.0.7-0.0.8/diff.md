# Comparing `tmp/functioncalming-0.0.7.tar.gz` & `tmp/functioncalming-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functioncalming-0.0.7.tar", max compression
+gzip compressed data, was "functioncalming-0.0.8.tar", max compression
```

## Comparing `functioncalming-0.0.7.tar` & `functioncalming-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2024-04-03 13:50:14.359647 functioncalming-0.0.7/LICENSE
--rw-r--r--   0        0        0     7412 2024-04-03 17:49:36.616998 functioncalming-0.0.7/README.md
--rw-r--r--   0        0        0       90 2024-04-03 13:50:14.359876 functioncalming-0.0.7/functioncalming/__init__.py
--rw-r--r--   0        0        0    22304 2024-04-03 17:55:37.039789 functioncalming-0.0.7/functioncalming/client.py
--rw-r--r--   0        0        0     4308 2024-04-03 13:50:14.360289 functioncalming-0.0.7/functioncalming/distil.py
--rw-r--r--   0        0        0     7047 2024-04-03 17:22:50.208270 functioncalming-0.0.7/functioncalming/utils.py
--rw-r--r--   0        0        0      749 2024-04-03 17:55:59.808034 functioncalming-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8167 1970-01-01 00:00:00.000000 functioncalming-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-03 13:50:14.359647 functioncalming-0.0.8/LICENSE
+-rw-r--r--   0        0        0     7412 2024-04-03 17:49:36.616998 functioncalming-0.0.8/README.md
+-rw-r--r--   0        0        0       73 2024-04-08 13:16:50.206511 functioncalming-0.0.8/functioncalming/__init__.py
+-rw-r--r--   0        0        0    25285 2024-04-09 15:20:58.848674 functioncalming-0.0.8/functioncalming/client.py
+-rw-r--r--   0        0        0      573 2024-04-09 09:19:47.440351 functioncalming-0.0.8/functioncalming/types.py
+-rw-r--r--   0        0        0     7503 2024-04-09 14:11:47.438473 functioncalming-0.0.8/functioncalming/utils.py
+-rw-r--r--   0        0        0      749 2024-04-09 15:26:57.276005 functioncalming-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8167 1970-01-01 00:00:00.000000 functioncalming-0.0.8/PKG-INFO
```

### Comparing `functioncalming-0.0.7/LICENSE` & `functioncalming-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `functioncalming-0.0.7/README.md` & `functioncalming-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `functioncalming-0.0.7/functioncalming/client.py` & `functioncalming-0.0.8/functioncalming/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import dataclasses
+import functools
 import uuid
 
 import json
 import logging
 import os
-from typing import Callable, TextIO, Awaitable, Literal
+from typing import TextIO, Literal, Dict
 from functools import cached_property
 
-from openai._types import NOT_GIVEN
+from openai._types import NOT_GIVEN, NotGiven
+from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_message_tool_call import Function
 from pydantic import BaseModel, ValidationError
 from openai import AsyncOpenAI
 
 from openai.types.chat import ChatCompletion, ChatCompletionMessage, ChatCompletionMessageToolCall, \
     ChatCompletionToolMessageParam, ChatCompletionSystemMessageParam, ChatCompletionUserMessageParam, \
-    ChatCompletionToolChoiceOptionParam, ChatCompletionAssistantMessageParam, ChatCompletionMessageParam
+    ChatCompletionToolChoiceOptionParam, ChatCompletionAssistantMessageParam, ChatCompletionMessageParam, \
+    ChatCompletionToolParam
 from openai.types.completion_usage import CompletionUsage
-from functioncalming.utils import Messages, invoke_callback_function, FineTuningData, InnerValidationError, \
-    create_openai_function, OpenAIFunction, ToolCallError
+from functioncalming.utils import invoke_callback_function, FineTuningData, InnerValidationError, \
+    create_openai_function, OpenAIFunction, ToolCallError, create_abbreviated_openai_function, \
+    serialize_openai_function_result, log_finetuning_data
+from functioncalming.types import BaseModelOrJsonCompatible, Messages, BaseModelFunction
 
 _client = None
 
 
 def get_client():
     global _client
     if not _client:
@@ -37,20 +42,14 @@
     global _client
     _client = client
 
 
 DEFAULT_BEHAVIOR = "default_behavior"
 
 
-type SimpleJsonCompatible = str | int | float | bool
-type JsonCompatible = dict[str, SimpleJsonCompatible | JsonCompatible] | list[SimpleJsonCompatible | JsonCompatible] | SimpleJsonCompatible
-type BaseModelOrJsonCompatible = BaseModel | JsonCompatible
-type BaseModelFunction = Callable[..., BaseModelOrJsonCompatible] | Callable[..., Awaitable[BaseModelOrJsonCompatible]]
-
-
 COSTS_BY_MODEL = {
     # GPT-4 Turbo
     "gpt-4-turbo": (0.01, 0.03),
     "gpt-4-0125-preview": (0.01, 0.03),  # actually a Turbo model
     "gpt-4-1106-preview": (0.01, 0.03),  # actually a Turbo model
     "gpt-4-vision-preview": (0.01, 0.03),
     "gpt-4-1106-vision-preview": (0.01, 0.03),
@@ -71,15 +70,15 @@
     "gpt-3.5-turbo-16k": (0.0005, 0.0015),
 }
 
 
 class ToolCallShortcut:
     def __init__(self, message: ChatCompletionMessage):
         self.model = None
-        self.message: ChatCompletionMessage = message
+        self.choices = [Choice(finish_reason="tool_calls", index=0, message=message)]
         self.usage: CompletionUsage = CompletionUsage(
             completion_tokens=0, prompt_tokens=0, total_tokens=0
         )
 
 
 @dataclasses.dataclass
 class CalmResponse:
@@ -87,29 +86,26 @@
     tool_call_results: list[BaseModelOrJsonCompatible]
     messages: Messages
     error: Exception | None
     retries_done: int
 
     _rewritten_from: int
     _omitted_messages: Messages
-    _unaltered_first_message: ChatCompletionMessageParam | None
 
     # multiple completions means there were retries
     raw_completions: list[ChatCompletion | ToolCallShortcut]
     """
     All the ChatCompletion objects returned by OpenAI during this call, ordered chronologically (last is newest).
-    Multiple completions may be returned if retrys were performed.
+    Multiple completions may be returned if retries were performed.
     """
 
     @cached_property
     def messages_raw(self):
         """The non-rewritten message history as it was actually performed against the API."""
         res = self.messages[:self._rewritten_from] + self._omitted_messages
-        if self._unaltered_first_message is not None:
-            res[0] = self._unaltered_first_message
         return res
 
     @property
     def last_message(self) -> ChatCompletionAssistantMessageParam:
         return self.messages[-1]
 
     @property
@@ -149,234 +145,354 @@
         return model, total_cost, usage
 
 
 async def get_completion(
         messages: Messages | None = None,
         system_prompt: str | None = None,
         user_message: str | None = None,
-        distil_system_prompt: str | None = None,
         tools: list[type[BaseModel] | BaseModelFunction] | None = None,
         tool_choice: Literal[DEFAULT_BEHAVIOR] | ChatCompletionToolChoiceOptionParam = DEFAULT_BEHAVIOR,
+        abbreviate_tools: bool = False,
+        abbreviation_system_prompt: str | None = "Shortcut tool calling active! If calling tools, omit arguments.",
         retries: int = 0,
-        pass_results_to_model: bool = True,
         rewrite_log_destination: str | TextIO | None = None,
         rewrite_log_extra_data: dict | None = None,
         openai_client: AsyncOpenAI | None = None,
         model: Literal["gpt-3.5-turbo", "gpt-4-1106-preview"] | str = None,
+        _track_raw_request_summaries: bool = False,
         **kwargs
 ) -> CalmResponse:
     """
     Get a completion with validated function call responses from the chat completions API.
 
     :param messages: Message history. Should be None if system_prompt and/or user_message are set
-    :param system_prompt: Initial system message (will be added to the beginning of the history - typically used without a 'history' param)
-        (if set, do not supply an initial system message in 'history')
-    :param user_message: Next user message (will be appended to the history)
-    :param distil_system_prompt: If set, the first message of the history will be rewritten to this system message
-        (useful for distillation trainng data generation)
+    :param system_prompt: Initial system message. Will be added to the beginning of the history, typically used without
+        the 'messages' param. (if set, do not supply an initial system message in 'messages')
+    :param user_message: Next user message (will be appended to the message history)
     :param tools: list of available tools, given either as BaseModels or functions that return BaseModel instances
     :param tool_choice: By default, forces a tool call if only one tool is available. Otherwise, same as vanilla OpenAI
+    :param abbreviate_tools: If true, tools are passed to the model without their param signature first to save tokens.
+        Once the model tries to call a tool, the conversation is replayed with the full definition of that tool only.
+        Setting this to True also allows one additional attempted generation (i.e. up to retries + 2 total calls to the
+        API)
+    :param abbreviation_system_prompt: An optional system prompt to insert in the message history before generating the
+        first completion during abbreviated tool calling. Usually this should tell the model not to supply tool
+        arguments to not waste tokens.
     :param retries: number of attempts to give the model to fix broken function calls (first try not counted)
-    :param rewrite_history_in_place: If true, the history that was passed in will be modified in-place
-    :param pass_results_to_model: If true, function results (or created models) are added to the message history
     :param rewrite_log_destination: filename or io handle to log fine-tuning data to
     :param rewrite_log_extra_data: extra data to merge into the jsonl line for this log entry
     :param openai_client: optional AsyncOpenAI client to use (use set_client() to set a default client)
     :param model: Which OpenAI model to use for the completion
-    :param kwargs:
-    :return: a tuple of (created models or function responses, rewritten message history)
+    :param _track_raw_request_summaries: If true, adds a _raw_request_summary field to each of the objects in
+        CalmResponse.raw_completions. This can be useful for understanding the full (virtual) message history and set of
+        tools that was included with each request.
+    :param kwargs: Other keyword arguments to pass to the OpenAI completions API call
+    :return: a CalmResponse object
     """
     # make a copy, we do not edit the passed-in message history
-    if messages is not None:
-        messages = messages[:]
+    internal_messages = messages[:] if messages is not None else []
+    retries = max(0, retries)
 
-    messages = initialize_and_validate_message_history(
-        messages=messages,
+    internal_messages = initialize_and_validate_message_history(
+        messages=internal_messages,
         system_prompt=system_prompt,
-        user_message=user_message,
-        distil_system_prompt=distil_system_prompt
+        user_message=user_message
     )
-    rewrite_cutoff = len(messages)
     openai_client = openai_client or get_client()
 
     model = model or os.environ.get("OPENAI_MODEL")
     if model is None:
         raise ValueError("No model specified and OPENAI_MODEL is not set.")
 
     tools = tools or []
-    openai_functions, distillery_openai_functions = process_tool_definitions(tools)
-    available_function_names: set[str] = set(openai_functions.keys())
+    calm_functions = process_tool_definitions(tools)
+
+    abbreviation_mode = abbreviate_tools
+    abbreviation_mode_attempted_calls: set[str] = set()
 
+    available_function_names: set[str] = set(calm_functions.openai_functions.keys())
+
+    # tracks successful tool call outputs
     result_instances: list[BaseModel] = []
-    tries_done = 0  # first try is not a retry
+
+    # for tracking what "really happened"
+    total_completions_generated = 0
+    total_generations_allowed = (2 if abbreviation_mode else 1) + retries
+    raw_completions: list[ChatCompletion | ToolCallShortcut] = []
+
+    # for message history rewriting
+    rewrite_cutoff = len(internal_messages)
     successful_tool_calls: list[ChatCompletionMessageToolCall] = []
     successful_tool_responses: list[ChatCompletionToolMessageParam] = []
-    last_message_dict = None
+
+    if abbreviation_mode and abbreviation_system_prompt is not None:
+        # this will be cut off once abbreviation mode is no longer active
+        internal_messages.append({"role": 'system', 'content': abbreviation_system_prompt})
 
     errors: list[Exception] | None = []
-    raw_completions: list[ChatCompletion | ToolCallShortcut] = []
-    while tries_done + 1 <= 1 + retries:
-        tries_done += 1
-        if tool_choice == DEFAULT_BEHAVIOR:
-            current_tool_choice = get_tool_choice_for_default_behavior(available_function_names)
-        else:
-            current_tool_choice = tool_choice
+    while total_completions_generated < total_generations_allowed:
+        openai_functions: dict[str, OpenAIFunction] = calm_functions.openai_functions
 
-        shortcut: ChatCompletionMessage | None = await maybe_shortcut_trivial_function_call(
-            available_function_names,
-            openai_functions
+        if abbreviation_mode:
+            if total_completions_generated == total_generations_allowed - 1:
+                raise ToolCallError(
+                    f"Ran out of retries during abbreviation phase "
+                    f"({total_completions_generated} completions have been generated, 1 remains, but we are still in abbreviation mode: full tool calls can't be executed)"
+                ) from ExceptionGroup("Tool calling validation errors", errors)
+            openai_functions = calm_functions.abbreviated_openai_functions
+
+        generated_completion = await _generate_one_completion(
+            messages=internal_messages,
+            openai_functions=openai_functions,
+            available_function_names=available_function_names,
+            tool_choice=tool_choice,
+            model=model,
+            openai_client=openai_client,
+            _track_raw_request_summaries=_track_raw_request_summaries,
+            **kwargs
         )
+        total_completions_generated += 1
+        raw_completions.append(generated_completion)
 
-        if shortcut is not None:
-            last_message = shortcut
-            raw_completions.append(
-                ToolCallShortcut(message=shortcut)
-            )
-        else:
-            completion: ChatCompletion = await openai_client.chat.completions.create(
-                messages=messages,
-                model=model,
-                tools=[openai_functions[name].tool_definition for name in available_function_names] or NOT_GIVEN,
-                tool_choice=current_tool_choice,
-                **kwargs
-            )
-            raw_completions.append(completion)
-            last_message: ChatCompletionMessage = completion.choices[0].message
-
-        messages.append(last_message.model_dump(
-            exclude_unset=True, exclude_none=True
-        ))  # make sure the history only has dict objects
+        last_message: ChatCompletionMessage = generated_completion.choices[0].message
+        internal_messages.append(
+            # make sure the history only has dict objects
+            last_message.model_dump(exclude_unset=True, exclude_none=True)
+        )
 
         if not last_message.tool_calls:
+            # no tool calls: just break the loop (we're done)
             break
 
-        num_successful = 0
-        num_failed = 0
-        current_errors: list[ValidationError | ToolCallError] = []
-        new_available_function_names = set()
-        for tool_call in last_message.tool_calls:
-            function_name = tool_call.function.name
-
-            if function_name not in openai_functions:
-                e = ToolCallError(f"Error: function `{function_name}` does not exist.")
-                handle_function_calling_error(
-                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
-                )
-                new_available_function_names = available_function_names  # could be anything
-                num_failed += 1
-                continue
-
-            openai_function = openai_functions[function_name]
-            try:
-                arguments = json.loads(tool_call.function.arguments)
-            except json.JSONDecodeError as e:
-                new_available_function_names.add(function_name)  # available for retry
-                handle_function_calling_error(
-                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
-                )
-                num_failed += 1
-                continue
+        # there were tool calls, let's try to execute them
+        outcomes = await execute_tool_calls(
+            tool_calls=last_message.tool_calls,
+            openai_functions=openai_functions
+        )
 
-            try:
-                result_instance, result_for_model, maybe_serialized_result = await invoke_callback_function(
-                    openai_function,
-                    kwargs=arguments,
-                    history=messages,
-                    serialize_result_for_model=pass_results_to_model
-                )
-                tool_response = ChatCompletionToolMessageParam(
-                    role="tool",
-                    tool_call_id=tool_call.id,
-                    content=result_for_model
-                )
-                if openai_function.is_distillery:
-                    distillery_tool = distillery_openai_functions[function_name]
-                    tool_call, tool_response = adjust_distillery_call_for_clean_history(
-                        new_function_name=distillery_tool.name,
-                        serialized_result=maybe_serialized_result,
-                        tool_call=tool_call
-                    )
-                messages.append(tool_response)
-                result_instances.append(result_instance)
-                successful_tool_calls.append(tool_call)
-                successful_tool_responses.append(tool_response)
-                num_successful += 1
-            except InnerValidationError as e:
-                # There is not really a need for any custom handling vs. other exceptions here - we just raise.
-                # I am just making clear that *inner* validation errors will not lead to a retry,
-                # since the model did fine calling the tool here.
-                # To force a retry due to a semantic error the model should correct, raise a ToolCallError instead
-                raise e
-            except (ValidationError, ToolCallError) as e:
-                new_available_function_names.add(function_name)  # available for retry
-                handle_function_calling_error(
-                    e=e, current_errors=current_errors, history=messages, tool_call=tool_call
-                )
-                num_failed += 1
+        new_successful_instances = [outcome.result for outcome in outcomes if outcome.success]
+        new_successful_tool_calls = [outcome.raw_tool_call for outcome in outcomes if outcome.success]
+        new_successful_tool_responses = [outcome.to_response() for outcome in outcomes if outcome.success]
+        # Note: this may be a mixture of successful responses and errors
+        new_messages = [outcome.to_response() for outcome in outcomes]
+
+        # 'errors' is overwritten intentionally, we only ever care about the errors of the last tool call(s)
+        errors = [outcome.result for outcome in outcomes if not outcome.success]
+
+        if abbreviation_mode:
+            # track any (valid) function that the model tried to call
+            #  once we exit abbreviation mode, all of them need to be available
+            abbreviation_mode_attempted_calls |= set(
+                outcome.tool_name for outcome in outcomes if outcome.tool_name is not None
+            )
 
-        if not num_failed:
-            errors = []
+            # if we are still in abbreviation mode and all calls were successful:
+            #   turn off abbreviation mode
+            #   reset the message history to before the tool calls
+            #   but only allow the tool calls that were actually made
+            if not errors:
+                # end loop early, cutting all of the abbreviated function calls from the message history
+                internal_messages = internal_messages[:rewrite_cutoff]
+                abbreviation_mode = False
+                # however, also restrict the set of functions to those that the model actually tried to call
+                available_function_names = abbreviation_mode_attempted_calls
+                # on the next iteration, the model will now be able to choose only from these functions,
+                #  but now with full definitions given
+                continue
+        else:
+            # if we are not in abbreviation mode, we just track the outputs and go on to handle errors
+            result_instances += new_successful_instances
+            successful_tool_calls += new_successful_tool_calls
+            successful_tool_responses += new_successful_tool_responses
+
+        internal_messages += new_messages
+
+        if errors:
+            # error handling logic actually looks the same between abbreviation mode and regular mode
+            num_failed = len(errors)
+            num_successful = sum(outcome.success for outcome in outcomes)
+
+            tool_names_for_next_attempt = set(outcome.tool_name for outcome in outcomes if not outcome.success)
+            if None in tool_names_for_next_attempt:
+                # the model called an unknown function: we can't tell which one it needs to retry,
+                # so we pass in all names again to let it retry any one of them
+                tool_names_for_next_attempt = available_function_names
+
+            logging.debug(f"Attempt {total_completions_generated}/{retries + 1}: {num_failed} errors")
+            internal_messages.append({
+                "role": "system",
+                "content": f"{num_failed}/{num_failed + num_successful} tool calls failed. "
+                           f"Please carefully recall the tool definition(s) and repeat all failed calls "
+                           f"(but only repeat the failed calls!)."
+            })
+            available_function_names = tool_names_for_next_attempt
+        else:
+            # defensive; if we were in abbreviation mode with no errors, the loop should have been continued above
+            assert not abbreviation_mode
+            # no errors: break the loop
             break
 
-        logging.debug(f"Attempt {tries_done}/{retries + 1}: {num_failed} errors")
-        errors = current_errors
-        messages.append({
-            "role": "system",
-            "content": f"{num_failed}/{num_failed + num_successful} tool calls failed. "
-                       f"Please carefully recall the function definition(s) and repeat all failed calls "
-                       f"(but only repeat the failed calls!)."
-        })
-        available_function_names = new_available_function_names
-
-    unaltered_first_message, omitted_messages = rewrite_message_history(
-        messages=messages,
+    omitted_messages = rewrite_message_history(
+        messages=internal_messages,
         rewrite_cutoff=rewrite_cutoff,
         successful_tool_calls=successful_tool_calls,
-        successful_tool_responses=successful_tool_responses,
-        distil_system_prompt=distil_system_prompt,
+        successful_tool_responses=successful_tool_responses
     )
 
     final_error = None
     if errors:
-        final_error = ExceptionGroup("Function calling validation errors", errors)
+        final_error = ExceptionGroup("Tool calling validation errors", errors)
     elif rewrite_log_destination is not None:
-        functions_coalesced: list[OpenAIFunction] = list({**openai_functions, **distillery_openai_functions}.values())
+        functions_coalesced: list[OpenAIFunction] = list(calm_functions.openai_functions.values())
         log_finetuning_data(
             destination=rewrite_log_destination,
-            messages=messages,
+            messages=internal_messages,
             functions=functions_coalesced,
             extra_data=rewrite_log_extra_data
         )
 
     return CalmResponse(
         success=final_error is None,
         tool_call_results=result_instances,
-        messages=messages,
+        messages=internal_messages,
         _rewritten_from=rewrite_cutoff,
         _omitted_messages=omitted_messages,
-        _unaltered_first_message=unaltered_first_message,
         error=final_error,
-        retries_done=tries_done - 1,
+        retries_done=total_completions_generated - (2 if abbreviate_tools else 1),
         raw_completions=raw_completions
     )
 
 
-def handle_function_calling_error(
-        e: ValidationError | ToolCallError | json.JSONDecodeError,
-        current_errors: list[ValidationError | ToolCallError | json.JSONDecodeError],
-        history: Messages,
-        tool_call
+@dataclasses.dataclass
+class RawRequestSummary:
+    messages: Messages
+    tools: list[ChatCompletionToolParam] | NotGiven
+    tool_choice: ChatCompletionToolChoiceOptionParam | dict | NotGiven
+
+
+async def _generate_one_completion(
+        messages: Messages,
+        openai_functions: dict[str, OpenAIFunction],
+        available_function_names: set[str],
+        tool_choice: Literal[DEFAULT_BEHAVIOR] | ChatCompletionToolChoiceOptionParam,
+        model: str,  # todo
+        openai_client: AsyncOpenAI,
+        _track_raw_request_summaries: bool,
+        **kwargs
 ):
-    tool_response = ChatCompletionToolMessageParam(
-        role="tool",
-        tool_call_id=tool_call.id,
-        content=f"Error: {e}"
+    if tool_choice == DEFAULT_BEHAVIOR:
+        current_tool_choice = get_tool_choice_for_default_behavior(available_function_names)
+    else:
+        current_tool_choice = tool_choice
+
+    current_tools = [openai_functions[name].tool_definition for name in available_function_names] or NOT_GIVEN
+
+    shortcut: ChatCompletionMessage | None = await maybe_shortcut_trivial_function_call(
+        available_function_names,
+        openai_functions
     )
-    history.append(tool_response)
-    current_errors.append(e)
+    generated_completion: ChatCompletion | ToolCallShortcut
+    if shortcut is not None:
+        generated_completion = ToolCallShortcut(message=shortcut)
+    else:
+        generated_completion = await openai_client.chat.completions.create(
+            messages=messages,
+            model=model,
+            tools=current_tools,
+            tool_choice=current_tool_choice,
+            **kwargs
+        )
+
+    if _track_raw_request_summaries:
+        generated_completion._raw_request_summary = RawRequestSummary(
+            messages=messages[:], tools=current_tools, tool_choice=current_tool_choice
+        )
+    return generated_completion
+
+
+@dataclasses.dataclass
+class ToolCallOutcome:
+    success: bool
+    tool_call_id: str
+    raw_tool_call: ChatCompletionMessageToolCall
+    result: BaseModelOrJsonCompatible | Exception
+    tool_name: str | None
+
+    def to_response(self) -> ChatCompletionToolMessageParam:
+        return ChatCompletionToolMessageParam(
+            role="tool",
+            tool_call_id=self.tool_call_id,
+            content=serialize_openai_function_result(self.result) if self.success else f"Error: {self.result}"
+        )
+
+
+async def execute_tool_calls(
+        tool_calls: list[ChatCompletionMessageToolCall], openai_functions
+) -> list[ToolCallOutcome]:
+    outcomes = []
+    for tool_call in tool_calls:
+        function_name = tool_call.function.name
+
+        if function_name not in openai_functions:
+            e = ToolCallError(f"Error: function `{function_name}` does not exist.")
+
+            outcomes.append(
+                ToolCallOutcome(
+                    success=False,
+                    tool_call_id=tool_call.id,
+                    raw_tool_call=tool_call,
+                    result=e,
+                    tool_name=None
+                )
+            )
+            continue
+
+        openai_function = openai_functions[function_name]
+        try:
+            arguments = json.loads(tool_call.function.arguments)
+        except json.JSONDecodeError as e:
+            outcomes.append(
+                ToolCallOutcome(
+                    success=False,
+                    tool_call_id=tool_call.id,
+                    raw_tool_call=tool_call,
+                    result=e,
+                    tool_name=function_name
+                )
+            )
+            continue
+
+        try:
+            result_instance = await openai_function.callback(**arguments)
+            outcomes.append(
+                ToolCallOutcome(
+                    success=True,
+                    tool_call_id=tool_call.id,
+                    raw_tool_call=tool_call,
+                    result=result_instance,
+                    tool_name=function_name
+                )
+            )
+        except InnerValidationError as e:
+            # There is not really a need for any custom handling vs. other exceptions here - we just raise.
+            # I am just making clear that *inner* validation errors will not lead to a retry,
+            # since the model did fine calling the tool here.
+            # To force a retry due to a semantic error the model should correct, raise a ToolCallError instead
+            raise e
+        except (ValidationError, ToolCallError) as e:
+            outcomes.append(
+                ToolCallOutcome(
+                    success=False,
+                    tool_call_id=tool_call.id,
+                    raw_tool_call=tool_call,
+                    result=e,
+                    tool_name=function_name
+                )
+            )
+    return outcomes
 
 
 async def maybe_shortcut_trivial_function_call(
         available_function_names: set[str], openai_functions: dict[str, OpenAIFunction]
 ) -> ChatCompletionMessage | None:
     last_message = None
     if len(available_function_names) == 1:
@@ -396,23 +512,21 @@
                     )
                 ]
             )
     return last_message
 
 
 def initialize_and_validate_message_history(
-        messages: Messages | None, system_prompt, user_message, distil_system_prompt
+        messages: Messages | None, system_prompt, user_message
 ) -> Messages:
     """
     Initialize and update the history in-place based on the supplied system prompt and user_message.
-    After this call, we guarantee that, if a distil_system_prompt was supplied, the first message in the history is a
-    system message (which will be replaced with the distillation prompt during history rewriting).
+    After this call, we guarantee that, if a system_prompt was supplied, the first message in the history is a
+    system message.
     """
-    messages = messages[:] if messages is not None else []
-
     if not (messages or system_prompt or user_message):
         raise ValueError(
             "No input - supply at least 'messages', 'system_prompt' and/or 'user_message'"
         )
 
     if system_prompt:
         if messages:
@@ -428,36 +542,37 @@
                 "Cowardly refusing to replace it / append another one."
             )
         messages.insert(0, ChatCompletionSystemMessageParam(role="system", content=system_prompt))
 
     if user_message:
         messages.append(ChatCompletionUserMessageParam(role="user", content=user_message))
 
-    if distil_system_prompt and messages[0]["role"] != "system":
-        raise ValueError(
-            "Cannot use 'distil_system_prompt' if the first message in the history is not a system message. "
-            "Either use the 'system_message' param or supply a history that starts with a system message."
-        )
-
     return messages
 
 
-def process_tool_definitions(tools_raw):
+@dataclasses.dataclass
+class ProcessedFunctions:
+    openai_functions: dict[str, OpenAIFunction]
+    abbreviated_openai_functions: dict[str, OpenAIFunction]
+
+
+def process_tool_definitions(tools_raw) -> ProcessedFunctions:
     openai_functions: dict[str, OpenAIFunction] = {}
     # Note: these are indexed by their original name
-    distillery_openai_functions: dict[str, OpenAIFunction] = {}
+    abbreviated_functions: dict[str, OpenAIFunction] = {}
     for model_or_fn in tools_raw:
         openai_function = create_openai_function(model_or_fn)
         openai_functions[openai_function.name] = openai_function
 
-        if openai_function.is_distillery:
-            distillery_openai_function = create_openai_function(model_or_fn.__functioncalming_distil_model__)
-            distillery_openai_functions[openai_function.name] = distillery_openai_function
+        abbreviated_function = create_abbreviated_openai_function(model_or_fn=model_or_fn)
+        abbreviated_functions[abbreviated_function.name] = abbreviated_function
 
-    return openai_functions, distillery_openai_functions
+    return ProcessedFunctions(
+        openai_functions=openai_functions, abbreviated_openai_functions=abbreviated_functions
+    )
 
 
 def get_tool_choice_for_default_behavior(
         openai_function_names: list[str] | set[str]
 ) -> ChatCompletionToolChoiceOptionParam:
     tool_choice: ChatCompletionToolChoiceOptionParam
     if not openai_function_names:
@@ -465,86 +580,30 @@
     elif len(openai_function_names) == 1:
         tool_choice = {"type": "function", "function": {"name": list(openai_function_names)[0]}}
     else:
         tool_choice = "auto"
     return tool_choice
 
 
-def adjust_distillery_call_for_clean_history(
-        *,
-        new_function_name: str,
-        serialized_result: str | None,
-        tool_call: ChatCompletionMessageToolCall,
-) -> tuple[ChatCompletionMessageToolCall, ChatCompletionToolMessageParam]:
-    adjusted_tool_call = ChatCompletionMessageToolCall(
-        id=tool_call.id,
-        type="function",
-        function=Function(
-            name=new_function_name,
-            arguments=serialized_result
-        )
-    )
-    adjusted_tool_response = ChatCompletionToolMessageParam(
-        role="tool",
-        tool_call_id=tool_call.id,
-        content='{"result": "success"}',
-    )
-    return adjusted_tool_call, adjusted_tool_response
-
-
 def rewrite_message_history(
         *,
         messages: Messages,
         rewrite_cutoff: int,
         successful_tool_calls: list[ChatCompletionMessageToolCall],
         successful_tool_responses: list[ChatCompletionToolMessageParam],
-        distil_system_prompt: str | None,
 ):
     """
     Rewrite the history by removing all messages (not just the failed calls) and replacing them with a single clean
     multi call and its responses, starting from the cutoff index.
     """
-    unaltered_first_message = None
     omitted_messages = messages[rewrite_cutoff:]
     if successful_tool_calls:
-        if distil_system_prompt is not None:
-            unaltered_first_message = messages[0]
-            assert unaltered_first_message["role"] == "system", "First message must be a system message when using 'distil_system_prompt'"
-            messages[0] = {
-                **messages[0],
-                "content": distil_system_prompt
-            }
-
         messages[rewrite_cutoff:] = [
             {
                 "role": "assistant",
                 "tool_calls": [tc.model_dump() for tc in successful_tool_calls],
                 "content": None,
             },
             *successful_tool_responses
         ]
-    return unaltered_first_message, omitted_messages
-
+    return omitted_messages
 
-
-def log_finetuning_data(
-        destination: str | TextIO,
-        messages: Messages,
-        functions: list[OpenAIFunction],
-        extra_data: dict | None = None
-):
-    if extra_data is not None and "messages" in extra_data:
-        logging.warning("'messages' key is being overwritten by extra data!")
-
-    if extra_data is not None and "functions" in extra_data:
-        logging.warning("'functions' key is being overwritten by extra data!")
-
-    fd = FineTuningData(
-        **{**dict(messages=messages, functions=[t.definition for t in functions]), **(extra_data or {})}
-    )
-
-    log_entry = f"{fd.model_dump_json()}\n"
-    if isinstance(destination, str):
-        with open(destination, "a") as outf:
-            outf.write(log_entry)
-    else:
-        destination.write(log_entry)
```

### Comparing `functioncalming-0.0.7/functioncalming/utils.py` & `functioncalming-0.0.8/functioncalming/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import logging
 
 import functools
 import inspect
 import json
 from inspect import Parameter
 from types import MappingProxyType
-from typing import Callable, Awaitable
+from typing import Callable, Awaitable, TextIO
 
 from docstring_parser import parse, Docstring
 from openai.types.chat import ChatCompletionMessageParam, ChatCompletionToolParam, ChatCompletionMessage
 from openai.types.shared_params import FunctionDefinition
 from pydantic import BaseModel, RootModel, create_model, Field, ValidationError
+from pydantic.fields import FieldInfo
 
-type Messages = list[ChatCompletionMessageParam]
+from functioncalming.types import BaseModelOrJsonCompatible, Messages
 
 
 def pascal_to_snake(pascal_string):
     snake_list = [pascal_string[0].lower()]
 
     for char in pascal_string[1:]:
         if char.isupper():
@@ -35,78 +36,79 @@
         super().__init__(messages)
         self.original_error = original_error
 
 
 class ToolCallError(ValueError):
     pass
 
+
 @dataclasses.dataclass
 class OpenAIFunction:
     name: str
     definition: FunctionDefinition
     callback: Callable[[...], Awaitable[BaseModel]]
-    callback_expects_user_message: bool
     callback_expects_args_from_model: bool
-    is_distillery: bool
 
     @functools.cached_property
     def tool_definition(self) -> ChatCompletionToolParam:
         return ChatCompletionToolParam(type="function", function=self.definition)
 
 
 @functools.lru_cache()
 def create_openai_function(model_or_fn: BaseModel | Callable) -> OpenAIFunction:
     # double check: do we need to iterate through the whole schema to find references to plain name and replace them?
     # could see this being the case for recursive models
     name = pascal_to_snake(model_or_fn.__name__)
-    is_distillery = getattr(model_or_fn, "__is_functioncalming_distillery__", False)
     description = model_or_fn.__doc__
     if description is None:
         logging.warning(f"Tool {model_or_fn} does not have a docstring! Model may not know how to use it.")
         description = ""
 
     if isinstance(model_or_fn, type) and issubclass(model_or_fn, BaseModel):
         as_model = model_or_fn
 
         async def callback(*args, **kwargs):  # this is just to always make the callback awaitable
             return model_or_fn(*args, **kwargs)
 
     elif inspect.isfunction(model_or_fn):
-        description, param_descriptions = description_and_param_docs_from_docstring(description)
-        as_model = basemodel_from_function(model_or_fn, name, param_descriptions)
+        description, param_descriptions_from_docstring = description_and_param_docs_from_docstring(description)
+        as_model = basemodel_from_function(
+            model_or_fn, name, param_descriptions_from_docstring
+        )
         callback = create_callback_function_for_tool_use(model_or_fn, as_model)
     else:
         raise ValueError(f"Don't know how to turn {model_or_fn} into an OpenAI function")
 
     schema = as_model.model_json_schema()
 
-    # we want to hide this from the OpenAI model, but know whether we need to pass it back in later
-    expects_user_message = schema["properties"].pop("user_message", None) is not None
-    if expects_user_message and "user_message" in schema["required"]:
-        schema["required"].remove("user_message")
-
     expects_args_from_model = bool(schema["properties"])
 
     schema.pop("title", None)
     schema.pop("description", None)
 
     return OpenAIFunction(
         name=name,
         definition=FunctionDefinition(
             name=name,
             description=description.strip(),
             parameters=schema
         ),
         callback=callback,
-        callback_expects_user_message=expects_user_message,
-        callback_expects_args_from_model=expects_args_from_model,
-        is_distillery=is_distillery
+        callback_expects_args_from_model=expects_args_from_model
     )
 
 
+def create_abbreviated_openai_function(model_or_fn: Callable | BaseModel) -> OpenAIFunction:
+    async def stub() -> None:
+        pass
+    stub.__name__ = model_or_fn.__name__
+    stub.__doc__ = model_or_fn.__doc__
+    return create_openai_function(stub)
+
+
 def description_and_param_docs_from_docstring(function_docstring):
     param_descriptions = {}
     description = function_docstring
     if function_docstring is not None:
         docstring: Docstring = parse(function_docstring)
         description = docstring.long_description or docstring.short_description or function_docstring
         param_descriptions = {p.arg_name: p.description for p in docstring.params}
@@ -133,60 +135,84 @@
                 original_error=e
             ) from e
         return res
 
     return callback
 
 
-def basemodel_from_function(model_or_fn, name, param_descriptions) -> type[BaseModel]:
+# def compile_param_description(annotation, default, description_from_docstring):
+#     if description_from_docstring:
+#         return description_from_docstring
+#     if isinstance(default, FieldInfo) and default.description:
+#         return default.description
+
+
+def basemodel_from_function(model_or_fn, name, param_descriptions_from_docstring) -> type[BaseModel]:
     # TypeAdapter(model_or_fn) might be suitable too - unfortunately it doesn't care about docstrings
     params: MappingProxyType[str, Parameter] = inspect.signature(model_or_fn).parameters
     as_model = create_model(
         name,
         **{
             name: (
                 param.annotation,
                 Field(
                     default=(... if param.default is Parameter.empty else param.default),
-                    description=param_descriptions.get(name)
+                    description=param_descriptions_from_docstring.get(name)
                 )
             )
             for name, param
             in params.items()
         }
     )
     return as_model
 
 
+def serialize_openai_function_result(result: BaseModelOrJsonCompatible):
+    if isinstance(result, (BaseModel, RootModel)):
+        return result.model_dump_json()
+    return json.dumps(result)
+
+
 async def invoke_callback_function(
         openai_function: OpenAIFunction,
         kwargs: dict,
-        history: Messages,
-        serialize_result_for_model: bool
-) -> tuple[BaseModel, str, str | None]:
-    if openai_function.callback_expects_user_message:
-        last_user_message = ([m["content"] for m in history if m["role"] == "user"] or [None])[-1]
-        if last_user_message is None:
-            raise ValueError("No user message to supply to callback function!")
-        kwargs = {**kwargs, "user_message": last_user_message}
-
+) -> tuple[BaseModel, str]:
     result = await openai_function.callback(**kwargs)
 
-    result_for_model = "{'result': 'success'}"
-    serialized = None
-    if serialize_result_for_model or openai_function.is_distillery:
-        if isinstance(result, (BaseModel, RootModel)):
-            serialized = result.model_dump_json()
-        else:
-            serialized = json.dumps(result)
-
-    if serialize_result_for_model:
-        result_for_model = serialized
+    if isinstance(result, (BaseModel, RootModel)):
+        serialized = result.model_dump_json()
+    else:
+        serialized = json.dumps(result)
 
-    return result, result_for_model, serialized
+    return result, serialized
 
 
 class FineTuningData(BaseModel, extra="allow"):
     messages: Messages
     # todo: update this to Tool as soon as finetuning does not require legacy format anymore
     #  https://platform.openai.com/docs/guides/fine-tuning/fine-tuning-examples
     functions: list[FunctionDefinition]
+
+
+
+def log_finetuning_data(
+        destination: str | TextIO,
+        messages: Messages,
+        functions: list[OpenAIFunction],
+        extra_data: dict | None = None
+):
+    if extra_data is not None and "messages" in extra_data:
+        logging.warning("'messages' key is being overwritten by extra data!")
+
+    if extra_data is not None and "functions" in extra_data:
+        logging.warning("'functions' key is being overwritten by extra data!")
+
+    fd = FineTuningData(
+        **{**dict(messages=messages, functions=[t.definition for t in functions]), **(extra_data or {})}
+    )
+
+    log_entry = f"{fd.model_dump_json()}\n"
+    if isinstance(destination, str):
+        with open(destination, "a") as outf:
+            outf.write(log_entry)
+    else:
+        destination.write(log_entry)
```

### Comparing `functioncalming-0.0.7/pyproject.toml` & `functioncalming-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "functioncalming"
-version = "0.0.7"
+version = "0.0.8"
 description = "Robust and reliable OpenAI function calling"
 authors = ["Philipp Dowling <phdowling@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/phdowling/functioncalming"
 repository = "https://github.com/phdowling/functioncalming"
 keywords = ["openai", "function-calling", "distillation", "fine-tuning", "pydantic", "validation", "llm"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 openai = "^1.3.7"
 pydantic = "^2.5.2"
-docstring-parser = "^0.15"
+docstring-parser = "^0.16"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
 python-dotenv = "^1.0.0"
```

### Comparing `functioncalming-0.0.7/PKG-INFO` & `functioncalming-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: functioncalming
-Version: 0.0.7
+Version: 0.0.8
 Summary: Robust and reliable OpenAI function calling
 Home-page: https://github.com/phdowling/functioncalming
 License: MIT
 Keywords: openai,function-calling,distillation,fine-tuning,pydantic,validation,llm
 Author: Philipp Dowling
 Author-email: phdowling@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: docstring-parser (>=0.16,<0.17)
 Requires-Dist: openai (>=1.3.7,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Project-URL: Repository, https://github.com/phdowling/functioncalming
 Description-Content-Type: text/markdown
 
 # functioncalming
 Get (near-)guaranteed structured responses from OpenAI using pydantic and function calling (and, if you like, fine-tuning).
```

