# Comparing `tmp/hugegraph-python-1.0.0.9.tar.gz` & `tmp/hugegraph-python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.9.tar", last modified: Thu Jun 15 09:07:19 2023, max compression
+gzip compressed data, was "hugegraph-python-1.3.0.tar", last modified: Tue Apr  9 10:28:59 2024, max compression
```

## Comparing `hugegraph-python-1.0.0.9.tar` & `hugegraph-python-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,67 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.831722 hugegraph-python-1.0.0.9/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.9/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1350 2023-06-15 09:07:19.831280 hugegraph-python-1.0.0.9/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      866 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.9/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.810373 hugegraph-python-1.0.0.9/hugegraph/
--rw-rw-r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/hugegraph/__init__.py
--rw-rw-r--   0 zsm        (501) staff       (20)     3731 2023-06-15 09:06:22.000000 hugegraph-python-1.0.0.9/hugegraph/connection.py
--rw-r--r--   0 zsm        (501) staff       (20)     1070 2023-04-14 07:32:18.000000 hugegraph-python-1.0.0.9/hugegraph/constants.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.813068 hugegraph-python-1.0.0.9/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1350 2023-06-15 09:07:19.000000 hugegraph-python-1.0.0.9/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      856 2023-06-15 09:07:19.000000 hugegraph-python-1.0.0.9/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 09:07:19.000000 hugegraph-python-1.0.0.9/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)       36 2023-06-15 09:07:19.000000 hugegraph-python-1.0.0.9/hugegraph_python.egg-info/top_level.txt
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.816110 hugegraph-python-1.0.0.9/manager/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/manager/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     2136 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.9/manager/common.py
--rw-rw-r--   0 zsm        (501) staff       (20)    13726 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.9/manager/graph_manager.py
--rw-r--r--   0 zsm        (501) staff       (20)     1677 2023-06-15 02:47:44.000000 hugegraph-python-1.0.0.9/manager/gremlin_manager.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.819787 hugegraph-python-1.0.0.9/manager/schema/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/manager/schema/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     6471 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.9/manager/schema/edge_label.py
--rw-r--r--   0 zsm        (501) staff       (20)     4158 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.9/manager/schema/index_label.py
--rw-r--r--   0 zsm        (501) staff       (20)     6540 2023-04-14 07:47:12.000000 hugegraph-python-1.0.0.9/manager/schema/property_key.py
--rw-r--r--   0 zsm        (501) staff       (20)     6555 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.9/manager/schema/vertex_label.py
--rw-rw-r--   0 zsm        (501) staff       (20)     6366 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.9/manager/schema_manager.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.825067 hugegraph-python-1.0.0.9/models/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/models/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     2038 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.9/models/edge_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     2203 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.9/models/edge_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1973 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.9/models/index_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1609 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.9/models/property_key_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1317 2023-04-18 04:39:59.000000 hugegraph-python-1.0.0.9/models/respon_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1503 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.9/models/vertex_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1989 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.9/models/vertex_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 09:07:19.831854 hugegraph-python-1.0.0.9/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 09:07:06.000000 hugegraph-python-1.0.0.9/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.827139 hugegraph-python-1.0.0.9/test/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/test/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)      624 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.9/test/test.py
--rw-r--r--   0 zsm        (501) staff       (20)     1959 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.9/test/test_df.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:07:19.830809 hugegraph-python-1.0.0.9/utils/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.9/utils/__init__.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1532 2023-04-14 04:34:09.000000 hugegraph-python-1.0.0.9/utils/exceptions.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1745 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.9/utils/huge_decorator.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1221 2023-04-13 11:39:44.000000 hugegraph-python-1.0.0.9/utils/huge_requests.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1474 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.9/utils/util.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.889299 hugegraph-python-1.3.0/
+-rw-r--r--   0 zsm        (501) staff       (20)     2473 2024-04-09 10:28:59.889092 hugegraph-python-1.3.0/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)     1883 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/README.md
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2024-04-09 10:28:59.889335 hugegraph-python-1.3.0/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1787 2024-04-09 10:23:13.000000 hugegraph-python-1.3.0/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.875947 hugegraph-python-1.3.0/src/
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.888836 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     2473 2024-04-09 10:28:59.000000 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)     1924 2024-04-09 10:28:59.000000 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2024-04-09 10:28:59.000000 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       68 2024-04-09 10:28:59.000000 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/requires.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       18 2024-04-09 10:28:59.000000 hugegraph-python-1.3.0/src/hugegraph_python.egg-info/top_level.txt
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.877684 hugegraph-python-1.3.0/src/pyhugegraph/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/__init__.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.880777 hugegraph-python-1.3.0/src/pyhugegraph/api/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)    13242 2024-02-29 11:53:10.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/auth.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2219 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/common.py
+-rw-r--r--   0 zsm        (501) staff       (20)    13668 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/graph.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2961 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/graphs.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2051 2024-02-20 11:40:22.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/gremlin.py
+-rw-r--r--   0 zsm        (501) staff       (20)     4625 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/metric.py
+-rw-r--r--   0 zsm        (501) staff       (20)     7346 2024-02-20 11:40:22.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.882231 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6760 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/edge_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     4281 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/index_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     7077 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/property_key.py
+-rw-r--r--   0 zsm        (501) staff       (20)     7087 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/vertex_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2839 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/task.py
+-rw-r--r--   0 zsm        (501) staff       (20)    11910 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/traverser.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2721 2024-02-20 10:46:00.000000 hugegraph-python-1.3.0/src/pyhugegraph/api/variable.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2971 2024-02-20 10:43:36.000000 hugegraph-python-1.3.0/src/pyhugegraph/client.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.883014 hugegraph-python-1.3.0/src/pyhugegraph/example/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/example/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2749 2024-03-08 08:35:35.000000 hugegraph-python-1.3.0/src/pyhugegraph/example/hugegraph_example.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1812 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/example/hugegraph_test.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.885211 hugegraph-python-1.3.0/src/pyhugegraph/structure/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2026 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/edge_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2469 2024-02-20 10:36:03.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/edge_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1708 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/graph_instance.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2051 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/gremlin_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1964 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/index_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1599 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/property_key_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1305 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/response_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1491 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/vertex_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2179 2024-02-20 10:36:03.000000 hugegraph-python-1.3.0/src/pyhugegraph/structure/vertex_label_data.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.886361 hugegraph-python-1.3.0/src/pyhugegraph/utils/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)      908 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/constants.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1504 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/exceptions.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1813 2024-02-20 11:40:22.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/huge_decorator.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1255 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/huge_requests.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1785 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/pyhugegraph/utils/util.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.876016 hugegraph-python-1.3.0/src/tests/
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-04-09 10:28:59.888557 hugegraph-python-1.3.0/src/tests/api/
+-rw-r--r--   0 zsm        (501) staff       (20)      785 2024-02-20 09:30:26.000000 hugegraph-python-1.3.0/src/tests/api/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     7827 2024-03-08 08:24:08.000000 hugegraph-python-1.3.0/src/tests/api/test_auth.py
+-rw-r--r--   0 zsm        (501) staff       (20)     7458 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/tests/api/test_graph.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1880 2024-02-20 10:36:03.000000 hugegraph-python-1.3.0/src/tests/api/test_graphs.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2863 2024-02-20 11:32:15.000000 hugegraph-python-1.3.0/src/tests/api/test_gremlin.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2501 2024-02-20 10:36:03.000000 hugegraph-python-1.3.0/src/tests/api/test_metric.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2669 2024-02-20 11:26:48.000000 hugegraph-python-1.3.0/src/tests/api/test_schema.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1982 2024-02-20 10:36:03.000000 hugegraph-python-1.3.0/src/tests/api/test_task.py
+-rw-r--r--   0 zsm        (501) staff       (20)     9514 2024-02-29 11:53:02.000000 hugegraph-python-1.3.0/src/tests/api/test_traverser.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2600 2024-02-20 11:32:15.000000 hugegraph-python-1.3.0/src/tests/api/test_variable.py
```

### Comparing `hugegraph-python-1.0.0.9/hugegraph/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/hugegraph/constants.py` & `hugegraph-python-1.3.0/src/pyhugegraph/utils/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-class Graph(str):
+class Constants(str):
     CONFORM_MESSAGE = "I%27m+sure+to+delete+all+data"
