# Comparing `tmp/llm_optimized_inference-0.1.1-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,35 +1,37 @@
-Zip file size: 52688 bytes, number of entries: 33
--rw-rw-r--  2.0 unx      249 b- defN 24-Mar-14 22:06 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Mar-14 22:06 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-Mar-14 22:06 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx       18 b- defN 24-Mar-14 22:09 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    32346 b- defN 24-Mar-14 22:06 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3119 b- defN 24-Mar-14 22:06 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     1153 b- defN 24-Mar-14 22:06 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-Mar-14 22:06 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5011 b- defN 24-Mar-14 22:06 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-Mar-14 22:06 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     7102 b- defN 24-Mar-14 22:06 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1332 b- defN 24-Mar-14 22:06 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     1111 b- defN 24-Mar-14 22:06 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    11422 b- defN 24-Mar-14 22:06 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    22716 b- defN 24-Mar-14 22:06 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     3708 b- defN 24-Mar-14 22:06 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-14 22:06 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     1878 b- defN 24-Mar-14 22:06 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-Mar-14 22:06 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2090 b- defN 24-Mar-14 22:06 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     5498 b- defN 24-Mar-14 22:06 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-Mar-14 22:06 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-Mar-14 22:06 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx     6307 b- defN 24-Mar-14 22:06 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx    10555 b- defN 24-Mar-14 22:06 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-Mar-14 22:06 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    13854 b- defN 24-Mar-14 22:06 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx     1927 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx     1694 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/metadata.json
--rw-rw-r--  2.0 unx        4 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx     3847 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx     3341 b- defN 24-Mar-14 22:09 llm_optimized_inference-0.1.1.dist-info/RECORD
-33 files, 154653 bytes uncompressed, 47174 bytes compressed:  69.5%
+Zip file size: 64182 bytes, number of entries: 35
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-09 00:35 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-09 00:35 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-Apr-09 00:35 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-Apr-09 00:35 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28124 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-09 00:35 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     5210 b- defN 24-Apr-09 00:35 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-09 00:35 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-09 00:35 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-Apr-09 00:35 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-09 00:35 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-09 00:35 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6935 b- defN 24-Apr-09 00:35 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-09 00:35 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-09 00:35 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-09 00:35 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-09 00:35 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8520 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10755 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    13820 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3056 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3489 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/RECORD
+35 files, 208031 bytes uncompressed, 58380 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -30,14 +30,17 @@
 
 Filename: llm/optimized/inference/managed_inference.py
 Comment: 
 
 Filename: llm/optimized/inference/model_config_factory.py
 Comment: 
 
+Filename: llm/optimized/inference/model_utils.py
+Comment: 
+
 Filename: llm/optimized/inference/prompt_formatter.py
 Comment: 
 
 Filename: llm/optimized/inference/replica_manager.py
 Comment: 
 
 Filename: llm/optimized/inference/score.py
@@ -63,38 +66,41 @@
 
 Filename: llm/optimized/inference/custom_model_configurations/schema_output.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/__init__.py
 Comment: 
 
+Filename: llm/optimized/inference/engine/_hf_predictors.py
+Comment: 
+
 Filename: llm/optimized/inference/engine/engine.py
 Comment: 
 
+Filename: llm/optimized/inference/engine/hf_engine.py
+Comment: 
+
 Filename: llm/optimized/inference/engine/mii_engine.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.1.dist-info/DESCRIPTION.rst
-Comment: 
-
-Filename: llm_optimized_inference-0.1.1.dist-info/metadata.json
+Filename: llm_optimized_inference-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.1.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.1.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.1.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.1.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1 +1,5 @@
-VERSION = "0.1.1"
+# ---------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# ---------------------------------------------------------
+
+VERSION = "0.1.2"
```

## llm/optimized/inference/api_server.py

```diff
@@ -14,25 +14,26 @@
 import yaml
 import shutil
 from azure.ai.contentsafety import ContentSafetyClient
 from azure.ai.contentsafety.models import AnalyzeTextOptions, AnalyzeImageOptions, ImageData
 from azure.core.credentials import AzureKeyCredential
 from azure.core.pipeline.policies import HeadersPolicy
 from azureml.ai.monitoring import Collector
-from llm.optimized.inference.constants import EngineName, ServerSetupParams, SupportedTask, TaskType
+from llm.optimized.inference.constants import EngineName, ServerSetupParams, SupportedTask, TaskType, ALL_TASKS
 from llm.optimized.inference.model_config_factory import ModelConfigFactory
 from llm.optimized.inference.fm_score import FMScore
 from llm.optimized.inference.logging_config import configure_logger
 from llm.optimized.inference.managed_inference import MIRPayload
 from mlflow.pyfunc.scoring_server import _get_jsonable_obj
 from llm.optimized.inference.utils import box_logger, map_env_vars_to_vllm_server_args
 from llm.optimized.inference.configs import EngineConfig, TaskConfig
 from transformers import AutoTokenizer
 from llm.optimized.inference.engine import InferenceResult
-import llm.optimized.inference.api_server_setup
+from llm.optimized.inference.model_utils import build_configs_from_model
+from llm.optimized.inference import api_server_setup
 
 # openai api imports
 import argparse
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse, Response, StreamingResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.openapi.utils import get_openapi
@@ -453,16 +454,15 @@
         )
     else:
         raw_prompt = data["messages"]
         messages = {'input_data': {'input_string': raw_prompt, 'parameters': parameters}}
     new_data.update(messages)
     request_id = f"cmpl-{random_uuid()}"
     created_time = int(time.monotonic())
-    
-    tokenizer = AutoTokenizer.from_pretrained(g_engine_config["model_id"])
+    tokenizer = AutoTokenizer.from_pretrained(g_engine_config["model_id"], trust_remote_code=True)
     num_prompt_tokens = len(tokenizer.apply_chat_template(raw_prompt, tokenize=True))
 
     inference_results = None
     try:
         inference_results, result_dict = await send_request(new_data)
     except:
         if inference_results is None:
@@ -538,15 +538,15 @@
             raw_prompt = [raw_prompt]
         messages = {'input_data': raw_prompt, 'params': parameters}
     new_data.update(messages)
     request_id = f"cmpl-{random_uuid()}"
     created_time = int(time.monotonic())
     
     num_prompt_tokens = 0
-    tokenizer = AutoTokenizer.from_pretrained(g_engine_config["model_id"])  
+    tokenizer = AutoTokenizer.from_pretrained(g_engine_config["model_id"], trust_remote_code=True)  
     for prompt in raw_prompt:
         num_prompt_tokens += len(tokenizer.encode(prompt))
 
     inference_results = None
     try:
         inference_results, result_dict = await send_request(new_data)
     except:
@@ -629,18 +629,18 @@
             inference_results = g_fmscorer.run(payload)
         
         if task_type == SupportedTask.CHAT_COMPLETION:
             outputs = {str(i): res.response for i, res in enumerate(inference_results)}
             results = {
                 "output": f"{outputs['0']}",
             }  # outputs will only have one key for chat-completion
-        elif task_type == SupportedTask.TEXT_TO_IMAGE:
+        elif task_type in [SupportedTask.TEXT_TO_IMAGE, SupportedTask.TEXT_TO_IMAGE_INPAINTING]:
             results = [dataclasses.asdict(res.response) for res in inference_results]
         else:
-            assert task_type == SupportedTask.TEXT_GENERATION and isinstance(
+            assert task_type in ALL_TASKS and isinstance(
                 payload.query,
                 list,
             ), "query should be a list for text-generation"
             # With models converted to transformers flavor from hftransformersv2 flavor, 
             # the output is a list of strings
             if payload.is_preview_format:
                 # TODO: Remove this once all models are updated to new format
@@ -714,122 +714,35 @@
                 os.getenv("AZUREML_MODEL_DIR", ""),
                 DEPRECATED_MLFLOW_MODEL_PATH,
             )
             tokenizer_path = model_path
 
         config_path = os.path.join(model_path, "config.json")
         
