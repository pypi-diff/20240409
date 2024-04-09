# Comparing `tmp/etcd_client_py-0.2.4.tar.gz` & `tmp/etcd_client_py-0.3.0.tar.gz`

## Comparing `etcd_client_py-0.2.4.tar` & `etcd_client_py-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 etcd_client_py-0.2.4/Cargo.toml
--rw-r--r--   0     1001      127     4201 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/.github/workflows/ci.yml
--rw-r--r--   0     1001      127       69 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/.gitignore
--rw-r--r--   0     1001      127     1060 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/LICENSE
--rw-r--r--   0     1001      127      146 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/Makefile
--rw-r--r--   0     1001      127     1029 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/README.md
--rw-r--r--   0     1001      127    10920 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/etcd_client.pyi
--rw-r--r--   0     1001      127        0 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/py.typed
--rw-r--r--   0     1001      127       37 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/pytest.ini
--rw-r--r--   0     1001      127       42 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/requirements.txt
--rw-r--r--   0     1001      127     4948 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/client.rs
--rw-r--r--   0     1001      127     9274 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/communicator.rs
--rw-r--r--   0     1001      127     2283 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/compare.rs
--rw-r--r--   0     1001      127     1331 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/condvar.rs
--rw-r--r--   0     1001      127     3520 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/error.rs
--rw-r--r--   0     1001      127     2212 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/lib.rs
--rw-r--r--   0     1001      127     5636 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/lock_manager.rs
--rw-r--r--   0     1001      127     1828 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/txn.rs
--rw-r--r--   0     1001      127      389 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/txn_response.rs
--rw-r--r--   0     1001      127     3659 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/watch.rs
--rw-r--r--   0     1001      127     2550 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/watch_event.rs
--rw-r--r--   0     1001      127     1465 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/src/watch_event_stream.rs
--rw-r--r--   0     1001      127     1284 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/tests/conftest.py
--rw-r--r--   0     1001      127    20466 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/tests/harness.py
--rw-r--r--   0     1001      127     8962 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/tests/test.py
--rw-r--r--   0     1001      127    34775 2024-02-16 00:39:09.000000 etcd_client_py-0.2.4/Cargo.lock
--rw-r--r--   0     1001      127      707 2024-02-16 00:39:00.000000 etcd_client_py-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 etcd_client_py-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 etcd_client_py-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      127     4201 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1002 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127       69 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/.gitignore
+-rw-r--r--   0     1001      127     1060 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/LICENSE
+-rw-r--r--   0     1001      127      145 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/Makefile
+-rw-r--r--   0     1001      127     1029 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/README.md
+-rw-r--r--   0     1001      127    10633 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/etcd_client.pyi
+-rw-r--r--   0     1001      127        0 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/py.typed
+-rw-r--r--   0     1001      127       37 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/pytest.ini
+-rw-r--r--   0     1001      127       42 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/requirements.txt
+-rw-r--r--   0     1001      127     4948 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/client.rs
+-rw-r--r--   0     1001      127     7810 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/communicator.rs
+-rw-r--r--   0     1001      127     2628 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/compare.rs
+-rw-r--r--   0     1001      127     1331 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/condvar.rs
+-rw-r--r--   0     1001      127     3520 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/error.rs
+-rw-r--r--   0     1001      127     2212 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      127     5641 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/lock_manager.rs
+-rw-r--r--   0     1001      127     2031 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/txn.rs
+-rw-r--r--   0     1001      127      389 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/txn_response.rs
+-rw-r--r--   0     1001      127     3661 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/watch.rs
+-rw-r--r--   0     1001      127     2504 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/watch_event.rs
+-rw-r--r--   0     1001      127     1465 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/src/watch_event_stream.rs
+-rw-r--r--   0     1001      127     1284 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/tests/conftest.py
+-rw-r--r--   0     1001      127    21149 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/tests/harness.py
+-rw-r--r--   0     1001      127     8962 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/tests/test.py
+-rw-r--r--   0     1001      127    34775 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/Cargo.lock
+-rw-r--r--   0     1001      127      707 2024-04-09 08:53:13.000000 etcd_client_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 etcd_client_py-0.3.0/PKG-INFO
```

### Comparing `etcd_client_py-0.2.4/.github/workflows/ci.yml` & `etcd_client_py-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/LICENSE` & `etcd_client_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/README.md` & `etcd_client_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/etcd_client.pyi` & `etcd_client_py-0.3.0/etcd_client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, AsyncIterator, Final, Optional
 
 @dataclass
 class EtcdLockOption:
-    lock_name: str
+    lock_name: bytes
     timeout: Optional[float]
     ttl: Optional[int]
 
 class CompareOp:
     """ """
 
     EQUAL: Final[Any]
