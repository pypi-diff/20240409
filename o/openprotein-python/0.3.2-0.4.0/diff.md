# Comparing `tmp/openprotein_python-0.3.2.tar.gz` & `tmp/openprotein_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.3.2.tar", max compression
+gzip compressed data, was "openprotein_python-0.4.0.tar", max compression
```

## Comparing `openprotein_python-0.3.2.tar` & `openprotein_python-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     6553 2023-08-10 03:05:58.099196 openprotein_python-0.3.2/README.md
--rw-r--r--   0        0        0     2278 2024-03-21 06:21:22.757337 openprotein_python-0.3.2/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.3.2/openprotein/_version.py
--rw-r--r--   0        0        0      147 2024-03-21 05:26:52.241520 openprotein_python-0.3.2/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13238 2023-10-25 10:16:30.071062 openprotein_python-0.3.2/openprotein/api/data.py
--rw-r--r--   0        0        0     8603 2024-03-21 10:29:09.911013 openprotein_python-0.3.2/openprotein/api/design.py
--rw-r--r--   0        0        0    22748 2024-03-22 05:10:47.354575 openprotein_python-0.3.2/openprotein/api/embedding.py
--rw-r--r--   0        0        0     9140 2024-03-22 07:00:11.128371 openprotein_python-0.3.2/openprotein/api/fold.py
--rw-r--r--   0        0        0    10419 2024-03-22 08:34:04.919254 openprotein_python-0.3.2/openprotein/api/jobs.py
--rw-r--r--   0        0        0    40137 2024-03-22 06:41:47.476714 openprotein_python-0.3.2/openprotein/api/poet.py
--rw-r--r--   0        0        0    18331 2024-03-22 08:54:47.522435 openprotein_python-0.3.2/openprotein/api/predict.py
--rw-r--r--   0        0        0    19328 2024-03-21 11:43:40.519972 openprotein_python-0.3.2/openprotein/api/train.py
--rw-r--r--   0        0        0     4070 2024-03-22 08:02:29.424290 openprotein_python-0.3.2/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-07 09:39:52.532056 openprotein_python-0.3.2/openprotein/config.py
--rw-r--r--   0        0        0     1479 2023-09-19 08:42:51.415490 openprotein_python-0.3.2/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.3.2/openprotein/fasta.py
--rw-r--r--   0        0        0     8299 2024-03-22 08:49:02.658493 openprotein_python-0.3.2/openprotein/jobs.py
--rw-r--r--   0        0        0     5588 2024-03-21 08:47:30.852389 openprotein_python-0.3.2/openprotein/models.py
--rw-r--r--   0        0        0     1412 2024-03-22 06:30:40.101576 openprotein_python-0.3.2/openprotein/schemas.py
--rw-r--r--   0        0        0      595 2024-03-22 09:41:17.418340 openprotein_python-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7331 1970-01-01 00:00:00.000000 openprotein_python-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     6547 2024-04-09 02:52:00.438597 openprotein_python-0.4.0/README.md
+-rw-r--r--   0        0        0     2841 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.4.0/openprotein/_version.py
+-rw-r--r--   0        0        0      148 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    25646 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/align.py
+-rw-r--r--   0        0        0    13759 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/data.py
+-rw-r--r--   0        0        0    16169 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/design.py
+-rw-r--r--   0        0        0    33640 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    12214 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/fold.py
+-rw-r--r--   0        0        0    10523 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    18226 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17476 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/predict.py
+-rw-r--r--   0        0        0    18835 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/train.py
+-rw-r--r--   0        0        0     4060 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/base.py
+-rw-r--r--   0        0        0      232 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/config.py
+-rw-r--r--   0        0        0     1479 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.4.0/openprotein/fasta.py
+-rw-r--r--   0        0        0     1889 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/futures.py
+-rw-r--r--   0        0        0     5775 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/jobs.py
+-rw-r--r--   0        0        0     1504 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/schemas.py
+-rw-r--r--   0        0        0      595 2024-04-09 03:30:11.136957 openprotein_python-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 openprotein_python-0.4.0/PKG-INFO
```

### Comparing `openprotein_python-0.3.2/LICENSE.txt` & `openprotein_python-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.3.2/README.md` & `openprotein_python-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 ``` 
 session.jobs.get(JOB_ID)  # Replace JOB_ID with the ID of the specific job to be retrieved
 ```
 
 ### Resuming Jobs
 Jobs from prior workflows can be resumed using the load_job method provided by each API. 
 ```
-session.train.load_job(JOB_ID)  # Replace JOB_ID with the ID of the training job to resume
+session.load_job(JOB_ID)  # Replace JOB_ID with the ID of the training job to resume
 ```
 
 ## PoET interface
 The PoET Interface allows scoring, generating, and retrieving sequences using the PoET model.
 
 ### Scoring Sequences
 To score sequences, use the score function. Provide a prompt and a list of queries. The results will be a list of (sequence, score) pydantic objects.
```

### Comparing `openprotein_python-0.3.2/openprotein/api/data.py` & `openprotein_python-0.4.0/openprotein/api/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 import pandas as pd
 import pydantic
-from typing import Optional, List
+from pydantic import BaseModel
+from typing import Optional, List, Union
+from datetime import datetime
 from io import BytesIO
-
-from openprotein.models import AssayMetadata, AssayDataPage
 from openprotein.errors import APIError
 from openprotein.base import APISession
 import openprotein.config as config
 
 
+class AssayMetadata(BaseModel):
+    assay_name: str
+    assay_description: str
+    assay_id: str
+    original_filename: str
+    created_date: datetime
+    num_rows: int
+    num_entries: int
+    measurement_names: List[str]
+    sequence_length: Optional[int] = None
+
+
+class AssayDataRow(BaseModel):
+    mut_sequence: str
+    measurement_values: List[Union[float, None]]
+
+
+class AssayDataPage(BaseModel):
+    assaymetadata: AssayMetadata
+    page_size: int
+    page_offset: int
+    assaydata: List[AssayDataRow]
+
+
 def list_models(session: APISession, assay_id: str) -> List:
     """
     List models assoicated with assay.
 
     Parameters
     ----------
     session : APISession
@@ -113,15 +137,15 @@
 
     Raises
     ------
     InvalidJob
         If no assay metadata with the specified assay_id is found.
     """
 
-    endpoint = f"v1/assaydata/metadata"
+    endpoint = "v1/assaydata/metadata"
     response = session.get(endpoint, params={"assay_id": assay_id})
     if response.status_code == 200:
         data = pydantic.parse_obj_as(AssayMetadata, response.json())
     else:
         raise APIError(f"Unable to list assay data: {response.text}")
     if data == []:
         raise APIError(f"No assay with id={assay_id} found")
@@ -219,14 +243,15 @@
         return pydantic.parse_obj_as(AssayDataPage, response.json())
     else:
         raise APIError(f"Unable to get assay data page: {response.text}")
 
 
 class AssayDataset:
     """Future Job for manipulating results"""
+
     def __init__(self, session: APISession, metadata: AssayMetadata):
         """
         init for AssayDataset.
 
         Parameters
         ----------
         session : APISession
@@ -460,15 +485,15 @@
         Raises
         ------
         KeyError
             If no assay dataset with the given ID is found.
         """
         return get_assay_metadata(self.session, assay_id)
 
-    def load_job(self, assay_id: str) -> AssayDataset:
+    def load_assay(self, assay_id: str) -> AssayDataset:
         """
         Reload a Submitted job to resume from where you left off!
 
 
         Parameters
         ----------
         assay_id : str
```

### Comparing `openprotein_python-0.3.2/openprotein/api/embedding.py` & `openprotein_python-0.4.0/openprotein/api/embedding.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,127 @@
 from openprotein.base import APISession
-from openprotein.api.jobs import (
-    Job,
-    AsyncJobFuture,
-    MappedAsyncJobFuture,
-    PagedAsyncJobFuture,
-    job_get,
-    load_job
-)
-from openprotein.errors import InvalidJob
+from openprotein.api.jobs import AsyncJobFuture, MappedAsyncJobFuture, job_get
 import openprotein.config as config
-from openprotein.jobs import SVDJob
-from openprotein.models import (
-    ModelDescription,
-    TokenInfo,
-    ModelMetadata,
-    EmbeddedSequence,
-    SVDMetadata,
+from openprotein.jobs import Job, ResultsParser, JobStatus
+from openprotein.api.align import PromptFuture, validate_prompt
+from openprotein.api.poet import (
+    PoetGenerateFuture,
+    poet_score_post,
+    poet_single_site_post,
+    poet_generate_post,
 )
+from openprotein.futures import FutureBase, FutureFactory
 
-from openprotein.jobs import MultiJob
-
-import pydantic
+from pydantic import BaseModel, parse_obj_as
 import numpy as np
-from datetime import datetime
-from base64 import b64decode
-from typing import Optional, List, Tuple, Dict, Union, Any
-from collections import namedtuple
+from typing import Optional, List, Union, Any
 import io
+from datetime import datetime
 
 
 PATH_PREFIX = "v1/embeddings"
 
 
-def embedding_models_get(session: APISession) -> List[str]:
+class ModelDescription(BaseModel):
+    citation_title: Optional[str] = None
+    doi: Optional[str] = None
+    summary: str = "Protein language model for embeddings"
+
+
+class TokenInfo(BaseModel):
+    id: int
+    token: str
+    primary: bool
+    description: str
+
+
+class ModelMetadata(BaseModel):
+    model_id: str
+    description: ModelDescription
+    max_sequence_length: Optional[int] = None
+    dimension: int
+    output_types: List[str]
+    input_tokens: List[str]
+    output_tokens: Optional[List[str]] = None
+    token_descriptions: List[List[TokenInfo]]
+
+
+class EmbeddedSequence(BaseModel):
+    class Config:
+        arbitrary_types_allowed = True
+
+    sequence: bytes
+    embedding: np.ndarray
+
+    def __iter__(self):
+        yield self.sequence
+        yield self.embedding
+
+    def __len__(self):
+        return 2
+
+    def __getitem__(self, i):
+        if i == 0:
+            return self.sequence
+        elif i == 1:
+            return self.embedding
+
+
+class SVDMetadata(BaseModel):
+    id: str
+    status: JobStatus
+    created_date: Optional[datetime] = None
+    model_id: str
+    n_components: int
+    reduction: Optional[str] = None
+    sequence_length: Optional[int] = None
+
+    def is_done(self):
+        return self.status.done()
+
+
+# split these out by module for another layer of control
+class EmbBase:
+    # overridden by subclasses
+    # get correct emb model
+    model_id = None
+
+    @classmethod
+    def get_model(cls):
+        if isinstance(cls.model_id, str):
+            return [cls.model_id]
+        return cls.model_id
+
+
+class EmbFactory:
+    """Factory class for creating Future instances based on job_type."""
+
+    @staticmethod
+    def create_model(session, model_id, default=None):
+        """
+        Create and return an instance of the appropriate Future class based on the job type.
+
+        Returns:
+        - An instance of the appropriate Future class.
+        """
+        # Dynamically discover all subclasses of FutureBase
+        future_classes = EmbBase.__subclasses__()
+
+        # Find the Future class that matches the job type
+        for future_class in future_classes:
+            if model_id in future_class.get_model():
+                return future_class(session=session, model_id=model_id)
+        # default to ProtembedModel
+        try:
+            return default(session=session, model_id=model_id)
+        except Exception:  # type: ignore
+            raise ValueError(f"Unsupported model_id type: {model_id}")
+
+
+def embedding_models_list_get(session: APISession) -> List[str]:
     """
     List available embeddings models.
 
     Args:
         session (APISession): API session
 
     Returns:
@@ -45,26 +130,22 @@
 
     endpoint = PATH_PREFIX + "/models"
     response = session.get(endpoint)
     result = response.json()
     return result
 
 
-# alias embedding_models_list_get to embedding_models_get
-embedding_models_list_get = embedding_models_get
-
-
 def embedding_model_get(session: APISession, model_id: str) -> ModelMetadata:
     endpoint = PATH_PREFIX + f"/models/{model_id}"
     response = session.get(endpoint)
     result = response.json()
     return ModelMetadata(**result)
 
 
-def embedding_get(session: APISession, job_id: str) -> List[bytes]:
+def embedding_get(session: APISession, job_id: str) -> FutureBase:
     """
     Get Job associated with the given request ID.
 
     Parameters
     ----------
     session : APISession
         Session object for API communication.
@@ -72,18 +153,17 @@
         job ID to fetch
 
     Returns
     -------
     sequences : List[bytes]
     """
 
-    endpoint = PATH_PREFIX + f"/{job_id}"
-    response = session.get(endpoint)
-    #return pydantic.parse_obj_as(List[bytes], response.json())
-    return MultiJob.parse_obj(response.json())
+    # endpoint = PATH_PREFIX + f"/{job_id}"
+    # response = session.get(endpoint)
+    return FutureFactory.create_future(session=session, job_id=job_id)
 
 
 def embedding_get_sequences(session: APISession, job_id: str) -> List[bytes]:
     """
     Get results associated with the given request ID.
 
     Parameters
@@ -95,15 +175,15 @@
 
     Returns
     -------
     sequences : List[bytes]
     """
     endpoint = PATH_PREFIX + f"/{job_id}/sequences"
     response = session.get(endpoint)
-    return pydantic.parse_obj_as(List[bytes], response.json())
+    return parse_obj_as(List[bytes], response.json())
 
 
 def embedding_get_sequence_result(
     session: APISession, job_id: str, sequence: bytes
 ) -> bytes:
     """
     Get encoded result for a sequence from the request ID.
@@ -138,26 +218,40 @@
     Returns:
         np.ndarray: decoded array
     """
     s = io.BytesIO(data)
     return np.load(s, allow_pickle=False)
 
 
-class EmbeddingResultFuture(MappedAsyncJobFuture):
+class EmbeddingResultFuture(MappedAsyncJobFuture, FutureBase):
     """Future Job for manipulating results"""