-        default_engine = EngineName.VLLM
-        tensor_parallel = os.getenv("TENSOR_PARALLEL", None)
-        if tensor_parallel:
-            tensor_parallel = int(tensor_parallel)
-        g_engine_config = {
-            "engine_name": os.getenv("ENGINE_NAME", default_engine),
-            "model_id": model_path,
-            "tokenizer": tokenizer_path,
-            "tensor_parallel": tensor_parallel,
-        }
 
         _init_cuda_visible_devices()
 
         abs_mlmodel_path = os.path.join(
             os.getenv("AZUREML_MODEL_DIR", ""),
             MLMODEL_PATH,
         )
         mlmodel = {}
         if abs_mlmodel_path and os.path.exists(abs_mlmodel_path):
             with open(abs_mlmodel_path) as f:
                 mlmodel = yaml.safe_load(f)
 
-        default_generator_configs = ""
-        task_config = None
         if mlmodel:
-            flavors = mlmodel.get("flavors", {})
             g_model_signature = mlmodel.get("signature", None)
-            if "transformers" in flavors:
-                # New MLModel format with transformers flavor
-                task_type = flavors["transformers"]["task"]
-
-                model_generator_configs = flavors["transformers"].get(
-                    "generator_config",
-                    {},
-                )
-                if task_type not in (
-                    SupportedTask.TEXT_GENERATION,
-                    SupportedTask.CHAT_COMPLETION,
-                ):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                # update default gen configs with model configs
-                default_generator_configs = get_generator_params(
-                    model_generator_configs,
-                )
-            elif "hftransformersv2" in flavors:
-                # Old MLModel format with hftransformersv2 flavor
-                # TODO: Remove this once all models are updated to new format
-                task_type = flavors["hftransformersv2"]["task_type"]
-                model_generator_configs = flavors["hftransformersv2"].get(
-                    "generator_config",
-                    {},
-                )
-
-                if task_type not in (
-                    SupportedTask.TEXT_GENERATION,
-                    SupportedTask.CHAT_COMPLETION,
-                ):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                # update default gen configs with model configs
-                default_generator_configs = get_generator_params(
-                    model_generator_configs,
-                )
-            elif "python_function" in flavors:
-
-                task_type = mlmodel["metadata"]["base_model_task"]
-                if task_type not in (TaskType.TEXT_TO_IMAGE):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                model_type = mlmodel["metadata"].get("model_type", "")
-                
-                model_config_builder = ModelConfigFactory.get_config_builder(task=task_type, model_type=model_type)
-                g_engine_config.update(
-                                        {
-                                            "engine_name": model_config_builder.engine,
-                                            "mii_config": model_config_builder.get_optimization_config(),
-                                            "custom_model_config_builder": model_config_builder,
-                                            "model_id": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), model_config_builder.MLFLOW_MODEL_PATH),
-                                            "tokenizer": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), model_config_builder.MLFLOW_MODEL_PATH, "tokenizer"),
-                                            "tensor_parallel": model_config_builder.tensor_parallel
-                                        }
-                                    )
-                task_config = model_config_builder.get_task_config()
-
-        if g_engine_config["engine_name"] in [EngineName.MII, EngineName.MII_V1] and "mii_config" not in g_engine_config:
-            mii_engine_config = {
-                "deployment_name": os.getenv("DEPLOYMENT_NAME", "llama-deployment"),
-                "mii_configs": {},
-            }
-
-            g_engine_config["mii_config"] = mii_engine_config
-
-        if g_engine_config["engine_name"] == EngineName.VLLM:
-            model_config = {}
-            vllm_config = map_env_vars_to_vllm_server_args()
-            if config_path and os.path.exists(config_path):
-                with open(config_path) as config_content:
-                    model_config = json.load(config_content)
-            g_engine_config["vllm_config"] = vllm_config
-            g_engine_config["model_config"] = model_config
-
-        task_config = {
-            "task_type": TaskType.CONVERSATIONAL
-            if task_type == SupportedTask.CHAT_COMPLETION
-            else TaskType.TEXT_GENERATION,
-        } if task_config is None else task_config
-
+            g_engine_config, task_config, default_generator_configs, task_type = build_configs_from_model(
+                mlmodel,
+                model_path,
+                config_path,
+                tokenizer_path
+            )
+        
         config = {
             "engine": g_engine_config,
             "task": task_config,
         }
 
         g_fmscorer = FMScore(config)
         g_fmscorer.init()
```

## llm/optimized/inference/configs.py

```diff
@@ -57,14 +57,16 @@
     port: int = DEFAULT_PORT
     tensor_parallel: Optional[int] = None
     trust_remote_code: bool = True
     mii_config: Optional[MiiEngineConfig] = None
     vllm_config: Optional[Dict] = None
     model_config: Optional[Dict] = None
     custom_model_config_builder: Optional[ModelConfigurationBuilder] = None
+    hf_config_path: Optional[str] = None
+    ml_model_info: Optional[Dict] = None
 
     @classmethod
     def from_dict(cls: Type[TypeVar("T")], d: Dict) -> TypeVar("T"):
         """Create a configuration from a dictionary."""
         if "mii_config" in d and isinstance(d["mii_config"], dict):
             d["mii_config"] = MiiEngineConfig.from_dict(d["mii_config"])
         return super().from_dict(d)
```

## llm/optimized/inference/constants.py

```diff
@@ -19,26 +19,158 @@
 
 class TaskType(str, Enum):
     """Enum representing the types of tasks."""
 
     TEXT_GENERATION = "text-generation"
     CONVERSATIONAL = "conversational"
     TEXT_TO_IMAGE = "text-to-image"
+    TEXT_CLASSIFICATION = "text-classification"
+    TEXT_CLASSIFICATION_MULTILABEL = "text-classification-multilabel"
+    NER = "text-named-entity-recognition"
+    SUMMARIZATION = "text-summarization"
+    QnA = "question-answering"
+    TRANSLATION = "text-translation"
+    TEXT_GENERATION_CODE = "text-generation-code"
+    FILL_MASK = "fill-mask"
+    CHAT_COMPLETION = "chat-completion"
+    TEXT_TO_IMAGE_INPAINTING = "text-to-image-inpainting"
 
     def __str__(self):
         """Return the string representation of the task type."""
         return self.value
 
 
 class SupportedTask:
     """Supported tasks by text-generation-inference."""
 
     TEXT_GENERATION = "text-generation"
     CHAT_COMPLETION = "chat-completion"
     TEXT_TO_IMAGE = "text-to-image"
+    TEXT_CLASSIFICATION = "text-classification"
+    TEXT_CLASSIFICATION_MULTILABEL = "text-classification-multilabel"
+    NER = "token-classification"
+    SUMMARIZATION = "summarization"
+    QnA = "question-answering"
+    TRANSLATION = "translation"
+    TEXT_GENERATION_CODE = "text-generation-code"
+    FILL_MASK = "fill-mask"
+    TEXT_TO_IMAGE_INPAINTING = "text-to-image-inpainting"
 
 
 class ServerSetupParams:
     """Parameters for setting up the server."""
 
     WAIT_TIME_MIN = 15  # time to wait for the server to become healthy
     DEFAULT_WORKER_COUNT = 1