-    HEADER_USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 " \
-                        "(KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36"
     HEADER_CONTENT_TYPE = "application/json"
```

### Comparing `hugegraph-python-1.0.0.9/manager/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/manager/common.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,56 +10,52 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-from hugegraph.constants import Graph
+from pyhugegraph.utils.constants import Constants
 
 
 class ParameterHolder:
     def __init__(self):
         self._dic = {}
 
     def set(self, key, value):
         self._dic[key] = value
 
     def get_value(self, key):
         if key not in self._dic:
             return None
-        else:
-            return self._dic[key]
+        return self._dic[key]
 
     def get_dic(self):
         return self._dic
 
     def get_keys(self):
         return self._dic.keys()
 
 
-class HugeGraphBase:
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        self._ip = ip
-        self._port = port
-        self._user = user
-        self._pwd = pwd
-        self._host = "http://{}:{}".format(ip, port)
-        self._auth = (user, pwd)
-        self._graph_name = graph_name
+class HugeParamsBase:
+    def __init__(self, graph_instance):
+        self._graph_instance = graph_instance
+        self._ip = graph_instance.ip
+        self._port = graph_instance.port
+        self._user = graph_instance.user_name
+        self._pwd = graph_instance.passwd
+        self._host = f"http://{graph_instance.ip}:{graph_instance.port}"
+        self._auth = (graph_instance.user_name, graph_instance.passwd)
+        self._graph_name = graph_instance.graph_name
         self._parameter_holder = None
-        self._headers = {
-            'User-Agent': Graph.HEADER_USER_AGENT,
-            'Content-Type': Graph.HEADER_CONTENT_TYPE
-        }
-        self._timeout = timeout
+        self._headers = {"Content-Type": Constants.HEADER_CONTENT_TYPE}
+        self._timeout = graph_instance.timeout
 
     def add_parameter(self, key, value):
         self._parameter_holder.set(key, value)
-        return
 
     def get_parameter_holder(self):
         return self._parameter_holder
 
     def create_parameter_holder(self):
         self._parameter_holder = ParameterHolder()
```

### Comparing `hugegraph-python-1.0.0.9/manager/graph_manager.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,287 +13,365 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import json
 
-from utils.huge_requests import HugeSession
-from manager.common import HugeGraphBase
-from models.vertex_data import VertexData
-from models.edge_data import EdgeData
-from utils.exceptions import NotFoundError, CreateError, RemoveError, UpdateError
-from utils.util import create_exception, authorized
-
-
-class GraphManager(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
-        self.session = None
-        self.set_session(HugeSession.new_session())
-
-    def set_session(self, session):
-        self.session = session
-
-    def close_session(self):
-        if self.session:
-            self.session.close()
+from pyhugegraph.utils.huge_requests import HugeSession
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.structure.vertex_data import VertexData
+from pyhugegraph.structure.edge_data import EdgeData
+from pyhugegraph.utils.exceptions import (
+    NotFoundError,
+    CreateError,
+    RemoveError,
+    UpdateError,
+)
+from pyhugegraph.utils.util import (
+    create_exception,
+    check_if_authorized,
+    check_if_success,
+)
+
+
+class GraphManager(HugeParamsBase):
+    def __init__(self, graph_instance):
+        super().__init__(graph_instance)
+        self.__session = HugeSession.new_session()
 
     def close(self):
-        self.close_session()
+        if self.__session:
+            self.__session.close()
 
-    def addVertex(self, label, properties):
-        data = dict()
-        data['label'] = label
+    def addVertex(self, label, properties, id=None):
+        data = {}
+        if id is not None:
+            data["id"] = id
+        data["label"] = label
         data["properties"] = properties
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices"
-        response = self.session.post(url, data=json.dumps(data), auth=self._auth,
-                                     headers=self._headers, timeout=self._timeout)
-        if response.status_code == 201 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/vertices"
+        response = self.__session.post(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, CreateError(f"create vertex failed: {str(response.content)}")
+        ):
             res = VertexData(json.loads(response.content))
             return res
-        else:
-            raise CreateError("create vertex failed: {}".format(response.content))
+        return None
 
     def addVertices(self, input_data):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices/batch"
+        url = f"{self._host}/graphs/{self._graph_name}/graph/vertices/batch"
+
         data = []
         for item in input_data:
-            data.append({'label': item[0], 'properties': item[1]})
-        response = self.session.post(url, data=json.dumps(data), auth=self._auth,
-                                     headers=self._headers, timeout=self._timeout)
-        if response.status_code == 201 and authorized(response):
+            data.append({"label": item[0], "properties": item[1]})
+        response = self.__session.post(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, CreateError(f"create vertexes failed: {str(response.content)}")
+        ):
             res = []
             for item in json.loads(response.content):
                 res.append(VertexData({"id": item}))
             return res
-        else:
-            raise CreateError("create vertexes failed: {}".format(response.content))
+        return None
 
     def appendVertex(self, vertex_id, properties):
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/graph/vertices/\"" + vertex_id + "\"?action=append"
-        data = {
-            "properties": properties
-        }
-        response = self.session.put(url, data=json.dumps(data), auth=self._auth,
-                                    headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = f'{self._host}/graphs/{self._graph_name}/graph/vertices/"{vertex_id}"?action=append'
+
+        data = {"properties": properties}
+        response = self.__session.put(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, UpdateError(f"append vertex failed: {str(response.content)}")
+        ):
             res = VertexData(json.loads(response.content))
             return res
-        else:
-            raise UpdateError("append vertex failed: {}".format(response.content))
+        return None
 
     def eliminateVertex(self, vertex_id, properties):
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/graph/vertices/\"" + vertex_id + "\"?action=eliminate"
-        data = {
-            "properties": properties
-        }
-        response = self.session.put(url, data=json.dumps(data), auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = (
+            f'{self._host}/graphs/{self._graph_name}/graph/vertices/"{vertex_id}"?action=eliminate'
+        )
+
+        data = {"properties": properties}
+        response = self.__session.put(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, UpdateError(f"eliminate vertex failed: {str(response.content)}")
+        ):
             res = VertexData(json.loads(response.content))
             return res
-        else:
-            raise UpdateError("eliminate vertex failed: {}".format(response.content))
+        return None
 
     def getVertexById(self, vertex_id):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices/\"" + vertex_id + "\""
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = f'{self._host}/graphs/{self._graph_name}/graph/vertices/"{vertex_id}"'
+
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, NotFoundError(f"Vertex not found: {str(response.content)}")):
             res = VertexData(json.loads(response.content))
             return res
-        else:
-            raise NotFoundError("Vertex not found: {}".format(response.content))
+        return None
+
+    def getVertexByPage(self, label, limit, page=None, properties=None):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/vertices?"
 
-    def getVertexByPage(self, label, limit, page, properties=None):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices?"
         para = ""
         para = para + "&label=" + label
         if properties:
             para = para + "&properties=" + json.dumps(properties)
         if page:
-            para += '&page={}'.format(page)
+            para += f"&page={page}"
         else:
-            para += '&page'
+            para += "&page"
         para = para + "&limit=" + str(limit)
         url = url + para[1:]
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, NotFoundError(f"Vertex not found: {str(response.content)}")):
             res = []
             for item in json.loads(response.content)["vertices"]:
                 res.append(VertexData(item))
             next_page = json.loads(response.content)["page"]
             return res, next_page
-        else:
-            raise NotFoundError("Vertex not found: {}".format(response.content))
+        return None
+
+    def getVertexByCondition(self, label="", limit=0, page=None, properties=None):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/vertices?"
 
-    def getVertexByCondition(self, label="",  limit=0, page='', properties=None):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices?"
         para = ""
         if label:
             para = para + "&label=" + label
         if properties:
             para = para + "&properties=" + json.dumps(properties)
         if limit > 0:
             para = para + "&limit=" + str(limit)
         if page:
-            para += '&page={}'.format(page)
+            para += f"&page={page}"
         else:
-            para += '&page'
+            para += "&page"
         url = url + para[1:]
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, NotFoundError(f"Vertex not found: {str(response.content)}")):
             res = []
             for item in json.loads(response.content)["vertices"]:
                 res.append(VertexData(item))
             return res
-        else:
-            raise NotFoundError("Vertex not found: {}".format(response.content))
+        return None
 
     def removeVertexById(self, vertex_id):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/vertices/\"" + vertex_id + "\""
-        response = self.session.delete(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 204 and authorized(response):
+        url = f'{self._host}/graphs/{self._graph_name}/graph/vertices/"{vertex_id}"'
+        response = self.__session.delete(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(
+            response, RemoveError(f"remove vertex failed: {str(response.content)}")
+        ):
             return response.content
-        else:
-            raise RemoveError("remove vertex failed: {}".format(response.content))
+        return None
 
     def addEdge(self, edge_label, out_id, in_id, properties):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/edges"
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges"
+
         data = {
             "label": edge_label,
             "outV": out_id,
             "inV": in_id,
-            "properties": properties
+            "properties": properties,
         }
-        response = self.session.post(url, data=json.dumps(data), auth=self._auth,
-                                     headers=self._headers, timeout=self._timeout)
-        if response.status_code == 201 and authorized(response):
+        response = self.__session.post(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(response, CreateError(f"created edge failed: {str(response.content)}")):
             res = EdgeData(json.loads(response.content))
             return res
-        else:
-            raise CreateError("created edge failed: {}".format(response.content))
+        return None
 
     def addEdges(self, input_data):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/edges/batch"
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges/batch"
+
         data = []
         for item in input_data:
-            data.append({'label': item[0], 'outV': item[1], 'inV': item[2], 'outVLabel': item[3],
-                         'inVLabel': item[4], 'properties': item[5]})
-        response = self.session.post(url, data=json.dumps(data), auth=self._auth,
-                                     headers=self._headers, timeout=self._timeout)
-        if response.status_code == 201 and authorized(response):
+            data.append(
+                {
+                    "label": item[0],
+                    "outV": item[1],
+                    "inV": item[2],
+                    "outVLabel": item[3],
+                    "inVLabel": item[4],
+                    "properties": item[5],
+                }
+            )
+        response = self.__session.post(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, CreateError(f"created edges failed:  {str(response.content)}")
+        ):
             res = []
             for item in json.loads(response.content):
                 res.append(EdgeData({"id": item}))
             return res
-        else:
-            raise CreateError("created edges failed:  {}".format(response.content))
+        return None
 
     def appendEdge(self, edge_id, properties):
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/graph/edges/" + edge_id + "?action=append"
-        data = {
-            "properties": properties
-        }
-        response = self.session.put(url, data=json.dumps(data), auth=self._auth,
-                                    headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges/{edge_id}?action=append"
+
+        data = {"properties": properties}
+        response = self.__session.put(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(response, UpdateError(f"append edge failed: {str(response.content)}")):
             res = EdgeData(json.loads(response.content))
             return res
-        else:
-            raise UpdateError("append edge failed: {}".format(response.content))
+        return None
 
     def eliminateEdge(self, edge_id, properties):
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/graph/edges/" + edge_id + "?action=eliminate"
-        data = {
-            "properties": properties
-        }
-        response = self.session.put(url, data=json.dumps(data), auth=self._auth,
-                                    headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges/{edge_id}?action=eliminate"
+
+        data = {"properties": properties}
+        response = self.__session.put(
+            url,
+            data=json.dumps(data),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        if check_if_success(
+            response, UpdateError(f"eliminate edge failed: {str(response.content)}")
+        ):
             res = EdgeData(json.loads(response.content))
             return res
-        else:
-            raise UpdateError("eliminate edge failed: {}".format(response.content))
+        return None
 
     def getEdgeById(self, edge_id):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/edges/" + edge_id
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges/{edge_id}"
+
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, NotFoundError(f"not found edge: {str(response.content)}")):
             res = EdgeData(json.loads(response.content))
             return res
-        else:
-            raise NotFoundError("not found edge: {}".format(response.content))
+        return None
+
+    def getEdgeByPage(
+        self,
+        label=None,
+        vertex_id=None,
+        direction=None,
+        limit=0,
+        page=None,
+        properties=None,
+    ):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges?"
 
-    def getEdgeByPage(self, label=None, vertex_id=None, direction=None, limit=0, page=None, properties=None):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/edges?"
         para = ""
         if vertex_id:
             if direction:
-                para = para + "&vertex_id=\"" + vertex_id + "\"&direction=" + direction
+                para = para + '&vertex_id="' + vertex_id + '"&direction=' + direction
             else:
                 raise NotFoundError("Direction can not be empty.")
         if label:
             para = para + "&label=" + label
         if properties:
             para = para + "&properties=" + json.dumps(properties)
-        if page is not None:
-            if page:
-                para += '&page={}'.format(page)
-            else:
-                para += '&page'
+        if page:
+            para += f"&page={page}"
+        else:
+            para += "&page"
         if limit > 0:
             para = para + "&limit=" + str(limit)
         url = url + para[1:]
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, NotFoundError(f"not found edges: {str(response.content)}")):
             res = []
             for item in json.loads(response.content)["edges"]:
                 res.append(EdgeData(item))
             return res, json.loads(response.content)["page"]
-        else:
-            raise NotFoundError("not found edges: {}".format(response.content))
+        return None
 
     def removeEdgeById(self, edge_id):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/graph/edges/" + edge_id
-        response = self.session.delete(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 204 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/graph/edges/{edge_id}"
+
+        response = self.__session.delete(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if check_if_success(response, RemoveError(f"remove edge failed: {str(response.content)}")):
             return response.content
-        else:
-            raise RemoveError("remove edge failed: {}".format(response.content))
+        return None
 
     def getVerticesById(self, vertex_ids):
         if not vertex_ids:
             return []
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/traversers/vertices?"
+        url = f"{self._host}/graphs/{self._graph_name}/traversers/vertices?"
         for vertex_id in vertex_ids:
-            url += 'ids="{}"&'.format(vertex_id)
+            url += f'ids="{vertex_id}"&'
         url = url.rstrip("&")
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if response.status_code == 200 and check_if_authorized(response):
             res = []
             for item in json.loads(response.content)["vertices"]:
                 res.append(VertexData(item))
             return res
-        else:
-            create_exception(response.content)
+        create_exception(response.content)
+        return None
 
     def getEdgesById(self, edge_ids):
         if not edge_ids:
             return []
-        url = self._host + "/graphs" + "/" + self._graph_name \
-              + "/traversers/edges?"
+        url = f"{self._host}/graphs/{self._graph_name}/traversers/edges?"
         for vertex_id in edge_ids:
-            url += 'ids={}&'.format(vertex_id)
+            url += f"ids={vertex_id}&"
         url = url.rstrip("&")
-        response = self.session.get(url, auth=self._auth, headers=self._headers, timeout=self._timeout)
-        if response.status_code == 200 and authorized(response):
+        response = self.__session.get(
+            url, auth=self._auth, headers=self._headers, timeout=self._timeout
+        )
+        if response.status_code == 200 and check_if_authorized(response):
             res = []
             for item in json.loads(response.content)["edges"]:
                 res.append(EdgeData(item))
             return res
-        else:
-            create_exception(response.content)
+        create_exception(response.content)
+        return None
```

### Comparing `hugegraph-python-1.0.0.9/manager/gremlin_manager.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/gremlin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,54 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-import json
-import re
-
-import requests
-
-from manager.common import HugeGraphBase
-from models.respon_data import ResponseData
-from utils.exceptions import NotFoundError
-from utils.util import authorized
-
-
-class GremlinManager(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
-
-    def exec(self, gremlin):
-        gremlin = re.sub("^g", self._graph_name + ".traversal()", gremlin)
-        url = self._host + "/gremlin?gremlin=" + gremlin
-        response = requests.get(url, auth=self._auth, headers=self._headers)
-        if response.status_code == 200 and authorized(response):
-            return ResponseData(json.loads(response.content)).result
-        else:
-            raise NotFoundError("Gremlin can't get results: {}".format(response.content))
-
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+import json
+
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.structure.gremlin_data import GremlinData
+from pyhugegraph.structure.response_data import ResponseData
+from pyhugegraph.utils.exceptions import NotFoundError
+from pyhugegraph.utils.huge_requests import HugeSession
+from pyhugegraph.utils.util import check_if_success
+
+
+class GremlinManager(HugeParamsBase):
+    def __init__(self, graph_instance):
+        super().__init__(graph_instance)
+        self.__session = HugeSession.new_session()
+
+    def close(self):
+        if self.__session:
+            self.__session.close()
+
+    def exec(self, gremlin):
+        url = f"{self._host}/gremlin"
+        gremlin_data = GremlinData(gremlin)
+        gremlin_data.aliases = {
+            "graph": self._graph_name,
+            "g": "__g_" + self._graph_name,
+        }
+        response = self.__session.post(
+            url,
+            data=gremlin_data.to_json(),
+            auth=self._auth,
+            headers=self._headers,
+            timeout=self._timeout,
+        )
+        error = NotFoundError(f"Gremlin can't get results: {str(response.content)}")
+        if check_if_success(response, error):
+            return ResponseData(json.loads(response.content)).result
+        return ""
```

### Comparing `hugegraph-python-1.0.0.9/manager/schema/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/manager/schema/edge_label.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/property_key.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,145 +13,180 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import json
 
-import requests
 
-from manager.common import HugeGraphBase
-from utils.huge_decorator import decorator_params, decorator_create
-from utils.exceptions import CreateError, UpdateError, RemoveError
-from utils.util import authorized
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.utils.exceptions import CreateError, UpdateError, RemoveError
+from pyhugegraph.utils.huge_decorator import decorator_params, decorator_create
+from pyhugegraph.utils.util import check_if_success, check_if_authorized
 
 
-class EdgeLabel(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
+class PropertyKey(HugeParamsBase):
+    def __init__(self, graph_instance, session):
+        super().__init__(graph_instance)
+        self.__session = session
 
     @decorator_params
-    def link(self, source_label, target_label):
-        self._parameter_holder.set("source_label", source_label)
-        self._parameter_holder.set("target_label", target_label)
+    def asInt(self):
+        self._parameter_holder.set("data_type", "INT")
         return self
 
     @decorator_params
-    def sourceLabel(self, source_label):
-        self._parameter_holder.set("source_label", source_label)
+    def asText(self):
+        self._parameter_holder.set("data_type", "TEXT")
         return self
 
     @decorator_params
-    def targetLabel(self, target_label):
-        self._parameter_holder.set("target_label", target_label)
+    def asDouble(self):
+        self._parameter_holder.set("data_type", "DOUBLE")
         return self
 
     @decorator_params
-    def userdata(self, *args):
-        if not self._parameter_holder.get_value("user_data"):
-            self._parameter_holder.set('user_data', dict())
-        user_data = self._parameter_holder.get_value("user_data")
-        i = 0
-        while i < len(args):
-            user_data[args[i]] = args[i+1]
-            i += 2
+    def asDate(self):
+        self._parameter_holder.set("data_type", "DATE")
+        return self
+
+    @decorator_params
+    def valueSingle(self):
+        self._parameter_holder.set("cardinality", "SINGLE")
+        return self
+
+    @decorator_params
+    def valueList(self):
+        self._parameter_holder.set("cardinality", "LIST")
         return self
 
     @decorator_params
-    def properties(self, *args):
-        self._parameter_holder.set("properties", list(args))
+    def valueSet(self):
+        self._parameter_holder.set("cardinality", "SET")
         return self
 
     @decorator_params
-    def singleTime(self):
-        self._parameter_holder.set("frequency", "SINGLE")
+    def calcMax(self):
+        self._parameter_holder.set("aggregate_type", "MAX")
         return self
 
     @decorator_params
-    def multiTimes(self):
-        self._parameter_holder.set("frequency", "MULTIPLE")
+    def calcMin(self):
+        self._parameter_holder.set("aggregate_type", "MIN")
         return self
 
     @decorator_params
-    def sortKeys(self, *args):
-        self._parameter_holder.set("sort_keys", list(args))
+    def calcSum(self):
+        self._parameter_holder.set("aggregate_type", "SUM")
         return self
 
     @decorator_params
-    def nullableKeys(self, *args):
-        nullable_keys = set(args)
-        self._parameter_holder.set("nullable_keys", list(nullable_keys))
+    def calcOld(self):
+        self._parameter_holder.set("aggregate_type", "OLD")
         return self
 
     @decorator_params
+    def userdata(self, *args):
+        user_data = self._parameter_holder.get_value("user_data")
+        if not user_data:
+            self._parameter_holder.set("user_data", {})
+            user_data = self._parameter_holder.get_value("user_data")
+        i = 0
+        while i < len(args):
+            user_data[args[i]] = args[i + 1]
+            i += 2
+        return self
+
     def ifNotExist(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels" \
-              + "/" + self._parameter_holder.get_value("name")
-        response = requests.get(url)
-        if response.status_code == 200 and authorized(response):
+        url = (
+            f"{self._host}/graphs/{self._graph_name}/schema/propertykeys/"
+            f'{self._parameter_holder.get_value("name")}'
+        )
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        if response.status_code == 200 and check_if_authorized(response):
             self._parameter_holder.set("not_exist", False)
         return self
 
     @decorator_create
     def create(self):
         dic = self._parameter_holder.get_dic()
-        data = dict()
-        keys = ['name', 'source_label', 'target_label', 'nullable_keys', 'properties',
-                'enable_label_index', 'sort_keys', 'user_data', 'frequency']
-        for key in keys:
-            if key in dic:
-                data[key] = dic[key]
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels"
-        response = requests.post(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+        property_keys = {"name": dic["name"]}
+        if "data_type" in dic:
+            property_keys["data_type"] = dic["data_type"]
+        if "cardinality" in dic:
+            property_keys["cardinality"] = dic["cardinality"]
+        url = f"{self._host}/graphs/{self._graph_name}/schema/propertykeys"
+        response = self.__session.post(
+            url, data=json.dumps(property_keys), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if response.status_code == 201:
-            return 'create EdgeLabel success, Detail: "{}"'.format(str(response.content))
-        else:
-            raise CreateError('CreateError: "create EdgeLabel failed", Detail:  "{}"'
-                              .format(str(response.content)))
+        if check_if_success(
+            response,
+            CreateError(
+                f'CreateError: "create PropertyKey failed", Detail: {str(response.content)}'
+            ),
+        ):
+            return f"create PropertyKey success, Detail: {str(response.content)}"
+        return f"create PropertyKey failed, Detail: {str(response.content)}"
 
     @decorator_params
-    def remove(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels" + "/" + \
-              self._parameter_holder.get_value("name")
-        res = requests.delete(url, auth=self._auth, headers=self._headers)
+    def append(self):
+        property_name = self._parameter_holder.get_value("name")
+        user_data = self._parameter_holder.get_value("user_data")
+        if not user_data:
+            user_data = {}
+        data = {"name": property_name, "user_data": user_data}
+
+        url = (
+            f"{self._host}/graphs/{self._graph_name}/schema/propertykeys/"
+            f"{property_name}/?action=append"
+        )
+        response = self.__session.put(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if res.status_code == 202:
-            return 'remove EdgeLabel success, Detail: "{}"'.format(str(res.content))
-        else:
-            raise RemoveError('RemoveError: "remove EdgeLabel failed", Detail:  "{}"'
-                              .format(str(res.content)))
+        if check_if_success(
+            response,
+            UpdateError(
+                f'UpdateError: "append PropertyKey failed", Detail: {str(response.content)}'
+            ),
+        ):
+            return f"append PropertyKey success, Detail: {str(response.content)}"
+        return f"append PropertyKey failed, Detail: {str(response.content)}"
 
     @decorator_params
-    def append(self):
-        dic = self._parameter_holder.get_dic()
-        data = dict()
-        keys = ['name', 'nullable_keys', 'properties', 'user_data']
-        for key in keys:
-            if key in dic:
-                data[key] = dic[key]
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels" \
-              + "/" + data["name"] + "?action=append"
-        res = requests.put(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+    def eliminate(self):
+        property_name = self._parameter_holder.get_value("name")
+        user_data = self._parameter_holder.get_value("user_data")
+        if not user_data:
+            user_data = {}
+        data = {"name": property_name, "user_data": user_data}
+
+        url = (
+            f"{self._host}/graphs/{self._graph_name}/schema/propertykeys/"
+            f"{property_name}/?action=eliminate"
+        )
+        response = self.__session.put(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if res.status_code == 200:
-            return 'append EdgeLabel success, Detail: "{}"'.format(str(res.content))
-        else:
-            raise UpdateError('UpdateError: "append EdgeLabel failed", Detail: "{}"'.format(str(res.content)))
+        error = UpdateError(
+            f'UpdateError: "eliminate PropertyKey failed", Detail: {str(response.content)}'
+        )
+        if check_if_success(response, error):
+            return f"eliminate PropertyKey success, Detail: {str(response.content)}"
+        return f"eliminate PropertyKey failed, Detail: {str(response.content)}"
 
     @decorator_params
-    def eliminate(self):
-        name = self._parameter_holder.get_value("name")
-        user_data = self._parameter_holder.get_value("user_data") if \
-            self._parameter_holder.get_value("user_data") else {}
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels" \
-              + "/" + self._parameter_holder.get_value("name") + "?action=eliminate"
-        data = {
-            "name": name,
-            "user_data": user_data
-        }
-        res = requests.put(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+    def remove(self):
+        dic = self._parameter_holder.get_dic()
+        url = f'{self._host}/graphs/{self._graph_name}/schema/propertykeys/{dic["name"]}'
+        response = self.__session.delete(url)
         self.clean_parameter_holder()
-        if res.status_code == 200:
-            return 'eliminate EdgeLabel success, Detail: "{}"'.format(str(res.content))
-        else:
-            raise UpdateError('UpdateError: "eliminate EdgeLabel failed", Detail: "{}"'.format(str(res.content)))
+        if check_if_success(
+            response,
+            RemoveError(
+                f'RemoveError: "delete PropertyKey failed", Detail: {str(response.content)}'
+            ),
+        ):
+            return f'delete PropertyKey success, Detail: {dic["name"]}'
+        return f"delete PropertyKey failed, Detail: {str(response.content)}"
```

### Comparing `hugegraph-python-1.0.0.9/manager/schema/index_label.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/index_label.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import json
 
-import requests
 
-from manager.common import HugeGraphBase
-from utils.huge_decorator import decorator_params, decorator_create
-from utils.exceptions import CreateError, RemoveError
-from utils.util import authorized
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.utils.huge_decorator import decorator_params, decorator_create
+from pyhugegraph.utils.exceptions import CreateError, RemoveError
+from pyhugegraph.utils.util import check_if_authorized, check_if_success
 
 
-class IndexLabel(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
+class IndexLabel(HugeParamsBase):
+    def __init__(self, graph_instance, session):
+        super().__init__(graph_instance)
+        self.__session = session
 
     @decorator_params
     def onV(self, vertex_label):
         self._parameter_holder.set("base_value", vertex_label)
         self._parameter_holder.set("base_type", "VERTEX_LABEL")
         return self
 
@@ -63,43 +63,49 @@
     @decorator_params
     def Search(self):
         self._parameter_holder.set("index_type", "SEARCH")
         return self
 
     @decorator_params
     def ifNotExist(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/indexlabels" \
-              + "/" + self._parameter_holder.get_value("name")
-        response = requests.get(url)
-        if response.status_code == 200 and authorized(response):
+        url = (
+            f"{self._host}/graphs/{self._graph_name}/schema/indexlabels/"
+            f'{self._parameter_holder.get_value("name")}'
+        )
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        if response.status_code == 200 and check_if_authorized(response):
             self._parameter_holder.set("not_exist", False)
         return self
 
     @decorator_create
     def create(self):
         dic = self._parameter_holder.get_dic()
-        data = dict()
+        data = {}
         data["name"] = dic["name"]
         data["base_type"] = dic["base_type"]
         data["base_value"] = dic["base_value"]
         data["index_type"] = dic["index_type"]
         data["fields"] = list(dic["fields"])
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/indexlabels"
-        res = requests.post(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/indexlabels"
+        response = self.__session.post(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if res.status_code == 202:
-            return 'create IndexLabel success, Deatil: "{}"'.format(str(res.content))
-        else:
-            raise CreateError('CreateError: "create IndexLabel failed", '
-                              'Detail "{}"'.format(str(res.content)))
+        error = CreateError(
+            f'CreateError: "create IndexLabel failed", Detail "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'create IndexLabel success, Deatil: "{str(response.content)}"'
+        return None
 
     @decorator_params
     def remove(self):
         name = self._parameter_holder.get_value("name")
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/indexlabels" + "/" + name
-        res = requests.delete(url, auth=self._auth, headers=self._headers)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/indexlabels/{name}"
+        response = self.__session.delete(url, auth=self._auth, headers=self._headers)
         self.clean_parameter_holder()
-        if res.status_code == 202:
-            return 'remove IndexLabel success, Deatil: "{}"'.format(str(res.content))
-        else:
-            raise RemoveError('RemoveError: "remove IndexLabel failed", '
-                              'Detail "{}"'.format(str(res.content)))
+        error = RemoveError(
+            f'RemoveError: "remove IndexLabel failed", Detail "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'remove IndexLabel success, Deatil: "{str(response.content)}"'
+        return None
```

### Comparing `hugegraph-python-1.0.0.9/manager/schema/property_key.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/schema_manage/vertex_label.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,161 +13,170 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import json
 
-import requests
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.utils.exceptions import CreateError, UpdateError, RemoveError
+from pyhugegraph.utils.huge_decorator import decorator_params, decorator_create
+from pyhugegraph.utils.util import check_if_success, check_if_authorized
 
-from manager.common import HugeGraphBase
-from utils.huge_decorator import decorator_params, decorator_create
-from utils.exceptions import CreateError, UpdateError, RemoveError
-from utils.util import authorized
 
-
-class PropertyKey(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
-
-    @decorator_params
-    def asInt(self):
-        self._parameter_holder.set("data_type", "INT")
-        return self
-
-    @decorator_params
-    def asText(self):
-        self._parameter_holder.set("data_type", "TEXT")
-        return self
+class VertexLabel(HugeParamsBase):
+    def __init__(self, graph_instance, session):
+        super().__init__(graph_instance)
+        self.__session = session
 
     @decorator_params
-    def asDouble(self):
-        self._parameter_holder.set("data_type", "DOUBLE")
+    def useAutomaticId(self):
+        self._parameter_holder.set("id_strategy", "AUTOMATIC")
         return self
 
     @decorator_params
-    def asDate(self):
-        self._parameter_holder.set("data_type", "DATE")
+    def useCustomizeStringId(self):
+        self._parameter_holder.set("id_strategy", "CUSTOMIZE_STRING")
         return self
 
     @decorator_params
-    def valueSingle(self):
-        self._parameter_holder.set("cardinality", "SINGLE")
+    def useCustomizeNumberId(self):
+        self._parameter_holder.set("id_strategy", "CUSTOMIZE_NUMBER")
         return self
 
     @decorator_params
-    def valueList(self):
-        self._parameter_holder.set("cardinality", "LIST")
+    def usePrimaryKeyId(self):
+        self._parameter_holder.set("id_strategy", "PRIMARY_KEY")
         return self
 
     @decorator_params
-    def valueSet(self):
-        self._parameter_holder.set("cardinality", "SET")
+    def properties(self, *args):
+        self._parameter_holder.set("properties", list(args))
         return self
 
     @decorator_params
-    def calcMax(self):
-        self._parameter_holder.set("aggregate_type", "MAX")
+    def primaryKeys(self, *args):
+        self._parameter_holder.set("primary_keys", list(args))
         return self
 
     @decorator_params
-    def calcMin(self):
-        self._parameter_holder.set("aggregate_type", "MIN")
+    def nullableKeys(self, *args):
+        self._parameter_holder.set("nullable_keys", list(args))
         return self
 
     @decorator_params
-    def calcSum(self):
-        self._parameter_holder.set("aggregate_type", "SUM")
-        return self
-
-    @decorator_params
-    def calcOld(self):
-        self._parameter_holder.set("aggregate_type", "OLD")
+    def enableLabelIndex(self, flag):
+        self._parameter_holder.set("enable_label_index", flag)
         return self
 
     @decorator_params
     def userdata(self, *args):
+        if "user_data" not in self._parameter_holder.get_keys():
+            self._parameter_holder.set("user_data", {})
         user_data = self._parameter_holder.get_value("user_data")
-        if not user_data:
-            self._parameter_holder.set("user_data", dict())
-            user_data = self._parameter_holder.get_value("user_data")
         i = 0
         while i < len(args):
             user_data[args[i]] = args[i + 1]
             i += 2
         return self
 
     def ifNotExist(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys" \
-              + "/" + self._parameter_holder.get_value("name")
-        response = requests.get(url)
-        if response.status_code == 200 and authorized(response):
+        url = (
+            f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels/"
+            f'{self._parameter_holder.get_value("name")}'
+        )
+
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        if response.status_code == 200 and check_if_authorized(response):
             self._parameter_holder.set("not_exist", False)
         return self
 
     @decorator_create
     def create(self):
         dic = self._parameter_holder.get_dic()
-        propertykeys = {
-            "name": dic["name"]
-        }
-        if "data_type" in dic:
-            propertykeys["data_type"] = dic["data_type"]
-        if "cardinality" in dic:
-            propertykeys["cardinality"] = dic["cardinality"]
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys"
-        res = requests.post(url, data=json.dumps(propertykeys), auth=self._auth, headers=self._headers)
+        key_list = [
+            "name",
+            "id_strategy",
+            "primary_keys",
+            "nullable_keys",
+            "index_labels",
+            "properties",
+            "enable_label_index",
+            "user_data",
+        ]
+        data = {}
+        for key in key_list:
+            if key in dic:
+                data[key] = dic[key]
+        url = f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels"
+        response = self.__session.post(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if res.status_code == 201:
-            return 'create PropertyKey success, Detail: {}'.format(res.content)
-        else:
-            raise CreateError('CreateError: "create PropertyKey failed", Detail: {}'.format(res.content))
+        error = CreateError(
+            f'CreateError: "create VertexLabel failed", Detail: "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'create VertexLabel success, Detail: "{str(response.content)}"'
+        return f'create VertexLabel failed, Detail: "{str(response.content)}"'
 
     @decorator_params
     def append(self):
-        property_name = self._parameter_holder.get_value("name")
-        user_data = self._parameter_holder.get_value("user_data")
-        if not user_data:
-            user_data = dict()
+        dic = self._parameter_holder.get_dic()
+        properties = dic["properties"] if "properties" in dic else []
+        nullable_keys = dic["nullable_keys"] if "nullable_keys" in dic else []
+        user_data = dic["user_data"] if "user_data" in dic else {}
+        url = (
+            f"{self._host}/graphs/{self._graph_name}"
+            f'/schema/vertexlabels/{dic["name"]}?action=append'
+        )
+
         data = {
-            "name": property_name,
-            "user_data": user_data
+            "name": dic["name"],
+            "properties": properties,
+            "nullable_keys": nullable_keys,
+            "user_data": user_data,
         }
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys" \
-              + "/" + property_name + "?action=append"
-        res = requests.put(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+        response = self.__session.put(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
         self.clean_parameter_holder()
-        if res.status_code == 200:
-            return 'append PropertyKey success, Detail: {}'.format(res.content)
-        else:
-            raise UpdateError('UpdateError: "append PropertyKey failed", Detail: {}'.format(res.content))
+        error = UpdateError(
+            f'UpdateError: "append VertexLabel failed", Detail: "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'append VertexLabel success, Detail: "{str(response.content)}"'
+        return f'append VertexLabel failed, Detail: "{str(response.content)}"'
 
     @decorator_params
-    def eliminate(self):
-        property_name = self._parameter_holder.get_value("name")
-        user_data = self._parameter_holder.get_value("user_data")
-        if not user_data:
-            user_data = dict()
-        data = {
-            "name": property_name,
-            "user_data": user_data
-        }
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys" \
-              + "/" + property_name + "?action=eliminate"
-        res = requests.put(url, data=json.dumps(data), auth=self._auth, headers=self._headers)
+    def remove(self):
+        name = self._parameter_holder.get_value("name")
+        url = f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels/{name}"
+        response = self.__session.delete(url, auth=self._auth, headers=self._headers)
         self.clean_parameter_holder()
-        if res.status_code == 200:
-            return 'eliminate PropertyKey success, Detail: {}'.format(str(res.content))
-        else:
-            raise UpdateError('UpdateError: "eliminate PropertyKey failed", Detail: {}'.format(str(res.content)))
+        error = RemoveError(
+            f'RemoveError: "remove VertexLabel failed", Detail: "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'remove VertexLabel success, Detail: "{str(response.content)}"'
+        return f'remove VertexLabel failed, Detail: "{str(response.content)}"'
 
     @decorator_params
-    def remove(self):
+    def eliminate(self):
+        name = self._parameter_holder.get_value("name")
+        url = f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels/{name}/?action=eliminate"
+
         dic = self._parameter_holder.get_dic()
-        url = self._host + "/graphs" + "/" + self._graph_name + \
-              "/schema/propertykeys" + "/" + dic["name"]
-        res = requests.delete(url)
-        self.clean_parameter_holder()
-        if res.status_code == 204:
-            return 'delete PropertyKey success, Detail: {}'.format(dic["name"])
-        else:
-            raise RemoveError('RemoveError: "delete PropertyKey failed", Detail: {}'.format(str(res.content)))
+        user_data = dic["user_data"] if "user_data" in dic else {}
+        data = {
+            "name": self._parameter_holder.get_value("name"),
+            "user_data": user_data,
+        }
+        response = self.__session.put(
+            url, data=json.dumps(data), auth=self._auth, headers=self._headers
+        )
+        error = UpdateError(
+            f'UpdateError: "eliminate VertexLabel failed", Detail: "{str(response.content)}"'
+        )
+        if check_if_success(response, error):
+            return f'eliminate VertexLabel success, Detail: "{str(response.content)}"'
+        return f'eliminate VertexLabel failed, Detail: "{str(response.content)}"'
```

### Comparing `hugegraph-python-1.0.0.9/manager/schema_manager.py` & `hugegraph-python-1.3.0/src/pyhugegraph/api/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,127 +14,152 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 import json
 
-import requests
-
-from models.property_key_data import PropertyKeyData
-from models.edge_label_data import EdgeLabelData
-from models.index_label_data import IndexLabelData
-from models.vertex_label_data import VertexLabelData
-
-from manager.common import HugeGraphBase
-from manager.schema.property_key import PropertyKey
-from manager.schema.edge_label import EdgeLabel
-from manager.schema.vertex_label import VertexLabel
-from manager.schema.index_label import IndexLabel
-from utils.exceptions import NotFoundError
-from utils.util import authorized
-
-
-class SchemaManager(HugeGraphBase):
-    def __init__(self, ip, port, graph_name, user, pwd, timeout):
-        super().__init__(ip, port, graph_name, user, pwd, timeout)
+from pyhugegraph.api.common import HugeParamsBase
+from pyhugegraph.api.schema_manage.edge_label import EdgeLabel
+from pyhugegraph.api.schema_manage.index_label import IndexLabel
+from pyhugegraph.api.schema_manage.property_key import PropertyKey
+from pyhugegraph.api.schema_manage.vertex_label import VertexLabel
+from pyhugegraph.structure.edge_label_data import EdgeLabelData
+from pyhugegraph.structure.index_label_data import IndexLabelData
+from pyhugegraph.structure.property_key_data import PropertyKeyData
+from pyhugegraph.structure.vertex_label_data import VertexLabelData
+from pyhugegraph.utils.exceptions import NotFoundError
+from pyhugegraph.utils.huge_requests import HugeSession
+from pyhugegraph.utils.util import check_if_success
+
+
+class SchemaManager(HugeParamsBase):
+    def __init__(self, graph_instance):
+        super().__init__(graph_instance)
+        self.__session = HugeSession.new_session()
+
+    def close(self):
+        if self.__session:
+            self.__session.close()
+
+    """
+    create schemas, including propertyKey/vertexLabel/edgeLabel/indexLabel
+    """
 
     def propertyKey(self, property_name):
-        property_key = PropertyKey(self._ip, self._port, self._graph_name, self._user, self._pwd, self._timeout)
+        property_key = PropertyKey(self._graph_instance, self.__session)
         property_key.create_parameter_holder()
         property_key.add_parameter("name", property_name)
         property_key.add_parameter("not_exist", True)
         return property_key
 
+    def vertexLabel(self, vertex_name):
+        vertex_label = VertexLabel(self._graph_instance, self.__session)
+        vertex_label.create_parameter_holder()
+        vertex_label.add_parameter("name", vertex_name)
+        # vertex_label.add_parameter("id_strategy", "AUTOMATIC")
+        vertex_label.add_parameter("not_exist", True)
+        return vertex_label
+
+    def edgeLabel(self, name):
+        edge_label = EdgeLabel(self._graph_instance, self.__session)
+        edge_label.create_parameter_holder()
+        edge_label.add_parameter("name", name)
+        edge_label.add_parameter("not_exist", True)
+        return edge_label
+
+    def indexLabel(self, name):
+        index_label = IndexLabel(self._graph_instance, self.__session)
+        index_label.create_parameter_holder()
+        index_label.add_parameter("name", name)
+        return index_label
+
+    def getSchema(self):
+        url = f"{self._host}/graphs/{self._graph_name}/schema"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        error = NotFoundError(f"schema not found: {str(response.content)}")
+        if check_if_success(response, error):
+            schema = json.loads(response.content)
+            return schema
+        return None
+
     def getPropertyKey(self, property_name):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys" \
-              + "/" + property_name
-        response = requests.get(url)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/schema/propertykeys/{property_name}"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        error = NotFoundError(f"PropertyKey not found: {str(response.content)}")
+        if check_if_success(response, error):
             property_keys_data = PropertyKeyData(json.loads(response.content))
             return property_keys_data
-        else:
-            raise NotFoundError("PorpertyKey not found: {}".format(response.content))
+        return None
 
     def getPropertyKeys(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/propertykeys"
-        response = requests.get(url)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/propertykeys"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
         res = []
-        if authorized(response):
+        if check_if_success(response):
             for item in json.loads(response.content)["propertykeys"]:
                 res.append(PropertyKeyData(item))
             return res
-
-    def vertexLabel(self, vertex_name):
-        vertex_label = VertexLabel(self._ip, self._port, self._graph_name, self._user, self._pwd, self._timeout)
-        vertex_label.create_parameter_holder()
-        vertex_label.add_parameter("name", vertex_name)
-        # vertex_label.add_parameter("id_strategy", "AUTOMATIC")
-        vertex_label.add_parameter("not_exist", True)
-        return vertex_label
+        return None
 
     def getVertexLabel(self, name):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/vertexlabels/" + name
-        response = requests.get(url, auth=self._auth, headers=self._headers)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels/{name}"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        error = NotFoundError(f"VertexLabel not found: {str(response.content)}")
+        if check_if_success(response, error):
             res = VertexLabelData(json.loads(response.content))
             return res
-        else:
-            raise NotFoundError("VertexLabel not found: {}".format(response.content))
+        return None
 
     def getVertexLabels(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/vertexlabels/"
-        response = requests.get(url, auth=self._auth, headers=self._headers)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/vertexlabels"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
         res = []
-        if authorized(response):
+        if check_if_success(response):
             for item in json.loads(response.content)["vertexlabels"]:
                 res.append(VertexLabelData(item))
-            return res
-
-    def edgeLabel(self, name):
-        edge_label = EdgeLabel(self._ip, self._port, self._graph_name, self._user, self._pwd, self._timeout)
-        edge_label.create_parameter_holder()
-        edge_label.add_parameter("name", name)
-        edge_label.add_parameter("not_exist", True)
-        return edge_label
+        return res
 
     def getEdgeLabel(self, label_name):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels" + "/" + label_name
-        response = requests.get(url, auth=self._auth, headers=self._headers)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/schema/edgelabels/{label_name}"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        error = NotFoundError(f"EdgeLabel not found: {str(response.content)}")
+        if check_if_success(response, error):
             res = EdgeLabelData(json.loads(response.content))
             return res
-        else:
-            raise NotFoundError("EdgeLabel not found: {}".format(response.content))
+        return None
 
     def getEdgeLabels(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/edgelabels"
-        response = requests.get(url, auth=self._auth, headers=self._headers)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/edgelabels"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
         res = []
-        if authorized(response):
+        if check_if_success(response):
             for item in json.loads(response.content)["edgelabels"]:
                 res.append(EdgeLabelData(item))
-            return res
+        return res
 
-    def indexLabel(self, name):
-        index_label = IndexLabel(self._ip, self._port, self._graph_name, self._user, self._pwd, self._timeout)
-        index_label.create_parameter_holder()
-        index_label.add_parameter("name", name)
-        return index_label
+    def getRelations(self):
+        url = f"{self._host}/graphs/{self._graph_name}/schema/edgelabels"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        res = []
+        if check_if_success(response):
+            for item in json.loads(response.content)["edgelabels"]:
+                res.append(EdgeLabelData(item).relations())
+        return res
 
     def getIndexLabel(self, name):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/indexlabels" + "/" + name
-        response = requests.get(url, auth=self._auth, headers=self._headers)
-        if response.status_code == 200 and authorized(response):
+        url = f"{self._host}/graphs/{self._graph_name}/schema/indexlabels/{name}"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
+        error = NotFoundError(f"EdgeLabel not found: {str(response.content)}")
+        if check_if_success(response, error):
             res = IndexLabelData(json.loads(response.content))
             return res
-        else:
-            raise NotFoundError("IndexLabel not found: {}".format(response.content))
+        return None
 
     def getIndexLabels(self):
-        url = self._host + "/graphs" + "/" + self._graph_name + "/schema/indexlabels"
-        response = requests.get(url, auth=self._auth, headers=self._headers)
+        url = f"{self._host}/graphs/{self._graph_name}/schema/indexlabels"
+        response = self.__session.get(url, auth=self._auth, headers=self._headers)
         res = []
-        if authorized(response):
-            for item in json.loads(response.content)['indexlabels']:
+        if check_if_success(response):
+            for item in json.loads(response.content)["indexlabels"]:
                 res.append(IndexLabelData(item))
-            return res
+        return res
```

### Comparing `hugegraph-python-1.0.0.9/models/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/example/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/models/edge_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/edge_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,9 @@
         return self.__inVLabel
 
     @property
     def properties(self):
         return self.__properties
 
     def __repr__(self):
-        res = "{}--{}-->{}".format(self.__outV, self.__label, self.__inV)
+        res = f"{self.__outV}--{self.__label}-->{self.__inV}"
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/edge_label_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/edge_label_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,11 +62,22 @@
     def nullableKeys(self):
         return self.__nullable_keys
 
     @property
     def userdata(self):
         return self.__user_data
 
+    def relations(self):
+        res = f"{self.__source_label}--{self.__name}-->{self.__target_label}"
+        return res
+
+    @property
+    def indexLabels(self):
+        return self.__index_labels
+
+    @property
+    def enableLabelIndex(self):
+        return self.__enable_label_index
+
     def __repr__(self):
-        res = "{}--{}-->{}".format(
-            self.__source_label, self.__name, self.__target_label)
+        res = f"name: {self.__name}, properties: {self.__properties}"
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/index_label_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/index_label_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,11 +46,12 @@
         return self.__fields
 
     @property
     def indexType(self):
         return self.__index_type
 
     def __repr__(self):
-        res = "index_name: {}, base_value: {}, base_type: {}, fields: [], index_type: {}"\
-            .format(self.__name, self.__base_value, self.__base_type, self.__fields,
-                    self.__index_type)
+        res = (
+            f"index_name: {self.__name}, base_value: {self.__base_value}, base_type:"
+            f" {self.__base_type}, fields: {self.__fields}, index_type: {self.__index_type}"
+        )
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/property_key_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/property_key_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         return self.__data_type
 
     @property
     def userdata(self):
         return self.__user_data
 
     def __repr__(self):
-        res = "name: {}, cardinality: {}, data_type: {}".format(
-            self.__name, self.__cardinality, self.__data_type
+        res = (
+            f"name: {self.__name}, cardinality: {self.__cardinality}, data_type: {self.__data_type}"
         )
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/respon_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/response_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         return self.__status
 
     @property
     def result(self):
         return self.__result
 
     def __repr__(self):
-        res = "id: {}, status: {}, result: {}".format(self.__id, self.__status, self.__result)
+        res = f"id: {self.__id}, status: {self.__status}, result: {self.__result}"
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/vertex_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/vertex_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         return self.__type
 
     @property
     def properties(self):
         return self.__properties
 
     def __repr__(self):
-        res = "id: {}, label: {}, type: {}".format(self.__id, self.__label, self.__type)
+        res = f"id: {self.__id}, label: {self.__label}, type: {self.__type}"
         return res
```

### Comparing `hugegraph-python-1.0.0.9/models/vertex_label_data.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/vertex_label_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,11 +52,21 @@
     def nullableKeys(self):
         return self.__nullable_keys
 
     @property
     def userdata(self):
         return self.__user_data
 
+    @property
+    def indexLabels(self):
+        return self.__index_labels
+
+    @property
+    def enableLabelIndex(self):
+        return self.__enable_label_index
+
     def __repr__(self):
-        res = "name: {}, primary_keys: {}, properties: {}".format(
-            self.__name, self.__primary_keys, self.__properties)
+        res = (
+            f"name: {self.__name}, primary_keys: {self.__primary_keys}, "
+            f"properties: {self.__properties}"
+        )
         return res
```

### Comparing `hugegraph-python-1.0.0.9/test/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/utils/__init__.py` & `hugegraph-python-1.3.0/src/pyhugegraph/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.9/utils/exceptions.py` & `hugegraph-python-1.3.0/src/pyhugegraph/utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,49 +14,51 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 class NotAuthorizedError(Exception):
     """
-        Not Authorized
+    Not Authorized
     """
 
+
 class InvalidParameter(Exception):
     """
-        Parameter setting error
+    Parameter setting error
     """
 
+
 class NotFoundError(Exception):
     """
-        no content found
+    no content found
     """
 
 
 class CreateError(Exception):
     """
-        Failed to create vertex or edge
+    Failed to create vertex or edge
     """
 
 
 class RemoveError(Exception):
     """
-        Failed to delete vertex or edge
+    Failed to delete vertex or edge
     """
 
 
 class UpdateError(Exception):
     """
-        Failed to modify node
+    Failed to modify node
     """
 
 
 class DataFormatError(Exception):
     """
-        Input data format error
+    Input data format error
     """
 
 
 class ServiceUnavailableException(Exception):
     """
-        The server is too busy to be available
+    The server is too busy to be available
     """
```

### Comparing `hugegraph-python-1.0.0.9/utils/huge_requests.py` & `hugegraph-python-1.3.0/src/pyhugegraph/utils/huge_requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 from urllib3.util.retry import Retry
 
 
 class HugeSession:
     @staticmethod
     def new_session():
         session = requests.Session()
-        retry = Retry(connect=3, backoff_factor=0.5)
+        retry = Retry(connect=5, backoff_factor=1)
         adapter = HTTPAdapter(max_retries=retry)
-        session.mount('http://', adapter)
-        session.mount('https://', adapter)
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+        session.keep_alive = False
         return session
```

### Comparing `hugegraph-python-1.0.0.9/utils/util.py` & `hugegraph-python-1.3.0/src/pyhugegraph/utils/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,23 +13,38 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import json
 
-from utils.exceptions import ServiceUnavailableException, NotAuthorizedError
+from pyhugegraph.utils.exceptions import (
+    ServiceUnavailableException,
+    NotAuthorizedError,
+    NotFoundError,
+)
 
 
-def create_exception(reponse_content):
-    data = json.loads(reponse_content)
+def create_exception(response_content):
+    data = json.loads(response_content)
     if "ServiceUnavailableException" in data["exception"]:
-        raise ServiceUnavailableException('ServiceUnavailableException, "message": "{}", "cause": "{}"'.
-                                           format(data["message"], data["cause"]))
-    else:
-        raise Exception(reponse_content)
+        raise ServiceUnavailableException(
+            f'ServiceUnavailableException, "message": "{data["message"]}",'
+            f' "cause": "{data["cause"]}"'
+        )
+    raise Exception(response_content)
 
 
-def authorized(response):
+def check_if_authorized(response):
     if response.status_code == 401:
-        raise NotAuthorizedError("Please check your username and password. {}".format(response.content))
+        raise NotAuthorizedError(
+            f"Please check your username and password. {str(response.content)}"
+        )
+    return True
+
+
+def check_if_success(response, error=None):
+    if (not str(response.status_code).startswith("20")) and check_if_authorized(response):
+        if error is None:
+            error = NotFoundError(response.content)
+        raise error
     return True
```