@@ -26,39 +26,39 @@
     """
     LESS: Final[Any]
     """
     """
 
 class Compare:
     @staticmethod
-    def version(key: str, cmp: "CompareOp", version: int) -> "Compare": ...
+    def version(key: bytes, cmp: "CompareOp", version: int) -> "Compare": ...
     """
     Compares the version of the given key.
     """
     @staticmethod
-    def create_revision(key: str, cmp: "CompareOp", revision: int) -> "Compare": ...
+    def create_revision(key: bytes, cmp: "CompareOp", revision: int) -> "Compare": ...
     """
     Compares the creation revision of the given key.
     """
     @staticmethod
-    def mod_revision(key: str, cmp: "CompareOp", revision: int) -> "Compare": ...
+    def mod_revision(key: bytes, cmp: "CompareOp", revision: int) -> "Compare": ...
     """
     Compares the last modified revision of the given key.
     """
     @staticmethod
-    def value(key: str, cmp: "CompareOp", value: str) -> "Compare": ...
+    def value(key: bytes, cmp: "CompareOp", value: bytes) -> "Compare": ...
     """
     Compares the value of the given key.
     """
     @staticmethod
-    def lease(key: str, cmp: "CompareOp", lease: int) -> "Compare": ...
+    def lease(key: bytes, cmp: "CompareOp", lease: int) -> "Compare": ...
     """
     Compares the lease id of the given key.
     """
-    def with_range(self, end: list[int]) -> "Compare": ...
+    def with_range(self, end: bytes) -> "Compare": ...
     """
     Sets the comparison to scan the range [key, end).
     """
     def with_prefix(self) -> "Compare": ...
     """
     Sets the comparison to scan all keys prefixed by the key.
     """
@@ -91,19 +91,19 @@
 
 class TxnOp:
     """
     Transaction operation.
     """
 
     @staticmethod
-    def get(key: str) -> "TxnOp": ...
+    def get(key: bytes) -> "TxnOp": ...
     @staticmethod
-    def put(key: str, value: str) -> "TxnOp": ...
+    def put(key: bytes, value: bytes) -> "TxnOp": ...
     @staticmethod
-    def delete(key: str) -> "TxnOp": ...
+    def delete(key: bytes) -> "TxnOp": ...
     @staticmethod
     def txn(txn: "Txn") -> "TxnOp": ...
 
 class TxnResponse:
     def succeeded(self) -> bool: ...
 
 class Client:
@@ -150,63 +150,55 @@
         """ """
     async def wait(self) -> None:
         """ """
     async def notify_waiters(self) -> None:
         """ """
 
 class Communicator:
-    async def get(self, key: str) -> str:
+    async def get(self, key: bytes) -> list[int]:
         """
         Gets the key from the key-value store.
         """
-    async def get_prefix(self, key: str) -> dict[str, Any]:
+    async def get_prefix(self, key: bytes) -> list[tuple[list[int], list[int]]]:
         """
         Gets the key from the key-value store.
         """
-    async def put(self, key: str, value: str) -> None:
-        """
-        Put the given key into the key-value store.
-        A put request increments the revision of the key-value store
-        and generates one event in the event history.
-        """
-    async def put_prefix(self, key: str, value: dict[str, Any]) -> None:
+    async def put(self, key: bytes, value: bytes) -> None:
         """
         Put the given key into the key-value store.
         A put request increments the revision of the key-value store
         and generates one event in the event history.
         """
     async def txn(self, txn: "Txn") -> "TxnResponse":
         """
         Processes multiple operations in a single transaction.
         A txn request increments the revision of the key-value store
         and generates events with the same revision for every completed operation.
         It is not allowed to modify the same key several times within one txn.
         """
-    async def delete(self, key: str) -> None:
+    async def delete(self, key: bytes) -> None:
         """
         Deletes the given key from the key-value store.
         """
-    async def delete_prefix(self, key: str) -> None:
+    async def delete_prefix(self, key: bytes) -> None:
         """
         Deletes the given key from the key-value store.
         """
-    async def keys_prefix(self, key: str) -> list[str]:
-        """ """
-    async def replace(self, key: str, initial_value: str, new_value: str) -> bool:
+    async def keys_prefix(self, key: bytes) -> list[list[int]]:
         """ """
-    async def lock(self, name: str) -> None:
+    async def lock(self, name: bytes) -> None:
         """
         Lock acquires a distributed shared lock on a given named lock.
         On success, it will return a unique key that exists so long as the
         lock is held by the caller. This key can be used in conjunction with
         transactions to safely ensure updates to etcd only occur while holding
         lock ownership. The lock is held until Unlock is called on the key or the
         lease associate with the owner expires.
         """
-    async def unlock(self, key: str) -> None:
+    async def unlock(self, name: bytes) -> None:
         """
         Unlock takes a key returned by Lock and releases the hold on lock. The
         next Lock caller waiting for the lock will then be woken up and given
         ownership of the lock.
         """
     async def lease_grant(self, ttl: int) -> None:
         """
@@ -221,28 +213,28 @@
     async def lease_keep_alive(self, id: int) -> None:
         """
         Keeps the lease alive by streaming keep alive requests from the client
         to the server and streaming keep alive responses from the server to the client.
         """
     def watch(
         self,
-        key: str,
+        key: bytes,
         *,
         once: Optional[bool] = False,
         ready_event: Optional["CondVar"] = None,
     ) -> "Watch":
         """
         Watches for events happening or that have happened. Both input and output
         are streams; the input stream is for creating and canceling watcher and the output
         stream sends events. The entire event history can be watched starting from the
         last compaction revision.
         """
     def watch_prefix(
         self,
-        key: str,
+        key: bytes,
         *,
         once: Optional[bool] = False,
         ready_event: Optional["CondVar"] = None,
     ) -> "Watch":
         """
         Watches for events happening or that have happened. Both input and output
         are streams; the input stream is for creating and canceling watcher and the output
@@ -257,24 +249,24 @@
         """ """
     async def __anext__(self) -> "WatchEvent":
         """ """
 
 class WatchEvent:
     """ """
 
-    key: str
-    value: str
+    key: bytes
+    value: bytes
     event: "WatchEventType"
-    prev_value: Optional[str]
+    prev_value: Optional[bytes]
 
     def __init__(
-        key: str,
-        value: str,
+        key: bytes,
+        value: bytes,
         event: "WatchEventType",
-        prev_value: Optional[str] = None,
+        prev_value: Optional[bytes] = None,
     ) -> None: ...
 
 class WatchEventType:
     """ """
 
     PUT: Final[Any]
     """
@@ -292,15 +284,15 @@
         """ """
     async def notify_waiters(self) -> None:
         """ """
 
 class ClientError(Exception):
     """ """
 
-class GRpcStatusError(ClientError):
+class GRPCStatusError(ClientError):
     """ """
 
 class InvalidArgsError(ClientError):
     """ """
 
 class IoError(ClientError):
     """ """
@@ -328,15 +320,15 @@
 
 class EndpointError(ClientError):
     """ """
 
 class LockError(ClientError):
     """ """
 