+
+
+class VLLMSupportedModels:
+    """VLLM Supported Models List."""
+
+    Models = {
+        "AquilaForCausalLM",
+        "BaiChuanForCausalLM",
+        "BloomForCausalLM",
+        "ChatGLMModel",
+        "DeciLMForCausalLM",
+        "FalconForCausalLM",
+        "GemmaForCausalLM",
+        "GPT2LMHeadModel",
+        "GPTBigCodeForCausalLM",
+        "GPTJForCausalLM",
+        "GPTNeoXForCausalLM",
+        "InternLMForCausalLM",
+        "InternLM2ForCausalLM",
+        "LlamaForCausalLM",
+        "MistralForCausalLM",
+        "MixtralForCausalLM",
+        "MPTForCausalLM",
+        "OLMoForCausalLM",
+        "OPTForCausalLM",
+        "OrionForCausalLM",
+        "QWenLMHeadModel",
+        "Qwen2ForCausalLM",
+        "RWForCausalLM",
+        "StableLmForCausalLM",
+        "DbrxForCausalLM"
+    }
+
+
+class MIISupportedModels:
+    """MII Supported Models."""
+
+    # TODO: Add more models from different tasks
+
+    Models = {
+        "BloomForCausalLM",
+        "GPT2LMHeadModel",
+        "GPTBigCodeForCausalLM",
+        "GPTJForCausalLM",
+        "GPTNeoXForCausalLM",
+        "LlamaForCausalLM",
+        "OPTForCausalLM",
+        "FalconForCausalLM",
+        "MistralForCausalLM",
+        "MixtralForCausalLM",
+        "PhiForCausalLM",
+        "QWenLMHeadModel"
+    }
+
+
+class VLLMSpecialModels:
+    """Models Types that require additional parameters to work with vllm."""
+
+    # TODO: Remove "RefinedWebModel" and "RefinedWeb" once falcon models are updated to latest huggingface commit
+
+    Models = {
+        "falcon": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
+        "RefinedWebModel": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
+        "RefinedWeb": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
+        "dbrx": {"args": ["trust-remote-code"]},
+        "deci_lm": {"args": ["trust-remote-code"]}
+    }
+
+    @classmethod
+    def get_kwargs(cls, model_type: str):
+        """Get the kwargs the vllm server needs for the model type."""
+        params = cls.Models.get(model_type, {})
+        return params.get("kwargs", {})
+
+    @classmethod
+    def get_args(cls, model_type: str):
+        """Get the args the vllm server needs for the model type."""
+        params = cls.Models.get(model_type, {})
+        return params.get("args", [])
+
+
+ALL_TASKS = [
+    SupportedTask.TEXT_TO_IMAGE,
+    SupportedTask.TEXT_CLASSIFICATION,
+    SupportedTask.TEXT_CLASSIFICATION_MULTILABEL,
+    SupportedTask.NER,
+    SupportedTask.SUMMARIZATION,
+    SupportedTask.QnA,
+    SupportedTask.TRANSLATION,
+    SupportedTask.FILL_MASK,
+    SupportedTask.TEXT_GENERATION,
+    SupportedTask.CHAT_COMPLETION,
+]
+
+VLLM_MII_TASKS = [
+    SupportedTask.TEXT_GENERATION,
+    SupportedTask.CHAT_COMPLETION,
+    TaskType.CONVERSATIONAL
+]
+
+MULTILABEL_SET = [
+    SupportedTask.TEXT_CLASSIFICATION_MULTILABEL,
+]
+
+CLASSIFICATION_SET = [
+    SupportedTask.TEXT_CLASSIFICATION,
+    SupportedTask.TEXT_CLASSIFICATION_MULTILABEL
+]
+
+MULTIPLE_OUTPUTS_SET = [
+    SupportedTask.NER,
+    SupportedTask.TEXT_CLASSIFICATION_MULTILABEL
+]
```

## llm/optimized/inference/fm_score.py

```diff
@@ -2,15 +2,15 @@
 # Licensed under the MIT License.
 """This module provides the FMScore class for running inference engines with given prompts and parameters."""
 import json
 import os
 from typing import Dict, List
 
 from llm.optimized.inference.configs import EngineConfig, TaskConfig
-from llm.optimized.inference.constants import TaskType
+from llm.optimized.inference.constants import TaskType, EngineName
 from llm.optimized.inference.engine.engine import InferenceResult
 from llm.optimized.inference.logging_config import configure_logger
 from llm.optimized.inference.managed_inference import MIRPayload
 from llm.optimized.inference.prompt_formatter import Llama2Formatter
 from llm.optimized.inference.replica_manager import ReplicaManager, ReplicaManagerConfig
 from llm.optimized.inference.utils import log_execution_time
 
@@ -31,15 +31,25 @@
     def __init__(self, config: Dict):
         """Initialize the FMScore with the given configuration."""
         self.task_config = TaskConfig.from_dict(config["task"])
         self.engine_config = EngineConfig.from_dict(config["engine"])
 
     def init(self):
         """Initialize the engine and formatter."""
-        self.replica_manager = self._init_replica_manager()
+        try:
+            self.replica_manager = self._init_replica_manager()
+        except Exception as e:
+            if self.engine_config.engine_name != EngineName.HF:
+                logger.warning(f"Replica manager failed to initialize with engine {self.engine_config.engine_name}")
+                logger.warning("Falling back to HF engine.")
+                self.engine_config.engine_name = EngineName.HF
+                self._init_replica_manager()
+            else:
+                logger.error(f"Failed to create Engine with exception {repr(e)}")
+                raise e
         self.formatter = self._initialize_formatter()
 
     def _init_replica_manager(self):
         replica_manager_config = ReplicaManagerConfig(
             engine_config=self.engine_config,
             task_config=self.task_config,
             num_replicas=int(os.environ.get("NUM_REPLICAS", -1)),
@@ -77,14 +87,20 @@
             self.formatter.format_prompt(self.task_config.task_type, prompt, payload.params)
             for prompt in payload.query
         ]
         inference_results = self.replica_manager.get_replica().generate(formatted_prompts, payload.params)
         return inference_results
 
     def _initialize_formatter(self):
+        if (
+            hasattr(self.engine_config, "custom_model_config_builder")
+            and self.engine_config.custom_model_config_builder
+        ):
+            return self.engine_config.custom_model_config_builder.get_formatter()
+
         formatter = get_formatter(model_name="Llama2")
         return formatter
 
     async def shutdown_async(self):
         """Terminate DS-MII Server."""
         await self.replica_manager.get_replica().shutdown_async()
```

## llm/optimized/inference/managed_inference.py

```diff
@@ -18,15 +18,15 @@
 DEFAULT_MODEL_PATH = "mlflow_model_folder/data/model"
 
 
 @dataclass
 class MIRPayload(SerializableDataClass):
     """Json serializable dataclass that represents the input received from the server."""
 
-    query: Union[str, List[str]]
+    query: Union[str, List[str], List[Tuple[str, str]]]
     params: Dict[str, Any]
     task_type: str
     is_preview_format: bool
 
     @classmethod
     def from_dict(cls, mir_input_data: Dict):
         """Create an instance of MIRPayload from input data received from the server."""
@@ -43,15 +43,15 @@
             self.query = [self.query]
 
     def update_params(self, new_params: Dict) -> None:
         """Update current parameters to the new parameters the MIRPayload should have."""
         self.params = new_params
 
 
-def get_processed_input_data_for_chat_completion(dialog: List[str]) -> str:
+def get_processed_input_data_for_chat_completion(dialog: List[str], add_generation_prompt: bool) -> str:
     r"""Process chat completion input request.
 
     example input:
     [
         {
             "role": "user",
             "content": "What is the tallest building in the world?"
@@ -74,33 +74,63 @@
     tokenizer_path = str(os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), DEFAULT_TOKENIZER_PATH))
     if not os.path.exists(tokenizer_path):
         tokenizer_path = os.path.join(
             os.getenv("AZUREML_MODEL_DIR", ""),
             DEFAULT_MODEL_PATH,
         )
     # use tokenizer defined in tokenizer_config
-    tokenizer = AutoTokenizer.from_pretrained(tokenizer_path, use_default_system_prompt=False)
+    tokenizer = AutoTokenizer.from_pretrained(tokenizer_path, use_default_system_prompt=False, trust_remote_code=True)
     # apply template to format chat conversation
-    chat_conv = tokenizer.apply_chat_template(dialog, tokenize=False)
+    chat_conv = tokenizer.apply_chat_template(dialog, tokenize=False, add_generation_prompt=add_generation_prompt)
     return chat_conv
 
 
-def process_input_data_for_text_to_image(inputs: Dict[str, any]) -> Tuple[List[str], Dict[str, Any]]:
+def process_input_data_for_text_to_image(
+    inputs: Dict[str, any]
+) -> Tuple[List[Tuple[str, str, str, str]], Dict[str, Any]]:
     """Process text to image task input request to make it suitable for model.
 
     :param inputs: input data
     :type inputs: Dict[str, any]