+
+    job_type = [
+        "/embeddings/embed",
+        "/embeddings/svd",
+        "/embeddings/attn",
+        "/embeddings/logits",
+        "/embeddings/embed_reduced",
+        "/svd/fit",
+        "/svd/embed",
+    ]
+
     def __init__(
         self,
         session: APISession,
         job: Job,
         sequences=None,
         max_workers=config.MAX_CONCURRENT_WORKERS,
     ):
         super().__init__(session, job, max_workers)
         self._sequences = sequences
 
+    def get(self, verbose=False) -> List:
+        return super().get(verbose=verbose)
+    
     @property
     def sequences(self):
         if self._sequences is None:
             self._sequences = embedding_get_sequences(self.session, self.job.job_id)
         return self._sequences
 
     @property
@@ -177,57 +271,64 @@
         Returns:
             np.ndarray: embeddings
         """
         data = embedding_get_sequence_result(self.session, self.job.job_id, sequence)
         return decode_embedding(data)
 
 
-def embedding_model_post(session: APISession,
-                         model_id: str,
-                         sequences: List[bytes],
-                         reduction: Optional[str]="MEAN"):
+def embedding_model_post(
+    session: APISession,
+    model_id: str,
+    sequences: List[bytes],
+    reduction: Optional[str] = "MEAN",
+    prompt_id: Optional[str] = None,
+):
     """
     POST a request for embeddings from the given model ID. Returns a Job object referring to this request
     that can be used to retrieve results later.
 
     Parameters
     ----------
     session : APISession
         Session object for API communication.
     model_id : str
         model ID to request results from
     sequences : List[bytes]
         sequences to request results for
     reduction : Optional[str]
         reduction to apply to the embeddings. options are None, "MEAN", or "SUM". defaul: "MEAN"
+    kwargs:
+        accepts prompt_id for Poet Jobs
 
     Returns
     -------
     job : Job
     """
     endpoint = PATH_PREFIX + f"/models/{model_id}/embed"
 
-    if isinstance(sequences[0], bytes):
-        sequences = [s.decode() for s in sequences]
+    sequences_unicode = [
+        (s if isinstance(s, str) else s.decode()) for s in sequences 
+    ]
     body = {
-        "sequences": sequences,
+        "sequences": sequences_unicode,
     }
-    body['reduction'] = reduction
+    if "prompt_id":
+        body["prompt_id"] = prompt_id
+    body["reduction"] = reduction
     response = session.post(endpoint, json=body)
-    return MultiJob.parse_obj(response.json())
-
-
-# alias embedding_post to embedding_model_post
-embedding_post = embedding_model_post
+    return FutureFactory.create_future(
+        session=session, response=response, sequences=sequences
+    )
 
 
 def embedding_model_logits_post(
     session: APISession,
     model_id: str,
-    sequences: List[bytes]
+    sequences: List[bytes],
+    prompt_id: Optional[str] = None,
 ) -> Job:
     """
     POST a request for logits from the given model ID. Returns a Job object referring to this request
     that can be used to retrieve results later.
 
     Parameters
     ----------
@@ -240,26 +341,34 @@
 
     Returns
     -------
     job : Job
     """
     endpoint = PATH_PREFIX + f"/models/{model_id}/logits"
 
-    sequences = [s.decode() for s in sequences]
+    sequences_unicode = [
+        (s if isinstance(s, str) else s.decode()) for s in sequences 
+    ]
     body = {
-        "sequences": sequences,
+        "sequences": sequences_unicode,
     }
+    if "prompt_id":
+        body["prompt_id"] = prompt_id
     response = session.post(endpoint, json=body)
-    return MultiJob.parse_obj(response.json())
+    return FutureFactory.create_future(
+        session=session, response=response, sequences=sequences
+    )
 
 
 def embedding_model_attn_post(
     session: APISession,
     model_id: str,
-    sequences: List[bytes] ) -> Job:
+    sequences: List[bytes],
+    prompt_id: Optional[str] = None,
+) -> Job:
     """
     POST a request for attention embeddings from the given model ID. \
         Returns a Job object referring to this request \
             that can be used to retrieve results later.
 
     Parameters
     ----------
@@ -272,27 +381,33 @@
 
     Returns
     -------
     job : Job
     """
     endpoint = PATH_PREFIX + f"/models/{model_id}/attn"
 
-    sequences = [s.decode() for s in sequences]
+    sequences_unicode = [
+        (s if isinstance(s, str) else s.decode()) for s in sequences 
+    ]
     body = {
-        "sequences": sequences,
+        "sequences": sequences_unicode,
     }
+    if "prompt_id":
+        body["prompt_id"] = prompt_id
     response = session.post(endpoint, json=body)
-    return MultiJob.parse_obj(response.json())
+    return FutureFactory.create_future(
+        session=session, response=response, sequences=sequences
+    )
 
 
 def svd_list_get(session: APISession) -> List[SVDMetadata]:
     """Get SVD job metadata for all SVDs. Including SVD dimension and sequence lengths."""
     endpoint = PATH_PREFIX + "/svd"
     response = session.get(endpoint)
-    return pydantic.parse_obj_as(List[SVDMetadata], response.json())
+    return parse_obj_as(List[SVDMetadata], response.json())
 
 
 def svd_get(session: APISession, svd_id: str) -> SVDMetadata:
     """Get SVD job metadata. Including SVD dimension and sequence lengths."""
     endpoint = PATH_PREFIX + f"/svd/{svd_id}"
     response = session.get(endpoint)
     return SVDMetadata(**response.json())
@@ -311,24 +426,25 @@
 
     Returns
     -------
     bool
     """
 
     endpoint = PATH_PREFIX + f"/svd/{svd_id}"
-    response = session.delete(endpoint)
+    session.delete(endpoint)
     return True
 
 
 def svd_fit_post(
     session: APISession,
     model_id: str,
     sequences: List[bytes],
     n_components: int = 1024,
     reduction: Optional[str] = None,
+    prompt_id: Optional[str] = None,
 ):
     """
     Create SVD fit job.
 
     Parameters
     ----------
     session : APISession
@@ -345,24 +461,28 @@
     Returns
     -------
     SVDJob
     """
 
     endpoint = PATH_PREFIX + "/svd"
 
-    sequences = [s.decode() for s in sequences]
+    sequences_unicode = [(s if isinstance(s, str) else s.decode()) for s in sequences]
     body = {
         "model_id": model_id,
-        "sequences": sequences,
+        "sequences": sequences_unicode,
         "n_components": n_components,
     }
     if reduction is not None:
         body["reduction"] = reduction
+    if prompt_id is not None:
+        body["prompt_id"] = prompt_id
+
     response = session.post(endpoint, json=body)
-    return MultiJob.parse_obj(response.json())
+    # return job for metadata
+    return ResultsParser.parse_obj(response)
 
 
 def svd_embed_post(session: APISession, svd_id: str, sequences: List[bytes]) -> Job:
     """
     POST a request for embeddings from the given SVD model.
 
     Parameters
@@ -376,105 +496,123 @@
 
     Returns
     -------
     Job
     """
     endpoint = PATH_PREFIX + f"/svd/{svd_id}/embed"
 
-    sequences = [s.decode() for s in sequences]
-    body = {"sequences": sequences}
+    sequences_unicode = [
+        (s if isinstance(s, str) else s.decode()) for s in sequences 
+    ]
+    body = {
+        "sequences": sequences_unicode,
+    }
     response = session.post(endpoint, json=body)
-    return MultiJob.parse_obj(response.json())
 
+    return FutureFactory.create_future(
+        session=session, response=response, sequences=sequences
+    )
 
-class ProtembedModel:
+
+class ProtembedModel(EmbBase):
     """
     Class providing inference endpoints for protein embedding models served by OpenProtein.
     """
 
+    model_id = "protembed"
+
     def __init__(self, session, model_id, metadata=None):
         self.session = session
         self.id = model_id
         self._metadata = metadata
+        self.__doc__ = self.__fmt_doc()
+
+    def __fmt_doc(self):
+        summary = str(self.metadata.description.summary)
+        return f"""\t{summary}
+        \t max_sequence_length = {self.metadata.max_sequence_length}
+        \t supported outputs = {self.metadata.output_types}
+        \t supported tokens = {self.metadata.input_tokens} 
+        """
 
     def __str__(self) -> str:
         return self.id
 
     def __repr__(self) -> str:
         return self.id
 
     @property
     def metadata(self):
-        return self.get_metadata()
+        if self._metadata is None:
+            self._metadata = self.get_metadata()
+        return self._metadata
 
     def get_metadata(self) -> ModelMetadata:
         """
         Get model metadata for this model.
 
         Returns
         -------
             ModelMetadata
         """
         if self._metadata is not None:
             return self._metadata
         self._metadata = embedding_model_get(self.session, self.id)
         return self._metadata
 
-    def embed(self, sequences: List[bytes], reduction: Optional[str]="MEAN"):
+    def embed(
+        self, sequences: List[bytes], reduction: Optional[str] = "MEAN"
+    ) -> EmbeddingResultFuture:
         """
         Embed sequences using this model.
 
         Parameters
         ----------
         sequences : List[bytes]
             sequences to SVD
         reduction: str
             embeddings reduction to use (e.g. mean)
 
         Returns
         -------
             EmbeddingResultFuture
         """
-        job = embedding_model_post(self.session,
-                                   model_id=self.id,
-                                   sequences=sequences,
-                                   reduction=reduction)
-        return EmbeddingResultFuture(self.session, job, sequences=sequences)
+        return embedding_model_post(
+            self.session, model_id=self.id, sequences=sequences, reduction=reduction
+        )
 
     def logits(self, sequences: List[bytes]) -> EmbeddingResultFuture:
         """
         logit embeddings for sequences using this model.
 
         Parameters
         ----------
         sequences : List[bytes]
             sequences to SVD
 
         Returns
         -------
             EmbeddingResultFuture
         """
-        job = embedding_model_logits_post(self.session, self.id, sequences)
-        return EmbeddingResultFuture(self.session, job, sequences=sequences)
+        return embedding_model_logits_post(self.session, self.id, sequences)
 
     def attn(self, sequences: List[bytes]) -> EmbeddingResultFuture:
         """
         Attention embeddings for sequences using this model.
 
         Parameters
         ----------
         sequences : List[bytes]
             sequences to SVD
 
         Returns
         -------
             EmbeddingResultFuture
         """
-        job = embedding_model_attn_post(self.session, self.id, sequences)
-        return EmbeddingResultFuture(self.session, job, sequences=sequences)
+        return embedding_model_attn_post(self.session, self.id, sequences)
 
     def fit_svd(
         self,
         sequences: List[bytes],
         n_components: int = 1024,
         reduction: Optional[str] = None,
     ) -> Any:
@@ -501,24 +639,31 @@
         job = svd_fit_post(
             self.session,
             model_id,
             sequences,
             n_components=n_components,
             reduction=reduction,
         )
-        metadata = svd_get(self.session, job.job_id)
+        if isinstance(job, Job):
+            job_id = job.job_id
+        else:
+            job_id = job.job.job_id
+        metadata = svd_get(self.session, job_id)
         return SVDModel(self.session, metadata)
 
 
-class SVDModel(AsyncJobFuture):
+class SVDModel(AsyncJobFuture, FutureBase):
     """
     Class providing embedding endpoint for SVD models. \
         Also allows retrieving embeddings of sequences used to fit the SVD with `get`.
     """
 
+    # actually a future, not a model!
+    job_type = "/svd"
+
     def __init__(self, session: APISession, metadata: SVDMetadata):
         self.session = session
         self._metadata = metadata
         self._job = None
 
     def __str__(self) -> str:
         return str(self.metadata)
@@ -565,19 +710,19 @@
         Delete this SVD model.
         """
         return svd_delete(self.session, self.id)
 
     def get_job(self) -> Job:
         """Get job associated with this SVD model"""
         return job_get(self.session, self.id)
-    
+
     def get(self):
         # overload for AsyncJobFuture
         return self
-    
+
     @property
     def job(self) -> Job:
         if self._job is None:
             self._job = self.get_job()
         return self._job
 
     @job.setter
@@ -602,46 +747,351 @@
         -------
             EmbeddingResultFuture: class for futher job manipulation
         """
         return EmbeddingResultFuture(self.session, self.get_job())
 
     def embed(self, sequences: List[bytes]) -> EmbeddingResultFuture:
         """
-        Use this SVD model to reduce embeddings results. 
+        Use this SVD model to reduce embeddings results.
 
         Parameters
         ----------
         sequences : List[bytes]
             List of protein sequences.
 
         Returns
         -------
         EmbeddingResultFuture
             Class for further job manipulation.
         """
