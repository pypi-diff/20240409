# Comparing `tmp/aio_code_editor-0.6.3.tar.gz` & `tmp/aio_code_editor-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_code_editor-0.6.3.tar", max compression
+gzip compressed data, was "aio_code_editor-0.7.0.tar", max compression
```

## Comparing `aio_code_editor-0.6.3.tar` & `aio_code_editor-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-03-24 06:07:03.870674 aio_code_editor-0.6.3/aio_code_editor/__init__.py
--rw-r--r--   0        0        0      578 2024-03-30 10:01:05.175490 aio_code_editor-0.6.3/aio_code_editor/app.py
--rw-r--r--   0        0        0     2294 2024-03-31 03:54:20.345213 aio_code_editor-0.6.3/aio_code_editor/css.py
--rw-r--r--   0        0        0   117981 2024-03-22 01:42:07.806699 aio_code_editor-0.6.3/aio_code_editor/shark.png
--rw-r--r--   0        0        0     4376 2024-03-31 07:13:00.372803 aio_code_editor-0.6.3/aio_code_editor/ui.py
--rw-r--r--   0        0        0      505 2024-03-30 09:56:18.757803 aio_code_editor-0.6.3/aio_code_editor/until.py
--rw-r--r--   0        0        0      379 2024-03-31 07:13:21.797596 aio_code_editor-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      621 2024-03-24 15:07:16.978760 aio_code_editor-0.6.3/README.md
--rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 aio_code_editor-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-24 06:07:03.870674 aio_code_editor-0.7.0/aio_code_editor/__init__.py
+-rw-r--r--   0        0        0      578 2024-03-30 10:01:05.175490 aio_code_editor-0.7.0/aio_code_editor/app.py
+-rw-r--r--   0        0        0     2294 2024-03-31 03:54:20.345213 aio_code_editor-0.7.0/aio_code_editor/css.py
+-rw-r--r--   0        0        0   117981 2024-03-22 01:42:07.806699 aio_code_editor-0.7.0/aio_code_editor/shark.png
+-rw-r--r--   0        0        0     5442 2024-04-09 07:30:57.063612 aio_code_editor-0.7.0/aio_code_editor/ui.py
+-rw-r--r--   0        0        0      505 2024-03-30 09:56:18.757803 aio_code_editor-0.7.0/aio_code_editor/until.py
+-rw-r--r--   0        0        0      379 2024-04-09 07:36:42.005059 aio_code_editor-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      621 2024-03-24 15:07:16.978760 aio_code_editor-0.7.0/README.md
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 aio_code_editor-0.7.0/PKG-INFO
```

### Comparing `aio_code_editor-0.6.3/aio_code_editor/app.py` & `aio_code_editor-0.7.0/aio_code_editor/app.py`

 * *Files identical despite different names*

### Comparing `aio_code_editor-0.6.3/aio_code_editor/css.py` & `aio_code_editor-0.7.0/aio_code_editor/css.py`

 * *Files identical despite different names*

### Comparing `aio_code_editor-0.6.3/aio_code_editor/shark.png` & `aio_code_editor-0.7.0/aio_code_editor/shark.png`

 * *Files identical despite different names*

### Comparing `aio_code_editor-0.6.3/aio_code_editor/ui.py` & `aio_code_editor-0.7.0/aio_code_editor/ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import streamlit as st
 from code_editor import code_editor
 from aio_code_editor.css import info_bar_input, info_bar_output, output_btns, input_btns
 import subprocess
 from aio_code_editor.until import check_code, write_code
 import os
-import random
+import sys
+import importlib
 
 environ = os.environ.copy()
 environ['PYTHONIOENCODING'] = 'utf-8'
 
 def side_bar():
     with st.sidebar:
         st.markdown("## :heartbeat: :heartbeat: Hướng dẫn  :heartbeat: :heartbeat:")