-    :raises Exception: if input data is not in expected format
-    :return: Processed input data for model and parameters
-    :rtype: Tuple[List[str], Dict[str, Any]]
+    :return: Processed input data in list of tuple (prompt and negative_prompt(optional)) for model and parameters.
+    For text-to-image-inpainting task, it will return `init_image` and `mask_image`.
+    For text-to-image task these values would be None
+    :rtype: Tuple[List[Tuple[str, str]], Dict[str, Any]]
     """
     params = inputs.pop("parameters", {})
     if "columns" in inputs and "data" in inputs:
         input_df = pd.DataFrame(**inputs)
-        input_data = input_df["prompt"].to_list()
+        prompt_data = input_df["prompt"].to_list()
+        number_of_prompts = len(prompt_data)
+
+        negative_prompt_data = (
+            input_df["negative_prompt"].to_list()
+            if "negative_prompt" in input_df.columns
+            else [""] * number_of_prompts
+        )
+
+        init_image = (
+            input_df["image"].to_list()
+            if "image" in input_df.columns
+            else [None] * number_of_prompts
+        )
+
+        mask_image = (
+            input_df["mask_image"].to_list()
+            if "image" in input_df.columns
+            else [None] * number_of_prompts
+        )
+
+        input_data = []
+        for i in range(number_of_prompts):
+            input_data.append([prompt_data[i],
+                               "" if pd.isna(negative_prompt_data[i]) else negative_prompt_data[i],
+                               init_image[i],
+                               mask_image[i]
+                               ])
     return input_data, params
 
 
 def get_request_data(data) -> (Tuple)[Union[str, List[str]], Dict[str, Any], str, bool]:
     """Process and validate inference request.
 
     return type for chat-completion: str, dict, str, bool
@@ -113,15 +143,15 @@
         # TODO: Update this check once all tasks are updated to use new input format
         if task_type != TaskType.TEXT_GENERATION:
             if not isinstance(inputs, dict):
                 raise Exception("Invalid input data")
 
         if task_type == "chat-completion":
             task_type = TaskType.CONVERSATIONAL
-        elif task_type == TaskType.TEXT_TO_IMAGE:
+        elif task_type in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING]:
             input_data, params = process_input_data_for_text_to_image(inputs)
             return input_data, params, task_type, is_preview_format
 
         input_data = []  # type: Union[str, List[str]]
         params = {}  # type: Dict[str, Any]
 
         # Input format is being updated
@@ -140,27 +170,36 @@
             raise Exception("query is not a list")
 
         if not isinstance(params, dict):
             raise Exception("parameters is not a dict")
 
         if task_type == TaskType.CONVERSATIONAL:
             logger.info("chat-completion task. Processing input data")
-            input_data = get_processed_input_data_for_chat_completion(input_data)
+            add_generation_prompt = params.pop("add_generation_prompt", True)
+            input_data = get_processed_input_data_for_chat_completion(input_data, add_generation_prompt)
 
         return input_data, params, task_type, is_preview_format
     except Exception as e:
         task_type = data.get("task_type", TaskType.TEXT_GENERATION)
         if task_type == "chat-completion":
             correct_input_format = (
                 '{"input_data": {"input_string": [{"role":"user", "content": "str1"}, '
                 '{"role": "assistant", "content": "str2"} ....], "parameters": {"k1":"v1", "k2":"v2"}}}'
             )
         elif task_type == TaskType.TEXT_TO_IMAGE:
             correct_input_format = (
-                '{"input_data": {"columns": ["prompt"], "data": ["prompt sample 1", "prompt sample 2"], '
+                '{"input_data": {"columns": ["prompt", "negative_prompt"], \
+                "data": [{"prompt": "prompt(str)", "negative_prompt": "negative prompt (optional, str)"}], '
+                '"parameters": {"k1":"v1", "k2":"v2"}}}'
+            )
+        elif task_type == TaskType.TEXT_TO_IMAGE_INPAINTING:
+            correct_input_format = (
+                '{"input_data": {"columns": ["prompt", "negative_prompt", "image", "mask_image"], \
+                "data": [{"prompt": "prompt(str)", "negative_prompt": "negative prompt (optional, str)", \
+                "image": "init_image (base64/url)", "mask_image": "mask_image (base64/url)"}], '
                 '"parameters": {"k1":"v1", "k2":"v2"}}}'
             )
         else:
             correct_input_format = (
                 '{"input_data": ["str1", "str2", ...], '
                 '"params": {"k1":"v1", "k2":"v2"}}'
             )
