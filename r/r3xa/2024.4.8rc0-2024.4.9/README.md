# Comparing `tmp/r3xa-2024.4.8rc0.tar.gz` & `tmp/r3xa-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3xa-2024.4.8rc0.tar", max compression
+gzip compressed data, was "r3xa-2024.4.9.tar", max compression
```

## Comparing `r3xa-2024.4.8rc0.tar` & `r3xa-2024.4.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      205 2024-04-08 14:53:40.771597 r3xa-2024.4.8rc0/README.md
--rw-r--r--   0        0        0     1553 2024-04-08 14:53:40.771597 r3xa-2024.4.8rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 14:53:40.797597 r3xa-2024.4.8rc0/r3xa/__init__.py
--rw-r--r--   0        0        0     3864 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/r3xa/gui/gui.py
--rw-r--r--   0        0        0     7128 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/r3xa/metadata.py
--rw-r--r--   0        0        0      552 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/r3xa/scripts.py
--rw-r--r--   0        0        0     1225 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/r3xa/utils.py
--rw-r--r--   0        0        0      515 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/r3xa/validation.py
--rw-r--r--   0        0        0    30724 2024-04-08 14:53:40.772597 r3xa-2024.4.8rc0/resources/schema.json
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 r3xa-2024.4.8rc0/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-09 21:03:33.990332 r3xa-2024.4.9/README.md
+-rw-r--r--   0        0        0     1603 2024-04-09 21:03:33.990332 r3xa-2024.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 21:03:34.013332 r3xa-2024.4.9/r3xa/__init__.py
+-rw-r--r--   0        0        0    13620 2024-04-09 21:03:33.990332 r3xa-2024.4.9/r3xa/gui.py
+-rw-r--r--   0        0        0     7340 2024-04-09 21:03:33.990332 r3xa-2024.4.9/r3xa/metadata.py
+-rw-r--r--   0        0        0     1167 2024-04-09 21:03:33.990332 r3xa-2024.4.9/r3xa/scripts.py
+-rw-r--r--   0        0        0     2743 2024-04-09 21:03:33.990332 r3xa-2024.4.9/r3xa/utils.py
+-rw-r--r--   0        0        0      515 2024-04-09 21:03:33.991332 r3xa-2024.4.9/r3xa/validation.py
+-rw-r--r--   0        0        0    30249 2024-04-09 21:03:33.991332 r3xa-2024.4.9/resources/schema.json
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 r3xa-2024.4.9/PKG-INFO
```

### Comparing `r3xa-2024.4.8rc0/pyproject.toml` & `r3xa-2024.4.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r3xa"
-version = "2024.4.8c"
+version = "2024.4.9"
 description = "Remember, Reuse and Replicate eXperiments and Analyses"
 authors = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 maintainers = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 homepage = "https://photomecanics.gitlab.io/r3xa/doc"
 repository = "https://gitlab.com/photomecanics/r3xa"
 keywords = []
 readme = "README.md"