@@ -34,30 +35,49 @@
         st.image("https://ia800202.us.archive.org/30/items/shark_202403/shark.png", width=150)
 
 def codes_box(sample_code, min_raw=5, max_raw=20):
     response_dict = code_editor(sample_code, buttons=input_btns, height=[min_raw, max_raw], info= info_bar_input)
     codes = response_dict["text"]
     # get lines number of sample_code
     line_nums = len(sample_code.split('\n'))    
-    type = response_dict["type"]
-    return codes, type, response_dict, line_nums
+    res_type = response_dict["type"]
+    return codes, res_type, response_dict, line_nums
 
 def output_box(response_dict, results, min_raw=5, max_raw=20, err=0):
     num_rows = response_dict['cursor']['row']
     if num_rows<min_raw:
         code_editor(results, buttons=output_btns, height= [min_raw, min_raw], info=info_bar_output)
     elif num_rows>=max_raw:
         code_editor(results, buttons=output_btns, height= [max_raw, max_raw] , info=info_bar_output)
              
     elif num_rows>=min_raw and num_rows<=max_raw:
         code_editor(results, buttons=output_btns, height= [int(num_rows)+1-err, max_raw], info=info_bar_output)
-    
-def run_code(file_name, codes, type, response_dict, download=False):
+
+def run_plot(file_name, codes, res_type, download=False):
+    if check_code(codes):     
+        if res_type == "submit":
+            # Lưu mã vào file Python
+            write_code(codes, file_name)
+            # Hiển thị button đownload file
+            if download:
+                st.download_button(
+                    label="Save file",
+                    data=open(file_name, 'rb').read(),
+                    file_name= file_name,
+                    mime="text/plain")
+            # Thực thi file Python và lấy đầu ra và lỗi (nếu có)
+            module_name  = file_name.split(".")[0]
+            if module_name in sys.modules:
+                importlib.reload(sys.modules[module_name])
+            else:
+                importlib.import_module(module_name)
+                
+def run_code(file_name, codes, res_type, response_dict, download=False):
     if check_code(codes):     
-        if type == "submit":
+        if res_type == "submit":
             # Lưu mã vào file Python
             write_code(codes, file_name)
             # Hiển thị button đownload file
             if download:
                 st.download_button(
                     label="Save file",
                     data=open(file_name, 'rb').read(),
@@ -73,22 +93,25 @@
             elif result.stdout == "":
                 output_box(response_dict, result.stderr, err=1)
             else:
                 output_box(response_dict, f"{result.stdout}\n{result.stderr}", err=1)
     else:
         st.error("Mã của bạn có thể nguy hiểm, vui lòng kiểm tra lại!")
 
-def code_io(sample=''' ''', l=1, r=1, min_raw=5, max_raw=20, download=False, key=None ):
+def code_io(sample=''' ''', l=1, r=1, min_raw=5, max_raw=20, download=False, key=None, type_out="python" ):
     col1, col2 = st.columns([l, r])
     with col1:
-        codes, type, response_dict, line_nums = codes_box(sample, min_raw, max_raw)
+        codes, res_type, response_dict, line_nums = codes_box(sample, min_raw, max_raw)
 
     with col2:
-        if type=="":
+        if res_type=="":
             if line_nums<min_raw:
                 line_nums = min_raw
             elif line_nums>=max_raw:
                 line_nums = max_raw
             code_editor("", buttons=output_btns, height= [line_nums, max_raw] , info=info_bar_output, key=key)
 
         else:
-            run_code(file_name="st-test.py", codes=codes, type=type, response_dict=response_dict, download=download)
+            if type_out=="python":
+                run_code(file_name="st-test.py", codes=codes, res_type=res_type, response_dict=response_dict, download=download)
+            elif type_out=="plot":
+                run_plot(file_name="st-test.py", codes=codes, res_type=res_type, download=download)
```

### Comparing `aio_code_editor-0.6.3/README.md` & `aio_code_editor-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aio_code_editor-0.6.3/PKG-INFO` & `aio_code_editor-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-code-editor
-Version: 0.6.3
+Version: 0.7.0
 Summary: 
 Author: NguyenDinhTiem
 Author-email: nguyendinhtiem1999@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