```

## llm/optimized/inference/model_config_factory.py

```diff
@@ -22,11 +22,11 @@
         :param kwargs: keyword arguments (model_type: supported model family for task).
         :type kwargs: dict
         :raises ValueError: Invalid task or model type
         :return: model configuration object
         :rtype: ModelConfiguration
         """
         model_type = kwargs.pop("model_type", "")
-        if task == TaskType.TEXT_TO_IMAGE and model_type == "stable-diffusion":
+        if task in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING] and model_type == "stable-diffusion":
             return DiffusionConfigurationBuilder(task)
         else:
             raise ValueError("Invalid task or model type.")
```

## llm/optimized/inference/prompt_formatter.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """Module for formatting prompts for different tasks and models."""
 from abc import ABC, abstractmethod
-from typing import Dict, Union
+from typing import Dict, List, Union
 
 from llm.optimized.inference.constants import TaskType
 from llm.optimized.inference.conversation import Conversation
 
 
 class AbstractPromptFormatter(ABC):
     """Abstract base class for prompt formatters."""
@@ -28,8 +28,23 @@
     def format_prompt(
         self,
         task_type: TaskType,
         query: Union[str, Conversation],
         params: Dict,
     ) -> str:
         """Format the prompt for Llama2 models. Currently a placeholder."""
+        if task_type == TaskType.QnA:
+            return list(query)
         return str(query)
+
+
+class Text2ImgFormatter(AbstractPromptFormatter):
+    """Prompt formatter for stable diffusion text2img models."""
+
+    def format_prompt(
+        self,
+        task_type: TaskType,
+        query: List[tuple[str, Union[str, None]]],
+        params: Dict,
+    ) -> str:
+        """Format the prompt for text 2 image models. Currently a placeholder."""
+        return query
```

## llm/optimized/inference/replica_manager.py

```diff
@@ -1,34 +1,35 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """This class provides model replication and load balancing functionality."""
 import os
 import random
 import tempfile
 import time
-from concurrent.futures import ProcessPoolExecutor
+import torch
+from concurrent.futures import ThreadPoolExecutor
+import traceback
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import List
 
-import torch
 from llm.optimized.inference.configs import EngineConfig, TaskConfig
 from llm.optimized.inference.engine import BaseEngine
 from llm.optimized.inference.logging_config import configure_logger
 
 logger = configure_logger(__name__)
 
 
 def get_engine(engine_config: EngineConfig, task_config: TaskConfig) -> BaseEngine:
     """Return the appropriate engine based on the engine name."""
     engine_name = engine_config.engine_name
     if engine_name == "hf":
-        from engine import HfEngine
+        from llm.optimized.inference.engine.hf_engine import HfEngine
 
-        return HfEngine(engine_config)
+        return HfEngine(engine_config, task_config)
     elif engine_name == "vllm":
         from llm.optimized.inference.engine.vllm_engine import VLLMEngine
 
         return VLLMEngine(engine_config, task_config)
     elif engine_name == "mii":
         from llm.optimized.inference.engine.mii_engine_v2 import MiiEngineV2
 
@@ -70,14 +71,17 @@
 class ReplicaManager:
     """Class for managing replicas of a model."""
 
     def __init__(self, replica_config: ReplicaManagerConfig):
         """Initialize the ReplicaManager."""
         self._replica_config = replica_config
         self._engine_config = self._replica_config.engine_config
+        self.is_hf = False
+        if self._engine_config.engine_name == "hf":
+            self.is_hf = True
         self._task_config = self._replica_config.task_config
 
         self.engine_replicas = []  # type: List[BaseEngine]
         self._replica_index = 0  # index of the next available replica
 
         self._set_defaults()
 
@@ -112,47 +116,59 @@
 
         if os.path.exists(flag_file_path):
             logger.info(
                 f"PID[{os.getpid()}] Model already being loaded by another worker.",
             )
             # wait for all replicas to finish loading the model
             while os.path.exists(flag_file_path):
+                logger.info(f"Waiting for model to finish loading. Current worker pid: {os.getpid()}")
                 time.sleep(5)
             for engine in self.engine_replicas:
                 engine.init_client()
         else:
             try:
                 with open(flag_file_path, "x"):
                     logger.info(
                         f"Lock acquired by worker with pid: {os.getpid()}. Loading model. \
 Using tensor parallel of {self._tensor_parallel} GPUs per replica.",
                     )
                     process_is_loading_model = True
                     logger.handlers[0].flush()
                     os.environ["LOGGING_WORKER_ID"] = str(os.getpid())
-                    # Start replicas in parallel using ProcessPoolExecutor
-                    with ProcessPoolExecutor() as executor:
-                        executor.map(
-                            self._launch_single_replica,
-                            range(num_replicas),
-                        )
+
+                    if self._engine_config.engine_name == "hf":
+                        # Synchronously create model instances
+                        logger.info("Launching Replicas synchronously")
+                        for idx in range(num_replicas):
+                            logger.info(f"Launching Replica: {idx}")
+                            self.engine_replicas[idx] = self._launch_single_replica(idx)
+                    else:
+                        # Start replicas in parallel using ProcessPoolExecutor
+                        with ThreadPoolExecutor() as executor:
+                            self.engine_replicas = list(
+                                executor.map(
+                                    self._launch_single_replica,
+                                    range(num_replicas),
+                                )
+                            )
             except FileExistsError:
                 logger.info(
                     f"Model already being loaded by another worker. Waiting for model to finish loading. "
                     f"Current worker pid: {os.getpid()}",
                 )
 
         if process_is_loading_model:
             # Load the model and print GPU information
             logger.info("###### GPU INFO ######")
             logger.info(os.system("nvidia-smi"))
             logger.info("###### GPU INFO ######")
 
             if os.path.exists(flag_file_path):
                 os.remove(flag_file_path)
+
         if os.environ.get("LOGGING_WORKER_ID", "") == str(os.getpid()):
             print(f"Initialized {self._replica_config.num_replicas} replicas.")
             print(f"Server URIs: {[engine.server_url for engine in self.engine_replicas]}")
 
     def _launch_single_replica(self, replica_idx):
         """Launch a single replica."""
         engine_replica = self.engine_replicas[replica_idx]
@@ -169,14 +185,16 @@
                 f"Starting replica {replica_idx + 1} with GPUs {cuda_visible_devices} "
                 f"for engine: {engine_replica.engine_config.engine_name}",
             )
             engine_replica.load_model(env=local_env)
             engine_replica.init_client()
         except Exception as e:
             logger.error(f"Failed to start replica {replica_idx + 1} with GPUs {cuda_visible_devices}: {e}")
+            traceback.print_exc()
+        return engine_replica
 
     def _get_gpu_ids_for_replica(self, replica_idx: int, gpu_ids_list: List[int]) -> List[int]:
         """Get the GPU IDs for a specific replica."""
         # By default, use all available GPUs
         if self._tensor_parallel in ["", None]:
             replica_gpu_ids = gpu_ids_list
         else:
@@ -196,14 +214,15 @@
         )
         return replica
 
     def _get_tensor_parallel(self):
         """Get the tensor parallel configuration for each replica."""
         # evenly divide the available GPUs among the replicas
         res = max(torch.cuda.device_count() // self._replica_config.num_replicas, 1)
+        logger.info(f"Using tensor parallel of {res} GPUs per replica.")
         return res
 
     def _set_defaults(self):
         """Do some sanity checks and set default values for the replica config and tensor parallel."""
         if self._replica_config.num_replicas >= 1:
             # num_replicas is set by the user
             if self._replica_config.engine_config.tensor_parallel in [None, ""]:
```

## llm/optimized/inference/score.py

```diff
@@ -13,32 +13,35 @@
 import torch
 import yaml
 from azure.ai.contentsafety import ContentSafetyClient
 from azure.ai.contentsafety.models import AnalyzeTextOptions, AnalyzeImageOptions, ImageData
 from azure.core.credentials import AzureKeyCredential
 from azure.core.pipeline.policies import HeadersPolicy
 from azureml.ai.monitoring import Collector
-from llm.optimized.inference.constants import EngineName, SupportedTask, TaskType
+from llm.optimized.inference.constants import EngineName, SupportedTask, TaskType, ALL_TASKS, VLLMSupportedModels, MIISupportedModels
 from llm.optimized.inference.model_config_factory import ModelConfigFactory
 from llm.optimized.inference.fm_score import FMScore
 from llm.optimized.inference.logging_config import configure_logger
 from llm.optimized.inference.managed_inference import MIRPayload
 from mlflow.pyfunc.scoring_server import _get_jsonable_obj
 from llm.optimized.inference.utils import box_logger, map_env_vars_to_vllm_server_args
+from llm.optimized.inference.model_utils import build_configs_from_model, get_generator_params
 
 logger = configure_logger(__name__)
 
 # AACS
 g_aacs_threshold = int(os.environ.get("CONTENT_SAFETY_THRESHOLD", 2))
 g_aacs_client = None
 
 # default values
 DEVICE_COUNT = torch.cuda.device_count()
 MLMODEL_PATH = "mlflow_model_folder/MLmodel"
 DEPRECATED_MLFLOW_MODEL_PATH = "mlflow_model_folder/data/model"
+DEPRECATED_MLFLOW_CONFIG_PATH = "mlflow_model_folder/data/config"
+DEPRECATED_MLFLOW_TOKENIZER_PATH = "mlflow_model_folder/data/tokenizer"
 DEFAULT_MLFLOW_MODEL_PATH = "mlflow_model_folder/model"
 DEFAULT_TOKENIZER_PATH = "mlflow_model_folder/components/tokenizer"
 task_type = SupportedTask.TEXT_GENERATION
 g_fmscorer: FMScore = None
 g_model_signature = None
 
 # # metrics tracking
@@ -253,27 +256,14 @@
 
     return key
 
 
 # endregion
 
 
-def get_generator_params(params: dict):
-    """Return accumulated generator params."""
-    updated_params = {}
-    # map 'max_gen_len' to 'max_new_tokens' if present
-    if "max_gen_len" in params:
-        logger.warning("max_gen_len is deprecated. Use max_new_tokens")
-        params["max_new_tokens"] = params["max_gen_len"]
-        del params["max_gen_len"]
-
-    updated_params.update(params)
-    return updated_params
-
-
 def _init_cuda_visible_devices():
     import torch
 
     if "CUDA_VISIBLE_DEVICES" in os.environ:
         return
 
     if "NVIDIA_VISIBLE_DEVICES" in os.environ and os.environ["NVIDIA_VISIBLE_DEVICES"] != "all":
@@ -284,14 +274,15 @@
         gpu_ids = [str(i) for i in range(torch.cuda.device_count())]
     else:
         # if no GPU is available, don't set anything
         return
     os.environ["CUDA_VISIBLE_DEVICES"] = ",".join(gpu_ids)
 
 
+
 def init():
     """Initialize text-generation-inference server and client."""
     global g_fmscorer
     global task_type
     global g_aacs_client
     global g_model_signature
 
@@ -312,136 +303,52 @@
             endpoint,
             AzureKeyCredential(key),
             headers_policy=headers_policy,
         )
     except Exception as e:
         AACS_error = e
     try:
-        model_path = os.path.join(
-            os.getenv("AZUREML_MODEL_DIR", ""),
-            DEFAULT_MLFLOW_MODEL_PATH,
-        )
-
-        tokenizer_path = os.path.join(
-            os.getenv("AZUREML_MODEL_DIR", ""),
-            DEFAULT_TOKENIZER_PATH,
-        )
-
-        # Maintain Backwards Compatibility with old file structure
-        if not os.path.exists(model_path):
+        if os.path.exists(os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), DEFAULT_MLFLOW_MODEL_PATH)):
             model_path = os.path.join(
                 os.getenv("AZUREML_MODEL_DIR", ""),
-                DEPRECATED_MLFLOW_MODEL_PATH,
+                DEFAULT_MLFLOW_MODEL_PATH,
             )
-            tokenizer_path = model_path
-
-        config_path = os.path.join(model_path, "config.json")
-        
-        default_engine = EngineName.VLLM
-        tensor_parallel = os.getenv("TENSOR_PARALLEL", None)
-        if tensor_parallel:
-            tensor_parallel = int(tensor_parallel)
-        engine_config = {
-            "engine_name": os.getenv("ENGINE_NAME", default_engine),
-            "model_id": model_path,
-            "tokenizer": tokenizer_path,
-            "tensor_parallel": tensor_parallel,
-        }
+            config_path = os.path.join(model_path, "config.json")
+            tokenizer_path = os.path.join(
+                os.getenv("AZUREML_MODEL_DIR", ""), DEFAULT_TOKENIZER_PATH
+            )
+        else:
+            model_path = os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), DEPRECATED_MLFLOW_MODEL_PATH)
+            config_path = os.path.join(
+                os.getenv("AZUREML_MODEL_DIR", ""), DEPRECATED_MLFLOW_CONFIG_PATH, "config.json"
+            )
+            tokenizer_path = os.path.join(
+                os.getenv("AZUREML_MODEL_DIR", ""), DEPRECATED_MLFLOW_TOKENIZER_PATH
+            )
+            
 
         _init_cuda_visible_devices()
 
         abs_mlmodel_path = os.path.join(
             os.getenv("AZUREML_MODEL_DIR", ""),
             MLMODEL_PATH,
         )
         mlmodel = {}
         if abs_mlmodel_path and os.path.exists(abs_mlmodel_path):
             with open(abs_mlmodel_path) as f:
                 mlmodel = yaml.safe_load(f)
 
-        default_generator_configs = ""
-        task_config = None
         if mlmodel:
-            flavors = mlmodel.get("flavors", {})
             g_model_signature = mlmodel.get("signature", None)
-            if "transformers" in flavors:
-                task_type = flavors["transformers"]["task"]
-
-                model_generator_configs = flavors["transformers"].get(
-                    "generator_config",
-                    {},
-                )
-                if task_type not in (
-                    SupportedTask.TEXT_GENERATION,
-                    SupportedTask.CHAT_COMPLETION,
-                ):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                # update default gen configs with model configs
-                default_generator_configs = get_generator_params(
-                    model_generator_configs,
-                )
-            elif "hftransformersv2" in flavors:
-                task_type = flavors["hftransformersv2"]["task_type"]
-
-                model_generator_configs = flavors["hftransformersv2"].get(
-                    "generator_config",
-                    {},
-                )
-                if task_type not in (
-                    SupportedTask.TEXT_GENERATION,
-                    SupportedTask.CHAT_COMPLETION,
-                ):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                # update default gen configs with model configs
-                default_generator_configs = get_generator_params(
-                    model_generator_configs,
-                )
-            elif "python_function" in flavors:
-                task_type = mlmodel["metadata"]["base_model_task"]
-                if task_type not in (TaskType.TEXT_TO_IMAGE):
-                    raise Exception(f"Unsupported task_type {task_type}")
-
-                model_type = mlmodel["metadata"].get("model_type", "")
-                
-                model_config_builder = ModelConfigFactory.get_config_builder(task=task_type, model_type=model_type)
-                engine_config.update(
-                                        {
-                                            "engine_name": model_config_builder.engine,
-                                            "mii_config": model_config_builder.get_optimization_config(),
-                                            "custom_model_config_builder": model_config_builder,
-                                            "model_id": os.path.join(os.getenv("AZUREML_MODEL_DIR", ""), model_config_builder.model_path),
-                                            "tensor_parallel": model_config_builder.tensor_parallel
-                                        }
-                                    )
-                task_config = model_config_builder.get_task_config()
-
-        if engine_config["engine_name"] in [EngineName.MII, EngineName.MII_V1] and "mii_config" not in engine_config:
-            mii_engine_config = {
-                "deployment_name": os.getenv("DEPLOYMENT_NAME", "llama-deployment"),
-                "mii_configs": {},
-            }
-
-            engine_config["mii_config"] = mii_engine_config
-
-        if engine_config["engine_name"] == EngineName.VLLM:
-            model_config = {}
-            vllm_config = map_env_vars_to_vllm_server_args()
-            if config_path and os.path.exists(config_path):
-                with open(config_path) as config_content:
-                    model_config = json.load(config_content)
-            engine_config["vllm_config"] = vllm_config
-            engine_config["model_config"] = model_config
-
-        task_config = {
-            "task_type": TaskType.CONVERSATIONAL
-            if task_type == SupportedTask.CHAT_COMPLETION
-            else TaskType.TEXT_GENERATION,
-        } if task_config is None else task_config
+        engine_config, task_config, default_generator_configs, task_type = build_configs_from_model(
+            mlmodel,
+            model_path,
+            config_path,
+            tokenizer_path
+        )
 
         config = {
             "engine": engine_config,
             "task": task_config,
         }
 
         g_fmscorer = FMScore(config)
```

## llm/optimized/inference/utils.py

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """This module provides a decorator to log the execution time of functions."""
 import os
 import time
 import io
 import base64
+import requests
 
 import torch
 
 from llm.optimized.inference.logging_config import configure_logger
 from PIL.Image import Image
 
 logger = configure_logger(__name__)
@@ -82,14 +83,16 @@
     }
 
     cli_args = {}
     for env_var, cli_arg in env_to_cli_map.items():
         if env_var in os.environ:
             cli_args[cli_arg] = os.environ[env_var]
 
+    box_logger(f"vLLM server arguments: {cli_args}")
+
     return cli_args
 
 
 def image_to_base64(img: Image, format: str) -> str:
     """
     Convert image into Base64 encoded string.
 