-        job = svd_embed_post(self.session, self.id, sequences)
-        return EmbeddingResultFuture(self.session, job, sequences=sequences)
+        return svd_embed_post(self.session, self.id, sequences)
+        # return EmbeddingResultFuture(self.session, job, sequences=sequences)
+
+
+class OpenProteinModel(ProtembedModel):
+    """
+    Class providing inference endpoints for proprietary protein embedding models served by OpenProtein.
+
+    Examples
+    --------
+    View specific model details (inc supported tokens) with the `?` operator.
+
+    .. code-block:: python
+
+        import openprotein
+        session = openprotein.connect(username="user", password="password")
+        session.embedding.prot_seq?
+    """
+
+
+class PoETModel(OpenProteinModel, EmbBase):
+    """
+    Class for OpenProtein's foundation model PoET - NB. PoET functions are dependent on a prompt supplied via the align endpoints.
+
+    Examples
+    --------
+    View specific model details (inc supported tokens) with the `?` operator.
+
+    .. code-block:: python
+
+        import openprotein
+        session = openprotein.connect(username="user", password="password")
+        session.embedding.poet?
+
+
+    """
+
+    model_id = "poet"
+
+    # Add model to explicitly require prompt_id
+    def __init__(self, session, model_id, metadata=None):
+        self.session = session
+        self.id = model_id
+        self._metadata = metadata
+        # could add prompt here?
+
+    def embed(
+        self,
+        prompt: Union[str, PromptFuture],
+        sequences: List[bytes],
+        reduction: Optional[str] = "MEAN",
+    ) -> EmbeddingResultFuture:
+        """
+        Embed sequences using this model.
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        sequence : bytes
+            Sequence to embed.
+        reduction: str
+            embeddings reduction to use (e.g. mean)
+        Returns
+        -------
+            EmbeddingResultFuture
+        """
+        prompt_id = validate_prompt(prompt)
+        # return super().embed(sequences=sequences, reduction=reduction, prompt_id=prompt_id)
+        return embedding_model_post(
+            self.session,
+            model_id=self.id,
+            sequences=sequences,
+            prompt_id=prompt_id,
+            reduction=reduction,
+        )
+
+    def logits(
+        self,
+        prompt: Union[str, PromptFuture],
+        sequences: List[bytes],
+    ) -> EmbeddingResultFuture:
+        """
+        logit embeddings for sequences using this model.
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        sequence : bytes
+            Sequence to analyse.
+
+        Returns
+        -------
+            EmbeddingResultFuture
+        """
+        prompt_id = validate_prompt(prompt)
+        # return super().logits(sequences=sequences, prompt_id=prompt_id)
+        return embedding_model_logits_post(
+            self.session, self.id, sequences=sequences, prompt_id=prompt_id
+        )
+
+    def attn():
+        """Not Available for Poet."""
+        raise ValueError("Attn not yet supported for poet")
+
+    def score(self, prompt: Union[str, PromptFuture], sequences: List[bytes]):
+        """
+        Score query sequences using the specified prompt.
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        sequence : bytes
+            Sequence to analyse.
+        Returns
+        -------
+        results
+            The scores of the query sequences.
+        """
+        prompt_id = validate_prompt(prompt)
+        return poet_score_post(self.session, prompt_id, sequences)
+
+    def single_site(self, prompt: Union[str, PromptFuture], sequence: bytes):
+        """
+        Score all single substitutions of the query sequence using the specified prompt.
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        sequence : bytes
+            Sequence to analyse.
+        Returns
+        -------
+        results
+            The scores of the mutated sequence.
+        """
+        prompt_id = validate_prompt(prompt)
+        return poet_single_site_post(self.session, sequence, prompt_id=prompt_id)
+
+    def generate(
+        self,
+        prompt: Union[str, PromptFuture],
+        num_samples=100,
+        temperature=1.0,
+        topk=None,
+        topp=None,
+        max_length=1000,
+        seed=None,
+    ) -> PoetGenerateFuture:
+        """
+        Generate protein sequences conditioned on a prompt.
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        num_samples : int, optional
+            The number of samples to generate, by default 100.
+        temperature : float, optional
+            The temperature for sampling. Higher values produce more random outputs, by default 1.0.
+        topk : int, optional
+            The number of top-k residues to consider during sampling, by default None.
+        topp : float, optional
+            The cumulative probability threshold for top-p sampling, by default None.
+        max_length : int, optional
+            The maximum length of generated proteins, by default 1000.
+        seed : int, optional
+            Seed for random number generation, by default a random number.
+
+        Raises
+        ------
+        APIError
+            If there is an issue with the API request.
+
+        Returns
+        -------
+        Job
+            An object representing the status and information about the generation job.
+        """
+        prompt_id = validate_prompt(prompt)
+        return poet_generate_post(
+            self.session,
+            prompt_id,
+            num_samples=num_samples,
+            temperature=temperature,
+            topk=topk,
+            topp=topp,
+            max_length=max_length,
+            random_seed=seed,
+        )
+
+    def fit_svd(
+        self,
+        prompt: Union[str, PromptFuture],
+        sequences: List[bytes],
+        n_components: int = 1024,
+        reduction: Optional[str] = None,
+    ) -> SVDModel:
+        """
+        Fit an SVD on the embedding results of this model. 
+
+        This function will create an SVDModel based on the embeddings from this model \
+            as well as the hyperparameters specified in the args.  
+
+        Parameters
+        ----------
+        prompt: Union[str, PromptFuture]
+            prompt from an align workflow to condition Poet model
+        sequences : List[bytes] 
+            sequences to SVD
+        n_components: int 
+            number of components in SVD. Will determine output shapes
+        reduction: str
+            embeddings reduction to use (e.g. mean)
+
+
+        Returns
+        -------
+            SVDModel
+        """
+        prompt = validate_prompt(prompt)
+
+        job = svd_fit_post(
+            self.session,
+            model_id=self.id,
+            sequences=sequences,
+            n_components=n_components,
+            reduction=reduction,
+            prompt_id=prompt,
+        )
+        metadata = svd_get(self.session, job.job_id)
+        return SVDModel(self.session, metadata)
+
+
+class ESMModel(ProtembedModel):
+    """
+    Class providing inference endpoints for Facebook's ESM protein language Models.
+
+    Examples
+    --------
+    View specific model details (inc supported tokens) with the `?` operator.
+
+    .. code-block:: python
+
+        import openprotein
+        session = openprotein.connect(username="user", password="password")
+        session.embedding.esm2_t12_35M_UR50D?"""
 
 
 class EmbeddingAPI:
     """
     This class defines a high level interface for accessing the embeddings API.
-    """
+
+    You can access all our models either via :meth:`get_model` or directly through the session's embedding attribute using the model's ID and the desired method. For example, to use the attention method on the protein sequence model, you would use ``session.embedding.prot_seq.attn()``.
+
+    Examples
+    --------
+    Accessing a model's method:
+
+    .. code-block:: python
+
+        # To call the attention method on the protein sequence model:
+        import openprotein
+        session = openprotein.connect(username="user", password="password")
+        session.embedding.prot_seq.attn()
+
+    Using the `get_model` method:
+
+    .. code-block:: python
+
+        # Get a model instance by name:
+        import openprotein
+        session = openprotein.connect(username="user", password="password")
+        # list available models:
+        print(session.embedding.list_models() )
+        # init model by name
+        model = session.embedding.get_model('prot-seq')
+    """
+
+    # added for static typing, eg pylance, for autocomplete
+    # at init these are all overwritten.
+    prot_seq: OpenProteinModel
+    rotaprot_large_uniref50w: OpenProteinModel
+    rotaprot_large_uniref90_ft: OpenProteinModel
+    poet: PoETModel
+
+    esm1b_t33_650M_UR50S: ESMModel
+    esm1v_t33_650M_UR90S_1: ESMModel
+    esm1v_t33_650M_UR90S_2: ESMModel
+    esm1v_t33_650M_UR90S_3: ESMModel
+    esm1v_t33_650M_UR90S_4: ESMModel
+    esm1v_t33_650M_UR90S_5: ESMModel
+    esm2_t12_35M_UR50D: ESMModel
+    esm2_t30_150M_UR50D: ESMModel
+    esm2_t33_650M_UR50D: ESMModel
+    esm2_t36_3B_UR50D: ESMModel
+    esm2_t6_8M_UR50D: ESMModel
 
     def __init__(self, session: APISession):
         self.session = session
+        # dynamically add models from  api list
+        self._load_models()
+
+    def _load_models(self):
+        # Dynamically add model instances as attributes - precludes any drift
+        models = self.list_models()
+        for model in models:
+            model_name = model.id.replace("-", "_")  # hyphens out
+            setattr(self, model_name, model)
 
     def list_models(self) -> List[ProtembedModel]:
         """list models available for creating embeddings of your sequences"""
         models = []
         for model_id in embedding_models_list_get(self.session):
-            models.append(ProtembedModel(self.session, model_id))
+            models.append(
+                EmbFactory.create_model(
+                    session=self.session, model_id=model_id, default=ProtembedModel
+                )
+            )
         return models
 
-    def get_model(self, model_id: str) -> ProtembedModel:
+    def get_model(self, name: str):
         """
         Get model by model_id. 
 
         ProtembedModel allows all the usual job manipulation: \
             e.g. making POST and GET requests for this model specifically. 
 
 
@@ -656,83 +1106,41 @@
             The model
 
         Raises
         ------
         HTTPError
             If the GET request does not succeed.
         """
-        return ProtembedModel(self.session, model_id)
-
-    def embed(self,
-              model: Union[ProtembedModel,SVDModel, str],
-                           sequences: List[bytes],
-                           reduction="MEAN"):
-        """
-        Embed sequences using the specified model.
-
-        Parameters
-        ----------
-        model : Union[ProtembedModel, SVDModel, str]
-            The model to use for embedding. This can be an instance of ProtembedModel, SVDModel,
-            or a string representing the model_id.
-        sequences : List[bytes]
-            List of byte sequences to be embedded.
-        reduction : str, optional
-            The reduction operation to be applied on the embeddings.
-            Options are None, "MEAN", or "SUM". Default is None.
-
-        Returns
-        -------
-        EmbeddingResultFuture
-            An instance of EmbeddingResultFuture
-
-        Raises
-        ------
-        TypeError
-            If the input model is neither ProtembedModel, SVDModel, nor str.
-        """
-        if isinstance(model, ProtembedModel):
-            model_id = model.id
-            job = embedding_model_post(
-                self.session, model_id, sequences, reduction=reduction
-            )
-        elif isinstance(model, SVDModel):
-            svd_id = model.id
-            job = svd_embed_post(self.session, svd_id, sequences)
-        else:
-            # we assume model is the model_id
-            model_id = model
-            job = embedding_model_post(
-                self.session, model_id, sequences, reduction=reduction
-            )
-        return EmbeddingResultFuture(self.session, job, sequences=sequences)
+        model_name = name.replace("-", "_")
+        return getattr(self, model_name)
 
-    def get_results(self, job) -> EmbeddingResultFuture:
+    def __get_results(self, job) -> EmbeddingResultFuture:
         """
         Retrieves the results of an embedding job.
 
         Parameters
         ----------
         job : Job
             The embedding job whose results are to be retrieved.
 
         Returns
         -------
         EmbeddingResultFuture
             An instance of EmbeddingResultFuture
         """
-        return EmbeddingResultFuture(self.session, job)
+        return FutureFactory.create_future(job=job, session=self.session)
 
-    def fit_svd(
+    def __fit_svd(
         self,
         model_id: str,
         sequences: List[bytes],
         n_components: int = 1024,
         reduction: Optional[str] = None,
-    ):
+        **kwargs,
+    ) -> SVDModel:
         """
         Fit an SVD on the sequences with the specified model_id and hyperparameters (n_components).
 
         Parameters
         ----------
         model_id : str
             The ID of the model to fit the SVD on.
@@ -746,15 +1154,18 @@
         Returns
         -------
         SVDModel
             The model with the SVD fit.
         """
         model = self.get_model(model_id)
         return model.fit_svd(
-            sequences=sequences, n_components=n_components, reduction=reduction
+            sequences=sequences,
+            n_components=n_components,
+            reduction=reduction,
+            **kwargs,
         )
 
     def get_svd(self, svd_id: str) -> SVDModel:
         """
         Get SVD job results. Including SVD dimension and sequence lengths.
 
         Requires a successful SVD job from fit_svd
@@ -767,15 +1178,15 @@
         -------
         SVDModel
             The model with the SVD fit.
         """
         metadata = svd_get(self.session, svd_id)
         return SVDModel(self.session, metadata)
 
-    def delete_svd(self, svd_id: str) -> bool:
+    def __delete_svd(self, svd_id: str) -> bool:
         """
         Delete SVD model.
 
         Parameters
         ----------
         svd_id : str
             The ID of the SVD  job.
@@ -799,15 +1210,15 @@
             SVDModels
 
         """
         return [
             SVDModel(self.session, metadata) for metadata in svd_list_get(self.session)
         ]
 
-    def get_svd_results(self, job: Job):
+    def __get_svd_results(self, job: Job):
         """
         Get SVD job results. Including SVD dimension and sequence lengths.
 
         Requires a successful SVD job from fit_svd
 
         Parameters
         ----------
@@ -815,40 +1226,7 @@
             SVD JobFuture
         Returns
         -------
         SVDModel
             The model with the SVD fit.
         """
         return EmbeddingResultFuture(self.session, job)
-
-    def load_job(self, job_id: str) -> Job:
-        """
-        Reload a Submitted job to resume from where you left off!
-
-
-        Parameters
-        ----------
-        job_id : str
-            The identifier of the job whose details are to be loaded.
-
-        Returns
-        -------
-        Job
-            Job
-
-        Raises
-        ------
-        HTTPError
-            If the request to the server fails.
-        InvalidJob
-            If the Job is of the wrong type
-
-        """
-        job_details = load_job(self.session, job_id)
-        sequences = embedding_get_sequences(self.session, job_id=job_id)
-        if "embed" not in job_details.job_type:
-            raise InvalidJob(
-                f"Job {job_id} is of type {job_details.job_type} not embeddings"
-            )
-        if len(sequences) == 0:
-            raise InvalidJob(f"Unable to load sequences for job {job_id}")
-        return EmbeddingResultFuture(self.session, job_details, sequences=sequences)
```

### Comparing `openprotein_python-0.3.2/openprotein/api/jobs.py` & `openprotein_python-0.4.0/openprotein/api/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # Jobs and job centric flows
 
 
-from datetime import datetime
-from typing import List, Optional, Union
+from typing import List, Union
 import concurrent.futures
 import time
-from enum import Enum
 
 import tqdm
 import pydantic
-from pydantic import BaseModel, ConfigDict
 
-from openprotein.errors import TimeoutException
 from openprotein.base import APISession
 import openprotein.config as config
-from openprotein.jobs import job_get, MultiJob, Job
+from openprotein.jobs import job_get, ResultsParser, Job
+from openprotein.futures import FutureFactory
 
 
-def load_job(session: APISession, job_id: str) -> MultiJob:
+def load_job(session: APISession, job_id: str) -> FutureFactory:
     """
     Reload a Submitted job to resume from where you left off!
 
 
     Parameters
     ----------
     session : APISession
