# Comparing `tmp/identity-trace-python-agent-1.0.5.tar.gz` & `tmp/identity-trace-python-agent-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "identity-trace-python-agent-1.0.5.tar", last modified: Fri Mar 29 21:17:19 2024, max compression
+gzip compressed data, was "identity-trace-python-agent-1.0.6.tar", last modified: Mon Apr  8 23:03:20 2024, max compression
```

## Comparing `identity-trace-python-agent-1.0.5.tar` & `identity-trace-python-agent-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-03-29 21:17:19.304187 identity-trace-python-agent-1.0.5/
--rw-r--r--   0 mamoon     (501) staff       (20)      321 2024-03-29 21:17:19.303908 identity-trace-python-agent-1.0.5/PKG-INFO
-drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-03-29 21:17:19.302762 identity-trace-python-agent-1.0.5/identity_trace/
--rw-r--r--   0 mamoon     (501) staff       (20)       57 2024-03-28 12:00:23.000000 identity-trace-python-agent-1.0.5/identity_trace/__init__.py
--rw-r--r--   0 mamoon     (501) staff       (20)     5391 2024-03-29 21:13:34.000000 identity-trace-python-agent-1.0.5/identity_trace/decorator.py
--rw-r--r--   0 mamoon     (501) staff       (20)      609 2024-03-29 21:14:11.000000 identity-trace-python-agent-1.0.5/identity_trace/registry.py
--rw-r--r--   0 mamoon     (501) staff       (20)     3917 2024-03-29 21:14:29.000000 identity-trace-python-agent-1.0.5/identity_trace/runner.py
--rw-r--r--   0 mamoon     (501) staff       (20)     1275 2024-03-29 21:13:50.000000 identity-trace-python-agent-1.0.5/identity_trace/tracer.py
-drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-03-29 21:17:19.303671 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/
--rw-r--r--   0 mamoon     (501) staff       (20)      321 2024-03-29 21:17:19.000000 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/PKG-INFO
--rw-r--r--   0 mamoon     (501) staff       (20)      394 2024-03-29 21:17:19.000000 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/SOURCES.txt
--rw-r--r--   0 mamoon     (501) staff       (20)        1 2024-03-29 21:17:19.000000 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/dependency_links.txt
--rw-r--r--   0 mamoon     (501) staff       (20)       20 2024-03-29 21:17:19.000000 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/requires.txt
--rw-r--r--   0 mamoon     (501) staff       (20)       15 2024-03-29 21:17:19.000000 identity-trace-python-agent-1.0.5/identity_trace_python_agent.egg-info/top_level.txt
--rw-r--r--   0 mamoon     (501) staff       (20)       38 2024-03-29 21:17:19.304238 identity-trace-python-agent-1.0.5/setup.cfg
--rw-r--r--   0 mamoon     (501) staff       (20)      437 2024-03-29 21:17:17.000000 identity-trace-python-agent-1.0.5/setup.py
+drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-04-08 23:03:20.911370 identity-trace-python-agent-1.0.6/
+-rw-r--r--   0 mamoon     (501) staff       (20)      321 2024-04-08 23:03:20.911051 identity-trace-python-agent-1.0.6/PKG-INFO
+drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-04-08 23:03:20.909546 identity-trace-python-agent-1.0.6/identity_trace/
+-rw-r--r--   0 mamoon     (501) staff       (20)       57 2024-03-28 12:00:23.000000 identity-trace-python-agent-1.0.6/identity_trace/__init__.py
+-rw-r--r--   0 mamoon     (501) staff       (20)     5916 2024-04-08 22:54:29.000000 identity-trace-python-agent-1.0.6/identity_trace/decorator.py
+-rw-r--r--   0 mamoon     (501) staff       (20)      966 2024-04-05 02:35:01.000000 identity-trace-python-agent-1.0.6/identity_trace/registry.py
+-rw-r--r--   0 mamoon     (501) staff       (20)     7519 2024-04-08 22:54:55.000000 identity-trace-python-agent-1.0.6/identity_trace/runner.py
+-rw-r--r--   0 mamoon     (501) staff       (20)     1275 2024-03-29 21:24:19.000000 identity-trace-python-agent-1.0.6/identity_trace/tracer.py
+drwxr-xr-x   0 mamoon     (501) staff       (20)        0 2024-04-08 23:03:20.910727 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/
+-rw-r--r--   0 mamoon     (501) staff       (20)      321 2024-04-08 23:03:20.000000 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/PKG-INFO
+-rw-r--r--   0 mamoon     (501) staff       (20)      394 2024-04-08 23:03:20.000000 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 mamoon     (501) staff       (20)        1 2024-04-08 23:03:20.000000 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 mamoon     (501) staff       (20)       20 2024-04-08 23:03:20.000000 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/requires.txt
+-rw-r--r--   0 mamoon     (501) staff       (20)       15 2024-04-08 23:03:20.000000 identity-trace-python-agent-1.0.6/identity_trace_python_agent.egg-info/top_level.txt
+-rw-r--r--   0 mamoon     (501) staff       (20)       38 2024-04-08 23:03:20.911446 identity-trace-python-agent-1.0.6/setup.cfg
+-rw-r--r--   0 mamoon     (501) staff       (20)      437 2024-04-08 23:03:11.000000 identity-trace-python-agent-1.0.6/setup.py
```

### Comparing `identity-trace-python-agent-1.0.5/identity_trace/decorator.py` & `identity-trace-python-agent-1.0.6/identity_trace/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from .registry import register_frame, is_frame_registered, remove_frame, register_function
+from .registry import register_frame, is_frame_registered, remove_frame, register_function, get_function_processor_callbacks
 from .tracer import trace_function
 import inspect
 import json
 import datetime
 
 
 class FunctionTrace:
