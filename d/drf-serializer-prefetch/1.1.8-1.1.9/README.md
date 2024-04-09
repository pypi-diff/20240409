# Comparing `tmp/drf-serializer-prefetch-1.1.8.tar.gz` & `tmp/drf-serializer-prefetch-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.1.8.tar", last modified: Tue Nov 21 20:55:17 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.1.9.tar", last modified: Fri Dec  8 18:41:49 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.1.8.tar` & `drf-serializer-prefetch-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:55:17.088192 drf-serializer-prefetch-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2023-11-21 20:55:17.088192 drf-serializer-prefetch-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:55:17.088192 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2023-11-21 20:55:17.000000 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-21 20:55:17.000000 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 20:55:17.000000 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-21 20:55:17.000000 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-21 20:55:17.000000 drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:55:17.084191 drf-serializer-prefetch-1.1.8/serializer_prefetch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/serializer_prefetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/serializer_prefetch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/serializer_prefetch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 20:55:17.088192 drf-serializer-prefetch-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 20:55:17.084191 drf-serializer-prefetch-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    29435 2023-11-21 20:55:09.000000 drf-serializer-prefetch-1.1.8/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 18:41:49.586524 drf-serializer-prefetch-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2023-12-08 18:41:49.586524 drf-serializer-prefetch-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 18:41:49.582524 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2023-12-08 18:41:49.000000 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-08 18:41:49.000000 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 18:41:49.000000 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 18:41:49.000000 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-08 18:41:49.000000 drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 18:41:49.582524 drf-serializer-prefetch-1.1.9/serializer_prefetch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/serializer_prefetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/serializer_prefetch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/serializer_prefetch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 18:41:49.586524 drf-serializer-prefetch-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 18:41:49.582524 drf-serializer-prefetch-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29984 2023-12-08 18:41:38.000000 drf-serializer-prefetch-1.1.9/tests/test_serializers.py
```

### Comparing `drf-serializer-prefetch-1.1.8/LICENSE` & `drf-serializer-prefetch-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/PKG-INFO` & `drf-serializer-prefetch-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.1.8
+Version: 1.1.9
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2.0
```

### Comparing `drf-serializer-prefetch-1.1.8/README.md` & `drf-serializer-prefetch-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.1.9/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.1.8
+Version: 1.1.9
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2.0
```

### Comparing `drf-serializer-prefetch-1.1.8/pyproject.toml` & `drf-serializer-prefetch-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.1.9/serializer_prefetch/base.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/serializer_prefetch/utils.py` & `drf-serializer-prefetch-1.1.9/serializer_prefetch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 def is_model_field(model, source):
     if hasattr(model, "_meta"):
         try:
             model_field = model._meta.get_field(source)
             if not isinstance(model_field, DjangoModelField | ForeignObjectRel):
                 return False
         except FieldDoesNotExist:
+            if source.endswith("_set"):
+                return is_model_field(model, source[:-4])
+
             return False
 
     return True
 
 
 def join_prefetch(current_relation: Prefetch | str, item: Prefetch | str):
     if isinstance(item, str):
```

### Comparing `drf-serializer-prefetch-1.1.8/setup.py` & `drf-serializer-prefetch-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Standard libraries
 from pathlib import Path
 
 # drf-serializer-prefetch
 from setuptools import find_packages, setup
 
-VERSION = "1.1.8"
+VERSION = "1.1.9"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
```

### Comparing `drf-serializer-prefetch-1.1.8/tests/models.py` & `drf-serializer-prefetch-1.1.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/tests/serializers.py` & `drf-serializer-prefetch-1.1.9/tests/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/tests/test_conditions.py` & `drf-serializer-prefetch-1.1.9/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/tests/test_errors.py` & `drf-serializer-prefetch-1.1.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.1.8/tests/test_serializers.py` & `drf-serializer-prefetch-1.1.9/tests/test_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 # Rest Framework
 from rest_framework import serializers
 
 # drf-serializer-prefetch
 from serializer_prefetch import PrefetchingSerializerMixin
 from tests.models import Continent, Country, Pizza, Topping
-from tests.serializers import CountrySerializer, PizzaSerializer, ToppingSerializer
+from tests.serializers import (
+    ContinentSerializer,
+    CountrySerializer,
+    PizzaSerializer,
+    ToppingSerializer,
+)
 
 
 class SerializersTestCase(TestCase):
     @classmethod
     def setUpTestData(cls) -> None:
         cls.america = Continent.objects.create(label="America")
         cls.asia = Continent.objects.create(label="Asia")
@@ -940,7 +945,23 @@
                 fields = ("label", "toppings")
 
         pizzas = Pizza.objects.all()
         serializer = PizzaSerializer(pizzas, many=True)
 
         with self.assertNumQueries(2):
             serializer.data
+
+    def test_reverse_many_to_many_relation(self):
+        class ContinentSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            country_set = CountrySerializer(many=True)
+
+            class Meta:
+                model = Continent
+                fields = ("label", "country_set")
+
+        continents = Continent.objects.all()
+        serializer = ContinentSerializer(continents, many=True)
+
+        with self.assertNumQueries(2):
+            serializer.data
```