-class GRpcStatusCode(Enum):
+class GRPCStatusCode(Enum):
     Ok = 0
     """The operation completed successfully."""
 
     Cancelled = 1
     """The operation was cancelled."""
 
     Unknown = 2
```

### Comparing `etcd_client_py-0.2.4/src/client.rs` & `etcd_client_py-0.3.0/src/client.rs`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/src/communicator.rs` & `etcd_client_py-0.3.0/src/communicator.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-use etcd_client::{Client as EtcdClient, PutOptions};
+use etcd_client::Client as EtcdClient;
 use etcd_client::{DeleteOptions, GetOptions, WatchOptions};
-use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
+use pyo3::types::PyBytes;
 use pyo3_asyncio::tokio::future_into_py;
-use std::collections::HashMap;
 use std::sync::Arc;
 use tokio::sync::Mutex;
 
 use crate::condvar::PyCondVar;
 use crate::error::PyClientError;
 use crate::txn::PyTxn;
 use crate::txn_response::PyTxnResponse;
@@ -15,89 +14,82 @@
 
 #[pyclass(name = "Communicator")]
 pub struct PyCommunicator(pub Arc<Mutex<EtcdClient>>);
 
 #[pymethods]
 impl PyCommunicator {
     // TODO: Implement and use the CRUD response types
-    fn get<'a>(&'a self, py: Python<'a>, key: String) -> PyResult<&'a PyAny> {
+    fn get<'a>(&'a self, py: Python<'a>, key: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let key = key.as_bytes().to_vec();
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let result = client.get(key, None).await;
             result
                 .map(|response| {
                     let kvs = response.kvs();
                     if !kvs.is_empty() {
-                        Some(String::from_utf8(kvs[0].value().to_owned()).unwrap())
+                        Some(kvs[0].value().to_owned())
                     } else {
                         None
                     }
                 })
                 .map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn get_prefix<'a>(&'a self, py: Python<'a>, prefix: String) -> PyResult<&'a PyAny> {
+    fn get_prefix<'a>(&'a self, py: Python<'a>, prefix: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let prefix = prefix.as_bytes().to_vec();
+
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let options = GetOptions::new().with_prefix();
             let result = client.get(prefix, Some(options)).await;
             result
                 .map(|response| {
-                    let mut result = HashMap::new();
+                    let mut list = vec![];
                     let kvs = response.kvs();
                     for kv in kvs {
-                        let key = String::from_utf8(kv.key().to_owned()).unwrap();
-                        let value = String::from_utf8(kv.value().to_owned()).unwrap();
-                        result.insert(key, value);
+                        list.push((kv.key().to_owned(), kv.value().to_owned()));
                     }
-                    result
+                    list
                 })
                 .map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn put<'a>(&'a self, py: Python<'a>, key: String, value: String) -> PyResult<&'a PyAny> {
+    fn put<'a>(&'a self, py: Python<'a>, key: &PyBytes, value: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let key = key.as_bytes().to_vec();
+        let value = value.as_bytes().to_vec();
+
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let result = client.put(key, value, None).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn put_prefix<'a>(
-        &'a self,
-        py: Python<'a>,
-        prefix: String,
-        value: String,
-    ) -> PyResult<&'a PyAny> {
+    fn delete<'a>(&'a self, py: Python<'a>, key: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
-        future_into_py(py, async move {
-            let mut client = client.lock().await;
-            let options = PutOptions::new().with_prev_key();
-            let result = client.put(prefix, value, Some(options)).await;
-            result.map(|_| ()).map_err(|e| PyClientError(e).into())
-        })
-    }
+        let key = key.as_bytes().to_vec();
 
-    fn delete<'a>(&'a self, py: Python<'a>, key: String) -> PyResult<&'a PyAny> {
-        let client = self.0.clone();
         future_into_py(py, async move {
             let mut client = client.lock().await;
 
             let result = client.delete(key, None).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn delete_prefix<'a>(&'a self, py: Python<'a>, key: String) -> PyResult<&'a PyAny> {
+    fn delete_prefix<'a>(&'a self, py: Python<'a>, key: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let key = key.as_bytes().to_vec();
+
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let options = DeleteOptions::new().with_prefix();
             let result = client.delete(key, Some(options)).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
@@ -110,79 +102,53 @@
             let result = client.txn(txn.0).await;
             result
                 .map(PyTxnResponse)
                 .map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn replace<'a>(
-        &'a self,
-        py: Python<'a>,
-        key: String,
-        initial_val: String,
-        new_val: String,
-    ) -> PyResult<&'a PyAny> {
+    fn keys_prefix<'a>(&'a self, py: Python<'a>, key: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
-        future_into_py(py, async move {
-            let mut client = client.lock().await;
-            match client.get(key.clone(), None).await {
-                Ok(response) => {
-                    if let Some(key_value) = response.kvs().get(0) {
-                        if *key_value.value_str().unwrap() == initial_val {
-                            match client.put(key, new_val, None).await {
-                                Ok(_) => Ok(true), // replace successful
-                                Err(e) => Err(PyClientError(e)),
-                            }
-                        } else {
-                            Ok(false) // initial_val not equal to current value
-                        }
-                    } else {
-                        Ok(false) // Key does not exist
-                    }
-                }
-                Err(e) => Err(PyClientError(e)),
-            }
-            .map_err(|e| PyErr::new::<PyException, _>(format!("{}", e.0)))
-        })
-    }
+        let key = key.as_bytes().to_vec();
 
-    fn keys_prefix<'a>(&'a self, py: Python<'a>, key: String) -> PyResult<&'a PyAny> {
-        let client = self.0.clone();
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let options = GetOptions::new().with_prefix();
             let result = client.get(key, Some(options)).await;
             result
                 .map(|response| {
                     let mut result = Vec::new();
                     let kvs = response.kvs();
                     for kv in kvs {
-                        let key = String::from_utf8(kv.key().to_owned()).unwrap();
-                        result.push(key);
+                        result.push(kv.key().to_owned());
                     }
                     result
                 })
                 .map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn lock<'a>(&'a self, py: Python<'a>, name: String) -> PyResult<&'a PyAny> {
+    fn lock<'a>(&'a self, py: Python<'a>, name: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let name = name.as_bytes().to_vec();
+
         future_into_py(py, async move {
             let mut client = client.lock().await;
             let result = client.lock(name, None).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
 
-    fn unlock<'a>(&'a self, py: Python<'a>, key: String) -> PyResult<&'a PyAny> {
+    fn unlock<'a>(&'a self, py: Python<'a>, name: &PyBytes) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
+        let name = name.as_bytes().to_vec();
+
         future_into_py(py, async move {
             let mut client = client.lock().await;
-            let result = client.unlock(key).await;
+            let result = client.unlock(name).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
 
     // TODO: Implement and use the response types of `lease` type's methods
     fn lease_grant<'a>(&'a self, py: Python<'a>, ttl: i64) -> PyResult<&'a PyAny> {
         let client = self.0.clone();
@@ -218,32 +184,34 @@
             let result = client.lease_keep_alive(id).await;
             result.map(|_| ()).map_err(|e| PyClientError(e).into())
         })
     }
 
     fn watch(
         &self,
-        key: String,
+        key: &PyBytes,
         once: Option<bool>,
         ready_event: Option<PyCondVar>,
         cleanup_event: Option<PyCondVar>,
     ) -> PyWatch {
         let client = self.0.clone();
+        let key = key.as_bytes().to_vec();
         let once = once.unwrap_or(false);
         PyWatch::new(client, key, once, None, ready_event, cleanup_event)
     }
 
     fn watch_prefix(
         &self,
-        key: String,
+        key: &PyBytes,
         once: Option<bool>,
         ready_event: Option<PyCondVar>,
         cleanup_event: Option<PyCondVar>,
     ) -> PyWatch {
         let client = self.0.clone();
+        let key = key.as_bytes().to_vec();
         let once = once.unwrap_or(false);
         let options = WatchOptions::new().with_prefix();
         PyWatch::new(client, key, once, Some(options), ready_event, cleanup_event)
     }
 }
 
 impl PyCommunicator {
```