@@ -102,14 +105,41 @@
     """
     buffered = io.BytesIO()
     img.save(buffered, format=format)
     img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
     return img_str
 
 
+def convert_image_to_bytes(image: str) -> bytes:
+    """Convert image into bytes.
+
+    :param image: The Base64 encoded string to be decoded or http url.
+    :type image: str
+    :return: The decoded bytes object.
+    :rtype: bytes
+    """
+    try:
+        if image.startswith("http://") or image.startswith("https://"):
+            try:
+                image = requests.get(image, stream=True)
+                image = image.content
+            except Exception as ex:
+                raise Exception(
+                    f"Failed to download the image from the URL. {str(ex)}."
+                    "Alternatively, use images in base64 format."
+                )
+        else:
+            image = base64.b64decode(image)
+    except Exception as ex:
+        raise ValueError(
+            f"Image should be either URL or in base64 format. URLs must start with `http://` or `https://`. {str(ex)}"
+        )
+    return image
+
+
 def get_gpu_device_capability() -> float:
     """
     Get the GPU device capability version.
 
     :return: GPU device capability version
     :rtype: float
     """
```

## llm/optimized/inference/custom_model_configurations/base_configuration_builder.py

```diff
@@ -3,14 +3,15 @@
 
 """The base configuration class for all type of models."""
 
 
 from abc import ABC, abstractmethod
 from typing import List, Dict
 
+from llm.optimized.inference.prompt_formatter import AbstractPromptFormatter, Llama2Formatter
 from llm.optimized.inference.constants import EngineName
 
 
 class ModelConfigurationBuilder(ABC):
     """Base class for model configurations builder for optimization engine configuration."""
 
     MLFLOW_MODEL_PATH = "mlflow_model_folder/data/model"
@@ -68,7 +69,22 @@
     def update_mii_model_config(self, model_config: object) -> None:
         """Override the default MII model configuration.
 
         :param model_config: MII model configuration
         :type model_config: mii.ModelConfig
         """
         pass
+
+    def pre_processing(self, queries: Dict, **kwargs) -> None:
+        """Preprocess and update the input queries dictionary for the model. \
+        Default implementation is do "nothing".
+
+        :param queries: input queries
+        :type queries: Dict
+        :param kwargs: additional arguments
+        :type kwargs: Dict
+        """
+        pass
+
+    def get_formatter(self) -> AbstractPromptFormatter:
+        """Get the query formatter object. Default is Llama2 model formatter."""
+        return Llama2Formatter()
```

## llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py

```diff
@@ -10,22 +10,24 @@
 
 try:
     from mii.config import ModelConfig
     from mii.legacy.models.utils import ImageResponse
 except ImportError:
     print("MII installation skipped for unit testing.")
 
+from llm.optimized.inference.prompt_formatter import Text2ImgFormatter, AbstractPromptFormatter
+
 from llm.optimized.inference.custom_model_configurations.base_configuration_builder import ModelConfigurationBuilder
 from llm.optimized.inference.constants import EngineName, TaskType
 from llm.optimized.inference.custom_model_configurations.schema_output import (
     ImageTaskInferenceResult,
     TextToImageSchema,
 )
 from llm.optimized.inference.logging_config import configure_logger
-from llm.optimized.inference.utils import get_gpu_device_capability
+from llm.optimized.inference.utils import convert_image_to_bytes, get_gpu_device_capability
 
 logger = configure_logger(__name__)
 
 
 class DiffusionConfigurationBuilder(ModelConfigurationBuilder):
     """Diffusion model configuration builder for optimization inference configuration."""
 
@@ -68,16 +70,17 @@
 
     def get_optimization_config(self) -> Dict[str, str]:
         """Optimization config for diffusion model.
 
         :return: optimization configuration
         :rtype: Dict[str, str]
         """
+        default_deployment_name = f"{self._task}-deployment"[:30]
         return {
-            "deployment_name": os.getenv("DEPLOYMENT_NAME", "text2image-deployment"),
+            "deployment_name": os.getenv("DEPLOYMENT_NAME", default_deployment_name),
             "mii_configs": {},
         }
 
     @staticmethod
     def _post_processing_text_to_image(
         responses: "ImageResponse", inference_time: float, prompts: List[str] = None
     ) -> List[ImageTaskInferenceResult]:
@@ -96,15 +99,15 @@
         images = responses.images
         nsfw_content_detected = responses.nsfw_content_detected
         for i in range(len(images)):
             result.append(
                 ImageTaskInferenceResult(
                     response=TextToImageSchema(
                         generated_image=images[i],
-                        prompt=prompts[i] if prompts else None,
+                        prompt=prompts[i][0] if prompts else None,
                         nsfw_content_detected=nsfw_content_detected[i] if nsfw_content_detected else None,
                     ),
                     inference_time_ms=inference_time,
                 )
             )
         return result
 
@@ -116,15 +119,17 @@
         :param inference_time: inference time in milliseconds
         :type inference_time: float
         :param kwargs: additional arguments
         :type kwargs: Dict
         :return: processed model response
         :rtype: List of ImageTaskInferenceResult
         """