@@ -36,26 +33,24 @@
 
     Raises
     ------
     HTTPError
         If the request to the server fails.
 
     """
-    endpoint = f"v1/jobs/{job_id}"
-    response = session.get(endpoint)
-    return MultiJob.parse_obj(response.json())
+    return FutureFactory.create_future(session=session, job_id=job_id)
 
 
 def jobs_list(
     session: APISession,
     status=None,
     job_type=None,
     assay_id=None,
     more_recent_than=None,
-) -> List[MultiJob]:
+) -> List[Job]:
     """
     Retrieve a list of jobs filtered by specific criteria.
 
     Parameters
     ----------
     session : APISession
         The current API session for communication with the server.
@@ -82,65 +77,73 @@
         params["job_type"] = job_type
     if assay_id is not None:
         params["assay_id"] = assay_id
     if more_recent_than is not None:
         params["more_recent_than"] = more_recent_than
 
     response = session.get(endpoint, params=params)
-    return pydantic.parse_obj_as(List[MultiJob], response.json())
+    # return jobs, not futures
+    return pydantic.parse_obj_as(List[ResultsParser], response.json())
 
 
 class JobsAPI:
     """API wrapper to get jobs."""
 
+    # This will continue to get jobs, not futures.
+
     def __init__(self, session: APISession):
         self.session = session
 
     def list(
         self, status=None, job_type=None, assay_id=None, more_recent_than=None
-    ) -> List[MultiJob]:
-        """ List jobs"""
+    ) -> List[Job]:
+        """List jobs"""
         return jobs_list(
             self.session,
             status=status,
             job_type=job_type,
             assay_id=assay_id,
             more_recent_than=more_recent_than,
         )
 
-    def get(self, job_id) -> MultiJob:
+    def get(self, job_id) -> Job:
         """get Job by ID"""
-        return job_get(self.session, job_id)
+        return load_job(self.session, job_id)
+        # return job_get(self.session, job_id)
+
+    def __load(self, job_id) -> FutureFactory:
+        return load_job(self.session, job_id)
 
     def wait(
-        self, job: MultiJob, interval=config.POLLING_INTERVAL, timeout=None, verbose=False
+        self, job: Job, interval=config.POLLING_INTERVAL, timeout=None, verbose=False
     ):
         return job.wait(
             self.session, interval=interval, timeout=timeout, verbose=verbose
         )
 
 
 class AsyncJobFuture:
-    def __init__(self, session: APISession, job: Union[MultiJob, str]):
+    def __init__(self, session: APISession, job: Union[Job, str]):
         if isinstance(job, str):
             job = job_get(session, job)
         self.session = session
         self.job = job
 
     def refresh(self):
-        """ refresh job status"""
+        """refresh job status"""
         self.job = self.job.refresh(self.session)
 
     @property
     def status(self):
         return self.job.status
 
     @property
     def progress(self):
         return self.job.progress_counter or 0
+
     @property
     def num_records(self):
         return self.job.num_records
 
     def done(self):
         return self.job.done()
 
@@ -166,53 +169,58 @@
         """
         job = self.job.wait(
             self.session, interval=interval, timeout=timeout, verbose=verbose
         )
         self.job = job
         return self.done()
 
-    def wait(self, interval: int=config.POLLING_INTERVAL, timeout: int=None, verbose:bool=False):
+    def wait(
+        self,
+        interval: int = config.POLLING_INTERVAL,
+        timeout: int = None,
+        verbose: bool = False,
+    ):
         """
         Wait for job to complete, then fetch results.
 
         Args:
             interval (int, optional): time between polling. Defaults to config.POLLING_INTERVAL.
             timeout (int, optional): max time to wait. Defaults to None.
             verbose (bool, optional): verbosity flag. Defaults to False.
 
         Returns:
             results: results of job
         """
-        time.sleep(1) # buffer for BE to register job
+        time.sleep(1)  # buffer for BE to register job
         job = self.job.wait(
             self.session, interval=interval, timeout=timeout, verbose=verbose
         )
         self.job = job
         return self.get(verbose=verbose)
 
 
 class StreamingAsyncJobFuture(AsyncJobFuture):
     def stream(self):
         raise NotImplementedError()
 
-    def get(self, verbose=False):
+    def get(self, verbose=False) -> List:
         generator = self.stream()
         if verbose:
             total = None
             if hasattr(self, "__len__"):
                 total = len(self)
             generator = tqdm.tqdm(
                 generator, desc="Retrieving", total=total, position=0, mininterval=1.0
             )
         return [entry for entry in generator]
 
 
 class MappedAsyncJobFuture(StreamingAsyncJobFuture):
     def __init__(
-        self, session: APISession, job: MultiJob, max_workers=config.MAX_CONCURRENT_WORKERS
+        self, session: APISession, job: Job, max_workers=config.MAX_CONCURRENT_WORKERS
     ):
         """
         Retrieve results from asynchronous, mapped endpoints. Use `max_workers` > 0 to enable concurrent retrieval of multiple pages.
         """
         super().__init__(session, job)
         self.max_workers = max_workers
         self._cache = {}
@@ -268,15 +276,15 @@
 
 class PagedAsyncJobFuture(StreamingAsyncJobFuture):
     DEFAULT_PAGE_SIZE = 1024
 
     def __init__(
         self,
         session: APISession,
-        job: MultiJob,
+        job: Job,
         page_size=None,
         num_records=None,
         max_workers=config.MAX_CONCURRENT_WORKERS,
     ):
         """
         Retrieve results from asynchronous, paged endpoints. Use `max_workers` > 0 to enable concurrent retrieval of multiple pages.
         """
```

### Comparing `openprotein_python-0.3.2/openprotein/api/poet.py` & `openprotein_python-0.4.0/openprotein/api/align.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,88 @@
-from typing import Optional, List, Union, BinaryIO, Iterator
+from typing import Iterator, Optional, List, BinaryIO, Literal, Union
+from pydantic import BaseModel, Field, validator, root_validator
+from enum import Enum
 from io import BytesIO
 import random
 import csv
 import codecs
 import requests
 
 from openprotein.base import APISession
 from openprotein.api.jobs import (
     AsyncJobFuture,
-    StreamingAsyncJobFuture,
 )
 
-from openprotein.jobs import MultiJob, JobType,JobStatus, job_get, job_args_get
-
-from openprotein.api.jobs import load_job #as base_load_job
-import openprotein.config as config
-
-from openprotein.models import (
-    MSASamplingMethod,
-    PoetInputType,
-    PoetScoreResult,
-    PoetSSPResult,
+from openprotein.jobs import (
+    ResultsParser,
+    Job,
+    register_job_type,
+    JobType,
+    job_args_get,
 )
 
-from openprotein.jobs import MultiJob, JobType
+import openprotein.config as config
 
 from openprotein.errors import (
     InvalidParameterError,
     MissingParameterError,
     APIError,
-    InvalidJob,
 )
+from openprotein.futures import FutureBase, FutureFactory
+
 
+class PoetInputType(str, Enum):
+    INPUT = "RAW"
+    MSA = "GENERATED"
+    PROMPT = "PROMPT"
+
+
+class MSASamplingMethod(str, Enum):
+    RANDOM = "RANDOM"
+    NEIGHBORS = "NEIGHBORS"
+    NEIGHBORS_NO_LIMIT = "NEIGHBORS_NO_LIMIT"
+    NEIGHBORS_NONGAP_NORM_NO_LIMIT = "NEIGHBORS_NONGAP_NORM_NO_LIMIT"
+    TOP = "TOP"
+
+
+class PromptPostParams(BaseModel):
+    msa_id: str
+    num_sequences: Optional[int] = Field(None, ge=0, lt=100)
+    num_residues: Optional[int] = Field(None, ge=0, lt=24577)
+    method: MSASamplingMethod = MSASamplingMethod.NEIGHBORS_NONGAP_NORM_NO_LIMIT
+    homology_level: float = Field(0.8, ge=0, le=1)
+    max_similarity: float = Field(1.0, ge=0, le=1)
+    min_similarity: float = Field(0.0, ge=0, le=1)
+    always_include_seed_sequence: bool = False
+    num_ensemble_prompts: int = 1
+    random_seed: Optional[int] = None
+
+
+@register_job_type(JobType.align_align)
+class MSAJob(Job):
+    msa_id: Optional[str] = None
+    job_type: Literal[JobType.align_align] = JobType.align_align
+
+    @root_validator
+    def set_msa_id(cls, values):
+        if not values.get("msa_id"):
+            values["msa_id"] = values.get("job_id")
+        return values
+
+
+@register_job_type(JobType.align_prompt)
+class PromptJob(MSAJob):
+    prompt_id: Optional[str] = None
+    job_type: Literal[JobType.align_prompt] = JobType.align_prompt
+
+    @root_validator
+    def set_prompt_id(cls, values):
+        if not values.get("prompt_id"):
+            values["prompt_id"] = values.get("job_id")
+        return values
 
 
 def csv_stream(response: requests.Response) -> csv.reader:
     """
     Returns a CSV reader from a requests.Response object.
 
     Parameters
@@ -92,15 +139,15 @@
 
     response = session.get(endpoint, params=params, stream=True)
     return response
 
 
 def get_input(
     self: APISession,
-    job: MultiJob,
+    job: Job,
     input_type: PoetInputType,
     prompt_index: Optional[int] = None,
 ) -> csv.reader:
     """
     Get input data for a given job.
 
     Parameters
@@ -121,15 +168,15 @@
     """
     job_id = job.job_id
     response = get_align_job_inputs(self, job_id, input_type, prompt_index=prompt_index)
     return csv_stream(response)
 
 
 def get_prompt(
-    self: APISession, job: MultiJob, prompt_index: Optional[int] = None
+    self: APISession, job: Job, prompt_index: Optional[int] = None
 ) -> csv.reader:
     """
     Get the prompt for a given job.
 
     Parameters
     ----------
     self : APISession
@@ -143,15 +190,15 @@
     -------
     csv.reader
         A CSV reader for the prompt data.
     """
     return get_input(self, job, PoetInputType.PROMPT, prompt_index=prompt_index)
 
 
-def get_seed(self: APISession, job: MultiJob) -> csv.reader:
+def get_seed(self: APISession, job: Job) -> csv.reader:
     """
     Get the seed for a given MSA job.
 
     Parameters
     ----------
     self : APISession
         The API session.
@@ -162,15 +209,15 @@
     -------
     csv.reader
         A CSV reader for the seed sequence.
     """
     return get_input(self, job, PoetInputType.INPUT)
 
 
-def get_msa(self: APISession, job: MultiJob) -> csv.reader:
+def get_msa(self: APISession, job: Job) -> csv.reader:
     """
     Get the generated MSA (Multiple Sequence Alignment) for a given job.
 
     Parameters
     ----------
     self : APISession
         The API session.
@@ -223,30 +270,30 @@
         msa_file = BytesIO(b"\n".join([b">seed", seed]))
         is_seed = True
 
     params = {"is_seed": is_seed}
     files = {"msa_file": msa_file}
 
     response = session.post(endpoint, files=files, params=params)
-    return MultiJob.parse_obj(response.json() )
+    return FutureFactory.create_future(session=session, response=response)
 
 
 def prompt_post(
     session: APISession,
     msa_id: str,
     num_sequences: Optional[int] = None,
     num_residues: Optional[int] = None,
     method: MSASamplingMethod = MSASamplingMethod.NEIGHBORS_NONGAP_NORM_NO_LIMIT,
     homology_level: float = 0.8,
     max_similarity: float = 1.0,
     min_similarity: float = 0.0,
     always_include_seed_sequence: bool = False,
     num_ensemble_prompts: int = 1,
     random_seed: Optional[int] = None,
-):
+) -> PromptJob:
     """
     Create a protein sequence prompt from a linked MSA (Multiple Sequence Alignment) for PoET Jobs.
 
     The MSA is specified by msa_id and created in msa_post.
 
     Parameters
     ----------
@@ -324,21 +371,21 @@
     }
     if num_sequences is not None:
         params["max_msa_sequences"] = num_sequences
     if num_residues is not None:
         params["max_msa_tokens"] = num_residues
 
     response = session.post(endpoint, params=params)
-    return MultiJob.parse_obj(response.json() )
+    return FutureFactory.create_future(session=session, response=response)
 
 
 def upload_prompt_post(
     session: APISession,
     prompt_file: BinaryIO,
-) -> MultiJob:
+):
     """
     Directly upload a prompt.
 
     Bypass post_msa and prompt_post steps entirely. In this case PoET will use the prompt as is.
     You can specify multiple prompts (one per replicate) with an `<END_PROMPT>\n` between CSVs.
 
     Parameters
@@ -359,22 +406,20 @@
         An object representing the status and results of the prompt job.
     """
 
     endpoint = "v1/poet/align/upload_prompt"
     files = {"prompt_file": prompt_file}
     try:
         response = session.post(endpoint, files=files)
-        return MultiJob.parse_obj(response.json() )
+        return FutureFactory.create_future(session=session, response=response)
     except Exception as exc:
         raise APIError(f"Failed to upload prompt post: {exc}") from exc
 
 
