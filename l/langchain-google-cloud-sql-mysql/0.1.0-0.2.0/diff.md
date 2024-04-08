# Comparing `tmp/langchain_google_cloud_sql_mysql-0.1.0-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_mysql-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 21310 bytes, number of entries: 11
--rw-r--r--  2.0 unx      879 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/__init__.py
--rw-r--r--  2.0 unx     4647 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/chat_message_history.py
--rw-r--r--  2.0 unx    11012 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/engine.py
--rw-r--r--  2.0 unx    11939 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Feb-26 18:26 langchain_google_cloud_sql_mysql/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Feb-26 18:28 langchain_google_cloud_sql_mysql-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    17611 b- defN 24-Feb-26 18:28 langchain_google_cloud_sql_mysql-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-26 18:28 langchain_google_cloud_sql_mysql-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Feb-26 18:28 langchain_google_cloud_sql_mysql-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1120 b- defN 24-Feb-26 18:28 langchain_google_cloud_sql_mysql-0.1.0.dist-info/RECORD
-11 files, 59288 bytes uncompressed, 19348 bytes compressed:  67.4%
+Zip file size: 29964 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/__init__.py
+-rw-r--r--  2.0 unx     4636 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/chat_message_history.py
+-rw-r--r--  2.0 unx    14907 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/engine.py
+-rw-r--r--  2.0 unx     3430 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/indexes.py
+-rw-r--r--  2.0 unx    11912 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/py.typed
+-rw-r--r--  2.0 unx    29952 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/vectorstore.py
+-rw-r--r--  2.0 unx      597 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18482 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1326 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD
+13 files, 97876 bytes uncompressed, 27670 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -3,32 +3,38 @@
 
 Filename: langchain_google_cloud_sql_mysql/chat_message_history.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_mysql/engine.py
 Comment: 
 
+Filename: langchain_google_cloud_sql_mysql/indexes.py
+Comment: 
+
 Filename: langchain_google_cloud_sql_mysql/loader.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_mysql/py.typed
 Comment: 
 
+Filename: langchain_google_cloud_sql_mysql/vectorstore.py
+Comment: 
+
 Filename: langchain_google_cloud_sql_mysql/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.1.0.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.1.0.dist-info/METADATA
+Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.1.0.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.1.0.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.1.0.dist-info/RECORD
+Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_mysql/__init__.py

```diff
@@ -9,18 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .chat_message_history import MySQLChatMessageHistory
-from .engine import MySQLEngine
+from .engine import Column, MySQLEngine
+from .indexes import DistanceMeasure, IndexType, QueryOptions, SearchType, VectorIndex
 from .loader import MySQLDocumentSaver, MySQLLoader
+from .vectorstore import MySQLVectorStore
 from .version import __version__
 
 __all__ = [
+    "Column",
+    "DistanceMeasure",
+    "IndexType",
     "MySQLChatMessageHistory",
     "MySQLDocumentSaver",
     "MySQLEngine",
     "MySQLLoader",
+    "MySQLVectorStore",
+    "QueryOptions",
+    "SearchType",
+    "VectorIndex",
     "__version__",
 ]
```

## langchain_google_cloud_sql_mysql/chat_message_history.py

```diff
@@ -21,15 +21,15 @@
 from .engine import MySQLEngine
 
 
 class MySQLChatMessageHistory(BaseChatMessageHistory):
     """Chat message history stored in a Cloud SQL MySQL database.
 
     Args:
-        engine (MySQLEngine): SQLAlchemy connection pool engine for managing
+        engine (MySQLEngine): Connection pool engine for managing
             connections to Cloud SQL for MySQL.
         session_id (str): Arbitrary key that is used to store the messages
             of a single chat session.
         table_name (str): The name of the table to use for storing/retrieving
             the chat message history.
     """
```

## langchain_google_cloud_sql_mysql/engine.py