@@ -26,20 +26,25 @@
     parent_id = None
     executed_successfully = None
     error = None
 
     start_time = None
     end_time = None
 
+    children = []
+
+    execution_context = None
+
     def serialize(self):
         return dict(
             config={
                 'trace_input': self.config['trace_input'],
                 'trace_output': self.config['trace_output'],
             },
+            executionContext = self.execution_context,
             packageName=self.package_name,
             fileName=self.file_name,
             moduleName=self.module_name,
             name=self.name,
             description=self.description,
             functionID=self.function_id,
             input=json.loads(self.input),
@@ -64,14 +69,16 @@
 
         package_name = caller_module_frame.f_globals['__package__']
         file_name = caller_module_frame.f_globals['__file__']
         module_name = caller_module_frame.f_globals['__name__']
         function_name = name or func.__name__
         function_id = id(func)
 
+
+        
         
 
         def inner(*args, **kwargs):
 
             # register current function run
             frame = inspect.currentframe()
 
@@ -88,14 +95,15 @@
                 
                 parent_context_copy = copy_parent_context(parent_execution_context)
                 execution_context.update(parent_context_copy)
 
             register_frame(frame, execution_context)
 
             function_trace_instance = FunctionTrace()
+            function_trace_instance.execution_context = dict()
             function_trace_instance.name = function_name
             function_trace_instance.file_name = file_name
             function_trace_instance.package_name = package_name
             function_trace_instance.function_id = function_id
             function_trace_instance.parent_id = parent_id
             function_trace_instance.module_name = module_name
 
@@ -106,15 +114,23 @@
             if function_trace_instance.config.get('trace_input', None):
                 function_trace_instance.input = function_trace_instance.config['serializer']([
                     *args, kwargs
                 ])
 
             try:
                 function_trace_instance.start_time = datetime.datetime.now().timestamp()
-                output = func(*args, **kwargs)
+                output = None
+                
+                funtion_to_call = func
+                callbacks = get_function_processor_callbacks()
+                if callbacks:
+                    funtion_to_call = callbacks(function_trace_instance, funtion_to_call)
+                
+                output = funtion_to_call(*args, **kwargs)
+                
                 function_trace_instance.end_time = datetime.datetime.now().timestamp()
 
                 if function_trace_instance.config.get('trace_output', None):
                     # serialize input
                     function_trace_instance.output = function_trace_instance.config['serializer'](
                         output)
```

### Comparing `identity-trace-python-agent-1.0.5/identity_trace/registry.py` & `identity-trace-python-agent-1.0.6/identity_trace/registry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 
 _function_registry = {}
 __function_registry = {}
+__function_processor_map = dict()
 
 
 def register_frame(frame, execution_context):
     _function_registry[_get_frame_id(frame)] = execution_context
 
 
 def is_frame_registered(frame):
@@ -23,7 +24,23 @@
 
 def register_function(function_name, func):
     __function_registry[function_name] = func
 
 
 def get_function_by_name(function_name):
     return __function_registry.get(function_name, None)
+
+
+def register_function_processor(callback):
+
+    __function_processor_map['callback'] = callback
+
+
+def remove_function_processor_callback():
+
+    try:
+        del __function_processor_map['callback']
+    except:
+        ...
+
+def get_function_processor_callbacks():
+    return __function_processor_map.get('callback', None)
```

### Comparing `identity-trace-python-agent-1.0.5/identity_trace/tracer.py` & `identity-trace-python-agent-1.0.6/identity_trace/tracer.py`

 * *Files identical despite different names*