-def poet_score_post(
-    session: APISession, prompt_id: str, queries: List[bytes]
-) -> MultiJob:
+def poet_score_post(session: APISession, prompt_id: str, queries: List[bytes]):
     """
     Submits a job to score sequences based on the given prompt.
 
     Parameters
     ----------
     session : APISession
         An instance of APISession to manage interactions with the API.
@@ -404,15 +449,15 @@
         queries = [i.encode() for i in queries]
     try:
         variant_file = BytesIO(b"\n".join(queries))
         params = {"prompt_id": prompt_id}
         response = session.post(
             endpoint, files={"variant_file": variant_file}, params=params
         )
-        return MultiJob.parse_obj(response.json() )
+        return FutureFactory.create_future(session=session, response=response)
     except Exception as exc:
         raise APIError(f"Failed to post poet score: {exc}") from exc
 
 
 def poet_score_get(
     session: APISession, job_id, page_size=config.POET_PAGE_SIZE, page_offset=0
 ):
@@ -448,20 +493,20 @@
         )
 
     response = session.get(
         endpoint,
         params={"job_id": job_id, "page_size": page_size, "page_offset": page_offset},
     )
 
-    return MultiJob.parse_obj(response.json() )
+    return FutureFactory.create_future(session=session, response=response)
 
 
-class PoetFutureMixin:
+class AlignFutureMixin:
     session: APISession
-    job: MultiJob
+    job: Job
 
     def get_input(self, input_type: PoetInputType):
         """See child function docs."""
         return get_input(self.session, self.job, input_type)
 
     def get_prompt(self, prompt_index: Optional[int] = None):
         """See child function docs."""
@@ -476,15 +521,15 @@
         return get_msa(self.session, self.job)
 
     @property
     def id(self):
         return self.job.job_id
 
 
-class MSAFuture(PoetFutureMixin, AsyncJobFuture):
+class MSAFuture(AlignFutureMixin, AsyncJobFuture, FutureBase):
     """
     Represents a result of a MSA job.
 
     Attributes
     ----------
     session : APISession
         An instance of APISession for API interactions.
@@ -500,15 +545,17 @@
 
     Returns
     -------
     List[PoetScoreResult]
         The list of results from the PoET scoring job.
     """
 
-    def __init__(self, session: APISession, job: MultiJob, page_size=config.POET_PAGE_SIZE):
+    job_type = "/align/align"
+
+    def __init__(self, session: APISession, job: Job, page_size=config.POET_PAGE_SIZE):
         """
         init a PoetScoreFuture instance.
 
         Parameters
         ----------
         session : APISession
             An instance of APISession for API interactions.
@@ -524,15 +571,15 @@
         self._prompt_id = None
 
     def __str__(self) -> str:
         return str(self.job)
 
     def __repr__(self) -> str:
         return repr(self.job)
-    
+
     @property
     def id(self):
         return self.job.job_id
 
     @property
     def prompt_id(self):
         if self.job.job_type == "/align/prompt" and self._prompt_id is None:
@@ -542,35 +589,37 @@
     @property
     def msa_id(self):
         if self.job.job_type == "/align/align" and self._msa_id is None:
             self._msa_id = self.job.job_id
         return self._msa_id
 
     def wait(self, verbose: bool = False):
-        _ = self.job.wait(self.session,
-                             interval=config.POLLING_INTERVAL,
-                             timeout=config.POLLING_TIMEOUT,
-                             verbose=False)  # no progress to track
+        _ = self.job.wait(
+            self.session,
+            interval=config.POLLING_INTERVAL,
+            timeout=config.POLLING_TIMEOUT,
+            verbose=False,
+        )  # no progress to track
         return self.get()
 
-    def get(self, verbose: bool = False):
+    def get(self, verbose: bool = False) -> csv.reader:
         return self.get_msa()
 
     def sample_prompt(
         self,
         num_sequences: Optional[int] = None,
         num_residues: Optional[int] = None,
         method: MSASamplingMethod = MSASamplingMethod.NEIGHBORS_NONGAP_NORM_NO_LIMIT,
         homology_level: float = 0.8,
         max_similarity: float = 1.0,
         min_similarity: float = 0.0,
         always_include_seed_sequence: bool = False,
         num_ensemble_prompts: int = 1,
         random_seed: Optional[int] = None,
-    ):
+    ) -> PromptJob:
         """
         Create a protein sequence prompt from a linked MSA (Multiple Sequence Alignment) for PoET Jobs.
 
         Parameters
         ----------
         num_sequences : int, optional
             Maximum number of sequences in the prompt. Must be  <100.
@@ -599,30 +648,30 @@
             If both or none of 'num_sequences', 'num_residues' is specified.
 
         Returns
         -------
         PromptJob
         """
         msa_id = self.msa_id