```diff
@@ -27,14 +27,29 @@
 
 if TYPE_CHECKING:
     import google.auth.credentials
     import pymysql
 
 USER_AGENT = "langchain-google-cloud-sql-mysql-python/" + __version__
 
+from dataclasses import dataclass
+
+
+@dataclass
+class Column:
+    name: str
+    data_type: str
+    nullable: bool = True
+
+    def __post_init__(self):
+        if not isinstance(self.name, str):
+            raise ValueError("Column name must be type string")
+        if not isinstance(self.data_type, str):
+            raise ValueError("Column data_type must be type string")
+
 
 def _get_iam_principal_email(
     credentials: google.auth.credentials.Credentials,
 ) -> str:
     """Get email address associated with current authenticated IAM principal.
 
     Email will be used for automatic IAM database authentication to Cloud SQL.
@@ -202,14 +217,41 @@
 
         Returns:
             (sqlalchemy.engine.Connection): a single DBAPI connection checked
                 out from the connection pool.
         """
         return self.engine.connect()
 
+    def _execute(self, query: str, params: Optional[dict] = None) -> None:
+        """Executes a SQL query within a transaction."""
+        with self.engine.connect() as conn:
+            conn.execute(sqlalchemy.text(query), params)
+            conn.commit()
+
+    def _execute_outside_tx(self, query: str, params: Optional[dict] = None) -> None:
+        """Executes a SQL query with autocommit (outside of transaction)."""
+        with self.engine.connect() as conn:
+            conn = conn.execution_options(isolation_level="AUTOCOMMIT")
+            conn.execute(sqlalchemy.text(query), params)
+
+    def _fetch(self, query: str, params: Optional[dict] = None):
+        """Fetch results from a SQL query."""
+        with self.engine.connect() as conn:
+            result = conn.execute(sqlalchemy.text(query), params)
+            result_map = result.mappings()
+            result_fetch = result_map.fetchall()
+            return result_fetch
+
+    def _fetch_rows(self, query: str, params: Optional[dict] = None):
+        """Fetch results from a SQL query as rows."""
+        with self.engine.connect() as conn:
+            result = conn.execute(sqlalchemy.text(query), params)
+            result_fetch = result.fetchall()  # Directly fetch rows
+            return result_fetch
+
     def init_chat_history_table(self, table_name: str) -> None:
         """Create table with schema required for MySQLChatMessageHistory class.
 
         Required schema is as follows:
 
             CREATE TABLE {table_name} (
                 id INT AUTO_INCREMENT PRIMARY KEY,
@@ -289,7 +331,55 @@
 
         Returns:
             (sqlalchemy.Table): The loaded table.
         """
         metadata = sqlalchemy.MetaData()
         sqlalchemy.MetaData.reflect(metadata, bind=self.engine, only=[table_name])
         return metadata.tables[table_name]
+
+    def init_vectorstore_table(
+        self,
+        table_name: str,
+        vector_size: int,
+        content_column: str = "content",
+        embedding_column: str = "embedding",
+        metadata_columns: List[Column] = [],
+        metadata_json_column: str = "langchain_metadata",
+        id_column: str = "langchain_id",
+        overwrite_existing: bool = False,
+        store_metadata: bool = True,
+    ) -> None:
+        """
+        Create a table for saving of vectors to be used with MySQLVectorStore.
+
+        Args:
+            table_name (str): The MySQL database table name.
+            vector_size (int): Vector size for the embedding model to be used.
+            content_column (str): Name of the column to store document content.
+                Default: `page_content`.
+            embedding_column (str) : Name of the column to store vector embeddings.
+                Default: `embedding`.
+            metadata_columns (List[Column]): A list of Columns to create for custom
+                metadata. Default: []. Optional.
+            metadata_json_column (str): The column to store extra metadata in JSON format.
+                Default: `langchain_metadata`. Optional.
+            id_column (str):  Name of the column to store ids.
+                Default: `langchain_id`. Optional,
+            overwrite_existing (bool): Whether to drop existing table. Default: False.
+            store_metadata (bool): Whether to store metadata in the table.
+                Default: True.
+        """
+        query = f"""CREATE TABLE `{table_name}`(
+            `{id_column}` CHAR(36) PRIMARY KEY,
+            `{content_column}` TEXT NOT NULL,
+            `{embedding_column}` vector({vector_size}) USING VARBINARY NOT NULL"""
+        for column in metadata_columns:
+            nullable = "NOT NULL" if not column.nullable else ""
+            query += f",\n`{column.name}` {column.data_type} {nullable}"
+        if store_metadata:
+            query += f""",\n`{metadata_json_column}` JSON"""
+        query += "\n);"
+
+        with self.engine.connect() as conn:
+            if overwrite_existing:
+                conn.execute(sqlalchemy.text(f"DROP TABLE IF EXISTS `{table_name}`"))
+            conn.execute(sqlalchemy.text(query))
```