### Comparing `etcd_client_py-0.2.4/src/compare.rs` & `etcd_client_py-0.3.0/src/compare.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use etcd_client::{Compare, CompareOp};
 use pyo3::prelude::*;
 use pyo3::pyclass::CompareOp as PyO3CompareOp;
+use pyo3::types::PyBytes;
 
 #[derive(Clone)]
 #[pyclass(name = "CompareOp")]
 pub struct PyCompareOp(CompareOp);
 
 #[pymethods]
 impl PyCompareOp {
@@ -38,39 +39,46 @@
 #[derive(Clone)]
 #[pyclass(name = "Compare")]
 pub struct PyCompare(pub Compare);
 
 #[pymethods]
 impl PyCompare {
     #[staticmethod]
-    fn version(key: String, cmp: PyCompareOp, version: i64) -> PyResult<Self> {
+    fn version(key: &PyBytes, cmp: PyCompareOp, version: i64) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         Ok(PyCompare(Compare::version(key, cmp.0, version)))
     }
 
     #[staticmethod]
-    fn create_revision(key: String, cmp: PyCompareOp, revision: i64) -> PyResult<Self> {
+    fn create_revision(key: &PyBytes, cmp: PyCompareOp, revision: i64) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         Ok(PyCompare(Compare::create_revision(key, cmp.0, revision)))
     }
 
     #[staticmethod]
-    fn mod_revision(key: String, cmp: PyCompareOp, revision: i64) -> PyResult<Self> {
+    fn mod_revision(key: &PyBytes, cmp: PyCompareOp, revision: i64) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         Ok(PyCompare(Compare::mod_revision(key, cmp.0, revision)))
     }
 
     #[staticmethod]
-    fn value(key: String, cmp: PyCompareOp, value: String) -> PyResult<Self> {
+    fn value(key: &PyBytes, cmp: PyCompareOp, value: &PyBytes) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
+        let value = value.as_bytes().to_vec();
         Ok(PyCompare(Compare::value(key, cmp.0, value)))
     }
 
     #[staticmethod]
-    fn lease(key: String, cmp: PyCompareOp, lease: i64) -> PyResult<Self> {
+    fn lease(key: &PyBytes, cmp: PyCompareOp, lease: i64) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         Ok(PyCompare(Compare::lease(key, cmp.0, lease)))
     }
 
-    fn with_range(&self, end: String) -> PyResult<Self> {
+    fn with_range(&self, end: &PyBytes) -> PyResult<Self> {
+        let end = end.as_bytes().to_vec();
         Ok(PyCompare(self.0.clone().with_range(end)))
     }
 
     fn with_prefix(&self) -> PyResult<Self> {
         Ok(PyCompare(self.0.clone().with_prefix()))
     }
 }
```

### Comparing `etcd_client_py-0.2.4/src/condvar.rs` & `etcd_client_py-0.3.0/src/condvar.rs`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/src/error.rs` & `etcd_client_py-0.3.0/src/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 use pyo3::{create_exception, exceptions::PyException, types::PyDict, PyErr, Python, *};
 use std::fmt::Debug;
 
 create_exception!(etcd_client, ClientError, PyException);
-create_exception!(etcd_client, GRpcStatusError, ClientError);
+create_exception!(etcd_client, GRPCStatusError, ClientError);
 create_exception!(etcd_client, InvalidArgsError, ClientError);
 create_exception!(etcd_client, InvalidUriError, ClientError);
 create_exception!(etcd_client, IoError, ClientError);
 create_exception!(etcd_client, TransportError, ClientError);
 create_exception!(etcd_client, WatchError, ClientError);
 create_exception!(etcd_client, Utf8Error, ClientError);
 create_exception!(etcd_client, LeaseKeepAliveError, ClientError);
 create_exception!(etcd_client, ElectError, ClientError);
 create_exception!(etcd_client, InvalidHeaderValueError, ClientError);
 create_exception!(etcd_client, EndpointError, ClientError);
 create_exception!(etcd_client, LockError, ClientError);
 
-#[pyclass(name = "GRpcStatusCode")]
-pub enum PyGRpcStatusCode {
+#[pyclass(name = "GRPCStatusCode")]
+pub enum PyGRPCStatusCode {
     Ok = 0,
     Cancelled = 1,
     Unknown = 2,
     InvalidArgument = 3,
     DeadlineExceeded = 4,
     NotFound = 5,
     AlreadyExists = 6,
@@ -50,15 +50,15 @@
                     .set_item("details", e.details().to_vec())
                     .unwrap();
                 error_details
                     .set_item("message", e.message().to_owned())
                     .unwrap();
 
                 let kv_args: PyObject = error_details.into_py(py);
-                GRpcStatusError::new_err(kv_args)
+                GRPCStatusError::new_err(kv_args)
             }),
             etcd_client::Error::InvalidArgs(e) => {
                 InvalidArgsError::new_err(format!("InvalidArgsError(err={})", e))
             }
             etcd_client::Error::InvalidUri(e) => {
                 InvalidUriError::new_err(format!("InvalidUriError(err={})", e))
             }
```

### Comparing `etcd_client_py-0.2.4/src/lib.rs` & `etcd_client_py-0.3.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 mod watch_event_stream;
 
 use client::{PyClient, PyConnectOptions};
 use communicator::PyCommunicator;
 use compare::{PyCompare, PyCompareOp};
 use condvar::PyCondVar;
 use error::{
-    ClientError, ElectError, EndpointError, GRpcStatusError, InvalidArgsError,
-    InvalidHeaderValueError, InvalidUriError, IoError, LeaseKeepAliveError, PyGRpcStatusCode,
+    ClientError, ElectError, EndpointError, GRPCStatusError, InvalidArgsError,
+    InvalidHeaderValueError, InvalidUriError, IoError, LeaseKeepAliveError, PyGRPCStatusCode,
     TransportError, Utf8Error, WatchError,
 };
 use lock_manager::PyEtcdLockOption;
 use pyo3::prelude::*;
 use txn::{PyTxn, PyTxnOp};
 use txn_response::PyTxnResponse;
 use watch::PyWatch;
@@ -41,18 +41,18 @@
     module.add_class::<PyCompareOp>()?;
 
     module.add_class::<PyTxn>()?;
     module.add_class::<PyTxnOp>()?;
     module.add_class::<PyTxnResponse>()?;
     module.add_class::<PyEtcdLockOption>()?;
 
-    module.add_class::<PyGRpcStatusCode>()?;
+    module.add_class::<PyGRPCStatusCode>()?;
 
     module.add("ClientError", py.get_type::<ClientError>())?;
-    module.add("GRpcStatusError", py.get_type::<GRpcStatusError>())?;
+    module.add("GRPCStatusError", py.get_type::<GRPCStatusError>())?;
     module.add("InvalidArgsError", py.get_type::<InvalidArgsError>())?;
     module.add("IoError", py.get_type::<IoError>())?;
     module.add("InvalidUriError", py.get_type::<InvalidUriError>())?;
     module.add("TransportError", py.get_type::<TransportError>())?;
     module.add("WatchError", py.get_type::<WatchError>())?;
     module.add("Utf8Error", py.get_type::<Utf8Error>())?;
     module.add("LeaseKeepAliveError", py.get_type::<LeaseKeepAliveError>())?;
```

### Comparing `etcd_client_py-0.2.4/src/lock_manager.rs` & `etcd_client_py-0.3.0/src/lock_manager.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 use crate::{
     client::PyClient,
     communicator::PyCommunicator,
-    error::{GRpcStatusError, LockError, PyClientError},
+    error::{GRPCStatusError, LockError, PyClientError},
 };
 use etcd_client::{Client as EtcdClient, LockOptions};
 
-use pyo3::prelude::*;
+use pyo3::{prelude::*, types::PyBytes};
 use std::time::Duration;
 use tokio::time::{sleep, timeout};
 
 #[derive(Debug, Clone)]
 #[pyclass(get_all, set_all, name = "EtcdLockOption")]
 pub struct PyEtcdLockOption {
-    pub lock_name: String,
+    pub lock_name: Vec<u8>,
     pub timeout: Option<f64>,
     pub ttl: Option<i64>,
 }
 
 #[pymethods]
 impl PyEtcdLockOption {
     #[new]
-    fn new(lock_name: String, timeout: Option<f64>, ttl: Option<i64>) -> Self {
+    fn new(lock_name: &PyBytes, timeout: Option<f64>, ttl: Option<i64>) -> Self {
+        let lock_name = lock_name.as_bytes().to_vec();
         Self {
             lock_name,
             timeout,
             ttl,
         }
     }
 
     fn __repr__(&self) -> PyResult<String> {
         Ok(format!(
-            "EtcdLockOption(lock_name={}, timeout={:?}, ttl={:?})",
+            "EtcdLockOption(lock_name={:?}, timeout={:?}, ttl={:?})",
             self.lock_name, self.timeout, self.ttl
         ))
     }
 }
 
 pub struct EtcdLockManager {
     pub client: PyClient,
-    pub lock_name: String,
+    pub lock_name: Vec<u8>,
     pub ttl: Option<i64>,
     pub timeout_seconds: Option<f64>,
-    pub lock_id: Option<String>,
+    pub lock_id: Option<Vec<u8>>,
     pub lease_id: Option<i64>,
     pub lease_keepalive_task: Option<tokio::task::JoinHandle<Result<(), PyClientError>>>,
 }
 
 impl EtcdLockManager {
     pub fn new(client: PyClient, lock_opt: PyEtcdLockOption) -> Self {
         Self {
@@ -94,23 +95,19 @@
                 Duration::from_secs_f64(self.timeout_seconds.unwrap()),
                 async {
                     let lock_req_options = self
                         .lease_id
                         .map(|lease_id| LockOptions::new().with_lease(lease_id));
 
                     let lock_res = client
-                        .lock(self.lock_name.clone().as_bytes(), lock_req_options)
+                        .lock(self.lock_name.clone(), lock_req_options)
                         .await
                         .map_err(PyClientError)?;
 
-                    self.lock_id = Some(
-                        std::str::from_utf8(lock_res.key())
-                            .expect("Invalid utf8 chars includeded in lock request!")
-                            .to_owned(),
-                    );
+                    self.lock_id = Some(lock_res.key().to_vec());
                     Ok(())
                 },
             )
             .await;
 
         match timeout_result {
             Ok(Ok(_)) => {}
@@ -119,15 +116,15 @@
                 if let Some(lease_id) = self.lease_id {
                     match client.lease_revoke(lease_id).await {
                         Ok(_lease_revoke_res) => {}
                         Err(e) => match e {
                             etcd_client::Error::GRpcStatus(status)
                                 if status.code() != tonic::Code::NotFound =>
                             {
-                                return Err(GRpcStatusError::new_err(status.to_string()))
+                                return Err(GRPCStatusError::new_err(status.to_string()))
                             }
                             _ => return Err(PyClientError(e).into()),
                         },
                     }
                     return Err(LockError::new_err(timedout_err.to_string()));
                 }
             }
@@ -156,15 +153,19 @@
             lease_keepalive_task.abort();
         }
 
         if let Some(lease_id) = self.lease_id {
             client.lease_revoke(lease_id).await.map_err(PyClientError)?;
         } else {
             client
-                .unlock(self.lock_id.as_ref().unwrap().as_bytes())
+                .unlock(
+                    self.lock_id
+                        .to_owned()
+                        .expect("Failed to unlock due to lock_id is None"),
+                )
                 .await
                 .map_err(PyClientError)?;
         }
 
         self.lock_id = None;
         self.lease_id = None;
```

### Comparing `etcd_client_py-0.2.4/src/txn.rs` & `etcd_client_py-0.3.0/src/txn.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 use etcd_client::{DeleteOptions, GetOptions, PutOptions, Txn, TxnOp};
-use pyo3::prelude::*;
+use pyo3::{prelude::*, types::PyBytes};
 
 use crate::compare::PyCompare;
 
 #[derive(Debug, Clone)]
 #[pyclass(name = "TxnOp")]
 pub struct PyTxnOp(pub TxnOp);
 
 #[pymethods]
 impl PyTxnOp {
     #[staticmethod]
-    fn get(key: String) -> PyResult<Self> {
+    fn get(key: &PyBytes) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         let options = GetOptions::new();
         Ok(PyTxnOp(TxnOp::get(key, Some(options))))
     }
+
     #[staticmethod]
-    fn put(key: String, value: String) -> PyResult<Self> {
+    fn put(key: &PyBytes, value: &PyBytes) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
+        let value = value.as_bytes().to_vec();
         let options = PutOptions::new();
         Ok(PyTxnOp(TxnOp::put(key, value, Some(options))))
     }
 
     #[staticmethod]
-    fn delete(key: String) -> PyResult<Self> {
+    fn delete(key: &PyBytes) -> PyResult<Self> {
+        let key = key.as_bytes().to_vec();
         let options = DeleteOptions::new();
         Ok(PyTxnOp(TxnOp::delete(key, Some(options))))
     }
 
     #[staticmethod]
     fn txn(txn: PyTxn) -> PyResult<Self> {
         Ok(PyTxnOp(TxnOp::txn(txn.0)))
```

### Comparing `etcd_client_py-0.2.4/src/watch.rs` & `etcd_client_py-0.3.0/src/watch.rs`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 use crate::error::PyClientError;
 use crate::watch_event_stream::PyWatchEventStream;
 
 #[pyclass(name = "Watch")]
 #[derive(Clone)]
 pub struct PyWatch {
     client: Arc<Mutex<EtcdClient>>,
-    key: String,
+    key: Vec<u8>,
     once: bool,
     options: Option<WatchOptions>,
     watcher: Arc<Mutex<Option<Watcher>>>,
     event_stream_init_notifier: Arc<Notify>,
     event_stream: Arc<Mutex<Option<PyWatchEventStream>>>,
     ready_event: Option<PyCondVar>,
     #[allow(dead_code)]
     cleanup_event: Option<PyCondVar>,
 }
 
 impl PyWatch {
     pub fn new(
         client: Arc<Mutex<EtcdClient>>,
-        key: String,
+        key: Vec<u8>,
         once: bool,
         options: Option<WatchOptions>,
         ready_event: Option<PyCondVar>,
         cleanup_event: Option<PyCondVar>,
     ) -> Self {
         Self {
             client,
```

### Comparing `etcd_client_py-0.2.4/src/watch_event.rs` & `etcd_client_py-0.3.0/src/watch_event.rs`

 * *Files 5% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 use pyo3::prelude::*;
 use pyo3::pyclass::CompareOp;
 
 // Note: Event = namedtuple("Event", "key event value"), not asyncio.Event, threading.Event
 #[pyclass(get_all, name = "WatchEvent")]
 #[derive(PartialEq, Eq, Clone, Debug)]
 pub struct PyWatchEvent {
-    key: String,
-    value: String,
+    key: Vec<u8>,
+    value: Vec<u8>,
     event: PyWatchEventType,
-    prev_value: Option<String>,
+    prev_value: Option<Vec<u8>>,
 }
 
 #[pymethods]
 impl PyWatchEvent {
     #[new]
     #[pyo3(signature = (key, value, event, prev_value))]
     fn new(
-        key: String,
-        value: String,
+        key: Vec<u8>,
+        value: Vec<u8>,
         event: PyWatchEventType,
-        prev_value: Option<String>,
+        prev_value: Option<Vec<u8>>,
     ) -> Self {
         Self {
             key,
             value,
             event,
             prev_value,
         }
     }
 
     pub fn __repr__(&self) -> String {
         format!(
-            "Event(event={:?}, key={}, value={}, prev_value={:?})",
+            "Event(event={:?}, key={:?}, value={:?}, prev_value={:?})",
             self.event, self.key, self.value, self.prev_value
         )
     }
 
     fn __richcmp__(&self, py: Python, other: &Self, op: CompareOp) -> PyObject {
         match op {
             CompareOp::Eq => (self == other).into_py(py),
@@ -46,16 +46,16 @@
         }
     }
 }
 
 impl From<EtcdClientEvent> for PyWatchEvent {
     fn from(event: EtcdClientEvent) -> Self {
         let kv = event.kv().unwrap();
-        let key = String::from_utf8(kv.key().to_owned()).unwrap();
-        let value = String::from_utf8(kv.value().to_owned()).unwrap();
+        let key = kv.key().to_owned();
+        let value = kv.value().to_owned();
         let prev_value = None;
         let event = PyWatchEventType(event.event_type());
         Self {
             key,
             value,
             event,
             prev_value,
```

### Comparing `etcd_client_py-0.2.4/src/watch_event_stream.rs` & `etcd_client_py-0.3.0/src/watch_event_stream.rs`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/tests/conftest.py` & `etcd_client_py-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/tests/harness.py` & `etcd_client_py-0.3.0/tests/harness.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
+Backend.AI AsyncEtcd Client Copy
+Ref: https://github.com/lablup/backend.ai/blob/main/src/ai/backend/common/etcd.py
+=================================================================================
+"""
+
+"""
 An asynchronous client wrapper for etcd v3 API.
 
 It uses the etcd3 library using a thread pool executor.
 We plan to migrate to aioetcd3 library but it requires more work to get maturity.
 Fortunately, etcd3's watchers are not blocking because they are implemented
 using callbacks in separate threads.
 """
 
-from __future__ import annotations
-
 import asyncio
 from dataclasses import dataclass
 import enum
 import functools
 import logging
 from collections import ChainMap, namedtuple
 from typing import (
@@ -40,16 +44,16 @@
     Txn as EtcdTransactionAction,
     TxnOp,
     Compare,
     Communicator as EtcdCommunicator,
     CompareOp,
     CondVar,
     ConnectOptions,
-    GRpcStatusCode,
-    GRpcStatusError,
+    GRPCStatusCode,
+    GRPCStatusError,
     WatchEvent,
 )
 
 
 class QueueSentinel(enum.Enum):
     CLOSED = 0
     TIMEOUT = 1
@@ -60,15 +64,15 @@
     host: str
     port: int
 
     def __str__(self):
         return f"{self.host}:{self.port}"
 
     @classmethod
-    def parse(cls, s: str) -> HostPortPair:
+    def parse(cls, s: str) -> "HostPortPair":
         if ":" in s:
             host, port_str = s.rsplit(":")
             port = int(port_str)
         else:
             host = s
             port = 2379
         return cls(host, port)
@@ -216,15 +220,15 @@
         :param scope: The config scope for putting the values.
         :param scope_prefix_map: The scope map used to mangle the prefix for the config scope.
         :return:
         """
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         async with self.etcd.connect() as communicator:
-            await communicator.put(mangled_key, str(val))
+            await communicator.put(mangled_key.encode(self.encoding), str(val).encode(self.encoding))
 
     async def put_prefix(
         self,
         key: str,
         dict_obj: NestedStrKeyedMapping,
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
@@ -256,15 +260,15 @@
 
         _flatten(key, cast(NestedStrKeyedDict, dict_obj))
 
         async with self.etcd.connect() as communicator:
             actions = []
             for k, v in flattened_dict.items():
                 actions.append(
-                    TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}"), str(v))
+                    TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding), str(v).encode(self.encoding))
                 )
 
             await communicator.txn(
                 EtcdTransactionAction().and_then(actions).or_else([])
             )
 
     async def put_dict(
@@ -285,15 +289,15 @@
         :return:
         """
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
 
         actions = []
         for k, v in flattened_dict_obj.items():
             actions.append(
-                TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}"), str(v))
+                TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding), str(v).encode(self.encoding))
             )
 
         async with self.etcd.connect() as communicator:
             await communicator.txn(
                 EtcdTransactionAction().and_then(actions).or_else([])
             )
 
@@ -333,18 +337,18 @@
             scope_prefixes = [_scope_prefix_map[ConfigScopes.GLOBAL]]
         else:
             raise ValueError("Invalid scope prefix value")
 
         async with self.etcd.connect() as communicator:
             for scope_prefix in scope_prefixes:
                 value = await communicator.get(
-                    self._mangle_key(f"{_slash(scope_prefix)}{key}")
+                    self._mangle_key(f"{_slash(scope_prefix)}{key}").encode(self.encoding)
                 )
                 if value is not None:
-                    return value
+                    return bytes(value).decode(self.encoding)
         return None
 
     async def get_prefix(
         self,
         key_prefix: str,
         *,
         scope: ConfigScopes = ConfigScopes.MERGED,
@@ -405,17 +409,17 @@
             raise ValueError("Invalid scope prefix value")
         pair_sets: List[List[Mapping | Tuple]] = []
         async with self.etcd.connect() as communicator:
             for scope_prefix in scope_prefixes:
                 mangled_key_prefix = self._mangle_key(
                     f"{_slash(scope_prefix)}{key_prefix}"
                 )
-                values = await communicator.get_prefix(mangled_key_prefix)
+                values = await communicator.get_prefix(mangled_key_prefix.encode(self.encoding))
                 pair_sets.append(
-                    [(self._demangle_key(k), v) for k, v in values.items()]
+                    [(self._demangle_key(bytes(k).decode(self.encoding)), bytes(v).decode(self.encoding)) for k, v in values]
                 )
 
         configs = [
             make_dict_from_pairs(f"{_slash(scope_prefix)}{key_prefix}", pairs, "/")
             for scope_prefix, pairs in zip(scope_prefixes, pair_sets)
         ]
         return ChainMap(*configs)
@@ -436,18 +440,18 @@
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
 
         async with self.etcd.connect() as communicator:
             result = await communicator.txn(
                 EtcdTransactionAction()
                 .when(
                     [
-                        Compare.value(mangled_key, CompareOp.EQUAL, initial_val),
+                        Compare.value(mangled_key.encode(self.encoding), CompareOp.EQUAL, initial_val.encode(self.encoding)),
                     ]
                 )
-                .and_then([TxnOp.put(mangled_key, new_val)])
+                .and_then([TxnOp.put(mangled_key.encode(self.encoding), new_val.encode(self.encoding))])
                 .or_else([])
             )
 
             return result.succeeded()
 
     async def delete(
         self,
@@ -455,43 +459,43 @@
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         async with self.etcd.connect() as communicator:
-            await communicator.delete(mangled_key)
+            await communicator.delete(mangled_key.encode(self.encoding))
 
     async def delete_multi(
         self,
         keys: Iterable[str],
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         async with self.etcd.connect() as communicator:
             actions = []
             for k in keys:
                 actions.append(
-                    TxnOp.delete(self._mangle_key(f"{_slash(scope_prefix)}{k}"))
+                    TxnOp.delete(self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding))
                 )
             communicator.txn(EtcdTransactionAction().and_then(actions).or_else([]))
 
     async def delete_prefix(
         self,
         key_prefix: str,
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key_prefix = self._mangle_key(f"{_slash(scope_prefix)}{key_prefix}")
         async with self.etcd.connect() as communicator:
-            await communicator.delete_prefix(mangled_key_prefix)
+            await communicator.delete_prefix(mangled_key_prefix.encode(self.encoding))
 
     async def _watch_impl(
         self,
         iterator_factory: Callable[[EtcdCommunicator], AsyncIterator[WatchEvent]],
         scope_prefix_len: int,
         once: bool,
         cleanup_event: Optional[CondVar] = None,
@@ -504,15 +508,15 @@
                     if wait_timeout is not None:
                         try:
                             ev = await asyncio.wait_for(
                                 iterator.__anext__(), wait_timeout
                             )
                         except asyncio.TimeoutError:
                             pass
-                    yield Event(ev.key[scope_prefix_len:], ev.event, ev.value)
+                    yield Event(bytes(ev.key).decode(self.encoding)[scope_prefix_len:], ev.event, bytes(ev.value).decode(self.encoding))
                     if once:
                         return
         finally:
             if cleanup_event:
                 cleanup_event.notify_waiters()
 
     async def watch(
@@ -531,28 +535,28 @@
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         ended_without_error = False
 
         while not ended_without_error:
             try:
                 async for ev in self._watch_impl(
                     lambda communicator: communicator.watch(
-                        mangled_key,
+                        mangled_key.encode(self.encoding),
                         ready_event=ready_event,
                     ),
                     scope_prefix_len,
                     once,
                     cleanup_event=cleanup_event,
                     wait_timeout=wait_timeout,
                 ):
                     yield ev
                 ended_without_error = True
-            except GRpcStatusError as e:
+            except GRPCStatusError as e:
                 err_detail = e.args[0]
 
-                if err_detail["code"] == GRpcStatusCode.Unavailable:
+                if err_detail["code"] == GRPCStatusCode.Unavailable:
                     log.warn(
                         "watch(): error while connecting to Etcd server, retrying..."
                     )
                     await asyncio.sleep(self.watch_reconnect_intvl)
                     ended_without_error = False
                 else:
                     raise
@@ -573,28 +577,28 @@
         mangled_key_prefix = self._mangle_key(f"{_slash(scope_prefix)}{key_prefix}")
         ended_without_error = False
 
         while not ended_without_error:
             try:
                 async for ev in self._watch_impl(
                     lambda communicator: communicator.watch_prefix(
-                        mangled_key_prefix,
+                        mangled_key_prefix.encode(self.encoding),
                         ready_event=ready_event,
                     ),
                     scope_prefix_len,
                     once,
                     cleanup_event=cleanup_event,
                     wait_timeout=wait_timeout,
                 ):
                     yield ev
                 ended_without_error = True
-            except GRpcStatusError as e:
+            except GRPCStatusError as e:
                 err_detail = e.args[0]
 
-                if err_detail["code"] == GRpcStatusCode.Unavailable:
+                if err_detail["code"] == GRPCStatusCode.Unavailable:
                     log.warn(
                         "watch_prefix(): error while connecting to Etcd server, retrying..."
                     )
                     await asyncio.sleep(self.watch_reconnect_intvl)
                     ended_without_error = False
                 else:
                     raise e
```

### Comparing `etcd_client_py-0.2.4/tests/test.py` & `etcd_client_py-0.3.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/Cargo.lock` & `etcd_client_py-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
  "tonic-build",
  "tower",
  "tower-service",
 ]
 
 [[package]]
 name = "etcd-client-py"
-version = "0.2.4"
+version = "0.3.0"
 dependencies = [
  "etcd-client",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tokio-stream",
  "tonic",
```

### Comparing `etcd_client_py-0.2.4/pyproject.toml` & `etcd_client_py-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `etcd_client_py-0.2.4/PKG-INFO` & `etcd_client_py-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: etcd-client-py
-Version: 0.2.4
+Version: 0.3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Summary: Yet another etcd-client API binding based on the Rust's etcd-client package
 Keywords: etcd,binding,rust,etcd-client
 Author: Sanghyeon Seo, Joongi Kim
 Author-email: seosh@lablup.com, joongi@lablup.com
```