-        job = prompt_post(
+        return prompt_post(
             self.session,
             msa_id,
             num_sequences=num_sequences,
             num_residues=num_residues,
             method=method,
             homology_level=homology_level,
             max_similarity=max_similarity,
             min_similarity=min_similarity,
             always_include_seed_sequence=always_include_seed_sequence,
             num_ensemble_prompts=num_ensemble_prompts,
             random_seed=random_seed,
         )
-        return PromptFuture(self.session, job, self.msa_id)
 
-class PromptFuture(MSAFuture):
+
+class PromptFuture(MSAFuture, FutureBase):
     """
     Represents a result of a prompt job.
 
     Attributes
     ----------
     session : APISession
         An instance of APISession for API interactions.
@@ -638,18 +687,20 @@
 
     Returns
     -------
     List[PoetScoreResult]
         The list of results from the PoET scoring job.
     """
 
+    job_type = "/align/prompt"
+
     def __init__(
         self,
         session: APISession,
-        job: MultiJob,
+        job: Job,
         page_size=config.POET_PAGE_SIZE,
         msa_id: Optional[str] = None,
     ):
         """
         init a PoetScoreFuture instance.
 
         Parameters
@@ -657,484 +708,54 @@
             session (APISession): An instance of APISession for API interactions.
             job (Job): The PoET scoring job.
             page_size (int, optional): The number of results to fetch in a single page. Defaults to config.POET_PAGE_SIZE.
 
         """
         super().__init__(session, job)
         self.page_size = page_size
+
+        if msa_id is None:
+            msa_id = job_args_get(self.session, job.job_id).get("root_msa")
         self._msa_id = msa_id
 
-    def get(self, verbose: bool = False):
+    def get(self, verbose: bool = False) -> csv.reader:
         return self.get_prompt()
 
 
-class PoetScoreFuture(PoetFutureMixin, AsyncJobFuture):
-    """
-    Represents a result of a PoET scoring job.
-
-    Attributes
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    job : Job
-        The PoET scoring job.
-    page_size : int
-        The number of results to fetch in a single page.    
-
-    Methods
-    -------
-    get(verbose=False)
-        Get the final results of the PoET  job.
-
-    """
-
-    def __init__(self, session: APISession, job: MultiJob, page_size=config.POET_PAGE_SIZE):
-        """
-        init a PoetScoreFuture instance.
-
-        Parameters
-        ----------
-            session (APISession): An instance of APISession for API interactions.
-            job (Job): The PoET scoring job.
-            page_size (int, optional): The number of results to fetch in a single page. Defaults to config.POET_PAGE_SIZE.
-
-        """
-        super().__init__(session, job)
-        self.page_size = page_size
-
-    def get(self, verbose=False) -> List[PoetScoreResult]:
-        """
-        Get the final results of the PoET scoring job.
-
-        Parameters
-        ----------
-        verbose : bool, optional
-            If True, print verbose output. Defaults to False.
-
-        Raises
-        ------
-        APIError
-            If there is an issue with the API request.
-
-        Returns
-        -------
-        List[PoetScoreResult]
-            A list of PoetScoreResult objects representing the scoring results.
-        """
-        job_id = self.job.job_id
-        step = self.page_size
-
-        results = []
-        num_returned = step
-        offset = 0
-
-        while num_returned >= step:
-            try:
-                response = poet_score_get(
-                    self.session,
-                    job_id,
-                    page_offset=offset,
-                    page_size=step,
-                )
-                results += response.result
-                num_returned = len(response.result)
-                offset += num_returned
-            except APIError as exc:
-                if verbose:
-                    print(f"Failed to get results: {exc}")
-                return results
-        return results
-
-
-def poet_single_site_post(
-    session: APISession, variant, parent_id=None, prompt_id=None
-) -> MultiJob:
-    """
-    Request PoET single-site analysis for a variant.
-
-    This function will mutate every position in the variant to every amino acid and return the scores.
-    Note that if parent_id is set then it will inherit all prompt properties of that parent.
-
-    Parameters
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    variant : str
-        The variant to analyze.
-    parent_id : str, optional
-        The ID of the parent job. Either parent_id or prompt_id must be set. Defaults to None.
-    prompt_id : str, optional
-        The ID of the prompt. Either parent_id or prompt_id must be set. Defaults to None.
-
-    Raises
-    ------
-    APIError
-        If the input parameters are invalid or there is an issue with the API request.
-
-    Returns
-    -------
-    PoetSSPJob
-        An object representing the status and results of the PoET single-site analysis job.
-        Note that the input variant score is given as `X0X`.
-    """
-    endpoint = "v1/poet/single_site"
-
-    if (parent_id is None and prompt_id is None) or (
-        parent_id is not None and prompt_id is not None
-    ):
-        raise InvalidParameterError("Either parent_id or prompt_id must be set.")
-
-    params = {"variant": variant}
-    if prompt_id is not None:
-        params["prompt_id"] = prompt_id
-    if parent_id is not None:
-        params["parent_id"] = parent_id
-
-    try:
-        response = session.post(endpoint, params=params)
-        return MultiJob.parse_obj(response.json()) 
-    except Exception as exc:
-        raise APIError(f"Failed to post poet single-site analysis: {exc}") from exc
-
-
-def poet_single_site_get(
-    session: APISession, job_id: str, page_size: int = 100, page_offset: int = 0
-) -> MultiJob:
-    """
-    Fetch paged results of a PoET single-site analysis job.
-
-    Parameters
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    job_id : str
-        The ID of the PoET single-site analysis job to fetch results from.
-    page_size : int, optional
-        The number of results to fetch in a single page. Defaults to 100.
-    page_offset : int, optional
-        The offset (number of results) to start fetching results from. Defaults to 0.
-
-    Raises
-    ------
-    APIError
-        If there is an issue with the API request.
-
-    Returns
-    -------
-    PoetSSPJob
-        An object representing the status and results of the PoET single-site analysis job.
-    """
-    endpoint = "v1/poet/single_site"
-
-    params = {"job_id": job_id, "page_size": page_size, "page_offset": page_offset}
-
-    try:
-        response = session.get(endpoint, params=params)
-        return MultiJob.parse_obj(response.json()) 
-    except Exception as exc:
-        raise APIError(
-            f"Failed to get poet single-site analysis results: {exc}"
-        ) from exc
-
-
-class PoetSingleSiteFuture(PoetFutureMixin, AsyncJobFuture):
-    """
-    Represents a result of a PoET single-site analysis job.
-
-    Attributes
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    job : Job
-        The PoET scoring job.
-    page_size : int
-        The number of results to fetch in a single page.
-
-    Methods
-    -------
-    get(verbose=False)
-        Get the final results of the PoET  job.
-
-    """
-
-    def __init__(self, session: APISession, job: MultiJob, page_size=config.POET_PAGE_SIZE):
-        """
-        init a PoetSingleSiteFuture instance.
-
-        Parameters
-        ----------
-            session (APISession): An instance of APISession for API interactions.
-            job (Job): The PoET single-site analysis job.
-            page_size (int, optional): The number of results to fetch in a single page. Defaults to config.POET_PAGE_SIZE.
-
-        """
-        super().__init__(session, job)
-        self.page_size = page_size
-
-    def get(self, verbose=False) -> List[PoetSSPResult]:
-        """
-        Get the results of a PoET single-site analysis job.
-
-        Parameters
-        ----------
-        verbose : bool, optional
-            If True, print verbose output. Defaults to False.
-
-        Returns
-        -------
-        Dict[bytes, float]
-            A dictionary mapping mutation codes to scores.
-
-        Raises
-        ------
-        APIError
-            If there is an issue with the API request.
-        """
-        job_id = self.job.job_id
-        step = self.page_size
-
-        results = []
-        num_returned = step
-        offset = 0
-
-        while num_returned >= step:
-            try:
-                response = poet_single_site_get(
-                    self.session,
-                    job_id,
-                    page_offset=offset,
-                    page_size=step,
-                )
-                results += response.result
-                num_returned = len(response.result)
-                offset += num_returned
-            except APIError as exc:
-                if verbose:
-                    print(f"Failed to get results: {exc}")
-                return results
-        return results
-
-
-def poet_generate_post(
-    session: APISession,
-    prompt_id: str,
-    num_samples=100,
-    temperature=1.0,
-    topk=None,
-    topp=None,
-    max_length=1000,
-    random_seed=None,
-) -> MultiJob:
-    """
-    Generate protein sequences with a prompt.
-
-    Parameters
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    prompt_id : str
-        The ID of the prompt to generate samples from.
-    num_samples : int, optional
-        The number of samples to generate. Defaults to 100.
-    temperature : float, optional
-        The temperature for sampling. Higher values produce more random outputs. Defaults to 1.0.
-    topk : int, optional
-        The number of top-k residues to consider during sampling. Defaults to None.
-    topp : float, optional
-        The cumulative probability threshold for top-p sampling. Defaults to None.
-    max_length : int, optional
-        The maximum length of generated proteins. Defaults to 1000.
-    random_seed : int, optional
-        Seed for random number generation. Defaults to a random number.
-
-    Raises
-    ------
-    APIError
-        If there is an issue with the API request.
-
-    Returns
-    -------
-    Job
-        An object representing the status and information about the generation job.
-    """
-    endpoint = "v1/poet/generate"
-
-    if not (0.1 <= temperature <= 2):
-        raise InvalidParameterError("The 'temperature' must be between 0.1 and 2.")
-    if topk:
-        if not (2 <= topk <= 20):
-            raise InvalidParameterError("The 'topk' must be between 2 and 22.")
-    if topp:
-        if not (0 <= topp <= 1):
-            raise InvalidParameterError("The 'topp' must be between 0 and 1.")
-    if random_seed:
-        if not (0 <= random_seed <= 2**32):
-            raise InvalidParameterError("The 'random_seed' must be between 0 and 1.")
-
-    if random_seed is None:
-        random_seed = random.randrange(2**32)
-
-    params = {
-        "prompt_id": prompt_id,
-        "generate_n": num_samples,
-        "temperature": temperature,
-        "maxlen": max_length,
-        "seed": random_seed,
-    }
-    if topk is not None:
-        params["topk"] = topk
-    if topp is not None:
-        params["topp"] = topp
-
-    try:
-        response = session.post(endpoint, params=params)
-        return MultiJob.parse_obj(response.json())
-    except Exception as exc:
-        raise APIError(f"Failed to post PoET generation request: {exc}") from exc
-
-
-def poet_generate_get(session: APISession, job_id) -> requests.Response:
-    """
-    Get the results of a PoET generation job.
-
-    Parameters
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    job_id : str
-        Job ID from a poet/generate job.
-
-    Raises
-    ------
-    APIError
-        If there is an issue with the API request.
-
-    Returns
-    -------
-    requests.Response
-        The response object containing the results of the PoET generation job.
-    """
-    endpoint = "v1/poet/generate"
-
-    params = {"job_id": job_id}
-
-    try:
-        response = session.get(endpoint, params=params, stream=True)
-        return response
-    except Exception as exc:
-        raise APIError(f"Failed to get poet generation results: {exc}") from exc
-
-
-class PoetGenerateFuture(PoetFutureMixin, StreamingAsyncJobFuture):
-    """
-    Represents a result of a PoET generation job.
-
-    Attributes
-    ----------
-    session : APISession
-        An instance of APISession for API interactions.
-    job : Job
-        The PoET scoring job.
-
-    Methods:
-        stream() -> Iterator[PoetScoreResult]:
-            Stream the results of the PoET generation job.
-
-    """
-
-    def stream(self) -> Iterator[PoetScoreResult]:
-        """
-        Stream the results from the response.
-
-        Returns
-        ------
-        PoetScoreResult: Yield
-            A result object containing the sequence, score, and name.
-
-        Raises
-        ------
-        APIError
-            If the request fails.
-        """
-        try:
-            response = poet_generate_get(self.session, self.job.job_id)
-            for tokens in csv_stream(response):
-                try:
-                    name, sequence = tokens[:2]
-                    score = [float(s) for s in tokens[2:]]
-                    sequence = sequence.encode()
-                    sample = PoetScoreResult(sequence=sequence, score=score, name=name)
-                    yield sample
-                except (IndexError, ValueError) as exc:
-                    # Skip malformed or incomplete tokens
-                    print(
-                        f"Skipping malformed or incomplete tokens: {tokens} with {exc}"
-                    )
-        except APIError as exc:
-            print(f"Failed to stream PoET generation results: {exc}")
-
-
 Prompt = Union[PromptFuture, str]
 
 
 def validate_prompt(prompt: Prompt):
     """helper function to validate prompt_id is prompt type"""
-    prompt_id = prompt
-    if isinstance(prompt, PromptFuture):
-        prompt_id = prompt.prompt_id
-    return prompt_id
+    if not (isinstance(prompt, PromptFuture) or isinstance(prompt, str)):
+        raise ValueError(
+            f"Expect prompt to be either a PromptFuture or str, got {type(prompt)}"
+        )
+    if isinstance(prompt, str):
+        return prompt
+    return prompt.prompt_id
+
 
 def validate_msa(msa: Union[MSAFuture, str]):
     """helper function to validate prompt_id is prompt type"""
-    msa_id = msa
-    if isinstance(msa, MSAFuture) or isinstance(msa, MultiJob):
-        msa_id = msa.msa_id
-    return msa_id
+    if not (isinstance(msa, MSAFuture) or isinstance(msa, str)):
+        raise ValueError(
+            f"Expect prompt to be either a MSAFuture or str, got {type(msa)}"
+        )
+    if isinstance(msa, str):
+        return msa
+    return msa.msa_id
+
 
-class PoetAPI:
+class AlignAPI:
     """API interface for calling Poet and Align endpoints"""
 
     def __init__(self, session: APISession):
         self.session = session
 
-    def load_job(self, job_id: str) -> PromptFuture:
-        """
-        Reload a previously ran prompt job to resume where you left off.
-
-        Parameters
-        ----------
-        prompt_id : str
-            ID for job.
-
-        Raises
-        ------
-        InvalidJob
-            If job is of incorrect type.
-
-        Returns
-        -------
-        PromptFuture
-            Job to resume workflows.
-        """
-        job = load_job(self.session, job_id)
-        if job.job_type == JobType.align:
-            return MSAFuture(self.session, job) 
-        elif job.job_type == JobType.align_prompt:
-            msa_id = job_args_get(self.session, job_id).get("root_msa")
-            job.msa_id = msa_id
-            return PromptFuture(self.session, job, msa_id=msa_id)
-        elif job.job_type == JobType.prots2prot_single_site:
-            return PoetSingleSiteFuture(self.session, job)
-        elif job.job_type == JobType.prots2prot:
-            return PoetScoreFuture(self.session, job)
-        elif job.job_type == JobType.prots2prot_generate:
-            return PoetGenerateFuture(self.session, job)
-        
-
-
     def upload_msa(self, msa_file) -> MSAFuture:
         """
         Upload an MSA from file.
 
         Parameters
         ----------
         msa_file : str, optional
@@ -1146,16 +767,15 @@
             If there is an issue with the API request.
 
         Returns
         -------
         MSAJob
             Job object containing the details of the MSA upload.
         """
-        job = msa_post(self.session, msa_file=msa_file)
-        return MSAFuture(self.session, job)
+        return msa_post(self.session, msa_file=msa_file)
 
     def create_msa(self, seed: bytes) -> MSAFuture:
         """
         Construct an MSA via homology search with the seed sequence.
 
         Parameters
         ----------
@@ -1168,18 +788,17 @@
             If there is an issue with the API request.
 
         Returns
         -------
         MSAJob
             Job object containing the details of the MSA construction.
         """
-        job = msa_post(self.session, seed=seed)
-        return MSAFuture(self.session, job)
+        return msa_post(self.session, seed=seed)
 
-    def upload_prompt(self, prompt_file: BinaryIO) -> MultiJob:
+    def upload_prompt(self, prompt_file: BinaryIO) -> Job:
         """
         Directly upload a prompt.
 
         Bypass post_msa and prompt_post steps entirely. In this case PoET will use the prompt as is.
         You can specify multiple prompts (one per replicate) with an <END_PROMPT> and newline between CSVs.
 
         Parameters
@@ -1193,18 +812,17 @@
             If there is an issue with the API request.
 
         Returns
         -------
         PromptJob
             An object representing the status and results of the prompt job.
         """
-        job = upload_prompt_post(self.session, prompt_file)
-        return PromptFuture(self.session, job)
+        return upload_prompt_post(self.session, prompt_file)
 
-    def get_prompt(self, job: MultiJob, prompt_index: Optional[int] = None) -> csv.reader:
+    def get_prompt(self, job: Job, prompt_index: Optional[int] = None) -> csv.reader:
         """
         Get prompts for a given job.
 
         Parameters
         ----------
         job : Job
             The job for which to retrieve data.
@@ -1216,15 +834,15 @@
         csv.reader
             A CSV reader for the response data.
         """
         return get_input(
             self.session, job, PoetInputType.PROMPT, prompt_index=prompt_index
         )
 
-    def get_seed(self, job: MultiJob) -> csv.reader:
+    def get_seed(self, job: Job) -> csv.reader:
         """
         Get input data for a given msa job.
 
         Parameters
         ----------
         job : Job
             The job for which to retrieve data.
@@ -1232,116 +850,22 @@
         Returns
         -------
         csv.reader
             A CSV reader for the response data.
         """
         return get_input(self.session, job, PoetInputType.INPUT)
 
-    def get_msa(self, job: MultiJob) -> csv.reader:
+    def get_msa(self, job: Job) -> csv.reader:
         """
         Get generated MSA for a given job.
 
         Parameters
         ----------
         job : Job
             The job for which to retrieve data.
 
         Returns
         -------
         csv.reader
             A CSV reader for the response data.
         """
         return get_input(self.session, job, PoetInputType.MSA)
-
-
-    def score(self, prompt: Prompt, queries: List[bytes]) -> PoetScoreFuture:
-        """
-        Score query sequences using the specified prompt.
-
-        Parameters
-        ----------
-        prompt : Prompt
-            Prompt job to use for scoring the sequences.
-        queries : List[bytes]
-            Sequences to score.
-
-        Returns
-        -------
-        results
-            The scores of the query sequences.
-        """
-        prompt_id = validate_prompt(prompt)
-        response = poet_score_post(self.session, prompt_id, queries)
-        return PoetScoreFuture(self.session, response)
-
-    def single_site(self, prompt: Prompt, sequence: bytes) -> PoetSingleSiteFuture:
-        """
-        Score all single substitutions of the query sequence using the specified prompt.
-
-        Parameters
-        ----------
-        prompt : Prompt
-            Prompt job to use for scoring the sequences.
-        sequence : bytes
-            Sequence to analyse.
-
-        Returns
-        -------
-        results
-            The scores of the mutated sequence.
-        """
-        prompt_id = validate_prompt(prompt)
-        response = poet_single_site_post(self.session, sequence, prompt_id=prompt_id)
-        return PoetSingleSiteFuture(self.session, response)
-
-    def generate(
-        self,
-        prompt: Prompt,
-        num_samples=100,
-        temperature=1.0,
-        topk=None,
-        topp=None,
-        max_length=1000,
-        seed=None,
-    ) -> PoetGenerateFuture:
-        """
-        Generate protein sequences conditioned on a prompt.
-
-        Parameters
-        ----------
-        prompt : PromptJob
-            The prompt to use for generating sequences.
-        num_samples : int, optional
-            The number of samples to generate, by default 100.
-        temperature : float, optional
-            The temperature for sampling. Higher values produce more random outputs, by default 1.0.
-        topk : int, optional
-            The number of top-k residues to consider during sampling, by default None.
-        topp : float, optional
-            The cumulative probability threshold for top-p sampling, by default None.
-        max_length : int, optional
-            The maximum length of generated proteins, by default 1000.
-        seed : int, optional
-            Seed for random number generation, by default a random number.
-
-        Raises
-        ------
-        APIError
-            If there is an issue with the API request.
-
-        Returns
-        -------
-        Job
-            An object representing the status and information about the generation job.
-        """
-        prompt_id = validate_prompt(prompt)
-        job = poet_generate_post(
-            self.session,
-            prompt_id,
-            num_samples=num_samples,
-            temperature=temperature,
-            topk=topk,
-            topp=topp,
-            max_length=max_length,
-            random_seed=seed,
-        )
-        return PoetGenerateFuture(self.session, job)
```

### Comparing `openprotein_python-0.3.2/openprotein/api/predict.py` & `openprotein_python-0.4.0/openprotein/api/predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,79 @@
-from typing import Optional, List, Union
-import pydantic
+from typing import Optional, List, Union, Any, Dict, Literal
+from pydantic import BaseModel
 
 from openprotein.base import APISession
 from openprotein.api.jobs import AsyncJobFuture
-from openprotein.models import (
-    SequenceDataset,
-    SequenceData,
-)
-
-from openprotein.jobs import Job, MultiJob, JobType,JobStatus, PredictJob, PredictSingleSiteJob 
-from openprotein.errors import InvalidParameterError, APIError, InvalidJob
-from openprotein.api.train import TrainFuture
-from openprotein.api.jobs import load_job
+from openprotein.jobs import ResultsParser, Job, register_job_type, JobType, JobStatus
+from openprotein.errors import InvalidParameterError, APIError
+from openprotein.futures import FutureFactory, FutureBase
+
+
+class SequenceData(BaseModel):
+    sequence: str
+
+
+class SequenceDataset(BaseModel):
+    sequences: List[str]
+
+
+class Prediction(BaseModel):
+    """Prediction details."""
+
+    model_id: str
+    model_name: str
+    properties: Dict[str, Dict[str, float]]
+
+
+class PredictJobBase(Job):
+    # might be none if just fetching
+    job_id: Optional[str] = None
+    job_type: str
+    status: JobStatus
+
+
+@register_job_type(JobType.workflow_predict)
+class PredictJob(PredictJobBase):
+    """Properties about predict job returned via API."""
+
+    class SequencePrediction(BaseModel):
+        """Sequence prediction."""
+
+        sequence: str
+        predictions: List[Prediction] = []
+
+    result: Optional[List[SequencePrediction]] = None
+    job_type: Literal[JobType.workflow_predict] = JobType.workflow_predict
+
+
+@register_job_type(JobType.worflow_predict_single_site)
+class PredictSingleSiteJob(PredictJobBase):
+    """Properties about single-site prediction job returned via API."""
+
+    class SequencePrediction(BaseModel):
+        """Sequence prediction."""
+
+        position: int
+        amino_acid: str
+        # sequence: str
+        predictions: List[Prediction] = []
+
+    result: Optional[List[SequencePrediction]] = None
+    job_type: Literal[JobType.worflow_predict_single_site] = (
+        JobType.worflow_predict_single_site
+    )
 
 
 def _create_predict_job(
     session: APISession,
     endpoint: str,
     payload: dict,
     model_ids: Optional[List[str]] = None,
     train_job_id: Optional[str] = None,
-) -> PredictJob:
+) -> FutureBase:
     """
     Creates a Predict request and returns the job object.
 
     This function makes a post request to the specified endpoint with the payload.
     Either 'model_ids' or 'train_job_id' should be provided but not both.
 
     Parameters
@@ -69,35 +118,35 @@
 
     if model_ids is not None:
         payload["model_id"] = model_ids
     else:
         payload["train_job_id"] = train_job_id
 
     response = session.post(endpoint, json=payload)
-    return MultiJob.parse_obj(response.json())
+    return FutureFactory.create_future(session=session, response=response)
 
 
 def create_predict_job(
     session: APISession,
     sequences: SequenceDataset,
-    train_job: TrainFuture,
+    train_job: Any,
     model_ids: Optional[List[str]] = None,
 ) -> PredictJob:
     """
     Creates a predict job with a given set of sequences and a train job.
 
     This function will use the sequences and train job ID to create a new Predict job.
 
     Parameters
     ----------
     session : APISession
         APIsession with auth
     sequences : SequenceDataset
         The dataset containing the sequences to predict