## langchain_google_cloud_sql_mysql/loader.py

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
-from collections.abc import Iterable
-from typing import Any, Dict, Iterator, List, Optional, Sequence, cast
+from typing import Any, Dict, Iterable, Iterator, List, Optional, cast
 
 import pymysql
 import sqlalchemy
 from langchain_community.document_loaders.base import BaseLoader
 from langchain_core.documents import Document
 
 from .engine import MySQLEngine
@@ -26,15 +25,15 @@
 DEFAULT_METADATA_COL = "langchain_metadata"
 
 
 def _parse_doc_from_row(
     content_columns: Iterable[str],
     metadata_columns: Iterable[str],
     row: Dict,
-    metadata_json_column: str = DEFAULT_METADATA_COL,
+    metadata_json_column: Optional[str] = DEFAULT_METADATA_COL,
 ) -> Document:
     page_content = " ".join(
         str(row[column]) for column in content_columns if column in row
     )
     metadata: Dict[str, Any] = {}
     # unnest metadata from langchain_metadata column
     if row.get(metadata_json_column):
```

## langchain_google_cloud_sql_mysql/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## Comparing `langchain_google_cloud_sql_mysql-0.1.0.dist-info/LICENSE` & `langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_mysql-0.1.0.dist-info/METADATA` & `langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-mysql
-Version: 0.1.0
+Version: 0.2.0
 Summary: LangChain integrations for Google Cloud SQL for MySQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -211,22 +211,23 @@
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/blob/main/CHANGELOG.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
+Requires-Dist: numpy <2.0.0,>=1.24.4
 Requires-Dist: SQLAlchemy <3.0.0,>=2.0.7
 Requires-Dist: cloud-sql-python-connector[pymysql] <2.0.0,>=1.7.0
 Provides-Extra: test
-Requires-Dist: black[jupyter] ==24.2.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==24.3.0 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.8.0 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.5 ; extra == 'test'
-Requires-Dist: pytest ==8.0.1 ; extra == 'test'
+Requires-Dist: mypy ==1.9.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
+Requires-Dist: pytest ==8.1.1 ; extra == 'test'
 
 # Cloud SQL for MySQL for LangChain
 
 This package contains the [LangChain][langchain] integrations for Cloud SQL for MySQL.
 
 > **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
 
@@ -255,14 +256,38 @@
 ```bash
 pip install virtualenv
 virtualenv <your-env>
 source <your-env>/bin/activate
 <your-env>/bin/pip install langchain-google-cloud-sql-mysql
 ```
 
+## Vector Store Usage
+
+Use a [vector store](https://python.langchain.com/docs/modules/data_connection/vectorstores/) to store
+embedded data and perform vector search.
+
+```python
+from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLVectorStore
+from langchain_google_vertexai import VertexAIEmbeddings
+
+
+engine = MySQLEngine.from_instance("project-id", "region", "my-instance", "my-database")
+engine.init_vectorstore_table(
+    table_name="my-table-name",
+    vector_size=768,  # Vector size for `VertexAIEmbeddings()`
+)
+vectorstore = MySQLVectorStore(
+    engine,
+    embedding_service=VertextAIEmbeddings(),
+    table_name="my-table-name",
+)
+```
+
+See the full [Vector Store][vectorstore] tutorial.
+
 ## Document Loader Usage
 
 Use a [document loader](https://python.langchain.com/docs/modules/data_connection/document_loaders/) to load data as LangChain `Document`s.
 
 ```python
 from langchain_google_cloud_sql_mysql import MySQLEngine, MySQLLoader
 
@@ -317,7 +342,8 @@
 [billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 [api]: https://console.cloud.google.com/flows/enableapi?apiid=sqladmin.googleapis.com
 [auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
 [venv]: https://virtualenv.pypa.io/en/latest/
 [loader]: ./docs/document_loader.ipynb
 [history]: ./docs/chat_message_history.ipynb
 [langchain]: https://github.com/langchain-ai/langchain
+[vectorstore]: https://github.com/googleapis/langchain-google-cloud-sql-mysql-python/tree/main/docs/vector_store.ipynb
```