-        TASK_POST_PROCESSING_MAP = {TaskType.TEXT_TO_IMAGE: self._post_processing_text_to_image}
+        TASK_POST_PROCESSING_MAP = {TaskType.TEXT_TO_IMAGE: self._post_processing_text_to_image,
+                                    TaskType.TEXT_TO_IMAGE_INPAINTING: self._post_processing_text_to_image
+                                    }
         prompts = kwargs.get("prompts")
         result = TASK_POST_PROCESSING_MAP[self._task](responses, inference_time, prompts)
         return result
 
     def update_mii_model_config(self, model_config: "ModelConfig") -> None:
         """Override the default MII model configuration depending on task and GPU compute capability.
 
@@ -135,7 +140,76 @@
         model_config.load_with_sys_mem = False  # Not supported for diffusers
         model_config.task = self._task
         model_config.model_path = self.MLFLOW_MODEL_PATH
         if get_gpu_device_capability() <= 7.0:
             model_config.replace_with_kernel_inject = False
             model_config.meta_tensor = True
             model_config.enable_cuda_graph = True
+
+    def get_formatter(self) -> AbstractPromptFormatter:
+        """Return formatter object for specific tasks supported by diffusion model."""
+        TASK_FORMATTER_MAP = {
+            TaskType.TEXT_TO_IMAGE: Text2ImgFormatter,
+            TaskType.TEXT_TO_IMAGE_INPAINTING: Text2ImgFormatter
+        }
+        return TASK_FORMATTER_MAP[self._task]()
+
+    def pre_processing(self, queries: Dict, **kwargs) -> None:
+        """Preprocess the input queries for the model.
+
+        :param queries: input queries
+        :type queries: Dict
+        :param kwargs: additional arguments
+        :type kwargs: Dict
+        """
+        TASK_PRE_PROCESSING_MAP = {TaskType.TEXT_TO_IMAGE: self._pre_processing_text_to_image,
+                                   TaskType.TEXT_TO_IMAGE_INPAINTING: self._pre_processing_text_to_image_inpainting
+                                   }
+        TASK_PRE_PROCESSING_MAP[self._task](queries)
+
+    def _pre_processing_text_to_image_inpainting(self, queries: Dict) -> None:
+        """Preprocess the input queries for inpainting task.
+
+        :param queries: input queries
+        :type queries: Dict
+        :param kwargs: additional arguments
+        :type kwargs: Dict
+        """
+        input_dict = queries.pop("query")
+
+        prompt = []
+        negative_prompt = []
+        image = []
+        mask_image = []
+        for i in range(len(input_dict)):
+            prompt.append(input_dict[i][0])
+            if len(input_dict[i]) > 1:
+                negative_prompt.append(input_dict[i][1])
+            else:
+                negative_prompt.append("")
+            image.append(convert_image_to_bytes(input_dict[i][2]))
+            mask_image.append(convert_image_to_bytes(input_dict[i][3]))
+        queries["prompt"] = prompt
+        queries["negative_prompt"] = negative_prompt
+        queries["image"] = image
+        queries["mask_image"] = mask_image
+
+    def _pre_processing_text_to_image(self, queries: Dict, **kwargs) -> None:
+        """Preprocess the input queries for the text to image task.
+
+        :param queries: input queries
+        :type queries: Dict
+        :param kwargs: additional arguments
+        :type kwargs: Dict
+        """
+        input_dict = queries.pop("query")
+
+        prompt = []
+        negative_prompt = []
+        for i in range(len(input_dict)):
+            prompt.append(input_dict[i][0])
+            if len(input_dict[i]) > 1:
+                negative_prompt.append(input_dict[i][1])
+            else:
+                negative_prompt.append("")
+        queries["prompt"] = prompt
+        queries["negative_prompt"] = negative_prompt
```

## llm/optimized/inference/engine/engine.py

```diff
@@ -6,19 +6,17 @@
 import os
 import socket
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
-import torch
-from llm.optimized.inference.configs import EngineConfig
 from llm.optimized.inference.constants import ServerSetupParams, TaskType
 from llm.optimized.inference.logging_config import configure_logger
-from transformers import AutoModelForCausalLM, AutoTokenizer
+from transformers import AutoTokenizer
 from llm.optimized.inference.utils import box_logger, log_execution_time
 
 logger = configure_logger(__name__)
 
 
 @dataclass
 class InferenceResult:
@@ -26,14 +24,15 @@
 
     response: str
     inference_time_ms: float
     time_per_token_ms: float
     generated_tokens: List[Any]
     prompt_num: int
     error: Optional[str] = None
+    scores: Optional[List[Any]] = None
 
     def print_results(self):
         """Print the inference results of a single prompt."""
         if self.error:
             msg = f"## Inference Results ##\n ERROR: {self.error}"
         else:
             # TODO: record time per prompt in mii so we can show inference time for each prompt
@@ -106,51 +105,13 @@
             time.sleep(30)
         raise Exception("Server did not become healthy within 15 minutes.")
 
     @log_execution_time
     def get_tokens(self, response: str):
         """Load tokenizer and get tokens from a prompt."""
         if not hasattr(self, "tokenizer"):
-            self.tokenizer = AutoTokenizer.from_pretrained(self.engine_config.tokenizer)
+            if getattr(self.engine_config, "tokenizer", None) is not None:
+                self.tokenizer = AutoTokenizer.from_pretrained(self.engine_config.tokenizer, trust_remote_code=True)
+            else:
+                self.tokenizer = AutoTokenizer.from_pretrained(self.engine_config.model_id, trust_remote_code=True)
         tokens = self.tokenizer.encode(response)
         return tokens
-
-
-class HfEngine(BaseEngine):
-    """Inference engine using Hugging Face methods."""
-
-    def __init__(self, engine_config: EngineConfig):
-        """Initialize the HfEngine with the given engine configuration."""
-        self.engine_config = engine_config
-
-    def load_model(self, env=None):
-        """Load the model from the pretrained model specified in the engine configuration."""
-        self.tokenizer = AutoTokenizer.from_pretrained(self.engine_config.tokenizer)
-        self.model = AutoModelForCausalLM.from_pretrained(self.engine_config.model_id)
-        # move to the model to the GPU if testing on GPU
-        if torch.cuda.is_available():
-            self.model.to("cuda")
-        self.model.eval()
-
-    @log_execution_time
-    def generate(self, prompts: List[str], params: Dict) -> List[InferenceResult]:
-        """Generate responses for given prompts."""
-        inference_results = []  # type: List[InferenceResult]
-        with torch.no_grad():
-            for i, prompt in enumerate(prompts):
-                start_time = time.time()
-                input_ids = self.tokenizer.encode(prompt, return_tensors="pt")
-                output = self.model.generate(input_ids, max_new_tokens=20)
-                generated_text = self.tokenizer.decode(
-                    output[0],
-                    skip_special_tokens=True,
-                )
-                inference_time_ms = (time.time() - start_time) * 1000
-                num_tokens = len(output[0])
-                time_per_token_ms = inference_time_ms / num_tokens if num_tokens > 0 else 0
-                result = InferenceResult(
-                    response=generated_text,
-                    inference_time_ms=inference_time_ms,
-                    time_per_token_ms=time_per_token_ms,
-                )
-                inference_results.append(result)
-        return inference_results
```

## llm/optimized/inference/engine/mii_engine.py

```diff
@@ -65,19 +65,23 @@
     async def generate(self, prompts: List[str], params: Dict) -> List[InferenceResult]:
         """Generate responses for given prompts."""
         if self.model is None:
             logger.warning("MII client not initialized. Initializing now.")
             self.init_client()
         queries = {"query": prompts}
         start_time = time.time()
+
+        if self.custom_model_config_builder:
+            # if custom model configuration builder available, then do model level input transformation.
+            self.custom_model_config_builder.pre_processing(queries, **params)
+
         try:
             responses = await self.model._request_async_response(queries, **params)
         except Exception as e:
-            raise Exception(
-                json.dumps({"error": "Error in processing request", "exception": str(e)}))
+            raise Exception(json.dumps({"error": "Error in processing request", "exception": str(e)}))
         inference_time_ms = (time.time() - start_time) * 1000
 
         if self.custom_model_config_builder is not None:
             return self.custom_model_config_builder.post_processing(responses, inference_time_ms, prompts=prompts)
 
         inference_results = []  # type: List[InferenceResult]
         return_full_text = params.pop("return_full_text", True)
@@ -217,9 +221,8 @@
                 shutil.copy(os.path.join(src, file), dst)
 
     async def shutdown_async(self):
         """Terminate DS-MII Server."""
         try:
             await self.model.terminate_async()
         except Exception as e:
-            raise Exception(
-                json.dumps({"error": "Error in processing request", "exception": str(e)}))
+            raise Exception(json.dumps({"error": "Error in processing request", "exception": str(e)}))
```

## llm/optimized/inference/engine/vllm_engine.py

```diff
@@ -16,14 +16,15 @@
 import time
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict, List
 
 import requests
 import torch.cuda
 from llm.optimized.inference.configs import EngineConfig, TaskConfig
+from llm.optimized.inference.constants import VLLMSpecialModels
 from llm.optimized.inference.engine import BaseEngine, InferenceResult
 from llm.optimized.inference.logging_config import configure_logger
 from llm.optimized.inference.utils import log_execution_time
 
 logger = configure_logger(__name__)
 
 # fmt: off
@@ -60,14 +61,15 @@
 
     def __init__(self, engine_config: EngineConfig, task_config: TaskConfig):
         """Initialize the VLLMEngine with the given engine and task configurations."""
         self.engine_config: EngineConfig = engine_config
         self.task_config: TaskConfig = task_config
         self._vllm_args: Dict = self.engine_config.vllm_config or {}
         self._model_config: Dict = self.engine_config.model_config or {}
+        self._model_type: str = self._model_config.get("model_type", "")
 
         # Not all vllm arguments require a value
         self._vllm_additional_args: List[str] = []
         self._load_vllm_defaults()
         self._verify_and_convert_float_type()
         self._verify_and_modify_tensor_parallel_size()
 
@@ -97,23 +99,20 @@
             self._vllm_args["tensor-parallel-size"] = (
                 self.engine_config.tensor_parallel
                 if self.engine_config.tensor_parallel is not None
                 else torch.cuda.device_count()
             )
         if "model" not in self._vllm_args:
             self._vllm_args["model"] = self.engine_config.model_id
+
         if "tokenizer" not in self._vllm_args:
             self._vllm_args["tokenizer"] = self.engine_config.tokenizer
 
-        model_type = self._model_config.get("model_type", "")
-
-        # TODO: Remove "RefinedWebModel" and "RefinedWeb" once falcon models are updated to latest huggingface commit
-        if model_type == "falcon" or model_type == "RefinedWebModel" or model_type == "RefinedWeb":
-            self._vllm_args["gpu-memory-utilization"] = 0.95
-            self._vllm_additional_args.append("trust-remote-code")
+        self._vllm_args.update(VLLMSpecialModels.get_kwargs(self._model_type))
+        self._vllm_additional_args.extend(VLLMSpecialModels.get_args(self._model_type))
         self._vllm_additional_args.append("disable-log-requests")
 
     def _verify_and_convert_float_type(self):
         """Check to see whether the model's float type is compatible with the compute type selected.
 
         Bfloat16 is only supported on GPUs such as A100s. V100s do not support bfloat16, only float16.
         Converting from bfloat16 to float16 is ok in this case.