-    train_job : TrainFuture
+    train_job : Any
         The Train job: this model will be used for making Predicts.
     model_ids: List[str]
         specific IDs for models
 
     Returns
     -------
     PredictJob
@@ -122,27 +171,27 @@
         session, endpoint, payload, model_ids=model_ids, train_job_id=train_job.id
     )
 
 
 def create_predict_single_site(
     session: APISession,
     sequence: SequenceData,
-    train_job: TrainFuture,
+    train_job: Any,
     model_ids: Optional[List[str]] = None,
 ) -> PredictJob:
     """
     Creates a predict job for single site mutants with a given sequence and a train job.
 
     Parameters
     ----------
     session : APISession
         APIsession with auth
     sequence : SequenceData
         The sequence for which single site mutants predictions will be made.
-    train_job : TrainFuture
+    train_job : Any
         The train job whose model will be used for making Predicts.
     model_ids: List[str]
         specific IDs for models
 
     Returns
     -------
     PredictJob
@@ -200,16 +249,16 @@
     params = {}
     if page_size is not None:
         params["page_size"] = page_size
     if page_offset is not None:
         params["page_offset"] = page_offset
 
     response = session.get(endpoint, params=params)
-
-    return MultiJob.parse_obj(response.json())
+    # get results to assemble into list
+    return ResultsParser.parse_obj(response.json())
 
 
 def get_single_site_prediction_results(
     session: APISession,
     job_id: str,
     page_size: Optional[int] = None,
     page_offset: Optional[int] = None,
@@ -242,16 +291,16 @@
     params = {}
     if page_size is not None:
         params["page_size"] = page_size
     if page_offset is not None:
         params["page_offset"] = page_offset
 
     response = session.get(endpoint, params=params)
-
-    return MultiJob.parse_obj(response.json())
+    # get results to assemble into list
+    return ResultsParser.parse_obj(response)
 
 
 class PredictFutureMixin:
     """
     Class to to retrieve results from a Predict job.
 
     Attributes
@@ -299,34 +348,56 @@
             return get_single_site_prediction_results(
                 self.session, self.id, page_size, page_offset
             )
         else:
             return get_prediction_results(self.session, self.id, page_size, page_offset)
 
 
-class PredictFuture(PredictFutureMixin, AsyncJobFuture):
+class PredictFuture(PredictFutureMixin, AsyncJobFuture, FutureBase):
     """Future Job for manipulating results"""
-    def __init__(self,
-                 session: APISession,
-                 job:PredictJob,
-                 page_size=1000):
+
+    job_type = [JobType.workflow_predict, JobType.worflow_predict_single_site]
+
+    def __init__(self, session: APISession, job: PredictJob, page_size=1000):
         super().__init__(session, job)
         self.page_size = page_size
 
     def __str__(self) -> str:
         return str(self.job)
 
     def __repr__(self) -> str:
         return repr(self.job)
 
     @property
     def id(self):
         return self.job.job_id
 
-    def get(self, verbose: bool = False) -> Union[PredictSingleSiteJob, PredictJob]:
+    def _fmt_results(self, results):
+        properties = set(results[0].dict()["predictions"][0]["properties"].keys())
+        dict_results = {}
+        for p in properties:
+            dict_results[p] = {}
+            for i, r in enumerate(results):
+                s = r.sequence
+                props = r.predictions[0].properties[p]
+                dict_results[p][s] = {"mean": props["y_mu"], "variance": props["y_var"]}
+        return dict_results
+
+    def _fmt_ssp_results(self, results):
+        properties = set(results[0].dict()["predictions"][0]["properties"].keys())
+        dict_results = {}
+        for p in properties:
+            dict_results[p] = {}
+            for i, r in enumerate(results):
+                s = f"{r.position+1}{r.amino_acid}"
+                props = r.predictions[0].properties[p]
+                dict_results[p][s] = {"mean": props["y_mu"], "variance": props["y_var"]}
+        return dict_results
+
+    def get(self, verbose: bool = False) -> Dict:
         """
         Get all the results of the predict job.
 
         Args:
             verbose (bool, optional): If True, print verbose output. Defaults False.
 
         Raises:
@@ -346,60 +417,48 @@
                 response = self.get_results(page_offset=offset, page_size=step)
                 results += response.result
                 num_returned = len(response.result)
                 offset += num_returned
             except APIError as exc:
                 if verbose:
                     print(f"Failed to get results: {exc}")
-                return results
-        return results
+        if self.job.job_type == JobType.workflow_predict:
+            return self._fmt_results(results)
+        else:
+            return self._fmt_ssp_results(results)
 
 
-class TrainPredictAdapter(PredictFuture):
-    """Future Job for manipulating results"""
-    def __init__(self, session: APISession,
-                 model_id:Optional[str] = None,
-                 page_size=1000):
-        super().__init__(session, job=None)
-        self.page_size = page_size
-        self.model_id = model_id
+class PredictService:
+    """interface for calling Predict endpoints"""
 
-    
-    def create(
-        self,
-        sequences: List) -> PredictFuture:
-        pass
-
-class PredictAPI:
-    """API interface for calling Predict endpoints"""
     def __init__(self, session: APISession):
         """
-        Initialize a new instance of the PredictAPI class.
+        Initialize a new instance of the PredictService class.
 
         Parameters
         ----------
         session : APISession
             APIsession with auth
         """
         self.session = session
 
     def create_predict_job(
         self,
         sequences: List,
-        train_job: TrainFuture,
+        train_job: Any,
         model_ids: Optional[List[str]] = None,
     ) -> PredictFuture:
         """
         Creates a new Predict job for a given list of sequences and a trained model.
 
         Parameters
         ----------
         sequences : List
             The list of sequences to be used for the Predict job.
-        train_job : TrainFuture
+        train_job : Any
             The train job object representing the trained model.
         model_ids : List[str], optional
             The list of model ids to be used for Predict. Default is None.
 
         Returns
         -------
         PredictFuture
@@ -424,36 +483,38 @@
                         for s in sequences
                     ]
                 ):
                     raise InvalidParameterError(
                         f"Predict sequences length {len(sequences[0])}  != training assaydata ({train_job.assaymetadata.sequence_length})"
                     )
         if not train_job.done():
-            raise InvalidParameterError(
-                f"train job has status {train_job.status.value}, Predict requires status SUCCESS"
-            )
+            print(f"WARNING: training job has status {train_job.status}")
+            # raise InvalidParameterError(
+            #    f"train job has status {train_job.status.value}, Predict requires status SUCCESS"
+            # )
 
         sequence_dataset = SequenceDataset(sequences=sequences)
-        job = create_predict_job(self.session, sequence_dataset, train_job, model_ids=model_ids)
-        return PredictFuture(self.session, job)
+        return create_predict_job(
+            self.session, sequence_dataset, train_job, model_ids=model_ids
+        )
 
     def create_predict_single_site(
         self,
         sequence: str,
-        train_job: TrainFuture,
+        train_job: Any,
         model_ids: Optional[List[str]] = None,
     ) -> PredictFuture:
         """
         Creates a new Predict job for single site mutation analysis with a trained model.
 
         Parameters
         ----------
         sequence : str
             The sequence for single site analysis.
-        train_job : TrainFuture
+        train_job : Any
             The train job object representing the trained model.
         model_ids : List[str], optional
             The list of model ids to be used for Predict. Default is None.
 
         Returns
         -------
         PredictFuture
@@ -474,110 +535,16 @@
             if train_job.assaymetadata.sequence_length is not None:
                 if any([train_job.assaymetadata.sequence_length != len(sequence)]):
                     raise InvalidParameterError(
                         f"Predict sequences length {len(sequence)}  != training assaydata ({train_job.assaymetadata.sequence_length})"
                     )
         train_job.refresh()
         if not train_job.done():
-            raise InvalidParameterError(
-                f"train job has status {train_job.status.value}, Predict requires status SUCCESS"
-            )
+            print(f"WARNING: training job has status {train_job.status}")
+            # raise InvalidParameterError(
+            #    f"train job has status {train_job.status.value}, Predict requires status SUCCESS"
+            # )
 
         sequence_dataset = SequenceData(sequence=sequence)
-        job = create_predict_single_site(self.session, sequence_dataset, train_job, model_ids=model_ids)
-        return PredictFuture(self.session, job)
-
-    def get_prediction_results(
-        self,
-        job_id: str,
-        page_size: Optional[int] = None,
-        page_offset: Optional[int] = None,
-    ) -> PredictJob:
-        """
-        Retrieves the results of a Predict job.
-
-        Parameters
-        ----------
-        job_id : str
-            The ID of the Predict job.
-        page_size : Optional[int], default is None
-            The number of results to be returned per page. If None, all results are returned.
-        page_offset : Optional[int], default is None
-            The number of results to skip. If None, defaults to 0.
-
-        Returns
-        -------
-        PredictJob
-            The job object representing the Predict job.
-
-        Raises
-        ------
-        HTTPError
-            If the GET request does not succeed.
-        """
-        job_details = get_prediction_results(
-            self.session, job_id, page_size, page_offset
-        )
-        return PredictFuture(self.session, job_details)
-
-    def get_single_site_prediction_results(
-        self,
-        job_id: str,
-        page_size: Optional[int] = None,
-        page_offset: Optional[int] = None,
-    ) -> PredictSingleSiteJob:
-        """
-        Retrieves the results of a single site Predict job.
-
-        Parameters
-        ----------
-        job_id : str
-            The ID of the Predict job.
-        page_size : Optional[int], default is None
-            The number of results to be returned per page. If None, all results are returned.
-        page_offset : Optional[int], default is None
-            The page number to start retrieving results from. If None, defaults to 0.
-
-        Returns
-        -------
-        PredictSingleSiteJob
-            The job object representing the single site Predict job.
-
-        Raises
-        ------
-        HTTPError
-            If the GET request does not succeed.
-        """
-        job_details = get_single_site_prediction_results(
-            self.session, job_id, page_size, page_offset
+        return create_predict_single_site(
+            self.session, sequence_dataset, train_job, model_ids=model_ids
         )
-        return PredictFuture(self.session, job_details)
-
-    def load_job(self, job_id: str) -> PredictFuture:
-        """
-        Reload a Submitted job to resume from where you left off!
-
-
-        Parameters
-        ----------
-        job_id : str
-            The identifier of the job whose details are to be loaded.
-
-        Returns
-        -------
-        Job
-            PredictJob
-
-        Raises
-        ------
-        HTTPError
-            If the request to the server fails.
-        InvalidJob
-            If the Job is of the wrong type
-
-        """
-        job_details = load_job(self.session, job_id)
-        if job_details.job_type not in [JobType.predict, JobType.predict_single_site]:
-            raise InvalidJob(
-                f"Job {job_id} is not of type {JobType.predict} or {JobType.predict_single_site}"
-            )
-        return PredictFuture(self.session, job_details)
```

### Comparing `openprotein_python-0.3.2/openprotein/api/train.py` & `openprotein_python-0.4.0/openprotein/api/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,49 @@
 from typing import Optional, List, Union
+from pydantic import BaseModel
+
 import pydantic
 from openprotein.base import APISession
 from openprotein.api.jobs import AsyncJobFuture, Job
+from openprotein.futures import FutureFactory, FutureBase
 
-from openprotein.models import TrainGraph
 from openprotein.errors import InvalidParameterError, APIError, InvalidJob
 from openprotein.api.data import AssayDataset, AssayMetadata
-from openprotein.jobs import Job, MultiJob, JobType,JobStatus, CVResults, Jobplus 
-
+from openprotein.jobs import JobType
+from openprotein.api.predict import PredictService, PredictFuture
+from datetime import datetime
+
+
+class CVItem(BaseModel):
+    row_index: int
+    sequence: str
+    measurement_name: str
+    y: float
+    y_mu: float
+    y_var: float
+
+
+class CVResults(Job):
+    num_rows: int
+    page_size: int
+    page_offset: int
+    result: List[CVItem]
+
+
+class TrainStep(BaseModel):
+    step: int
+    loss: float
+    tag: str
+    tags: dict
+
+
+class TrainGraph(BaseModel):
+    traingraph: List[TrainStep]
+    created_date: datetime
+    job_id: str
 
 
 def list_models(session: APISession, job_id: str) -> List:
     """
     List models assoicated with job
 
     Parameters
@@ -77,15 +109,15 @@
 def _train_job(
     session: APISession,
     endpoint: str,
     assaydataset: AssayDataset,
     measurement_name: Union[str, List[str]],
     model_name: str = "",
     force_preprocess: Optional[bool] = False,
-) -> Jobplus:
+) -> Job:
     """
     Create a training job.
 
     Validate inputs, format  data, sends the job training request to the endpoint,
 
     Parses the response into a `Job` object.
 
@@ -136,15 +168,16 @@
         "measurement_name": measurement_name,
         "model_name": model_name,
     }
     params = {"force_preprocess": str(force_preprocess).lower()}
 
     response = session.post(endpoint, params=params, json=data)
     response.raise_for_status()
-    return MultiJob.parse_obj(response.json())
+    return FutureFactory.create_future(session=session, response=response)
+
 
 def create_train_job(
     session: APISession,
     assaydataset: AssayDataset,
     measurement_name: Union[str, List[str]],
     model_name: str = "",
     force_preprocess: Optional[bool] = False,
@@ -222,42 +255,14 @@
 def get_training_results(session: APISession, job_id: str) -> TrainGraph:
     """Get Training results (e.g. loss etc) of job."""
     endpoint = f"v1/workflow/train/{job_id}"
     response = session.get(endpoint)
     return TrainGraph(**response.json())
 
 
-def load_job(session: APISession, job_id: str) -> Jobplus:
-    """
-    Reload a Submitted job to resume from where you left off!
-
-
-    Parameters
-    ----------
-    session : APISession
-        The current API session for communication with the server.
-    job_id : str
-        The identifier of the job whose details are to be loaded.
-
-    Returns
-    -------
-    Job
-        Job
-
-    Raises
-    ------
-    HTTPError
-        If the request to the server fails.
-
-    """
-    endpoint = f"v1/workflow/train/job/{job_id}"
-    response = session.get(endpoint)
-    return MultiJob.parse_obj(response.json())
-
-
 class CVFutureMixin:
     """
     A mixin class to provide cross-validation job submission and retrieval.
 
     Attributes
     ----------
     session : APISession
