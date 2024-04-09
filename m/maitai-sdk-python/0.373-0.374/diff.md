# Comparing `tmp/maitai_sdk_python-0.373.tar.gz` & `tmp/maitai_sdk_python-0.374.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai_sdk_python-0.373.tar", last modified: Sat Mar 30 19:36:22 2024, max compression
+gzip compressed data, was "maitai_sdk_python-0.374.tar", last modified: Tue Apr  9 05:16:09 2024, max compression
```

## Comparing `maitai_sdk_python-0.373.tar` & `maitai_sdk_python-0.374.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 19:36:22.031530 maitai_sdk_python-0.373/
--rw-rw-rw-   0        0        0      356 2024-03-30 19:36:22.030530 maitai_sdk_python-0.373/PKG-INFO
--rw-rw-rw-   0        0        0     5177 2024-03-30 19:34:09.000000 maitai_sdk_python-0.373/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 19:36:22.004430 maitai_sdk_python-0.373/maitai/
--rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai_sdk_python-0.373/maitai/__init__.py
--rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai_sdk_python-0.373/maitai/_config.py
--rw-rw-rw-   0        0        0      563 2024-03-30 17:50:15.000000 maitai_sdk_python-0.373/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     7050 2024-03-30 19:35:04.000000 maitai_sdk_python-0.373/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai_sdk_python-0.373/maitai/_loadable.py
--rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai_sdk_python-0.373/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-03-30 19:36:22.029168 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      356 2024-03-30 19:36:21.000000 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-03-30 19:36:21.000000 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 19:36:21.000000 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-30 19:36:21.000000 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 19:36:21.000000 maitai_sdk_python-0.373/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 19:36:22.032530 maitai_sdk_python-0.373/setup.cfg
--rw-rw-rw-   0        0        0      554 2024-03-30 19:35:14.000000 maitai_sdk_python-0.373/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.439869 maitai_sdk_python-0.374/
+-rw-rw-rw-   0        0        0      356 2024-04-09 05:16:09.438869 maitai_sdk_python-0.374/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai_sdk_python-0.374/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.411136 maitai_sdk_python-0.374/maitai/
+-rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai_sdk_python-0.374/maitai/__init__.py
+-rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai_sdk_python-0.374/maitai/_config.py
+-rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai_sdk_python-0.374/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0     7111 2024-04-09 05:13:46.000000 maitai_sdk_python-0.374/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai_sdk_python-0.374/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai_sdk_python-0.374/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.436869 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      356 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-09 05:16:09.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:16:09.440505 maitai_sdk_python-0.374/setup.cfg
+-rw-rw-rw-   0        0        0      554 2024-04-09 05:14:38.000000 maitai_sdk_python-0.374/setup.py
```

### Comparing `maitai_sdk_python-0.373/README.md` & `maitai_sdk_python-0.374/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Welcome to the MaiTai Python SDK guide. This document will help you get started with integrating the MaiTai SDK into your application for evaluating AI outputs. Follow the steps below to install, configure, and use the SDK effectively.
 
 ## Installation
 
 To install the MaiTai SDK, run the following command in your terminal:
 
 ```bash
-pip install maitai-python
+pip install maitai-sdk-python
 ```
 
 ## Configuration
 
 Before you can start evaluating AI outputs, you need to initialize the SDK with your `application_id` and `api_key`. These credentials are essential for authenticating your requests to the MaiTai service.
 
 1. Obtain your `application_id` and `api_key` from the MaiTai platform.
@@ -112,8 +112,8 @@
 maitai.Evaluator.evaluate(session_id, reference_id, content)
 ```
 
 This will send the evaluation request to the MaiTai service asynchronously. Ensure that your `application_id` and `api_key` are correctly set as shown in the Configuration section above.
 
 ## Conclusion
 
-You're now ready to start using the MaiTai Python SDK to evaluate AI outputs in your application. Remember to follow best practices for managing your `api_key` and `application_id` securely within your application. If you encounter any issues or have further questions, refer to the [MaiTai Documentation](https://docs.maitai.ai) or reach out to the support team.
+You're now ready to start using the MaiTai Python SDK to evaluate AI outputs in your application. Remember to follow best practices for managing your `api_key` and `application_id` securely within your application. If you encounter any issues or have further questions, refer to the [MaiTai Documentation](https://docs.maitai.ai) or reach out to the support team.
```

### Comparing `maitai_sdk_python-0.373/maitai/_config.py` & `maitai_sdk_python-0.374/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.373/maitai/_eval_request.py` & `maitai_sdk_python-0.374/maitai/_eval_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         self.id = -1
         self.date_created = -1
         self.application_id = -1
         self.session_id = None
         self.reference_id = None
         self.evaluation_content_type = ''
         self.evaluation_content = ''
+        self.action_type = ''
 
 
 class EvalRequestEncoder(JSONEncoder):
     def default(self, o):
         try:
             return o.__dict__
         except Exception as e:
```

### Comparing `maitai_sdk_python-0.373/maitai/_evaluator.py` & `maitai_sdk_python-0.374/maitai/_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 
     @classmethod
     def evaluate(cls, session_id, reference_id, content):
         eval_request: EvalRequest = cls.create_eval_request(session_id, reference_id, content)
         cls.send_evaluation_request(eval_request)
 
     @classmethod
-    def create_eval_request(cls, session_id, reference_id, content):
+    def create_eval_request(cls, session_id, reference_id, action_type, content):
         if type(content) != str:
             raise Exception('Content must be a string')
         eval_request: EvalRequest = EvalRequest()
         eval_request.application_id = config.application_id
         eval_request.session_id = session_id
         eval_request.reference_id = reference_id
+        eval_request.action_type = action_type
         eval_request.evaluation_content = content
         eval_request.evaluation_content_type = 'text'
         return eval_request
 
     @classmethod
     def update_session_context(cls, session_id, context):
         if type(context) != dict:
```

### Comparing `maitai_sdk_python-0.373/maitai/_loadable.py` & `maitai_sdk_python-0.374/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.373/setup.py` & `maitai_sdk_python-0.374/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai_sdk_python',
-    version='0.373',
+    version='0.374',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     # Optional metadata
     author='Christian DalSanto',
     author_email='christian@yewpay.com',
```

