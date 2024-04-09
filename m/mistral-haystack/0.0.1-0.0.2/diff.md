# Comparing `tmp/mistral_haystack-0.0.1.tar.gz` & `tmp/mistral_haystack-0.0.2.tar.gz`

## Comparing `mistral_haystack-0.0.1.tar` & `mistral_haystack-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/examples/indexing_pipeline.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/examples/streaming_chat_with_rag.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/pydoc/config.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/embedders/mistral/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/embedders/mistral/document_embedder.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/embedders/mistral/text_embedder.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/generators/mistral/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/generators/mistral/chat/__init__.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/src/haystack_integrations/components/generators/mistral/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/tests/test_mistral_chat_generator.py
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/tests/test_mistral_document_embedder.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/tests/test_mistral_text_embedder.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/README.md
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 mistral_haystack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/examples/indexing_pipeline.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/examples/streaming_chat_with_rag.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/pydoc/config.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/embedders/mistral/__init__.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/embedders/mistral/document_embedder.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/embedders/mistral/text_embedder.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/generators/mistral/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/generators/mistral/chat/__init__.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/src/haystack_integrations/components/generators/mistral/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/tests/test_mistral_chat_generator.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/tests/test_mistral_document_embedder.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/tests/test_mistral_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/README.md
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 mistral_haystack-0.0.2/PKG-INFO
```

### Comparing `mistral_haystack-0.0.1/examples/indexing_pipeline.py` & `mistral_haystack-0.0.2/examples/indexing_pipeline.py`

 * *Files identical despite different names*

### Comparing `mistral_haystack-0.0.1/examples/streaming_chat_with_rag.py` & `mistral_haystack-0.0.2/examples/streaming_chat_with_rag.py`

 * *Files identical despite different names*

### Comparing `mistral_haystack-0.0.1/pydoc/config.yml` & `mistral_haystack-0.0.2/pydoc/config.yml`

 * *Files 20% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
   type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
   excerpt: Mistral integration for Haystack
-  category_slug: haystack-integrations
+  category_slug: integrations-api
   title: Mistral
   slug: integrations-mistral
-  order: 40
+  order: 150
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_mistral.md
```