@@ -279,70 +284,49 @@
     train_job_id: str
     job: Job
 
     def crossvalidate(self):
         """
         Submit a cross-validation job to the server.
 
-        If the job has already been submitted, an InvalidJob exception is raised.
-
         Returns
         -------
         Job
             The Job object for this cross-validation job.
 
-        Raises
-        ------
-        InvalidJob
-            If the job has already been submitted.
         """
-        if self.job is None:
-            self.job = crossvalidate(self.session, self.train_job_id)
-            return self.job
-        else:
-            raise InvalidJob(
-                "CV Job has already been submitted. Use get_crossvalidation() instead."
-            )
+        self.job = crossvalidate(self.session, self.train_job_id)
+        return self.job
 
     def get_crossvalidation(
         self, page_size: Optional[int] = None, page_offset: Optional[int] = 0
     ):
         """
         Retrieves the results of the cross-validation job.
 
-        If no job has been submitted, an InvalidJob exception is raised.
 
         Parameters
         ----------
         page_size : int, optional
             The number of items to retrieve in a single request..
         page_offset : int, optional
             The offset to start retrieving items from. Default is 0.
 
         Returns
         -------
         dict
             The results of the cross-validation job.
 
-        Raises
-        ------
-        InvalidJob
-            If no job has been submitted.
         """
-        if self.job is not None:
-            return get_crossvalidation(
-                self.session, self.job.job_id, page_size, page_offset
-            )
-        else:
-            raise InvalidJob(
-                "No CV Job has been submitted! Call crossvalidate() and try again."
-            )
+        return get_crossvalidation(
+            self.session, self.job.job_id, page_size, page_offset
+        )
 
 
-class CVFuture(CVFutureMixin, AsyncJobFuture):
+class CVFuture(CVFutureMixin, AsyncJobFuture, FutureBase):
     """
     This class helps initiating, submitting, and retrieving the
     results of a cross-validation job.
 
     Attributes
     ----------
     session : APISession
@@ -350,22 +334,18 @@
     train_job_id : str
         The id of the training job associated with this cross-validation job.
     job : Job
         The Job object for this cross-validation job.
     page_size : int
         The number of items to retrieve in a single request.
 
-    Methods
-    -------
-    __str__():
-        Returns a string representation of the cross-validation job.
-    __repr__():
-        Returns a detailed representation of the cross-validation job.
     """
 
+    job_type = [JobType.workflow_crossvalidate]
+
     def __init__(self, session: APISession, train_job_id: str, job: Job = None):
         """
         Constructs a new CVFuture instance.
 
         Parameters
         ----------
         session : APISession
@@ -385,15 +365,18 @@
     def __repr__(self) -> str:
         return repr(self.job)
 
     @property
     def id(self):
         return self.job.job_id
 
-    def get(self, verbose: bool = False) -> CVResults:
+    def _fmt_results(self, results):
+        return [i.dict() for i in results]
+
+    def get(self, verbose: bool = False) -> List:
         """
         Get all the results of the CV job.
 
         Args:
             verbose (bool, optional): If True, print verbose output. Defaults False.
 
         Raises:
@@ -413,16 +396,16 @@
                 response = self.get_crossvalidation(page_offset=offset, page_size=step)
                 results += response.result
                 num_returned = len(response.result)
                 offset += num_returned
             except APIError as exc:
                 if verbose:
                     print(f"Failed to get results: {exc}")
-                return results
-        return results
+                return self._fmt_results(results)
+        return self._fmt_results(results)
 
 
 class TrainFutureMixin:
     """
     This class provides functionality for retrieving the
     results of a training job and initiating cross-validation jobs.
 
@@ -439,55 +422,51 @@
         Returns the results of the training job.
     crossvalidate():
         Submits a cross-validation job and returns it.
     """
 
     session: APISession
     job: Job
-    _crossvalidation = None
+
+    def _fmt_results(self, results):
+        train_dict = {}
+        tags = set([i.tag for i in results.traingraph])
+        for tag in tags:
+            train_dict[tag] = [
+                i.loss for i in results.traingraph if i.dict()["tag"] == tag
+            ]
+        return train_dict
 
     def get_results(self) -> TrainGraph:
         """
         Gets the results of the training job.
 
         Returns
         -------
         TrainGraph
             The results of the training job.
         """
-        return get_training_results(self.session, self.job.job_id)
+        results = get_training_results(self.session, self.job.job_id)
+        return self._fmt_results(results)
 
     def crossvalidate(self):
         """
-        Submits a cross-validation job. 
+        Submits a cross-validation job.
 
         If a cross-validation job has already been created, it returns that job.
         Otherwise, it creates a new cross-validation job and returns it.
 
         Returns
         -------
         CVFuture
             The cross-validation job associated with this training job.
         """
-        if self._crossvalidation is None:
-            cv = CVFuture(self.session, train_job_id = self.job.job_id)
-            cv.crossvalidate()
-            self._crossvalidation = cv
-        return self._crossvalidation
-
-    def get_assay_data(self):
-        """
-        NOT IMPLEMENTED.
-
-        Get the assay data used for the training job.
-
-        Returns:
-            The assay data.
-        """
-        raise NotImplementedError("get_assay_data is not available.")
+        cv = CVFuture(self.session, train_job_id=self.job.job_id)
+        job = cv.crossvalidate()  # noqa: F841
+        return cv
 
     def list_models(self):
         """
         List models assoicated with job
 
         Parameters
         ----------
@@ -500,58 +479,100 @@
         -------
         List
             List of models
         """
         return list_models(self.session, self.job.job_id)
 
 
-class TrainFuture(TrainFutureMixin, AsyncJobFuture):
+class TrainFuture(TrainFutureMixin, AsyncJobFuture, FutureBase):
     """Future Job for manipulating results"""
+
+    job_type = [JobType.workflow_train]
+
     def __init__(
         self,
         session: APISession,
         job: Job,
         assaymetadata: Optional[AssayMetadata] = None,
     ):
         super().__init__(session, job)
         self.assaymetadata = assaymetadata
+        self._predict = PredictService(session)
+
+    def predict(
+        self, sequences: List[str], model_ids: Optional[List[str]] = None
+    ) -> PredictFuture:
+        """
+        Creates a predict job based on the training job.
+
+        Parameters
+        ----------
+        sequences : List[str]
+            The list of sequences to be used for the Predict job.
+        model_ids : List[str], optional
+            The list of model ids to be used for Predict. Default is None.
+
+        Returns
+        -------
+        PredictFuture
+            The job object representing the Predict job.
+        """
+        return self._predict.create_predict_job(sequences, self, model_ids=model_ids)
+
+    def predict_single_site(
+        self,
+        sequence: str,
+        model_ids: Optional[List[str]] = None,
+    ) -> PredictFuture:
+        """
+        Creates a new Predict job for single site mutation analysis with a trained model.
+
+        Parameters
+        ----------
+        sequence : str
+            The sequence for single site analysis.
+        train_job : Any
+            The train job object representing the trained model.
+        model_ids : List[str], optional
+            The list of model ids to be used for Predict. Default is None.
+
+        Returns
+        -------
+        PredictFuture
+            The job object representing the Predict job.
+
+        Creates a predict job based on the training job
+        """
+        return self._predict.create_predict_single_site(
+            sequence, self, model_ids=model_ids
+        )
 
     def __str__(self) -> str:
         return str(self.job)
 
     def __repr__(self) -> str:
         return repr(self.job)
 
     @property
     def id(self):
         return self.job.job_id
 
-    def get_assay_data(self):
-        """
-        NOT IMPLEMENTED.
-
-        Get the assay data used for the training job.
-
-        Returns:
-            The assay data.
-        """
-        return self.get_assay_data()
-
     def get(self, verbose: bool = False) -> TrainGraph:
         try:
             results = self.get_results()
         except APIError as exc:
             if verbose:
                 print(f"Failed to get results: {exc}")
             raise exc
         return results
 
 
 class TrainingAPI:
     """API interface for calling Train endpoints"""
+
     def __init__(
         self,
         session: APISession,
     ):
         self.session = session
         self.assay = None
 
@@ -590,44 +611,41 @@
             If any measurement name provided does not exist in the AssayDataset,
             or if the AssayDataset has fewer than 3 data points.
         HTTPError
             If the request to the server fails.
         """
         if isinstance(measurement_name, str):
             measurement_name = [measurement_name]
-        job_details = create_train_job(
+        return create_train_job(
             self.session, assaydataset, measurement_name, model_name, force_preprocess
         )
-        return TrainFuture(self.session, job_details, assaydataset)
 
     def _create_training_job_br(
         self,
         assaydataset: AssayDataset,
         measurement_name: Union[str, List[str]],
         model_name: str = "",
         force_preprocess: Optional[bool] = False,
     ) -> TrainFuture:
         """Same as create_training_job."""
-        job_details = _create_train_job_br(
+        return _create_train_job_br(
             self.session, assaydataset, measurement_name, model_name, force_preprocess
         )
-        return TrainFuture(self.session, job_details, assaydataset)
 
     def _create_training_job_gp(
         self,
         assaydataset: AssayDataset,
         measurement_name: Union[str, List[str]],
         model_name: str = "",
         force_preprocess: Optional[bool] = False,
     ) -> TrainFuture:
         """Same as create_training_job."""
-        job_details = _create_train_job_gp(
+        return _create_train_job_gp(
             self.session, assaydataset, measurement_name, model_name, force_preprocess
         )
-        return TrainFuture(self.session, job_details, assaydataset)
 
     def get_training_results(self, job_id: str) -> TrainFuture:
         """
         Get training results (e.g. loss etc).
 
         Parameters
         ----------
@@ -636,39 +654,8 @@
 
 
         Returns
         -------
         TrainFuture
             A TrainFuture Job
         """
-        job_details = get_training_results(self.session, job_id)
-        return TrainFuture(self.session, job_details)
-
-    def load_job(self, job_id: str) -> Jobplus:
-        """
-        Reload a Submitted job to resume from where you left off!
-
-
-        Parameters
-        ----------
-        job_id : str
-            The identifier of the job whose details are to be loaded.
-
-        Returns
-        -------
-        Job
-            Job
-
-        Raises
-        ------
-        HTTPError
-            If the request to the server fails.
-        InvalidJob
-            If the Job is of the wrong type
-
-        """
-        job_details = load_job(self.session, job_id)
-        assay_metadata = None
-
-        if job_details.job_type != JobType.train:
-            raise InvalidJob(f"Job {job_id} is not of type {JobType.train}")
-        return TrainFuture(self.session, job_details, assay_metadata)
+        return get_training_results(self.session, job_id)
```

### Comparing `openprotein_python-0.3.2/openprotein/base.py` & `openprotein_python-0.4.0/openprotein/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,18 @@
     password : str
         The password of the user.
 
     Examples
     --------
     >>> session = APISession("username", "password")
     """
-    
 
     def __init__(self, username:str,
                  password:str,
-                 backend:str = "https://dev.api.openprotein.ai/api/",
+                 backend:str = "https://api.openprotein.ai/api/",
                  timeout:int = 180):
         super().__init__()
         self.backend = backend
         self.verify = True
         self.timeout = timeout
 
         # Custom retry strategies
@@ -54,15 +53,14 @@
         retry = Retry(total=4,
                       backoff_factor=3, #0,1,4,13s
                       status_forcelist=[500, 502, 503, 504, 101, 104]) 
         adapter = HTTPAdapter(max_retries=retry)
         self.mount('https://', adapter)
         self.login(username, password)
 
-
     def post(self, url, data=None, json=None, **kwargs):
         r"""Sends a POST request. Returns :class:`Response` object.
 
         :param url: URL for the new :class:`Request` object.
         :param data: (optional) Dictionary, list of tuples, bytes, or file-like
             object to send in the body of the :class:`Request`.
         :param json: (optional) json to send in the body of the :class:`Request`.
```

### Comparing `openprotein_python-0.3.2/openprotein/errors.py` & `openprotein_python-0.4.0/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.3.2/openprotein/fasta.py` & `openprotein_python-0.4.0/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.3.2/pyproject.toml` & `openprotein_python-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.3.2"
+version = "0.4.0"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.3.2/PKG-INFO` & `openprotein_python-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.3.2
+Version: 0.4.0
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -111,15 +111,15 @@
 ``` 
 session.jobs.get(JOB_ID)  # Replace JOB_ID with the ID of the specific job to be retrieved
 ```
 
 ### Resuming Jobs
 Jobs from prior workflows can be resumed using the load_job method provided by each API. 
 ```
-session.train.load_job(JOB_ID)  # Replace JOB_ID with the ID of the training job to resume
+session.load_job(JOB_ID)  # Replace JOB_ID with the ID of the training job to resume
 ```
 
 ## PoET interface
 The PoET Interface allows scoring, generating, and retrieving sequences using the PoET model.
 
 ### Scoring Sequences
 To score sequences, use the score function. Provide a prompt and a list of queries. The results will be a list of (sequence, score) pydantic objects.
```

