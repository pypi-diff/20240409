# Comparing `tmp/one4all_iop_models-0.1.4.tar.gz` & `tmp/one4all_iop_models-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one4all_iop_models-0.1.4.tar", max compression
+gzip compressed data, was "one4all_iop_models-0.1.5.tar", max compression
```

## Comparing `one4all_iop_models-0.1.4.tar` & `one4all_iop_models-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      364 2024-04-05 11:27:20.728544 one4all_iop_models-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-05 11:27:20.728544 one4all_iop_models-0.1.4/one4all_iop_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 11:27:20.728544 one4all_iop_models-0.1.4/one4all_iop_models/ros_models/__init__.py
--rw-r--r--   0        0        0     2595 2024-04-05 11:27:20.728544 one4all_iop_models-0.1.4/one4all_iop_models/ros_models/robot.py
--rw-r--r--   0        0        0      547 2024-04-05 11:27:20.728544 one4all_iop_models-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-04-09 08:19:59.741936 one4all_iop_models-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:19:59.741936 one4all_iop_models-0.1.5/one4all_iop_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:19:59.741936 one4all_iop_models-0.1.5/one4all_iop_models/ros_models/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-09 08:19:59.741936 one4all_iop_models-0.1.5/one4all_iop_models/ros_models/robot.py
+-rw-r--r--   0        0        0      547 2024-04-09 08:19:59.741936 one4all_iop_models-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.5/PKG-INFO
```

### Comparing `one4all_iop_models-0.1.4/one4all_iop_models/ros_models/robot.py` & `one4all_iop_models-0.1.5/one4all_iop_models/ros_models/robot.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     @validator('name')
     def validate_name(cls, v):
         if v != "awcombo":
             raise ValueError("name must be 'awcombo'")
         return v
 
-    def __init__(self, x, y, angle):
+    def __init__(self, name, x, y, angle):
         self.x = x
         self.y = y
         self. angle = angle
 
 
 class Joint(BaseModel):
     name: Literal["joint"] = "joint"
@@ -43,15 +43,15 @@
 
     @validator('name')
     def validate_name(cls, v):
         if v != "joint":
             raise ValueError("name must be 'joint'")
         return v
 
-    def __init__(self, j1, j2, j3, j4, j5, j6):
+    def __init__(self, name, j1, j2, j3, j4, j5, j6):
         self.j1 = j1
         self.j2 = j2
         self.j3 = j3
         self.j4 = j4
         self.j5 = j5
         self.j6 = j6
 
@@ -64,15 +64,15 @@
 
     @validator('name')
     def validate_name(cls, v):
         if v != "carte":
             raise ValueError("name must be 'carte'")
         return v
 
-    def __init__(self, x, y, z):
+    def __init__(self, name, x, y, z):
         self.x = x
         self.y = y
         self.z = z
 
 
 class Increm(BaseModel):
     name: Literal["increm"] = "increm"
@@ -81,14 +81,14 @@
 
     @validator('name')
     def validate_name(cls, v):
         if v != "increm":
             raise ValueError("name must be 'increm'")
         return v
 
-    def __init__(self, axis, delta):
+    def __init__(self, name, axis, delta):
         self.axis = axis
         self.delta = delta
 
 
 class SubTask(BaseModel):
     actions: List[Union[Increm, AWCombo, Carte, Joint]]
```

### Comparing `one4all_iop_models-0.1.4/pyproject.toml` & `one4all_iop_models-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one4all-iop-models"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Ignacio Jimenez <ignacio.jimenez@idener.ai>"]
 readme = "README.md"
 packages = [{include = "one4all_iop_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `one4all_iop_models-0.1.4/PKG-INFO` & `one4all_iop_models-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one4all-iop-models
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Ignacio Jimenez
 Author-email: ignacio.jimenez@idener.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