@@ -15,14 +15,15 @@
 ]
 include = ["resources/schema.json"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 jsonschema = "*"
 python-slugify = "*"
+PyQt5 = "=5.15.2"
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pre-commit = "*"
 coverage = "*"
@@ -30,14 +31,15 @@
 poethepoet = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
+r3xa = "r3xa.scripts:script_gui"
 r3xa-validate = "r3xa.scripts:script_validate"
 
 [tool.poe.tasks]
 # build html doc
 doc_json = "poetry run generate-schema-doc --config no_link_to_reused_ref --config copy_js --config no_collapse_long_descriptions --config no_collapse_long_examples resources/schema.json doc/index.html"
 doc = ["doc_json"]
 # build coverage
```

### Comparing `r3xa-2024.4.8rc0/r3xa/metadata.py` & `r3xa-2024.4.9/r3xa/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import slugify
 import json
 
-from r3xa.utils import get_schema, random_slug, obj
+from r3xa.utils import get_schema, random_slug, obj, obj_iter, slugify_file_name, highlight_json
 from r3xa.validation import validate
 
 #####################
 # Meta data classes #
 #####################
 
 
@@ -15,40 +15,27 @@
     ```json
     {
         "unit": {"type": "string"},
         "value": {"type": "float"},
         "scale": {"type": "float"}
     }
     ```
-
-    Note:
-    -----
-       `scale` is not returned if None
-       `value` is returned as null if None
     """
 
     def __init__(self, unit: str, value: float = None, scale: float = None):
         self.unit = unit
         self.value = value
         self.scale = scale
 
-    def __iter__(self):
-        yield "unit", self.unit
-        yield "value", self.value
-        # return scale only if defined
-        if self.scale:
-            yield "scale", self.scale
-
     def __str__(self):
-        if self.value and self.scale:
-            return f"{self.value} {self.unit} (x{self.scale:.1e} to SI)"
-        elif self.value:
-            return f"{self.value} {self.unit}"
-        else:
-            return self.unit
+        return highlight_json(self)
+
+    def __iter__(self):
+        for k, v in obj_iter(self):
+            yield k, v
 
 
 class DataSetFile:
     """Independant class that handles data set file (either `timestamps` or `data`) to produces json objects formated as:
     ```json
     {
         "filename": {"type": "string"},
@@ -60,60 +47,48 @@
 
     def __init__(self, filename: str, data_range: list, delimiter: str = ";"):
         self.filename = filename
         self.data_range = data_range
         self.delimiter = delimiter
 
     def __iter__(self):
-        for k, v in self.__dict__.items():
+        for k, v in obj_iter(self):
             yield k, v
 
     def __str__(self):
-        return f"{self.filename} from {self.data_range[0]} to {self.data_range[1]}"
+        return highlight_json(self)
 
 
 class Data:
     """Generic parent class for `data_sets`, `data_sources` and `settings`.
     It can take any `key: values` arguments to keep flexible in view of specs changes.
     Therefore it is agnostic to the specifications implemented in the scheme.
 
     It implements the `__iter__` function to ease the conversion to json objects.
     """
 
-    def __init__(self, title="My Data", **kwargs):
-        # force title default to be sure to build an id
-        self.title = title
-
+    def __init__(self, **kwargs):
         # get all attributes from the kwargs and set them
         for k, v in kwargs.items():
+            # if obj(v):
+            #     setattr(self, k, v)
             setattr(self, k, v)
 
         # define an ID of the data as the slugified title appended with and random slug
-        self.id = slugify.slugify(self.title) + "_" + random_slug()
-
-        print(f"Init {self}")
+        if not hasattr(self, "id"):
+            if hasattr(self, "title"):
+                self.id = slugify.slugify(self.title) + "_" + random_slug()
+            else:
+                self.id = "no_title_" + random_slug()
 
     def __str__(self):
-        return f"{self.title} [{self.id}]"
+        return highlight_json(self)
 
     def __iter__(self):
-        """Defines the conversion between instance and dictionnary
-        It does ouput unset values and convert list of Iterable to dict if possible.
-        """
-        for k, v in self.__dict__.items():
-            # ignore unset values
-            if not v:
-                continue
-
-            # convert list of Iterable to list of dict if possible
-            # used for our own classes where __iter__ is defined
-            if isinstance(v, list):
-                v = [obj(_) for _ in v]
-
-            # yield the key: value pair
+        for k, v in obj_iter(self):
             yield k, v
 
     def check_keywords(self, data_type):
         """Raise ValueError if the attributes of the instance does not match
         any required keys of each objects of data_type.
 
         data_type can be "setting", "data_source" or "data_set"
@@ -146,89 +121,124 @@
         missing = set.intersection(*missing_keys)
 
         if len(missing):
             raise ValueError(f"Missing at least the following keys: {missing}")
 
 
 class Setting(Data):
-    def __init__(self, title="My setting", **kwargs):
-        super().__init__(title=title, **kwargs)
-        self.check_keywords("setting")
-
-    def __str__(self):
-        return f"Setting: {self.title} [{self.id}]"
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if len(kwargs):  # skip check if no kwargs entered
+            self.check_keywords("setting")
+
+    def load_json(self, payload):
+        for k, v in payload.items():
+            setattr(self, k, obj(v))
 
 
 class DataSource(Data):
-    def __init__(self, title="My data source", **kwargs):
-        super().__init__(title=title, **kwargs)
-        self.check_keywords("data_source")
-
-    def __str__(self):
-        return f"Data source: {self.title} [{self.id}]"
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if len(kwargs):  # skip check if no kwargs entered
+            self.check_keywords("data_source")
 
     def add_data_set(self, data_set: Data):
         self.input_data_set = data_set.id
 
 
 class DataSet(Data):
-    def __init__(self, title="My data set", **kwargs):
-        super().__init__(title=title, **kwargs)
-        self.check_keywords("data_set")
-
-    def __str__(self):
-        return f"Data set: {self.title} [{self.id}]"
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if len(kwargs):  # skip check if no kwargs entered
+            self.check_keywords("data_set")
 
     def add_data_source(self, data_source: Data):
         if not hasattr(self, "data_sources"):
             self.data_sources = []
         self.data_sources.append(data_source.id)
         # self.data_sources = datasource.id
 
 
 class MetaData:
     def __init__(self, **kargs):
         schema = get_schema()
         for k, v in kargs.items():
-            setattr(self, k, v)
+            if obj(v):
+                setattr(self, k, v)
+
+        # add by default settings / data_sources and data_sets
+        for k in ["settings", "data_sources", "data_sets"]:
+            if not hasattr(self, k):
+                setattr(self, k, [])
+
+            # sanity check to remove duplicated ID
+            data = {d.id: d for d in getattr(self, k)}
+            setattr(self, k, list(data.values()))
 
         # enforce version from schema
         self.version = schema["properties"]["version"]["const"]
 
+    def __iter__(self):
+        for k, v in obj_iter(self):
+            yield k, v
+
+    def __str__(self):
+        return highlight_json(self)
+
+    def validate(self):
+        validate(dict(self))
+
+    def create_or_modify(self, what, where):
+        """Insure that when we had Data we don't duplicate the same ID."""
+        # get existing data and use id as a key
+        data = {d.id: d for d in getattr(self, where)}
+
+        # add current data to existing (by the key)
+        data[what.id] = what
+
+        # convert dict to list of data
+        setattr(self, where, list(data.values()))
+
     def add_setting(self, setting: Setting):
-        if not hasattr(self, "settings"):
-            self.settings = []
-        self.settings.append(setting)
+        self.create_or_modify(setting, "settings")
 
     def add_data_source(self, data_source: DataSource):
-        if not hasattr(self, "data_sources"):
-            self.data_sources = []
-        self.data_sources.append(data_source)
+        self.create_or_modify(data_source, "data_sources")
 
     def add_data_set(self, data_set: DataSet):
-        if not hasattr(self, "data_sets"):
-            self.data_sets = []
-        self.data_sets.append(data_set)
-
-    def create_json(self, name: str = None, check: bool = True):
-        # init metadata dictionary
-        metadata = {}
+        self.create_or_modify(data_set, "data_sets")
 
-        # slugify the json file name
-        # if not set use the title
-        name = slugify.slugify(name if name else self.title)
+    def load(self, payload):
+        """Fill class attributes based on a payload"""
+        # Global
+        for k, v in payload.items():
+            if k in ["settings", "data_sources", "data_sets"]:
+                continue
+            if not obj(v):
+                continue
+            setattr(self, k, obj(v))
 
-        # build dictionnary
-        for k, v in self.__dict__.items():
-            # ignore specific keywords
-            # if k in []:
-            #     continue
+        # Settings
+        for p in payload.get("settings", []):
+            s = Setting()
+            s.load_json(p)
+            self.add_setting(s)
 
-            # convert iterable to sereliazable objects
-            metadata[k] = obj(v)
+        # Data Source
 
-        # write file
-        json.dump(metadata, open(f"{name}.json", "w"), indent=4)
+        # Data Sets
 
+    def save_json(self, name: str = None, check: bool = True):
+        """Appends .json to name"""
         # check validity
         if check:
-            validate(metadata)
+            validate(dict(self))
+
+        # slugify the json file name
+        # if not set use the title
+        if name:
+            name = slugify_file_name(name)
+        else:
+            name = slugify.slugify(self.title)
+
+        # write file
+        json.dump(dict(self), open(name + ".json", "w"), indent=4)
```

### Comparing `r3xa-2024.4.8rc0/r3xa/validation.py` & `r3xa-2024.4.9/r3xa/validation.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.8rc0/resources/schema.json` & `r3xa-2024.4.9/resources/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957017275620792%*

 * *Differences: {"'$defs'": "{'setting': {'generic': {'properties': {'kind': OrderedDict([('title', 'Kind'), "*

 * *            "('description', 'The kind of setting'), ('type', 'string'), ('const', 'generic')])}, "*

 * *            "'required': {insert: [(3, 'kind')]}}, 'specimen': {'properties': {'size': {'$ref': "*

 * *            "'#/$defs/types/unit', delete: ['type']}, 'kind': OrderedDict([('title', 'Kind'), "*

 * *            "('description', 'The kind of setting'), ('type', 'string'), ('const', 'specimen')]), "*

 * *            "delete: [' […]*

```diff
@@ -495,75 +495,71 @@
                         "type": "string"
                     },
                     "id": {
                         "description": "ID of the setting",
                         "title": "ID",
                         "type": "string"
                     },
+                    "kind": {
+                        "const": "generic",
+                        "description": "The kind of setting",
+                        "title": "Kind",
+                        "type": "string"
+                    },
                     "title": {
                         "description": "The title of setting",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "title",
-                    "description"
+                    "description",
+                    "kind"
                 ],
                 "title": "Generic setting",
                 "type": "object"
             },
             "specimen": {
                 "additionalProperties": false,
                 "description": "A specimen",
                 "properties": {
-                    "cad": {
-                        "description": "File of the CAD",
-                        "title": "CAD",
-                        "type": "string"
-                    },
                     "description": {
                         "description": "The description of your setting",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
                         "description": "ID of the setting",
                         "title": "ID",
                         "type": "string"
                     },
-                    "patterning_feature_size": {
-                        "$ref": "#/$defs/types/unit",
-                        "description": "The patterning feature size",
-                        "title": "Patterning feature size"
-                    },
-                    "patterning_technique": {
-                        "description": "The patterning technique",
-                        "examples": [
-                            "Base coat of white spray paint with ink stamped speckles"
-                        ],
-                        "title": "Patterning technique",
+                    "kind": {
+                        "const": "specimen",
+                        "description": "The kind of setting",
+                        "title": "Kind",
                         "type": "string"
                     },
                     "size": {
+                        "$ref": "#/$defs/types/unit",
                         "description": "The size of the specimen",
-                        "title": "Size",
-                        "type": "string"
+                        "title": "Size"
                     },
                     "title": {
                         "description": "The title of setting",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "title",
-                    "description"
+                    "description",
+                    "kind"
                 ],
                 "title": "Specimen",
                 "type": "object"
             }
         },
         "types": {
             "data set_file": {
@@ -638,26 +634,18 @@
                         "description": "ratio to the main unit",
                         "type": "number"
                     },
                     "unit": {
                         "type": "string"
                     },
                     "value": {
-                        "anyOf": [
-                            {
-                                "type": "number"
-                            },
-                            {
-                                "type": "null"
-                            }
-                        ]
+                        "type": "number"
                     }
                 },
                 "required": [
-                    "value",
                     "unit"
                 ],
                 "type": "object"
             },
             "uri": {
                 "$comment": "regex to prohibit spaces and accents.",
                 "description": "Name, path or ULR of the file (no spaces, no accents)",
@@ -665,22 +653,22 @@
             }
         }
     },
     "additionalProperties": false,
     "description": "This is the specs for the R3XA experiments and analysis meta data template.",
     "properties": {
         "authors": {
+            "$ref": "#/$defs/types/string",
             "description": "Authors of the data sets",
             "examples": [
                 "M. Palin, J. Cleese",
                 "ORCID",
                 "HAL-ID"
             ],
-            "title": "Author",
-            "type": "string"
+            "title": "Author"
         },
         "data_sets": {
             "description": "The data sets :)",
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/data_set/file"
@@ -717,17 +705,17 @@
                 "2020-03-17"
             ],
             "pattern": "^[1-2]{1}[0-9]{3}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$",
             "title": "Date",
             "type": "string"
         },
         "description": {
+            "$ref": "#/$defs/types/string",
             "description": "The description of the data sets",
-            "title": "Description",
-            "type": "string"
+            "title": "Description"
         },
         "documentation": {
             "$ref": "#/$defs/types/uri",
             "description": "URI to the documentation (pdf)",
             "examples": [
                 "./doc/my_doc.pdf",
                 "https://zenodo.org/records/42/doc/my_doc.pdf"
@@ -762,24 +750,25 @@
                     }
                 ]
             },
             "title": "Settings",
             "type": "array"
         },
         "title": {
+            "$ref": "#/$defs/types/string",
             "description": "The title of the data sets",
             "example": [
                 "DICComposite2.0",
                 "My awesome data sets"
             ],
             "title": "Title",
             "type": "string"
         },
         "version": {
-            "const": "2024.4.8",
+            "const": "2024.4.9",
             "description": "Version of the schema used",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "title",
```

### Comparing `r3xa-2024.4.8rc0/PKG-INFO` & `r3xa-2024.4.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: r3xa
-Version: 2024.4.8rc0
+Version: 2024.4.9
 Summary: Remember, Reuse and Replicate eXperiments and Analyses
 Home-page: https://photomecanics.gitlab.io/r3xa/doc
 Author: Emmanuel Roubin
 Author-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Maintainer: Emmanuel Roubin
 Maintainer-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Public Domain
 Classifier: Natural Language :: French
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyQt5 (==5.15.2)
 Requires-Dist: jsonschema
 Requires-Dist: python-slugify
 Project-URL: Repository, https://gitlab.com/photomecanics/r3xa
 Description-Content-Type: text/markdown
 
 # R3XA
 ## Remember, Reuse and Replicate eXperiments and Analyses
```

