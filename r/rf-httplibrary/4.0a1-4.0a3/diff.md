# Comparing `tmp/rf_httplibrary-4.0a1-py3-none-any.whl.zip` & `tmp/rf_httplibrary-4.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15105 bytes, number of entries: 8
--rw-rw-r--  2.0 unx    50459 b- defN 22-Sep-01 13:58 HttpLibrary/HttpLibrary.py
--rw-rw-r--  2.0 unx     1077 b- defN 22-Jun-02 08:45 HttpLibrary/__init__.py
--rw-rw-r--  2.0 unx     1124 b- defN 22-Sep-01 13:58 HttpLibrary/version.py
--rw-rw-r--  2.0 unx     1072 b- defN 22-Sep-01 14:08 rf_httplibrary-4.0a1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3262 b- defN 22-Sep-01 14:08 rf_httplibrary-4.0a1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-01 14:08 rf_httplibrary-4.0a1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 22-Sep-01 14:08 rf_httplibrary-4.0a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      664 b- defN 22-Sep-01 14:08 rf_httplibrary-4.0a1.dist-info/RECORD
-8 files, 57762 bytes uncompressed, 13945 bytes compressed:  75.9%
+Zip file size: 15181 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx    50459 b- defN 24-Apr-09 14:00 HttpLibrary/HttpLibrary.py
+-rw-rw-r--  2.0 unx     1077 b- defN 24-Apr-09 13:35 HttpLibrary/__init__.py
+-rw-rw-r--  2.0 unx     1124 b- defN 24-Apr-09 14:17 HttpLibrary/version.py
+-rw-rw-r--  2.0 unx     1072 b- defN 24-Apr-09 14:17 rf_httplibrary-4.0a3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3454 b- defN 24-Apr-09 14:17 rf_httplibrary-4.0a3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 14:17 rf_httplibrary-4.0a3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-09 14:17 rf_httplibrary-4.0a3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      664 b- defN 24-Apr-09 14:17 rf_httplibrary-4.0a3.dist-info/RECORD
+8 files, 57954 bytes uncompressed, 14021 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: HttpLibrary/__init__.py
 Comment: 
 
 Filename: HttpLibrary/version.py
 Comment: 
 
-Filename: rf_httplibrary-4.0a1.dist-info/LICENSE
+Filename: rf_httplibrary-4.0a3.dist-info/LICENSE
 Comment: 
 
-Filename: rf_httplibrary-4.0a1.dist-info/METADATA
+Filename: rf_httplibrary-4.0a3.dist-info/METADATA
 Comment: 
 
-Filename: rf_httplibrary-4.0a1.dist-info/WHEEL
+Filename: rf_httplibrary-4.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: rf_httplibrary-4.0a1.dist-info/top_level.txt
+Filename: rf_httplibrary-4.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: rf_httplibrary-4.0a1.dist-info/RECORD
+Filename: rf_httplibrary-4.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HttpLibrary/version.py

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = '4.0a1'
+VERSION = '4.0a3'
```

## Comparing `rf_httplibrary-4.0a1.dist-info/LICENSE` & `rf_httplibrary-4.0a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rf_httplibrary-4.0a1.dist-info/METADATA` & `rf_httplibrary-4.0a3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: rf-httplibrary
-Version: 4.0a1
+Version: 4.0a3
 Summary: HTTP Request Test Library.
 Home-page: https://github.com/MainSystemDev/rf-httplibrary
 Author: Shiela Buitizon
 Author-email: shiela.buitizon@mnltechnology.com
 License: license
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: jsonpath-rw-ext (>=0.1.9)
 Requires-Dist: jsonpath-rw (==1.4.0)
 Requires-Dist: jsonschema (==3.2.0)
-Requires-Dist: requests-toolbelt (==0.9.1)
-Requires-Dist: requests (==2.22.0)
+Requires-Dist: requests
+Requires-Dist: requests-toolbelt
 Requires-Dist: robotframework (>=5.0.1)
-Requires-Dist: urllib3 (>=1.25.11)
 
 HttpLibrary
 ================
 
 
 
 Authors:
@@ -87,23 +87,36 @@
     Close Http Session    
 ```
 
 ### Keyword Documentation  
 View the latest keyword [documentation here](https://mainsystemdev.github.io/rf-httplibrary/) for more information about this library.
 
 
+### Install dependecy in local virtual environment
+
+```bash
+pip install .
+```
 ### Generating Local Documentation
 
 To Generate the keyword Documentation, simply run:
 ```bash
 python -m robot.libdoc HttpLibrary docs/index.html
 ```
 Where: docs.html is the output file.
 Note that the library must first be installed before generating a documentation.
 
+
 ### Execute Unit Test
 
-```    
-    python -m unittest
-    python setup.py test
+```bash
+python -m unittest
+python setup.py test
+```
+
+### Install requirements-dev.txt in shell runner
+This is for running pep8 style guide for python
+
+```bash
+sudo -H pip install -r requirements-dev.txt
 ```
```

## Comparing `rf_httplibrary-4.0a1.dist-info/RECORD` & `rf_httplibrary-4.0a3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 HttpLibrary/HttpLibrary.py,sha256=TL3Wm7XRpDnTLrB8_SKGRbT9fQTOg-R84aDroMuOkWc,50459
 HttpLibrary/__init__.py,sha256=XWototkrxGhGcnAkpzobIs4SIlBzbRvnGLvP47bLCm0,1077
-HttpLibrary/version.py,sha256=O9qU_id2oVk-9bA-j5mWKpy33ap73vchgxmaBQXvDe8,1124
-rf_httplibrary-4.0a1.dist-info/LICENSE,sha256=5DYCqfSuUFS8QMpjCHmvR28PfLroTxJb7qcHitp_0Wk,1072
-rf_httplibrary-4.0a1.dist-info/METADATA,sha256=SBgdo7N2dsO7AyNNlMjZLES4jfhvGfRKrmR_gSHxaH4,3262
-rf_httplibrary-4.0a1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-rf_httplibrary-4.0a1.dist-info/top_level.txt,sha256=xoWbmapj3adFgmFoMQ4PpdBdzJwlbl7OYf1DDpu13Gk,12
-rf_httplibrary-4.0a1.dist-info/RECORD,,
+HttpLibrary/version.py,sha256=iIWVKsPFUag5AZVmhzAP6SoUPNCwjh-QGGQDSk3xWCA,1124
+rf_httplibrary-4.0a3.dist-info/LICENSE,sha256=5DYCqfSuUFS8QMpjCHmvR28PfLroTxJb7qcHitp_0Wk,1072
+rf_httplibrary-4.0a3.dist-info/METADATA,sha256=vYmvi2YqkYoGHjmrfCDocXXzfYzl97mDbdMXfdv6puU,3454
+rf_httplibrary-4.0a3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rf_httplibrary-4.0a3.dist-info/top_level.txt,sha256=xoWbmapj3adFgmFoMQ4PpdBdzJwlbl7OYf1DDpu13Gk,12
+rf_httplibrary-4.0a3.dist-info/RECORD,,
```