@@ -132,20 +131,22 @@
                     f"of at least 8.0. Your {gpu_name} GPU has compute capability "
                     f"{compute_capability[0]}.{compute_capability[1]}. "
                     f"bfloat16 will be converted to float16.",
                 )
 
     def _verify_and_modify_tensor_parallel_size(self):
         """Check to see if the tensor parallel size is compatible with the models's number of attention heads."""
-        model_type = self._model_config.get("model_type", "")
         num_attention_heads = self._model_config.get("num_attention_heads", 1)
 
         # TODO: Remove if statement once falcon models are updated to latest huggingface commit
-        if model_type == "RefinedWebModel" or model_type == "RefinedWeb":
+        if self._model_type == "RefinedWebModel" or self._model_type == "RefinedWeb":
             num_attention_heads = self._model_config.get("n_head", 1)
+        
+        if self._model_type == "dbrx":
+            num_attention_heads = self._model_config.get("n_heads", 1)
 
         tensor_parallel_size = self._vllm_args["tensor-parallel-size"]
         new_tensor_parallel_size = tensor_parallel_size
         if tensor_parallel_size != 0:
             while num_attention_heads % new_tensor_parallel_size != 0:
                 new_tensor_parallel_size -= 1
         if tensor_parallel_size != new_tensor_parallel_size:
```