### Comparing `mistral_haystack-0.0.1/src/haystack_integrations/components/embedders/mistral/document_embedder.py` & `mistral_haystack-0.0.2/src/haystack_integrations/components/embedders/mistral/document_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,35 @@
         suffix: str = "",
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
-        Create a MistralDocumentEmbedder component.
-        :param api_key: The Mistral API key.
-        :param model: The name of the model to use.
-        :param api_base_url: The Mistral API Base url, defaults to None. For more details, see Mistral [docs](https://docs.mistral.ai/api/).
-        :param prefix: A string to add to the beginning of each text.
-        :param suffix: A string to add to the end of each text.
-        :param batch_size: Number of Documents to encode at once.
-        :param progress_bar: Whether to show a progress bar or not. Can be helpful to disable in production deployments
-                             to keep the logs clean.
-        :param meta_fields_to_embed: List of meta fields that should be embedded along with the Document text.
-        :param embedding_separator: Separator used to concatenate the meta fields to the Document text.
+        Creates a MistralDocumentEmbedder component.
+
+        :param api_key:
+            The Mistral API key.
+        :param model:
+            The name of the model to use.
+        :param api_base_url:
+            The Mistral API Base url. For more details, see Mistral [docs](https://docs.mistral.ai/api/).
+        :param prefix:
+            A string to add to the beginning of each text.
+        :param suffix:
+            A string to add to the end of each text.
+        :param batch_size:
+            Number of Documents to encode at once.
+        :param progress_bar:
+            Whether to show a progress bar or not. Can be helpful to disable in production deployments to keep
+            the logs clean.
+        :param meta_fields_to_embed:
+            List of meta fields that should be embedded along with the Document text.
+        :param embedding_separator:
+            Separator used to concatenate the meta fields to the Document text.
         """
         super(MistralDocumentEmbedder, self).__init__(  # noqa: UP008
             api_key=api_key,
             model=model,
             dimensions=None,
             api_base_url=api_base_url,
             organization=None,
```

### Comparing `mistral_haystack-0.0.1/src/haystack_integrations/components/embedders/mistral/text_embedder.py` & `mistral_haystack-0.0.2/src/haystack_integrations/components/embedders/mistral/text_embedder.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,49 +7,53 @@
 from haystack.components.embedders import OpenAITextEmbedder
 from haystack.utils.auth import Secret
 
 
 @component
 class MistralTextEmbedder(OpenAITextEmbedder):
     """
-     A component for embedding strings using Mistral models.
+    A component for embedding strings using Mistral models.
 
-     Usage example:
+    Usage example:
      ```python
     from haystack_integrations.components.embedders.mistral.text_embedder import MistralTextEmbedder
 
-     text_to_embed = "I love pizza!"
-
-     text_embedder = MistralTextEmbedder()
-
-     print(text_embedder.run(text_to_embed))
-
-     # {'embedding': [0.017020374536514282, -0.023255806416273117, ...],
-     # 'meta': {'model': 'text-embedding-ada-002-v2',
-     #          'usage': {'prompt_tokens': 4, 'total_tokens': 4}}}
-     ```
+    text_to_embed = "I love pizza!"
+    text_embedder = MistralTextEmbedder()
+    print(text_embedder.run(text_to_embed))
+
+    # output:
+    # {'embedding': [0.017020374536514282, -0.023255806416273117, ...],
+    # 'meta': {'model': 'mistral-embed',
+    #          'usage': {'prompt_tokens': 4, 'total_tokens': 4}}}
+    ```
     """
 
     def __init__(
         self,
         api_key: Secret = Secret.from_env_var("MISTRAL_API_KEY"),
         model: str = "mistral-embed",
         api_base_url: Optional[str] = "https://api.mistral.ai/v1",
         prefix: str = "",
         suffix: str = "",
     ):
         """
-        Create an MistralTextEmbedder component.
+        Creates an MistralTextEmbedder component.
 
-        :param api_key: The Misttal API key.
-        :param model: The name of the Mistral embedding models to be used.
-        :param api_base_url: The Mistral API Base url, defaults to `https://api.mistral.ai/v1`.
-                             For more details, see Mistral [docs](https://docs.mistral.ai/api/).
-        :param prefix: A string to add to the beginning of each text.
-        :param suffix: A string to add to the end of each text.
+        :param api_key:
+            The Mistral API key.
+        :param model:
+            The name of the Mistral embedding model to be used.
+        :param api_base_url:
+            The Mistral API Base url.
+            For more details, see Mistral [docs](https://docs.mistral.ai/api/).
+        :param prefix:
+            A string to add to the beginning of each text.
+        :param suffix:
+            A string to add to the end of each text.
         """
         super(MistralTextEmbedder, self).__init__(  # noqa: UP008
             api_key=api_key,
             model=model,
             dimensions=None,
             api_base_url=api_base_url,
             organization=None,
```

### Comparing `mistral_haystack-0.0.1/src/haystack_integrations/components/generators/mistral/chat/chat_generator.py` & `mistral_haystack-0.0.2/src/haystack_integrations/components/generators/mistral/chat/chat_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,35 @@
 from haystack.dataclasses import StreamingChunk
 from haystack.utils.auth import Secret
 
 
 @component
 class MistralChatGenerator(OpenAIChatGenerator):
     """
-    Enables text generation using Mistral's large language models (LLMs).
-    Currently supports `mistral-tiny`, `mistral-small` and `mistral-medium`
-    models accessed through the chat completions API endpoint.
+    Enables text generation using Mistral AI generative models.
+    For supported models, see [Mistral AI docs](https://docs.mistral.ai/platform/endpoints/#operation/listModels).
 
-    Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
-    directly to this component via the `**generation_kwargs` parameter in __init__ or the `**generation_kwargs`
+    Users can pass any text generation parameters valid for the Mistral Chat Completion API
+    directly to this component via the `generation_kwargs` parameter in `__init__` or the `generation_kwargs`
     parameter in `run` method.
 
+    Key Features and Compatibility:
+    - **Primary Compatibility**: Designed to work seamlessly with the Mistral API Chat Completion endpoint.
+    - **Streaming Support**: Supports streaming responses from the Mistral API Chat Completion endpoint.
+    - **Customizability**: Supports all parameters supported by the Mistral API Chat Completion endpoint.
+
+    This component uses the ChatMessage format for structuring both input and output,
+    ensuring coherent and contextually relevant responses in chat-based text generation scenarios.
+    Details on the ChatMessage format can be found in the
+    [Haystack docs](https://docs.haystack.deepset.ai/v2.0/docs/data-classes#chatmessage)
+
     For more details on the parameters supported by the Mistral API, refer to the
     [Mistral API Docs](https://docs.mistral.ai/api/).
 
+    Usage example:
     ```python
     from haystack_integrations.components.generators.mistral import MistralChatGenerator
     from haystack.dataclasses import ChatMessage
 
     messages = [ChatMessage.from_user("What's Natural Language Processing?")]
 
     client = MistralChatGenerator()
@@ -34,60 +44,51 @@
     print(response)
 
     >>{'replies': [ChatMessage(content='Natural Language Processing (NLP) is a branch of artificial intelligence
     >>that focuses on enabling computers to understand, interpret, and generate human language in a way that is
     >>meaningful and useful.', role=<ChatRole.ASSISTANT: 'assistant'>, name=None,
     >>meta={'model': 'mistral-tiny', 'index': 0, 'finish_reason': 'stop',
     >>'usage': {'prompt_tokens': 15, 'completion_tokens': 36, 'total_tokens': 51}})]}
-
     ```
-
-     Key Features and Compatibility:
-         - **Primary Compatibility**: Designed to work seamlessly with the Mistral API Chat Completion endpoint.
-         - **Streaming Support**: Supports streaming responses from the Mistral API Chat Completion endpoint.
-         - **Customizability**: Supports all parameters supported by the Mistral API Chat Completion endpoint.
-
-     Input and Output Format:
-         - **ChatMessage Format**: This component uses the ChatMessage format for structuring both input and output,
-           ensuring coherent and contextually relevant responses in chat-based text generation scenarios.
-           Details on the ChatMessage format can be found at: https://github.com/openai/openai-python/blob/main/chatml.md.
-           Note that the Mistral API does not accept `system` messages yet. You can use `user` and `assistant` messages.
     """
 
     def __init__(
         self,
         api_key: Secret = Secret.from_env_var("MISTRAL_API_KEY"),
         model: str = "mistral-tiny",
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         api_base_url: Optional[str] = "https://api.mistral.ai/v1",
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
         Creates an instance of MistralChatGenerator. Unless specified otherwise in the `model`, this is for Mistral's
         `mistral-tiny` model.
 
-        :param api_key: The Mistral API key.
-        :param model: The name of the Mistral chat completion model to use.
-        :param streaming_callback: A callback function that is called when a new token is received from the stream.
+        :param api_key:
+            The Mistral API key.
+        :param model:
+            The name of the Mistral chat completion model to use.
+        :param streaming_callback:
+            A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
-        :param api_base_url: The Mistral API Base url, defaults to `https://api.mistral.ai/v1`.
-                             For more details, see Mistral [docs](https://docs.mistral.ai/api/).
-        :param generation_kwargs: Other parameters to use for the model. These parameters are all sent directly to
-            the Mistrak endpoint. See [Mistral API docs](https://docs.mistral.ai/api/t) for
-            more details.
+        :param api_base_url:
+            The Mistral API Base url.
+            For more details, see Mistral [docs](https://docs.mistral.ai/api/).
+        :param generation_kwargs:
+            Other parameters to use for the model. These parameters are all sent directly to
+            the Mistral endpoint. See [Mistral API docs](https://docs.mistral.ai/api/) for more details.
             Some of the supported parameters:
             - `max_tokens`: The maximum number of tokens the output text can have.
             - `temperature`: What sampling temperature to use. Higher values mean the model will take more risks.
                 Try 0.9 for more creative applications and 0 (argmax sampling) for ones with a well-defined answer.
             - `top_p`: An alternative to sampling with temperature, called nucleus sampling, where the model
                 considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens
                 comprising the top 10% probability mass are considered.
             - `stream`: Whether to stream back partial progress. If set, tokens will be sent as data-only server-sent
                 events as they become available, with the stream terminated by a data: [DONE] message.
-            - `stop`: One or more sequences after which the LLM should stop generating tokens.
             - `safe_prompt`: Whether to inject a safety prompt before all conversations.
             - `random_seed`: The seed to use for random sampling.
         """
         super(MistralChatGenerator, self).__init__(  # noqa: UP008
             api_key=api_key,
             model=model,
             streaming_callback=streaming_callback,
```

### Comparing `mistral_haystack-0.0.1/tests/test_mistral_chat_generator.py` & `mistral_haystack-0.0.2/tests/test_mistral_chat_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,26 +143,28 @@
                 "streaming_callback": "haystack.components.generators.utils.print_streaming_chunk",
                 "generation_kwargs": {"max_tokens": 10, "some_test_param": "test-params"},
             },
         }
         with pytest.raises(ValueError, match="None of the .* environment variables are set"):
             MistralChatGenerator.from_dict(data)
 
-    def test_run(self, chat_messages):
+    def test_run(self, chat_messages, mock_chat_completion, monkeypatch):  # noqa: ARG002
+        monkeypatch.setenv("MISTRAL_API_KEY", "fake-api-key")
         component = MistralChatGenerator()
         response = component.run(chat_messages)
 
         # check that the component returns the correct ChatMessage response
         assert isinstance(response, dict)
         assert "replies" in response
         assert isinstance(response["replies"], list)
         assert len(response["replies"]) == 1
         assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
 
-    def test_run_with_params(self, chat_messages, mock_chat_completion):
+    def test_run_with_params(self, chat_messages, mock_chat_completion, monkeypatch):
+        monkeypatch.setenv("MISTRAL_API_KEY", "fake-api-key")
         component = MistralChatGenerator(generation_kwargs={"max_tokens": 10, "temperature": 0.5})
         response = component.run(chat_messages)
 
         # check that the component calls the OpenAI API with the correct parameters
         _, kwargs = mock_chat_completion.call_args
         assert kwargs["max_tokens"] == 10
         assert kwargs["temperature"] == 0.5
@@ -170,35 +172,14 @@
         # check that the component returns the correct response
         assert isinstance(response, dict)
         assert "replies" in response
         assert isinstance(response["replies"], list)
         assert len(response["replies"]) == 1
         assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
 
-    def test_run_with_params_streaming(self, chat_messages):
-        streaming_callback_called = False
-
-        def streaming_callback(chunk: StreamingChunk) -> None:  # noqa: ARG001
-            nonlocal streaming_callback_called
-            streaming_callback_called = True
-
-        component = MistralChatGenerator(streaming_callback=streaming_callback)
-        response = component.run(chat_messages)
-
-        # check we called the streaming callback
-        assert streaming_callback_called
-
-        # check that the component still returns the correct response
-        assert isinstance(response, dict)
-        assert "replies" in response
-        assert isinstance(response["replies"], list)
-        assert len(response["replies"]) == 1
-        assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
-        assert "Paris" in response["replies"][0].content  # see mock_chat_completion_chunk
-
     def test_check_abnormal_completions(self, caplog):
         component = MistralChatGenerator(api_key=Secret.from_token("test-api-key"))
         messages = [
             ChatMessage.from_assistant(
                 "", meta={"finish_reason": "content_filter" if i % 2 == 0 else "length", "index": i}
             )
             for i, _ in enumerate(range(4))
```

### Comparing `mistral_haystack-0.0.1/tests/test_mistral_document_embedder.py` & `mistral_haystack-0.0.2/tests/test_mistral_document_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from haystack.utils import Secret
 from haystack_integrations.components.embedders.mistral.document_embedder import MistralDocumentEmbedder
 
 pytestmark = pytest.mark.embedders
 
 
 class TestMistralDocumentEmbedder:
-    def test_init_default(self):
+    def test_init_default(self, monkeypatch):
+        monkeypatch.setenv("MISTRAL_API_KEY", "test-api-key")
+
         embedder = MistralDocumentEmbedder()
         assert embedder.api_key == Secret.from_env_var(["MISTRAL_API_KEY"])
         assert embedder.model == "mistral-embed"
         assert embedder.api_base_url == "https://api.mistral.ai/v1"
         assert embedder.prefix == ""
         assert embedder.suffix == ""
         assert embedder.batch_size == 32
@@ -42,15 +44,17 @@
         assert embedder.prefix == "START"
         assert embedder.suffix == "END"
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == "-"
 
-    def test_to_dict(self):
+    def test_to_dict(self, monkeypatch):
+        monkeypatch.setenv("MISTRAL_API_KEY", "test-api-key")
+
         embedder_component = MistralDocumentEmbedder()
         component_dict = embedder_component.to_dict()
         assert component_dict == {
             "type": "haystack_integrations.components.embedders.mistral.document_embedder.MistralDocumentEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["MISTRAL_API_KEY"], "strict": True, "type": "env_var"},
                 "model": "mistral-embed",
@@ -95,15 +99,15 @@
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": "-",
             },
         }
 
     @pytest.mark.skipif(
         not os.environ.get("MISTRAL_API_KEY", None),
-        reason="Export an env var called MISTRAL_API_KEY containing the Cohere API key to run this test.",
+        reason="Export an env var called MISTRAL_API_KEY containing the Mistral API key to run this test.",
     )
     @pytest.mark.integration
     def test_run(self):
         embedder = MistralDocumentEmbedder()
 
         docs = [
             Document(content="I love cheese", meta={"topic": "Cuisine"}),
```

### Comparing `mistral_haystack-0.0.1/tests/test_mistral_text_embedder.py` & `mistral_haystack-0.0.2/tests/test_mistral_text_embedder.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,41 +7,48 @@
 from haystack.utils import Secret
 from haystack_integrations.components.embedders.mistral.text_embedder import MistralTextEmbedder
 
 pytestmark = pytest.mark.embedders
 
 
 class TestMistralTextEmbedder:
-    def test_init_default(self):
+    def test_init_default(self, monkeypatch):
+        monkeypatch.setenv("MISTRAL_API_KEY", "test-api-key")
+
         embedder = MistralTextEmbedder()
         assert embedder.api_key == Secret.from_env_var(["MISTRAL_API_KEY"])
+        assert embedder.api_base_url == "https://api.mistral.ai/v1"
         assert embedder.model == "mistral-embed"
         assert embedder.prefix == ""
         assert embedder.suffix == ""
 
     def test_init_with_parameters(self):
         embedder = MistralTextEmbedder(
             api_key=Secret.from_token("test-api-key"),
             model="mistral-embed-v2",
             prefix="START",
             suffix="END",
         )
         assert embedder.api_key == Secret.from_token("test-api-key")
+        assert embedder.api_base_url == "https://api.mistral.ai/v1"
         assert embedder.model == "mistral-embed-v2"
         assert embedder.prefix == "START"
         assert embedder.suffix == "END"
 
-    def test_to_dict(self):
+    def test_to_dict(self, monkeypatch):
+        monkeypatch.setenv("MISTRAL_API_KEY", "test-api-key")
+
         embedder_component = MistralTextEmbedder()
         component_dict = embedder_component.to_dict()
         assert component_dict == {
             "type": "haystack_integrations.components.embedders.mistral.text_embedder.MistralTextEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["MISTRAL_API_KEY"], "strict": True, "type": "env_var"},
                 "model": "mistral-embed",
+                "api_base_url": "https://api.mistral.ai/v1",
                 "dimensions": None,
                 "organization": None,
                 "prefix": "",
                 "suffix": "",
             },
         }
 
@@ -56,24 +63,25 @@
         )
         component_dict = embedder.to_dict()
         assert component_dict == {
             "type": "haystack_integrations.components.embedders.mistral.text_embedder.MistralTextEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["ENV_VAR"], "strict": False, "type": "env_var"},
                 "model": "mistral-embed-v2",
+                "api_base_url": "https://custom-api-base-url.com",
                 "dimensions": None,
                 "organization": None,
                 "prefix": "START",
                 "suffix": "END",
             },
         }
 
     @pytest.mark.skipif(
         not os.environ.get("MISTRAL_API_KEY", None),
-        reason="Export an env var called MISTRAL_API_KEY containing the Cohere API key to run this test.",
+        reason="Export an env var called MISTRAL_API_KEY containing the Mistral API key to run this test.",
     )
     @pytest.mark.integration
     def test_run(self):
         embedder = MistralTextEmbedder()
         text = "The food was delicious"
         result = embedder.run(text)
         assert all(isinstance(x, float) for x in result["embedding"])
```

### Comparing `mistral_haystack-0.0.1/.gitignore` & `mistral_haystack-0.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 .pyre/
 
 # IDEs
 .vscode
 
 # Docs generation artifacts
 _readme_*.md
+.idea
```

### Comparing `mistral_haystack-0.0.1/LICENSE.txt` & `mistral_haystack-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mistral_haystack-0.0.1/README.md` & `mistral_haystack-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mistral_haystack-0.0.1/pyproject.toml` & `mistral_haystack-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["haystack-ai>=2.0.0b6"]
+dependencies = ["haystack-ai"]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/mistral#readme"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/mistral"
 
 [tool.hatch.build.targets.wheel]
@@ -57,20 +57,20 @@
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive --explicit-package-bases {args:src/ tests}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
 all = ["style", "typing"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -123,27 +123,28 @@
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
-[tool.coverage.paths]
-mistral_haystack = [
-  "src/haystack_integrations",
-  "*/mistral/src/haystack_integrations",
-]
-tests = ["tests", "*/mistral/tests"]
 
 [tool.coverage.report]
-exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
 
 [[tool.mypy.overrides]]
 module = [
   "mistral.*",
   "haystack.*",
   "haystack_integrations.*",
   "openai.*",
```

### Comparing `mistral_haystack-0.0.1/PKG-INFO` & `mistral_haystack-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mistral-haystack
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/mistral#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/mistral
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: haystack-ai>=2.0.0b6
+Requires-Dist: haystack-ai
 Description-Content-Type: text/markdown
 
 # mistral-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mistral-haystack.svg)](https://pypi.org/project/mistral-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mistral-haystack.svg)](https://pypi.org/project/mistral-haystack)
```

