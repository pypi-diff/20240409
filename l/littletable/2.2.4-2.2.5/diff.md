# Comparing `tmp/littletable-2.2.4.tar.gz` & `tmp/littletable-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littletable-2.2.4.tar", last modified: Thu Mar 21 19:25:19 2024, max compression
+gzip compressed data, was "littletable-2.2.5.tar", last modified: Tue Apr  9 01:44:58 2024, max compression
```

## Comparing `littletable-2.2.4.tar` & `littletable-2.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-21 19:25:19.644679 littletable-2.2.4/
--rw-rw-r--   0 paul      (1000) paul      (1000)    37980 2024-03-21 14:32:06.000000 littletable-2.2.4/CHANGES
--rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-09-20 02:26:55.000000 littletable-2.2.4/HowToUseLittletable.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-09-20 02:26:55.000000 littletable-2.2.4/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-09-20 02:26:55.000000 littletable-2.2.4/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)     7541 2024-03-21 19:25:19.644679 littletable-2.2.4/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-09-20 02:26:55.000000 littletable-2.2.4/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-03-21 19:25:19.644679 littletable-2.2.4/littletable.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     7541 2024-03-21 19:25:19.000000 littletable-2.2.4/littletable.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      249 2024-03-21 19:25:19.000000 littletable-2.2.4/littletable.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2024-03-21 19:25:19.000000 littletable-2.2.4/littletable.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       12 2024-03-21 19:25:19.000000 littletable-2.2.4/littletable.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)   174092 2024-03-21 14:32:06.000000 littletable-2.2.4/littletable.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2024-03-21 19:25:19.648679 littletable-2.2.4/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1517 2024-03-21 14:32:06.000000 littletable-2.2.4/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)   115622 2023-09-20 02:26:55.000000 littletable-2.2.4/unit_tests.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-04-09 01:44:58.004729 littletable-2.2.5/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    39011 2024-04-09 01:35:09.000000 littletable-2.2.5/CHANGES
+-rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-09-20 02:26:55.000000 littletable-2.2.5/HowToUseLittletable.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-09-20 02:26:55.000000 littletable-2.2.5/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-09-20 02:26:55.000000 littletable-2.2.5/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)     7541 2024-04-09 01:44:58.004729 littletable-2.2.5/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-09-20 02:26:55.000000 littletable-2.2.5/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2024-04-09 01:44:58.004729 littletable-2.2.5/littletable.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     7541 2024-04-09 01:44:57.000000 littletable-2.2.5/littletable.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      249 2024-04-09 01:44:57.000000 littletable-2.2.5/littletable.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2024-04-09 01:44:57.000000 littletable-2.2.5/littletable.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       12 2024-04-09 01:44:57.000000 littletable-2.2.5/littletable.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)   175186 2024-04-09 01:35:09.000000 littletable-2.2.5/littletable.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2024-04-09 01:44:58.004729 littletable-2.2.5/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1517 2024-03-21 14:32:06.000000 littletable-2.2.5/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)   117943 2024-04-09 01:35:09.000000 littletable-2.2.5/unit_tests.py
```

### Comparing `littletable-2.2.4/CHANGES` & `littletable-2.2.5/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,41 @@
 NOTE: Deprecated features will be removed in the 3.0 release of `littletable`:
 - `DataObject` class, replace with `typing.SimpleNamespace`, `dict`, `namedtuple`, or
   other user-defined class
 - `Table.re_match(patt)` comparator is deprecated, replace with
   `re.compile(patt).match`
 
 
+Version 2.2.5
+-------------
+- Enhanced `Table.by`, `Table.all`, and `Table.search` methods to accept a field name that is not
+  a valid identifier by using a callable interface:
+
+        tbl = lt.csv_import(
+            "https://github.com/lukes/ISO-3166-Countries-with-Regional-Codes/blob/master/all/all.csv?raw=true"
+            )
+
+        # field "region" is a valid Python identifier
+        regions = list(tbl.all.region.unique)
+
+        # field "sub-region" is not a valid Python identifier, use callable interface
+        sub_regions = list(tbl.all("sub-region").unique)
+
+- Added `examples/pyscript/matplotlib.html` example, showing how to use `littletable` within
+  a Pyscript static HTML file.
+
+- Fixed minor code error in `Table.by` when determining if an index is unique or not.
+  (Not a bug, just fixed some bug-prone code.)
+
+- Expanded `peps.py` example to Jupyter Notebook `PEPs data demo.ipynb`.
+
+- Renamed `delete_index` to `drop_index` for more symmetry with SQL. `delete_index` is retained
+  for compatibility.
+
+
 Version 2.2.4
 -------------
 - Added support for Python 3.13.
 
 - Renamed `sort` to `orderby` to make the symmetry with relational SQL more apparent.
   `sort` will be retained as a deprecated compatibility name.
```

### Comparing `littletable-2.2.4/LICENSE` & `littletable-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `littletable-2.2.4/PKG-INFO` & `littletable-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `littletable-2.2.4/README.md` & `littletable-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `littletable-2.2.4/littletable.egg-info/PKG-INFO` & `littletable-2.2.5/littletable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Download-URL: https://pypi.org/project/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `littletable-2.2.4/littletable.py` & `littletable-2.2.5/littletable.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     import rich
     from rich import box
 except ImportError:
     rich = None
     box = None
 
 version_info = namedtuple("version_info", "major minor micro release_level serial")
-__version_info__ = version_info(2, 2, 4, "final", 0)
+__version_info__ = version_info(2, 2, 5, "final", 0)
 __version__ = (
     "{}.{}.{}".format(*__version_info__[:3])
     + (f"{__version_info__.release_level[0]}{__version_info__.serial}", "")[
         __version_info__.release_level == "final"
     ]
 )
 __version_time__ = "21 Mar 2024 07:59 UTC"
@@ -526,14 +526,17 @@
     def __init__(self, ind, table):
         self._index = ind
         self._table: Table = table
 
     def __getattr__(self, attr):
         return getattr(self._index, attr)
 
+    def __call__(self, attr):
+        return getattr(self, attr)
+
     def _getitem_using_slice(self, k):
         where_selector = {
             (False, False, False): lambda: ValueError("must specify start and/or stop values for slice"),
             (False, True, False): lambda: Table.lt(k.stop),
             (True, False, False): lambda: Table.ge(k.start),
             (True, True, False): lambda: (Table.in_range(k.start, k.stop)
                                           if k.start < k.stop
@@ -623,14 +626,17 @@
                 vals = table_index.keys()
             else:
                 vals = chain.from_iterable(
                     repeat(k, len(table_index[k])) for k in table_index.keys()
                 )
         return _TableAttributeValueLister.UniquableIterator(vals)
 
+    def __call__(self, attr):
+        return getattr(self, attr)
+
 
 class _TableSearcher:
     def __init__(self, table):
         self.__table = table
 
     def __getattr__(self, attr):
         ret = partial(self.__table._search, attr)
@@ -664,14 +670,17 @@
             "min_score": int,
             "include_words": bool,
             "as_table": bool,
             "return": 'Table | list[tuple]'
         }
         return ret
 
+    def __call__(self, attr):
+        return getattr(self, attr)
+
     def __dir__(self):
         return list(self.__table._search_indexes)
 
 
 class _IndexAccessor:
     def __init__(self, table):
         self._table = table
@@ -698,39 +707,45 @@
             index behave very much like a Python dict)
           - if the index is non-unique, then all matching objects will be returned in a new Table,
             just as if a regular query had been performed; if no objects match the key value, an empty
             Table is returned and no exception is raised.
 
         If there is no index defined for the given attribute, then C{AttributeError} is raised.
         """
-        if attr in self._table._indexes:
-            ret = self._table._indexes[attr]
-            if isinstance(ret, _UniqueObjIndex):
-                ret = _UniqueObjIndexWrapper(ret, self._table)
-                ret.__doc__ = textwrap.dedent(
+        attr_index = self._table._indexes.get(attr)
+        if attr_index is not None:
+            if isinstance(attr_index, _UniqueObjIndex):
+                attr_index_wrapper = _UniqueObjIndexWrapper(attr_index, self._table)
+                attr_index_wrapper.__doc__ = textwrap.dedent(
                     f"""\
                     Index accessor by {attr!r}
                     
                     tbl.by.{attr}[attr_value] returns the object having {attr}=attr_value.
                     If no such object exists, raises KeyError.
                     """
                 )
-            if isinstance(ret, _ObjIndex):
-                ret = _ObjIndexWrapper(ret, self._table)
-                ret.__doc__ = textwrap.dedent(
+
+            else:
+                attr_index_wrapper = _ObjIndexWrapper(attr_index, self._table)
+                attr_index_wrapper.__doc__ = textwrap.dedent(
                     f"""\
                     Index accessor by {attr!r}
 
                     tbl.by.{attr}[attr_value] returns a new Table of all objects having {attr}=attr_value.
                     If no matching objects exist, returns an empty Table.
                     """
                 )
-            return ret
+
+            return attr_index_wrapper
+
         raise AttributeError(f"Table {self._table.table_name!r} has no index {attr!r}")
 
+    def __call__(self, attr):
+        return getattr(self, attr)
+
 
 _ImportExportDataContainer = Union[str, Path, Iterable[str], TextIO]
 
 
 class ImportSourceType(Enum):
     file = 0
     string = 1
@@ -1027,24 +1042,27 @@
 class Table(Generic[TableContent]):
     """
     Table is the main class in C{littletable}, for representing a collection of SimpleNamespaces or
     user-defined objects with publicly accessible attributes or properties.  Tables can be:
      - created, with an optional name, using standard Python L{C{Table() constructor}<__init__>}
      - indexed, with multiple indexes, with unique or non-unique values, see L{create_index}
      - queried, specifying values to exact match in the desired records, see L{where}
+     - searched, specifying words to search for in values, where words may be found in text
+       attributes, see L{create_search_index}
      - filtered (using L{where}), using a simple predicate function to match desired records;
        useful for selecting using inequalities or compound conditions
      - accessed directly for keyed values, using C{table.indexattribute[key]} - see L{__getattr__}
      - joined, using L{join_on} to identify attribute to be used for joining with another table, and
        L{join} or operator '+' to perform the actual join
      - pivoted, using L{pivot} to create a nested structure of sub-tables grouping objects
        by attribute values
      - grouped, using L{groupby} to create a summary table of computed values, grouped by a key
        attribute
-     - L{imported<csv_import>}/L{exported<csv_export>} to CSV-format files
+     - L{imported<csv_import>}/L{exported<csv_export>} to CSV-format files; also supports working
+       with TSV files, JSON files, and Excel spreadsheet files
     Queries and joins return their results as new Table objects, so that queries and joins can
     be easily performed as a succession of operations.
     """
 
     lt = staticmethod(_make_comparator(operator.lt))
     le = staticmethod(_make_comparator(operator.le))
     gt = staticmethod(_make_comparator(operator.gt))
@@ -1068,15 +1086,15 @@
         _make_comparator2(lambda lower, x, upper: x is not None and lower <= x < upper)
     )
 
     INNER_JOIN = object()
     LEFT_OUTER_JOIN = object()
     RIGHT_OUTER_JOIN = object()
     FULL_OUTER_JOIN = object()
-    OUTER_JOIN_TYPES = (LEFT_OUTER_JOIN, RIGHT_OUTER_JOIN, FULL_OUTER_JOIN)
+    _OUTER_JOIN_TYPES = (LEFT_OUTER_JOIN, RIGHT_OUTER_JOIN, FULL_OUTER_JOIN)
 
     @staticmethod
     def _wrap_dict(dd: Mapping[str, Any]) -> default_row_class:
         # do recursive wrap of dicts to namespace types
         ret = default_row_class(
             **{
                 k: v if not isinstance(v, Mapping) else Table._wrap_dict(v)
@@ -1218,49 +1236,62 @@
 
         self.import_time = None
         self.create_time = datetime.datetime.now().astimezone(datetime.timezone.utc)
         self.modify_time = self.create_time
 
         """
         C{'by'} is added as a pseudo-attribute on tables, to provide
-        dict-like access to the underlying records in the table by index key, as in::
+        dict-like 
+
+
+
+        """
+
+    @property
+    def all(self) -> _TableAttributeValueLister:
+        """
+        Use C{'all'} to access all the values of a particular table column as a sequence.
+        This is useful if passing the values on to another function that works with sequences
+        of values::
+
+            sum(customers.by.zipcode["12345"].all.order_total)
+
+        The follow-on attribute C{'unique'} can be added to return a list of values with
+        duplicates suppressed::
+
+            customer_zip_codes = customers.all.zipcode.unique
+
+        C{'all'} and C{'unique'} return a generator of the attribute values.
+        """
+        return _TableAttributeValueLister(self)
+
+    @property
+    def by(self) -> _IndexAccessor:
+        """
+        Use C{'by'} to access the Table's records by index key, as in::
 
             employees.by.socsecnum["000-00-0000"]
             customers.by.zipcode["12345"]
 
         The behavior differs slightly for unique and non-unique indexes:
          - if the index is unique, then retrieving a matching object, will return just the object;
            if there is no matching object, C{KeyError} is raised (making a table with a unique
            index behave very much like a Python dict)
          - if the index is non-unique, then all matching objects will be returned in a new Table,
            just as if a regular query had been performed; if no objects match the key value, an empty
            Table is returned and no exception is raised.
 
         If there is no index defined for the given attribute, then C{AttributeError} is raised.
-
-        C{'all'} is added as a pseudo-attribute to tables, to provide access to the
-        values of a particular table column as a sequence. This is useful if passing the
-        values on to another function that works with sequences of values.
-
-            sum(customers.by.zipcode["12345"].all.order_total)
-
         """
-
-    @property
-    def all(self) -> _TableAttributeValueLister:
-        return _TableAttributeValueLister(self)
-
-    @property
-    def by(self) -> _IndexAccessor:
         return _IndexAccessor(self)
 
     @property
     def search(self) -> _TableSearcher:
         """
-        Use search to find records matching given query.
+        Use C{'search'} to find records matching given query.
         Query is a list of keywords that may be found in a document. Keywords may be prefixed with
         "+" or "-" to indicate desired inclusion or exclusion. '++' and '--' will indicate a
         mandatory inclusion or exclusion. All other keywords will be optional,
         and will count toward a search score. Matching records will be returned in a list of
         (score, record) tuples, in descending order by score.
 
         Score will be computed as:
@@ -1399,15 +1430,15 @@
         Create full copy of the current table, including table contents
         and index definitions.
         """
         ret = self.copy_template().insert_many(self.obs)(name)
         return ret
 
     def create_index(
-        self, attr: str, unique: bool = False, accept_none: bool = False
+        self, attr: str, unique: bool = False, accept_none: bool = False, force: bool = False
     ) -> Table[TableContent]:
         """
         Create a new index on a given attribute.
 
         Having an index improves performance of sort and pivot methods.
         It also enables retrieving table contents using
         'table.by.<attr_name>[attr_value]' syntax.
@@ -1428,15 +1459,21 @@
         @param unique: flag indicating whether the indexed field values are
             expected to be unique across table entries
         @type unique: boolean
         @param accept_none: flag indicating whether None is an acceptable
             unique key value for this attribute (always True for non-unique
             indexes, default=False for unique indexes)
         @type accept_none: boolean
+        @param force: flag indicating whether the index should be created
+            even it if already exists (default = False)
+        @type force: boolean
         """
+        if force:
+            self.drop_index(attr)
+
         if attr in self._indexes:
             raise ValueError(f"index {attr!r} already defined for table")
 
         if unique:
             self._indexes[attr] = _UniqueObjIndex(attr, accept_none)
             self._uniqueIndexes = [
                 ind for ind in self._indexes.values() if ind.is_unique
@@ -1452,54 +1489,53 @@
                 if obval is not None or accept_none:
                     ind[obval] = obj
                 else:
                     raise KeyError("None is not an allowed key")
             return self
 
         except KeyError:
-            del self._indexes[attr]
-            self._uniqueIndexes = [
-                ind for ind in self._indexes.values() if ind.is_unique
-            ]
+            self.drop_index(attr)
             raise
 
-    def delete_index(self, attr: str) -> Table[TableContent]:
+    def drop_index(self, attr: str) -> Table[TableContent]:
         """
         Deletes an index from the Table.  Can be used to drop and rebuild an index,
         or to convert a non-unique index to a unique index, or vice versa.
         @param attr: name of an indexed attribute
         @type attr: string
         """
         if attr in self._indexes:
             del self._indexes[attr]
             self._uniqueIndexes = [
                 ind for ind in self._indexes.values() if ind.is_unique
             ]
         return self
 
+    delete_index = drop_index
+
     def get_index(self, attr: str) -> _ReadonlyObjIndexWrapper:
         return _ReadonlyObjIndexWrapper(self._indexes[attr], self.copy_template())
 
-    NON_WORD_STRIPPER_RE = re.compile(r"[^\w_]?([\w._-]*)[^\w.]*")
-    NON_WORD_STRIPPER2_RE = re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)(!>_-)$")
-    ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
-    SIGNIFICANT_WORD_ENDING_RE = re.compile(rf"[a-z]{{2,}}({'|'.join(_significant_word_endings)})$")
-
-    PLURAL_ENDING_IN_IES = re.compile(r"(.*[^aeiouy])ies$")
-    PLURAL_ENDING_IN_ES = re.compile(r"(.*(?:ch|ss|sh|x))es$")
-    PLURAL_ENDING_IN_ES2 = re.compile(r"(.*(?:[bcdfghklmnprstuvwxz]|(qu))e)s$")
-    PLURAL_ENDING_IN_S = re.compile(r"(.*[^aeious])s$")
-    SINGULAR_ENDING_IN_S = re.compile(r"(.*(?:ness|ics))$")
-
-    PLURAL_MATCH_SUBS = (
-        (PLURAL_ENDING_IN_IES, r"\1y"),
-        (PLURAL_ENDING_IN_ES, r"\1"),
-        (PLURAL_ENDING_IN_ES2, r"\1"),
-        (SINGULAR_ENDING_IN_S, r"\1"),
-        (PLURAL_ENDING_IN_S, r"\1"),
+    _NON_WORD_STRIPPER_RE = re.compile(r"[^\w_]?([\w._-]*)[^\w.]*")
+    _NON_WORD_STRIPPER2_RE = re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)(!>_-)$")
+    _ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
+    _SIGNIFICANT_WORD_ENDING_RE = re.compile(rf"[a-z]{{2,}}({'|'.join(_significant_word_endings)})$")
+
+    _PLURAL_ENDING_IN_IES = re.compile(r"(.*[^aeiouy])ies$")
+    _PLURAL_ENDING_IN_ES = re.compile(r"(.*(?:ch|ss|sh|x))es$")
+    _PLURAL_ENDING_IN_ES2 = re.compile(r"(.*(?:[bcdfghklmnprstuvwxz]|(qu))e)s$")
+    _PLURAL_ENDING_IN_S = re.compile(r"(.*[^aeious])s$")
+    _SINGULAR_ENDING_IN_S = re.compile(r"(.*(?:ness|ics))$")
+
+    _PLURAL_MATCH_SUBS = (
+        (_PLURAL_ENDING_IN_IES, r"\1y"),
+        (_PLURAL_ENDING_IN_ES, r"\1"),
+        (_PLURAL_ENDING_IN_ES2, r"\1"),
+        (_SINGULAR_ENDING_IN_S, r"\1"),
+        (_PLURAL_ENDING_IN_S, r"\1"),
     )
 
     @staticmethod
     def _normalize_word(s: str) -> str:
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
             re.compile(r"((?:\w\.){2,})"),
@@ -1516,51 +1552,51 @@
     @staticmethod
     def _normalize_word_gen(s: str, sw: frozenset) -> Iterable[str]:
         s = s.lower()
         if s in sw:
             return
 
         # strip non-word chars from front and back
-        stripper = Table.NON_WORD_STRIPPER_RE
+        stripper = Table._NON_WORD_STRIPPER_RE
         s = stripper.match(s).group(1)
 
         if s in sw:
             return
 
         # catch plurals
         if (sa := s.rstrip(",.!?;:'\"-")).isalpha():
             s = sa
             if s in sw:
                 return
 
             # check common plurals - if not found, check common plural patterns
             if not (sing := _plurals_map.get(s)):
-                sing = next((sub_match[0] for re_sub, re_repl in Table.PLURAL_MATCH_SUBS
+                sing = next((sub_match[0] for re_sub, re_repl in Table._PLURAL_MATCH_SUBS
                             if (sub_match := re_sub.subn(re_repl, s))[1]),
                             s)
 
             if sing and sing != s:
                 yield sing
             yield s
 
             # also add special ending words for code and documentation parsing
             if (
                 s.endswith(_significant_word_endings)
-                and (m := Table.SIGNIFICANT_WORD_ENDING_RE.match(s))
+                and (m := Table._SIGNIFICANT_WORD_ENDING_RE.match(s))
             ):
                 yield m[1]
 
             return
 
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
-            Table.ACRONYM_WITH_PERIODS,
+            Table._ACRONYM_WITH_PERIODS,
             # words that may be hyphenated or snake-case
             # (strip off any leading single non-word character)
-            Table.NON_WORD_STRIPPER2_RE,
+            Table._NON_WORD_STRIPPER2_RE,
         ]
         for match_re in match_res:
             if match := match_re.match(s):
                 g1 = match.group(1).lower()
                 yield g1.replace(".", "")
                 for sep in "-":
                     if sep in g1:
@@ -1704,15 +1740,15 @@
                 for kwd in self._normalize_word_gen(keyword[1:], stopwords):
                     plus_matches.pop(kwd, None)
                     if kwd not in minus_matches and kwd not in excl_matches:
                         minus_matches[kwd] = set(search_index.get(kwd, []))
 
             else:
                 for kwd in self._normalize_word_gen(keyword, stopwords):
-                    if m := Table.SIGNIFICANT_WORD_ENDING_RE.match(keyword):
+                    if m := Table._SIGNIFICANT_WORD_ENDING_RE.match(keyword):
                         if kwd == m[1]:
                             continue
                     if kwd in plus_matches or kwd in minus_matches:
                         continue
                     opt_matches[kwd] = set(search_index.get(kwd, []))
 
         # process word groups to determine correct set of reqd_matches
@@ -2392,19 +2428,19 @@
             object in each table)
         @type attrlist: string, or list of strings or C{(table,attribute[,alias])} tuples
             (list may contain both strings and tuples)
         @param kwargs: attributes to join on, given as additional named arguments
             of the form C{table1attr="table2attr"}, or a dict mapping attribute names.
         @returns: a new Table containing the joined data as new SimpleNamespaces
         """
-        if join_type not in Table.OUTER_JOIN_TYPES:
+        if join_type not in Table._OUTER_JOIN_TYPES:
             join_names = [
                 nm
                 for nm, join_var in vars(Table).items()
-                if join_var in Table.OUTER_JOIN_TYPES
+                if join_var in Table._OUTER_JOIN_TYPES
             ]
             raise ValueError(
                 f"join argument must be one of [{', '.join(f'Table.{nm}' for nm in join_names)}]"
             )
 
         if not kwargs:
             raise TypeError(
@@ -2942,14 +2978,16 @@
         @param encoding: string (default="UTF-8"); if csv_dest is provided as a string
             representing an output filename, an encoding argument can be provided
         @type encoding: string
         @param delimiter: string (default=",") - overridable delimiter for value separator
         @type delimiter: string
         @param kwargs: additional keyword args to pass through to csv.DictWriter
         @type kwargs: named arguments (optional)
+
+        If no destination file is given, the CSV-formatted data is returned as a string.
         """
         non_writer_args = "encoding csv_dest fieldnames".split()
         writer_args = {
             k: v for k, v in kwargs.items() if k not in non_writer_args
         }
         close_on_exit = False
         return_dest_value = False
```

### Comparing `littletable-2.2.4/setup.py` & `littletable-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `littletable-2.2.4/unit_tests.py` & `littletable-2.2.5/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -797,6431 +797,6576 @@
 000031c0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
 000031d0: 2e61 7373 6572 7452 6169 7365 7328 4b65  .assertRaises(Ke
 000031e0: 7945 7272 6f72 293a 0a20 2020 2020 2020  yError):.       
 000031f0: 2020 2020 2074 6162 6c65 2e69 6e73 6572       table.inser
 00003200: 7428 7365 6c66 2e6d 616b 655f 6461 7461  t(self.make_data
 00003210: 5f6f 626a 6563 7428 4e6f 6e65 2c20 312c  _object(None, 1,
 00003220: 2030 2929 0a0a 2020 2020 2020 2020 7461   0))..        ta
-00003230: 626c 652e 6465 6c65 7465 5f69 6e64 6578  ble.delete_index
-00003240: 2827 6127 290a 2020 2020 2020 2020 7461  ('a').        ta
-00003250: 626c 652e 696e 7365 7274 2873 656c 662e  ble.insert(self.
-00003260: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00003270: 2834 2c20 312c 2030 2929 0a0a 2020 2020  (4, 1, 0))..    
-00003280: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00003290: 7365 7274 5261 6973 6573 284b 6579 4572  sertRaises(KeyEr
-000032a0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-000032b0: 2020 7461 626c 652e 6372 6561 7465 5f69    table.create_i
-000032c0: 6e64 6578 2827 6127 2c20 756e 6971 7565  ndex('a', unique
-000032d0: 3d54 7275 6529 0a0a 2020 2020 6465 6620  =True)..    def 
-000032e0: 7465 7374 5f69 6e73 6572 745f 6469 6374  test_insert_dict
-000032f0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00003300: 2074 6162 6c65 203d 206c 742e 5461 626c   table = lt.Tabl
-00003310: 6528 290a 2020 2020 2020 2020 7461 626c  e().        tabl
-00003320: 652e 696e 7365 7274 287b 2261 223a 2031  e.insert({"a": 1
-00003330: 2c20 2262 223a 2032 2c20 2263 223a 2033  , "b": 2, "c": 3
-00003340: 7d29 0a20 2020 2020 2020 2074 6162 6c65  }).        table
-00003350: 2e69 6e73 6572 7428 7b22 6122 3a20 342c  .insert({"a": 4,
-00003360: 2022 6222 3a20 352c 2022 6322 3a20 367d   "b": 5, "c": 6}
-00003370: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-00003380: 6372 6561 7465 5f69 6e64 6578 2827 6127  create_index('a'
-00003390: 2c20 756e 6971 7565 3d54 7275 6529 0a20  , unique=True). 
-000033a0: 2020 2020 2020 2072 6563 302c 2072 6563         rec0, rec
-000033b0: 3120 3d20 7461 626c 650a 2020 2020 2020  1 = table.      
-000033c0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000033d0: 616c 287b 2261 223a 2031 2c20 2262 223a  al({"a": 1, "b":
-000033e0: 2032 2c20 2263 223a 2033 7d2c 2076 6172   2, "c": 3}, var
-000033f0: 7328 7265 6330 2929 0a20 2020 2020 2020  s(rec0)).       
-00003400: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00003410: 6c28 6c74 2e64 6566 6175 6c74 5f72 6f77  l(lt.default_row
-00003420: 5f63 6c61 7373 2c20 7479 7065 2872 6563  _class, type(rec
-00003430: 3029 290a 2020 2020 2020 2020 7365 6c66  0)).        self
-00003440: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
-00003450: 6765 7461 7474 7228 7265 6330 2c20 2261  getattr(rec0, "a
-00003460: 2229 290a 0a20 2020 2020 2020 2023 2069  "))..        # i
-00003470: 6e73 6572 7420 6120 6e65 7374 6564 2064  nsert a nested d
-00003480: 6963 740a 2020 2020 2020 2020 7461 626c  ict.        tabl
-00003490: 652e 636c 6561 7228 290a 2020 2020 2020  e.clear().      
-000034a0: 2020 7461 626c 652e 696e 7365 7274 287b    table.insert({
-000034b0: 2261 223a 2031 2c20 2262 223a 2032 2c20  "a": 1, "b": 2, 
-000034c0: 2263 223a 2033 2c20 2264 223a 207b 2278  "c": 3, "d": {"x
-000034d0: 223a 2031 3030 2c20 2279 223a 2032 3030  ": 100, "y": 200
-000034e0: 7d7d 290a 2020 2020 2020 2020 7461 626c  }}).        tabl
-000034f0: 652e 696e 7365 7274 287b 2261 223a 2034  e.insert({"a": 4
-00003500: 2c20 2262 223a 2035 2c20 2263 223a 2036  , "b": 5, "c": 6
-00003510: 2c20 2264 223a 207b 2278 223a 2031 3031  , "d": {"x": 101
-00003520: 2c20 2279 223a 2032 3031 7d7d 290a 2020  , "y": 201}}).  
-00003530: 2020 2020 2020 7265 6330 2c20 7265 6331        rec0, rec1
-00003540: 203d 2074 6162 6c65 0a20 2020 2020 2020   = table.       
-00003550: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00003560: 6c28 3130 302c 2072 6563 302e 642e 7829  l(100, rec0.d.x)
-00003570: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003580: 7365 7274 4571 7561 6c28 3130 312c 2072  sertEqual(101, r
-00003590: 6563 312e 642e 7829 0a0a 2020 2020 6465  ec1.d.x)..    de
-000035a0: 6620 7465 7374 5f77 6865 7265 5f65 7175  f test_where_equ
-000035b0: 616c 7328 7365 6c66 293a 0a20 2020 2020  als(self):.     
-000035c0: 2020 2074 6573 745f 7369 7a65 203d 2031     test_size = 1
-000035d0: 300a 2020 2020 2020 2020 7461 626c 6520  0.        table 
-000035e0: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-000035f0: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00003600: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-00003610: 7a65 290a 0a20 2020 2020 2020 2073 656c  ze)..        sel
-00003620: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00003630: 7374 5f73 697a 652a 7465 7374 5f73 697a  st_size*test_siz
-00003640: 652c 206c 656e 2874 6162 6c65 2e77 6865  e, len(table.whe
-00003650: 7265 2861 3d35 2929 290a 2020 2020 2020  re(a=5))).      
-00003660: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003670: 616c 2830 2c20 6c65 6e28 7461 626c 652e  al(0, len(table.
-00003680: 7768 6572 6528 613d 2d31 2929 290a 0a20  where(a=-1))).. 
-00003690: 2020 2064 6566 2074 6573 745f 7768 6572     def test_wher
-000036a0: 655f 6571 7561 6c73 5f6e 6f6e 6528 7365  e_equals_none(se
-000036b0: 6c66 293a 0a20 2020 2020 2020 2074 6573  lf):.        tes
-000036c0: 745f 7369 7a65 203d 2031 300a 2020 2020  t_size = 10.    
-000036d0: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
-000036e0: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
-000036f0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00003700: 742c 2074 6573 745f 7369 7a65 290a 0a20  t, test_size).. 
-00003710: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00003720: 7274 4571 7561 6c28 302c 206c 656e 2874  rtEqual(0, len(t
-00003730: 6162 6c65 2e77 6865 7265 2861 3d35 2c20  able.where(a=5, 
-00003740: 623d 7465 7374 5f73 697a 6529 2929 0a0a  b=test_size)))..
-00003750: 2020 2020 6465 6620 7465 7374 5f77 6865      def test_whe
-00003760: 7265 5f65 7175 616c 735f 7769 7468 5f69  re_equals_with_i
-00003770: 6e64 6578 2873 656c 6629 3a0a 2020 2020  ndex(self):.    
-00003780: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00003790: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-000037a0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000037b0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000037c0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-000037d0: 697a 6529 0a20 2020 2020 2020 2074 6162  ize).        tab
-000037e0: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
-000037f0: 2761 2729 0a0a 2020 2020 2020 2020 7365  'a')..        se
-00003800: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00003810: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-00003820: 7a65 2c20 6c65 6e28 7461 626c 652e 7768  ze, len(table.wh
-00003830: 6572 6528 613d 3529 2929 0a20 2020 2020  ere(a=5))).     
-00003840: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00003850: 7561 6c28 302c 206c 656e 2874 6162 6c65  ual(0, len(table
-00003860: 2e77 6865 7265 2861 3d2d 3129 2929 0a0a  .where(a=-1)))..
-00003870: 2020 2020 6465 6620 7465 7374 5f77 6865      def test_whe
-00003880: 7265 5f72 616e 6765 2873 656c 6629 3a0a  re_range(self):.
-00003890: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-000038a0: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-000038b0: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
-000038c0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-000038d0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-000038e0: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-000038f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003900: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-00003910: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
-00003920: 652e 7768 6572 6528 6c61 6d62 6461 2072  e.where(lambda r
-00003930: 6563 3a20 7265 632e 6120 3d3d 2072 6563  ec: rec.a == rec
-00003940: 2e62 2929 290a 0a20 2020 2064 6566 2074  .b)))..    def t
-00003950: 6573 745f 7768 6572 655f 636f 6d70 6172  est_where_compar
-00003960: 6174 6f72 2873 656c 6629 3a0a 2020 2020  ator(self):.    
-00003970: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00003980: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-00003990: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000039a0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000039b0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-000039c0: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
-000039d0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-000039e0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-000039f0: 7a65 2a34 2c20 6c65 6e28 7461 626c 652e  ze*4, len(table.
-00003a00: 7768 6572 6528 613d 6c74 2e54 6162 6c65  where(a=lt.Table
-00003a10: 2e6c 7428 3429 2929 290a 2020 2020 2020  .lt(4)))).      
-00003a20: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003a30: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-00003a40: 745f 7369 7a65 2a28 342b 3129 2c20 6c65  t_size*(4+1), le
-00003a50: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
-00003a60: 6c74 2e54 6162 6c65 2e6c 6528 3429 2929  lt.Table.le(4)))
-00003a70: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00003a80: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-00003a90: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
-00003aa0: 7465 7374 5f73 697a 652d 342d 3129 2c20  test_size-4-1), 
-00003ab0: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003ac0: 613d 6c74 2e54 6162 6c65 2e67 7428 3429  a=lt.Table.gt(4)
-00003ad0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00003ae0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00003af0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00003b00: 2a28 7465 7374 5f73 697a 652d 3429 2c20  *(test_size-4), 
-00003b10: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003b20: 613d 6c74 2e54 6162 6c65 2e67 6528 3429  a=lt.Table.ge(4)
-00003b30: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00003b40: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00003b50: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00003b60: 2a28 7465 7374 5f73 697a 652d 3129 2c20  *(test_size-1), 
-00003b70: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003b80: 613d 6c74 2e54 6162 6c65 2e6e 6528 3429  a=lt.Table.ne(4)
-00003b90: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00003ba0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00003bb0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00003bc0: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00003bd0: 6528 613d 6c74 2e54 6162 6c65 2e65 7128  e(a=lt.Table.eq(
-00003be0: 3429 2929 290a 2020 2020 2020 2020 7365  4)))).        se
-00003bf0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00003c00: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
-00003c10: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
-00003c20: 6162 6c65 2e65 7128 3429 2c20 623d 6c74  able.eq(4), b=lt
-00003c30: 2e54 6162 6c65 2e65 7128 3429 2929 290a  .Table.eq(4)))).
-00003c40: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003c50: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00003c60: 7a65 2a74 6573 745f 7369 7a65 2a34 2c20  ze*test_size*4, 
-00003c70: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003c80: 613d 6c74 2e54 6162 6c65 2e62 6574 7765  a=lt.Table.betwe
-00003c90: 656e 2833 2c20 3829 2929 290a 2020 2020  en(3, 8)))).    
-00003ca0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003cb0: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
-00003cc0: 6573 745f 7369 7a65 2a34 2c20 6c65 6e28  est_size*4, len(
-00003cd0: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003ce0: 2e54 6162 6c65 2e77 6974 6869 6e28 322c  .Table.within(2,
-00003cf0: 2035 2929 2929 0a20 2020 2020 2020 2073   5)))).        s
-00003d00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00003d10: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
-00003d20: 697a 652a 332c 206c 656e 2874 6162 6c65  ize*3, len(table
-00003d30: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003d40: 652e 696e 5f72 616e 6765 2832 2c20 3529  e.in_range(2, 5)
-00003d50: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00003d60: 2e61 7373 6572 7445 7175 616c 2830 2c20  .assertEqual(0, 
-00003d70: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003d80: 613d 6c74 2e54 6162 6c65 2e62 6574 7765  a=lt.Table.betwe
-00003d90: 656e 2833 2c20 3329 2929 290a 2020 2020  en(3, 3)))).    
-00003da0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003db0: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
-00003dc0: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
-00003dd0: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
-00003de0: 6162 6c65 2e77 6974 6869 6e28 332c 2033  able.within(3, 3
-00003df0: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
-00003e00: 662e 6173 7365 7274 4571 7561 6c28 302c  f.assertEqual(0,
-00003e10: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00003e20: 2861 3d6c 742e 5461 626c 652e 696e 5f72  (a=lt.Table.in_r
-00003e30: 616e 6765 2833 2c20 3329 2929 290a 2020  ange(3, 3)))).  
-00003e40: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00003e50: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-00003e60: 2a74 6573 745f 7369 7a65 2a34 2c20 6c65  *test_size*4, le
-00003e70: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
-00003e80: 6c74 2e54 6162 6c65 2e69 735f 696e 285b  lt.Table.is_in([
-00003e90: 322c 2034 2c20 362c 2038 5d29 2929 290a  2, 4, 6, 8])))).
-00003ea0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003eb0: 6572 7445 7175 616c 2830 2c20 6c65 6e28  ertEqual(0, len(
-00003ec0: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
-00003ed0: 2e54 6162 6c65 2e69 735f 696e 285b 5d29  .Table.is_in([])
-00003ee0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-00003ef0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00003f00: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00003f10: 2a28 7465 7374 5f73 697a 652d 3429 2c20  *(test_size-4), 
-00003f20: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
-00003f30: 613d 6c74 2e54 6162 6c65 2e6e 6f74 5f69  a=lt.Table.not_i
-00003f40: 6e28 5b32 2c20 342c 2036 2c20 385d 2929  n([2, 4, 6, 8]))
-00003f50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00003f60: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-00003f70: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-00003f80: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
-00003f90: 6162 6c65 2e77 6865 7265 2861 3d6c 742e  able.where(a=lt.
-00003fa0: 5461 626c 652e 6e6f 745f 696e 285b 5d29  Table.not_in([])
-00003fb0: 2929 290a 0a20 2020 2020 2020 2023 2061  )))..        # a
-00003fc0: 6464 2061 2072 6563 6f72 6420 636f 6e74  dd a record cont
-00003fd0: 6169 6e69 6e67 2061 204e 6f6e 6520 7661  aining a None va
-00003fe0: 6c75 6520 746f 2074 6573 7420 6973 5f6e  lue to test is_n
-00003ff0: 6f6e 6520 616e 6420 6973 5f6e 6f74 5f6e  one and is_not_n
-00004000: 6f6e 6520 636f 6d70 6172 6174 6f72 730a  one comparators.
-00004010: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
-00004020: 7365 7274 2873 656c 662e 6d61 6b65 5f64  sert(self.make_d
-00004030: 6174 615f 6f62 6a65 6374 2861 3d31 2c20  ata_object(a=1, 
-00004040: 623d 322c 2063 3d4e 6f6e 6529 290a 2020  b=2, c=None)).  
-00004050: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00004060: 7445 7175 616c 2831 2c20 6c65 6e28 7461  tEqual(1, len(ta
-00004070: 626c 652e 7768 6572 6528 633d 6c74 2e54  ble.where(c=lt.T
-00004080: 6162 6c65 2e69 735f 6e6f 6e65 2829 2929  able.is_none()))
-00004090: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000040a0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-000040b0: 7369 7a65 2a74 6573 745f 7369 7a65 2a74  size*test_size*t
-000040c0: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
-000040d0: 626c 652e 7768 6572 6528 633d 6c74 2e54  ble.where(c=lt.T
-000040e0: 6162 6c65 2e69 735f 6e6f 745f 6e6f 6e65  able.is_not_none
-000040f0: 2829 2929 290a 0a20 2020 2020 2020 2023  ())))..        #
-00004100: 2061 6464 2061 2072 6563 6f72 6420 636f   add a record co
-00004110: 6e74 6169 6e69 6e67 2061 206d 6973 7369  ntaining a missi
-00004120: 6e67 2076 616c 7565 2074 6f20 7465 7374  ng value to test
-00004130: 2069 735f 6e75 6c6c 2061 6e64 2069 735f   is_null and is_
-00004140: 6e6f 745f 6e75 6c6c 2063 6f6d 7061 7261  not_null compara
-00004150: 746f 7273 0a20 2020 2020 2020 2074 6162  tors.        tab
-00004160: 6c65 2e69 6e73 6572 7428 7365 6c66 2e6d  le.insert(self.m
-00004170: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00004180: 613d 312c 2062 3d32 2c20 633d 2222 2929  a=1, b=2, c=""))
-00004190: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000041a0: 7365 7274 4571 7561 6c28 322c 206c 656e  sertEqual(2, len
-000041b0: 2874 6162 6c65 2e77 6865 7265 2863 3d6c  (table.where(c=l
-000041c0: 742e 5461 626c 652e 6973 5f6e 756c 6c28  t.Table.is_null(
-000041d0: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
-000041e0: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-000041f0: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
-00004200: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
-00004210: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00004220: 2863 3d6c 742e 5461 626c 652e 6973 5f6e  (c=lt.Table.is_n
-00004230: 6f74 5f6e 756c 6c28 2929 2929 0a0a 2020  ot_null())))..  
-00004240: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00004250: 2020 2020 2020 2074 6162 6c65 2e69 6e73         table.ins
-00004260: 6572 7428 7365 6c66 2e6d 616b 655f 6461  ert(self.make_da
-00004270: 7461 5f6f 626a 6563 7428 613d 312c 2062  ta_object(a=1, b
-00004280: 3d32 2929 0a20 2020 2020 2020 2065 7863  =2)).        exc
-00004290: 6570 7420 5479 7065 4572 726f 723a 0a20  ept TypeError:. 
-000042a0: 2020 2020 2020 2020 2020 2023 206e 6f74             # not
-000042b0: 2061 6c6c 2064 6174 6120 6f62 6a65 6374   all data object
-000042c0: 2074 7970 6573 2062 6569 6e67 2074 6573   types being tes
-000042d0: 7465 6420 7375 7070 6f72 7420 6d69 7373  ted support miss
-000042e0: 696e 6720 6174 7472 6962 7574 6573 0a20  ing attributes. 
-000042f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00004300: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00004310: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00004320: 7373 6572 7445 7175 616c 2833 2c20 6c65  ssertEqual(3, le
-00004330: 6e28 7461 626c 652e 7768 6572 6528 633d  n(table.where(c=
-00004340: 6c74 2e54 6162 6c65 2e69 735f 6e75 6c6c  lt.Table.is_null
-00004350: 2829 2929 290a 2020 2020 2020 2020 2020  ()))).          
-00004360: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00004370: 616c 2874 6573 745f 7369 7a65 202a 2074  al(test_size * t
-00004380: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-00004390: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
-000043a0: 7768 6572 6528 633d 6c74 2e54 6162 6c65  where(c=lt.Table
-000043b0: 2e69 735f 6e6f 745f 6e75 6c6c 2829 2929  .is_not_null()))
-000043c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000043d0: 7768 6572 655f 7374 725f 636f 6d70 6172  where_str_compar
-000043e0: 6174 6f72 2873 656c 6629 3a0a 2020 2020  ator(self):.    
-000043f0: 2020 2020 756e 6963 6f64 655f 6e75 6d62      unicode_numb
-00004400: 6572 7320 3d20 6c74 2e54 6162 6c65 2829  ers = lt.Table()
-00004410: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-00004420: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-00004430: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-00004440: 652c 636f 6465 5f76 616c 7565 2c6e 756d  e,code_value,num
-00004450: 6572 6963 5f76 616c 7565 0a20 2020 2020  eric_value.     
-00004460: 2020 2020 2020 2052 4f4d 414e 204e 554d         ROMAN NUM
-00004470: 4552 414c 204f 4e45 2c38 3534 342c 310a  ERAL ONE,8544,1.
-00004480: 2020 2020 2020 2020 2020 2020 524f 4d41              ROMA
-00004490: 4e20 4e55 4d45 5241 4c20 5457 4f2c 3835  N NUMERAL TWO,85
-000044a0: 3435 2c32 0a20 2020 2020 2020 2020 2020  45,2.           
-000044b0: 2052 4f4d 414e 204e 554d 4552 414c 2054   ROMAN NUMERAL T
-000044c0: 4852 4545 2c38 3534 362c 330a 2020 2020  HREE,8546,3.    
-000044d0: 2020 2020 2020 2020 524f 4d41 4e20 4e55          ROMAN NU
-000044e0: 4d45 5241 4c20 464f 5552 2c38 3534 372c  MERAL FOUR,8547,
-000044f0: 340a 2020 2020 2020 2020 2020 2020 524f  4.            RO
-00004500: 4d41 4e20 4e55 4d45 5241 4c20 4649 5645  MAN NUMERAL FIVE
-00004510: 2c38 3534 382c 350a 2020 2020 2020 2020  ,8548,5.        
-00004520: 2020 2020 524f 4d41 4e20 4e55 4d45 5241      ROMAN NUMERA
-00004530: 4c20 5349 582c 3835 3439 2c36 0a20 2020  L SIX,8549,6.   
-00004540: 2020 2020 2020 2020 2052 4f4d 414e 204e           ROMAN N
-00004550: 554d 4552 414c 2053 4556 454e 2c38 3535  UMERAL SEVEN,855
-00004560: 302c 370a 2020 2020 2020 2020 2020 2020  0,7.            
-00004570: 524f 4d41 4e20 4e55 4d45 5241 4c20 4549  ROMAN NUMERAL EI
-00004580: 4748 542c 3835 3531 2c38 0a20 2020 2020  GHT,8551,8.     
-00004590: 2020 2020 2020 2052 4f4d 414e 204e 554d         ROMAN NUM
-000045a0: 4552 414c 204e 494e 452c 3835 3532 2c39  ERAL NINE,8552,9
-000045b0: 0a20 2020 2020 2020 2020 2020 2052 4f4d  .            ROM
-000045c0: 414e 204e 554d 4552 414c 2054 454e 2c38  AN NUMERAL TEN,8
-000045d0: 3535 332c 3130 0a20 2020 2020 2020 2020  553,10.         
-000045e0: 2020 2053 5550 4552 5343 5249 5054 2054     SUPERSCRIPT T
-000045f0: 574f 2c31 3738 2c32 0a20 2020 2020 2020  WO,178,2.       
-00004600: 2020 2020 2053 5550 4552 5343 5249 5054       SUPERSCRIPT
-00004610: 2054 4852 4545 2c31 3739 2c33 0a20 2020   THREE,179,3.   
-00004620: 2020 2020 2020 2020 2053 5550 4552 5343           SUPERSC
-00004630: 5249 5054 204f 4e45 2c31 3835 2c31 0a20  RIPT ONE,185,1. 
-00004640: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
-00004650: 5343 5249 5054 205a 4552 4f2c 3833 3034  SCRIPT ZERO,8304
-00004660: 2c30 0a20 2020 2020 2020 2020 2020 2053  ,0.            S
-00004670: 5550 4552 5343 5249 5054 2046 4f55 522c  UPERSCRIPT FOUR,
-00004680: 3833 3038 2c34 0a20 2020 2020 2020 2020  8308,4.         
-00004690: 2020 2053 5550 4552 5343 5249 5054 2046     SUPERSCRIPT F
-000046a0: 4956 452c 3833 3039 2c35 0a20 2020 2020  IVE,8309,5.     
-000046b0: 2020 2020 2020 2053 5550 4552 5343 5249         SUPERSCRI
-000046c0: 5054 2053 4958 2c38 3331 302c 360a 2020  PT SIX,8310,6.  
-000046d0: 2020 2020 2020 2020 2020 5355 5045 5253            SUPERS
-000046e0: 4352 4950 5420 5345 5645 4e2c 3833 3131  CRIPT SEVEN,8311
-000046f0: 2c37 0a20 2020 2020 2020 2020 2020 2053  ,7.            S
-00004700: 5550 4552 5343 5249 5054 2045 4947 4854  UPERSCRIPT EIGHT
-00004710: 2c38 3331 322c 380a 2020 2020 2020 2020  ,8312,8.        
-00004720: 2020 2020 5355 5045 5253 4352 4950 5420      SUPERSCRIPT 
-00004730: 4e49 4e45 2c38 3331 332c 390a 2020 2020  NINE,8313,9.    
-00004740: 2020 2020 2020 2020 4349 5243 4c45 4420          CIRCLED 
-00004750: 4449 4749 5420 4f4e 452c 3933 3132 2c31  DIGIT ONE,9312,1
-00004760: 0a20 2020 2020 2020 2020 2020 2043 4952  .            CIR
-00004770: 434c 4544 2044 4947 4954 2054 574f 2c39  CLED DIGIT TWO,9
-00004780: 3331 332c 320a 2020 2020 2020 2020 2020  313,2.          
-00004790: 2020 4349 5243 4c45 4420 4449 4749 5420    CIRCLED DIGIT 
-000047a0: 5448 5245 452c 3933 3134 2c33 0a20 2020  THREE,9314,3.   
-000047b0: 2020 2020 2020 2020 2043 4952 434c 4544           CIRCLED
-000047c0: 2044 4947 4954 2046 4f55 522c 3933 3135   DIGIT FOUR,9315
-000047d0: 2c34 0a20 2020 2020 2020 2020 2020 2043  ,4.            C
-000047e0: 4952 434c 4544 2044 4947 4954 2046 4956  IRCLED DIGIT FIV
-000047f0: 452c 3933 3136 2c35 0a20 2020 2020 2020  E,9316,5.       
-00004800: 2020 2020 2043 4952 434c 4544 2044 4947       CIRCLED DIG
-00004810: 4954 2053 4958 2c39 3331 372c 360a 2020  IT SIX,9317,6.  
-00004820: 2020 2020 2020 2020 2020 4349 5243 4c45            CIRCLE
-00004830: 4420 4449 4749 5420 5345 5645 4e2c 3933  D DIGIT SEVEN,93
-00004840: 3138 2c37 0a20 2020 2020 2020 2020 2020  18,7.           
-00004850: 2043 4952 434c 4544 2044 4947 4954 2045   CIRCLED DIGIT E
-00004860: 4947 4854 2c39 3331 392c 380a 2020 2020  IGHT,9319,8.    
-00004870: 2020 2020 2020 2020 4349 5243 4c45 4420          CIRCLED 
-00004880: 4449 4749 5420 4e49 4e45 2c39 3332 302c  DIGIT NINE,9320,
-00004890: 390a 2020 2020 2020 2020 2020 2020 4349  9.            CI
-000048a0: 5243 4c45 4420 4449 4749 5420 5a45 524f  RCLED DIGIT ZERO
-000048b0: 2c39 3435 302c 300a 2020 2020 2020 2020  ,9450,0.        
-000048c0: 2020 2020 2222 2229 290a 0a20 2020 2020      """))..     
-000048d0: 2020 206f 6e65 7320 3d20 756e 6963 6f64     ones = unicod
-000048e0: 655f 6e75 6d62 6572 732e 7768 6572 6528  e_numbers.where(
-000048f0: 6e61 6d65 3d6c 742e 5461 626c 652e 656e  name=lt.Table.en
-00004900: 6473 7769 7468 2822 4f4e 4522 2929 0a20  dswith("ONE")). 
-00004910: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00004920: 7274 4571 7561 6c28 332c 206c 656e 286f  rtEqual(3, len(o
-00004930: 6e65 7329 290a 0a20 2020 2020 2020 2073  nes))..        s
-00004940: 7570 6572 7320 3d20 756e 6963 6f64 655f  upers = unicode_
-00004950: 6e75 6d62 6572 732e 7768 6572 6528 6e61  numbers.where(na
-00004960: 6d65 3d6c 742e 5461 626c 652e 7374 6172  me=lt.Table.star
-00004970: 7473 7769 7468 2822 5355 5045 5253 4352  tswith("SUPERSCR
-00004980: 4950 5422 2929 0a20 2020 2020 2020 2073  IPT")).        s
-00004990: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000049a0: 3130 2c20 6c65 6e28 7375 7065 7273 2929  10, len(supers))
-000049b0: 0a0a 2020 2020 2020 2020 2320 696d 706f  ..        # impo
-000049c0: 7274 2072 650a 2020 2020 2020 2020 2320  rt re.        # 
-000049d0: 7365 7665 6e73 203d 2075 6e69 636f 6465  sevens = unicode
-000049e0: 5f6e 756d 6265 7273 2e77 6865 7265 286c  _numbers.where(l
-000049f0: 616d 6264 6120 7265 633a 2072 652e 636f  ambda rec: re.co
-00004a00: 6d70 696c 6528 7222 2e2a 5345 5645 4e24  mpile(r".*SEVEN$
-00004a10: 2229 2e6d 6174 6368 2872 6563 2e6e 616d  ").match(rec.nam
-00004a20: 6529 290a 0a20 2020 2020 2020 2073 6576  e))..        sev
-00004a30: 656e 7320 3d20 756e 6963 6f64 655f 6e75  ens = unicode_nu
-00004a40: 6d62 6572 732e 7768 6572 6528 6e61 6d65  mbers.where(name
-00004a50: 3d6c 742e 5461 626c 652e 7265 5f6d 6174  =lt.Table.re_mat
-00004a60: 6368 2872 222e 2a53 4556 454e 2422 2929  ch(r".*SEVEN$"))
-00004a70: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00004a80: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
-00004a90: 2873 6576 656e 7329 290a 0a20 2020 2020  (sevens))..     
-00004aa0: 2020 2023 206d 616b 6520 6e61 6d65 7320     # make names 
-00004ab0: 616c 6c20 7469 746c 6520 6361 7365 0a20  all title case. 
-00004ac0: 2020 2020 2020 2075 6e69 636f 6465 5f6e         unicode_n
-00004ad0: 756d 6265 7273 2e61 6464 5f66 6965 6c64  umbers.add_field
-00004ae0: 2822 6e61 6d65 222c 206c 616d 6264 6120  ("name", lambda 
-00004af0: 7265 633a 2072 6563 2e6e 616d 652e 7469  rec: rec.name.ti
-00004b00: 746c 6528 2929 0a20 2020 2020 2020 2023  tle()).        #
-00004b10: 2075 7365 2072 6567 6578 2077 6974 6820   use regex with 
-00004b20: 7265 2066 6c61 670a 2020 2020 2020 2020  re flag.        
-00004b30: 696d 706f 7274 2072 650a 2020 2020 2020  import re.      
-00004b40: 2020 6369 7263 6c65 6420 3d20 756e 6963    circled = unic
-00004b50: 6f64 655f 6e75 6d62 6572 732e 7768 6572  ode_numbers.wher
-00004b60: 6528 6e61 6d65 3d6c 742e 5461 626c 652e  e(name=lt.Table.
-00004b70: 7265 5f6d 6174 6368 2872 2263 6972 636c  re_match(r"circl
-00004b80: 6564 222c 2066 6c61 6773 3d72 652e 4929  ed", flags=re.I)
-00004b90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00004ba0: 7373 6572 7445 7175 616c 2831 302c 206c  ssertEqual(10, l
-00004bb0: 656e 2863 6972 636c 6564 2929 0a0a 2020  en(circled))..  
-00004bc0: 2020 6465 6620 7465 7374 5f77 6865 7265    def test_where
-00004bd0: 5f61 7474 725f 6675 6e63 7469 6f6e 2873  _attr_function(s
-00004be0: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
-00004bf0: 7374 5f73 697a 6520 3d20 380a 2020 2020  st_size = 8.    
-00004c00: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
-00004c10: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
-00004c20: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00004c30: 742c 2074 6573 745f 7369 7a65 290a 0a20  t, test_size).. 
-00004c40: 2020 2020 2020 2064 6566 2069 735f 6f64         def is_od
-00004c50: 6428 7829 3a0a 2020 2020 2020 2020 2020  d(x):.          
-00004c60: 2020 7265 7475 726e 2062 6f6f 6c28 7820    return bool(x 
-00004c70: 2520 3229 0a0a 2020 2020 2020 2020 7365  % 2)..        se
-00004c80: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00004c90: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
-00004ca0: 7a65 2a74 6573 745f 7369 7a65 2f2f 322c  ze*test_size//2,
-00004cb0: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00004cc0: 2861 3d69 735f 6f64 6429 2929 0a0a 2020  (a=is_odd)))..  
-00004cd0: 2020 6465 6620 7465 7374 5f67 6574 5f73    def test_get_s
-00004ce0: 6c69 6365 2873 656c 6629 3a0a 2020 2020  lice(self):.    
-00004cf0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00004d00: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-00004d10: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00004d20: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-00004d30: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00004d40: 697a 6529 0a0a 2020 2020 2020 2020 7375  ize)..        su
-00004d50: 6274 6162 6c65 203d 2074 6162 6c65 5b30  btable = table[0
-00004d60: 3a3a 7465 7374 5f73 697a 655d 0a20 2020  ::test_size].   
-00004d70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00004d80: 4571 7561 6c28 7465 7374 5f73 697a 6520  Equal(test_size 
-00004d90: 2a20 7465 7374 5f73 697a 652c 206c 656e  * test_size, len
-00004da0: 2873 7562 7461 626c 6529 290a 0a20 2020  (subtable))..   
-00004db0: 2064 6566 2074 6573 745f 696e 6465 7869   def test_indexi
-00004dc0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
-00004dd0: 2020 6368 6172 7320 3d20 2241 4243 4445    chars = "ABCDE
-00004de0: 4647 4849 4a4b 4c4d 4e4f 5051 5253 5455  FGHIJKLMNOPQRSTU
-00004df0: 5657 5859 5a22 0a20 2020 2020 2020 206d  VWXYZ".        m
-00004e00: 616b 655f 7265 6320 3d20 6c61 6d62 6461  ake_rec = lambda
-00004e10: 2061 612c 2062 622c 2063 633a 2073 656c   aa, bb, cc: sel
-00004e20: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-00004e30: 6374 2863 6861 7273 5b61 615d 2c20 6368  ct(chars[aa], ch
-00004e40: 6172 735b 6262 5d2c 2063 6861 7273 5b63  ars[bb], chars[c
-00004e50: 635d 290a 2020 2020 2020 2020 7465 7374  c]).        test
-00004e60: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
-00004e70: 2020 2074 6162 6c65 203d 206d 616b 655f     table = make_
-00004e80: 7465 7374 5f74 6162 6c65 286d 616b 655f  test_table(make_
-00004e90: 7265 632c 2074 6573 745f 7369 7a65 290a  rec, test_size).
-00004ea0: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
-00004eb0: 6561 7465 5f69 6e64 6578 2827 6127 290a  eate_index('a').
-00004ec0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00004ed0: 7365 7274 5472 7565 2827 4127 2069 6e20  sertTrue('A' in 
-00004ee0: 7461 626c 652e 6279 2e61 290a 2020 2020  table.by.a).    
-00004ef0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00004f00: 7275 6528 2741 4127 206e 6f74 2069 6e20  rue('AA' not in 
-00004f10: 7461 626c 652e 6279 2e61 290a 2020 2020  table.by.a).    
-00004f20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00004f30: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
-00004f40: 2074 6573 745f 7369 7a65 2c20 6c65 6e28   test_size, len(
-00004f50: 7461 626c 652e 6279 2e61 5b27 4227 5d29  table.by.a['B'])
-00004f60: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00004f70: 7373 6572 7454 7275 6528 6973 696e 7374  ssertTrue(isinst
-00004f80: 616e 6365 2874 6162 6c65 2e62 792e 615b  ance(table.by.a[
-00004f90: 2742 275d 2c20 6c74 2e54 6162 6c65 2929  'B'], lt.Table))
-00004fa0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00004fb0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00004fc0: 4174 7472 6962 7574 6545 7272 6f72 293a  AttributeError):
-00004fd0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00004fe0: 6c65 2e62 792e 7a0a 0a20 2020 2020 2020  le.by.z..       
-00004ff0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00005000: 6c28 7465 7374 5f73 697a 652c 206c 656e  l(test_size, len
-00005010: 2874 6162 6c65 2e62 792e 612e 6b65 7973  (table.by.a.keys
-00005020: 2829 2929 0a0a 2020 2020 6465 6620 7465  ()))..    def te
-00005030: 7374 5f75 6e69 7175 655f 696e 6465 7869  st_unique_indexi
-00005040: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
-00005050: 2020 6368 6172 7320 3d20 2241 4243 4445    chars = "ABCDE
-00005060: 4647 4849 4a4b 4c4d 4e4f 5051 5253 5455  FGHIJKLMNOPQRSTU
-00005070: 5657 5859 5a22 0a20 2020 2020 2020 206d  VWXYZ".        m
-00005080: 616b 655f 756e 6971 7565 5f6b 6579 203d  ake_unique_key =
-00005090: 206c 616d 6264 6120 2a61 7267 733a 2027   lambda *args: '
-000050a0: 272e 6a6f 696e 2863 6861 7273 5b61 7267  '.join(chars[arg
-000050b0: 5d20 666f 7220 6172 6720 696e 2061 7267  ] for arg in arg
-000050c0: 7329 0a20 2020 2020 2020 206d 616b 655f  s).        make_
-000050d0: 7265 6320 3d20 6c61 6d62 6461 2061 612c  rec = lambda aa,
-000050e0: 2062 622c 2063 633a 2073 656c 662e 6d61   bb, cc: self.ma
-000050f0: 6b65 5f64 6174 615f 6f62 6a65 6374 286d  ke_data_object(m
-00005100: 616b 655f 756e 6971 7565 5f6b 6579 2861  ake_unique_key(a
-00005110: 612c 2062 622c 2063 6329 2c20 6368 6172  a, bb, cc), char
-00005120: 735b 6262 5d2c 2063 6861 7273 5b63 635d  s[bb], chars[cc]
-00005130: 290a 2020 2020 2020 2020 7465 7374 5f73  ).        test_s
-00005140: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
-00005150: 2074 6162 6c65 203d 206d 616b 655f 7465   table = make_te
-00005160: 7374 5f74 6162 6c65 286d 616b 655f 7265  st_table(make_re
-00005170: 632c 2074 6573 745f 7369 7a65 2928 2254  c, test_size)("T
-00005180: 6162 6c65 5f31 2229 0a20 2020 2020 2020  able_1").       
-00005190: 2074 6162 6c65 2e63 7265 6174 655f 696e   table.create_in
-000051a0: 6465 7828 2761 272c 2075 6e69 7175 653d  dex('a', unique=
-000051b0: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
-000051c0: 635f 7479 7065 203d 2074 7970 6528 7365  c_type = type(se
-000051d0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000051e0: 6563 7428 302c 2030 2c20 3029 290a 0a20  ect(0, 0, 0)).. 
-000051f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00005200: 7274 5472 7565 2827 4141 4127 2069 6e20  rtTrue('AAA' in 
-00005210: 7461 626c 652e 6279 2e61 290a 2020 2020  table.by.a).    
-00005220: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00005230: 7275 6528 2741 4127 206e 6f74 2069 6e20  rue('AA' not in 
-00005240: 7461 626c 652e 6279 2e61 290a 2020 2020  table.by.a).    
-00005250: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00005260: 7275 6528 6973 696e 7374 616e 6365 2874  rue(isinstance(t
-00005270: 6162 6c65 2e62 792e 615b 2742 4141 275d  able.by.a['BAA']
-00005280: 2c20 7265 635f 7479 7065 2929 0a20 2020  , rec_type)).   
-00005290: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-000052a0: 7373 6572 7452 6169 7365 7328 4b65 7945  ssertRaises(KeyE
-000052b0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-000052c0: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
-000052d0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-000052e0: 626a 6563 7428 4e6f 6e65 2c20 4e6f 6e65  bject(None, None
-000052f0: 2c20 4e6f 6e65 2929 0a0a 2020 2020 2020  , None))..      
-00005300: 2020 2320 6372 6561 7465 2064 7570 6c69    # create dupli
-00005310: 6361 7465 2069 6e64 6578 0a20 2020 2020  cate index.     
-00005320: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-00005330: 6572 7452 6169 7365 7328 5661 6c75 6545  ertRaises(ValueE
-00005340: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-00005350: 2020 2074 6162 6c65 2e63 7265 6174 655f     table.create_
-00005360: 696e 6465 7828 2761 272c 2075 6e69 7175  index('a', uniqu
-00005370: 653d 5472 7565 2c20 6163 6365 7074 5f6e  e=True, accept_n
-00005380: 6f6e 653d 5472 7565 290a 0a20 2020 2020  one=True)..     
-00005390: 2020 2023 2063 7265 6174 6520 756e 6971     # create uniq
-000053a0: 7565 2069 6e64 6578 2074 6861 7420 616c  ue index that al
-000053b0: 6c6f 7773 204e 6f6e 6520 7661 6c75 6573  lows None values
-000053c0: 0a20 2020 2020 2020 2074 6162 6c65 2e64  .        table.d
-000053d0: 656c 6574 655f 696e 6465 7828 2761 2729  elete_index('a')
-000053e0: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-000053f0: 7265 6174 655f 696e 6465 7828 2761 272c  reate_index('a',
-00005400: 2075 6e69 7175 653d 5472 7565 2c20 6163   unique=True, ac
-00005410: 6365 7074 5f6e 6f6e 653d 5472 7565 290a  cept_none=True).
-00005420: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
-00005430: 7365 7274 2873 656c 662e 6d61 6b65 5f64  sert(self.make_d
-00005440: 6174 615f 6f62 6a65 6374 284e 6f6e 652c  ata_object(None,
-00005450: 204e 6f6e 652c 2027 4127 2929 0a0a 2020   None, 'A'))..  
-00005460: 2020 2020 2020 7374 725f 6e6f 6e65 5f63        str_none_c
-00005470: 6f6d 7061 7265 203d 206c 616d 6264 6120  ompare = lambda 
-00005480: 783a 2078 2069 6620 6973 696e 7374 616e  x: x if isinstan
-00005490: 6365 2878 2c20 7374 7229 2065 6c73 6520  ce(x, str) else 
-000054a0: 6368 7228 3235 3529 2a31 3030 0a20 2020  chr(255)*100.   
-000054b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000054c0: 4571 7561 6c28 736f 7274 6564 2874 6162  Equal(sorted(tab
-000054d0: 6c65 2e62 792e 612e 6b65 7973 2829 2c20  le.by.a.keys(), 
-000054e0: 6b65 793d 7374 725f 6e6f 6e65 5f63 6f6d  key=str_none_com
-000054f0: 7061 7265 292c 0a20 2020 2020 2020 2020  pare),.         
-00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005510: 736f 7274 6564 2874 6162 6c65 2e61 6c6c  sorted(table.all
-00005520: 2e61 2c20 6b65 793d 7374 725f 6e6f 6e65  .a, key=str_none
-00005530: 5f63 6f6d 7061 7265 2929 0a0a 2020 2020  _compare))..    
-00005540: 2020 2020 2320 6e6f 7720 6472 6f70 2069      # now drop i
-00005550: 6e64 6578 2061 6e64 2072 6563 7265 6174  ndex and recreat
-00005560: 6520 6e6f 7420 7065 726d 6974 7469 6e67  e not permitting
-00005570: 204e 6f6e 652c 2073 686f 756c 6420 7261   None, should ra
-00005580: 6973 6520 6578 6365 7074 696f 6e0a 2020  ise exception.  
-00005590: 2020 2020 2020 7461 626c 652e 6465 6c65        table.dele
-000055a0: 7465 5f69 6e64 6578 2827 6127 290a 2020  te_index('a').  
-000055b0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000055c0: 6173 7365 7274 5261 6973 6573 284b 6579  assertRaises(Key
-000055d0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-000055e0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-000055f0: 5f69 6e64 6578 2827 6127 2c20 756e 6971  _index('a', uniq
-00005600: 7565 3d54 7275 652c 2061 6363 6570 745f  ue=True, accept_
-00005610: 6e6f 6e65 3d46 616c 7365 290a 0a20 2020  none=False)..   
-00005620: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
-00005630: 655f 696e 6465 7828 2761 272c 2075 6e69  e_index('a', uni
-00005640: 7175 653d 5472 7565 2c20 6163 6365 7074  que=True, accept
-00005650: 5f6e 6f6e 653d 5472 7565 290a 2020 2020  _none=True).    
-00005660: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-00005670: 5f69 6e64 6578 2827 6327 290a 0a20 2020  _index('c')..   
-00005680: 2020 2020 2069 6d70 6f72 7420 7070 7269       import ppri
-00005690: 6e74 0a20 2020 2020 2020 2069 6e66 6f20  nt.        info 
-000056a0: 3d20 7461 626c 652e 696e 666f 2829 0a20  = table.info(). 
-000056b0: 2020 2020 2020 2070 7072 696e 742e 7070         pprint.pp
-000056c0: 7269 6e74 2869 6e66 6f29 0a20 2020 2020  rint(info).     
-000056d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000056e0: 7561 6c28 2754 6162 6c65 5f31 272c 2069  ual('Table_1', i
-000056f0: 6e66 6f5b 276e 616d 6527 5d29 0a20 2020  nfo['name']).   
-00005700: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00005710: 4571 7561 6c28 5b27 6127 2c20 2762 272c  Equal(['a', 'b',
-00005720: 2027 6327 5d2c 206c 6973 7428 736f 7274   'c'], list(sort
-00005730: 6564 2869 6e66 6f5b 2766 6965 6c64 7327  ed(info['fields'
-00005740: 5d29 2929 0a20 2020 2020 2020 2073 656c  ]))).        sel
-00005750: 662e 6173 7365 7274 4571 7561 6c28 5b28  f.assertEqual([(
-00005760: 2761 272c 2054 7275 6529 2c20 2827 6327  'a', True), ('c'
-00005770: 2c20 4661 6c73 6529 5d2c 206c 6973 7428  , False)], list(
-00005780: 736f 7274 6564 2869 6e66 6f5b 2769 6e64  sorted(info['ind
-00005790: 6578 6573 275d 2929 290a 2020 2020 2020  exes']))).      
-000057a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000057b0: 616c 2831 3030 312c 2069 6e66 6f5b 276c  al(1001, info['l
-000057c0: 656e 275d 290a 0a20 2020 2064 6566 2074  en'])..    def t
-000057d0: 6573 745f 6368 6169 6e65 645f 696e 6465  est_chained_inde
-000057e0: 7869 6e67 2873 656c 6629 3a0a 2020 2020  xing(self):.    
-000057f0: 2020 2020 6368 6172 7320 3d20 2241 4243      chars = "ABC
-00005800: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
-00005810: 5455 5657 5859 5a22 0a20 2020 2020 2020  TUVWXYZ".       
-00005820: 206d 616b 655f 7265 6320 3d20 6c61 6d62   make_rec = lamb
-00005830: 6461 2061 612c 2062 622c 2063 633a 2073  da aa, bb, cc: s
-00005840: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00005850: 6a65 6374 2863 6861 7273 5b61 6120 2520  ject(chars[aa % 
-00005860: 6c65 6e28 6368 6172 7329 5d2c 0a20 2020  len(chars)],.   
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058a0: 2020 2020 2020 2020 2063 6861 7273 5b62           chars[b
-000058b0: 6220 2520 6c65 6e28 6368 6172 7329 5d2c  b % len(chars)],
-000058c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00005900: 7273 5b63 6320 2520 6c65 6e28 6368 6172  rs[cc % len(char
-00005910: 7329 5d29 0a20 2020 2020 2020 2074 6573  s)]).        tes
-00005920: 745f 7369 7a65 203d 2031 300a 2020 2020  t_size = 10.    
-00005930: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
-00005940: 5f74 6573 745f 7461 626c 6528 6d61 6b65  _test_table(make
-00005950: 5f72 6563 2c20 7465 7374 5f73 697a 6529  _rec, test_size)
-00005960: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-00005970: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
-00005980: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-00005990: 7265 6174 655f 696e 6465 7828 2762 2729  reate_index('b')
-000059a0: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
-000059b0: 7265 6174 655f 696e 6465 7828 2763 2729  reate_index('c')
-000059c0: 0a0a 2020 2020 2020 2020 6368 6169 6e65  ..        chaine
-000059d0: 645f 7461 626c 6520 3d20 7461 626c 652e  d_table = table.
-000059e0: 6279 2e62 5b27 4127 5d2e 6279 2e63 5b27  by.b['A'].by.c['
-000059f0: 4327 5d0a 2020 2020 2020 2020 666f 7220  C'].        for 
-00005a00: 7265 6320 696e 2063 6861 696e 6564 5f74  rec in chained_t
-00005a10: 6162 6c65 3a0a 2020 2020 2020 2020 2020  able:.          
-00005a20: 2020 7072 696e 7428 7265 6329 0a0a 2020    print(rec)..  
-00005a30: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00005a40: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-00005a50: 2c20 6c65 6e28 6368 6169 6e65 645f 7461  , len(chained_ta
-00005a60: 626c 6529 290a 0a20 2020 2064 6566 2074  ble))..    def t
-00005a70: 6573 745f 7061 7273 655f 6461 7465 7469  est_parse_dateti
-00005a80: 6d65 5f74 7261 6e73 666f 726d 2873 656c  me_transform(sel
-00005a90: 6629 3a0a 2020 2020 2020 2020 696d 706f  f):.        impo
-00005aa0: 7274 2064 6174 6574 696d 650a 0a20 2020  rt datetime..   
-00005ab0: 2020 2020 2064 6174 6120 3d20 7465 7874       data = text
-00005ac0: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-00005ad0: 0a20 2020 2020 2020 2061 2c62 2c63 0a20  .        a,b,c. 
-00005ae0: 2020 2020 2020 2032 3030 312d 3031 2d30         2001-01-0
-00005af0: 3120 3030 3a33 343a 3536 2c41 2c31 3030  1 00:34:56,A,100
-00005b00: 0a20 2020 2020 2020 2032 3030 312d 3031  .        2001-01
-00005b10: 2d30 3220 3031 3a33 343a 3536 2c42 2c31  -02 01:34:56,B,1
-00005b20: 3031 0a20 2020 2020 2020 2032 3030 312d  01.        2001-
-00005b30: 3032 2d33 3020 3032 3a33 343a 3536 2c43  02-30 02:34:56,C
-00005b40: 2c31 3032 0a20 2020 2020 2020 202c 442c  ,102.        ,D,
-00005b50: 3130 330a 2020 2020 2020 2020 2222 2229  103.        """)
-00005b60: 0a20 2020 2020 2020 2074 6573 745f 6b77  .        test_kw
-00005b70: 6172 6773 203d 205b 0a20 2020 2020 2020  args = [.       
-00005b80: 2020 2020 207b 2765 6d70 7479 273a 2027       {'empty': '
-00005b90: 272c 2027 6f6e 5f65 7272 6f72 273a 204e  ', 'on_error': N
-00005ba0: 6f6e 657d 2c0a 2020 2020 2020 2020 2020  one},.          
-00005bb0: 2020 7b27 656d 7074 7927 3a20 274e 2f41    {'empty': 'N/A
-00005bc0: 272c 2027 6f6e 5f65 7272 6f72 273a 2064  ', 'on_error': d
-00005bd0: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00005be0: 2e6d 696e 7d2c 0a20 2020 2020 2020 2020  .min},.         
-00005bf0: 2020 207b 2765 6d70 7479 273a 2064 6174     {'empty': dat
-00005c00: 6574 696d 652e 6461 7465 7469 6d65 2e6d  etime.datetime.m
-00005c10: 696e 2c20 276f 6e5f 6572 726f 7227 3a20  in, 'on_error': 
-00005c20: 2727 7d2c 0a20 2020 2020 2020 205d 0a20  ''},.        ]. 
-00005c30: 2020 2020 2020 2066 6f72 206b 7761 7267         for kwarg
-00005c40: 7320 696e 2074 6573 745f 6b77 6172 6773  s in test_kwargs
-00005c50: 3a0a 2020 2020 2020 2020 2020 2020 7462  :.            tb
-00005c60: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e63  l = lt.Table().c
-00005c70: 7376 5f69 6d70 6f72 7428 6461 7461 2c0a  sv_import(data,.
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00005cb0: 6d73 3d7b 2761 273a 206c 742e 5461 626c  ms={'a': lt.Tabl
-00005cc0: 652e 7061 7273 655f 6461 7465 7469 6d65  e.parse_datetime
-00005cd0: 2827 2559 2d25 6d2d 2564 2025 483a 254d  ('%Y-%m-%d %H:%M
-00005ce0: 3a25 5327 2c0a 2020 2020 2020 2020 2020  :%S',.          
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
-00005d40: 7d29 0a20 2020 2020 2020 2020 2020 2070  }).            p
-00005d50: 7269 6e74 285b 7374 7228 6129 2066 6f72  rint([str(a) for
-00005d60: 2061 2069 6e20 7462 6c2e 616c 6c2e 615d   a in tbl.all.a]
-00005d70: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
-00005d80: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00005d90: 2822 7465 7374 2054 6162 6c65 2e70 6172  ("test Table.par
-00005da0: 7365 5f64 6174 655f 7469 6d65 2065 7272  se_date_time err
-00005db0: 6f72 7322 2c20 2a2a 6b77 6172 6773 293a  ors", **kwargs):
-00005dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005dd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00005de0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00005df0: 2020 2020 2020 205b 6b77 6172 6773 5b22         [kwargs["
-00005e00: 6f6e 5f65 7272 6f72 225d 2c20 6b77 6172  on_error"], kwar
-00005e10: 6773 5b22 656d 7074 7922 5d5d 2c0a 2020  gs["empty"]],.  
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e30: 2020 6c69 7374 2874 626c 2e61 6c6c 2e61    list(tbl.all.a
-00005e40: 295b 2d32 3a5d 0a20 2020 2020 2020 2020  )[-2:].         
-00005e50: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00005e60: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00005e70: 7375 6254 6573 7428 2274 6573 7420 5461  subTest("test Ta
-00005e80: 626c 652e 7061 7273 655f 6461 7465 5f74  ble.parse_date_t
-00005e90: 696d 6520 7661 6c69 6422 2c20 2a2a 6b77  ime valid", **kw
-00005ea0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
-00005eb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00005ec0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00005ed0: 2020 2020 2020 2020 2020 2020 205b 6461               [da
-00005ee0: 7465 7469 6d65 2e64 6174 6574 696d 6528  tetime.datetime(
-00005ef0: 3230 3031 2c20 312c 2031 2c20 302c 2033  2001, 1, 1, 0, 3
-00005f00: 342c 2035 3629 2c0a 2020 2020 2020 2020  4, 56),.        
-00005f10: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00005f20: 6574 696d 652e 6461 7465 7469 6d65 2832  etime.datetime(2
-00005f30: 3030 312c 2031 2c20 322c 2031 2c20 3334  001, 1, 2, 1, 34
-00005f40: 2c20 3536 295d 2c0a 2020 2020 2020 2020  , 56)],.        
-00005f50: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00005f60: 2874 626c 2e61 6c6c 2e61 295b 3a32 5d0a  (tbl.all.a)[:2].
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00005f90: 7061 7273 655f 6461 7465 5f74 7261 6e73  parse_date_trans
-00005fa0: 666f 726d 2873 656c 6629 3a0a 2020 2020  form(self):.    
-00005fb0: 2020 2020 696d 706f 7274 2064 6174 6574      import datet
-00005fc0: 696d 650a 0a20 2020 2020 2020 2064 6174  ime..        dat
-00005fd0: 6120 3d20 7465 7874 7772 6170 2e64 6564  a = textwrap.ded
-00005fe0: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-00005ff0: 2061 2c62 2c63 0a20 2020 2020 2020 2032   a,b,c.        2
-00006000: 3030 312d 3031 2d30 3120 3030 3a33 343a  001-01-01 00:34:
-00006010: 3536 2c41 2c31 3030 0a20 2020 2020 2020  56,A,100.       
-00006020: 2032 3030 312d 3031 2d30 3220 3031 3a33   2001-01-02 01:3
-00006030: 343a 3536 2c42 2c31 3031 0a20 2020 2020  4:56,B,101.     
-00006040: 2020 2032 3030 312d 3032 2d33 3020 3032     2001-02-30 02
-00006050: 3a33 343a 3536 2c43 2c31 3032 0a20 2020  :34:56,C,102.   
-00006060: 2020 2020 202c 442c 3130 330a 2020 2020       ,D,103.    
-00006070: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
-00006080: 2074 6573 745f 6b77 6172 6773 203d 205b   test_kwargs = [
-00006090: 0a20 2020 2020 2020 2020 2020 207b 2765  .            {'e
-000060a0: 6d70 7479 273a 2027 272c 2027 6f6e 5f65  mpty': '', 'on_e
-000060b0: 7272 6f72 273a 204e 6f6e 657d 2c0a 2020  rror': None},.  
-000060c0: 2020 2020 2020 2020 2020 7b27 656d 7074            {'empt
-000060d0: 7927 3a20 274e 2f41 272c 2027 6f6e 5f65  y': 'N/A', 'on_e
-000060e0: 7272 6f72 273a 2064 6174 6574 696d 652e  rror': datetime.
-000060f0: 6461 7465 2e6d 696e 7d2c 0a20 2020 2020  date.min},.     
-00006100: 2020 2020 2020 207b 2765 6d70 7479 273a         {'empty':
-00006110: 2064 6174 6574 696d 652e 6461 7465 2e6d   datetime.date.m
-00006120: 696e 2c20 276f 6e5f 6572 726f 7227 3a20  in, 'on_error': 
-00006130: 2727 7d2c 0a20 2020 2020 2020 205d 0a20  ''},.        ]. 
-00006140: 2020 2020 2020 2066 6f72 206b 7761 7267         for kwarg
-00006150: 7320 696e 2074 6573 745f 6b77 6172 6773  s in test_kwargs
-00006160: 3a0a 2020 2020 2020 2020 2020 2020 7462  :.            tb
-00006170: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e63  l = lt.Table().c
-00006180: 7376 5f69 6d70 6f72 7428 6461 7461 2c0a  sv_import(data,.
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-000061c0: 6d73 3d7b 2761 273a 206c 742e 5461 626c  ms={'a': lt.Tabl
-000061d0: 652e 7061 7273 655f 6461 7465 2827 2559  e.parse_date('%Y
-000061e0: 2d25 6d2d 2564 2025 483a 254d 3a25 5327  -%m-%d %H:%M:%S'
-000061f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00006240: 2a6b 7761 7267 7329 7d29 0a20 2020 2020  *kwargs)}).     
-00006250: 2020 2020 2020 2070 7269 6e74 285b 7374         print([st
-00006260: 7228 6129 2066 6f72 2061 2069 6e20 7462  r(a) for a in tb
-00006270: 6c2e 616c 6c2e 615d 290a 0a20 2020 2020  l.all.a])..     
-00006280: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00006290: 2e73 7562 5465 7374 2822 7465 7374 2054  .subTest("test T
-000062a0: 6162 6c65 2e70 6172 7365 5f64 6174 655f  able.parse_date_
-000062b0: 7469 6d65 2065 7272 6f72 7322 2c20 2a2a  time errors", **
-000062c0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-000062d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000062e0: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-000062f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00006300: 6b77 6172 6773 5b22 6f6e 5f65 7272 6f72  kwargs["on_error
-00006310: 225d 2c20 6b77 6172 6773 5b22 656d 7074  "], kwargs["empt
-00006320: 7922 5d5d 2c0a 2020 2020 2020 2020 2020  y"]],.          
-00006330: 2020 2020 2020 2020 2020 6c69 7374 2874            list(t
-00006340: 626c 2e61 6c6c 2e61 295b 2d32 3a5d 0a20  bl.all.a)[-2:]. 
-00006350: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006360: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00006370: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00006380: 2274 6573 7420 5461 626c 652e 7061 7273  "test Table.pars
-00006390: 655f 6461 7465 5f74 696d 6520 7661 6c69  e_date_time vali
-000063a0: 6422 2c20 2a2a 6b77 6172 6773 293a 0a20  d", **kwargs):. 
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000063c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000063d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000063e0: 2020 2020 205b 6461 7465 7469 6d65 2e64       [datetime.d
-000063f0: 6174 6528 3230 3031 2c20 312c 2031 292c  ate(2001, 1, 1),
-00006400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006410: 2020 2020 2020 6461 7465 7469 6d65 2e64        datetime.d
-00006420: 6174 6528 3230 3031 2c20 312c 2032 295d  ate(2001, 1, 2)]
-00006430: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006440: 2020 2020 2020 6c69 7374 2874 626c 2e61        list(tbl.a
-00006450: 6c6c 2e61 295b 3a32 5d0a 2020 2020 2020  ll.a)[:2].      
-00006460: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00006470: 2064 6566 2074 6573 745f 7061 7273 655f   def test_parse_
-00006480: 7469 6d65 6465 6c74 615f 7472 616e 7366  timedelta_transf
-00006490: 6f72 6d28 7365 6c66 293a 0a20 2020 2020  orm(self):.     
-000064a0: 2020 2069 6d70 6f72 7420 6461 7465 7469     import dateti
-000064b0: 6d65 0a0a 2020 2020 2020 2020 7072 6f63  me..        proc
-000064c0: 6573 735f 6461 7461 203d 2074 6578 7477  ess_data = textw
-000064d0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-000064e0: 2020 2020 2020 2020 2020 2020 656c 6170              elap
-000064f0: 7365 645f 7469 6d65 2c65 7170 742c 6576  sed_time,eqpt,ev
-00006500: 656e 742c 6c6f 742c 7069 6563 6573 0a20  ent,lot,pieces. 
-00006510: 2020 2020 2020 2020 2020 2030 3a30 303a             0:00:
-00006520: 3030 2c44 5249 4c4c 3031 2c4c 6f74 5374  00,DRILL01,LotSt
-00006530: 6172 742c 5043 4231 3436 2c31 0a20 2020  art,PCB146,1.   
-00006540: 2020 2020 2020 2020 2030 3a30 303a 3430           0:00:40
-00006550: 2c44 5249 4c4c 3031 2c54 6f6f 6c31 2c50  ,DRILL01,Tool1,P
-00006560: 4342 3134 362c 320a 2020 2020 2020 2020  CB146,2.        
-00006570: 2020 2020 303a 3033 3a34 352c 4452 494c      0:03:45,DRIL
-00006580: 4c30 312c 546f 6f6c 322c 5043 4231 3436  L01,Tool2,PCB146
-00006590: 2c34 0a20 2020 2020 2020 2020 2020 2030  ,4.            0
-000065a0: 3a30 363a 3136 2c44 5249 4c4c 3031 2c4c  :06:16,DRILL01,L
-000065b0: 6f74 456e 642c 5043 4231 3436 2c38 0a20  otEnd,PCB146,8. 
-000065c0: 2020 2020 2020 2020 2020 2022 2222 290a             """).
-000065d0: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
-000065e0: 726d 7320 3d20 7b27 656c 6170 7365 645f  rms = {'elapsed_
-000065f0: 7469 6d65 273a 206c 742e 5461 626c 652e  time': lt.Table.
-00006600: 7061 7273 655f 7469 6d65 6465 6c74 6128  parse_timedelta(
-00006610: 2225 483a 254d 3a25 5322 292c 0a20 2020  "%H:%M:%S"),.   
+00003230: 626c 652e 6472 6f70 5f69 6e64 6578 2827  ble.drop_index('
+00003240: 6127 290a 2020 2020 2020 2020 7461 626c  a').        tabl
+00003250: 652e 696e 7365 7274 2873 656c 662e 6d61  e.insert(self.ma
+00003260: 6b65 5f64 6174 615f 6f62 6a65 6374 2834  ke_data_object(4
+00003270: 2c20 312c 2030 2929 0a0a 2020 2020 2020  , 1, 0))..      
+00003280: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00003290: 7274 5261 6973 6573 284b 6579 4572 726f  rtRaises(KeyErro
+000032a0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000032b0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+000032c0: 6578 2827 6127 2c20 756e 6971 7565 3d54  ex('a', unique=T
+000032d0: 7275 6529 0a0a 2020 2020 6465 6620 7465  rue)..    def te
+000032e0: 7374 5f69 6e73 6572 745f 6469 6374 7328  st_insert_dicts(
+000032f0: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+00003300: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+00003310: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+00003320: 696e 7365 7274 287b 2261 223a 2031 2c20  insert({"a": 1, 
+00003330: 2262 223a 2032 2c20 2263 223a 2033 7d29  "b": 2, "c": 3})
+00003340: 0a20 2020 2020 2020 2074 6162 6c65 2e69  .        table.i
+00003350: 6e73 6572 7428 7b22 6122 3a20 342c 2022  nsert({"a": 4, "
+00003360: 6222 3a20 352c 2022 6322 3a20 367d 290a  b": 5, "c": 6}).
+00003370: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
+00003380: 6561 7465 5f69 6e64 6578 2827 6127 2c20  eate_index('a', 
+00003390: 756e 6971 7565 3d54 7275 6529 0a20 2020  unique=True).   
+000033a0: 2020 2020 2072 6563 302c 2072 6563 3120       rec0, rec1 
+000033b0: 3d20 7461 626c 650a 2020 2020 2020 2020  = table.        
+000033c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000033d0: 287b 2261 223a 2031 2c20 2262 223a 2032  ({"a": 1, "b": 2
+000033e0: 2c20 2263 223a 2033 7d2c 2076 6172 7328  , "c": 3}, vars(
+000033f0: 7265 6330 2929 0a20 2020 2020 2020 2073  rec0)).        s
+00003400: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003410: 6c74 2e64 6566 6175 6c74 5f72 6f77 5f63  lt.default_row_c
+00003420: 6c61 7373 2c20 7479 7065 2872 6563 3029  lass, type(rec0)
+00003430: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003440: 7373 6572 7445 7175 616c 2831 2c20 7265  ssertEqual(1, re
+00003450: 6330 2e61 290a 0a20 2020 2020 2020 2023  c0.a)..        #
+00003460: 2069 6e73 6572 7420 6120 6e65 7374 6564   insert a nested
+00003470: 2064 6963 740a 2020 2020 2020 2020 7461   dict.        ta
+00003480: 626c 652e 636c 6561 7228 290a 2020 2020  ble.clear().    
+00003490: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
+000034a0: 287b 2261 223a 2031 2c20 2262 223a 2032  ({"a": 1, "b": 2
+000034b0: 2c20 2263 223a 2033 2c20 2264 223a 207b  , "c": 3, "d": {
+000034c0: 2278 223a 2031 3030 2c20 2279 223a 2032  "x": 100, "y": 2
+000034d0: 3030 7d7d 290a 2020 2020 2020 2020 7461  00}}).        ta
+000034e0: 626c 652e 696e 7365 7274 287b 2261 223a  ble.insert({"a":
+000034f0: 2034 2c20 2262 223a 2035 2c20 2263 223a   4, "b": 5, "c":
+00003500: 2036 2c20 2264 223a 207b 2278 223a 2031   6, "d": {"x": 1
+00003510: 3031 2c20 2279 223a 2032 3031 7d7d 290a  01, "y": 201}}).
+00003520: 2020 2020 2020 2020 7265 6330 2c20 7265          rec0, re
+00003530: 6331 203d 2074 6162 6c65 0a20 2020 2020  c1 = table.     
+00003540: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00003550: 7561 6c28 3130 302c 2072 6563 302e 642e  ual(100, rec0.d.
+00003560: 7829 0a20 2020 2020 2020 2073 656c 662e  x).        self.
+00003570: 6173 7365 7274 4571 7561 6c28 3130 312c  assertEqual(101,
+00003580: 2072 6563 312e 642e 7829 0a0a 2020 2020   rec1.d.x)..    
+00003590: 6465 6620 7465 7374 5f77 6865 7265 5f65  def test_where_e
+000035a0: 7175 616c 7328 7365 6c66 293a 0a20 2020  quals(self):.   
+000035b0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+000035c0: 2031 300a 2020 2020 2020 2020 7461 626c   10.        tabl
+000035d0: 6520 3d20 6d61 6b65 5f74 6573 745f 7461  e = make_test_ta
+000035e0: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+000035f0: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+00003600: 7369 7a65 290a 0a20 2020 2020 2020 2073  size)..        s
+00003610: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003620: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
+00003630: 697a 652c 206c 656e 2874 6162 6c65 2e77  ize, len(table.w
+00003640: 6865 7265 2861 3d35 2929 290a 2020 2020  here(a=5))).    
+00003650: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003660: 7175 616c 2830 2c20 6c65 6e28 7461 626c  qual(0, len(tabl
+00003670: 652e 7768 6572 6528 613d 2d31 2929 290a  e.where(a=-1))).
+00003680: 0a20 2020 2064 6566 2074 6573 745f 7768  .    def test_wh
+00003690: 6572 655f 6571 7561 6c73 5f6e 6f6e 6528  ere_equals_none(
+000036a0: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+000036b0: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
+000036c0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+000036d0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+000036e0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000036f0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+00003700: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00003710: 7365 7274 4571 7561 6c28 302c 206c 656e  sertEqual(0, len
+00003720: 2874 6162 6c65 2e77 6865 7265 2861 3d35  (table.where(a=5
+00003730: 2c20 623d 7465 7374 5f73 697a 6529 2929  , b=test_size)))
+00003740: 0a0a 2020 2020 6465 6620 7465 7374 5f77  ..    def test_w
+00003750: 6865 7265 5f65 7175 616c 735f 7769 7468  here_equals_with
+00003760: 5f69 6e64 6578 2873 656c 6629 3a0a 2020  _index(self):.  
+00003770: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00003780: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+00003790: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+000037a0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+000037b0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+000037c0: 5f73 697a 6529 0a20 2020 2020 2020 2074  _size).        t
+000037d0: 6162 6c65 2e63 7265 6174 655f 696e 6465  able.create_inde
+000037e0: 7828 2761 2729 0a0a 2020 2020 2020 2020  x('a')..        
+000037f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003800: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+00003810: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
+00003820: 7768 6572 6528 613d 3529 2929 0a20 2020  where(a=5))).   
+00003830: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00003840: 4571 7561 6c28 302c 206c 656e 2874 6162  Equal(0, len(tab
+00003850: 6c65 2e77 6865 7265 2861 3d2d 3129 2929  le.where(a=-1)))
+00003860: 0a0a 2020 2020 6465 6620 7465 7374 5f77  ..    def test_w
+00003870: 6865 7265 5f72 616e 6765 2873 656c 6629  here_range(self)
+00003880: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
+00003890: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
+000038a0: 2074 6162 6c65 203d 206d 616b 655f 7465   table = make_te
+000038b0: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+000038c0: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+000038d0: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+000038e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000038f0: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
+00003900: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
+00003910: 626c 652e 7768 6572 6528 6c61 6d62 6461  ble.where(lambda
+00003920: 2072 6563 3a20 7265 632e 6120 3d3d 2072   rec: rec.a == r
+00003930: 6563 2e62 2929 290a 0a20 2020 2064 6566  ec.b)))..    def
+00003940: 2074 6573 745f 7768 6572 655f 636f 6d70   test_where_comp
+00003950: 6172 6174 6f72 2873 656c 6629 3a0a 2020  arator(self):.  
+00003960: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00003970: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+00003980: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+00003990: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+000039a0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+000039b0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+000039c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000039d0: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+000039e0: 7369 7a65 2a34 2c20 6c65 6e28 7461 626c  size*4, len(tabl
+000039f0: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
+00003a00: 6c65 2e6c 7428 3429 2929 290a 2020 2020  le.lt(4)))).    
+00003a10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003a20: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
+00003a30: 6573 745f 7369 7a65 2a28 342b 3129 2c20  est_size*(4+1), 
+00003a40: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
+00003a50: 613d 6c74 2e54 6162 6c65 2e6c 6528 3429  a=lt.Table.le(4)
+00003a60: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
+00003a70: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00003a80: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+00003a90: 2a28 7465 7374 5f73 697a 652d 342d 3129  *(test_size-4-1)
+00003aa0: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003ab0: 6528 613d 6c74 2e54 6162 6c65 2e67 7428  e(a=lt.Table.gt(
+00003ac0: 3429 2929 290a 2020 2020 2020 2020 7365  4)))).        se
+00003ad0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00003ae0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00003af0: 7a65 2a28 7465 7374 5f73 697a 652d 3429  ze*(test_size-4)
+00003b00: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003b10: 6528 613d 6c74 2e54 6162 6c65 2e67 6528  e(a=lt.Table.ge(
+00003b20: 3429 2929 290a 2020 2020 2020 2020 7365  4)))).        se
+00003b30: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00003b40: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00003b50: 7a65 2a28 7465 7374 5f73 697a 652d 3129  ze*(test_size-1)
+00003b60: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003b70: 6528 613d 6c74 2e54 6162 6c65 2e6e 6528  e(a=lt.Table.ne(
+00003b80: 3429 2929 290a 2020 2020 2020 2020 7365  4)))).        se
+00003b90: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00003ba0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00003bb0: 7a65 2c20 6c65 6e28 7461 626c 652e 7768  ze, len(table.wh
+00003bc0: 6572 6528 613d 6c74 2e54 6162 6c65 2e65  ere(a=lt.Table.e
+00003bd0: 7128 3429 2929 290a 2020 2020 2020 2020  q(4)))).        
+00003be0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003bf0: 2874 6573 745f 7369 7a65 2c20 6c65 6e28  (test_size, len(
+00003c00: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
+00003c10: 2e54 6162 6c65 2e65 7128 3429 2c20 623d  .Table.eq(4), b=
+00003c20: 6c74 2e54 6162 6c65 2e65 7128 3429 2929  lt.Table.eq(4)))
+00003c30: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003c40: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00003c50: 7369 7a65 2a74 6573 745f 7369 7a65 2a34  size*test_size*4
+00003c60: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003c70: 6528 613d 6c74 2e54 6162 6c65 2e62 6574  e(a=lt.Table.bet
+00003c80: 7765 656e 2833 2c20 3829 2929 290a 2020  ween(3, 8)))).  
+00003c90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00003ca0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00003cb0: 2a74 6573 745f 7369 7a65 2a34 2c20 6c65  *test_size*4, le
+00003cc0: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003cd0: 6c74 2e54 6162 6c65 2e77 6974 6869 6e28  lt.Table.within(
+00003ce0: 322c 2035 2929 2929 0a20 2020 2020 2020  2, 5)))).       
+00003cf0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00003d00: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
+00003d10: 5f73 697a 652a 332c 206c 656e 2874 6162  _size*3, len(tab
+00003d20: 6c65 2e77 6865 7265 2861 3d6c 742e 5461  le.where(a=lt.Ta
+00003d30: 626c 652e 696e 5f72 616e 6765 2832 2c20  ble.in_range(2, 
+00003d40: 3529 2929 290a 2020 2020 2020 2020 7365  5)))).        se
+00003d50: 6c66 2e61 7373 6572 7445 7175 616c 2830  lf.assertEqual(0
+00003d60: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003d70: 6528 613d 6c74 2e54 6162 6c65 2e62 6574  e(a=lt.Table.bet
+00003d80: 7765 656e 2833 2c20 3329 2929 290a 2020  ween(3, 3)))).  
+00003d90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00003da0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00003db0: 2a74 6573 745f 7369 7a65 2c20 6c65 6e28  *test_size, len(
+00003dc0: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
+00003dd0: 2e54 6162 6c65 2e77 6974 6869 6e28 332c  .Table.within(3,
+00003de0: 2033 2929 2929 0a20 2020 2020 2020 2073   3)))).        s
+00003df0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003e00: 302c 206c 656e 2874 6162 6c65 2e77 6865  0, len(table.whe
+00003e10: 7265 2861 3d6c 742e 5461 626c 652e 696e  re(a=lt.Table.in
+00003e20: 5f72 616e 6765 2833 2c20 3329 2929 290a  _range(3, 3)))).
+00003e30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003e40: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+00003e50: 7a65 2a74 6573 745f 7369 7a65 2a34 2c20  ze*test_size*4, 
+00003e60: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
+00003e70: 613d 6c74 2e54 6162 6c65 2e69 735f 696e  a=lt.Table.is_in
+00003e80: 285b 322c 2034 2c20 362c 2038 5d29 2929  ([2, 4, 6, 8])))
+00003e90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003ea0: 7373 6572 7445 7175 616c 2830 2c20 6c65  ssertEqual(0, le
+00003eb0: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003ec0: 6c74 2e54 6162 6c65 2e69 735f 696e 285b  lt.Table.is_in([
+00003ed0: 5d29 2929 290a 2020 2020 2020 2020 7365  ])))).        se
+00003ee0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00003ef0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00003f00: 7a65 2a28 7465 7374 5f73 697a 652d 3429  ze*(test_size-4)
+00003f10: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003f20: 6528 613d 6c74 2e54 6162 6c65 2e6e 6f74  e(a=lt.Table.not
+00003f30: 5f69 6e28 5b32 2c20 342c 2036 2c20 385d  _in([2, 4, 6, 8]
+00003f40: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
+00003f50: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
+00003f60: 7374 5f73 697a 652a 7465 7374 5f73 697a  st_size*test_siz
+00003f70: 652a 7465 7374 5f73 697a 652c 206c 656e  e*test_size, len
+00003f80: 2874 6162 6c65 2e77 6865 7265 2861 3d6c  (table.where(a=l
+00003f90: 742e 5461 626c 652e 6e6f 745f 696e 285b  t.Table.not_in([
+00003fa0: 5d29 2929 290a 0a20 2020 2020 2020 2023  ]))))..        #
+00003fb0: 2061 6464 2061 2072 6563 6f72 6420 636f   add a record co
+00003fc0: 6e74 6169 6e69 6e67 2061 204e 6f6e 6520  ntaining a None 
+00003fd0: 7661 6c75 6520 746f 2074 6573 7420 6973  value to test is
+00003fe0: 5f6e 6f6e 6520 616e 6420 6973 5f6e 6f74  _none and is_not
+00003ff0: 5f6e 6f6e 6520 636f 6d70 6172 6174 6f72  _none comparator
+00004000: 730a 2020 2020 2020 2020 7461 626c 652e  s.        table.
+00004010: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
+00004020: 5f64 6174 615f 6f62 6a65 6374 2861 3d31  _data_object(a=1
+00004030: 2c20 623d 322c 2063 3d4e 6f6e 6529 290a  , b=2, c=None)).
+00004040: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00004050: 6572 7445 7175 616c 2831 2c20 6c65 6e28  ertEqual(1, len(
+00004060: 7461 626c 652e 7768 6572 6528 633d 6c74  table.where(c=lt
+00004070: 2e54 6162 6c65 2e69 735f 6e6f 6e65 2829  .Table.is_none()
+00004080: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
+00004090: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+000040a0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+000040b0: 2a74 6573 745f 7369 7a65 2c20 6c65 6e28  *test_size, len(
+000040c0: 7461 626c 652e 7768 6572 6528 633d 6c74  table.where(c=lt
+000040d0: 2e54 6162 6c65 2e69 735f 6e6f 745f 6e6f  .Table.is_not_no
+000040e0: 6e65 2829 2929 290a 0a20 2020 2020 2020  ne())))..       
+000040f0: 2023 2061 6464 2061 2072 6563 6f72 6420   # add a record 
+00004100: 636f 6e74 6169 6e69 6e67 2061 206d 6973  containing a mis
+00004110: 7369 6e67 2076 616c 7565 2074 6f20 7465  sing value to te
+00004120: 7374 2069 735f 6e75 6c6c 2061 6e64 2069  st is_null and i
+00004130: 735f 6e6f 745f 6e75 6c6c 2063 6f6d 7061  s_not_null compa
+00004140: 7261 746f 7273 0a20 2020 2020 2020 2074  rators.        t
+00004150: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
+00004160: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00004170: 7428 613d 312c 2062 3d32 2c20 633d 2222  t(a=1, b=2, c=""
+00004180: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00004190: 6173 7365 7274 4571 7561 6c28 322c 206c  assertEqual(2, l
+000041a0: 656e 2874 6162 6c65 2e77 6865 7265 2863  en(table.where(c
+000041b0: 3d6c 742e 5461 626c 652e 6973 5f6e 756c  =lt.Table.is_nul
+000041c0: 6c28 2929 2929 0a20 2020 2020 2020 2073  l()))).        s
+000041d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000041e0: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+000041f0: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00004200: 652c 206c 656e 2874 6162 6c65 2e77 6865  e, len(table.whe
+00004210: 7265 2863 3d6c 742e 5461 626c 652e 6973  re(c=lt.Table.is
+00004220: 5f6e 6f74 5f6e 756c 6c28 2929 2929 0a0a  _not_null())))..
+00004230: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00004240: 2020 2020 2020 2020 2074 6162 6c65 2e69           table.i
+00004250: 6e73 6572 7428 7365 6c66 2e6d 616b 655f  nsert(self.make_
+00004260: 6461 7461 5f6f 626a 6563 7428 613d 312c  data_object(a=1,
+00004270: 2062 3d32 2929 0a20 2020 2020 2020 2065   b=2)).        e
+00004280: 7863 6570 7420 5479 7065 4572 726f 723a  xcept TypeError:
+00004290: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
+000042a0: 6f74 2061 6c6c 2064 6174 6120 6f62 6a65  ot all data obje
+000042b0: 6374 2074 7970 6573 2062 6569 6e67 2074  ct types being t
+000042c0: 6573 7465 6420 7375 7070 6f72 7420 6d69  ested support mi
+000042d0: 7373 696e 6720 6174 7472 6962 7574 6573  ssing attributes
+000042e0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+000042f0: 730a 2020 2020 2020 2020 656c 7365 3a0a  s.        else:.
+00004300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004310: 2e61 7373 6572 7445 7175 616c 2833 2c20  .assertEqual(3, 
+00004320: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
+00004330: 633d 6c74 2e54 6162 6c65 2e69 735f 6e75  c=lt.Table.is_nu
+00004340: 6c6c 2829 2929 290a 2020 2020 2020 2020  ll()))).        
+00004350: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00004360: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
+00004370: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
+00004380: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
+00004390: 652e 7768 6572 6528 633d 6c74 2e54 6162  e.where(c=lt.Tab
+000043a0: 6c65 2e69 735f 6e6f 745f 6e75 6c6c 2829  le.is_not_null()
+000043b0: 2929 290a 0a20 2020 2064 6566 2074 6573  )))..    def tes
+000043c0: 745f 7768 6572 655f 7374 725f 636f 6d70  t_where_str_comp
+000043d0: 6172 6174 6f72 2873 656c 6629 3a0a 2020  arator(self):.  
+000043e0: 2020 2020 2020 756e 6963 6f64 655f 6e75        unicode_nu
+000043f0: 6d62 6572 7320 3d20 6c74 2e54 6162 6c65  mbers = lt.Table
+00004400: 2829 2e63 7376 5f69 6d70 6f72 7428 7465  ().csv_import(te
+00004410: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
+00004420: 225c 0a20 2020 2020 2020 2020 2020 206e  "\.            n
+00004430: 616d 652c 636f 6465 5f76 616c 7565 2c6e  ame,code_value,n
+00004440: 756d 6572 6963 5f76 616c 7565 0a20 2020  umeric_value.   
+00004450: 2020 2020 2020 2020 2052 4f4d 414e 204e           ROMAN N
+00004460: 554d 4552 414c 204f 4e45 2c38 3534 342c  UMERAL ONE,8544,
+00004470: 310a 2020 2020 2020 2020 2020 2020 524f  1.            RO
+00004480: 4d41 4e20 4e55 4d45 5241 4c20 5457 4f2c  MAN NUMERAL TWO,
+00004490: 3835 3435 2c32 0a20 2020 2020 2020 2020  8545,2.         
+000044a0: 2020 2052 4f4d 414e 204e 554d 4552 414c     ROMAN NUMERAL
+000044b0: 2054 4852 4545 2c38 3534 362c 330a 2020   THREE,8546,3.  
+000044c0: 2020 2020 2020 2020 2020 524f 4d41 4e20            ROMAN 
+000044d0: 4e55 4d45 5241 4c20 464f 5552 2c38 3534  NUMERAL FOUR,854
+000044e0: 372c 340a 2020 2020 2020 2020 2020 2020  7,4.            
+000044f0: 524f 4d41 4e20 4e55 4d45 5241 4c20 4649  ROMAN NUMERAL FI
+00004500: 5645 2c38 3534 382c 350a 2020 2020 2020  VE,8548,5.      
+00004510: 2020 2020 2020 524f 4d41 4e20 4e55 4d45        ROMAN NUME
+00004520: 5241 4c20 5349 582c 3835 3439 2c36 0a20  RAL SIX,8549,6. 
+00004530: 2020 2020 2020 2020 2020 2052 4f4d 414e             ROMAN
+00004540: 204e 554d 4552 414c 2053 4556 454e 2c38   NUMERAL SEVEN,8
+00004550: 3535 302c 370a 2020 2020 2020 2020 2020  550,7.          
+00004560: 2020 524f 4d41 4e20 4e55 4d45 5241 4c20    ROMAN NUMERAL 
+00004570: 4549 4748 542c 3835 3531 2c38 0a20 2020  EIGHT,8551,8.   
+00004580: 2020 2020 2020 2020 2052 4f4d 414e 204e           ROMAN N
+00004590: 554d 4552 414c 204e 494e 452c 3835 3532  UMERAL NINE,8552
+000045a0: 2c39 0a20 2020 2020 2020 2020 2020 2052  ,9.            R
+000045b0: 4f4d 414e 204e 554d 4552 414c 2054 454e  OMAN NUMERAL TEN
+000045c0: 2c38 3535 332c 3130 0a20 2020 2020 2020  ,8553,10.       
+000045d0: 2020 2020 2053 5550 4552 5343 5249 5054       SUPERSCRIPT
+000045e0: 2054 574f 2c31 3738 2c32 0a20 2020 2020   TWO,178,2.     
+000045f0: 2020 2020 2020 2053 5550 4552 5343 5249         SUPERSCRI
+00004600: 5054 2054 4852 4545 2c31 3739 2c33 0a20  PT THREE,179,3. 
+00004610: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
+00004620: 5343 5249 5054 204f 4e45 2c31 3835 2c31  SCRIPT ONE,185,1
+00004630: 0a20 2020 2020 2020 2020 2020 2053 5550  .            SUP
+00004640: 4552 5343 5249 5054 205a 4552 4f2c 3833  ERSCRIPT ZERO,83
+00004650: 3034 2c30 0a20 2020 2020 2020 2020 2020  04,0.           
+00004660: 2053 5550 4552 5343 5249 5054 2046 4f55   SUPERSCRIPT FOU
+00004670: 522c 3833 3038 2c34 0a20 2020 2020 2020  R,8308,4.       
+00004680: 2020 2020 2053 5550 4552 5343 5249 5054       SUPERSCRIPT
+00004690: 2046 4956 452c 3833 3039 2c35 0a20 2020   FIVE,8309,5.   
+000046a0: 2020 2020 2020 2020 2053 5550 4552 5343           SUPERSC
+000046b0: 5249 5054 2053 4958 2c38 3331 302c 360a  RIPT SIX,8310,6.
+000046c0: 2020 2020 2020 2020 2020 2020 5355 5045              SUPE
+000046d0: 5253 4352 4950 5420 5345 5645 4e2c 3833  RSCRIPT SEVEN,83
+000046e0: 3131 2c37 0a20 2020 2020 2020 2020 2020  11,7.           
+000046f0: 2053 5550 4552 5343 5249 5054 2045 4947   SUPERSCRIPT EIG
+00004700: 4854 2c38 3331 322c 380a 2020 2020 2020  HT,8312,8.      
+00004710: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
+00004720: 5420 4e49 4e45 2c38 3331 332c 390a 2020  T NINE,8313,9.  
+00004730: 2020 2020 2020 2020 2020 4349 5243 4c45            CIRCLE
+00004740: 4420 4449 4749 5420 4f4e 452c 3933 3132  D DIGIT ONE,9312
+00004750: 2c31 0a20 2020 2020 2020 2020 2020 2043  ,1.            C
+00004760: 4952 434c 4544 2044 4947 4954 2054 574f  IRCLED DIGIT TWO
+00004770: 2c39 3331 332c 320a 2020 2020 2020 2020  ,9313,2.        
+00004780: 2020 2020 4349 5243 4c45 4420 4449 4749      CIRCLED DIGI
+00004790: 5420 5448 5245 452c 3933 3134 2c33 0a20  T THREE,9314,3. 
+000047a0: 2020 2020 2020 2020 2020 2043 4952 434c             CIRCL
+000047b0: 4544 2044 4947 4954 2046 4f55 522c 3933  ED DIGIT FOUR,93
+000047c0: 3135 2c34 0a20 2020 2020 2020 2020 2020  15,4.           
+000047d0: 2043 4952 434c 4544 2044 4947 4954 2046   CIRCLED DIGIT F
+000047e0: 4956 452c 3933 3136 2c35 0a20 2020 2020  IVE,9316,5.     
+000047f0: 2020 2020 2020 2043 4952 434c 4544 2044         CIRCLED D
+00004800: 4947 4954 2053 4958 2c39 3331 372c 360a  IGIT SIX,9317,6.
+00004810: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
+00004820: 4c45 4420 4449 4749 5420 5345 5645 4e2c  LED DIGIT SEVEN,
+00004830: 3933 3138 2c37 0a20 2020 2020 2020 2020  9318,7.         
+00004840: 2020 2043 4952 434c 4544 2044 4947 4954     CIRCLED DIGIT
+00004850: 2045 4947 4854 2c39 3331 392c 380a 2020   EIGHT,9319,8.  
+00004860: 2020 2020 2020 2020 2020 4349 5243 4c45            CIRCLE
+00004870: 4420 4449 4749 5420 4e49 4e45 2c39 3332  D DIGIT NINE,932
+00004880: 302c 390a 2020 2020 2020 2020 2020 2020  0,9.            
+00004890: 4349 5243 4c45 4420 4449 4749 5420 5a45  CIRCLED DIGIT ZE
+000048a0: 524f 2c39 3435 302c 300a 2020 2020 2020  RO,9450,0.      
+000048b0: 2020 2020 2020 2222 2229 290a 0a20 2020        """))..   
+000048c0: 2020 2020 206f 6e65 7320 3d20 756e 6963       ones = unic
+000048d0: 6f64 655f 6e75 6d62 6572 732e 7768 6572  ode_numbers.wher
+000048e0: 6528 6e61 6d65 3d6c 742e 5461 626c 652e  e(name=lt.Table.
+000048f0: 656e 6473 7769 7468 2822 4f4e 4522 2929  endswith("ONE"))
+00004900: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00004910: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
+00004920: 286f 6e65 7329 290a 0a20 2020 2020 2020  (ones))..       
+00004930: 2073 7570 6572 7320 3d20 756e 6963 6f64   supers = unicod
+00004940: 655f 6e75 6d62 6572 732e 7768 6572 6528  e_numbers.where(
+00004950: 6e61 6d65 3d6c 742e 5461 626c 652e 7374  name=lt.Table.st
+00004960: 6172 7473 7769 7468 2822 5355 5045 5253  artswith("SUPERS
+00004970: 4352 4950 5422 2929 0a20 2020 2020 2020  CRIPT")).       
+00004980: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00004990: 6c28 3130 2c20 6c65 6e28 7375 7065 7273  l(10, len(supers
+000049a0: 2929 0a0a 2020 2020 2020 2020 2320 696d  ))..        # im
+000049b0: 706f 7274 2072 650a 2020 2020 2020 2020  port re.        
+000049c0: 2320 7365 7665 6e73 203d 2075 6e69 636f  # sevens = unico
+000049d0: 6465 5f6e 756d 6265 7273 2e77 6865 7265  de_numbers.where
+000049e0: 286c 616d 6264 6120 7265 633a 2072 652e  (lambda rec: re.
+000049f0: 636f 6d70 696c 6528 7222 2e2a 5345 5645  compile(r".*SEVE
+00004a00: 4e24 2229 2e6d 6174 6368 2872 6563 2e6e  N$").match(rec.n
+00004a10: 616d 6529 290a 0a20 2020 2020 2020 2073  ame))..        s
+00004a20: 6576 656e 7320 3d20 756e 6963 6f64 655f  evens = unicode_
+00004a30: 6e75 6d62 6572 732e 7768 6572 6528 6e61  numbers.where(na
+00004a40: 6d65 3d6c 742e 5461 626c 652e 7265 5f6d  me=lt.Table.re_m
+00004a50: 6174 6368 2872 222e 2a53 4556 454e 2422  atch(r".*SEVEN$"
+00004a60: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00004a70: 6173 7365 7274 4571 7561 6c28 332c 206c  assertEqual(3, l
+00004a80: 656e 2873 6576 656e 7329 290a 0a20 2020  en(sevens))..   
+00004a90: 2020 2020 2023 206d 616b 6520 6e61 6d65       # make name
+00004aa0: 7320 616c 6c20 7469 746c 6520 6361 7365  s all title case
+00004ab0: 0a20 2020 2020 2020 2075 6e69 636f 6465  .        unicode
+00004ac0: 5f6e 756d 6265 7273 2e61 6464 5f66 6965  _numbers.add_fie
+00004ad0: 6c64 2822 6e61 6d65 222c 206c 616d 6264  ld("name", lambd
+00004ae0: 6120 7265 633a 2072 6563 2e6e 616d 652e  a rec: rec.name.
+00004af0: 7469 746c 6528 2929 0a20 2020 2020 2020  title()).       
+00004b00: 2023 2075 7365 2072 6567 6578 2077 6974   # use regex wit
+00004b10: 6820 7265 2066 6c61 670a 2020 2020 2020  h re flag.      
+00004b20: 2020 696d 706f 7274 2072 650a 2020 2020    import re.    
+00004b30: 2020 2020 6369 7263 6c65 6420 3d20 756e      circled = un
+00004b40: 6963 6f64 655f 6e75 6d62 6572 732e 7768  icode_numbers.wh
+00004b50: 6572 6528 6e61 6d65 3d6c 742e 5461 626c  ere(name=lt.Tabl
+00004b60: 652e 7265 5f6d 6174 6368 2872 2263 6972  e.re_match(r"cir
+00004b70: 636c 6564 222c 2066 6c61 6773 3d72 652e  cled", flags=re.
+00004b80: 4929 290a 2020 2020 2020 2020 7365 6c66  I)).        self
+00004b90: 2e61 7373 6572 7445 7175 616c 2831 302c  .assertEqual(10,
+00004ba0: 206c 656e 2863 6972 636c 6564 2929 0a0a   len(circled))..
+00004bb0: 2020 2020 6465 6620 7465 7374 5f77 6865      def test_whe
+00004bc0: 7265 5f61 7474 725f 6675 6e63 7469 6f6e  re_attr_function
+00004bd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004be0: 7465 7374 5f73 697a 6520 3d20 380a 2020  test_size = 8.  
+00004bf0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+00004c00: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+00004c10: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00004c20: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+00004c30: 0a20 2020 2020 2020 2064 6566 2069 735f  .        def is_
+00004c40: 6f64 6428 7829 3a0a 2020 2020 2020 2020  odd(x):.        
+00004c50: 2020 2020 7265 7475 726e 2062 6f6f 6c28      return bool(
+00004c60: 7820 2520 3229 0a0a 2020 2020 2020 2020  x % 2)..        
+00004c70: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00004c80: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+00004c90: 7369 7a65 2a74 6573 745f 7369 7a65 2f2f  size*test_size//
+00004ca0: 322c 206c 656e 2874 6162 6c65 2e77 6865  2, len(table.whe
+00004cb0: 7265 2861 3d69 735f 6f64 6429 2929 0a0a  re(a=is_odd)))..
+00004cc0: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+00004cd0: 5f73 6c69 6365 2873 656c 6629 3a0a 2020  _slice(self):.  
+00004ce0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00004cf0: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+00004d00: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+00004d10: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00004d20: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+00004d30: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00004d40: 7375 6274 6162 6c65 203d 2074 6162 6c65  subtable = table
+00004d50: 5b30 3a3a 7465 7374 5f73 697a 655d 0a20  [0::test_size]. 
+00004d60: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00004d70: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+00004d80: 6520 2a20 7465 7374 5f73 697a 652c 206c  e * test_size, l
+00004d90: 656e 2873 7562 7461 626c 6529 290a 0a20  en(subtable)).. 
+00004da0: 2020 2064 6566 2074 6573 745f 696e 6465     def test_inde
+00004db0: 7869 6e67 2873 656c 6629 3a0a 2020 2020  xing(self):.    
+00004dc0: 2020 2020 6368 6172 7320 3d20 2241 4243      chars = "ABC
+00004dd0: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
+00004de0: 5455 5657 5859 5a22 0a20 2020 2020 2020  TUVWXYZ".       
+00004df0: 206d 616b 655f 7265 6320 3d20 6c61 6d62   make_rec = lamb
+00004e00: 6461 2061 612c 2062 622c 2063 633a 2073  da aa, bb, cc: s
+00004e10: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+00004e20: 6a65 6374 2863 6861 7273 5b61 615d 2c20  ject(chars[aa], 
+00004e30: 6368 6172 735b 6262 5d2c 2063 6861 7273  chars[bb], chars
+00004e40: 5b63 635d 290a 2020 2020 2020 2020 7465  [cc]).        te
+00004e50: 7374 5f73 697a 6520 3d20 3130 0a20 2020  st_size = 10.   
+00004e60: 2020 2020 2074 6162 6c65 203d 206d 616b       table = mak
+00004e70: 655f 7465 7374 5f74 6162 6c65 286d 616b  e_test_table(mak
+00004e80: 655f 7265 632c 2074 6573 745f 7369 7a65  e_rec, test_size
+00004e90: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+00004ea0: 6372 6561 7465 5f69 6e64 6578 2827 6127  create_index('a'
+00004eb0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004ec0: 6173 7365 7274 5472 7565 2827 4127 2069  assertTrue('A' i
+00004ed0: 6e20 7461 626c 652e 6279 2e61 290a 2020  n table.by.a).  
+00004ee0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00004ef0: 7454 7275 6528 2741 4127 206e 6f74 2069  tTrue('AA' not i
+00004f00: 6e20 7461 626c 652e 6279 2e61 290a 2020  n table.by.a).  
+00004f10: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00004f20: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00004f30: 202a 2074 6573 745f 7369 7a65 2c20 6c65   * test_size, le
+00004f40: 6e28 7461 626c 652e 6279 2e61 5b27 4227  n(table.by.a['B'
+00004f50: 5d29 290a 2020 2020 2020 2020 7365 6c66  ])).        self
+00004f60: 2e61 7373 6572 7454 7275 6528 6973 696e  .assertTrue(isin
+00004f70: 7374 616e 6365 2874 6162 6c65 2e62 792e  stance(table.by.
+00004f80: 615b 2742 275d 2c20 6c74 2e54 6162 6c65  a['B'], lt.Table
+00004f90: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00004fa0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00004fb0: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
+00004fc0: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00004fd0: 6162 6c65 2e62 792e 7a0a 0a20 2020 2020  able.by.z..     
+00004fe0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00004ff0: 7561 6c28 7465 7374 5f73 697a 652c 206c  ual(test_size, l
+00005000: 656e 2874 6162 6c65 2e62 792e 612e 6b65  en(table.by.a.ke
+00005010: 7973 2829 2929 0a0a 2020 2020 6465 6620  ys()))..    def 
+00005020: 7465 7374 5f75 6e69 7175 655f 696e 6465  test_unique_inde
+00005030: 7869 6e67 2873 656c 6629 3a0a 2020 2020  xing(self):.    
+00005040: 2020 2020 6368 6172 7320 3d20 2241 4243      chars = "ABC
+00005050: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
+00005060: 5455 5657 5859 5a22 0a20 2020 2020 2020  TUVWXYZ".       
+00005070: 206d 616b 655f 756e 6971 7565 5f6b 6579   make_unique_key
+00005080: 203d 206c 616d 6264 6120 2a61 7267 733a   = lambda *args:
+00005090: 2027 272e 6a6f 696e 2863 6861 7273 5b61   ''.join(chars[a
+000050a0: 7267 5d20 666f 7220 6172 6720 696e 2061  rg] for arg in a
+000050b0: 7267 7329 0a20 2020 2020 2020 206d 616b  rgs).        mak
+000050c0: 655f 7265 6320 3d20 6c61 6d62 6461 2061  e_rec = lambda a
+000050d0: 612c 2062 622c 2063 633a 2073 656c 662e  a, bb, cc: self.
+000050e0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+000050f0: 286d 616b 655f 756e 6971 7565 5f6b 6579  (make_unique_key
+00005100: 2861 612c 2062 622c 2063 6329 2c20 6368  (aa, bb, cc), ch
+00005110: 6172 735b 6262 5d2c 2063 6861 7273 5b63  ars[bb], chars[c
+00005120: 635d 290a 2020 2020 2020 2020 7465 7374  c]).        test
+00005130: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
+00005140: 2020 2074 6162 6c65 203d 206d 616b 655f     table = make_
+00005150: 7465 7374 5f74 6162 6c65 286d 616b 655f  test_table(make_
+00005160: 7265 632c 2074 6573 745f 7369 7a65 2928  rec, test_size)(
+00005170: 2254 6162 6c65 5f31 2229 0a20 2020 2020  "Table_1").     
+00005180: 2020 2074 6162 6c65 2e63 7265 6174 655f     table.create_
+00005190: 696e 6465 7828 2761 272c 2075 6e69 7175  index('a', uniqu
+000051a0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+000051b0: 7265 635f 7479 7065 203d 2074 7970 6528  rec_type = type(
+000051c0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+000051d0: 626a 6563 7428 302c 2030 2c20 3029 290a  bject(0, 0, 0)).
+000051e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000051f0: 7365 7274 5472 7565 2827 4141 4127 2069  sertTrue('AAA' i
+00005200: 6e20 7461 626c 652e 6279 2e61 290a 2020  n table.by.a).  
+00005210: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00005220: 7454 7275 6528 2741 4127 206e 6f74 2069  tTrue('AA' not i
+00005230: 6e20 7461 626c 652e 6279 2e61 290a 2020  n table.by.a).  
+00005240: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00005250: 7454 7275 6528 6973 696e 7374 616e 6365  tTrue(isinstance
+00005260: 2874 6162 6c65 2e62 792e 615b 2742 4141  (table.by.a['BAA
+00005270: 275d 2c20 7265 635f 7479 7065 2929 0a20  '], rec_type)). 
+00005280: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00005290: 2e61 7373 6572 7452 6169 7365 7328 4b65  .assertRaises(Ke
+000052a0: 7945 7272 6f72 293a 0a20 2020 2020 2020  yError):.       
+000052b0: 2020 2020 2074 6162 6c65 2e69 6e73 6572       table.inser
+000052c0: 7428 7365 6c66 2e6d 616b 655f 6461 7461  t(self.make_data
+000052d0: 5f6f 626a 6563 7428 4e6f 6e65 2c20 4e6f  _object(None, No
+000052e0: 6e65 2c20 4e6f 6e65 2929 0a0a 2020 2020  ne, None))..    
+000052f0: 2020 2020 2320 6372 6561 7465 2064 7570      # create dup
+00005300: 6c69 6361 7465 2069 6e64 6578 0a20 2020  licate index.   
+00005310: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00005320: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
+00005330: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+00005340: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
+00005350: 655f 696e 6465 7828 2761 272c 2075 6e69  e_index('a', uni
+00005360: 7175 653d 5472 7565 2c20 6163 6365 7074  que=True, accept
+00005370: 5f6e 6f6e 653d 5472 7565 290a 0a20 2020  _none=True)..   
+00005380: 2020 2020 2023 2063 7265 6174 6520 756e       # create un
+00005390: 6971 7565 2069 6e64 6578 2074 6861 7420  ique index that 
+000053a0: 616c 6c6f 7773 204e 6f6e 6520 7661 6c75  allows None valu
+000053b0: 6573 0a20 2020 2020 2020 2074 6162 6c65  es.        table
+000053c0: 2e64 726f 705f 696e 6465 7828 2761 2729  .drop_index('a')
+000053d0: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
+000053e0: 7265 6174 655f 696e 6465 7828 2761 272c  reate_index('a',
+000053f0: 2075 6e69 7175 653d 5472 7565 2c20 6163   unique=True, ac
+00005400: 6365 7074 5f6e 6f6e 653d 5472 7565 290a  cept_none=True).
+00005410: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
+00005420: 7365 7274 2873 656c 662e 6d61 6b65 5f64  sert(self.make_d
+00005430: 6174 615f 6f62 6a65 6374 284e 6f6e 652c  ata_object(None,
+00005440: 204e 6f6e 652c 2027 4127 2929 0a0a 2020   None, 'A'))..  
+00005450: 2020 2020 2020 7374 725f 6e6f 6e65 5f63        str_none_c
+00005460: 6f6d 7061 7265 203d 206c 616d 6264 6120  ompare = lambda 
+00005470: 783a 2078 2069 6620 6973 696e 7374 616e  x: x if isinstan
+00005480: 6365 2878 2c20 7374 7229 2065 6c73 6520  ce(x, str) else 
+00005490: 6368 7228 3235 3529 2a31 3030 0a20 2020  chr(255)*100.   
+000054a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000054b0: 4571 7561 6c28 736f 7274 6564 2874 6162  Equal(sorted(tab
+000054c0: 6c65 2e62 792e 612e 6b65 7973 2829 2c20  le.by.a.keys(), 
+000054d0: 6b65 793d 7374 725f 6e6f 6e65 5f63 6f6d  key=str_none_com
+000054e0: 7061 7265 292c 0a20 2020 2020 2020 2020  pare),.         
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 736f 7274 6564 2874 6162 6c65 2e61 6c6c  sorted(table.all
+00005510: 2e61 2c20 6b65 793d 7374 725f 6e6f 6e65  .a, key=str_none
+00005520: 5f63 6f6d 7061 7265 2929 0a0a 2020 2020  _compare))..    
+00005530: 2020 2020 2320 6e6f 7720 6472 6f70 2069      # now drop i
+00005540: 6e64 6578 2061 6e64 2072 6563 7265 6174  ndex and recreat
+00005550: 6520 6e6f 7420 7065 726d 6974 7469 6e67  e not permitting
+00005560: 204e 6f6e 652c 2073 686f 756c 6420 7261   None, should ra
+00005570: 6973 6520 6578 6365 7074 696f 6e0a 2020  ise exception.  
+00005580: 2020 2020 2020 7461 626c 652e 6472 6f70        table.drop
+00005590: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
+000055a0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+000055b0: 7365 7274 5261 6973 6573 284b 6579 4572  sertRaises(KeyEr
+000055c0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+000055d0: 2020 7461 626c 652e 6372 6561 7465 5f69    table.create_i
+000055e0: 6e64 6578 2827 6127 2c20 756e 6971 7565  ndex('a', unique
+000055f0: 3d54 7275 652c 2061 6363 6570 745f 6e6f  =True, accept_no
+00005600: 6e65 3d46 616c 7365 290a 0a20 2020 2020  ne=False)..     
+00005610: 2020 2074 6162 6c65 2e63 7265 6174 655f     table.create_
+00005620: 696e 6465 7828 2761 272c 2075 6e69 7175  index('a', uniqu
+00005630: 653d 5472 7565 2c20 6163 6365 7074 5f6e  e=True, accept_n
+00005640: 6f6e 653d 5472 7565 290a 2020 2020 2020  one=True).      
+00005650: 2020 7461 626c 652e 6372 6561 7465 5f69    table.create_i
+00005660: 6e64 6578 2827 6327 290a 0a20 2020 2020  ndex('c')..     
+00005670: 2020 2069 6d70 6f72 7420 7070 7269 6e74     import pprint
+00005680: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+00005690: 7461 626c 652e 696e 666f 2829 0a20 2020  table.info().   
+000056a0: 2020 2020 2070 7072 696e 742e 7070 7269       pprint.ppri
+000056b0: 6e74 2869 6e66 6f29 0a20 2020 2020 2020  nt(info).       
+000056c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000056d0: 6c28 2754 6162 6c65 5f31 272c 2069 6e66  l('Table_1', inf
+000056e0: 6f5b 276e 616d 6527 5d29 0a20 2020 2020  o['name']).     
+000056f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005700: 7561 6c28 5b27 6127 2c20 2762 272c 2027  ual(['a', 'b', '
+00005710: 6327 5d2c 206c 6973 7428 736f 7274 6564  c'], list(sorted
+00005720: 2869 6e66 6f5b 2766 6965 6c64 7327 5d29  (info['fields'])
+00005730: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00005740: 6173 7365 7274 4571 7561 6c28 5b28 2761  assertEqual([('a
+00005750: 272c 2054 7275 6529 2c20 2827 6327 2c20  ', True), ('c', 
+00005760: 4661 6c73 6529 5d2c 206c 6973 7428 736f  False)], list(so
+00005770: 7274 6564 2869 6e66 6f5b 2769 6e64 6578  rted(info['index
+00005780: 6573 275d 2929 290a 2020 2020 2020 2020  es']))).        
+00005790: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000057a0: 2831 3030 312c 2069 6e66 6f5b 276c 656e  (1001, info['len
+000057b0: 275d 290a 0a20 2020 2064 6566 2074 6573  '])..    def tes
+000057c0: 745f 756e 6971 7565 5f69 6e64 6578 5f63  t_unique_index_c
+000057d0: 7265 6174 696f 6e28 7365 6c66 293a 0a20  reation(self):. 
+000057e0: 2020 2020 2020 2074 6162 6c65 203d 206c         table = l
+000057f0: 742e 5461 626c 6528 290a 2020 2020 2020  t.Table().      
+00005800: 2020 7461 626c 652e 696e 7365 7274 287b    table.insert({
+00005810: 2261 223a 2031 2c20 2262 223a 2032 2c20  "a": 1, "b": 2, 
+00005820: 2263 223a 2033 7d29 0a20 2020 2020 2020  "c": 3}).       
+00005830: 2074 6162 6c65 2e69 6e73 6572 7428 7b22   table.insert({"
+00005840: 6122 3a20 342c 2022 6222 3a20 352c 2022  a": 4, "b": 5, "
+00005850: 6322 3a20 367d 290a 2020 2020 2020 2020  c": 6}).        
+00005860: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+00005870: 6578 2822 6122 2c20 756e 6971 7565 3d54  ex("a", unique=T
+00005880: 7275 6529 0a20 2020 2020 2020 2074 6162  rue).        tab
+00005890: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
+000058a0: 2262 2229 0a0a 2020 2020 2020 2020 7365  "b")..        se
+000058b0: 6c66 2e61 7373 6572 7449 7349 6e73 7461  lf.assertIsInsta
+000058c0: 6e63 6528 7461 626c 652e 6279 2e61 2c20  nce(table.by.a, 
+000058d0: 6c74 2e5f 556e 6971 7565 4f62 6a49 6e64  lt._UniqueObjInd
+000058e0: 6578 5772 6170 7065 7229 0a20 2020 2020  exWrapper).     
+000058f0: 2020 2073 656c 662e 6173 7365 7274 4973     self.assertIs
+00005900: 496e 7374 616e 6365 2874 6162 6c65 2e62  Instance(table.b
+00005910: 792e 612c 206c 742e 5f4f 626a 496e 6465  y.a, lt._ObjInde
+00005920: 7857 7261 7070 6572 290a 0a20 2020 2020  xWrapper)..     
+00005930: 2020 2073 656c 662e 6173 7365 7274 4e6f     self.assertNo
+00005940: 7449 7349 6e73 7461 6e63 6528 7461 626c  tIsInstance(tabl
+00005950: 652e 6279 2e62 2c20 6c74 2e5f 556e 6971  e.by.b, lt._Uniq
+00005960: 7565 4f62 6a49 6e64 6578 5772 6170 7065  ueObjIndexWrappe
+00005970: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
+00005980: 6173 7365 7274 4973 496e 7374 616e 6365  assertIsInstance
+00005990: 2874 6162 6c65 2e62 792e 622c 206c 742e  (table.by.b, lt.
+000059a0: 5f4f 626a 496e 6465 7857 7261 7070 6572  _ObjIndexWrapper
+000059b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000059c0: 6368 6169 6e65 645f 696e 6465 7869 6e67  chained_indexing
+000059d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000059e0: 6368 6172 7320 3d20 2241 4243 4445 4647  chars = "ABCDEFG
+000059f0: 4849 4a4b 4c4d 4e4f 5051 5253 5455 5657  HIJKLMNOPQRSTUVW
+00005a00: 5859 5a22 0a20 2020 2020 2020 206d 616b  XYZ".        mak
+00005a10: 655f 7265 6320 3d20 6c61 6d62 6461 2061  e_rec = lambda a
+00005a20: 612c 2062 622c 2063 633a 2073 656c 662e  a, bb, cc: self.
+00005a30: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00005a40: 2863 6861 7273 5b61 6120 2520 6c65 6e28  (chars[aa % len(
+00005a50: 6368 6172 7329 5d2c 0a20 2020 2020 2020  chars)],.       
+00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2063 6861 7273 5b62 6220 2520       chars[bb % 
+00005aa0: 6c65 6e28 6368 6172 7329 5d2c 0a20 2020  len(chars)],.   
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 2020 2020 2020 2063 6861 7273 5b63           chars[c
+00005af0: 6320 2520 6c65 6e28 6368 6172 7329 5d29  c % len(chars)])
+00005b00: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00005b10: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
+00005b20: 7461 626c 6520 3d20 6d61 6b65 5f74 6573  table = make_tes
+00005b30: 745f 7461 626c 6528 6d61 6b65 5f72 6563  t_table(make_rec
+00005b40: 2c20 7465 7374 5f73 697a 6529 0a20 2020  , test_size).   
+00005b50: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
+00005b60: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
+00005b70: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
+00005b80: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
+00005b90: 2020 2020 2074 6162 6c65 2e63 7265 6174       table.creat
+00005ba0: 655f 696e 6465 7828 2763 2729 0a0a 2020  e_index('c')..  
+00005bb0: 2020 2020 2020 6368 6169 6e65 645f 7461        chained_ta
+00005bc0: 626c 6520 3d20 7461 626c 652e 6279 2e62  ble = table.by.b
+00005bd0: 5b27 4127 5d2e 6279 2e63 5b27 4327 5d0a  ['A'].by.c['C'].
+00005be0: 2020 2020 2020 2020 666f 7220 7265 6320          for rec 
+00005bf0: 696e 2063 6861 696e 6564 5f74 6162 6c65  in chained_table
+00005c00: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00005c10: 696e 7428 7265 6329 0a0a 2020 2020 2020  int(rec)..      
+00005c20: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005c30: 616c 2874 6573 745f 7369 7a65 2c20 6c65  al(test_size, le
+00005c40: 6e28 6368 6169 6e65 645f 7461 626c 6529  n(chained_table)
+00005c50: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00005c60: 7061 7273 655f 6461 7465 7469 6d65 5f74  parse_datetime_t
+00005c70: 7261 6e73 666f 726d 2873 656c 6629 3a0a  ransform(self):.
+00005c80: 2020 2020 2020 2020 696d 706f 7274 2064          import d
+00005c90: 6174 6574 696d 650a 0a20 2020 2020 2020  atetime..       
+00005ca0: 2064 6174 6120 3d20 7465 7874 7772 6170   data = textwrap
+00005cb0: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+00005cc0: 2020 2020 2061 2c62 2c63 0a20 2020 2020       a,b,c.     
+00005cd0: 2020 2032 3030 312d 3031 2d30 3120 3030     2001-01-01 00
+00005ce0: 3a33 343a 3536 2c41 2c31 3030 0a20 2020  :34:56,A,100.   
+00005cf0: 2020 2020 2032 3030 312d 3031 2d30 3220       2001-01-02 
+00005d00: 3031 3a33 343a 3536 2c42 2c31 3031 0a20  01:34:56,B,101. 
+00005d10: 2020 2020 2020 2032 3030 312d 3032 2d33         2001-02-3
+00005d20: 3020 3032 3a33 343a 3536 2c43 2c31 3032  0 02:34:56,C,102
+00005d30: 0a20 2020 2020 2020 202c 442c 3130 330a  .        ,D,103.
+00005d40: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
+00005d50: 2020 2020 2074 6573 745f 6b77 6172 6773       test_kwargs
+00005d60: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00005d70: 207b 2765 6d70 7479 273a 2027 272c 2027   {'empty': '', '
+00005d80: 6f6e 5f65 7272 6f72 273a 204e 6f6e 657d  on_error': None}
+00005d90: 2c0a 2020 2020 2020 2020 2020 2020 7b27  ,.            {'
+00005da0: 656d 7074 7927 3a20 274e 2f41 272c 2027  empty': 'N/A', '
+00005db0: 6f6e 5f65 7272 6f72 273a 2064 6174 6574  on_error': datet
+00005dc0: 696d 652e 6461 7465 7469 6d65 2e6d 696e  ime.datetime.min
+00005dd0: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
+00005de0: 2765 6d70 7479 273a 2064 6174 6574 696d  'empty': datetim
+00005df0: 652e 6461 7465 7469 6d65 2e6d 696e 2c20  e.datetime.min, 
+00005e00: 276f 6e5f 6572 726f 7227 3a20 2727 7d2c  'on_error': ''},
+00005e10: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00005e20: 2020 2066 6f72 206b 7761 7267 7320 696e     for kwargs in
+00005e30: 2074 6573 745f 6b77 6172 6773 3a0a 2020   test_kwargs:.  
+00005e40: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
+00005e50: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00005e60: 6d70 6f72 7428 6461 7461 2c0a 2020 2020  mport(data,.    
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e90: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
+00005ea0: 2761 273a 206c 742e 5461 626c 652e 7061  'a': lt.Table.pa
+00005eb0: 7273 655f 6461 7465 7469 6d65 2827 2559  rse_datetime('%Y
+00005ec0: 2d25 6d2d 2564 2025 483a 254d 3a25 5327  -%m-%d %H:%M:%S'
+00005ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 202a 2a6b 7761 7267 7329 7d29 0a20     **kwargs)}). 
+00005f30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00005f40: 285b 7374 7228 6129 2066 6f72 2061 2069  ([str(a) for a i
+00005f50: 6e20 7462 6c2e 616c 6c2e 615d 290a 0a20  n tbl.all.a]).. 
+00005f60: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00005f70: 7365 6c66 2e73 7562 5465 7374 2822 7465  self.subTest("te
+00005f80: 7374 2054 6162 6c65 2e70 6172 7365 5f64  st Table.parse_d
+00005f90: 6174 655f 7469 6d65 2065 7272 6f72 7322  ate_time errors"
+00005fa0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00005fb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005fc0: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 205b 6b77 6172 6773 5b22 6f6e 5f65     [kwargs["on_e
+00005ff0: 7272 6f72 225d 2c20 6b77 6172 6773 5b22  rror"], kwargs["
+00006000: 656d 7074 7922 5d5d 2c0a 2020 2020 2020  empty"]],.      
+00006010: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00006020: 7374 2874 626c 2e61 6c6c 2e61 295b 2d32  st(tbl.all.a)[-2
+00006030: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
+00006040: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00006050: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00006060: 6573 7428 2274 6573 7420 5461 626c 652e  est("test Table.
+00006070: 7061 7273 655f 6461 7465 5f74 696d 6520  parse_date_time 
+00006080: 7661 6c69 6422 2c20 2a2a 6b77 6172 6773  valid", **kwargs
+00006090: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000060a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000060b0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+000060c0: 2020 2020 2020 2020 205b 6461 7465 7469           [dateti
+000060d0: 6d65 2e64 6174 6574 696d 6528 3230 3031  me.datetime(2001
+000060e0: 2c20 312c 2031 2c20 302c 2033 342c 2035  , 1, 1, 0, 34, 5
+000060f0: 3629 2c0a 2020 2020 2020 2020 2020 2020  6),.            
+00006100: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
+00006110: 652e 6461 7465 7469 6d65 2832 3030 312c  e.datetime(2001,
+00006120: 2031 2c20 322c 2031 2c20 3334 2c20 3536   1, 2, 1, 34, 56
+00006130: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+00006140: 2020 2020 2020 2020 6c69 7374 2874 626c          list(tbl
+00006150: 2e61 6c6c 2e61 295b 3a32 5d0a 2020 2020  .all.a)[:2].    
+00006160: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00006170: 2020 2064 6566 2074 6573 745f 7061 7273     def test_pars
+00006180: 655f 6461 7465 5f74 7261 6e73 666f 726d  e_date_transform
+00006190: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000061a0: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
+000061b0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000061c0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+000061d0: 2222 225c 0a20 2020 2020 2020 2061 2c62  """\.        a,b
+000061e0: 2c63 0a20 2020 2020 2020 2032 3030 312d  ,c.        2001-
+000061f0: 3031 2d30 3120 3030 3a33 343a 3536 2c41  01-01 00:34:56,A
+00006200: 2c31 3030 0a20 2020 2020 2020 2032 3030  ,100.        200
+00006210: 312d 3031 2d30 3220 3031 3a33 343a 3536  1-01-02 01:34:56
+00006220: 2c42 2c31 3031 0a20 2020 2020 2020 2032  ,B,101.        2
+00006230: 3030 312d 3032 2d33 3020 3032 3a33 343a  001-02-30 02:34:
+00006240: 3536 2c43 2c31 3032 0a20 2020 2020 2020  56,C,102.       
+00006250: 202c 442c 3130 330a 2020 2020 2020 2020   ,D,103.        
+00006260: 2222 2229 0a20 2020 2020 2020 2074 6573  """).        tes
+00006270: 745f 6b77 6172 6773 203d 205b 0a20 2020  t_kwargs = [.   
+00006280: 2020 2020 2020 2020 207b 2765 6d70 7479           {'empty
+00006290: 273a 2027 272c 2027 6f6e 5f65 7272 6f72  ': '', 'on_error
+000062a0: 273a 204e 6f6e 657d 2c0a 2020 2020 2020  ': None},.      
+000062b0: 2020 2020 2020 7b27 656d 7074 7927 3a20        {'empty': 
+000062c0: 274e 2f41 272c 2027 6f6e 5f65 7272 6f72  'N/A', 'on_error
+000062d0: 273a 2064 6174 6574 696d 652e 6461 7465  ': datetime.date
+000062e0: 2e6d 696e 7d2c 0a20 2020 2020 2020 2020  .min},.         
+000062f0: 2020 207b 2765 6d70 7479 273a 2064 6174     {'empty': dat
+00006300: 6574 696d 652e 6461 7465 2e6d 696e 2c20  etime.date.min, 
+00006310: 276f 6e5f 6572 726f 7227 3a20 2727 7d2c  'on_error': ''},
+00006320: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00006330: 2020 2066 6f72 206b 7761 7267 7320 696e     for kwargs in
+00006340: 2074 6573 745f 6b77 6172 6773 3a0a 2020   test_kwargs:.  
+00006350: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
+00006360: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00006370: 6d70 6f72 7428 6461 7461 2c0a 2020 2020  mport(data,.    
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
+000063b0: 2761 273a 206c 742e 5461 626c 652e 7061  'a': lt.Table.pa
+000063c0: 7273 655f 6461 7465 2827 2559 2d25 6d2d  rse_date('%Y-%m-
+000063d0: 2564 2025 483a 254d 3a25 5327 2c0a 2020  %d %H:%M:%S',.  
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00006430: 7267 7329 7d29 0a20 2020 2020 2020 2020  rgs)}).         
+00006440: 2020 2070 7269 6e74 285b 7374 7228 6129     print([str(a)
+00006450: 2066 6f72 2061 2069 6e20 7462 6c2e 616c   for a in tbl.al
+00006460: 6c2e 615d 290a 0a20 2020 2020 2020 2020  l.a])..         
+00006470: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00006480: 5465 7374 2822 7465 7374 2054 6162 6c65  Test("test Table
+00006490: 2e70 6172 7365 5f64 6174 655f 7469 6d65  .parse_date_time
+000064a0: 2065 7272 6f72 7322 2c20 2a2a 6b77 6172   errors", **kwar
+000064b0: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
+000064c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000064d0: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+000064e0: 2020 2020 2020 2020 2020 205b 6b77 6172             [kwar
+000064f0: 6773 5b22 6f6e 5f65 7272 6f72 225d 2c20  gs["on_error"], 
+00006500: 6b77 6172 6773 5b22 656d 7074 7922 5d5d  kwargs["empty"]]
+00006510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006520: 2020 2020 2020 6c69 7374 2874 626c 2e61        list(tbl.a
+00006530: 6c6c 2e61 295b 2d32 3a5d 0a20 2020 2020  ll.a)[-2:].     
+00006540: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00006550: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00006560: 656c 662e 7375 6254 6573 7428 2274 6573  elf.subTest("tes
+00006570: 7420 5461 626c 652e 7061 7273 655f 6461  t Table.parse_da
+00006580: 7465 5f74 696d 6520 7661 6c69 6422 2c20  te_time valid", 
+00006590: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+000065a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000065b0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
+000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065d0: 205b 6461 7465 7469 6d65 2e64 6174 6528   [datetime.date(
+000065e0: 3230 3031 2c20 312c 2031 292c 0a20 2020  2001, 1, 1),.   
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006600: 2020 6461 7465 7469 6d65 2e64 6174 6528    datetime.date(
+00006610: 3230 3031 2c20 312c 2032 295d 2c0a 2020  2001, 1, 2)],.  
 00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2027 7069 6563 6573 273a 2069 6e74     'pieces': int
-00006640: 7d0a 2020 2020 2020 2020 6461 7461 203d  }.        data =
-00006650: 206c 742e 5461 626c 6528 6622 5072 6f63   lt.Table(f"Proc
-00006660: 6573 7320 7374 6570 2065 6c61 7073 6564  ess step elapsed
-00006670: 2074 696d 6573 2229 2e63 7376 5f69 6d70   times").csv_imp
-00006680: 6f72 7428 7072 6f63 6573 735f 6461 7461  ort(process_data
-00006690: 2c20 7472 616e 7366 6f72 6d73 3d74 7261  , transforms=tra
-000066a0: 6e73 666f 726d 7329 0a20 2020 2020 2020  nsforms).       
-000066b0: 2064 6174 612e 6372 6561 7465 5f69 6e64   data.create_ind
-000066c0: 6578 2822 656c 6170 7365 645f 7469 6d65  ex("elapsed_time
-000066d0: 2229 0a0a 2020 2020 2020 2020 5f30 305f  ")..        _00_
-000066e0: 3031 5f33 3020 3d20 6461 7465 7469 6d65  01_30 = datetime
-000066f0: 2e74 696d 6564 656c 7461 2873 6563 6f6e  .timedelta(secon
-00006700: 6473 3d39 3029 0a20 2020 2020 2020 2073  ds=90).        s
-00006710: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00006720: 332c 2073 756d 2864 6174 612e 6279 2e65  3, sum(data.by.e
-00006730: 6c61 7073 6564 5f74 696d 655b 3a5f 3030  lapsed_time[:_00
-00006740: 5f30 315f 3330 5d2e 616c 6c2e 7069 6563  _01_30].all.piec
-00006750: 6573 2929 0a0a 2020 2020 6465 6620 7465  es))..    def te
-00006760: 7374 5f73 6c69 6365 645f 696e 6465 7869  st_sliced_indexi
-00006770: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
-00006780: 2020 7472 616e 7366 6f72 6d73 203d 207b    transforms = {
-00006790: 0a20 2020 2020 2020 2020 2020 2027 706f  .            'po
-000067a0: 7027 3a20 696e 742c 0a20 2020 2020 2020  p': int,.       
-000067b0: 2020 2020 2027 656c 6576 273a 2069 6e74       'elev': int
-000067c0: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
-000067d0: 6174 273a 2066 6c6f 6174 2c0a 2020 2020  at': float,.    
-000067e0: 2020 2020 2020 2020 276c 6f6e 6727 3a20          'long': 
-000067f0: 666c 6f61 742c 0a20 2020 2020 2020 207d  float,.        }
-00006800: 0a20 2020 2020 2020 2075 735f 7070 6c20  .        us_ppl 
-00006810: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00006820: 5f69 6d70 6f72 7428 2265 7861 6d70 6c65  _import("example
-00006830: 732f 7573 5f70 706c 2e63 7376 222c 0a20  s/us_ppl.csv",. 
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-00006870: 3d74 7261 6e73 666f 726d 732c 0a20 2020  =transforms,.   
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 292e 7365 6c65 6374 2822 6964      ).select("id
-000068b0: 206e 616d 6520 656c 6576 206c 6174 206c   name elev lat l
-000068c0: 6f6e 6720 706f 7022 290a 2020 2020 2020  ong pop").      
-000068d0: 2020 7072 696e 7428 7573 5f70 706c 2e69    print(us_ppl.i
-000068e0: 6e66 6f28 2929 0a20 2020 2020 2020 2075  nfo()).        u
-000068f0: 735f 7070 6c2e 6372 6561 7465 5f69 6e64  s_ppl.create_ind
-00006900: 6578 2822 6e61 6d65 2229 0a20 2020 2020  ex("name").     
-00006910: 2020 2075 735f 7070 6c2e 6372 6561 7465     us_ppl.create
-00006920: 5f69 6e64 6578 2822 656c 6576 2229 0a0a  _index("elev")..
-00006930: 2020 2020 2020 2020 7465 7374 203d 2022          test = "
-00006940: 656c 6576 203c 2030 220a 2020 2020 2020  elev < 0".      
-00006950: 2020 6c6f 775f 7070 6c5f 7768 6572 6520    low_ppl_where 
-00006960: 3d20 7573 5f70 706c 2e77 6865 7265 2865  = us_ppl.where(e
-00006970: 6c65 763d 6c74 2e54 6162 6c65 2e6c 7428  lev=lt.Table.lt(
-00006980: 3029 2928 7465 7374 290a 2020 2020 2020  0))(test).      
-00006990: 2020 6c6f 775f 7070 6c5f 736c 6963 6520    low_ppl_slice 
-000069a0: 3d20 7573 5f70 706c 2e62 792e 656c 6576  = us_ppl.by.elev
-000069b0: 5b3a 305d 2866 227b 7465 7374 7d20 2873  [:0](f"{test} (s
-000069c0: 6c69 6365 6429 2229 0a20 2020 2020 2020  liced)").       
-000069d0: 206c 6f77 5f70 706c 5f73 6c69 6365 2e70   low_ppl_slice.p
-000069e0: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-000069f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00006a00: 6c28 6c69 7374 286c 6f77 5f70 706c 5f77  l(list(low_ppl_w
-00006a10: 6865 7265 2e61 6c6c 2e69 6429 2c20 6c69  here.all.id), li
-00006a20: 7374 286c 6f77 5f70 706c 5f73 6c69 6365  st(low_ppl_slice
-00006a30: 2e61 6c6c 2e69 6429 290a 0a20 2020 2020  .all.id))..     
-00006a40: 2020 2074 6573 7420 3d20 2265 6c65 7620     test = "elev 
-00006a50: 3e3d 2031 3030 3022 0a20 2020 2020 2020  >= 1000".       
-00006a60: 2068 695f 7070 6c5f 7768 6572 6520 3d20   hi_ppl_where = 
-00006a70: 7573 5f70 706c 2e77 6865 7265 2865 6c65  us_ppl.where(ele
-00006a80: 763d 6c74 2e54 6162 6c65 2e67 6528 3130  v=lt.Table.ge(10
-00006a90: 3030 2929 2874 6573 7429 0a20 2020 2020  00))(test).     
-00006aa0: 2020 2068 695f 7070 6c5f 736c 6963 6520     hi_ppl_slice 
-00006ab0: 3d20 7573 5f70 706c 2e62 792e 656c 6576  = us_ppl.by.elev
-00006ac0: 5b31 3030 303a 5d28 6622 7b74 6573 747d  [1000:](f"{test}
-00006ad0: 2028 736c 6963 6564 2922 290a 2020 2020   (sliced)").    
-00006ae0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00006af0: 7175 616c 286c 6973 7428 6869 5f70 706c  qual(list(hi_ppl
-00006b00: 5f77 6865 7265 2e61 6c6c 2e69 6429 2c20  _where.all.id), 
-00006b10: 6c69 7374 2868 695f 7070 6c5f 736c 6963  list(hi_ppl_slic
-00006b20: 652e 616c 6c2e 6964 2929 0a0a 2020 2020  e.all.id))..    
-00006b30: 2020 2020 7465 7374 203d 2022 3020 3c3d      test = "0 <=
-00006b40: 2065 6c65 7620 3c20 3130 3022 0a20 2020   elev < 100".   
-00006b50: 2020 2020 206c 6f77 5f70 706c 5f77 6865       low_ppl_whe
-00006b60: 7265 203d 2075 735f 7070 6c2e 7768 6572  re = us_ppl.wher
-00006b70: 6528 656c 6576 3d6c 742e 5461 626c 652e  e(elev=lt.Table.
-00006b80: 6765 2830 2929 2e77 6865 7265 2865 6c65  ge(0)).where(ele
-00006b90: 763d 6c74 2e54 6162 6c65 2e6c 7428 3130  v=lt.Table.lt(10
-00006ba0: 3029 2928 7465 7374 290a 2020 2020 2020  0))(test).      
-00006bb0: 2020 6c6f 775f 7070 6c5f 736c 6963 6520    low_ppl_slice 
-00006bc0: 3d20 7573 5f70 706c 2e62 792e 656c 6576  = us_ppl.by.elev
-00006bd0: 5b30 3a31 3030 5d28 6622 7b74 6573 747d  [0:100](f"{test}
-00006be0: 2028 736c 6963 6564 2922 290a 2020 2020   (sliced)").    
-00006bf0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00006c00: 7175 616c 286c 6973 7428 6c6f 775f 7070  qual(list(low_pp
-00006c10: 6c5f 7768 6572 652e 616c 6c2e 6964 292c  l_where.all.id),
-00006c20: 206c 6973 7428 6c6f 775f 7070 6c5f 736c   list(low_ppl_sl
-00006c30: 6963 652e 616c 6c2e 6964 2929 0a0a 2020  ice.all.id))..  
-00006c40: 2020 2020 2020 615f 7070 6c5f 7768 6572        a_ppl_wher
-00006c50: 6520 3d20 7573 5f70 706c 2e77 6865 7265  e = us_ppl.where
-00006c60: 286e 616d 653d 6c74 2e54 6162 6c65 2e67  (name=lt.Table.g
-00006c70: 6528 2241 2229 292e 7768 6572 6528 6e61  e("A")).where(na
-00006c80: 6d65 3d6c 742e 5461 626c 652e 6c74 2822  me=lt.Table.lt("
-00006c90: 4322 2929 0a20 2020 2020 2020 2061 5f70  C")).        a_p
-00006ca0: 706c 5f73 6c69 6365 203d 2075 735f 7070  pl_slice = us_pp
-00006cb0: 6c2e 6279 2e6e 616d 655b 2241 223a 2243  l.by.name["A":"C
-00006cc0: 225d 0a20 2020 2020 2020 2073 656c 662e  "].        self.
-00006cd0: 6173 7365 7274 4571 7561 6c28 6c69 7374  assertEqual(list
-00006ce0: 2861 5f70 706c 5f77 6865 7265 2e61 6c6c  (a_ppl_where.all
-00006cf0: 2e69 6429 2c20 6c69 7374 2861 5f70 706c  .id), list(a_ppl
-00006d00: 5f73 6c69 6365 2e61 6c6c 2e69 6429 290a  _slice.all.id)).
-00006d10: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
-00006d20: 6e5f 696e 7465 6765 725f 736c 6963 6564  n_integer_sliced
-00006d30: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
-00006d40: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00006d50: 6461 7465 7469 6d65 0a0a 2020 2020 2020  datetime..      
-00006d60: 2020 7361 6c65 735f 6461 7461 203d 2074    sales_data = t
-00006d70: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
-00006d80: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
-00006d90: 6461 7465 2c63 7573 746f 6d65 722c 736b  date,customer,sk
-00006da0: 752c 7174 790a 2020 2020 2020 2020 2020  u,qty.          
-00006db0: 2020 3230 3030 2f30 312f 3031 2c30 3032    2000/01/01,002
-00006dc0: 302c 414e 5649 4c2d 3030 312c 310a 2020  0,ANVIL-001,1.  
-00006dd0: 2020 2020 2020 2020 2020 3230 3030 2f30            2000/0
-00006de0: 312f 3031 2c30 3032 302c 4252 4453 442d  1/01,0020,BRDSD-
-00006df0: 3030 312c 320a 2020 2020 2020 2020 2020  001,2.          
-00006e00: 2020 3230 3030 2f30 322f 3135 2c30 3032    2000/02/15,002
-00006e10: 302c 4252 4453 442d 3030 312c 340a 2020  0,BRDSD-001,4.  
-00006e20: 2020 2020 2020 2020 2020 3230 3030 2f30            2000/0
-00006e30: 332f 3331 2c30 3032 302c 4252 4453 442d  3/31,0020,BRDSD-
-00006e40: 3030 312c 380a 2020 2020 2020 2020 2020  001,8.          
-00006e50: 2020 3230 3030 2f30 332f 3331 2c30 3032    2000/03/31,002
-00006e60: 302c 4d41 474e 542d 3030 312c 3136 0a20  0,MAGNT-001,16. 
-00006e70: 2020 2020 2020 2020 2020 2032 3030 302f             2000/
-00006e80: 3034 2f30 312c 3030 3230 2c52 4f42 4f54  04/01,0020,ROBOT
-00006e90: 2d30 3031 2c33 320a 2020 2020 2020 2020  -001,32.        
-00006ea0: 2020 2020 3230 3030 2f30 342f 3135 2c30      2000/04/15,0
-00006eb0: 3032 302c 4252 4453 442d 3030 312c 3634  020,BRDSD-001,64
-00006ec0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-00006ed0: 290a 0a20 2020 2020 2020 2074 7261 6e73  )..        trans
-00006ee0: 666f 726d 7320 3d20 7b27 6461 7465 273a  forms = {'date':
-00006ef0: 206c 742e 5461 626c 652e 7061 7273 655f   lt.Table.parse_
-00006f00: 6461 7465 2822 2559 2f25 6d2f 2564 2229  date("%Y/%m/%d")
-00006f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006f20: 2020 2020 2020 2020 2771 7479 273a 2069          'qty': i
-00006f30: 6e74 7d0a 2020 2020 2020 2020 7361 6c65  nt}.        sale
-00006f40: 7320 3d20 6c74 2e54 6162 6c65 2829 2e63  s = lt.Table().c
-00006f50: 7376 5f69 6d70 6f72 7428 7361 6c65 735f  sv_import(sales_
-00006f60: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-00006f90: 7366 6f72 6d73 3d74 7261 6e73 666f 726d  sforms=transform
-00006fa0: 732c 290a 0a20 2020 2020 2020 2073 616c  s,)..        sal
-00006fb0: 6573 2e63 7265 6174 655f 696e 6465 7828  es.create_index(
-00006fc0: 2264 6174 6522 290a 2020 2020 2020 2020  "date").        
-00006fd0: 6a61 6e5f 3031 203d 2064 6174 6574 696d  jan_01 = datetim
-00006fe0: 652e 6461 7465 2832 3030 302c 2031 2c20  e.date(2000, 1, 
-00006ff0: 3129 0a20 2020 2020 2020 2061 7072 5f30  1).        apr_0
-00007000: 3120 3d20 6461 7465 7469 6d65 2e64 6174  1 = datetime.dat
-00007010: 6528 3230 3030 2c20 342c 2031 290a 2020  e(2000, 4, 1).  
-00007020: 2020 2020 2020 6669 7273 745f 7174 725f        first_qtr_
-00007030: 7361 6c65 7320 3d20 7361 6c65 732e 6279  sales = sales.by
-00007040: 2e64 6174 655b 6a61 6e5f 3031 3a20 6170  .date[jan_01: ap
-00007050: 725f 3031 5d0a 2020 2020 2020 2020 6669  r_01].        fi
-00007060: 7273 745f 7174 725f 7361 6c65 732e 7072  rst_qtr_sales.pr
-00007070: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-00007080: 7072 696e 7428 6c69 7374 2866 6972 7374  print(list(first
-00007090: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
-000070a0: 6b75 2929 0a0a 2020 2020 2020 2020 7365  ku))..        se
-000070b0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-000070c0: 6973 7428 6669 7273 745f 7174 725f 7361  ist(first_qtr_sa
-000070d0: 6c65 732e 616c 6c2e 736b 7529 2c0a 2020  les.all.sku),.  
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 2020 2020 205b 2741 4e56 494c 2d30         ['ANVIL-0
-00007100: 3031 272c 2027 4252 4453 442d 3030 3127  01', 'BRDSD-001'
-00007110: 2c20 2742 5244 5344 2d30 3031 272c 2027  , 'BRDSD-001', '
-00007120: 4252 4453 442d 3030 3127 2c20 274d 4147  BRDSD-001', 'MAG
-00007130: 4e54 2d30 3031 275d 2c0a 2020 2020 2020  NT-001'],.      
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00007160: 662e 6173 7365 7274 4571 7561 6c28 3331  f.assertEqual(31
-00007170: 2c20 7375 6d28 6669 7273 745f 7174 725f  , sum(first_qtr_
-00007180: 7361 6c65 732e 616c 6c2e 7174 7929 290a  sales.all.qty)).
-00007190: 0a20 2020 2020 2020 2023 2075 7365 2064  .        # use d
-000071a0: 6174 6520 7374 7269 6e67 7320 6173 2072  ate strings as r
-000071b0: 616e 6765 2076 616c 7565 730a 2020 2020  ange values.    
-000071c0: 2020 2020 7472 616e 7366 6f72 6d73 203d      transforms =
-000071d0: 207b 2771 7479 273a 2069 6e74 7d0a 2020   {'qty': int}.  
-000071e0: 2020 2020 2020 7361 6c65 7320 3d20 6c74        sales = lt
-000071f0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-00007200: 6f72 7428 7361 6c65 735f 6461 7461 2c0a  ort(sales_data,.
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-00007240: 3d74 7261 6e73 666f 726d 732c 290a 0a20  =transforms,).. 
-00007250: 2020 2020 2020 2073 616c 6573 2e63 7265         sales.cre
-00007260: 6174 655f 696e 6465 7828 2264 6174 6522  ate_index("date"
-00007270: 290a 2020 2020 2020 2020 6669 7273 745f  ).        first_
-00007280: 7174 725f 7361 6c65 7320 3d20 7361 6c65  qtr_sales = sale
-00007290: 732e 6279 2e64 6174 655b 2232 3030 302f  s.by.date["2000/
-000072a0: 3031 2f30 3122 3a20 2232 3030 302f 3034  01/01": "2000/04
-000072b0: 2f30 3122 5d0a 2020 2020 2020 2020 6669  /01"].        fi
-000072c0: 7273 745f 7174 725f 7361 6c65 732e 7072  rst_qtr_sales.pr
-000072d0: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-000072e0: 7072 696e 7428 6c69 7374 2866 6972 7374  print(list(first
-000072f0: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
-00007300: 6b75 2929 0a0a 2020 2020 2020 2020 7365  ku))..        se
-00007310: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00007320: 6973 7428 6669 7273 745f 7174 725f 7361  ist(first_qtr_sa
-00007330: 6c65 732e 616c 6c2e 736b 7529 2c0a 2020  les.all.sku),.  
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 2020 205b 2741 4e56 494c 2d30         ['ANVIL-0
-00007360: 3031 272c 2027 4252 4453 442d 3030 3127  01', 'BRDSD-001'
-00007370: 2c20 2742 5244 5344 2d30 3031 272c 2027  , 'BRDSD-001', '
-00007380: 4252 4453 442d 3030 3127 2c20 274d 4147  BRDSD-001', 'MAG
-00007390: 4e54 2d30 3031 275d 2c0a 2020 2020 2020  NT-001'],.      
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-000073c0: 662e 6173 7365 7274 4571 7561 6c28 3331  f.assertEqual(31
-000073d0: 2c20 7375 6d28 6669 7273 745f 7174 725f  , sum(first_qtr_
-000073e0: 7361 6c65 732e 616c 6c2e 7174 7929 290a  sales.all.qty)).
-000073f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00007400: 7365 7274 4571 7561 6c28 3331 2c20 7375  sertEqual(31, su
-00007410: 6d28 7361 6c65 732e 6279 2e64 6174 655b  m(sales.by.date[
-00007420: 3a22 3230 3030 2f30 342f 3031 225d 2e61  :"2000/04/01"].a
-00007430: 6c6c 2e71 7479 2929 0a20 2020 2020 2020  ll.qty)).       
-00007440: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007450: 6c28 3936 2c20 7375 6d28 7361 6c65 732e  l(96, sum(sales.
-00007460: 6279 2e64 6174 655b 2232 3030 302f 3034  by.date["2000/04
-00007470: 2f30 3122 3a5d 2e61 6c6c 2e71 7479 2929  /01":].all.qty))
-00007480: 0a0a 2020 2020 6465 6620 7465 7374 5f69  ..    def test_i
-00007490: 6e64 6578 5f64 6972 2873 656c 6629 3a0a  ndex_dir(self):.
-000074a0: 2020 2020 2020 2020 6368 6172 7320 3d20          chars = 
-000074b0: 2241 4243 4445 4647 4849 4a4b 4c4d 4e4f  "ABCDEFGHIJKLMNO
-000074c0: 5051 5253 5455 5657 5859 5a22 0a20 2020  PQRSTUVWXYZ".   
-000074d0: 2020 2020 206d 616b 655f 7265 6320 3d20       make_rec = 
-000074e0: 6c61 6d62 6461 2061 612c 2062 622c 2063  lambda aa, bb, c
-000074f0: 633a 2073 656c 662e 6d61 6b65 5f64 6174  c: self.make_dat
-00007500: 615f 6f62 6a65 6374 2863 6861 7273 5b61  a_object(chars[a
-00007510: 6120 2520 6c65 6e28 6368 6172 7329 5d2c  a % len(chars)],
-00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006630: 2020 6c69 7374 2874 626c 2e61 6c6c 2e61    list(tbl.all.a
+00006640: 295b 3a32 5d0a 2020 2020 2020 2020 2020  )[:2].          
+00006650: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00006660: 2074 6573 745f 7061 7273 655f 7469 6d65   test_parse_time
+00006670: 6465 6c74 615f 7472 616e 7366 6f72 6d28  delta_transform(
+00006680: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00006690: 6d70 6f72 7420 6461 7465 7469 6d65 0a0a  mport datetime..
+000066a0: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
+000066b0: 6461 7461 203d 2074 6578 7477 7261 702e  data = textwrap.
+000066c0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+000066d0: 2020 2020 2020 2020 656c 6170 7365 645f          elapsed_
+000066e0: 7469 6d65 2c65 7170 742c 6576 656e 742c  time,eqpt,event,
+000066f0: 6c6f 742c 7069 6563 6573 0a20 2020 2020  lot,pieces.     
+00006700: 2020 2020 2020 2030 3a30 303a 3030 2c44         0:00:00,D
+00006710: 5249 4c4c 3031 2c4c 6f74 5374 6172 742c  RILL01,LotStart,
+00006720: 5043 4231 3436 2c31 0a20 2020 2020 2020  PCB146,1.       
+00006730: 2020 2020 2030 3a30 303a 3430 2c44 5249       0:00:40,DRI
+00006740: 4c4c 3031 2c54 6f6f 6c31 2c50 4342 3134  LL01,Tool1,PCB14
+00006750: 362c 320a 2020 2020 2020 2020 2020 2020  6,2.            
+00006760: 303a 3033 3a34 352c 4452 494c 4c30 312c  0:03:45,DRILL01,
+00006770: 546f 6f6c 322c 5043 4231 3436 2c34 0a20  Tool2,PCB146,4. 
+00006780: 2020 2020 2020 2020 2020 2030 3a30 363a             0:06:
+00006790: 3136 2c44 5249 4c4c 3031 2c4c 6f74 456e  16,DRILL01,LotEn
+000067a0: 642c 5043 4231 3436 2c38 0a20 2020 2020  d,PCB146,8.     
+000067b0: 2020 2020 2020 2022 2222 290a 0a20 2020         """)..   
+000067c0: 2020 2020 2074 7261 6e73 666f 726d 7320       transforms 
+000067d0: 3d20 7b27 656c 6170 7365 645f 7469 6d65  = {'elapsed_time
+000067e0: 273a 206c 742e 5461 626c 652e 7061 7273  ': lt.Table.pars
+000067f0: 655f 7469 6d65 6465 6c74 6128 2225 483a  e_timedelta("%H:
+00006800: 254d 3a25 5322 292c 0a20 2020 2020 2020  %M:%S"),.       
+00006810: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006820: 7069 6563 6573 273a 2069 6e74 7d0a 2020  pieces': int}.  
+00006830: 2020 2020 2020 6461 7461 203d 206c 742e        data = lt.
+00006840: 5461 626c 6528 6622 5072 6f63 6573 7320  Table(f"Process 
+00006850: 7374 6570 2065 6c61 7073 6564 2074 696d  step elapsed tim
+00006860: 6573 2229 2e63 7376 5f69 6d70 6f72 7428  es").csv_import(
+00006870: 7072 6f63 6573 735f 6461 7461 2c20 7472  process_data, tr
+00006880: 616e 7366 6f72 6d73 3d74 7261 6e73 666f  ansforms=transfo
+00006890: 726d 7329 0a20 2020 2020 2020 2064 6174  rms).        dat
+000068a0: 612e 6372 6561 7465 5f69 6e64 6578 2822  a.create_index("
+000068b0: 656c 6170 7365 645f 7469 6d65 2229 0a0a  elapsed_time")..
+000068c0: 2020 2020 2020 2020 5f30 305f 3031 5f33          _00_01_3
+000068d0: 3020 3d20 6461 7465 7469 6d65 2e74 696d  0 = datetime.tim
+000068e0: 6564 656c 7461 2873 6563 6f6e 6473 3d39  edelta(seconds=9
+000068f0: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+00006900: 6173 7365 7274 4571 7561 6c28 332c 2073  assertEqual(3, s
+00006910: 756d 2864 6174 612e 6279 2e65 6c61 7073  um(data.by.elaps
+00006920: 6564 5f74 696d 655b 3a5f 3030 5f30 315f  ed_time[:_00_01_
+00006930: 3330 5d2e 616c 6c2e 7069 6563 6573 2929  30].all.pieces))
+00006940: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+00006950: 6c69 6365 645f 696e 6465 7869 6e67 2873  liced_indexing(s
+00006960: 656c 6629 3a0a 2020 2020 2020 2020 7472  elf):.        tr
+00006970: 616e 7366 6f72 6d73 203d 207b 0a20 2020  ansforms = {.   
+00006980: 2020 2020 2020 2020 2027 706f 7027 3a20           'pop': 
+00006990: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
+000069a0: 2027 656c 6576 273a 2069 6e74 2c0a 2020   'elev': int,.  
+000069b0: 2020 2020 2020 2020 2020 276c 6174 273a            'lat':
+000069c0: 2066 6c6f 6174 2c0a 2020 2020 2020 2020   float,.        
+000069d0: 2020 2020 276c 6f6e 6727 3a20 666c 6f61      'long': floa
+000069e0: 742c 0a20 2020 2020 2020 207d 0a20 2020  t,.        }.   
+000069f0: 2020 2020 2075 735f 7070 6c20 3d20 6c74       us_ppl = lt
+00006a00: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+00006a10: 6f72 7428 2265 7861 6d70 6c65 732f 7573  ort("examples/us
+00006a20: 5f70 706c 2e63 7376 222c 0a20 2020 2020  _ppl.csv",.     
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 7472 616e 7366 6f72 6d73 3d74 7261    transforms=tra
+00006a60: 6e73 666f 726d 732c 0a20 2020 2020 2020  nsforms,.       
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a90: 292e 7365 6c65 6374 2822 6964 206e 616d  ).select("id nam
+00006aa0: 6520 656c 6576 206c 6174 206c 6f6e 6720  e elev lat long 
+00006ab0: 706f 7022 290a 2020 2020 2020 2020 7072  pop").        pr
+00006ac0: 696e 7428 7573 5f70 706c 2e69 6e66 6f28  int(us_ppl.info(
+00006ad0: 2929 0a20 2020 2020 2020 2075 735f 7070  )).        us_pp
+00006ae0: 6c2e 6372 6561 7465 5f69 6e64 6578 2822  l.create_index("
+00006af0: 6e61 6d65 2229 0a20 2020 2020 2020 2075  name").        u
+00006b00: 735f 7070 6c2e 6372 6561 7465 5f69 6e64  s_ppl.create_ind
+00006b10: 6578 2822 656c 6576 2229 0a0a 2020 2020  ex("elev")..    
+00006b20: 2020 2020 7465 7374 203d 2022 656c 6576      test = "elev
+00006b30: 203c 2030 220a 2020 2020 2020 2020 6c6f   < 0".        lo
+00006b40: 775f 7070 6c5f 7768 6572 6520 3d20 7573  w_ppl_where = us
+00006b50: 5f70 706c 2e77 6865 7265 2865 6c65 763d  _ppl.where(elev=
+00006b60: 6c74 2e54 6162 6c65 2e6c 7428 3029 2928  lt.Table.lt(0))(
+00006b70: 7465 7374 290a 2020 2020 2020 2020 6c6f  test).        lo
+00006b80: 775f 7070 6c5f 736c 6963 6520 3d20 7573  w_ppl_slice = us
+00006b90: 5f70 706c 2e62 792e 656c 6576 5b3a 305d  _ppl.by.elev[:0]
+00006ba0: 2866 227b 7465 7374 7d20 2873 6c69 6365  (f"{test} (slice
+00006bb0: 6429 2229 0a20 2020 2020 2020 206c 6f77  d)").        low
+00006bc0: 5f70 706c 5f73 6c69 6365 2e70 7265 7365  _ppl_slice.prese
+00006bd0: 6e74 2829 0a20 2020 2020 2020 2073 656c  nt().        sel
+00006be0: 662e 6173 7365 7274 4571 7561 6c28 6c69  f.assertEqual(li
+00006bf0: 7374 286c 6f77 5f70 706c 5f77 6865 7265  st(low_ppl_where
+00006c00: 2e61 6c6c 2e69 6429 2c20 6c69 7374 286c  .all.id), list(l
+00006c10: 6f77 5f70 706c 5f73 6c69 6365 2e61 6c6c  ow_ppl_slice.all
+00006c20: 2e69 6429 290a 0a20 2020 2020 2020 2074  .id))..        t
+00006c30: 6573 7420 3d20 2265 6c65 7620 3e3d 2031  est = "elev >= 1
+00006c40: 3030 3022 0a20 2020 2020 2020 2068 695f  000".        hi_
+00006c50: 7070 6c5f 7768 6572 6520 3d20 7573 5f70  ppl_where = us_p
+00006c60: 706c 2e77 6865 7265 2865 6c65 763d 6c74  pl.where(elev=lt
+00006c70: 2e54 6162 6c65 2e67 6528 3130 3030 2929  .Table.ge(1000))
+00006c80: 2874 6573 7429 0a20 2020 2020 2020 2068  (test).        h
+00006c90: 695f 7070 6c5f 736c 6963 6520 3d20 7573  i_ppl_slice = us
+00006ca0: 5f70 706c 2e62 792e 656c 6576 5b31 3030  _ppl.by.elev[100
+00006cb0: 303a 5d28 6622 7b74 6573 747d 2028 736c  0:](f"{test} (sl
+00006cc0: 6963 6564 2922 290a 2020 2020 2020 2020  iced)").        
+00006cd0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00006ce0: 286c 6973 7428 6869 5f70 706c 5f77 6865  (list(hi_ppl_whe
+00006cf0: 7265 2e61 6c6c 2e69 6429 2c20 6c69 7374  re.all.id), list
+00006d00: 2868 695f 7070 6c5f 736c 6963 652e 616c  (hi_ppl_slice.al
+00006d10: 6c2e 6964 2929 0a0a 2020 2020 2020 2020  l.id))..        
+00006d20: 7465 7374 203d 2022 3020 3c3d 2065 6c65  test = "0 <= ele
+00006d30: 7620 3c20 3130 3022 0a20 2020 2020 2020  v < 100".       
+00006d40: 206c 6f77 5f70 706c 5f77 6865 7265 203d   low_ppl_where =
+00006d50: 2075 735f 7070 6c2e 7768 6572 6528 656c   us_ppl.where(el
+00006d60: 6576 3d6c 742e 5461 626c 652e 6765 2830  ev=lt.Table.ge(0
+00006d70: 2929 2e77 6865 7265 2865 6c65 763d 6c74  )).where(elev=lt
+00006d80: 2e54 6162 6c65 2e6c 7428 3130 3029 2928  .Table.lt(100))(
+00006d90: 7465 7374 290a 2020 2020 2020 2020 6c6f  test).        lo
+00006da0: 775f 7070 6c5f 736c 6963 6520 3d20 7573  w_ppl_slice = us
+00006db0: 5f70 706c 2e62 792e 656c 6576 5b30 3a31  _ppl.by.elev[0:1
+00006dc0: 3030 5d28 6622 7b74 6573 747d 2028 736c  00](f"{test} (sl
+00006dd0: 6963 6564 2922 290a 2020 2020 2020 2020  iced)").        
+00006de0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00006df0: 286c 6973 7428 6c6f 775f 7070 6c5f 7768  (list(low_ppl_wh
+00006e00: 6572 652e 616c 6c2e 6964 292c 206c 6973  ere.all.id), lis
+00006e10: 7428 6c6f 775f 7070 6c5f 736c 6963 652e  t(low_ppl_slice.
+00006e20: 616c 6c2e 6964 2929 0a0a 2020 2020 2020  all.id))..      
+00006e30: 2020 615f 7070 6c5f 7768 6572 6520 3d20    a_ppl_where = 
+00006e40: 7573 5f70 706c 2e77 6865 7265 286e 616d  us_ppl.where(nam
+00006e50: 653d 6c74 2e54 6162 6c65 2e67 6528 2241  e=lt.Table.ge("A
+00006e60: 2229 292e 7768 6572 6528 6e61 6d65 3d6c  ")).where(name=l
+00006e70: 742e 5461 626c 652e 6c74 2822 4322 2929  t.Table.lt("C"))
+00006e80: 0a20 2020 2020 2020 2061 5f70 706c 5f73  .        a_ppl_s
+00006e90: 6c69 6365 203d 2075 735f 7070 6c2e 6279  lice = us_ppl.by
+00006ea0: 2e6e 616d 655b 2241 223a 2243 225d 0a20  .name["A":"C"]. 
+00006eb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00006ec0: 7274 4571 7561 6c28 6c69 7374 2861 5f70  rtEqual(list(a_p
+00006ed0: 706c 5f77 6865 7265 2e61 6c6c 2e69 6429  pl_where.all.id)
+00006ee0: 2c20 6c69 7374 2861 5f70 706c 5f73 6c69  , list(a_ppl_sli
+00006ef0: 6365 2e61 6c6c 2e69 6429 290a 0a20 2020  ce.all.id))..   
+00006f00: 2064 6566 2074 6573 745f 6e6f 6e5f 696e   def test_non_in
+00006f10: 7465 6765 725f 736c 6963 6564 5f69 6e64  teger_sliced_ind
+00006f20: 6578 696e 6728 7365 6c66 293a 0a20 2020  exing(self):.   
+00006f30: 2020 2020 2069 6d70 6f72 7420 6461 7465       import date
+00006f40: 7469 6d65 0a0a 2020 2020 2020 2020 7361  time..        sa
+00006f50: 6c65 735f 6461 7461 203d 2074 6578 7477  les_data = textw
+00006f60: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+00006f70: 2020 2020 2020 2020 2020 2020 6461 7465              date
+00006f80: 2c63 7573 746f 6d65 722c 736b 752c 7174  ,customer,sku,qt
+00006f90: 790a 2020 2020 2020 2020 2020 2020 3230  y.            20
+00006fa0: 3030 2f30 312f 3031 2c30 3032 302c 414e  00/01/01,0020,AN
+00006fb0: 5649 4c2d 3030 312c 310a 2020 2020 2020  VIL-001,1.      
+00006fc0: 2020 2020 2020 3230 3030 2f30 312f 3031        2000/01/01
+00006fd0: 2c30 3032 302c 4252 4453 442d 3030 312c  ,0020,BRDSD-001,
+00006fe0: 320a 2020 2020 2020 2020 2020 2020 3230  2.            20
+00006ff0: 3030 2f30 322f 3135 2c30 3032 302c 4252  00/02/15,0020,BR
+00007000: 4453 442d 3030 312c 340a 2020 2020 2020  DSD-001,4.      
+00007010: 2020 2020 2020 3230 3030 2f30 332f 3331        2000/03/31
+00007020: 2c30 3032 302c 4252 4453 442d 3030 312c  ,0020,BRDSD-001,
+00007030: 380a 2020 2020 2020 2020 2020 2020 3230  8.            20
+00007040: 3030 2f30 332f 3331 2c30 3032 302c 4d41  00/03/31,0020,MA
+00007050: 474e 542d 3030 312c 3136 0a20 2020 2020  GNT-001,16.     
+00007060: 2020 2020 2020 2032 3030 302f 3034 2f30         2000/04/0
+00007070: 312c 3030 3230 2c52 4f42 4f54 2d30 3031  1,0020,ROBOT-001
+00007080: 2c33 320a 2020 2020 2020 2020 2020 2020  ,32.            
+00007090: 3230 3030 2f30 342f 3135 2c30 3032 302c  2000/04/15,0020,
+000070a0: 4252 4453 442d 3030 312c 3634 0a20 2020  BRDSD-001,64.   
+000070b0: 2020 2020 2020 2020 2022 2222 290a 0a20           """).. 
+000070c0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000070d0: 7320 3d20 7b27 6461 7465 273a 206c 742e  s = {'date': lt.
+000070e0: 5461 626c 652e 7061 7273 655f 6461 7465  Table.parse_date
+000070f0: 2822 2559 2f25 6d2f 2564 2229 2c0a 2020  ("%Y/%m/%d"),.  
+00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007110: 2020 2020 2771 7479 273a 2069 6e74 7d0a      'qty': int}.
+00007120: 2020 2020 2020 2020 7361 6c65 7320 3d20          sales = 
+00007130: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00007140: 6d70 6f72 7428 7361 6c65 735f 6461 7461  mport(sales_data
+00007150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+00007180: 6d73 3d74 7261 6e73 666f 726d 732c 290a  ms=transforms,).
+00007190: 0a20 2020 2020 2020 2073 616c 6573 2e63  .        sales.c
+000071a0: 7265 6174 655f 696e 6465 7828 2264 6174  reate_index("dat
+000071b0: 6522 290a 2020 2020 2020 2020 6a61 6e5f  e").        jan_
+000071c0: 3031 203d 2064 6174 6574 696d 652e 6461  01 = datetime.da
+000071d0: 7465 2832 3030 302c 2031 2c20 3129 0a20  te(2000, 1, 1). 
+000071e0: 2020 2020 2020 2061 7072 5f30 3120 3d20         apr_01 = 
+000071f0: 6461 7465 7469 6d65 2e64 6174 6528 3230  datetime.date(20
+00007200: 3030 2c20 342c 2031 290a 2020 2020 2020  00, 4, 1).      
+00007210: 2020 6669 7273 745f 7174 725f 7361 6c65    first_qtr_sale
+00007220: 7320 3d20 7361 6c65 732e 6279 2e64 6174  s = sales.by.dat
+00007230: 655b 6a61 6e5f 3031 3a20 6170 725f 3031  e[jan_01: apr_01
+00007240: 5d0a 2020 2020 2020 2020 6669 7273 745f  ].        first_
+00007250: 7174 725f 7361 6c65 732e 7072 6573 656e  qtr_sales.presen
+00007260: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
+00007270: 7428 6c69 7374 2866 6972 7374 5f71 7472  t(list(first_qtr
+00007280: 5f73 616c 6573 2e61 6c6c 2e73 6b75 2929  _sales.all.sku))
+00007290: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+000072a0: 7373 6572 7445 7175 616c 286c 6973 7428  ssertEqual(list(
+000072b0: 6669 7273 745f 7174 725f 7361 6c65 732e  first_qtr_sales.
+000072c0: 616c 6c2e 736b 7529 2c0a 2020 2020 2020  all.sku),.      
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2020 205b 2741 4e56 494c 2d30 3031 272c     ['ANVIL-001',
+000072f0: 2027 4252 4453 442d 3030 3127 2c20 2742   'BRDSD-001', 'B
+00007300: 5244 5344 2d30 3031 272c 2027 4252 4453  RDSD-001', 'BRDS
+00007310: 442d 3030 3127 2c20 274d 4147 4e54 2d30  D-001', 'MAGNT-0
+00007320: 3031 275d 2c0a 2020 2020 2020 2020 2020  01'],.          
+00007330: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007340: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007350: 7365 7274 4571 7561 6c28 3331 2c20 7375  sertEqual(31, su
+00007360: 6d28 6669 7273 745f 7174 725f 7361 6c65  m(first_qtr_sale
+00007370: 732e 616c 6c2e 7174 7929 290a 0a20 2020  s.all.qty))..   
+00007380: 2020 2020 2023 2075 7365 2064 6174 6520       # use date 
+00007390: 7374 7269 6e67 7320 6173 2072 616e 6765  strings as range
+000073a0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+000073b0: 7472 616e 7366 6f72 6d73 203d 207b 2771  transforms = {'q
+000073c0: 7479 273a 2069 6e74 7d0a 2020 2020 2020  ty': int}.      
+000073d0: 2020 7361 6c65 7320 3d20 6c74 2e54 6162    sales = lt.Tab
+000073e0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+000073f0: 7361 6c65 735f 6461 7461 2c0a 2020 2020  sales_data,.    
+00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 7472 616e 7366 6f72 6d73 3d74 7261    transforms=tra
+00007430: 6e73 666f 726d 732c 290a 0a20 2020 2020  nsforms,)..     
+00007440: 2020 2073 616c 6573 2e63 7265 6174 655f     sales.create_
+00007450: 696e 6465 7828 2264 6174 6522 290a 2020  index("date").  
+00007460: 2020 2020 2020 6669 7273 745f 7174 725f        first_qtr_
+00007470: 7361 6c65 7320 3d20 7361 6c65 732e 6279  sales = sales.by
+00007480: 2e64 6174 655b 2232 3030 302f 3031 2f30  .date["2000/01/0
+00007490: 3122 3a20 2232 3030 302f 3034 2f30 3122  1": "2000/04/01"
+000074a0: 5d0a 2020 2020 2020 2020 6669 7273 745f  ].        first_
+000074b0: 7174 725f 7361 6c65 732e 7072 6573 656e  qtr_sales.presen
+000074c0: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
+000074d0: 7428 6c69 7374 2866 6972 7374 5f71 7472  t(list(first_qtr
+000074e0: 5f73 616c 6573 2e61 6c6c 2e73 6b75 2929  _sales.all.sku))
+000074f0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00007500: 7373 6572 7445 7175 616c 286c 6973 7428  ssertEqual(list(
+00007510: 6669 7273 745f 7174 725f 7361 6c65 732e  first_qtr_sales.
+00007520: 616c 6c2e 736b 7529 2c0a 2020 2020 2020  all.sku),.      
 00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00007560: 7273 5b62 6220 2520 6c65 6e28 6368 6172  rs[bb % len(char
-00007570: 7329 5d2c 0a20 2020 2020 2020 2020 2020  s)],.           
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075b0: 2063 6861 7273 5b63 6320 2520 6c65 6e28   chars[cc % len(
-000075c0: 6368 6172 7329 5d29 0a20 2020 2020 2020  chars)]).       
-000075d0: 2074 6573 745f 7369 7a65 203d 2031 300a   test_size = 10.
-000075e0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-000075f0: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-00007600: 6d61 6b65 5f72 6563 2c20 7465 7374 5f73  make_rec, test_s
-00007610: 697a 6529 0a20 2020 2020 2020 2074 6162  ize).        tab
-00007620: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
-00007630: 2761 2729 0a20 2020 2020 2020 2074 6162  'a').        tab
-00007640: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
-00007650: 2762 2729 0a0a 2020 2020 2020 2020 6469  'b')..        di
-00007660: 725f 6c69 7374 203d 2064 6972 2874 6162  r_list = dir(tab
-00007670: 6c65 2e62 7929 0a20 2020 2020 2020 2070  le.by).        p
-00007680: 7269 6e74 285b 6174 7472 2066 6f72 2061  rint([attr for a
-00007690: 7474 7220 696e 2064 6972 5f6c 6973 7420  ttr in dir_list 
-000076a0: 6966 206e 6f74 2061 7474 722e 7374 6172  if not attr.star
-000076b0: 7473 7769 7468 2822 5f22 295d 290a 0a20  tswith("_")]).. 
-000076c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000076d0: 7274 5472 7565 2828 2761 2720 696e 2064  rtTrue(('a' in d
-000076e0: 6972 5f6c 6973 7429 2061 6e64 2028 2762  ir_list) and ('b
-000076f0: 2720 696e 2064 6972 5f6c 6973 7429 2061  ' in dir_list) a
-00007700: 6e64 2028 2763 2720 6e6f 7420 696e 2064  nd ('c' not in d
-00007710: 6972 5f6c 6973 7429 290a 0a20 2020 2064  ir_list))..    d
-00007720: 6566 2074 6573 745f 6465 6c65 7465 5f62  ef test_delete_b
-00007730: 795f 6669 6c74 6572 2873 656c 6629 3a0a  y_filter(self):.
-00007740: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-00007750: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-00007760: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
-00007770: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-00007780: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00007790: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-000077a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000077b0: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-000077c0: 745f 7369 7a65 2c20 7461 626c 652e 6465  t_size, table.de
-000077d0: 6c65 7465 2862 3d35 2929 0a20 2020 2020  lete(b=5)).     
-000077e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000077f0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
-00007800: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
-00007810: 7a65 2d31 292c 206c 656e 2874 6162 6c65  ze-1), len(table
-00007820: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00007830: 6173 7365 7274 4571 7561 6c28 302c 2074  assertEqual(0, t
-00007840: 6162 6c65 2e64 656c 6574 6528 623d 2d31  able.delete(b=-1
-00007850: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00007860: 6173 7365 7274 4571 7561 6c28 302c 2074  assertEqual(0, t
-00007870: 6162 6c65 2e64 656c 6574 6528 2929 0a0a  able.delete())..
-00007880: 2020 2020 6465 6620 7465 7374 5f72 656d      def test_rem
-00007890: 6f76 655f 6d61 6e79 2873 656c 6629 3a0a  ove_many(self):.
-000078a0: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-000078b0: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-000078c0: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
-000078d0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-000078e0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-000078f0: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-00007900: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007910: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-00007920: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00007930: 2f32 2c20 6c65 6e28 7461 626c 652e 7768  /2, len(table.wh
-00007940: 6572 6528 6c61 6d62 6461 2074 3a20 742e  ere(lambda t: t.
-00007950: 6120 2520 3229 2929 0a20 2020 2020 2020  a % 2))).       
-00007960: 2074 6162 6c65 2e72 656d 6f76 655f 6d61   table.remove_ma
-00007970: 6e79 2874 6162 6c65 2e77 6865 7265 286c  ny(table.where(l
-00007980: 616d 6264 6120 743a 2074 2e61 2025 2032  ambda t: t.a % 2
-00007990: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000079a0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-000079b0: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-000079c0: 7465 7374 5f73 697a 652f 322c 206c 656e  test_size/2, len
-000079d0: 2874 6162 6c65 2929 0a20 2020 2020 2020  (table)).       
-000079e0: 2074 6162 6c65 5f6c 656e 203d 206c 656e   table_len = len
-000079f0: 2874 6162 6c65 290a 2020 2020 2020 2020  (table).        
-00007a00: 7461 626c 652e 7265 6d6f 7665 2874 6162  table.remove(tab
-00007a10: 6c65 5b31 5d29 0a20 2020 2020 2020 2073  le[1]).        s
-00007a20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00007a30: 7461 626c 655f 6c65 6e2d 312c 206c 656e  table_len-1, len
-00007a40: 2874 6162 6c65 2929 0a0a 2020 2020 6465  (table))..    de
-00007a50: 6620 7465 7374 5f61 6464 5f6e 6577 5f66  f test_add_new_f
-00007a60: 6965 6c64 2873 656c 6629 3a0a 2020 2020  ield(self):.    
-00007a70: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00007a80: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-00007a90: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00007aa0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-00007ab0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00007ac0: 697a 6529 0a0a 2020 2020 2020 2020 2320  ize)..        # 
-00007ad0: 6e6f 7420 616c 6c20 7374 6f72 6167 6520  not all storage 
-00007ae0: 636c 6173 7365 7320 7375 7070 6f72 7420  classes support 
-00007af0: 6164 6469 6e67 206e 6577 2066 6965 6c64  adding new field
-00007b00: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-00007b10: 662e 7374 6f72 6167 655f 7375 7070 6f72  f.storage_suppor
-00007b20: 7473 5f61 6464 5f66 6965 6c64 3a0a 2020  ts_add_field:.  
-00007b30: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00007b40: 6164 645f 6669 656c 6428 2764 272c 206c  add_field('d', l
-00007b50: 616d 6264 6120 7265 633a 2072 6563 2e61  ambda rec: rec.a
-00007b60: 2b72 6563 2e62 2b72 6563 2e63 290a 0a20  +rec.b+rec.c).. 
-00007b70: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00007b80: 2e63 7265 6174 655f 696e 6465 7828 2764  .create_index('d
-00007b90: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-00007ba0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00007bb0: 6c65 6e28 7261 6e67 6528 302c 2032 372b  len(range(0, 27+
-00007bc0: 3129 292c 206c 656e 2874 6162 6c65 2e62  1)), len(table.b
-00007bd0: 792e 642e 6b65 7973 2829 2929 0a0a 2020  y.d.keys()))..  
-00007be0: 2020 6465 6620 7465 7374 5f61 6464 5f66    def test_add_f
-00007bf0: 6965 6c64 5f6f 7665 725f 6578 6973 7469  ield_over_existi
-00007c00: 6e67 5f69 6e64 6578 6564 5f66 6965 6c64  ng_indexed_field
-00007c10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007c20: 7465 7374 5f73 697a 6520 3d20 320a 2020  test_size = 2.  
-00007c30: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
-00007c40: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-00007c50: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00007c60: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-00007c70: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
-00007c80: 6561 7465 5f69 6e64 6578 2827 6327 290a  eate_index('c').
-00007c90: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00007ca0: 7365 6c66 2e73 746f 7261 6765 5f69 735f  self.storage_is_
-00007cb0: 6d75 7461 626c 653a 0a20 2020 2020 2020  mutable:.       
-00007cc0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00007cd0: 2020 2020 2074 6162 6c65 2e61 6464 5f66       table.add_f
-00007ce0: 6965 6c64 2827 6327 2c20 6c61 6d62 6461  ield('c', lambda
-00007cf0: 2072 6563 3a20 2d31 290a 2020 2020 2020   rec: -1).      
-00007d00: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007d10: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00007d20: 5b72 6563 2e63 2066 6f72 2072 6563 2069  [rec.c for rec i
-00007d30: 6e20 7461 626c 655d 2c0a 2020 2020 2020  n table],.      
-00007d40: 2020 2020 2020 6c69 7374 2874 6162 6c65        list(table
-00007d50: 2e61 6c6c 2e63 292c 0a20 2020 2020 2020  .all.c),.       
-00007d60: 2020 2020 2022 616c 6c20 6c69 7374 2072       "all list r
-00007d70: 6561 6473 2069 6e64 6578 2c20 7768 6963  eads index, whic
-00007d80: 6820 6973 206e 6f74 2072 6562 7569 6c74  h is not rebuilt
-00007d90: 2062 7920 6164 645f 6669 656c 6422 2c0a   by add_field",.
-00007da0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00007db0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00007dc0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-00007dd0: 207b 2d31 7d2c 0a20 2020 2020 2020 2020   {-1},.         
-00007de0: 2020 2073 6574 2874 6162 6c65 2e62 792e     set(table.by.
-00007df0: 632e 6b65 7973 2829 292c 0a20 2020 2020  c.keys()),.     
-00007e00: 2020 2020 2020 2022 696e 6465 7820 6b65         "index ke
-00007e10: 7973 2061 7265 206e 6f74 2072 6562 7569  ys are not rebui
-00007e20: 6c74 2062 7920 6164 645f 6669 656c 6422  lt by add_field"
-00007e30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00007e40: 2064 6566 2074 6573 745f 6164 645f 7477   def test_add_tw
-00007e50: 6f5f 7461 626c 6573 2873 656c 6629 3a0a  o_tables(self):.
-00007e60: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-00007e70: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-00007e80: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
-00007e90: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
-00007ea0: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
-00007eb0: 7369 7a65 290a 2020 2020 2020 2020 6d61  size).        ma
-00007ec0: 6b65 5f72 6563 203d 206c 616d 6264 6120  ke_rec = lambda 
-00007ed0: 612c 622c 633a 2073 656c 662e 6d61 6b65  a,b,c: self.make
-00007ee0: 5f64 6174 615f 6f62 6a65 6374 2861 2b74  _data_object(a+t
-00007ef0: 6573 745f 7369 7a65 2c20 622c 2063 290a  est_size, b, c).
-00007f00: 2020 2020 2020 2020 7432 203d 206d 616b          t2 = mak
-00007f10: 655f 7465 7374 5f74 6162 6c65 286d 616b  e_test_table(mak
-00007f20: 655f 7265 632c 2074 6573 745f 7369 7a65  e_rec, test_size
-00007f30: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007f40: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-00007f50: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-00007f60: 7465 7374 5f73 697a 652a 322c 206c 656e  test_size*2, len
-00007f70: 2874 312b 7432 2929 0a20 2020 2020 2020  (t1+t2)).       
-00007f80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007f90: 6c28 7465 7374 5f73 697a 6520 2a20 7465  l(test_size * te
-00007fa0: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
-00007fb0: 697a 652c 206c 656e 2874 3129 290a 0a20  ize, len(t1)).. 
-00007fc0: 2020 2020 2020 2074 3120 2b3d 2074 320a         t1 += t2.
-00007fd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00007fe0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00007ff0: 7a65 202a 2074 6573 745f 7369 7a65 202a  ze * test_size *
-00008000: 2074 6573 745f 7369 7a65 202a 2032 2c20   test_size * 2, 
-00008010: 6c65 6e28 7431 2929 0a0a 2020 2020 2020  len(t1))..      
-00008020: 2020 6f66 6673 6574 203d 2074 6573 745f    offset = test_
-00008030: 7369 7a65 202a 2074 6573 745f 7369 7a65  size * test_size
-00008040: 0a20 2020 2020 2020 2074 3320 3d20 7431  .        t3 = t1
-00008050: 202b 2028 7365 6c66 2e6d 616b 655f 6461   + (self.make_da
-00008060: 7461 5f6f 626a 6563 7428 7265 632e 612b  ta_object(rec.a+
-00008070: 6f66 6673 6574 2c20 7265 632e 622c 2072  offset, rec.b, r
-00008080: 6563 2e63 2920 666f 7220 7265 6320 696e  ec.c) for rec in
-00008090: 2074 3229 0a20 2020 2020 2020 2073 656c   t2).        sel
-000080a0: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-000080b0: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
-000080c0: 697a 6520 2a20 7465 7374 5f73 697a 6520  ize * test_size 
-000080d0: 2a20 332c 206c 656e 2874 3329 290a 0a20  * 3, len(t3)).. 
-000080e0: 2020 2064 6566 2074 6573 745f 7461 626c     def test_tabl
-000080f0: 655f 696e 666f 2873 656c 6629 3a0a 2020  e_info(self):.  
-00008100: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00008110: 3d20 3130 0a20 2020 2020 2020 2077 6974  = 10.        wit
-00008120: 6820 7469 6d65 7374 616d 705f 7374 6172  h timestamp_star
-00008130: 745f 656e 6428 2920 6173 2074 696d 696e  t_end() as timin
-00008140: 673a 0a20 2020 2020 2020 2020 2020 2074  g:.            t
-00008150: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
-00008160: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
-00008170: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
-00008180: 7369 7a65 2928 2769 6e66 6f5f 7465 7374  size)('info_test
-00008190: 2729 0a0a 2020 2020 2020 2020 7431 2e63  ')..        t1.c
-000081a0: 7265 6174 655f 696e 6465 7828 2762 2729  reate_index('b')
-000081b0: 0a20 2020 2020 2020 2074 315f 696e 666f  .        t1_info
-000081c0: 203d 2074 312e 696e 666f 2829 0a20 2020   = t1.info().   
-000081d0: 2020 2020 2023 206d 7573 7420 736f 7274       # must sort
-000081e0: 2066 6965 6c64 7320 616e 6420 696e 6465   fields and inde
-000081f0: 7865 7320 7661 6c75 6573 2c20 666f 7220  xes values, for 
-00008200: 7465 7374 2063 6f6d 7061 7269 736f 6e73  test comparisons
-00008210: 0a20 2020 2020 2020 2074 315f 696e 666f  .        t1_info
-00008220: 5b27 6669 656c 6473 275d 2e73 6f72 7428  ['fields'].sort(
-00008230: 290a 2020 2020 2020 2020 7431 5f69 6e66  ).        t1_inf
-00008240: 6f5b 2769 6e64 6578 6573 275d 2e73 6f72  o['indexes'].sor
-00008250: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00008260: 2e61 7373 6572 7445 7175 616c 284e 6f6e  .assertEqual(Non
-00008270: 652c 2074 315f 696e 666f 2e70 6f70 2822  e, t1_info.pop("
-00008280: 6c61 7374 5f69 6d70 6f72 7422 2929 0a20  last_import")). 
-00008290: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000082a0: 7274 5472 7565 2874 696d 696e 672e 7374  rtTrue(timing.st
-000082b0: 6172 7420 3c3d 2074 315f 696e 666f 2e70  art <= t1_info.p
-000082c0: 6f70 2822 6372 6561 7465 6422 2920 3c3d  op("created") <=
-000082d0: 2074 696d 696e 672e 656e 6429 0a20 2020   timing.end).   
-000082e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000082f0: 5472 7565 2874 696d 696e 672e 7374 6172  True(timing.star
-00008300: 7420 3c3d 2074 315f 696e 666f 2e70 6f70  t <= t1_info.pop
-00008310: 2822 6d6f 6469 6669 6564 2229 203c 3d20  ("modified") <= 
-00008320: 7469 6d69 6e67 2e65 6e64 290a 2020 2020  timing.end).    
-00008330: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00008340: 7175 616c 287b 2766 6965 6c64 7327 3a20  qual({'fields': 
-00008350: 5b27 6127 2c20 2762 272c 2027 6327 5d2c  ['a', 'b', 'c'],
-00008360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008370: 2020 2020 2020 2020 2020 2027 696e 6465             'inde
-00008380: 7865 7327 3a20 5b28 2762 272c 2046 616c  xes': [('b', Fal
-00008390: 7365 295d 2c0a 2020 2020 2020 2020 2020  se)],.          
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 276c 656e 273a 2031 3030 302c 0a20 2020  'len': 1000,.   
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 2020 2020 2020 2027 6e61 6d65 273a 2027         'name': '
-000083e0: 696e 666f 5f74 6573 7427 7d2c 0a20 2020  info_test'},.   
-000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 2020 2020 2020 7431 5f69 6e66 6f2c 2022        t1_info, "
-00008410: 696e 7661 6c69 6420 696e 666f 2072 6573  invalid info res
-00008420: 756c 7473 2229 0a0a 0a40 6d61 6b65 5f74  ults")...@make_t
-00008430: 6573 745f 636c 6173 7365 730a 636c 6173  est_classes.clas
-00008440: 7320 5461 626c 654c 6973 7454 6573 7473  s TableListTests
-00008450: 3a0a 2020 2020 2222 220a 2020 2020 5465  :.    """.    Te
-00008460: 7374 7320 666f 7220 6163 6365 7373 696e  sts for accessin
-00008470: 6720 5461 626c 6573 2061 7320 6c69 7374  g Tables as list
-00008480: 732e 0a20 2020 2022 2222 0a20 2020 2064  s..    """.    d
-00008490: 6566 205f 7465 7374 5f69 6e69 7428 7365  ef _test_init(se
-000084a0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-000084b0: 662e 7465 7374 5f73 697a 6520 3d20 330a  f.test_size = 3.
-000084c0: 2020 2020 2020 2020 7365 6c66 2e74 3120          self.t1 
-000084d0: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-000084e0: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-000084f0: 5f6f 626a 6563 742c 2073 656c 662e 7465  _object, self.te
-00008500: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
-00008510: 2073 656c 662e 7465 7374 5f72 6563 203d   self.test_rec =
-00008520: 2073 656c 662e 6d61 6b65 5f64 6174 615f   self.make_data_
-00008530: 6f62 6a65 6374 2831 2c20 312c 2031 290a  object(1, 1, 1).
-00008540: 0a20 2020 2064 6566 2074 6573 745f 636f  .    def test_co
-00008550: 6e74 6169 6e73 2873 656c 6629 3a0a 2020  ntains(self):.  
-00008560: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
-00008570: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
-00008580: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00008590: 7365 6c66 2e74 6573 745f 7265 6320 696e  self.test_rec in
-000085a0: 2073 656c 662e 7431 2c20 2266 6169 6c65   self.t1, "faile
-000085b0: 6420 2769 6e27 2028 636f 6e74 6169 6e73  d 'in' (contains
-000085c0: 2920 7465 7374 2229 0a0a 2020 2020 6465  ) test")..    de
-000085d0: 6620 7465 7374 5f69 6e64 6578 5f66 696e  f test_index_fin
-000085e0: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-000085f0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
-00008600: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008610: 6173 7365 7274 4571 7561 6c28 3133 2c20  assertEqual(13, 
-00008620: 7365 6c66 2e74 312e 696e 6465 7828 7365  self.t1.index(se
-00008630: 6c66 2e74 6573 745f 7265 6329 2c20 2266  lf.test_rec), "f
-00008640: 6169 6c65 6420 2769 6e64 6578 3b20 7465  ailed 'index; te
-00008650: 7374 2028 6578 6973 7473 2922 290a 2020  st (exists)").  
-00008660: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00008670: 6e63 6528 7365 6c66 2e74 6573 745f 7265  nce(self.test_re
-00008680: 632c 2053 696d 706c 654e 616d 6573 7061  c, SimpleNamespa
-00008690: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
-000086a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000086b0: 6c28 3133 2c20 7365 6c66 2e74 312e 696e  l(13, self.t1.in
-000086c0: 6465 7828 7661 7273 2873 656c 662e 7465  dex(vars(self.te
-000086d0: 7374 5f72 6563 2929 2c20 2266 6169 6c65  st_rec)), "faile
-000086e0: 6420 2769 6e64 6578 3b20 7465 7374 2028  d 'index; test (
-000086f0: 6578 6973 7473 2922 290a 0a20 2020 2020  exists)")..     
-00008700: 2020 206e 6f5f 7375 6368 5f72 6563 203d     no_such_rec =
-00008710: 2073 656c 662e 6d61 6b65 5f64 6174 615f   self.make_data_
-00008720: 6f62 6a65 6374 2873 656c 662e 7465 7374  object(self.test
-00008730: 5f73 697a 652b 312c 2073 656c 662e 7465  _size+1, self.te
-00008740: 7374 5f73 697a 652b 312c 2073 656c 662e  st_size+1, self.
-00008750: 7465 7374 5f73 697a 652b 3129 0a20 2020  test_size+1).   
-00008760: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-00008770: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
-00008780: 6545 7272 6f72 2c20 6d73 673d 2266 6169  eError, msg="fai
-00008790: 6c65 6420 2769 6e64 6578 2720 7465 7374  led 'index' test
-000087a0: 2028 6e6f 7420 6578 6973 7473 2922 293a   (not exists)"):
-000087b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000087c0: 662e 7431 2e69 6e64 6578 286e 6f5f 7375  f.t1.index(no_su
-000087d0: 6368 5f72 6563 290a 0a20 2020 2064 6566  ch_rec)..    def
-000087e0: 2074 6573 745f 7265 6d6f 7665 2873 656c   test_remove(sel
-000087f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00008800: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-00008810: 2020 2020 2020 7265 6320 3d20 7365 6c66        rec = self
-00008820: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00008830: 7428 312c 2031 2c20 3129 0a20 2020 2020  t(1, 1, 1).     
-00008840: 2020 2070 7265 765f 6c65 6e20 3d20 6c65     prev_len = le
-00008850: 6e28 7365 6c66 2e74 3129 0a20 2020 2020  n(self.t1).     
-00008860: 2020 2073 656c 662e 7431 2e72 656d 6f76     self.t1.remov
-00008870: 6528 7265 6329 0a20 2020 2020 2020 2073  e(rec).        s
-00008880: 656c 662e 6173 7365 7274 4661 6c73 6528  elf.assertFalse(
-00008890: 7265 6320 696e 2073 656c 662e 7431 2c20  rec in self.t1, 
-000088a0: 2266 6169 6c65 6420 746f 2072 656d 6f76  "failed to remov
-000088b0: 6520 7265 636f 7264 2066 726f 6d20 7461  e record from ta
-000088c0: 626c 6520 2863 6f6e 7461 696e 7329 2229  ble (contains)")
-000088d0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000088e0: 7365 7274 4571 7561 6c28 7072 6576 5f6c  sertEqual(prev_l
-000088f0: 656e 2d31 2c20 6c65 6e28 7365 6c66 2e74  en-1, len(self.t
-00008900: 3129 2c20 2266 6169 6c65 6420 746f 2072  1), "failed to r
-00008910: 656d 6f76 6520 7265 636f 7264 2066 726f  emove record fro
-00008920: 6d20 7461 626c 6520 286c 656e 2922 290a  m table (len)").
-00008930: 0a20 2020 2020 2020 206e 6f5f 7375 6368  .        no_such
-00008940: 5f72 6563 203d 2073 656c 662e 6d61 6b65  _rec = self.make
-00008950: 5f64 6174 615f 6f62 6a65 6374 2873 656c  _data_object(sel
-00008960: 662e 7465 7374 5f73 697a 652b 312c 2073  f.test_size+1, s
-00008970: 656c 662e 7465 7374 5f73 697a 652b 312c  elf.test_size+1,
-00008980: 2073 656c 662e 7465 7374 5f73 697a 652b   self.test_size+
-00008990: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000089a0: 6173 7365 7274 4661 6c73 6528 6e6f 5f73  assertFalse(no_s
-000089b0: 7563 685f 7265 6320 696e 2073 656c 662e  uch_rec in self.
-000089c0: 7431 2c20 2266 6169 6c65 6420 746f 2063  t1, "failed to c
-000089d0: 7265 6174 6520 6e6f 6e2d 6578 6973 7465  reate non-existe
-000089e0: 6e74 2072 6563 6f72 6420 6672 6f6d 2074  nt record from t
-000089f0: 6162 6c65 2229 0a20 2020 2020 2020 2073  able").        s
-00008a00: 656c 662e 7431 2e72 656d 6f76 6528 6e6f  elf.t1.remove(no
-00008a10: 5f73 7563 685f 7265 6329 0a20 2020 2020  _such_rec).     
-00008a20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00008a30: 7561 6c28 7072 6576 5f6c 656e 2d31 2c20  ual(prev_len-1, 
-00008a40: 6c65 6e28 7365 6c66 2e74 3129 2c20 2266  len(self.t1), "f
-00008a50: 6169 6c65 6420 7265 6d6f 7669 6e67 206e  ailed removing n
-00008a60: 6f6e 2d65 7869 7374 656e 7420 7265 636f  on-existent reco
-00008a70: 7264 2066 726f 6d20 7461 626c 6520 286c  rd from table (l
-00008a80: 656e 2922 290a 0a20 2020 2020 2020 2069  en)")..        i
-00008a90: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
-00008aa0: 662e 7465 7374 5f72 6563 2c20 5369 6d70  f.test_rec, Simp
-00008ab0: 6c65 4e61 6d65 7370 6163 6529 3a0a 2020  leNamespace):.  
-00008ac0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00008ad0: 312e 7265 6d6f 7665 2876 6172 7328 7365  1.remove(vars(se
-00008ae0: 6c66 2e74 6573 745f 7265 6329 290a 2020  lf.test_rec)).  
-00008af0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00008b00: 7373 6572 7445 7175 616c 2870 7265 765f  ssertEqual(prev_
-00008b10: 6c65 6e2d 312c 206c 656e 2873 656c 662e  len-1, len(self.
-00008b20: 7431 292c 2022 6661 696c 6564 2074 6f20  t1), "failed to 
-00008b30: 7265 6d6f 7665 2072 6563 6f72 6420 6173  remove record as
-00008b40: 2064 6963 7420 6672 6f6d 2074 6162 6c65   dict from table
-00008b50: 2028 6c65 6e29 2229 0a0a 2020 2020 6465   (len)")..    de
-00008b60: 6620 7465 7374 5f69 6e64 6578 5f61 6363  f test_index_acc
-00008b70: 6573 7328 7365 6c66 293a 0a20 2020 2020  ess(self):.     
-00008b80: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-00008b90: 6974 2829 0a20 2020 2020 2020 2073 656c  it().        sel
-00008ba0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
-00008bb0: 6c66 2e74 6573 745f 7265 632c 2073 656c  lf.test_rec, sel
-00008bc0: 662e 7431 5b31 335d 2c20 2266 6169 6c65  f.t1[13], "faile
-00008bd0: 6420 696e 6465 7820 6163 6365 7373 2074  d index access t
-00008be0: 6573 7422 290a 0a20 2020 2064 6566 2074  est")..    def t
-00008bf0: 6573 745f 636f 756e 7428 7365 6c66 293a  est_count(self):
-00008c00: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00008c10: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
-00008c20: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00008c30: 7565 2873 656c 662e 7431 2e63 6f75 6e74  ue(self.t1.count
-00008c40: 2873 656c 662e 7465 7374 5f72 6563 2920  (self.test_rec) 
-00008c50: 3d3d 2031 2c20 2266 6169 6c65 6420 636f  == 1, "failed co
-00008c60: 756e 7420 7465 7374 2229 0a20 2020 2020  unt test").     
-00008c70: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00008c80: 2873 656c 662e 7465 7374 5f72 6563 2c20  (self.test_rec, 
-00008c90: 5369 6d70 6c65 4e61 6d65 7370 6163 6529  SimpleNamespace)
-00008ca0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008cb0: 6c66 2e61 7373 6572 7454 7275 6528 7365  lf.assertTrue(se
-00008cc0: 6c66 2e74 312e 636f 756e 7428 7661 7273  lf.t1.count(vars
-00008cd0: 2873 656c 662e 7465 7374 5f72 6563 2929  (self.test_rec))
-00008ce0: 203d 3d20 312c 2022 6661 696c 6564 2063   == 1, "failed c
-00008cf0: 6f75 6e74 2074 6573 7422 290a 0a20 2020  ount test")..   
-00008d00: 2064 6566 2074 6573 745f 6465 6c28 7365   def test_del(se
-00008d10: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00008d20: 662e 5f74 6573 745f 696e 6974 2829 0a20  f._test_init(). 
-00008d30: 2020 2020 2020 2062 6566 6f72 655f 6465         before_de
-00008d40: 6c5f 6c65 6e20 3d20 6c65 6e28 7365 6c66  l_len = len(self
-00008d50: 2e74 3129 0a20 2020 2020 2020 2064 656c  .t1).        del
-00008d60: 2073 656c 662e 7431 5b31 335d 0a20 2020   self.t1[13].   
-00008d70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00008d80: 4661 6c73 6528 7365 6c66 2e74 6573 745f  False(self.test_
-00008d90: 7265 6320 696e 2073 656c 662e 7431 2c20  rec in self.t1, 
-00008da0: 2266 6169 6c65 6420 6465 6c20 7465 7374  "failed del test
-00008db0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008dc0: 6173 7365 7274 4571 7561 6c28 6265 666f  assertEqual(befo
-00008dd0: 7265 5f64 656c 5f6c 656e 202d 2031 2c20  re_del_len - 1, 
-00008de0: 6c65 6e28 7365 6c66 2e74 3129 290a 0a20  len(self.t1)).. 
-00008df0: 2020 2064 6566 2074 6573 745f 706f 7028     def test_pop(
-00008e00: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00008e10: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
-00008e20: 0a20 2020 2020 2020 2062 6566 6f72 655f  .        before_
-00008e30: 706f 705f 6c65 6e20 3d20 6c65 6e28 7365  pop_len = len(se
-00008e40: 6c66 2e74 3129 0a20 2020 2020 2020 206f  lf.t1).        o
-00008e50: 626a 203d 2073 656c 662e 7431 2e70 6f70  bj = self.t1.pop
-00008e60: 2831 3329 0a20 2020 2020 2020 2073 656c  (13).        sel
-00008e70: 662e 6173 7365 7274 4661 6c73 6528 6f62  f.assertFalse(ob
-00008e80: 6a20 696e 2073 656c 662e 7431 290a 2020  j in self.t1).  
-00008e90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00008ea0: 7445 7175 616c 2873 656c 662e 7465 7374  tEqual(self.test
-00008eb0: 5f72 6563 2c20 6f62 6a29 0a20 2020 2020  _rec, obj).     
-00008ec0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00008ed0: 7561 6c28 6265 666f 7265 5f70 6f70 5f6c  ual(before_pop_l
-00008ee0: 656e 202d 2031 2c20 6c65 6e28 7365 6c66  en - 1, len(self
-00008ef0: 2e74 3129 290a 0a20 2020 2064 6566 2074  .t1))..    def t
-00008f00: 6573 745f 706f 705f 6c61 7374 2873 656c  est_pop_last(sel
-00008f10: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00008f20: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-00008f30: 2020 2020 2020 6265 666f 7265 5f70 6f70        before_pop
-00008f40: 5f6c 656e 203d 206c 656e 2873 656c 662e  _len = len(self.
-00008f50: 7431 290a 2020 2020 2020 2020 6578 7065  t1).        expe
-00008f60: 6374 6564 5f70 6f70 203d 2063 6f70 792e  cted_pop = copy.
-00008f70: 636f 7079 2873 656c 662e 7431 5b2d 315d  copy(self.t1[-1]
-00008f80: 290a 2020 2020 2020 2020 6f62 6a20 3d20  ).        obj = 
-00008f90: 7365 6c66 2e74 312e 706f 7028 290a 2020  self.t1.pop().  
-00008fa0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00008fb0: 7445 7175 616c 2865 7870 6563 7465 645f  tEqual(expected_
-00008fc0: 706f 702c 206f 626a 290a 2020 2020 2020  pop, obj).      
-00008fd0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00008fe0: 616c 2862 6566 6f72 655f 706f 705f 6c65  al(before_pop_le
-00008ff0: 6e20 2d20 312c 206c 656e 2873 656c 662e  n - 1, len(self.
-00009000: 7431 2929 0a0a 2020 2020 6465 6620 7465  t1))..    def te
-00009010: 7374 5f72 6576 6572 7365 6428 7365 6c66  st_reversed(self
-00009020: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00009030: 5f74 6573 745f 696e 6974 2829 0a20 2020  _test_init().   
-00009040: 2020 2020 206c 6173 745f 7265 6320 3d20       last_rec = 
-00009050: 6e65 7874 2872 6576 6572 7365 6428 7365  next(reversed(se
-00009060: 6c66 2e74 3129 290a 2020 2020 2020 2020  lf.t1)).        
-00009070: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00009080: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00009090: 6f62 6a65 6374 2832 2c20 322c 2032 292c  object(2, 2, 2),
-000090a0: 206c 6173 745f 7265 632c 2022 6661 696c   last_rec, "fail
-000090b0: 6564 2072 6576 6572 7365 6420 7465 7374  ed reversed test
-000090c0: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-000090d0: 5f69 7465 7228 7365 6c66 293a 0a20 2020  _iter(self):.   
-000090e0: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-000090f0: 696e 6974 2829 0a20 2020 2020 2020 2073  init().        s
-00009100: 656c 662e 6173 7365 7274 5472 7565 2873  elf.assertTrue(s
-00009110: 656c 662e 7465 7374 5f72 6563 2069 6e20  elf.test_rec in 
-00009120: 7365 6c66 2e74 312c 2022 6661 696c 6564  self.t1, "failed
-00009130: 2027 696e 2720 2863 6f6e 7461 696e 7329   'in' (contains)
-00009140: 2074 6573 7422 290a 0a20 2020 2064 6566   test")..    def
-00009150: 2074 6573 745f 6865 6164 5f61 6e64 5f74   test_head_and_t
-00009160: 6169 6c28 7365 6c66 293a 0a20 2020 2020  ail(self):.     
-00009170: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-00009180: 6974 2829 0a20 2020 2020 2020 2073 656c  it().        sel
-00009190: 662e 7431 2e63 7265 6174 655f 696e 6465  f.t1.create_inde
-000091a0: 7828 2261 2229 0a20 2020 2020 2020 2073  x("a").        s
-000091b0: 656c 662e 7431 2e63 7265 6174 655f 696e  elf.t1.create_in
-000091c0: 6465 7828 2263 2229 0a20 2020 2020 2020  dex("c").       
-000091d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000091e0: 6c28 7b22 6122 2c20 2263 227d 2c20 7365  l({"a", "c"}, se
-000091f0: 7428 7365 6c66 2e74 312e 5f69 6e64 6578  t(self.t1._index
-00009200: 6573 2e6b 6579 7328 2929 2c20 2266 6169  es.keys()), "fai
-00009210: 6c65 6420 746f 2063 7265 6174 6520 696e  led to create in
-00009220: 6465 7865 7322 290a 0a20 2020 2020 2020  dexes")..       
-00009230: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00009240: 6c28 7365 7428 7365 6c66 2e74 312e 5f69  l(set(self.t1._i
-00009250: 6e64 6578 6573 2e6b 6579 7328 2929 2c0a  ndexes.keys()),.
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009270: 2020 2020 2020 2020 2073 6574 2873 656c           set(sel
-00009280: 662e 7431 2e68 6561 6428 292e 5f69 6e64  f.t1.head()._ind
-00009290: 6578 6573 2e6b 6579 7328 2929 2c0a 2020  exes.keys()),.  
-000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092b0: 2020 2020 2020 2022 6661 696c 6564 2074         "failed t
-000092c0: 6f20 636f 7079 2069 6e64 6578 6573 2074  o copy indexes t
-000092d0: 6f20 6865 6164 2829 2229 0a20 2020 2020  o head()").     
-000092e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000092f0: 7561 6c28 7365 7428 7365 6c66 2e74 312e  ual(set(self.t1.
-00009300: 5f69 6e64 6578 6573 2e6b 6579 7328 2929  _indexes.keys())
-00009310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009320: 2020 2020 2020 2020 2020 2073 6574 2873             set(s
-00009330: 656c 662e 7431 2e74 6169 6c28 292e 5f69  elf.t1.tail()._i
-00009340: 6e64 6578 6573 2e6b 6579 7328 2929 2c0a  ndexes.keys()),.
-00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009360: 2020 2020 2020 2020 2022 6661 696c 6564           "failed
-00009370: 2074 6f20 636f 7079 2069 6e64 6578 6573   to copy indexes
-00009380: 2074 6f20 7461 696c 2829 2229 0a0a 2020   to tail()")..  
-00009390: 2020 6465 6620 7465 7374 5f75 6e69 7175    def test_uniqu
-000093a0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000093b0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
-000093c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000093d0: 6173 7365 7274 4571 7561 6c28 5b30 2c20  assertEqual([0, 
-000093e0: 312c 2032 5d2c 2073 6f72 7465 6428 5b72  1, 2], sorted([r
-000093f0: 6f77 2e61 2066 6f72 2072 6f77 2069 6e20  ow.a for row in 
-00009400: 7365 6c66 2e74 312e 756e 6971 7565 2827  self.t1.unique('
-00009410: 6127 295d 292c 2022 6661 696c 6564 2063  a')]), "failed c
-00009420: 616c 6c20 746f 2075 6e69 7175 6522 290a  all to unique").
-00009430: 0a20 2020 2064 6566 2074 6573 745f 616c  .    def test_al
-00009440: 6c5f 6163 6365 7373 6f72 2873 656c 6629  l_accessor(self)
-00009450: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00009460: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
-00009470: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00009480: 7175 616c 2873 756d 2828 5b69 5d2a 7365  qual(sum(([i]*se
-00009490: 6c66 2e74 6573 745f 7369 7a65 2a2a 3220  lf.test_size**2 
-000094a0: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-000094b0: 656c 662e 7465 7374 5f73 697a 6529 292c  elf.test_size)),
-000094c0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-000094d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000094e0: 6973 7428 7365 6c66 2e74 312e 616c 6c2e  ist(self.t1.all.
-000094f0: 6129 2c0a 2020 2020 2020 2020 2020 2020  a),.            
-00009500: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00009510: 696c 6564 2074 6f20 7375 6363 6573 7366  iled to successf
-00009520: 756c 6c79 2067 6574 2061 6c6c 2076 616c  ully get all val
-00009530: 7565 7320 696e 2027 6127 2229 0a0a 2020  ues in 'a'")..  
-00009540: 2020 2020 2020 616c 6c5f 6173 203d 2073        all_as = s
-00009550: 656c 662e 7431 2e61 6c6c 2e61 0a20 2020  elf.t1.all.a.   
-00009560: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009570: 5472 7565 2861 6c6c 5f61 7320 6973 2069  True(all_as is i
-00009580: 7465 7228 616c 6c5f 6173 292c 2022 616c  ter(all_as), "al
-00009590: 6c20 6974 6572 6174 6f72 2066 6169 6c73  l iterator fails
-000095a0: 2074 6f20 6964 656e 7469 6679 2061 7320   to identify as 
-000095b0: 6974 6572 2873 656c 6629 2229 0a0a 2020  iter(self)")..  
-000095c0: 2020 6465 6620 7465 7374 5f66 6f72 6d61    def test_forma
-000095d0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-000095e0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
-000095f0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00009600: 6173 7365 7274 4571 7561 6c28 5b27 3030  assertEqual(['00
-00009610: 2030 2030 272c 2027 3030 2030 2031 272c   0 0', '00 0 1',
-00009620: 2027 3030 2030 2032 275d 2c0a 2020 2020   '00 0 2'],.    
-00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009640: 2020 2020 206c 6973 7428 7365 6c66 2e74       list(self.t
-00009650: 312e 666f 726d 6174 2822 7b61 3a30 3264  1.format("{a:02d
-00009660: 7d20 7b62 7d20 7b63 7d22 2929 5b3a 335d  } {b} {c}"))[:3]
-00009670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009680: 2020 2020 2020 2020 2020 2022 6661 696c             "fail
-00009690: 6564 2074 6f20 6372 6561 7465 2066 6f72  ed to create for
-000096a0: 6d61 7474 6564 2072 6f77 7322 290a 0a20  matted rows").. 
-000096b0: 2020 2064 6566 2074 6573 745f 6173 5f68     def test_as_h
-000096c0: 746d 6c28 7365 6c66 293a 0a20 2020 2020  tml(self):.     
-000096d0: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-000096e0: 6974 2829 0a20 2020 2020 2020 2068 746d  it().        htm
-000096f0: 6c5f 6f75 7470 7574 203d 2073 656c 662e  l_output = self.
-00009700: 7431 5b3a 3130 5d2e 6173 5f68 746d 6c28  t1[:10].as_html(
-00009710: 6669 656c 6473 3d22 6120 6220 6322 290a  fields="a b c").
-00009720: 2020 2020 2020 2020 7072 696e 7428 6874          print(ht
-00009730: 6d6c 5f6f 7574 7075 7429 0a20 2020 2020  ml_output).     
-00009740: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00009750: 7565 2822 3c74 6865 6164 3e22 2069 6e20  ue("<thead>" in 
-00009760: 6874 6d6c 5f6f 7574 7075 7420 616e 6420  html_output and 
-00009770: 223c 7462 6f64 793e 2220 696e 2068 746d  "<tbody>" in htm
-00009780: 6c5f 6f75 7470 7574 2c0a 2020 2020 2020  l_output,.      
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097a0: 2020 2261 735f 6874 6d6c 2064 6f65 7320    "as_html does 
-000097b0: 6e6f 7420 696e 636c 7564 6520 7468 6561  not include thea
-000097c0: 6420 616e 6420 7462 6f64 7920 7461 6773  d and tbody tags
-000097d0: 2229 0a0a 2020 2020 2020 2020 6874 6d6c  ")..        html
-000097e0: 5f6c 696e 6573 203d 2068 746d 6c5f 6f75  _lines = html_ou
-000097f0: 7470 7574 2e73 706c 6974 6c69 6e65 7328  tput.splitlines(
-00009800: 290a 2020 2020 2020 2020 6864 725f 6c69  ).        hdr_li
-00009810: 6e65 203d 206e 6578 7428 6820 666f 7220  ne = next(h for 
-00009820: 6820 696e 2068 746d 6c5f 6c69 6e65 7320  h in html_lines 
-00009830: 6966 2022 6365 6e74 6572 2220 696e 2068  if "center" in h
-00009840: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009850: 7373 6572 7445 7175 616c 2827 3c74 723e  ssertEqual('<tr>
-00009860: 3c74 683e 3c64 6976 2061 6c69 676e 3d22  <th><div align="
-00009870: 6365 6e74 6572 223e 613c 2f64 6976 3e3c  center">a</div><
-00009880: 2f74 683e 270a 2020 2020 2020 2020 2020  /th>'.          
-00009890: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000098a0: 3c74 683e 3c64 6976 2061 6c69 676e 3d22  <th><div align="
-000098b0: 6365 6e74 6572 223e 623c 2f64 6976 3e3c  center">b</div><
-000098c0: 2f74 683e 270a 2020 2020 2020 2020 2020  /th>'.          
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000098e0: 3c74 683e 3c64 6976 2061 6c69 676e 3d22  <th><div align="
-000098f0: 6365 6e74 6572 223e 633c 2f64 6976 3e3c  center">c</div><
-00009900: 2f74 683e 3c2f 7472 3e27 2c0a 2020 2020  /th></tr>',.    
-00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2020 2068 6472 5f6c 696e 652c 0a20       hdr_line,. 
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2020 2020 2020 2266 6169 6c65 6420          "failed 
-00009950: 6173 5f68 746d 6c20 7769 7468 2061 6c6c  as_html with all
-00009960: 2066 6965 6c64 7322 290a 0a20 2020 2020   fields")..     
-00009970: 2020 2068 746d 6c5f 6f75 7470 7574 203d     html_output =
-00009980: 2073 656c 662e 7431 5b3a 3130 5d2e 6173   self.t1[:10].as
-00009990: 5f68 746d 6c28 6669 656c 6473 3d22 6120  _html(fields="a 
-000099a0: 2d62 2063 2229 0a20 2020 2020 2020 2070  -b c").        p
-000099b0: 7269 6e74 2868 746d 6c5f 6f75 7470 7574  rint(html_output
-000099c0: 290a 2020 2020 2020 2020 6874 6d6c 5f6c  ).        html_l
-000099d0: 696e 6573 203d 2068 746d 6c5f 6f75 7470  ines = html_outp
-000099e0: 7574 2e73 706c 6974 6c69 6e65 7328 290a  ut.splitlines().
-000099f0: 2020 2020 2020 2020 6864 725f 6c69 6e65          hdr_line
-00009a00: 203d 206e 6578 7428 6820 666f 7220 6820   = next(h for h 
-00009a10: 696e 2068 746d 6c5f 6c69 6e65 7320 6966  in html_lines if
-00009a20: 2022 6365 6e74 6572 2220 696e 2068 290a   "center" in h).
-00009a30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00009a40: 6572 7445 7175 616c 2827 3c74 723e 3c74  ertEqual('<tr><t
-00009a50: 683e 3c64 6976 2061 6c69 676e 3d22 6365  h><div align="ce
-00009a60: 6e74 6572 223e 613c 2f64 6976 3e3c 2f74  nter">a</div></t
-00009a70: 683e 270a 2020 2020 2020 2020 2020 2020  h>'.            
-00009a80: 2020 2020 2020 2020 2020 2020 2027 3c74               '<t
-00009a90: 683e 3c64 6976 2061 6c69 676e 3d22 6365  h><div align="ce
-00009aa0: 6e74 6572 223e 633c 2f64 6976 3e3c 2f74  nter">c</div></t
-00009ab0: 683e 3c2f 7472 3e27 2c0a 2020 2020 2020  h></tr>',.      
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ad0: 2020 2068 6472 5f6c 696e 652c 0a20 2020     hdr_line,.   
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 2020 2266 6169 6c65 6420 6173        "failed as
-00009b00: 5f68 746d 6c20 7769 7468 206e 6567 6174  _html with negat
-00009b10: 6564 2066 6965 6c64 2229 0a0a 2020 2020  ed field")..    
-00009b20: 2020 2020 6874 6d6c 5f6f 7574 7075 7420      html_output 
-00009b30: 3d20 7365 6c66 2e74 315b 3a31 305d 2e61  = self.t1[:10].a
-00009b40: 735f 6874 6d6c 2866 6965 6c64 733d 2261  s_html(fields="a
-00009b50: 2062 2063 222c 2066 6f72 6d61 7473 3d7b   b c", formats={
-00009b60: 2262 223a 2022 7b3a 3033 647d 227d 290a  "b": "{:03d}"}).
-00009b70: 2020 2020 2020 2020 7072 696e 7428 6874          print(ht
-00009b80: 6d6c 5f6f 7574 7075 7429 0a20 2020 2020  ml_output).     
-00009b90: 2020 2068 746d 6c5f 6c69 6e65 7320 3d20     html_lines = 
-00009ba0: 6874 6d6c 5f6f 7574 7075 742e 7370 6c69  html_output.spli
-00009bb0: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
-00009bc0: 2064 6174 615f 6c69 6e65 203d 206e 6578   data_line = nex
-00009bd0: 7428 6820 666f 7220 6820 696e 2068 746d  t(h for h in htm
-00009be0: 6c5f 6c69 6e65 7320 6966 2022 3c74 643e  l_lines if "<td>
-00009bf0: 2220 696e 2068 290a 2020 2020 2020 2020  " in h).        
-00009c00: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00009c10: 2827 3c74 626f 6479 3e3c 7472 3e3c 7464  ('<tbody><tr><td
-00009c20: 3e3c 6469 7620 616c 6967 6e3d 2272 6967  ><div align="rig
-00009c30: 6874 223e 303c 2f64 6976 3e3c 2f74 643e  ht">0</div></td>
-00009c40: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00009c50: 2020 2020 2020 2020 2020 2027 3c74 643e             '<td>
-00009c60: 3c64 6976 2061 6c69 676e 3d22 7269 6768  <div align="righ
-00009c70: 7422 3e30 3030 3c2f 6469 763e 3c2f 7464  t">000</div></td
-00009c80: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
-00009c90: 2020 2020 2020 2020 2020 2020 273c 7464              '<td
-00009ca0: 3e3c 6469 7620 616c 6967 6e3d 2272 6967  ><div align="rig
-00009cb0: 6874 223e 303c 2f64 6976 3e3c 2f74 643e  ht">0</div></td>
-00009cc0: 3c2f 7472 3e27 2c0a 2020 2020 2020 2020  </tr>',.        
-00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ce0: 2064 6174 615f 6c69 6e65 2c0a 2020 2020   data_line,.    
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2020 2022 6661 696c 6564 2061 735f       "failed as_
-00009d10: 6874 6d6c 2077 6974 6820 6e61 6d65 6420  html with named 
-00009d20: 6669 656c 6420 666f 726d 6174 2066 6f72  field format for
-00009d30: 2073 7065 6369 6669 6320 6669 656c 6422   specific field"
-00009d40: 290a 0a20 2020 2020 2020 2068 746d 6c5f  )..        html_
-00009d50: 6f75 7470 7574 203d 2073 656c 662e 7431  output = self.t1
-00009d60: 5b3a 3130 5d2e 6173 5f68 746d 6c28 6669  [:10].as_html(fi
-00009d70: 656c 6473 3d22 6120 6220 6322 2c20 666f  elds="a b c", fo
-00009d80: 726d 6174 733d 7b69 6e74 3a20 227b 3a30  rmats={int: "{:0
-00009d90: 3364 7d22 7d29 0a20 2020 2020 2020 2070  3d}"}).        p
-00009da0: 7269 6e74 2868 746d 6c5f 6f75 7470 7574  rint(html_output
-00009db0: 290a 2020 2020 2020 2020 6874 6d6c 5f6c  ).        html_l
-00009dc0: 696e 6573 203d 2068 746d 6c5f 6f75 7470  ines = html_outp
-00009dd0: 7574 2e73 706c 6974 6c69 6e65 7328 290a  ut.splitlines().
-00009de0: 2020 2020 2020 2020 6461 7461 5f6c 696e          data_lin
-00009df0: 6520 3d20 6e65 7874 2868 2066 6f72 2068  e = next(h for h
-00009e00: 2069 6e20 6874 6d6c 5f6c 696e 6573 2069   in html_lines i
-00009e10: 6620 223c 7464 3e22 2069 6e20 6829 0a20  f "<td>" in h). 
-00009e20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00009e30: 7274 4571 7561 6c28 273c 7462 6f64 793e  rtEqual('<tbody>
-00009e40: 3c74 723e 3c74 643e 3c64 6976 2061 6c69  <tr><td><div ali
-00009e50: 676e 3d22 7269 6768 7422 3e30 3030 3c2f  gn="right">000</
-00009e60: 6469 763e 3c2f 7464 3e27 0a20 2020 2020  div></td>'.     
-00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e80: 2020 2020 273c 7464 3e3c 6469 7620 616c      '<td><div al
-00009e90: 6967 6e3d 2272 6967 6874 223e 3030 303c  ign="right">000<
-00009ea0: 2f64 6976 3e3c 2f74 643e 270a 2020 2020  /div></td>'.    
-00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ec0: 2020 2020 2027 3c74 643e 3c64 6976 2061       '<td><div a
-00009ed0: 6c69 676e 3d22 7269 6768 7422 3e30 3030  lign="right">000
-00009ee0: 3c2f 6469 763e 3c2f 7464 3e3c 2f74 723e  </div></td></tr>
-00009ef0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00009f00: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00009f10: 5f6c 696e 652c 0a20 2020 2020 2020 2020  _line,.         
-00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f30: 2266 6169 6c65 6420 6173 5f68 746d 6c20  "failed as_html 
-00009f40: 7769 7468 2064 6174 6120 7479 7065 2066  with data type f
-00009f50: 6f72 6d61 7420 666f 7220 616c 6c20 6669  ormat for all fi
-00009f60: 656c 6473 2229 0a0a 2020 2020 2020 2020  elds")..        
-00009f70: 6874 6d6c 5f6f 7574 7075 7420 3d20 7365  html_output = se
-00009f80: 6c66 2e74 315b 3a31 305d 2e61 735f 6874  lf.t1[:10].as_ht
-00009f90: 6d6c 2866 6965 6c64 733d 2261 2062 2063  ml(fields="a b c
-00009fa0: 222c 2066 6f72 6d61 7473 3d7b 696e 743a  ", formats={int:
-00009fb0: 2022 7b3a 3033 647d 227d 2c20 6772 6f75   "{:03d}"}, grou
-00009fc0: 7062 793d 2261 2229 0a20 2020 2020 2020  pby="a").       
-00009fd0: 2070 7269 6e74 2868 746d 6c5f 6f75 7470   print(html_outp
-00009fe0: 7574 290a 2020 2020 2020 2020 6874 6d6c  ut).        html
-00009ff0: 5f6c 696e 6573 203d 2068 746d 6c5f 6f75  _lines = html_ou
-0000a000: 7470 7574 2e73 706c 6974 6c69 6e65 7328  tput.splitlines(
-0000a010: 290a 2020 2020 2020 2020 6461 7461 5f6c  ).        data_l
-0000a020: 696e 6520 3d20 6e65 7874 2868 2066 6f72  ine = next(h for
-0000a030: 2068 2069 6e20 6874 6d6c 5f6c 696e 6573   h in html_lines
-0000a040: 2069 6620 223c 7464 3e22 2069 6e20 6829   if "<td>" in h)
-0000a050: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000a060: 7365 7274 4571 7561 6c28 273c 7462 6f64  sertEqual('<tbod
-0000a070: 793e 3c74 723e 3c74 643e 3c64 6976 2061  y><tr><td><div a
-0000a080: 6c69 676e 3d22 7269 6768 7422 3e30 3030  lign="right">000
-0000a090: 3c2f 6469 763e 3c2f 7464 3e27 0a20 2020  </div></td>'.   
+00007540: 2020 205b 2741 4e56 494c 2d30 3031 272c     ['ANVIL-001',
+00007550: 2027 4252 4453 442d 3030 3127 2c20 2742   'BRDSD-001', 'B
+00007560: 5244 5344 2d30 3031 272c 2027 4252 4453  RDSD-001', 'BRDS
+00007570: 442d 3030 3127 2c20 274d 4147 4e54 2d30  D-001', 'MAGNT-0
+00007580: 3031 275d 2c0a 2020 2020 2020 2020 2020  01'],.          
+00007590: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000075a0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000075b0: 7365 7274 4571 7561 6c28 3331 2c20 7375  sertEqual(31, su
+000075c0: 6d28 6669 7273 745f 7174 725f 7361 6c65  m(first_qtr_sale
+000075d0: 732e 616c 6c2e 7174 7929 290a 0a20 2020  s.all.qty))..   
+000075e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000075f0: 4571 7561 6c28 3331 2c20 7375 6d28 7361  Equal(31, sum(sa
+00007600: 6c65 732e 6279 2e64 6174 655b 3a22 3230  les.by.date[:"20
+00007610: 3030 2f30 342f 3031 225d 2e61 6c6c 2e71  00/04/01"].all.q
+00007620: 7479 2929 0a20 2020 2020 2020 2073 656c  ty)).        sel
+00007630: 662e 6173 7365 7274 4571 7561 6c28 3936  f.assertEqual(96
+00007640: 2c20 7375 6d28 7361 6c65 732e 6279 2e64  , sum(sales.by.d
+00007650: 6174 655b 2232 3030 302f 3034 2f30 3122  ate["2000/04/01"
+00007660: 3a5d 2e61 6c6c 2e71 7479 2929 0a0a 2020  :].all.qty))..  
+00007670: 2020 6465 6620 7465 7374 5f69 6e64 6578    def test_index
+00007680: 5f64 6972 2873 656c 6629 3a0a 2020 2020  _dir(self):.    
+00007690: 2020 2020 6368 6172 7320 3d20 2241 4243      chars = "ABC
+000076a0: 4445 4647 4849 4a4b 4c4d 4e4f 5051 5253  DEFGHIJKLMNOPQRS
+000076b0: 5455 5657 5859 5a22 0a20 2020 2020 2020  TUVWXYZ".       
+000076c0: 206d 616b 655f 7265 6320 3d20 6c61 6d62   make_rec = lamb
+000076d0: 6461 2061 612c 2062 622c 2063 633a 2073  da aa, bb, cc: s
+000076e0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+000076f0: 6a65 6374 2863 6861 7273 5b61 6120 2520  ject(chars[aa % 
+00007700: 6c65 6e28 6368 6172 7329 5d2c 0a20 2020  len(chars)],.   
+00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007740: 2020 2020 2020 2020 2063 6861 7273 5b62           chars[b
+00007750: 6220 2520 6c65 6e28 6368 6172 7329 5d2c  b % len(chars)],
+00007760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007790: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+000077a0: 7273 5b63 6320 2520 6c65 6e28 6368 6172  rs[cc % len(char
+000077b0: 7329 5d29 0a20 2020 2020 2020 2074 6573  s)]).        tes
+000077c0: 745f 7369 7a65 203d 2031 300a 2020 2020  t_size = 10.    
+000077d0: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
+000077e0: 5f74 6573 745f 7461 626c 6528 6d61 6b65  _test_table(make
+000077f0: 5f72 6563 2c20 7465 7374 5f73 697a 6529  _rec, test_size)
+00007800: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
+00007810: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
+00007820: 0a20 2020 2020 2020 2074 6162 6c65 2e63  .        table.c
+00007830: 7265 6174 655f 696e 6465 7828 2762 2729  reate_index('b')
+00007840: 0a0a 2020 2020 2020 2020 6469 725f 6c69  ..        dir_li
+00007850: 7374 203d 2064 6972 2874 6162 6c65 2e62  st = dir(table.b
+00007860: 7929 0a20 2020 2020 2020 2070 7269 6e74  y).        print
+00007870: 285b 6174 7472 2066 6f72 2061 7474 7220  ([attr for attr 
+00007880: 696e 2064 6972 5f6c 6973 7420 6966 206e  in dir_list if n
+00007890: 6f74 2061 7474 722e 7374 6172 7473 7769  ot attr.startswi
+000078a0: 7468 2822 5f22 295d 290a 0a20 2020 2020  th("_")])..     
+000078b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+000078c0: 7565 2828 2761 2720 696e 2064 6972 5f6c  ue(('a' in dir_l
+000078d0: 6973 7429 2061 6e64 2028 2762 2720 696e  ist) and ('b' in
+000078e0: 2064 6972 5f6c 6973 7429 2061 6e64 2028   dir_list) and (
+000078f0: 2763 2720 6e6f 7420 696e 2064 6972 5f6c  'c' not in dir_l
+00007900: 6973 7429 290a 0a20 2020 2064 6566 2074  ist))..    def t
+00007910: 6573 745f 6465 6c65 7465 5f62 795f 6669  est_delete_by_fi
+00007920: 6c74 6572 2873 656c 6629 3a0a 2020 2020  lter(self):.    
+00007930: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+00007940: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
+00007950: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00007960: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+00007970: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+00007980: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
+00007990: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+000079a0: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+000079b0: 7a65 2c20 7461 626c 652e 6465 6c65 7465  ze, table.delete
+000079c0: 2862 3d35 2929 0a20 2020 2020 2020 2073  (b=5)).        s
+000079d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000079e0: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
+000079f0: 697a 652a 2874 6573 745f 7369 7a65 2d31  ize*(test_size-1
+00007a00: 292c 206c 656e 2874 6162 6c65 2929 0a20  ), len(table)). 
+00007a10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00007a20: 7274 4571 7561 6c28 302c 2074 6162 6c65  rtEqual(0, table
+00007a30: 2e64 656c 6574 6528 623d 2d31 2929 0a20  .delete(b=-1)). 
+00007a40: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00007a50: 7274 4571 7561 6c28 302c 2074 6162 6c65  rtEqual(0, table
+00007a60: 2e64 656c 6574 6528 2929 0a0a 2020 2020  .delete())..    
+00007a70: 6465 6620 7465 7374 5f72 656d 6f76 655f  def test_remove_
+00007a80: 6d61 6e79 2873 656c 6629 3a0a 2020 2020  many(self):.    
+00007a90: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+00007aa0: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
+00007ab0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00007ac0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+00007ad0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+00007ae0: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
+00007af0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00007b00: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00007b10: 7a65 2a74 6573 745f 7369 7a65 2f32 2c20  ze*test_size/2, 
+00007b20: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
+00007b30: 6c61 6d62 6461 2074 3a20 742e 6120 2520  lambda t: t.a % 
+00007b40: 3229 2929 0a20 2020 2020 2020 2074 6162  2))).        tab
+00007b50: 6c65 2e72 656d 6f76 655f 6d61 6e79 2874  le.remove_many(t
+00007b60: 6162 6c65 2e77 6865 7265 286c 616d 6264  able.where(lambd
+00007b70: 6120 743a 2074 2e61 2025 2032 2929 0a20  a t: t.a % 2)). 
+00007b80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00007b90: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+00007ba0: 652a 7465 7374 5f73 697a 652a 7465 7374  e*test_size*test
+00007bb0: 5f73 697a 652f 322c 206c 656e 2874 6162  _size/2, len(tab
+00007bc0: 6c65 2929 0a20 2020 2020 2020 2074 6162  le)).        tab
+00007bd0: 6c65 5f6c 656e 203d 206c 656e 2874 6162  le_len = len(tab
+00007be0: 6c65 290a 2020 2020 2020 2020 7461 626c  le).        tabl
+00007bf0: 652e 7265 6d6f 7665 2874 6162 6c65 5b31  e.remove(table[1
+00007c00: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+00007c10: 6173 7365 7274 4571 7561 6c28 7461 626c  assertEqual(tabl
+00007c20: 655f 6c65 6e2d 312c 206c 656e 2874 6162  e_len-1, len(tab
+00007c30: 6c65 2929 0a0a 2020 2020 6465 6620 7465  le))..    def te
+00007c40: 7374 5f61 6464 5f6e 6577 5f66 6965 6c64  st_add_new_field
+00007c50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007c60: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
+00007c70: 2020 2020 2020 2074 6162 6c65 203d 206d         table = m
+00007c80: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
+00007c90: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+00007ca0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
+00007cb0: 0a0a 2020 2020 2020 2020 2320 6e6f 7420  ..        # not 
+00007cc0: 616c 6c20 7374 6f72 6167 6520 636c 6173  all storage clas
+00007cd0: 7365 7320 7375 7070 6f72 7420 6164 6469  ses support addi
+00007ce0: 6e67 206e 6577 2066 6965 6c64 730a 2020  ng new fields.  
+00007cf0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00007d00: 6f72 6167 655f 7375 7070 6f72 7473 5f61  orage_supports_a
+00007d10: 6464 5f66 6965 6c64 3a0a 2020 2020 2020  dd_field:.      
+00007d20: 2020 2020 2020 7461 626c 652e 6164 645f        table.add_
+00007d30: 6669 656c 6428 2764 272c 206c 616d 6264  field('d', lambd
+00007d40: 6120 7265 633a 2072 6563 2e61 2b72 6563  a rec: rec.a+rec
+00007d50: 2e62 2b72 6563 2e63 290a 0a20 2020 2020  .b+rec.c)..     
+00007d60: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+00007d70: 6174 655f 696e 6465 7828 2764 2729 0a20  ate_index('d'). 
+00007d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007d90: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00007da0: 7261 6e67 6528 302c 2032 372b 3129 292c  range(0, 27+1)),
+00007db0: 206c 656e 2874 6162 6c65 2e62 792e 642e   len(table.by.d.
+00007dc0: 6b65 7973 2829 2929 0a0a 2020 2020 6465  keys()))..    de
+00007dd0: 6620 7465 7374 5f61 6464 5f66 6965 6c64  f test_add_field
+00007de0: 5f6f 7665 725f 6578 6973 7469 6e67 5f69  _over_existing_i
+00007df0: 6e64 6578 6564 5f66 6965 6c64 2873 656c  ndexed_field(sel
+00007e00: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+00007e10: 5f73 697a 6520 3d20 320a 2020 2020 2020  _size = 2.      
+00007e20: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00007e30: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00007e40: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00007e50: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
+00007e60: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
+00007e70: 5f69 6e64 6578 2827 6327 290a 0a20 2020  _index('c')..   
+00007e80: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00007e90: 2e73 746f 7261 6765 5f69 735f 6d75 7461  .storage_is_muta
+00007ea0: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
+00007eb0: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
+00007ec0: 2074 6162 6c65 2e61 6464 5f66 6965 6c64   table.add_field
+00007ed0: 2827 6327 2c20 6c61 6d62 6461 2072 6563  ('c', lambda rec
+00007ee0: 3a20 2d31 290a 2020 2020 2020 2020 7365  : -1).        se
+00007ef0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00007f00: 2020 2020 2020 2020 2020 2020 5b72 6563              [rec
+00007f10: 2e63 2066 6f72 2072 6563 2069 6e20 7461  .c for rec in ta
+00007f20: 626c 655d 2c0a 2020 2020 2020 2020 2020  ble],.          
+00007f30: 2020 6c69 7374 2874 6162 6c65 2e61 6c6c    list(table.all
+00007f40: 2e63 292c 0a20 2020 2020 2020 2020 2020  .c),.           
+00007f50: 2022 616c 6c20 6c69 7374 2072 6561 6473   "all list reads
+00007f60: 2069 6e64 6578 2c20 7768 6963 6820 6973   index, which is
+00007f70: 206e 6f74 2072 6562 7569 6c74 2062 7920   not rebuilt by 
+00007f80: 6164 645f 6669 656c 6422 2c0a 2020 2020  add_field",.    
+00007f90: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+00007fa0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007fb0: 0a20 2020 2020 2020 2020 2020 207b 2d31  .            {-1
+00007fc0: 7d2c 0a20 2020 2020 2020 2020 2020 2073  },.            s
+00007fd0: 6574 2874 6162 6c65 2e62 792e 632e 6b65  et(table.by.c.ke
+00007fe0: 7973 2829 292c 0a20 2020 2020 2020 2020  ys()),.         
+00007ff0: 2020 2022 696e 6465 7820 6b65 7973 2061     "index keys a
+00008000: 7265 206e 6f74 2072 6562 7569 6c74 2062  re not rebuilt b
+00008010: 7920 6164 645f 6669 656c 6422 2c0a 2020  y add_field",.  
+00008020: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00008030: 2074 6573 745f 7573 696e 675f 6163 6365   test_using_acce
+00008040: 7373 6f72 735f 7769 7468 5f66 6965 6c64  ssors_with_field
+00008050: 5f6e 616d 655f 7468 6174 5f69 735f 696e  _name_that_is_in
+00008060: 7661 6c69 645f 7079 7468 6f6e 5f69 6465  valid_python_ide
+00008070: 6e74 6966 6965 7228 7365 6c66 293a 0a20  ntifier(self):. 
+00008080: 2020 2020 2020 2023 2065 7863 6572 7074         # excerpt
+00008090: 2066 726f 6d20 6874 7470 733a 2f2f 6769   from https://gi
+000080a0: 7468 7562 2e63 6f6d 2f6c 756b 6573 2f49  thub.com/lukes/I
+000080b0: 534f 2d33 3136 362d 436f 756e 7472 6965  SO-3166-Countrie
+000080c0: 732d 7769 7468 2d52 6567 696f 6e61 6c2d  s-with-Regional-
+000080d0: 436f 6465 732f 626c 6f62 2f6d 6173 7465  Codes/blob/maste
+000080e0: 722f 616c 6c2f 616c 6c2e 6373 763f 7261  r/all/all.csv?ra
+000080f0: 773d 7472 7565 0a20 2020 2020 2020 2064  w=true.        d
+00008100: 6174 6120 3d20 7465 7874 7772 6170 2e64  ata = textwrap.d
+00008110: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
+00008120: 2020 206e 616d 652c 616c 7068 612d 322c     name,alpha-2,
+00008130: 616c 7068 612d 332c 636f 756e 7472 792d  alpha-3,country-
+00008140: 636f 6465 2c69 736f 5f33 3136 362d 322c  code,iso_3166-2,
+00008150: 7265 6769 6f6e 2c73 7562 2d72 6567 696f  region,sub-regio
+00008160: 6e2c 696e 7465 726d 6564 6961 7465 2d72  n,intermediate-r
+00008170: 6567 696f 6e2c 7265 6769 6f6e 2d63 6f64  egion,region-cod
+00008180: 652c 7375 622d 7265 6769 6f6e 2d63 6f64  e,sub-region-cod
+00008190: 652c 696e 7465 726d 6564 6961 7465 2d72  e,intermediate-r
+000081a0: 6567 696f 6e2d 636f 6465 0a20 2020 2020  egion-code.     
+000081b0: 2020 2041 6667 6861 6e69 7374 616e 2c41     Afghanistan,A
+000081c0: 462c 4146 472c 3030 342c 4953 4f20 3331  F,AFG,004,ISO 31
+000081d0: 3636 2d32 3a41 462c 4173 6961 2c53 6f75  66-2:AF,Asia,Sou
+000081e0: 7468 6572 6e20 4173 6961 2c22 222c 3134  thern Asia,"",14
+000081f0: 322c 3033 342c 2222 0a20 2020 2020 2020  2,034,"".       
+00008200: 20c3 856c 616e 6420 4973 6c61 6e64 732c   ..land Islands,
+00008210: 4158 2c41 4c41 2c32 3438 2c49 534f 2033  AX,ALA,248,ISO 3
+00008220: 3136 362d 323a 4158 2c45 7572 6f70 652c  166-2:AX,Europe,
+00008230: 4e6f 7274 6865 726e 2045 7572 6f70 652c  Northern Europe,
+00008240: 2222 2c31 3530 2c31 3534 2c22 220a 2020  "",150,154,"".  
+00008250: 2020 2020 2020 416c 6261 6e69 612c 414c        Albania,AL
+00008260: 2c41 4c42 2c30 3038 2c49 534f 2033 3136  ,ALB,008,ISO 316
+00008270: 362d 323a 414c 2c45 7572 6f70 652c 536f  6-2:AL,Europe,So
+00008280: 7574 6865 726e 2045 7572 6f70 652c 2222  uthern Europe,""
+00008290: 2c31 3530 2c30 3339 2c22 220a 2020 2020  ,150,039,"".    
+000082a0: 2020 2020 416c 6765 7269 612c 445a 2c44      Algeria,DZ,D
+000082b0: 5a41 2c30 3132 2c49 534f 2033 3136 362d  ZA,012,ISO 3166-
+000082c0: 323a 445a 2c41 6672 6963 612c 4e6f 7274  2:DZ,Africa,Nort
+000082d0: 6865 726e 2041 6672 6963 612c 2222 2c30  hern Africa,"",0
+000082e0: 3032 2c30 3135 2c22 220a 2020 2020 2020  02,015,"".      
+000082f0: 2020 416d 6572 6963 616e 2053 616d 6f61    American Samoa
+00008300: 2c41 532c 4153 4d2c 3031 362c 4953 4f20  ,AS,ASM,016,ISO 
+00008310: 3331 3636 2d32 3a41 532c 4f63 6561 6e69  3166-2:AS,Oceani
+00008320: 612c 506f 6c79 6e65 7369 612c 2222 2c30  a,Polynesia,"",0
+00008330: 3039 2c30 3631 2c22 220a 2020 2020 2020  09,061,"".      
+00008340: 2020 416e 646f 7272 612c 4144 2c41 4e44    Andorra,AD,AND
+00008350: 2c30 3230 2c49 534f 2033 3136 362d 323a  ,020,ISO 3166-2:
+00008360: 4144 2c45 7572 6f70 652c 536f 7574 6865  AD,Europe,Southe
+00008370: 726e 2045 7572 6f70 652c 2222 2c31 3530  rn Europe,"",150
+00008380: 2c30 3339 2c22 220a 2020 2020 2020 2020  ,039,"".        
+00008390: 416e 676f 6c61 2c41 4f2c 4147 4f2c 3032  Angola,AO,AGO,02
+000083a0: 342c 4953 4f20 3331 3636 2d32 3a41 4f2c  4,ISO 3166-2:AO,
+000083b0: 4166 7269 6361 2c53 7562 2d53 6168 6172  Africa,Sub-Sahar
+000083c0: 616e 2041 6672 6963 612c 4d69 6464 6c65  an Africa,Middle
+000083d0: 2041 6672 6963 612c 3030 322c 3230 322c   Africa,002,202,
+000083e0: 3031 370a 2020 2020 2020 2020 2222 2229  017.        """)
+000083f0: 0a20 2020 2020 2020 2074 626c 203d 206c  .        tbl = l
+00008400: 742e 6373 765f 696d 706f 7274 2864 6174  t.csv_import(dat
+00008410: 6129 0a0a 2020 2020 2020 2020 2320 7465  a)..        # te
+00008420: 7374 2027 616c 6c27 2061 6363 6573 736f  st 'all' accesso
+00008430: 720a 2020 2020 2020 2020 7365 6c66 2e61  r.        self.a
+00008440: 7373 6572 7445 7175 616c 285b 2741 7369  ssertEqual(['Asi
+00008450: 6127 2c20 2745 7572 6f70 6527 2c20 2741  a', 'Europe', 'A
+00008460: 6672 6963 6127 2c20 274f 6365 616e 6961  frica', 'Oceania
+00008470: 275d 2c20 6c69 7374 2874 626c 2e61 6c6c  '], list(tbl.all
+00008480: 2e72 6567 696f 6e2e 756e 6971 7565 2929  .region.unique))
+00008490: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000084a0: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+000084b0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+000084c0: 2020 2020 2020 2020 2027 536f 7574 6865           'Southe
+000084d0: 726e 2041 7369 6127 2c0a 2020 2020 2020  rn Asia',.      
+000084e0: 2020 2020 2020 2020 2020 274e 6f72 7468            'North
+000084f0: 6572 6e20 4575 726f 7065 272c 0a20 2020  ern Europe',.   
+00008500: 2020 2020 2020 2020 2020 2020 2027 536f               'So
+00008510: 7574 6865 726e 2045 7572 6f70 6527 2c0a  uthern Europe',.
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 274e 6f72 7468 6572 6e20 4166 7269 6361  'Northern Africa
+00008540: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00008550: 2020 2027 506f 6c79 6e65 7369 6127 2c0a     'Polynesia',.
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2753 7562 2d53 6168 6172 616e 2041 6672  'Sub-Saharan Afr
+00008580: 6963 6127 2c0a 2020 2020 2020 2020 2020  ica',.          
+00008590: 2020 5d2c 206c 6973 7428 7462 6c2e 616c    ], list(tbl.al
+000085a0: 6c28 2273 7562 2d72 6567 696f 6e22 292e  l("sub-region").
+000085b0: 756e 6971 7565 2929 0a0a 2020 2020 2020  unique))..      
+000085c0: 2020 2320 7465 7374 2027 6279 2720 6163    # test 'by' ac
+000085d0: 6365 7373 6f72 0a20 2020 2020 2020 2074  cessor.        t
+000085e0: 626c 2e63 7265 6174 655f 696e 6465 7828  bl.create_index(
+000085f0: 2273 7562 2d72 6567 696f 6e22 290a 2020  "sub-region").  
+00008600: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008610: 7445 7175 616c 285b 2741 6c62 616e 6961  tEqual(['Albania
+00008620: 272c 2027 416e 646f 7272 6127 5d2c 206c  ', 'Andorra'], l
+00008630: 6973 7428 7462 6c2e 6279 2822 7375 622d  ist(tbl.by("sub-
+00008640: 7265 6769 6f6e 2229 5b22 536f 7574 6865  region")["Southe
+00008650: 726e 2045 7572 6f70 6522 5d2e 616c 6c2e  rn Europe"].all.
+00008660: 6e61 6d65 2929 0a0a 2020 2020 2020 2020  name))..        
+00008670: 2320 7465 7374 2027 7365 6172 6368 2720  # test 'search' 
+00008680: 6163 6365 7373 6f72 0a20 2020 2020 2020  accessor.       
+00008690: 2074 626c 2e63 7265 6174 655f 7365 6172   tbl.create_sear
+000086a0: 6368 5f69 6e64 6578 2822 7375 622d 7265  ch_index("sub-re
+000086b0: 6769 6f6e 2229 0a20 2020 2020 2020 2073  gion").        s
+000086c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000086d0: 0a20 2020 2020 2020 2020 2020 205b 27c3  .            ['.
+000086e0: 856c 616e 6420 4973 6c61 6e64 7327 2c20  .land Islands', 
+000086f0: 2741 6c62 616e 6961 272c 2027 416e 646f  'Albania', 'Ando
+00008700: 7272 6127 5d2c 0a20 2020 2020 2020 2020  rra'],.         
+00008710: 2020 206c 6973 7428 7462 6c2e 7365 6172     list(tbl.sear
+00008720: 6368 2822 7375 622d 7265 6769 6f6e 2229  ch("sub-region")
+00008730: 2822 4575 726f 7065 2229 2e61 6c6c 2e6e  ("Europe").all.n
+00008740: 616d 6529 0a20 2020 2020 2020 2029 0a0a  ame).        )..
+00008750: 2020 2020 6465 6620 7465 7374 5f61 6464      def test_add
+00008760: 5f74 776f 5f74 6162 6c65 7328 7365 6c66  _two_tables(self
+00008770: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+00008780: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00008790: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+000087a0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+000087b0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+000087c0: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
+000087d0: 206d 616b 655f 7265 6320 3d20 6c61 6d62   make_rec = lamb
+000087e0: 6461 2061 2c62 2c63 3a20 7365 6c66 2e6d  da a,b,c: self.m
+000087f0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00008800: 612b 7465 7374 5f73 697a 652c 2062 2c20  a+test_size, b, 
+00008810: 6329 0a20 2020 2020 2020 2074 3220 3d20  c).        t2 = 
+00008820: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+00008830: 6d61 6b65 5f72 6563 2c20 7465 7374 5f73  make_rec, test_s
+00008840: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
+00008850: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00008860: 6573 745f 7369 7a65 2a74 6573 745f 7369  est_size*test_si
+00008870: 7a65 2a74 6573 745f 7369 7a65 2a32 2c20  ze*test_size*2, 
+00008880: 6c65 6e28 7431 2b74 3229 290a 2020 2020  len(t1+t2)).    
+00008890: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000088a0: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
+000088b0: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
+000088c0: 745f 7369 7a65 2c20 6c65 6e28 7431 2929  t_size, len(t1))
+000088d0: 0a0a 2020 2020 2020 2020 7431 202b 3d20  ..        t1 += 
+000088e0: 7432 0a20 2020 2020 2020 2073 656c 662e  t2.        self.
+000088f0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+00008900: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00008910: 6520 2a20 7465 7374 5f73 697a 6520 2a20  e * test_size * 
+00008920: 322c 206c 656e 2874 3129 290a 0a20 2020  2, len(t1))..   
+00008930: 2020 2020 206f 6666 7365 7420 3d20 7465       offset = te
+00008940: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
+00008950: 697a 650a 2020 2020 2020 2020 7433 203d  ize.        t3 =
+00008960: 2074 3120 2b20 2873 656c 662e 6d61 6b65   t1 + (self.make
+00008970: 5f64 6174 615f 6f62 6a65 6374 2872 6563  _data_object(rec
+00008980: 2e61 2b6f 6666 7365 742c 2072 6563 2e62  .a+offset, rec.b
+00008990: 2c20 7265 632e 6329 2066 6f72 2072 6563  , rec.c) for rec
+000089a0: 2069 6e20 7432 290a 2020 2020 2020 2020   in t2).        
+000089b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000089c0: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+000089d0: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
+000089e0: 7a65 202a 2033 2c20 6c65 6e28 7433 2929  ze * 3, len(t3))
+000089f0: 0a0a 2020 2020 6465 6620 7465 7374 5f74  ..    def test_t
+00008a00: 6162 6c65 5f69 6e66 6f28 7365 6c66 293a  able_info(self):
+00008a10: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00008a20: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
+00008a30: 7769 7468 2074 696d 6573 7461 6d70 5f73  with timestamp_s
+00008a40: 7461 7274 5f65 6e64 2829 2061 7320 7469  tart_end() as ti
+00008a50: 6d69 6e67 3a0a 2020 2020 2020 2020 2020  ming:.          
+00008a60: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00008a70: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00008a80: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00008a90: 7374 5f73 697a 6529 2827 696e 666f 5f74  st_size)('info_t
+00008aa0: 6573 7427 290a 0a20 2020 2020 2020 2074  est')..        t
+00008ab0: 312e 6372 6561 7465 5f69 6e64 6578 2827  1.create_index('
+00008ac0: 6227 290a 2020 2020 2020 2020 7431 5f69  b').        t1_i
+00008ad0: 6e66 6f20 3d20 7431 2e69 6e66 6f28 290a  nfo = t1.info().
+00008ae0: 2020 2020 2020 2020 2320 6d75 7374 2073          # must s
+00008af0: 6f72 7420 6669 656c 6473 2061 6e64 2069  ort fields and i
+00008b00: 6e64 6578 6573 2076 616c 7565 732c 2066  ndexes values, f
+00008b10: 6f72 2074 6573 7420 636f 6d70 6172 6973  or test comparis
+00008b20: 6f6e 730a 2020 2020 2020 2020 7431 5f69  ons.        t1_i
+00008b30: 6e66 6f5b 2766 6965 6c64 7327 5d2e 736f  nfo['fields'].so
+00008b40: 7274 2829 0a20 2020 2020 2020 2074 315f  rt().        t1_
+00008b50: 696e 666f 5b27 696e 6465 7865 7327 5d2e  info['indexes'].
+00008b60: 736f 7274 2829 0a20 2020 2020 2020 2073  sort().        s
+00008b70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00008b80: 4e6f 6e65 2c20 7431 5f69 6e66 6f2e 706f  None, t1_info.po
+00008b90: 7028 226c 6173 745f 696d 706f 7274 2229  p("last_import")
+00008ba0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00008bb0: 7373 6572 7454 7275 6528 7469 6d69 6e67  ssertTrue(timing
+00008bc0: 2e73 7461 7274 203c 3d20 7431 5f69 6e66  .start <= t1_inf
+00008bd0: 6f2e 706f 7028 2263 7265 6174 6564 2229  o.pop("created")
+00008be0: 203c 3d20 7469 6d69 6e67 2e65 6e64 290a   <= timing.end).
+00008bf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008c00: 6572 7454 7275 6528 7469 6d69 6e67 2e73  ertTrue(timing.s
+00008c10: 7461 7274 203c 3d20 7431 5f69 6e66 6f2e  tart <= t1_info.
+00008c20: 706f 7028 226d 6f64 6966 6965 6422 2920  pop("modified") 
+00008c30: 3c3d 2074 696d 696e 672e 656e 6429 0a20  <= timing.end). 
+00008c40: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00008c50: 7274 4571 7561 6c28 7b27 6669 656c 6473  rtEqual({'fields
+00008c60: 273a 205b 2761 272c 2027 6227 2c20 2763  ': ['a', 'b', 'c
+00008c70: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+00008c90: 6e64 6578 6573 273a 205b 2827 6227 2c20  ndexes': [('b', 
+00008ca0: 4661 6c73 6529 5d2c 0a20 2020 2020 2020  False)],.       
+00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cc0: 2020 2027 6c65 6e27 3a20 3130 3030 2c0a     'len': 1000,.
+00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ce0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+00008cf0: 3a20 2769 6e66 6f5f 7465 7374 277d 2c0a  : 'info_test'},.
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2020 2020 2020 2020 2074 315f 696e 666f           t1_info
+00008d20: 2c20 2269 6e76 616c 6964 2069 6e66 6f20  , "invalid info 
+00008d30: 7265 7375 6c74 7322 290a 0a0a 406d 616b  results")...@mak
+00008d40: 655f 7465 7374 5f63 6c61 7373 6573 0a63  e_test_classes.c
+00008d50: 6c61 7373 2054 6162 6c65 4c69 7374 5465  lass TableListTe
+00008d60: 7374 733a 0a20 2020 2022 2222 0a20 2020  sts:.    """.   
+00008d70: 2054 6573 7473 2066 6f72 2061 6363 6573   Tests for acces
+00008d80: 7369 6e67 2054 6162 6c65 7320 6173 206c  sing Tables as l
+00008d90: 6973 7473 2e0a 2020 2020 2222 220a 2020  ists..    """.  
+00008da0: 2020 6465 6620 5f74 6573 745f 696e 6974    def _test_init
+00008db0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008dc0: 7365 6c66 2e74 6573 745f 7369 7a65 203d  self.test_size =
+00008dd0: 2033 0a20 2020 2020 2020 2073 656c 662e   3.        self.
+00008de0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
+00008df0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00008e00: 6174 615f 6f62 6a65 6374 2c20 7365 6c66  ata_object, self
+00008e10: 2e74 6573 745f 7369 7a65 290a 2020 2020  .test_size).    
+00008e20: 2020 2020 7365 6c66 2e74 6573 745f 7265      self.test_re
+00008e30: 6320 3d20 7365 6c66 2e6d 616b 655f 6461  c = self.make_da
+00008e40: 7461 5f6f 626a 6563 7428 312c 2031 2c20  ta_object(1, 1, 
+00008e50: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
+00008e60: 5f63 6f6e 7461 696e 7328 7365 6c66 293a  _contains(self):
+00008e70: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+00008e80: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
+00008e90: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00008ea0: 7565 2873 656c 662e 7465 7374 5f72 6563  ue(self.test_rec
+00008eb0: 2069 6e20 7365 6c66 2e74 312c 2022 6661   in self.t1, "fa
+00008ec0: 696c 6564 2027 696e 2720 2863 6f6e 7461  iled 'in' (conta
+00008ed0: 696e 7329 2074 6573 7422 290a 0a20 2020  ins) test")..   
+00008ee0: 2064 6566 2074 6573 745f 696e 6465 785f   def test_index_
+00008ef0: 6669 6e64 2873 656c 6629 3a0a 2020 2020  find(self):.    
+00008f00: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+00008f10: 6e69 7428 290a 2020 2020 2020 2020 7365  nit().        se
+00008f20: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
+00008f30: 332c 2073 656c 662e 7431 2e69 6e64 6578  3, self.t1.index
+00008f40: 2873 656c 662e 7465 7374 5f72 6563 292c  (self.test_rec),
+00008f50: 2022 6661 696c 6564 2027 696e 6465 783b   "failed 'index;
+00008f60: 2074 6573 7420 2865 7869 7374 7329 2229   test (exists)")
+00008f70: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00008f80: 7374 616e 6365 2873 656c 662e 7465 7374  stance(self.test
+00008f90: 5f72 6563 2c20 5369 6d70 6c65 4e61 6d65  _rec, SimpleName
+00008fa0: 7370 6163 6529 3a0a 2020 2020 2020 2020  space):.        
+00008fb0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00008fc0: 7175 616c 2831 332c 2073 656c 662e 7431  qual(13, self.t1
+00008fd0: 2e69 6e64 6578 2876 6172 7328 7365 6c66  .index(vars(self
+00008fe0: 2e74 6573 745f 7265 6329 292c 2022 6661  .test_rec)), "fa
+00008ff0: 696c 6564 2027 696e 6465 783b 2074 6573  iled 'index; tes
+00009000: 7420 2865 7869 7374 7329 2229 0a0a 2020  t (exists)")..  
+00009010: 2020 2020 2020 6e6f 5f73 7563 685f 7265        no_such_re
+00009020: 6320 3d20 7365 6c66 2e6d 616b 655f 6461  c = self.make_da
+00009030: 7461 5f6f 626a 6563 7428 7365 6c66 2e74  ta_object(self.t
+00009040: 6573 745f 7369 7a65 2b31 2c20 7365 6c66  est_size+1, self
+00009050: 2e74 6573 745f 7369 7a65 2b31 2c20 7365  .test_size+1, se
+00009060: 6c66 2e74 6573 745f 7369 7a65 2b31 290a  lf.test_size+1).
+00009070: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00009080: 662e 6173 7365 7274 5261 6973 6573 2856  f.assertRaises(V
+00009090: 616c 7565 4572 726f 722c 206d 7367 3d22  alueError, msg="
+000090a0: 6661 696c 6564 2027 696e 6465 7827 2074  failed 'index' t
+000090b0: 6573 7420 286e 6f74 2065 7869 7374 7329  est (not exists)
+000090c0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000090d0: 7365 6c66 2e74 312e 696e 6465 7828 6e6f  self.t1.index(no
+000090e0: 5f73 7563 685f 7265 6329 0a0a 2020 2020  _such_rec)..    
+000090f0: 6465 6620 7465 7374 5f72 656d 6f76 6528  def test_remove(
+00009100: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00009110: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
+00009120: 0a20 2020 2020 2020 2072 6563 203d 2073  .        rec = s
+00009130: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+00009140: 6a65 6374 2831 2c20 312c 2031 290a 2020  ject(1, 1, 1).  
+00009150: 2020 2020 2020 7072 6576 5f6c 656e 203d        prev_len =
+00009160: 206c 656e 2873 656c 662e 7431 290a 2020   len(self.t1).  
+00009170: 2020 2020 2020 7365 6c66 2e74 312e 7265        self.t1.re
+00009180: 6d6f 7665 2872 6563 290a 2020 2020 2020  move(rec).      
+00009190: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+000091a0: 7365 2872 6563 2069 6e20 7365 6c66 2e74  se(rec in self.t
+000091b0: 312c 2022 6661 696c 6564 2074 6f20 7265  1, "failed to re
+000091c0: 6d6f 7665 2072 6563 6f72 6420 6672 6f6d  move record from
+000091d0: 2074 6162 6c65 2028 636f 6e74 6169 6e73   table (contains
+000091e0: 2922 290a 2020 2020 2020 2020 7365 6c66  )").        self
+000091f0: 2e61 7373 6572 7445 7175 616c 2870 7265  .assertEqual(pre
+00009200: 765f 6c65 6e2d 312c 206c 656e 2873 656c  v_len-1, len(sel
+00009210: 662e 7431 292c 2022 6661 696c 6564 2074  f.t1), "failed t
+00009220: 6f20 7265 6d6f 7665 2072 6563 6f72 6420  o remove record 
+00009230: 6672 6f6d 2074 6162 6c65 2028 6c65 6e29  from table (len)
+00009240: 2229 0a0a 2020 2020 2020 2020 6e6f 5f73  ")..        no_s
+00009250: 7563 685f 7265 6320 3d20 7365 6c66 2e6d  uch_rec = self.m
+00009260: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00009270: 7365 6c66 2e74 6573 745f 7369 7a65 2b31  self.test_size+1
+00009280: 2c20 7365 6c66 2e74 6573 745f 7369 7a65  , self.test_size
+00009290: 2b31 2c20 7365 6c66 2e74 6573 745f 7369  +1, self.test_si
+000092a0: 7a65 2b31 290a 2020 2020 2020 2020 7365  ze+1).        se
+000092b0: 6c66 2e61 7373 6572 7446 616c 7365 286e  lf.assertFalse(n
+000092c0: 6f5f 7375 6368 5f72 6563 2069 6e20 7365  o_such_rec in se
+000092d0: 6c66 2e74 312c 2022 6661 696c 6564 2074  lf.t1, "failed t
+000092e0: 6f20 6372 6561 7465 206e 6f6e 2d65 7869  o create non-exi
+000092f0: 7374 656e 7420 7265 636f 7264 2066 726f  stent record fro
+00009300: 6d20 7461 626c 6522 290a 2020 2020 2020  m table").      
+00009310: 2020 7365 6c66 2e74 312e 7265 6d6f 7665    self.t1.remove
+00009320: 286e 6f5f 7375 6368 5f72 6563 290a 2020  (no_such_rec).  
+00009330: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009340: 7445 7175 616c 2870 7265 765f 6c65 6e2d  tEqual(prev_len-
+00009350: 312c 206c 656e 2873 656c 662e 7431 292c  1, len(self.t1),
+00009360: 2022 6661 696c 6564 2072 656d 6f76 696e   "failed removin
+00009370: 6720 6e6f 6e2d 6578 6973 7465 6e74 2072  g non-existent r
+00009380: 6563 6f72 6420 6672 6f6d 2074 6162 6c65  ecord from table
+00009390: 2028 6c65 6e29 2229 0a0a 2020 2020 2020   (len)")..      
+000093a0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000093b0: 7365 6c66 2e74 6573 745f 7265 632c 2053  self.test_rec, S
+000093c0: 696d 706c 654e 616d 6573 7061 6365 293a  impleNamespace):
+000093d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000093e0: 662e 7431 2e72 656d 6f76 6528 7661 7273  f.t1.remove(vars
+000093f0: 2873 656c 662e 7465 7374 5f72 6563 2929  (self.test_rec))
+00009400: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009410: 662e 6173 7365 7274 4571 7561 6c28 7072  f.assertEqual(pr
+00009420: 6576 5f6c 656e 2d31 2c20 6c65 6e28 7365  ev_len-1, len(se
+00009430: 6c66 2e74 3129 2c20 2266 6169 6c65 6420  lf.t1), "failed 
+00009440: 746f 2072 656d 6f76 6520 7265 636f 7264  to remove record
+00009450: 2061 7320 6469 6374 2066 726f 6d20 7461   as dict from ta
+00009460: 626c 6520 286c 656e 2922 290a 0a20 2020  ble (len)")..   
+00009470: 2064 6566 2074 6573 745f 696e 6465 785f   def test_index_
+00009480: 6163 6365 7373 2873 656c 6629 3a0a 2020  access(self):.  
+00009490: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+000094a0: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+000094b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000094c0: 2873 656c 662e 7465 7374 5f72 6563 2c20  (self.test_rec, 
+000094d0: 7365 6c66 2e74 315b 3133 5d2c 2022 6661  self.t1[13], "fa
+000094e0: 696c 6564 2069 6e64 6578 2061 6363 6573  iled index acces
+000094f0: 7320 7465 7374 2229 0a0a 2020 2020 6465  s test")..    de
+00009500: 6620 7465 7374 5f63 6f75 6e74 2873 656c  f test_count(sel
+00009510: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00009520: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
+00009530: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009540: 7454 7275 6528 7365 6c66 2e74 312e 636f  tTrue(self.t1.co
+00009550: 756e 7428 7365 6c66 2e74 6573 745f 7265  unt(self.test_re
+00009560: 6329 203d 3d20 312c 2022 6661 696c 6564  c) == 1, "failed
+00009570: 2063 6f75 6e74 2074 6573 7422 290a 2020   count test").  
+00009580: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00009590: 6e63 6528 7365 6c66 2e74 6573 745f 7265  nce(self.test_re
+000095a0: 632c 2053 696d 706c 654e 616d 6573 7061  c, SimpleNamespa
+000095b0: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
+000095c0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+000095d0: 2873 656c 662e 7431 2e63 6f75 6e74 2876  (self.t1.count(v
+000095e0: 6172 7328 7365 6c66 2e74 6573 745f 7265  ars(self.test_re
+000095f0: 6329 2920 3d3d 2031 2c20 2266 6169 6c65  c)) == 1, "faile
+00009600: 6420 636f 756e 7420 7465 7374 2229 0a0a  d count test")..
+00009610: 2020 2020 6465 6620 7465 7374 5f64 656c      def test_del
+00009620: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00009630: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
+00009640: 290a 2020 2020 2020 2020 6265 666f 7265  ).        before
+00009650: 5f64 656c 5f6c 656e 203d 206c 656e 2873  _del_len = len(s
+00009660: 656c 662e 7431 290a 2020 2020 2020 2020  elf.t1).        
+00009670: 6465 6c20 7365 6c66 2e74 315b 3133 5d0a  del self.t1[13].
+00009680: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00009690: 6572 7446 616c 7365 2873 656c 662e 7465  ertFalse(self.te
+000096a0: 7374 5f72 6563 2069 6e20 7365 6c66 2e74  st_rec in self.t
+000096b0: 312c 2022 6661 696c 6564 2064 656c 2074  1, "failed del t
+000096c0: 6573 7422 290a 2020 2020 2020 2020 7365  est").        se
+000096d0: 6c66 2e61 7373 6572 7445 7175 616c 2862  lf.assertEqual(b
+000096e0: 6566 6f72 655f 6465 6c5f 6c65 6e20 2d20  efore_del_len - 
+000096f0: 312c 206c 656e 2873 656c 662e 7431 2929  1, len(self.t1))
+00009700: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+00009710: 6f70 2873 656c 6629 3a0a 2020 2020 2020  op(self):.      
+00009720: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+00009730: 7428 290a 2020 2020 2020 2020 6265 666f  t().        befo
+00009740: 7265 5f70 6f70 5f6c 656e 203d 206c 656e  re_pop_len = len
+00009750: 2873 656c 662e 7431 290a 2020 2020 2020  (self.t1).      
+00009760: 2020 6f62 6a20 3d20 7365 6c66 2e74 312e    obj = self.t1.
+00009770: 706f 7028 3133 290a 2020 2020 2020 2020  pop(13).        
+00009780: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00009790: 286f 626a 2069 6e20 7365 6c66 2e74 3129  (obj in self.t1)
+000097a0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000097b0: 7365 7274 4571 7561 6c28 7365 6c66 2e74  sertEqual(self.t
+000097c0: 6573 745f 7265 632c 206f 626a 290a 2020  est_rec, obj).  
+000097d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000097e0: 7445 7175 616c 2862 6566 6f72 655f 706f  tEqual(before_po
+000097f0: 705f 6c65 6e20 2d20 312c 206c 656e 2873  p_len - 1, len(s
+00009800: 656c 662e 7431 2929 0a0a 2020 2020 6465  elf.t1))..    de
+00009810: 6620 7465 7374 5f70 6f70 5f6c 6173 7428  f test_pop_last(
+00009820: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00009830: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
+00009840: 0a20 2020 2020 2020 2062 6566 6f72 655f  .        before_
+00009850: 706f 705f 6c65 6e20 3d20 6c65 6e28 7365  pop_len = len(se
+00009860: 6c66 2e74 3129 0a20 2020 2020 2020 2065  lf.t1).        e
+00009870: 7870 6563 7465 645f 706f 7020 3d20 636f  xpected_pop = co
+00009880: 7079 2e63 6f70 7928 7365 6c66 2e74 315b  py.copy(self.t1[
+00009890: 2d31 5d29 0a20 2020 2020 2020 206f 626a  -1]).        obj
+000098a0: 203d 2073 656c 662e 7431 2e70 6f70 2829   = self.t1.pop()
+000098b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000098c0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
+000098d0: 6564 5f70 6f70 2c20 6f62 6a29 0a20 2020  ed_pop, obj).   
+000098e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000098f0: 4571 7561 6c28 6265 666f 7265 5f70 6f70  Equal(before_pop
+00009900: 5f6c 656e 202d 2031 2c20 6c65 6e28 7365  _len - 1, len(se
+00009910: 6c66 2e74 3129 290a 0a20 2020 2064 6566  lf.t1))..    def
+00009920: 2074 6573 745f 7265 7665 7273 6564 2873   test_reversed(s
+00009930: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00009940: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
+00009950: 2020 2020 2020 2020 6c61 7374 5f72 6563          last_rec
+00009960: 203d 206e 6578 7428 7265 7665 7273 6564   = next(reversed
+00009970: 2873 656c 662e 7431 2929 0a20 2020 2020  (self.t1)).     
+00009980: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00009990: 7561 6c28 7365 6c66 2e6d 616b 655f 6461  ual(self.make_da
+000099a0: 7461 5f6f 626a 6563 7428 322c 2032 2c20  ta_object(2, 2, 
+000099b0: 3229 2c20 6c61 7374 5f72 6563 2c20 2266  2), last_rec, "f
+000099c0: 6169 6c65 6420 7265 7665 7273 6564 2074  ailed reversed t
+000099d0: 6573 7422 290a 0a20 2020 2064 6566 2074  est")..    def t
+000099e0: 6573 745f 6974 6572 2873 656c 6629 3a0a  est_iter(self):.
+000099f0: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00009a00: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+00009a10: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00009a20: 6528 7365 6c66 2e74 6573 745f 7265 6320  e(self.test_rec 
+00009a30: 696e 2073 656c 662e 7431 2c20 2266 6169  in self.t1, "fai
+00009a40: 6c65 6420 2769 6e27 2028 636f 6e74 6169  led 'in' (contai
+00009a50: 6e73 2920 7465 7374 2229 0a0a 2020 2020  ns) test")..    
+00009a60: 6465 6620 7465 7374 5f68 6561 645f 616e  def test_head_an
+00009a70: 645f 7461 696c 2873 656c 6629 3a0a 2020  d_tail(self):.  
+00009a80: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+00009a90: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+00009aa0: 7365 6c66 2e74 312e 6372 6561 7465 5f69  self.t1.create_i
+00009ab0: 6e64 6578 2822 6122 290a 2020 2020 2020  ndex("a").      
+00009ac0: 2020 7365 6c66 2e74 312e 6372 6561 7465    self.t1.create
+00009ad0: 5f69 6e64 6578 2822 6322 290a 2020 2020  _index("c").    
+00009ae0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009af0: 7175 616c 287b 2261 222c 2022 6322 7d2c  qual({"a", "c"},
+00009b00: 2073 6574 2873 656c 662e 7431 2e5f 696e   set(self.t1._in
+00009b10: 6465 7865 732e 6b65 7973 2829 292c 2022  dexes.keys()), "
+00009b20: 6661 696c 6564 2074 6f20 6372 6561 7465  failed to create
+00009b30: 2069 6e64 6578 6573 2229 0a0a 2020 2020   indexes")..    
+00009b40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009b50: 7175 616c 2873 6574 2873 656c 662e 7431  qual(set(self.t1
+00009b60: 2e5f 696e 6465 7865 732e 6b65 7973 2829  ._indexes.keys()
+00009b70: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00009b80: 2020 2020 2020 2020 2020 2020 7365 7428              set(
+00009b90: 7365 6c66 2e74 312e 6865 6164 2829 2e5f  self.t1.head()._
+00009ba0: 696e 6465 7865 732e 6b65 7973 2829 292c  indexes.keys()),
+00009bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bc0: 2020 2020 2020 2020 2020 2266 6169 6c65            "faile
+00009bd0: 6420 746f 2063 6f70 7920 696e 6465 7865  d to copy indexe
+00009be0: 7320 746f 2068 6561 6428 2922 290a 2020  s to head()").  
+00009bf0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009c00: 7445 7175 616c 2873 6574 2873 656c 662e  tEqual(set(self.
+00009c10: 7431 2e5f 696e 6465 7865 732e 6b65 7973  t1._indexes.keys
+00009c20: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
+00009c30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009c40: 7428 7365 6c66 2e74 312e 7461 696c 2829  t(self.t1.tail()
+00009c50: 2e5f 696e 6465 7865 732e 6b65 7973 2829  ._indexes.keys()
+00009c60: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00009c70: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
+00009c80: 6c65 6420 746f 2063 6f70 7920 696e 6465  led to copy inde
+00009c90: 7865 7320 746f 2074 6169 6c28 2922 290a  xes to tail()").
+00009ca0: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
+00009cb0: 6971 7565 2873 656c 6629 3a0a 2020 2020  ique(self):.    
+00009cc0: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+00009cd0: 6e69 7428 290a 2020 2020 2020 2020 7365  nit().        se
+00009ce0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00009cf0: 302c 2031 2c20 325d 2c20 736f 7274 6564  0, 1, 2], sorted
+00009d00: 285b 726f 772e 6120 666f 7220 726f 7720  ([row.a for row 
+00009d10: 696e 2073 656c 662e 7431 2e75 6e69 7175  in self.t1.uniqu
+00009d20: 6528 2761 2729 5d29 2c20 2266 6169 6c65  e('a')]), "faile
+00009d30: 6420 6361 6c6c 2074 6f20 756e 6971 7565  d call to unique
+00009d40: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+00009d50: 5f61 6c6c 5f61 6363 6573 736f 7228 7365  _all_accessor(se
+00009d60: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00009d70: 662e 5f74 6573 745f 696e 6974 2829 0a20  f._test_init(). 
+00009d80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00009d90: 7274 4571 7561 6c28 7375 6d28 285b 695d  rtEqual(sum(([i]
+00009da0: 2a73 656c 662e 7465 7374 5f73 697a 652a  *self.test_size*
+00009db0: 2a32 2066 6f72 2069 2069 6e20 7261 6e67  *2 for i in rang
+00009dc0: 6528 7365 6c66 2e74 6573 745f 7369 7a65  e(self.test_size
+00009dd0: 2929 2c20 5b5d 292c 0a20 2020 2020 2020  )), []),.       
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2020 6c69 7374 2873 656c 662e 7431 2e61    list(self.t1.a
+00009e00: 6c6c 2e61 292c 0a20 2020 2020 2020 2020  ll.a),.         
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e20: 2266 6169 6c65 6420 746f 2073 7563 6365  "failed to succe
+00009e30: 7373 6675 6c6c 7920 6765 7420 616c 6c20  ssfully get all 
+00009e40: 7661 6c75 6573 2069 6e20 2761 2722 290a  values in 'a'").
+00009e50: 0a20 2020 2020 2020 2061 6c6c 5f61 7320  .        all_as 
+00009e60: 3d20 7365 6c66 2e74 312e 616c 6c2e 610a  = self.t1.all.a.
+00009e70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00009e80: 6572 7454 7275 6528 616c 6c5f 6173 2069  ertTrue(all_as i
+00009e90: 7320 6974 6572 2861 6c6c 5f61 7329 2c20  s iter(all_as), 
+00009ea0: 2261 6c6c 2069 7465 7261 746f 7220 6661  "all iterator fa
+00009eb0: 696c 7320 746f 2069 6465 6e74 6966 7920  ils to identify 
+00009ec0: 6173 2069 7465 7228 7365 6c66 2922 290a  as iter(self)").
+00009ed0: 0a20 2020 2064 6566 2074 6573 745f 666f  .    def test_fo
+00009ee0: 726d 6174 2873 656c 6629 3a0a 2020 2020  rmat(self):.    
+00009ef0: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+00009f00: 6e69 7428 290a 2020 2020 2020 2020 7365  nit().        se
+00009f10: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00009f20: 2730 3020 3020 3027 2c20 2730 3020 3020  '00 0 0', '00 0 
+00009f30: 3127 2c20 2730 3020 3020 3227 5d2c 0a20  1', '00 0 2'],. 
+00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f50: 2020 2020 2020 2020 6c69 7374 2873 656c          list(sel
+00009f60: 662e 7431 2e66 6f72 6d61 7428 227b 613a  f.t1.format("{a:
+00009f70: 3032 647d 207b 627d 207b 637d 2229 295b  02d} {b} {c}"))[
+00009f80: 3a33 5d2c 0a20 2020 2020 2020 2020 2020  :3],.           
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00009fa0: 6169 6c65 6420 746f 2063 7265 6174 6520  ailed to create 
+00009fb0: 666f 726d 6174 7465 6420 726f 7773 2229  formatted rows")
+00009fc0: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+00009fd0: 735f 6874 6d6c 2873 656c 6629 3a0a 2020  s_html(self):.  
+00009fe0: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+00009ff0: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+0000a000: 6874 6d6c 5f6f 7574 7075 7420 3d20 7365  html_output = se
+0000a010: 6c66 2e74 315b 3a31 305d 2e61 735f 6874  lf.t1[:10].as_ht
+0000a020: 6d6c 2866 6965 6c64 733d 2261 2062 2063  ml(fields="a b c
+0000a030: 2229 0a20 2020 2020 2020 2070 7269 6e74  ").        print
+0000a040: 2868 746d 6c5f 6f75 7470 7574 290a 2020  (html_output).  
+0000a050: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000a060: 7454 7275 6528 223c 7468 6561 643e 2220  tTrue("<thead>" 
+0000a070: 696e 2068 746d 6c5f 6f75 7470 7574 2061  in html_output a
+0000a080: 6e64 2022 3c74 626f 6479 3e22 2069 6e20  nd "<tbody>" in 
+0000a090: 6874 6d6c 5f6f 7574 7075 742c 0a20 2020  html_output,.   
 0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 2020 2020 273c 7464 3e3c 6469 7620        '<td><div 
-0000a0c0: 616c 6967 6e3d 2272 6967 6874 223e 3030  align="right">00
-0000a0d0: 303c 2f64 6976 3e3c 2f74 643e 270a 2020  0</div></td>'.  
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2020 2020 2027 3c74 643e 3c64 6976         '<td><div
-0000a100: 2061 6c69 676e 3d22 7269 6768 7422 3e30   align="right">0
-0000a110: 3030 3c2f 6469 763e 3c2f 7464 3e3c 2f74  00</div></td></t
-0000a120: 723e 272c 0a20 2020 2020 2020 2020 2020  r>',.           
-0000a130: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000a140: 7461 5f6c 696e 652c 0a20 2020 2020 2020  ta_line,.       
-0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2020 2266 6169 6c65 6420 6173 5f68 746d    "failed as_htm
-0000a170: 6c20 7769 7468 2067 726f 7570 6279 2229  l with groupby")
-0000a180: 0a0a 2020 2020 2020 2020 6874 6d6c 5f6f  ..        html_o
-0000a190: 7574 7075 7420 3d20 7365 6c66 2e74 315b  utput = self.t1[
-0000a1a0: 3a31 305d 2e61 735f 6874 6d6c 2866 6965  :10].as_html(fie
-0000a1b0: 6c64 733d 2261 2062 2063 222c 2074 6162  lds="a b c", tab
-0000a1c0: 6c65 5f70 726f 7065 7274 6965 733d 7b22  le_properties={"
-0000a1d0: 626f 7264 6572 223a 2022 3222 7d29 0a20  border": "2"}). 
-0000a1e0: 2020 2020 2020 2070 7269 6e74 2868 746d         print(htm
-0000a1f0: 6c5f 6f75 7470 7574 290a 2020 2020 2020  l_output).      
-0000a200: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-0000a210: 6528 223c 7468 6561 643e 2220 696e 2068  e("<thead>" in h
-0000a220: 746d 6c5f 6f75 7470 7574 2061 6e64 2022  tml_output and "
-0000a230: 3c74 626f 6479 3e22 2069 6e20 6874 6d6c  <tbody>" in html
-0000a240: 5f6f 7574 7075 742c 0a20 2020 2020 2020  _output,.       
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2022 6173 5f68 746d 6c20 646f 6573 206e   "as_html does n
-0000a270: 6f74 2069 6e63 6c75 6465 2074 6865 6164  ot include thead
-0000a280: 2061 6e64 2074 626f 6479 2074 6167 7322   and tbody tags"
-0000a290: 290a 0a0a 2020 2020 6465 6620 7465 7374  )...    def test
-0000a2a0: 5f64 656c 6574 655f 736c 6963 6573 2873  _delete_slices(s
-0000a2b0: 656c 6629 3a0a 2020 2020 2020 2020 636f  elf):.        co
-0000a2c0: 6d70 6172 655f 6c69 7374 203d 206c 6973  mpare_list = lis
-0000a2d0: 7428 2241 4243 4445 4647 4849 4a4b 4c4d  t("ABCDEFGHIJKLM
-0000a2e0: 4e4f 5051 5253 5455 5657 5859 5a30 3132  NOPQRSTUVWXYZ012
-0000a2f0: 3334 3536 3738 3961 6263 6465 6667 6869  3456789abcdefghi
-0000a300: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-0000a310: 7a22 290a 2020 2020 2020 2020 7431 203d  z").        t1 =
-0000a320: 206c 742e 5461 626c 6528 292e 696e 7365   lt.Table().inse
-0000a330: 7274 5f6d 616e 7928 6c74 2e44 6174 614f  rt_many(lt.DataO
-0000a340: 626a 6563 7428 413d 6329 2066 6f72 2063  bject(A=c) for c
-0000a350: 2069 6e20 636f 6d70 6172 655f 6c69 7374   in compare_list
-0000a360: 290a 0a20 2020 2020 2020 2064 6566 206d  )..        def m
-0000a370: 696e 695f 7465 7374 2873 6c63 5f74 7570  ini_test(slc_tup
-0000a380: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-0000a390: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-0000a3a0: 6c63 5f74 7570 6c65 2c20 7475 706c 6529  lc_tuple, tuple)
-0000a3b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a3c0: 2020 6c61 6265 6c20 3d20 225b 7b7d 3a7b    label = "[{}:{
-0000a3d0: 7d3a 7b7d 5d22 2e66 6f72 6d61 7428 2a28  }:{}]".format(*(
-0000a3e0: 6920 6966 2069 2069 7320 6e6f 7420 4e6f  i if i is not No
-0000a3f0: 6e65 2065 6c73 6520 2727 2066 6f72 2069  ne else '' for i
-0000a400: 2069 6e20 736c 635f 7475 706c 6529 290a   in slc_tuple)).
-0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a420: 736c 6320 3d20 736c 6963 6528 2a73 6c63  slc = slice(*slc
-0000a430: 5f74 7570 6c65 290a 2020 2020 2020 2020  _tuple).        
-0000a440: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a450: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-0000a460: 3d20 7374 7228 736c 635f 7475 706c 6529  = str(slc_tuple)
-0000a470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a480: 2073 6c63 203d 2073 6c63 5f74 7570 6c65   slc = slc_tuple
-0000a490: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-0000a4a0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000a4b0: 6c61 6265 6c2c 2073 6c63 5f74 7570 6c65  label, slc_tuple
-0000a4c0: 3d73 6c63 5f74 7570 6c65 293a 0a20 2020  =slc_tuple):.   
-0000a4d0: 2020 2020 2020 2020 2020 2020 2064 656c               del
-0000a4e0: 2063 6f6d 7061 7265 5f6c 6973 745b 736c   compare_list[sl
-0000a4f0: 635d 0a20 2020 2020 2020 2020 2020 2020  c].             
-0000a500: 2020 2070 7269 6e74 286c 6162 656c 290a     print(label).
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 7072 696e 7428 2745 7870 6563 7465 6427  print('Expected'
-0000a530: 2c20 636f 6d70 6172 655f 6c69 7374 290a  , compare_list).
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 6465 6c20 7431 5b73 6c63 5d0a 2020 2020  del t1[slc].    
-0000a560: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000a570: 7428 274f 6273 6572 7665 6427 2c20 6c69  t('Observed', li
-0000a580: 7374 2874 312e 616c 6c2e 4129 290a 2020  st(t1.all.A)).  
-0000a590: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000a5a0: 696e 7428 290a 2020 2020 2020 2020 2020  int().          
-0000a5b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a5c0: 7445 7175 616c 2827 272e 6a6f 696e 2863  tEqual(''.join(c
-0000a5d0: 6f6d 7061 7265 5f6c 6973 7429 2c20 2727  ompare_list), ''
-0000a5e0: 2e6a 6f69 6e28 7431 2e61 6c6c 2e41 292c  .join(t1.all.A),
-0000a5f0: 2022 6661 696c 6564 2022 202b 206c 6162   "failed " + lab
-0000a600: 656c 290a 0a20 2020 2020 2020 206d 696e  el)..        min
-0000a610: 695f 7465 7374 2835 290a 2020 2020 2020  i_test(5).      
-0000a620: 2020 6d69 6e69 5f74 6573 7428 2d35 290a    mini_test(-5).
-0000a630: 2020 2020 2020 2020 6d69 6e69 5f74 6573          mini_tes
-0000a640: 7428 282d 352c 204e 6f6e 652c 204e 6f6e  t((-5, None, Non
-0000a650: 6529 290a 2020 2020 2020 2020 6d69 6e69  e)).        mini
-0000a660: 5f74 6573 7428 284e 6f6e 652c 2033 2c20  _test((None, 3, 
-0000a670: 4e6f 6e65 2929 0a20 2020 2020 2020 206d  None)).        m
-0000a680: 696e 695f 7465 7374 2828 4e6f 6e65 2c20  ini_test((None, 
-0000a690: 2d6c 656e 2863 6f6d 7061 7265 5f6c 6973  -len(compare_lis
-0000a6a0: 7429 2b33 2c20 4e6f 6e65 2929 0a20 2020  t)+3, None)).   
-0000a6b0: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
-0000a6c0: 4e6f 6e65 2c20 4e6f 6e65 2c20 3529 290a  None, None, 5)).
-0000a6d0: 2020 2020 2020 2020 6d69 6e69 5f74 6573          mini_tes
-0000a6e0: 7428 284e 6f6e 652c 204e 6f6e 652c 202d  t((None, None, -
-0000a6f0: 3529 290a 2020 2020 2020 2020 6d69 6e69  5)).        mini
-0000a700: 5f74 6573 7428 282d 352c 202d 322c 204e  _test((-5, -2, N
-0000a710: 6f6e 6529 290a 2020 2020 2020 2020 6d69  one)).        mi
-0000a720: 6e69 5f74 6573 7428 282d 322c 202d 352c  ni_test((-2, -5,
-0000a730: 202d 3129 290a 2020 2020 2020 2020 6d69   -1)).        mi
-0000a740: 6e69 5f74 6573 7428 2835 2c20 3230 2c20  ni_test((5, 20, 
-0000a750: 3229 290a 2020 2020 2020 2020 6d69 6e69  2)).        mini
-0000a760: 5f74 6573 7428 286c 656e 2863 6f6d 7061  _test((len(compa
-0000a770: 7265 5f6c 6973 7429 2c20 352c 202d 3329  re_list), 5, -3)
-0000a780: 290a 2020 2020 2020 2020 6d69 6e69 5f74  ).        mini_t
-0000a790: 6573 7428 2832 302c 2031 312c 202d 3729  est((20, 11, -7)
-0000a7a0: 290a 2020 2020 2020 2020 6d69 6e69 5f74  ).        mini_t
-0000a7b0: 6573 7428 2835 2c20 352c 204e 6f6e 6529  est((5, 5, None)
-0000a7c0: 290a 2020 2020 2020 2020 6d69 6e69 5f74  ).        mini_t
-0000a7d0: 6573 7428 284e 6f6e 652c 202d 3130 2c20  est((None, -10, 
-0000a7e0: 3529 290a 2020 2020 2020 2020 6d69 6e69  5)).        mini
-0000a7f0: 5f74 6573 7428 284e 6f6e 652c 202d 3130  _test((None, -10
-0000a800: 2c20 2d31 3029 290a 2020 2020 2020 2020  , -10)).        
-0000a810: 6d69 6e69 5f74 6573 7428 2831 3030 302c  mini_test((1000,
-0000a820: 2032 3030 302c 204e 6f6e 6529 290a 2020   2000, None)).  
-0000a830: 2020 2020 2020 6d69 6e69 5f74 6573 7428        mini_test(
-0000a840: 284e 6f6e 652c 204e 6f6e 652c 202d 3129  (None, None, -1)
-0000a850: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000a860: 636c 6561 7228 7365 6c66 293a 0a20 2020  clear(self):.   
-0000a870: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-0000a880: 696e 6974 2829 0a20 2020 2020 2020 206e  init().        n
-0000a890: 756d 5f66 6965 6c64 7320 3d20 6c65 6e28  um_fields = len(
-0000a8a0: 7365 6c66 2e74 312e 696e 666f 2829 5b22  self.t1.info()["
-0000a8b0: 6669 656c 6473 225d 290a 2020 2020 2020  fields"]).      
-0000a8c0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000a8d0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000a8e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000a8f0: 7561 6c28 7365 6c66 2e74 6573 745f 7369  ual(self.test_si
-0000a900: 7a65 202a 2a20 6e75 6d5f 6669 656c 6473  ze ** num_fields
-0000a910: 2c20 6c65 6e28 7365 6c66 2e74 3129 2c20  , len(self.t1), 
-0000a920: 2269 6e76 616c 6964 206c 656e 2229 0a20  "invalid len"). 
-0000a930: 2020 2020 2020 2073 656c 662e 7431 2e63         self.t1.c
-0000a940: 7265 6174 655f 696e 6465 7828 2261 2229  reate_index("a")
-0000a950: 0a0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-0000a960: 312e 636c 6561 7228 290a 2020 2020 2020  1.clear().      
-0000a970: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000a980: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000a990: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000a9a0: 7561 6c28 302c 206c 656e 2873 656c 662e  ual(0, len(self.
-0000a9b0: 7431 292c 2022 696e 7661 6c69 6420 6c65  t1), "invalid le
-0000a9c0: 6e20 6166 7465 7220 636c 6561 7222 290a  n after clear").
-0000a9d0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000a9e0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000a9f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000aa00: 7365 7274 4571 7561 6c28 312c 206c 656e  sertEqual(1, len
-0000aa10: 2873 656c 662e 7431 2e69 6e66 6f28 295b  (self.t1.info()[
-0000aa20: 2269 6e64 6578 6573 225d 292c 2022 696e  "indexes"]), "in
-0000aa30: 7661 6c69 6420 696e 6465 7865 7320 6166  valid indexes af
-0000aa40: 7465 7220 636c 6561 7222 290a 0a20 2020  ter clear")..   
-0000aa50: 2064 6566 2074 6573 745f 7374 6174 7328   def test_stats(
-0000aa60: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000aa70: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
-0000aa80: 0a20 2020 2020 2020 2066 6965 6c64 5f6e  .        field_n
-0000aa90: 616d 6573 203d 2073 656c 662e 7431 2e69  ames = self.t1.i
-0000aaa0: 6e66 6f28 295b 2266 6965 6c64 7322 5d0a  nfo()["fields"].
-0000aab0: 2020 2020 2020 2020 6e75 6d5f 6669 656c          num_fiel
-0000aac0: 6473 203d 206c 656e 2866 6965 6c64 5f6e  ds = len(field_n
-0000aad0: 616d 6573 290a 2020 2020 2020 2020 7431  ames).        t1
-0000aae0: 5f73 7461 7473 203d 2073 656c 662e 7431  _stats = self.t1
-0000aaf0: 2e73 7461 7473 2829 2e73 656c 6563 7428  .stats().select(
-0000ab00: 226e 616d 6520 636f 756e 7420 6d69 6e20  "name count min 
-0000ab10: 6d61 7820 6d65 616e 2229 0a20 2020 2020  max mean").     
-0000ab20: 2020 2066 6f72 2066 6965 6c64 6e61 6d65     for fieldname
-0000ab30: 2069 6e20 6669 656c 645f 6e61 6d65 733a   in field_names:
-0000ab40: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000ab50: 745f 7265 6320 3d20 7431 5f73 7461 7473  t_rec = t1_stats
-0000ab60: 2e62 792e 6e61 6d65 5b66 6965 6c64 6e61  .by.name[fieldna
-0000ab70: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-0000ab80: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000ab90: 7428 2263 6865 636b 2063 6f6d 7075 7465  t("check compute
-0000aba0: 6420 7374 6174 222c 2066 6965 6c64 6e61  d stat", fieldna
-0000abb0: 6d65 3d66 6965 6c64 6e61 6d65 293a 0a20  me=fieldname):. 
-0000abc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000abd0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000abe0: 6c74 2e44 6174 614f 626a 6563 7428 6e61  lt.DataObject(na
-0000abf0: 6d65 3d66 6965 6c64 6e61 6d65 2c0a 2020  me=fieldname,.  
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac20: 2020 2020 2020 2020 2020 2020 2063 6f75               cou
-0000ac30: 6e74 3d73 656c 662e 7465 7374 5f73 697a  nt=self.test_siz
-0000ac40: 6520 2a2a 206e 756d 5f66 6965 6c64 732c  e ** num_fields,
-0000ac50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 6d69 6e3d 302c 0a20 2020 2020 2020 2020  min=0,.         
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 6d61 783d 7365 6c66 2e74        max=self.t
-0000acc0: 6573 745f 7369 7a65 202d 2031 2c0a 2020  est_size - 1,.  
-0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acf0: 2020 2020 2020 2020 2020 2020 206d 6561               mea
-0000ad00: 6e3d 2873 656c 662e 7465 7374 5f73 697a  n=(self.test_siz
-0000ad10: 6520 2d20 3129 202f 2032 292c 0a20 2020  e - 1) / 2),.   
-0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000ad40: 6174 5f72 6563 2c0a 2020 2020 2020 2020  at_rec,.        
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 2020 2020 2066 2269 6e76 616c           f"inval
-0000ad70: 6964 2073 7461 7420 666f 7220 7b66 6965  id stat for {fie
-0000ad80: 6c64 6e61 6d65 7d22 290a 0a20 2020 2064  ldname}")..    d
-0000ad90: 6566 2074 6573 745f 7374 6174 7332 2873  ef test_stats2(s
-0000ada0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0000adb0: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
-0000adc0: 2020 2020 2020 2020 6669 656c 645f 6e61          field_na
-0000add0: 6d65 7320 3d20 7365 6c66 2e74 312e 696e  mes = self.t1.in
-0000ade0: 666f 2829 5b22 6669 656c 6473 225d 0a20  fo()["fields"]. 
-0000adf0: 2020 2020 2020 206e 756d 5f66 6965 6c64         num_field
-0000ae00: 7320 3d20 6c65 6e28 6669 656c 645f 6e61  s = len(field_na
-0000ae10: 6d65 7329 0a20 2020 2020 2020 2074 315f  mes).        t1_
-0000ae20: 7374 6174 7320 3d20 7365 6c66 2e74 312e  stats = self.t1.
-0000ae30: 7374 6174 7328 6279 5f66 6965 6c64 3d46  stats(by_field=F
-0000ae40: 616c 7365 290a 2020 2020 2020 2020 666f  alse).        fo
-0000ae50: 7220 7374 6174 2c20 7661 6c75 6520 696e  r stat, value in
-0000ae60: 2028 2827 6d69 6e27 2c20 3029 2c20 2827   (('min', 0), ('
-0000ae70: 6d61 7827 2c20 7365 6c66 2e74 6573 745f  max', self.test_
-0000ae80: 7369 7a65 202d 2031 292c 2028 2763 6f75  size - 1), ('cou
-0000ae90: 6e74 272c 2073 656c 662e 7465 7374 5f73  nt', self.test_s
-0000aea0: 697a 6520 2a2a 206e 756d 5f66 6965 6c64  ize ** num_field
-0000aeb0: 7329 2c29 3a0a 2020 2020 2020 2020 2020  s),):.          
-0000aec0: 2020 666f 7220 6669 656c 646e 616d 6520    for fieldname 
-0000aed0: 696e 2066 6965 6c64 5f6e 616d 6573 3a0a  in field_names:.
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000af00: 7428 2263 6865 636b 2063 6f6d 7075 7465  t("check compute
-0000af10: 6420 7374 6174 222c 2073 7461 743d 7374  d stat", stat=st
-0000af20: 6174 2c20 6669 656c 646e 616d 653d 6669  at, fieldname=fi
-0000af30: 656c 646e 616d 6529 3a0a 2020 2020 2020  eldname):.      
-0000af40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000af50: 6c66 2e61 7373 6572 7445 7175 616c 2876  lf.assertEqual(v
-0000af60: 616c 7565 2c20 6765 7461 7474 7228 7431  alue, getattr(t1
-0000af70: 5f73 7461 7473 2e62 792e 7374 6174 5b73  _stats.by.stat[s
-0000af80: 7461 745d 2c20 6669 656c 646e 616d 6529  tat], fieldname)
-0000af90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2066 2269 6e76 616c 6964 207b 7374     f"invalid {st
-0000afc0: 6174 7d20 7374 6174 2066 6f72 207b 6669  at} stat for {fi
-0000afd0: 656c 646e 616d 657d 2229 0a0a 2020 2020  eldname}")..    
-0000afe0: 6465 6620 7465 7374 5f73 7461 7473 3328  def test_stats3(
-0000aff0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000b000: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
-0000b010: 0a20 2020 2020 2020 2066 6965 6c64 5f6e  .        field_n
-0000b020: 616d 6573 203d 2073 656c 662e 7431 2e69  ames = self.t1.i
-0000b030: 6e66 6f28 295b 2266 6965 6c64 7322 5d0a  nfo()["fields"].
-0000b040: 2020 2020 2020 2020 6e75 6d5f 6669 656c          num_fiel
-0000b050: 6473 203d 206c 656e 2866 6965 6c64 5f6e  ds = len(field_n
-0000b060: 616d 6573 290a 0a20 2020 2020 2020 2023  ames)..        #
-0000b070: 2076 6572 6966 7920 7468 6174 2073 7461   verify that sta
-0000b080: 7473 2063 616e 2022 7374 6570 206f 7665  ts can "step ove
-0000b090: 7222 206e 6f6e 2d6e 756d 6572 6963 2064  r" non-numeric d
-0000b0a0: 6174 610a 2020 2020 2020 2020 7472 793a  ata.        try:
-0000b0b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b0c0: 662e 7431 5b30 5d2e 6120 3d20 226e 6f74  f.t1[0].a = "not
-0000b0d0: 2061 206e 756d 6265 7222 0a20 2020 2020   a number".     
-0000b0e0: 2020 2065 7863 6570 7420 2841 7474 7269     except (Attri
-0000b0f0: 6275 7465 4572 726f 722c 2054 7970 6545  buteError, TypeE
-0000b100: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-0000b110: 2020 2023 2073 6f6d 6520 7465 7374 2074     # some test t
-0000b120: 7970 6573 2061 7265 6e27 7420 6d75 7461  ypes aren't muta
-0000b130: 626c 652c 206d 7573 7420 7265 706c 6163  ble, must replac
-0000b140: 6520 7265 6320 7769 7468 2061 206d 6f64  e rec with a mod
-0000b150: 6966 6965 6420 6f6e 650a 2020 2020 2020  ified one.      
-0000b160: 2020 2020 2020 6d6f 645f 7265 6320 3d20        mod_rec = 
-0000b170: 7365 6c66 2e74 312e 706f 7028 3029 0a20  self.t1.pop(0). 
-0000b180: 2020 2020 2020 2020 2020 2072 6563 5f74             rec_t
-0000b190: 7970 6520 3d20 7479 7065 286d 6f64 5f72  ype = type(mod_r
-0000b1a0: 6563 290a 2020 2020 2020 2020 2020 2020  ec).            
-0000b1b0: 6e65 775f 7265 635f 6469 6374 203d 206c  new_rec_dict = l
-0000b1c0: 742e 5f74 6f5f 6469 6374 286d 6f64 5f72  t._to_dict(mod_r
-0000b1d0: 6563 290a 2020 2020 2020 2020 2020 2020  ec).            
-0000b1e0: 6e65 775f 7265 635f 6469 6374 5b27 6127  new_rec_dict['a'
-0000b1f0: 5d20 3d20 226e 6f74 2061 206e 756d 6265  ] = "not a numbe
-0000b200: 7222 0a20 2020 2020 2020 2020 2020 206e  r".            n
-0000b210: 6577 5f72 6563 203d 2072 6563 5f74 7970  ew_rec = rec_typ
-0000b220: 6528 2a2a 6e65 775f 7265 635f 6469 6374  e(**new_rec_dict
-0000b230: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000b240: 6c66 2e74 312e 696e 7365 7274 286e 6577  lf.t1.insert(new
-0000b250: 5f72 6563 290a 0a20 2020 2020 2020 2074  _rec)..        t
-0000b260: 315f 7374 6174 7320 3d20 7365 6c66 2e74  1_stats = self.t
-0000b270: 312e 7374 6174 7328 290a 2020 2020 2020  1.stats().      
-0000b280: 2020 7431 5f73 7461 7473 2822 7431 5f73    t1_stats("t1_s
-0000b290: 7461 7473 2229 0a20 2020 2020 2020 2074  tats").        t
-0000b2a0: 315f 7374 6174 732e 6373 765f 6578 706f  1_stats.csv_expo
-0000b2b0: 7274 2873 7973 2e73 7464 6f75 7429 0a20  rt(sys.stdout). 
-0000b2c0: 2020 2020 2020 2074 315f 7374 6174 732e         t1_stats.
-0000b2d0: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000b2e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000b2f0: 616c 2873 656c 662e 7465 7374 5f73 697a  al(self.test_siz
-0000b300: 6520 2a2a 206e 756d 5f66 6965 6c64 7320  e ** num_fields 
-0000b310: 2d20 312c 2074 315f 7374 6174 732e 6279  - 1, t1_stats.by
-0000b320: 2e6e 616d 655b 2261 225d 2e63 6f75 6e74  .name["a"].count
-0000b330: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000b340: 7374 6174 7334 2873 656c 6629 3a0a 2020  stats4(self):.  
-0000b350: 2020 2020 2020 7431 203d 206c 742e 5461        t1 = lt.Ta
-0000b360: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000b370: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000b380: 2822 2222 5c0a 2020 2020 2020 2020 612c  ("""\.        a,
-0000b390: 620a 2020 2020 2020 2020 312c 320a 2020  b.        1,2.  
-0000b3a0: 2020 2020 2020 332c 0a20 2020 2020 2020        3,.       
-0000b3b0: 2035 2c34 0a20 2020 2020 2020 2022 2222   5,4.        """
-0000b3c0: 292c 2074 7261 6e73 666f 726d 733d 7b7d  ), transforms={}
-0000b3d0: 2e66 726f 6d6b 6579 7328 5b22 6122 2c20  .fromkeys(["a", 
-0000b3e0: 2262 225d 2c20 696e 7429 290a 2020 2020  "b"], int)).    
-0000b3f0: 2020 2020 7431 5f73 7461 7473 203d 2074      t1_stats = t
-0000b400: 312e 7374 6174 7328 290a 2020 2020 2020  1.stats().      
-0000b410: 2020 7431 5f73 7461 7473 2e70 7265 7365    t1_stats.prese
-0000b420: 6e74 2829 0a20 2020 2020 2020 2070 7269  nt().        pri
-0000b430: 6e74 2874 315f 7374 6174 732e 696e 666f  nt(t1_stats.info
-0000b440: 2829 290a 0a20 2020 2020 2020 2065 7870  ())..        exp
-0000b450: 6563 7465 6420 3d20 6c74 2e54 6162 6c65  ected = lt.Table
-0000b460: 2829 2e63 7376 5f69 6d70 6f72 7428 7465  ().csv_import(te
-0000b470: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
-0000b480: 225c 0a20 2020 2020 2020 206e 616d 652c  "\.        name,
-0000b490: 6d65 616e 2c6d 696e 2c6d 6178 2c76 6172  mean,min,max,var
-0000b4a0: 6961 6e63 652c 7374 645f 6465 762c 636f  iance,std_dev,co
-0000b4b0: 756e 742c 6d69 7373 696e 670a 2020 2020  unt,missing.    
-0000b4c0: 2020 2020 612c 332e 302c 312c 352c 342c      a,3.0,1,5,4,
-0000b4d0: 322e 302c 332c 300a 2020 2020 2020 2020  2.0,3,0.        
-0000b4e0: 622c 332e 302c 322c 342c 322c 312e 3431  b,3.0,2,4,2,1.41
-0000b4f0: 342c 322c 310a 2020 2020 2020 2020 2222  4,2,1.        ""
-0000b500: 2229 2c20 7472 616e 7366 6f72 6d73 3d7b  "), transforms={
-0000b510: 7d2e 6672 6f6d 6b65 7973 2822 6d65 616e  }.fromkeys("mean
-0000b520: 206d 696e 206d 6178 2076 6172 6961 6e63   min max varianc
-0000b530: 6520 7374 645f 6465 7620 636f 756e 7420  e std_dev count 
-0000b540: 6d69 7373 696e 6722 2e73 706c 6974 2829  missing".split()
-0000b550: 2c20 6173 742e 6c69 7465 7261 6c5f 6576  , ast.literal_ev
-0000b560: 616c 2929 0a20 2020 2020 2020 2065 7870  al)).        exp
-0000b570: 6563 7465 642e 7072 6573 656e 7428 290a  ected.present().
-0000b580: 2020 2020 2020 2020 7072 696e 7428 6578          print(ex
-0000b590: 7065 6374 6564 2e69 6e66 6f28 2929 0a0a  pected.info())..
-0000b5a0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000b5b0: 662e 7375 6254 6573 7428 2263 6865 636b  f.subTest("check
-0000b5c0: 2063 6f6d 7075 7465 6420 7374 6174 2066   computed stat f
-0000b5d0: 6965 6c64 7322 293a 0a20 2020 2020 2020  ields"):.       
-0000b5e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b5f0: 4571 7561 6c28 6578 7065 6374 6564 2e69  Equal(expected.i
-0000b600: 6e66 6f28 295b 2266 6965 6c64 7322 5d2c  nfo()["fields"],
-0000b610: 2074 315f 7374 6174 732e 696e 666f 2829   t1_stats.info()
-0000b620: 5b22 6669 656c 6473 225d 290a 0a20 2020  ["fields"])..   
-0000b630: 2020 2020 2066 6f72 2065 7870 6563 7465       for expecte
-0000b640: 645f 726f 772c 2072 6f77 2069 6e20 7a69  d_row, row in zi
-0000b650: 7028 6578 7065 6374 6564 2c20 7431 5f73  p(expected, t1_s
-0000b660: 7461 7473 293a 0a20 2020 2020 2020 2020  tats):.         
-0000b670: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000b680: 5465 7374 2822 6368 6563 6b20 636f 6d70  Test("check comp
-0000b690: 7574 6564 2073 7461 7420 6174 7472 6962  uted stat attrib
-0000b6a0: 7574 6520 286e 616d 6529 222c 2072 6f77  ute (name)", row
-0000b6b0: 3d72 6f77 293a 0a20 2020 2020 2020 2020  =row):.         
-0000b6c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000b6d0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-0000b6e0: 5f72 6f77 2e6e 616d 652c 2072 6f77 2e6e  _row.name, row.n
-0000b6f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0000b700: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000b710: 7374 2822 6368 6563 6b20 636f 6d70 7574  st("check comput
-0000b720: 6564 2073 7461 7420 6174 7472 6962 7574  ed stat attribut
-0000b730: 6520 286d 6561 6e29 222c 2072 6f77 3d72  e (mean)", row=r
-0000b740: 6f77 293a 0a20 2020 2020 2020 2020 2020  ow):.           
-0000b750: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b760: 4571 7561 6c28 6578 7065 6374 6564 5f72  Equal(expected_r
-0000b770: 6f77 2e6d 6561 6e2c 2072 6f77 2e6d 6561  ow.mean, row.mea
-0000b780: 6e29 0a20 2020 2020 2020 2020 2020 2077  n).            w
-0000b790: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000b7a0: 2822 6368 6563 6b20 636f 6d70 7574 6564  ("check computed
-0000b7b0: 2073 7461 7420 6174 7472 6962 7574 6520   stat attribute 
-0000b7c0: 286d 696e 2922 2c20 726f 773d 726f 7729  (min)", row=row)
-0000b7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b7e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000b7f0: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
-0000b800: 6d69 6e2c 2072 6f77 2e6d 696e 290a 2020  min, row.min).  
-0000b810: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-0000b820: 656c 662e 7375 6254 6573 7428 2263 6865  elf.subTest("che
-0000b830: 636b 2063 6f6d 7075 7465 6420 7374 6174  ck computed stat
-0000b840: 2061 7474 7269 6275 7465 2028 6d61 7829   attribute (max)
-0000b850: 222c 2072 6f77 3d72 6f77 293a 0a20 2020  ", row=row):.   
-0000b860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b870: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000b880: 7065 6374 6564 5f72 6f77 2e6d 6178 2c20  pected_row.max, 
-0000b890: 726f 772e 6d61 7829 0a20 2020 2020 2020  row.max).       
-0000b8a0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000b8b0: 7562 5465 7374 2822 6368 6563 6b20 636f  ubTest("check co
-0000b8c0: 6d70 7574 6564 2073 7461 7420 6174 7472  mputed stat attr
-0000b8d0: 6962 7574 6520 2876 6172 6961 6e63 6529  ibute (variance)
-0000b8e0: 222c 2072 6f77 3d72 6f77 293a 0a20 2020  ", row=row):.   
-0000b8f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b900: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000b910: 7065 6374 6564 5f72 6f77 2e76 6172 6961  pected_row.varia
-0000b920: 6e63 652c 2072 6f77 2e76 6172 6961 6e63  nce, row.varianc
-0000b930: 6529 0a20 2020 2020 2020 2020 2020 2077  e).            w
-0000b940: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000b950: 2822 6368 6563 6b20 636f 6d70 7574 6564  ("check computed
-0000b960: 2073 7461 7420 6174 7472 6962 7574 6520   stat attribute 
-0000b970: 2873 7464 5f64 6576 2922 2c20 726f 773d  (std_dev)", row=
-0000b980: 726f 7729 3a0a 2020 2020 2020 2020 2020  row):.          
-0000b990: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000b9a0: 7445 7175 616c 2865 7870 6563 7465 645f  tEqual(expected_
-0000b9b0: 726f 772e 7374 645f 6465 762c 2072 6f77  row.std_dev, row
-0000b9c0: 2e73 7464 5f64 6576 290a 2020 2020 2020  .std_dev).      
-0000b9d0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000b9e0: 7375 6254 6573 7428 2263 6865 636b 2063  subTest("check c
-0000b9f0: 6f6d 7075 7465 6420 7374 6174 2061 7474  omputed stat att
-0000ba00: 7269 6275 7465 2028 636f 756e 7429 222c  ribute (count)",
-0000ba10: 2072 6f77 3d72 6f77 293a 0a20 2020 2020   row=row):.     
-0000ba20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ba30: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-0000ba40: 6374 6564 5f72 6f77 2e63 6f75 6e74 2c20  cted_row.count, 
-0000ba50: 726f 772e 636f 756e 7429 0a20 2020 2020  row.count).     
-0000ba60: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000ba70: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
-0000ba80: 636f 6d70 7574 6564 2073 7461 7420 6174  computed stat at
-0000ba90: 7472 6962 7574 6520 286d 6973 7369 6e67  tribute (missing
-0000baa0: 2922 2c20 726f 773d 726f 7729 3a0a 2020  )", row=row):.  
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000bac0: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0000bad0: 7870 6563 7465 645f 726f 772e 6d69 7373  xpected_row.miss
-0000bae0: 696e 672c 2072 6f77 2e6d 6973 7369 6e67  ing, row.missing
-0000baf0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000bb00: 7370 6c69 7462 7928 7365 6c66 293a 0a20  splitby(self):. 
-0000bb10: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-0000bb20: 745f 696e 6974 2829 0a20 2020 2020 2020  t_init().       
-0000bb30: 2069 735f 6f64 6420 3d20 6c61 6d62 6461   is_odd = lambda
-0000bb40: 2072 6563 3a20 7265 632e 6120 2520 320a   rec: rec.a % 2.
-0000bb50: 2020 2020 2020 2020 6576 656e 732c 206f          evens, o
-0000bb60: 6464 7320 3d20 7365 6c66 2e74 312e 7370  dds = self.t1.sp
-0000bb70: 6c69 7462 7928 6973 5f6f 6464 290a 2020  litby(is_odd).  
-0000bb80: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000bb90: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000bba0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000bbb0: 7274 4571 7561 6c28 6c65 6e28 6f64 6473  rtEqual(len(odds
-0000bbc0: 2920 2b20 6c65 6e28 6576 656e 7329 2c20  ) + len(evens), 
-0000bbd0: 6c65 6e28 7365 6c66 2e74 3129 290a 2020  len(self.t1)).  
-0000bbe0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000bbf0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000bc00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000bc10: 7274 4571 7561 6c28 6c65 6e28 6f64 6473  rtEqual(len(odds
-0000bc20: 292c 206c 656e 2873 656c 662e 7431 2e77  ), len(self.t1.w
-0000bc30: 6865 7265 2869 735f 6f64 6429 2929 0a0a  here(is_odd)))..
-0000bc40: 2020 2020 2020 2020 6576 656e 5f65 7665          even_eve
-0000bc50: 6e73 2c20 6f64 645f 6576 656e 7320 3d20  ns, odd_evens = 
-0000bc60: 6576 656e 732e 7370 6c69 7462 7928 6973  evens.splitby(is
-0000bc70: 5f6f 6464 290a 2020 2020 2020 2020 7769  _odd).        wi
-0000bc80: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000bc90: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000bca0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000bcb0: 302c 206c 656e 286f 6464 5f65 7665 6e73  0, len(odd_evens
-0000bcc0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-0000bcd0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-0000bce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bcf0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-0000bd00: 2865 7665 6e5f 6576 656e 7329 2c20 6c65  (even_evens), le
-0000bd10: 6e28 6576 656e 7329 290a 0a20 2020 2020  n(evens))..     
-0000bd20: 2020 2023 206d 616b 6520 7375 7265 2069     # make sure i
-0000bd30: 6e64 6578 6573 2061 7265 2070 7265 7365  ndexes are prese
-0000bd40: 7276 6564 0a20 2020 2020 2020 2073 656c  rved.        sel
-0000bd50: 662e 7431 2e63 7265 6174 655f 696e 6465  f.t1.create_inde
-0000bd60: 7828 2261 2229 0a20 2020 2020 2020 2065  x("a").        e
-0000bd70: 7665 6e73 2c20 6f64 6473 203d 2073 656c  vens, odds = sel
-0000bd80: 662e 7431 2e73 706c 6974 6279 2869 735f  f.t1.splitby(is_
-0000bd90: 6f64 6429 0a20 2020 2020 2020 2077 6974  odd).        wit
-0000bda0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000bdb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000bdc0: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0000bdd0: 656c 662e 7431 2e69 6e66 6f28 295b 2269  elf.t1.info()["i
-0000bde0: 6e64 6578 6573 225d 2c20 6576 656e 732e  ndexes"], evens.
-0000bdf0: 696e 666f 2829 5b22 696e 6465 7865 7322  info()["indexes"
-0000be00: 5d29 0a0a 2020 2020 2020 2020 2320 7465  ])..        # te
-0000be10: 7374 2070 6173 7369 6e67 2061 6e20 6174  st passing an at
-0000be20: 7472 6962 7574 6520 6173 2061 206b 6579  tribute as a key
-0000be30: 0a20 2020 2020 2020 207a 6572 6f73 2c20  .        zeros, 
-0000be40: 6e6f 6e5f 7a65 726f 7320 3d20 7365 6c66  non_zeros = self
-0000be50: 2e74 312e 7370 6c69 7462 7928 2261 2229  .t1.splitby("a")
-0000be60: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000be70: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000be80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000be90: 7373 6572 7454 7275 6528 616c 6c28 7265  ssertTrue(all(re
-0000bea0: 632e 6120 3d3d 2030 2066 6f72 2072 6563  c.a == 0 for rec
-0000beb0: 2069 6e20 7a65 726f 7329 290a 2020 2020   in zeros)).    
-0000bec0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000bed0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000bee0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000bef0: 5472 7565 2861 6c6c 2872 6563 2e61 2021  True(all(rec.a !
-0000bf00: 3d20 3020 666f 7220 7265 6320 696e 206e  = 0 for rec in n
-0000bf10: 6f6e 5f7a 6572 6f73 2929 0a0a 2020 2020  on_zeros))..    
-0000bf20: 2020 2020 2320 7465 7374 2075 7369 6e67      # test using
-0000bf30: 2070 7265 6469 6361 7465 2074 6861 7420   predicate that 
-0000bf40: 646f 6573 206e 6f74 2061 6c77 6179 7320  does not always 
-0000bf50: 7265 7475 726e 2030 206f 7220 310a 2020  return 0 or 1.  
-0000bf60: 2020 2020 2020 6973 5f6e 6f74 5f6d 756c        is_not_mul
-0000bf70: 7469 706c 655f 6f66 5f33 203d 206c 616d  tiple_of_3 = lam
-0000bf80: 6264 6120 7265 633a 2072 6563 2e61 2025  bda rec: rec.a %
-0000bf90: 2033 0a20 2020 2020 2020 206d 756c 7473   3.        mults
-0000bfa0: 5f6f 665f 332c 206e 6f6e 5f6d 756c 7473  _of_3, non_mults
-0000bfb0: 5f6f 665f 3320 3d20 7365 6c66 2e74 312e  _of_3 = self.t1.
-0000bfc0: 7370 6c69 7462 7928 6973 5f6e 6f74 5f6d  splitby(is_not_m
-0000bfd0: 756c 7469 706c 655f 6f66 5f33 290a 2020  ultiple_of_3).  
-0000bfe0: 2020 2020 2020 7072 696e 7428 6c69 7374        print(list
-0000bff0: 286e 6f6e 5f6d 756c 7473 5f6f 665f 332e  (non_mults_of_3.
-0000c000: 616c 6c2e 6129 290a 2020 2020 2020 2020  all.a)).        
-0000c010: 7072 696e 7428 6c69 7374 286d 756c 7473  print(list(mults
-0000c020: 5f6f 665f 332e 616c 6c2e 6129 290a 2020  _of_3.all.a)).  
-0000c030: 2020 2020 2020 2320 544f 444f 202d 2061        # TODO - a
-0000c040: 6464 2061 7373 6572 7473 2068 6572 650a  dd asserts here.
-0000c050: 0a0a 406d 616b 655f 7465 7374 5f63 6c61  ..@make_test_cla
-0000c060: 7373 6573 0a63 6c61 7373 2054 6162 6c65  sses.class Table
-0000c070: 4a6f 696e 5465 7374 733a 0a20 2020 2022  JoinTests:.    "
-0000c080: 2222 0a20 2020 2054 6573 7473 2066 6f72  "".    Tests for
-0000c090: 2054 6162 6c65 206a 6f69 6e20 6f70 6572   Table join oper
-0000c0a0: 6174 696f 6e73 2e0a 2020 2020 2222 220a  ations..    """.
-0000c0b0: 2020 2020 6465 6620 7465 7374 5f73 696d      def test_sim
-0000c0c0: 706c 655f 6a6f 696e 2873 656c 6629 3a0a  ple_join(self):.
-0000c0d0: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-0000c0e0: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-0000c0f0: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
-0000c100: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
-0000c110: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
-0000c120: 7369 7a65 290a 2020 2020 2020 2020 7431  size).        t1
-0000c130: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
-0000c140: 2729 0a0a 2020 2020 2020 2020 7432 203d  ')..        t2 =
-0000c150: 206c 742e 5461 626c 6528 290a 2020 2020   lt.Table().    
-0000c160: 2020 2020 7432 2e63 7265 6174 655f 696e      t2.create_in
-0000c170: 6465 7828 2761 2729 0a20 2020 2020 2020  dex('a').       
-0000c180: 2074 322e 696e 7365 7274 286c 742e 4461   t2.insert(lt.Da
-0000c190: 7461 4f62 6a65 6374 2861 3d31 2c20 643d  taObject(a=1, d=
-0000c1a0: 3130 3029 290a 0a20 2020 2020 2020 206a  100))..        j
-0000c1b0: 6f69 6e65 6420 3d20 2874 312e 6a6f 696e  oined = (t1.join
-0000c1c0: 5f6f 6e28 2761 2729 202b 2074 322e 6a6f  _on('a') + t2.jo
-0000c1d0: 696e 5f6f 6e28 2761 2729 2928 290a 2020  in_on('a'))().  
-0000c1e0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000c1f0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000c200: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000c210: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-0000c220: 6520 2a20 7465 7374 5f73 697a 652c 206c  e * test_size, l
-0000c230: 656e 286a 6f69 6e65 6429 290a 0a20 2020  en(joined))..   
-0000c240: 2020 2020 206a 6f69 6e65 6420 3d20 2874       joined = (t
-0000c250: 312e 6a6f 696e 5f6f 6e28 2761 2729 202b  1.join_on('a') +
-0000c260: 2074 3229 2829 0a20 2020 2020 2020 2077   t2)().        w
-0000c270: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000c280: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000c290: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000c2a0: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
-0000c2b0: 745f 7369 7a65 2c20 6c65 6e28 6a6f 696e  t_size, len(join
-0000c2c0: 6564 2929 0a0a 2020 2020 2020 2020 6a6f  ed))..        jo
-0000c2d0: 696e 6564 203d 2028 7431 202b 2074 322e  ined = (t1 + t2.
-0000c2e0: 6a6f 696e 5f6f 6e28 2761 2729 2928 290a  join_on('a'))().
-0000c2f0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000c300: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000c310: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000c320: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-0000c330: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
-0000c340: 206c 656e 286a 6f69 6e65 6429 290a 0a20   len(joined)).. 
-0000c350: 2020 2020 2020 2074 312e 6465 6c65 7465         t1.delete
-0000c360: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
-0000c370: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000c380: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000c390: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-0000c3a0: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
-0000c3b0: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
-0000c3c0: 2020 2020 2020 2020 206a 6f69 6e65 6420           joined 
-0000c3d0: 3d20 2874 3120 2b20 7432 2e6a 6f69 6e5f  = (t1 + t2.join_
-0000c3e0: 6f6e 2827 6127 2929 2829 0a0a 2020 2020  on('a'))()..    
-0000c3f0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000c400: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000c410: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-0000c420: 7373 6572 7452 6169 7365 7328 5479 7065  ssertRaises(Type
-0000c430: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-0000c440: 2020 2020 2020 2020 2320 696e 7661 6c69          # invali
-0000c450: 6420 6a6f 696e 2c20 6e6f 206b 7761 7267  d join, no kwarg
-0000c460: 7320 6c69 7374 696e 6720 6174 7472 6962  s listing attrib
-0000c470: 7574 6573 2074 6f20 6a6f 696e 206f 6e0a  utes to join on.
-0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c490: 7433 203d 2074 312e 6a6f 696e 2874 322c  t3 = t1.join(t2,
-0000c4a0: 2027 612c 6427 290a 0a20 2020 2020 2020   'a,d')..       
-0000c4b0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000c4c0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000c4d0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-0000c4e0: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
-0000c4f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0000c500: 2020 2020 2020 2320 696e 7661 6c69 6420        # invalid 
-0000c510: 6a6f 696e 2c20 6e6f 2073 7563 6820 6174  join, no such at
-0000c520: 7472 6962 7574 6520 277a 270a 2020 2020  tribute 'z'.    
-0000c530: 2020 2020 2020 2020 2020 2020 7433 203d              t3 =
-0000c540: 2074 312e 6a6f 696e 2874 322c 2027 612c   t1.join(t2, 'a,
-0000c550: 642c 7a27 2c20 613d 2761 2729 0a0a 2020  d,z', a='a')..  
-0000c560: 2020 2020 2020 7433 203d 2074 312e 6a6f        t3 = t1.jo
-0000c570: 696e 2874 322c 2027 612c 6427 2c20 613d  in(t2, 'a,d', a=
-0000c580: 2761 2729 0a20 2020 2020 2020 2077 6974  'a').        wit
-0000c590: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000c5a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000c5b0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-0000c5c0: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-0000c5d0: 7369 7a65 2c20 6c65 6e28 7433 2929 0a0a  size, len(t3))..
-0000c5e0: 2020 2020 2020 2020 7434 203d 2074 312e          t4 = t1.
-0000c5f0: 6a6f 696e 2874 322c 2061 3d27 6127 292e  join(t2, a='a').
-0000c600: 7365 6c65 6374 2827 6120 6320 6427 2c20  select('a c d', 
-0000c610: 653d 6c61 6d62 6461 2072 6563 3a20 7265  e=lambda rec: re
-0000c620: 632e 6120 2b20 7265 632e 6320 2b20 7265  c.a + rec.c + re
-0000c630: 632e 6429 0a20 2020 2020 2020 2077 6974  c.d).        wit
-0000c640: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000c650: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000c660: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-0000c670: 6c28 7265 632e 6520 3d3d 2072 6563 2e61  l(rec.e == rec.a
-0000c680: 2b72 6563 2e63 2b72 6563 2e64 2066 6f72  +rec.c+rec.d for
-0000c690: 2072 6563 2069 6e20 7434 2929 0a0a 2020   rec in t4))..  
-0000c6a0: 2020 2020 2020 2320 6a6f 696e 2074 6f20        # join to 
-0000c6b0: 656d 7074 7920 6c69 7374 2c20 7368 6f75  empty list, shou
-0000c6c0: 6c64 2072 6574 7572 6e20 656d 7074 7920  ld return empty 
-0000c6d0: 7461 626c 650a 2020 2020 2020 2020 656d  table.        em
-0000c6e0: 7074 795f 7461 626c 6520 3d20 6c74 2e54  pty_table = lt.T
-0000c6f0: 6162 6c65 2829 0a20 2020 2020 2020 2065  able().        e
-0000c700: 6d70 7479 5f74 6162 6c65 2e63 7265 6174  mpty_table.creat
-0000c710: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
-0000c720: 2020 2020 2074 3520 3d20 2874 312e 6a6f       t5 = (t1.jo
-0000c730: 696e 5f6f 6e28 2761 2729 202b 2065 6d70  in_on('a') + emp
-0000c740: 7479 5f74 6162 6c65 2928 290a 2020 2020  ty_table)().    
-0000c750: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000c760: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000c770: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000c780: 4571 7561 6c28 302c 206c 656e 2874 3529  Equal(0, len(t5)
-0000c790: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000c7a0: 6f75 7465 725f 6a6f 696e 7328 7365 6c66  outer_joins(self
-0000c7b0: 293a 0a20 2020 2020 2020 2074 3120 3d20  ):.        t1 = 
-0000c7c0: 6c74 2e54 6162 6c65 2822 6361 7461 6c6f  lt.Table("catalo
-0000c7d0: 6722 290a 2020 2020 2020 2020 7431 2e63  g").        t1.c
-0000c7e0: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
-0000c7f0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000c800: 2020 2020 2020 2020 2020 2073 6b75 2c63             sku,c
-0000c810: 6f6c 6f72 2c73 697a 652c 6d61 7465 7269  olor,size,materi
-0000c820: 616c 0a20 2020 2020 2020 2020 2020 2030  al.            0
-0000c830: 3031 2c72 6564 2c58 4c2c 636f 7474 6f6e  01,red,XL,cotton
-0000c840: 0a20 2020 2020 2020 2020 2020 2030 3032  .            002
-0000c850: 2c62 6c75 652c 584c 2c63 6f74 746f 6e2f  ,blue,XL,cotton/
-0000c860: 706f 6c79 0a20 2020 2020 2020 2020 2020  poly.           
-0000c870: 2030 3033 2c62 6c75 652c 4c2c 6c69 6e65   003,blue,L,line
-0000c880: 6e0a 2020 2020 2020 2020 2020 2020 3030  n.            00
-0000c890: 342c 7265 642c 4d2c 636f 7474 6f6e 0a20  4,red,M,cotton. 
-0000c8a0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
-0000c8b0: 0a0a 2020 2020 2020 2020 7432 203d 206c  ..        t2 = l
-0000c8c0: 742e 5461 626c 6528 2270 7269 6365 7322  t.Table("prices"
-0000c8d0: 290a 2020 2020 2020 2020 7432 2e63 7376  ).        t2.csv
-0000c8e0: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000c8f0: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000c900: 2020 2020 2020 2020 2073 6b75 2c75 6e69           sku,uni
-0000c910: 745f 7072 6963 652c 7369 7a65 0a20 2020  t_price,size.   
-0000c920: 2020 2020 2020 2020 2030 3031 2c31 302c           001,10,
-0000c930: 4c0a 2020 2020 2020 2020 2020 2020 3030  L.            00
-0000c940: 312c 3132 2c58 4c0a 2020 2020 2020 2020  1,12,XL.        
-0000c950: 2020 2020 3030 322c 3131 2c0a 2020 2020      002,11,.    
-0000c960: 2020 2020 2020 2020 3030 342c 392c 0a20          004,9,. 
-0000c970: 2020 2020 2020 2020 2020 2022 2222 292c             """),
-0000c980: 2074 7261 6e73 666f 726d 733d 7b27 7369   transforms={'si
-0000c990: 7a65 273a 206c 616d 6264 6120 783a 2078  ze': lambda x: x
-0000c9a0: 206f 7220 4e6f 6e65 7d29 0a20 2020 2020   or None}).     
-0000c9b0: 2020 2070 7269 6e74 2874 312e 696e 666f     print(t1.info
-0000c9c0: 2829 290a 0a20 2020 2020 2020 2074 312e  ())..        t1.
-0000c9d0: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
-0000c9e0: 2020 7432 2e70 7265 7365 6e74 2829 0a0a    t2.present()..
-0000c9f0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
-0000ca00: 6a6f 696e 2874 322c 2061 7574 6f5f 6372  join(t2, auto_cr
-0000ca10: 6561 7465 5f69 6e64 6578 6573 3d54 7275  eate_indexes=Tru
-0000ca20: 652c 2073 6b75 3d22 736b 7522 290a 2020  e, sku="sku").  
-0000ca30: 2020 2020 2020 7072 696e 7428 7433 2e69        print(t3.i
-0000ca40: 6e66 6f28 2929 0a20 2020 2020 2020 2074  nfo()).        t
-0000ca50: 332e 7072 6573 656e 7428 290a 2020 2020  3.present().    
-0000ca60: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000ca70: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000ca80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ca90: 4571 7561 6c28 342c 206c 656e 2874 3329  Equal(4, len(t3)
-0000caa0: 290a 0a20 2020 2020 2020 2074 3320 3d20  )..        t3 = 
-0000cab0: 7431 2e6a 6f69 6e28 7432 2c20 6175 746f  t1.join(t2, auto
-0000cac0: 5f63 7265 6174 655f 696e 6465 7865 733d  _create_indexes=
-0000cad0: 5472 7565 2c20 736b 753d 2273 6b75 222c  True, sku="sku",
-0000cae0: 2073 697a 653d 2273 697a 6522 290a 2020   size="size").  
-0000caf0: 2020 2020 2020 7433 2822 696e 6e65 7220        t3("inner 
-0000cb00: 6a6f 696e 202d 2022 202b 2074 332e 7461  join - " + t3.ta
-0000cb10: 626c 655f 6e61 6d65 290a 2020 2020 2020  ble_name).      
-0000cb20: 2020 7072 696e 7428 7433 2e69 6e66 6f28    print(t3.info(
-0000cb30: 2929 0a20 2020 2020 2020 2074 332e 7072  )).        t3.pr
-0000cb40: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-0000cb50: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000cb60: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000cb70: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000cb80: 6c28 312c 206c 656e 2874 3329 290a 0a20  l(1, len(t3)).. 
-0000cb90: 2020 2020 2020 2074 3320 3d20 7431 2e6f         t3 = t1.o
-0000cba0: 7574 6572 5f6a 6f69 6e28 6c74 2e54 6162  uter_join(lt.Tab
-0000cbb0: 6c65 2e52 4947 4854 5f4f 5554 4552 5f4a  le.RIGHT_OUTER_J
-0000cbc0: 4f49 4e2c 2074 322c 2073 6b75 3d22 736b  OIN, t2, sku="sk
-0000cbd0: 7522 2c20 7369 7a65 3d22 7369 7a65 2229  u", size="size")
-0000cbe0: 0a20 2020 2020 2020 2074 3328 2272 6967  .        t3("rig
-0000cbf0: 6874 206f 7574 6572 206a 6f69 6e20 2d20  ht outer join - 
-0000cc00: 2220 2b20 7433 2e74 6162 6c65 5f6e 616d  " + t3.table_nam
-0000cc10: 6529 0a20 2020 2020 2020 2070 7269 6e74  e).        print
-0000cc20: 2874 332e 696e 666f 2829 290a 2020 2020  (t3.info()).    
-0000cc30: 2020 2020 7433 2e70 7265 7365 6e74 2829      t3.present()
-0000cc40: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000cc50: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000cc60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000cc70: 7373 6572 7445 7175 616c 2834 2c20 6c65  ssertEqual(4, le
-0000cc80: 6e28 7433 2929 0a0a 2020 2020 2020 2020  n(t3))..        
-0000cc90: 7433 203d 2074 312e 6f75 7465 725f 6a6f  t3 = t1.outer_jo
-0000cca0: 696e 286c 742e 5461 626c 652e 4c45 4654  in(lt.Table.LEFT
-0000ccb0: 5f4f 5554 4552 5f4a 4f49 4e2c 2074 322c  _OUTER_JOIN, t2,
-0000ccc0: 2073 6b75 3d22 736b 7522 2c20 7369 7a65   sku="sku", size
-0000ccd0: 3d22 7369 7a65 2229 0a20 2020 2020 2020  ="size").       
-0000cce0: 2074 3328 226c 6566 7420 6f75 7465 7220   t3("left outer 
-0000ccf0: 6a6f 696e 202d 2022 202b 2074 332e 7461  join - " + t3.ta
-0000cd00: 626c 655f 6e61 6d65 290a 2020 2020 2020  ble_name).      
-0000cd10: 2020 7072 696e 7428 7433 2e69 6e66 6f28    print(t3.info(
-0000cd20: 2929 0a20 2020 2020 2020 2074 332e 7072  )).        t3.pr
-0000cd30: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-0000cd40: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000cd50: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000cd60: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000cd70: 6c28 322c 206c 656e 2874 3329 290a 0a20  l(2, len(t3)).. 
-0000cd80: 2020 2020 2020 2074 3320 3d20 7431 2e6f         t3 = t1.o
-0000cd90: 7574 6572 5f6a 6f69 6e28 6c74 2e54 6162  uter_join(lt.Tab
-0000cda0: 6c65 2e46 554c 4c5f 4f55 5445 525f 4a4f  le.FULL_OUTER_JO
-0000cdb0: 494e 2c20 7432 2c20 736b 753d 2273 6b75  IN, t2, sku="sku
-0000cdc0: 222c 2073 697a 653d 2273 697a 6522 290a  ", size="size").
-0000cdd0: 2020 2020 2020 2020 7433 2822 6675 6c6c          t3("full
-0000cde0: 206f 7574 6572 206a 6f69 6e20 2d20 2220   outer join - " 
-0000cdf0: 2b20 7433 2e74 6162 6c65 5f6e 616d 6529  + t3.table_name)
-0000ce00: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
-0000ce10: 332e 696e 666f 2829 290a 2020 2020 2020  3.info()).      
-0000ce20: 2020 7433 2e70 7265 7365 6e74 2829 0a20    t3.present(). 
-0000ce30: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000ce40: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-0000ce50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000ce60: 6572 7445 7175 616c 2831 322c 206c 656e  ertEqual(12, len
-0000ce70: 2874 3329 290a 0a20 2020 2064 6566 2074  (t3))..    def t
-0000ce80: 6573 745f 6f75 7465 725f 6a6f 696e 5f65  est_outer_join_e
-0000ce90: 7861 6d70 6c65 2873 656c 6629 3a0a 2020  xample(self):.  
-0000cea0: 2020 2020 2020 2320 6465 6669 6e65 2073        # define s
-0000ceb0: 7475 6465 6e74 2061 6e64 2072 6567 6973  tudent and regis
-0000cec0: 7472 6174 696f 6e20 6461 7461 0a20 2020  tration data.   
-0000ced0: 2020 2020 2073 7475 6465 6e74 7320 3d20       students = 
-0000cee0: 6c74 2e54 6162 6c65 2822 7374 7564 656e  lt.Table("studen
-0000cef0: 7473 2229 2e63 7376 5f69 6d70 6f72 7428  ts").csv_import(
-0000cf00: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-0000cf10: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
-0000cf20: 2073 7475 6465 6e74 5f69 642c 6e61 6d65   student_id,name
-0000cf30: 0a20 2020 2020 2020 2020 2020 2030 3030  .            000
-0000cf40: 312c 416c 6963 650a 2020 2020 2020 2020  1,Alice.        
-0000cf50: 2020 2020 3030 3032 2c42 6f62 0a20 2020      0002,Bob.   
-0000cf60: 2020 2020 2020 2020 2030 3030 332c 4368           0003,Ch
-0000cf70: 6172 6c69 650a 2020 2020 2020 2020 2020  arlie.          
-0000cf80: 2020 3030 3034 2c44 6176 650a 2020 2020    0004,Dave.    
-0000cf90: 2020 2020 2020 2020 3030 3035 2c45 6e69          0005,Eni
-0000cfa0: 640a 2020 2020 2020 2020 2020 2020 2222  d.            ""
-0000cfb0: 2229 290a 0a20 2020 2020 2020 2072 6567  "))..        reg
-0000cfc0: 6973 7472 6174 696f 6e73 203d 206c 742e  istrations = lt.
-0000cfd0: 5461 626c 6528 2272 6567 6973 7472 6174  Table("registrat
-0000cfe0: 696f 6e73 2229 2e63 7376 5f69 6d70 6f72  ions").csv_impor
-0000cff0: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000d000: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000d010: 2020 2073 7475 6465 6e74 5f69 642c 636f     student_id,co
-0000d020: 7572 7365 0a20 2020 2020 2020 2020 2020  urse.           
-0000d030: 2030 3030 312c 5053 5943 4831 3031 0a20   0001,PSYCH101. 
-0000d040: 2020 2020 2020 2020 2020 2030 3030 312c             0001,
-0000d050: 4341 4c43 310a 2020 2020 2020 2020 2020  CALC1.          
-0000d060: 2020 3030 3033 2c42 494f 3230 300a 2020    0003,BIO200.  
-0000d070: 2020 2020 2020 2020 2020 3030 3035 2c43            0005,C
-0000d080: 4845 4d31 3031 0a20 2020 2020 2020 2020  HEM101.         
-0000d090: 2020 2030 3030 362c 5048 5931 3031 0a20     0006,PHY101. 
-0000d0a0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
-0000d0b0: 0a0a 2020 2020 2020 2020 636f 7572 7365  ..        course
-0000d0c0: 7320 3d20 6c74 2e54 6162 6c65 2822 636f  s = lt.Table("co
-0000d0d0: 7572 7365 7322 292e 6373 765f 696d 706f  urses").csv_impo
-0000d0e0: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
-0000d0f0: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000d100: 2020 2020 636f 7572 7365 0a20 2020 2020      course.     
-0000d110: 2020 2020 2020 2042 494f 3230 300a 2020         BIO200.  
-0000d120: 2020 2020 2020 2020 2020 4341 4c43 310a            CALC1.
-0000d130: 2020 2020 2020 2020 2020 2020 4348 454d              CHEM
-0000d140: 3130 310a 2020 2020 2020 2020 2020 2020  101.            
-0000d150: 5053 5943 4831 3031 0a20 2020 2020 2020  PSYCH101.       
-0000d160: 2020 2020 2050 4531 3031 0a20 2020 2020       PE101.     
-0000d170: 2020 2020 2020 2022 2222 2929 0a0a 2020         """))..  
-0000d180: 2020 2020 2020 2320 7065 7266 6f72 6d20        # perform 
-0000d190: 6f75 7465 7220 6a6f 696e 2061 6e64 2073  outer join and s
-0000d1a0: 686f 7720 7265 7375 6c74 733a 0a20 2020  how results:.   
-0000d1b0: 2020 2020 206e 6f6e 5f72 6567 203d 2073       non_reg = s
-0000d1c0: 7475 6465 6e74 732e 6f75 7465 725f 6a6f  tudents.outer_jo
-0000d1d0: 696e 286c 742e 5461 626c 652e 5249 4748  in(lt.Table.RIGH
-0000d1e0: 545f 4f55 5445 525f 4a4f 494e 2c0a 2020  T_OUTER_JOIN,.  
-0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d210: 2020 2020 7265 6769 7374 7261 7469 6f6e      registration
-0000d220: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 2020 2020 2020 2020 2073 7475 6465 6e74           student
-0000d250: 5f69 643d 2273 7475 6465 6e74 5f69 6422  _id="student_id"
-0000d260: 292e 7768 6572 6528 636f 7572 7365 3d4e  ).where(course=N
-0000d270: 6f6e 6529 0a20 2020 2020 2020 206e 6f6e  one).        non
-0000d280: 5f72 6567 2e70 7265 7365 6e74 2829 0a20  _reg.present(). 
-0000d290: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
-0000d2a0: 7428 6e6f 6e5f 7265 672e 616c 6c2e 6e61  t(non_reg.all.na
-0000d2b0: 6d65 2929 0a20 2020 2020 2020 2077 6974  me)).        wit
-0000d2c0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000d2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000d2e0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
-0000d2f0: 2742 6f62 272c 2027 4461 7665 275d 2c20  'Bob', 'Dave'], 
-0000d300: 736f 7274 6564 286e 6f6e 5f72 6567 2e61  sorted(non_reg.a
-0000d310: 6c6c 2e6e 616d 6529 290a 0a20 2020 2020  ll.name))..     
-0000d320: 2020 2023 2063 6f75 7273 6573 2077 6974     # courses wit
-0000d330: 6820 6e6f 2073 7475 6465 6e74 730a 2020  h no students.  
-0000d340: 2020 2020 2020 6e6f 5f73 7475 6465 6e74        no_student
-0000d350: 7320 3d20 7265 6769 7374 7261 7469 6f6e  s = registration
-0000d360: 732e 6f75 7465 725f 6a6f 696e 286c 742e  s.outer_join(lt.
-0000d370: 5461 626c 652e 4c45 4654 5f4f 5554 4552  Table.LEFT_OUTER
-0000d380: 5f4a 4f49 4e2c 0a20 2020 2020 2020 2020  _JOIN,.         
-0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3b0: 636f 7572 7365 732c 0a20 2020 2020 2020  courses,.       
-0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 636f 7572 7365 3d22 636f 7572 7365    course="course
-0000d3f0: 2229 2e77 6865 7265 2873 7475 6465 6e74  ").where(student
-0000d400: 5f69 643d 4e6f 6e65 290a 2020 2020 2020  _id=None).      
-0000d410: 2020 6e6f 5f73 7475 6465 6e74 732e 7072    no_students.pr
-0000d420: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-0000d430: 7072 696e 7428 6c69 7374 286e 6f5f 7374  print(list(no_st
-0000d440: 7564 656e 7473 2e61 6c6c 2e63 6f75 7273  udents.all.cours
-0000d450: 6529 290a 2020 2020 2020 2020 7769 7468  e)).        with
-0000d460: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000d470: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d480: 662e 6173 7365 7274 4571 7561 6c28 5b27  f.assertEqual(['
-0000d490: 5045 3130 3127 5d2c 2073 6f72 7465 6428  PE101'], sorted(
-0000d4a0: 6e6f 5f73 7475 6465 6e74 732e 616c 6c2e  no_students.all.
-0000d4b0: 636f 7572 7365 2929 0a0a 0a20 2020 2020  course))...     
-0000d4c0: 2020 2066 756c 6c20 3d20 2073 7475 6465     full =  stude
-0000d4d0: 6e74 732e 6f75 7465 725f 6a6f 696e 286c  nts.outer_join(l
-0000d4e0: 742e 5461 626c 652e 4655 4c4c 5f4f 5554  t.Table.FULL_OUT
-0000d4f0: 4552 5f4a 4f49 4e2c 0a20 2020 2020 2020  ER_JOIN,.       
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d520: 6567 6973 7472 6174 696f 6e73 2c0a 2020  egistrations,.  
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d550: 2020 2020 7374 7564 656e 745f 6964 3d22      student_id="
-0000d560: 7374 7564 656e 745f 6964 2229 2e77 6865  student_id").whe
-0000d570: 7265 286c 616d 6264 6120 7265 633a 2072  re(lambda rec: r
-0000d580: 6563 2e63 6f75 7273 6520 6973 204e 6f6e  ec.course is Non
-0000d590: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 2020 206f 7220 7265 632e 6e61 6d65 2069     or rec.name i
-0000d5f0: 7320 4e6f 6e65 290a 2020 2020 2020 2020  s None).        
-0000d600: 6675 6c6c 2e70 7265 7365 6e74 2829 0a20  full.present(). 
-0000d610: 2020 2020 2020 2070 7269 6e74 2873 6f72         print(sor
-0000d620: 7465 6428 6675 6c6c 2e61 6c6c 2e73 7475  ted(full.all.stu
-0000d630: 6465 6e74 5f69 6429 290a 2020 2020 2020  dent_id)).      
-0000d640: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000d650: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000d660: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000d670: 7561 6c28 5b27 3030 3032 272c 2027 3030  ual(['0002', '00
-0000d680: 3034 272c 2027 3030 3036 275d 2c20 736f  04', '0006'], so
-0000d690: 7274 6564 2866 756c 6c2e 616c 6c2e 7374  rted(full.all.st
-0000d6a0: 7564 656e 745f 6964 2929 0a0a 0a40 6d61  udent_id))...@ma
-0000d6b0: 6b65 5f74 6573 745f 636c 6173 7365 730a  ke_test_classes.
-0000d6c0: 636c 6173 7320 5461 626c 6554 7261 6e73  class TableTrans
-0000d6d0: 666f 726d 5465 7374 733a 0a20 2020 2022  formTests:.    "
-0000d6e0: 2222 0a20 2020 2054 6573 7473 2074 6f20  "".    Tests to 
-0000d6f0: 6d75 7461 7465 2061 2054 6162 6c65 2e0a  mutate a Table..
-0000d700: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000d710: 7465 7374 5f73 6f72 7428 7365 6c66 293a  test_sort(self):
-0000d720: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-0000d730: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
-0000d740: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
-0000d750: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
-0000d760: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
-0000d770: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
-0000d780: 635f 6772 6f75 7073 203d 2030 0a20 2020  c_groups = 0.   
-0000d790: 2020 2020 2066 6f72 2063 5f76 616c 7565       for c_value
-0000d7a0: 2c20 7265 6373 2069 6e20 6974 6572 746f  , recs in iterto
-0000d7b0: 6f6c 732e 6772 6f75 7062 7928 7431 2c20  ols.groupby(t1, 
-0000d7c0: 6b65 793d 6c61 6d62 6461 2072 6563 3a20  key=lambda rec: 
-0000d7d0: 7265 632e 6329 3a0a 2020 2020 2020 2020  rec.c):.        
-0000d7e0: 2020 2020 635f 6772 6f75 7073 202b 3d20      c_groups += 
-0000d7f0: 310a 2020 2020 2020 2020 2020 2020 6c69  1.            li
-0000d800: 7374 2872 6563 7329 0a20 2020 2020 2020  st(recs).       
-0000d810: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000d820: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000d830: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000d840: 616c 2874 6573 745f 7369 7a65 202a 2074  al(test_size * t
-0000d850: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-0000d860: 7369 7a65 2c20 635f 6772 6f75 7073 290a  size, c_groups).
-0000d870: 0a20 2020 2020 2020 2074 312e 736f 7274  .        t1.sort
-0000d880: 2827 6327 290a 2020 2020 2020 2020 635f  ('c').        c_
-0000d890: 6772 6f75 7073 203d 2030 0a20 2020 2020  groups = 0.     
-0000d8a0: 2020 2066 6f72 2063 5f76 616c 7565 2c20     for c_value, 
-0000d8b0: 7265 6373 2069 6e20 6974 6572 746f 6f6c  recs in itertool
-0000d8c0: 732e 6772 6f75 7062 7928 7431 2c20 6b65  s.groupby(t1, ke
-0000d8d0: 793d 6c61 6d62 6461 2072 6563 3a20 7265  y=lambda rec: re
-0000d8e0: 632e 6329 3a0a 2020 2020 2020 2020 2020  c.c):.          
-0000d8f0: 2020 635f 6772 6f75 7073 202b 3d20 310a    c_groups += 1.
-0000d900: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-0000d910: 2872 6563 7329 0a20 2020 2020 2020 2077  (recs).        w
-0000d920: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000d930: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000d940: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000d950: 2874 6573 745f 7369 7a65 2c20 635f 6772  (test_size, c_gr
-0000d960: 6f75 7073 290a 2020 2020 2020 2020 7769  oups).        wi
-0000d970: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000d980: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000d990: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000d9a0: 302c 2074 315b 305d 2e63 290a 0a20 2020  0, t1[0].c)..   
-0000d9b0: 2020 2020 2074 312e 736f 7274 2827 6320       t1.sort('c 
-0000d9c0: 6465 7363 2729 0a20 2020 2020 2020 2077  desc').        w
-0000d9d0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000d9e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000d9f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000da00: 2874 6573 745f 7369 7a65 2d31 2c20 7431  (test_size-1, t1
-0000da10: 5b30 5d2e 6329 0a0a 2020 2020 6465 6620  [0].c)..    def 
-0000da20: 7465 7374 5f73 6f72 7432 2873 656c 6629  test_sort2(self)
-0000da30: 3a0a 0a20 2020 2020 2020 2072 6f77 5f74  :..        row_t
-0000da40: 7970 6520 3d20 7479 7065 2873 656c 662e  ype = type(self.
-0000da50: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-0000da60: 2830 2c30 2c30 2929 0a20 2020 2020 2020  (0,0,0)).       
-0000da70: 2074 7420 3d20 6c74 2e54 6162 6c65 2829   tt = lt.Table()
-0000da80: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-0000da90: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000daa0: 0a20 2020 2020 2020 2061 2c63 2c62 0a20  .        a,c,b. 
-0000dab0: 2020 2020 2020 2031 2c32 2c31 0a20 2020         1,2,1.   
-0000dac0: 2020 2020 2032 2c33 2c30 0a20 2020 2020       2,3,0.     
-0000dad0: 2020 2035 2c35 2c2d 310a 2020 2020 2020     5,5,-1.      
-0000dae0: 2020 332c 342c 2d31 0a20 2020 2020 2020    3,4,-1.       
-0000daf0: 2032 2c34 2c2d 3322 2222 292c 2072 6f77   2,4,-3"""), row
-0000db00: 5f63 6c61 7373 3d72 6f77 5f74 7970 652c  _class=row_type,
-0000db10: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
-0000db20: 2e66 726f 6d6b 6579 7328 2261 2062 2063  .fromkeys("a b c
-0000db30: 222e 7370 6c69 7428 292c 2069 6e74 2929  ".split(), int))
-0000db40: 0a0a 2020 2020 2020 2020 6465 6620 746f  ..        def to
-0000db50: 5f74 7570 6c65 7328 7429 3a0a 2020 2020  _tuples(t):.    
-0000db60: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-0000db70: 6973 7428 6d61 7028 6174 7472 6765 7474  ist(map(attrgett
-0000db80: 6572 282a 742e 696e 666f 2829 5b27 6669  er(*t.info()['fi
-0000db90: 656c 6473 275d 292c 2074 2929 0a0a 2020  elds']), t))..  
-0000dba0: 2020 2020 2020 7072 696e 7428 7474 2e69        print(tt.i
-0000dbb0: 6e66 6f28 295b 2766 6965 6c64 7327 5d29  nfo()['fields'])
-0000dbc0: 0a0a 2020 2020 2020 2020 736f 7274 5f61  ..        sort_a
-0000dbd0: 7267 203d 2022 6320 6222 2e73 706c 6974  rg = "c b".split
-0000dbe0: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
-0000dbf0: 2866 2253 6f72 7469 6e67 2062 7920 7b73  (f"Sorting by {s
-0000dc00: 6f72 745f 6172 6721 727d 2229 0a20 2020  ort_arg!r}").   
-0000dc10: 2020 2020 2074 742e 7368 7566 666c 6528       tt.shuffle(
-0000dc20: 290a 2020 2020 2020 2020 7474 2e73 6f72  ).        tt.sor
-0000dc30: 7428 736f 7274 5f61 7267 290a 2020 2020  t(sort_arg).    
-0000dc40: 2020 2020 7431 5f74 7570 6c65 7320 3d20      t1_tuples = 
-0000dc50: 746f 5f74 7570 6c65 7328 7474 290a 2020  to_tuples(tt).  
-0000dc60: 2020 2020 2020 666f 7220 7420 696e 2074        for t in t
-0000dc70: 315f 7475 706c 6573 3a0a 2020 2020 2020  1_tuples:.      
-0000dc80: 2020 2020 2020 7072 696e 7428 7429 0a20        print(t). 
-0000dc90: 2020 2020 2020 2070 7269 6e74 2829 0a0a         print()..
-0000dca0: 2020 2020 2020 2020 7474 2e73 6875 6666          tt.shuff
-0000dcb0: 6c65 2829 0a20 2020 2020 2020 2074 742e  le().        tt.
-0000dcc0: 736f 7274 2822 6222 290a 2020 2020 2020  sort("b").      
-0000dcd0: 2020 7474 2e73 6f72 7428 2263 2229 0a20    tt.sort("c"). 
-0000dce0: 2020 2020 2020 2074 325f 7475 706c 6573         t2_tuples
-0000dcf0: 203d 2074 6f5f 7475 706c 6573 2874 7429   = to_tuples(tt)
-0000dd00: 0a20 2020 2020 2020 2066 6f72 2074 2069  .        for t i
-0000dd10: 6e20 7432 5f74 7570 6c65 733a 0a20 2020  n t2_tuples:.   
-0000dd20: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
-0000dd30: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000dd40: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-0000dd50: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-0000dd60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dd70: 2e61 7373 6572 7445 7175 616c 2874 315f  .assertEqual(t1_
-0000dd80: 7475 706c 6573 2c20 7432 5f74 7570 6c65  tuples, t2_tuple
-0000dd90: 732c 2022 6661 696c 6564 206d 756c 7469  s, "failed multi
-0000dda0: 2d61 7474 7269 6275 7465 2073 6f72 742c  -attribute sort,
-0000ddb0: 2067 6976 656e 206c 6973 7420 6f66 2061   given list of a
-0000ddc0: 7474 7269 6275 7465 7322 290a 0a20 2020  ttributes")..   
-0000ddd0: 2020 2020 2073 6f72 745f 6172 6720 3d20       sort_arg = 
-0000dde0: 2263 2c62 220a 2020 2020 2020 2020 7072  "c,b".        pr
-0000ddf0: 696e 7428 6622 536f 7274 696e 6720 6279  int(f"Sorting by
-0000de00: 207b 736f 7274 5f61 7267 2172 7d22 290a   {sort_arg!r}").
-0000de10: 2020 2020 2020 2020 7474 2e73 6875 6666          tt.shuff
-0000de20: 6c65 2829 0a20 2020 2020 2020 2074 742e  le().        tt.
-0000de30: 736f 7274 2873 6f72 745f 6172 6729 0a20  sort(sort_arg). 
-0000de40: 2020 2020 2020 2074 315f 7475 706c 6573         t1_tuples
-0000de50: 203d 2074 6f5f 7475 706c 6573 2874 7429   = to_tuples(tt)
-0000de60: 0a20 2020 2020 2020 2066 6f72 2074 2069  .        for t i
-0000de70: 6e20 7431 5f74 7570 6c65 733a 0a20 2020  n t1_tuples:.   
-0000de80: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
-0000de90: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000dea0: 290a 0a20 2020 2020 2020 2074 742e 7368  )..        tt.sh
-0000deb0: 7566 666c 6528 290a 2020 2020 2020 2020  uffle().        
-0000dec0: 7474 2e73 6f72 7428 2262 2229 0a20 2020  tt.sort("b").   
-0000ded0: 2020 2020 2074 742e 736f 7274 2822 6322       tt.sort("c"
-0000dee0: 290a 2020 2020 2020 2020 7432 5f74 7570  ).        t2_tup
-0000def0: 6c65 7320 3d20 746f 5f74 7570 6c65 7328  les = to_tuples(
-0000df00: 7474 290a 2020 2020 2020 2020 666f 7220  tt).        for 
-0000df10: 7420 696e 2074 325f 7475 706c 6573 3a0a  t in t2_tuples:.
-0000df20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000df30: 7428 7429 0a20 2020 2020 2020 2070 7269  t(t).        pri
-0000df40: 6e74 2829 0a0a 2020 2020 2020 2020 7769  nt()..        wi
-0000df50: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000df60: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000df70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000df80: 7431 5f74 7570 6c65 732c 2074 325f 7475  t1_tuples, t2_tu
-0000df90: 706c 6573 2c20 2266 6169 6c65 6420 6d75  ples, "failed mu
-0000dfa0: 6c74 692d 6174 7472 6962 7574 6520 736f  lti-attribute so
-0000dfb0: 7274 2c20 6769 7665 6e20 636f 6d6d 612d  rt, given comma-
-0000dfc0: 7365 7061 7261 7465 6420 6174 7472 6962  separated attrib
-0000dfd0: 7574 6573 2073 7472 696e 6722 290a 0a20  utes string").. 
-0000dfe0: 2020 2020 2020 2073 6f72 745f 6172 6720         sort_arg 
-0000dff0: 3d20 2263 2c62 2064 6573 6322 0a20 2020  = "c,b desc".   
-0000e000: 2020 2020 2070 7269 6e74 2866 2253 6f72       print(f"Sor
-0000e010: 7469 6e67 2062 7920 7b73 6f72 745f 6172  ting by {sort_ar
-0000e020: 6721 727d 2229 0a20 2020 2020 2020 2074  g!r}").        t
-0000e030: 742e 7368 7566 666c 6528 290a 2020 2020  t.shuffle().    
-0000e040: 2020 2020 7474 2e73 6f72 7428 736f 7274      tt.sort(sort
-0000e050: 5f61 7267 290a 2020 2020 2020 2020 7431  _arg).        t1
-0000e060: 5f74 7570 6c65 7320 3d20 746f 5f74 7570  _tuples = to_tup
-0000e070: 6c65 7328 7474 290a 2020 2020 2020 2020  les(tt).        
-0000e080: 666f 7220 7420 696e 2074 315f 7475 706c  for t in t1_tupl
-0000e090: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000e0a0: 7072 696e 7428 7429 0a20 2020 2020 2020  print(t).       
-0000e0b0: 2070 7269 6e74 2829 0a0a 2020 2020 2020   print()..      
-0000e0c0: 2020 7474 2e73 6875 6666 6c65 2829 0a20    tt.shuffle(). 
-0000e0d0: 2020 2020 2020 2074 742e 736f 7274 2822         tt.sort("
-0000e0e0: 6220 6465 7363 2229 0a20 2020 2020 2020  b desc").       
-0000e0f0: 2074 742e 736f 7274 2822 6322 290a 2020   tt.sort("c").  
-0000e100: 2020 2020 2020 7432 5f74 7570 6c65 7320        t2_tuples 
-0000e110: 3d20 746f 5f74 7570 6c65 7328 7474 290a  = to_tuples(tt).
-0000e120: 2020 2020 2020 2020 666f 7220 7420 696e          for t in
-0000e130: 2074 325f 7475 706c 6573 3a0a 2020 2020   t2_tuples:.    
-0000e140: 2020 2020 2020 2020 7072 696e 7428 7429          print(t)
-0000e150: 0a20 2020 2020 2020 2070 7269 6e74 2829  .        print()
-0000e160: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-0000e170: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000e180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e190: 6173 7365 7274 4571 7561 6c28 7431 5f74  assertEqual(t1_t
-0000e1a0: 7570 6c65 732c 2074 325f 7475 706c 6573  uples, t2_tuples
-0000e1b0: 2c20 2266 6169 6c65 6420 6d69 7865 6420  , "failed mixed 
-0000e1c0: 6173 6365 6e64 696e 672f 6465 7363 656e  ascending/descen
-0000e1d0: 6469 6e67 206d 756c 7469 2d61 7474 7269  ding multi-attri
-0000e1e0: 6275 7465 2073 6f72 7422 290a 0a20 2020  bute sort")..   
-0000e1f0: 2064 6566 2074 6573 745f 736f 7274 3328   def test_sort3(
-0000e200: 7365 6c66 293a 0a20 2020 2020 2020 2065  self):.        e
-0000e210: 6d70 6c6f 7965 6573 203d 206c 742e 5461  mployees = lt.Ta
-0000e220: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000e230: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000e240: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000e250: 2020 656d 705f 6964 2c6e 616d 652c 6465    emp_id,name,de
-0000e260: 7074 2c73 616c 6172 792c 636f 6d6d 6973  pt,salary,commis
-0000e270: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
-0000e280: 2030 3030 312c 416c 6963 652c 5361 6c65   0001,Alice,Sale
-0000e290: 732c 3530 3030 302c 302e 350a 2020 2020  s,50000,0.5.    
-0000e2a0: 2020 2020 2020 2020 3030 3032 2c42 6f62          0002,Bob
-0000e2b0: 2c45 6e67 696e 6565 7269 6e67 2c31 3030  ,Engineering,100
-0000e2c0: 3030 302c 0a20 2020 2020 2020 2020 2020  000,.           
-0000e2d0: 2030 3030 332c 4368 6172 6c65 732c 5361   0003,Charles,Sa
-0000e2e0: 6c65 732c 3435 3030 302c 302e 370a 2020  les,45000,0.7.  
-0000e2f0: 2020 2020 2020 2020 2020 3030 3034 2c44            0004,D
-0000e300: 6176 652c 5361 6c65 732c 3435 3030 302c  ave,Sales,45000,
-0000e310: 302e 360a 2020 2020 2020 2020 2020 2020  0.6.            
-0000e320: 3030 3035 2c45 6d69 6c79 2c53 616c 6573  0005,Emily,Sales
-0000e330: 2c35 3030 3030 2c30 2e34 0a20 2020 2020  ,50000,0.4.     
-0000e340: 2020 2020 2020 2022 2222 292c 2074 7261         """), tra
-0000e350: 6e73 666f 726d 733d 7b22 7361 6c61 7279  nsforms={"salary
-0000e360: 223a 2069 6e74 2c20 2263 6f6d 6d69 7373  ": int, "commiss
-0000e370: 696f 6e22 3a20 666c 6f61 747d 290a 0a20  ion": float}).. 
-0000e380: 2020 2020 2020 2073 616c 6573 5f65 6d70         sales_emp
-0000e390: 6c6f 7965 6573 203d 2065 6d70 6c6f 7965  loyees = employe
-0000e3a0: 6573 2e77 6865 7265 2864 6570 743d 2253  es.where(dept="S
-0000e3b0: 616c 6573 2229 2e73 6f72 7428 2273 616c  ales").sort("sal
-0000e3c0: 6172 7920 6465 7363 2c63 6f6d 6d69 7373  ary desc,commiss
-0000e3d0: 696f 6e22 290a 0a20 2020 2020 2020 2073  ion")..        s
-0000e3e0: 616c 6573 5f65 6d70 6c6f 7965 6573 2e70  ales_employees.p
-0000e3f0: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-0000e400: 2070 7269 6e74 286c 6973 7428 7361 6c65   print(list(sale
-0000e410: 735f 656d 706c 6f79 6565 732e 616c 6c2e  s_employees.all.
-0000e420: 656d 705f 6964 2929 0a0a 2020 2020 2020  emp_id))..      
-0000e430: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000e440: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000e450: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000e460: 7561 6c28 5b27 3030 3035 272c 2027 3030  ual(['0005', '00
-0000e470: 3031 272c 2027 3030 3034 272c 2027 3030  01', '0004', '00
-0000e480: 3033 275d 2c0a 2020 2020 2020 2020 2020  03'],.          
-0000e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4a0: 2020 206c 6973 7428 7361 6c65 735f 656d     list(sales_em
-0000e4b0: 706c 6f79 6565 732e 616c 6c2e 656d 705f  ployees.all.emp_
-0000e4c0: 6964 2929 0a0a 2020 2020 6465 6620 7465  id))..    def te
-0000e4d0: 7374 5f75 6e69 7175 6528 7365 6c66 293a  st_unique(self):
-0000e4e0: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-0000e4f0: 7a65 203d 2031 300a 2020 2020 2020 2020  ze = 10.        
-0000e500: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
-0000e510: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
-0000e520: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
-0000e530: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
-0000e540: 7432 203d 2074 312e 756e 6971 7565 2829  t2 = t1.unique()
-0000e550: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000e560: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000e570: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000e580: 7373 6572 7445 7175 616c 286c 656e 2874  ssertEqual(len(t
-0000e590: 3129 2c20 6c65 6e28 7432 2929 0a0a 2020  1), len(t2))..  
-0000e5a0: 2020 2020 2020 7433 203d 2074 312e 756e        t3 = t1.un
-0000e5b0: 6971 7565 286b 6579 3d6c 616d 6264 6120  ique(key=lambda 
-0000e5c0: 7265 633a 2072 6563 2e63 290a 2020 2020  rec: rec.c).    
-0000e5d0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000e5e0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000e5f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000e600: 4571 7561 6c28 7465 7374 5f73 697a 652c  Equal(test_size,
-0000e610: 206c 656e 2874 3329 290a 0a0a 406d 616b   len(t3))...@mak
-0000e620: 655f 7465 7374 5f63 6c61 7373 6573 0a63  e_test_classes.c
-0000e630: 6c61 7373 2054 6162 6c65 4f75 7470 7574  lass TableOutput
-0000e640: 5465 7374 733a 0a20 2020 2022 2222 0a20  Tests:.    """. 
-0000e650: 2020 2054 6573 7473 2074 6f20 7665 7269     Tests to veri
-0000e660: 6679 206f 7574 7075 7420 666f 726d 7320  fy output forms 
-0000e670: 666f 7220 6120 5461 626c 652e 0a20 2020  for a Table..   
-0000e680: 2022 2222 0a20 2020 2064 6566 2074 6573   """.    def tes
-0000e690: 745f 6261 7369 635f 7072 6573 656e 7428  t_basic_present(
-0000e6a0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0000e6b0: 6620 7269 6368 2069 7320 4e6f 6e65 3a0a  f rich is None:.
-0000e6c0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-0000e6d0: 7274 2077 6172 6e69 6e67 730a 2020 2020  rt warnings.    
-0000e6e0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0000e6f0: 2e77 6172 6e28 2272 6963 6820 6e6f 7420  .warn("rich not 
-0000e700: 696e 7374 616c 6c65 642c 2063 616e 6e6f  installed, canno
-0000e710: 7420 7275 6e20 7465 7374 2229 0a20 2020  t run test").   
-0000e720: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000e730: 0a20 2020 2020 2020 2066 726f 6d20 7269  .        from ri
-0000e740: 6368 2069 6d70 6f72 7420 626f 780a 2020  ch import box.  
-0000e750: 2020 2020 2020 6672 6f6d 2069 6f20 696d        from io im
-0000e760: 706f 7274 2053 7472 696e 6749 4f0a 2020  port StringIO.  
-0000e770: 2020 2020 2020 7461 626c 6520 3d20 6c74        table = lt
-0000e780: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-0000e790: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
-0000e7a0: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-0000e7b0: 2020 2020 2061 2c62 0a20 2020 2020 2020       a,b.       
-0000e7c0: 2020 2020 2031 302c 3130 300a 2020 2020       10,100.    
-0000e7d0: 2020 2020 2020 2020 3230 2c32 3030 0a20          20,200. 
-0000e7e0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
-0000e7f0: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
-0000e800: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-0000e810: 206f 7574 203d 2053 7472 696e 6749 4f28   out = StringIO(
-0000e820: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-0000e830: 7072 6573 656e 7428 6669 6c65 3d6f 7574  present(file=out
-0000e840: 2c20 626f 783d 626f 782e 4153 4349 4929  , box=box.ASCII)
-0000e850: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-0000e860: 6420 3d20 7465 7874 7772 6170 2e64 6564  d = textwrap.ded
-0000e870: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-0000e880: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
-0000e890: 2b0a 2020 2020 2020 2020 2020 2020 7c20  +.            | 
-0000e8a0: 4120 207c 2042 2020 207c 0a20 2020 2020  A  | B   |.     
-0000e8b0: 2020 2020 2020 207c 2d2d 2d2d 2b2d 2d2d         |----+---
-0000e8c0: 2d2d 7c0a 2020 2020 2020 2020 2020 2020  --|.            
-0000e8d0: 7c20 3130 207c 2031 3030 207c 0a20 2020  | 10 | 100 |.   
-0000e8e0: 2020 2020 2020 2020 207c 2032 3020 7c20           | 20 | 
-0000e8f0: 3230 3020 7c0a 2020 2020 2020 2020 2020  200 |.          
-0000e900: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20    +----------+. 
-0000e910: 2020 2020 2020 2020 2020 2022 2222 290a             """).
-0000e920: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000e930: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000e940: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000e950: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000e960: 6564 2c20 6f75 742e 6765 7476 616c 7565  ed, out.getvalue
-0000e970: 2829 290a 0a20 2020 2020 2020 2023 2074  ())..        # t
-0000e980: 6573 7420 6275 6766 6978 2077 6865 6e20  est bugfix when 
-0000e990: 7461 626c 6520 6861 7320 6174 7472 6962  table has attrib
-0000e9a0: 7574 6520 2264 6566 6175 6c74 220a 2020  ute "default".  
-0000e9b0: 2020 2020 2020 7461 626c 6520 3d20 6c74        table = lt
-0000e9c0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-0000e9d0: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
-0000e9e0: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-0000e9f0: 2020 2020 2061 2c62 2c64 6566 6175 6c74       a,b,default
-0000ea00: 0a20 2020 2020 2020 2020 2020 2031 302c  .            10,
-0000ea10: 3130 302c 7075 7270 6c65 0a20 2020 2020  100,purple.     
-0000ea20: 2020 2020 2020 2031 352c 3135 302c 0a20         15,150,. 
-0000ea30: 2020 2020 2020 2020 2020 2032 302c 3230             20,20
-0000ea40: 302c 6f72 616e 6765 0a20 2020 2020 2020  0,orange.       
-0000ea50: 2020 2020 2022 2222 2929 0a20 2020 2020       """)).     
-0000ea60: 2020 2074 6162 6c65 2e70 7265 7365 6e74     table.present
-0000ea70: 2829 0a20 2020 2020 2020 206f 7574 203d  ().        out =
-0000ea80: 2053 7472 696e 6749 4f28 290a 2020 2020   StringIO().    
-0000ea90: 2020 2020 7461 626c 652e 7072 6573 656e      table.presen
-0000eaa0: 7428 6669 6c65 3d6f 7574 2c20 626f 783d  t(file=out, box=
-0000eab0: 626f 782e 4153 4349 4929 0a20 2020 2020  box.ASCII).     
-0000eac0: 2020 2065 7870 6563 7465 6420 3d20 7465     expected = te
-0000ead0: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
-0000eae0: 225c 0a20 2020 2020 2020 2020 2020 202b  "\.            +
-0000eaf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eb00: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2020  ----+.          
-0000eb10: 2020 7c20 4120 207c 2042 2020 207c 2044    | A  | B   | D
-0000eb20: 6566 6175 6c74 207c 0a20 2020 2020 2020  efault |.       
-0000eb30: 2020 2020 207c 2d2d 2d2d 2b2d 2d2d 2d2d       |----+-----
-0000eb40: 2b2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  +---------|.    
-0000eb50: 2020 2020 2020 2020 7c20 3130 207c 2031          | 10 | 1
-0000eb60: 3030 207c 2070 7572 706c 6520 207c 0a20  00 | purple  |. 
-0000eb70: 2020 2020 2020 2020 2020 207c 2031 3520             | 15 
-0000eb80: 7c20 3135 3020 7c20 2020 2020 2020 2020  | 150 |         
-0000eb90: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
-0000eba0: 3230 207c 2032 3030 207c 206f 7261 6e67  20 | 200 | orang
-0000ebb0: 6520 207c 0a20 2020 2020 2020 2020 2020  e  |.           
-0000ebc0: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
-0000ebd0: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-0000ebe0: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
-0000ebf0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000ec00: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000ec10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000ec20: 616c 2865 7870 6563 7465 642c 206f 7574  al(expected, out
-0000ec30: 2e67 6574 7661 6c75 6528 2929 0a0a 2020  .getvalue())..  
-0000ec40: 2020 2020 2020 2320 7465 7374 2067 726f        # test gro
-0000ec50: 7570 6279 0a20 2020 2020 2020 2074 6162  upby.        tab
-0000ec60: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-0000ec70: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000ec80: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000ec90: 2020 2020 2020 2020 2020 2020 612c 622c              a,b,
-0000eca0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-0000ecb0: 2020 2020 3130 2c31 3030 2c70 7572 706c      10,100,purpl
-0000ecc0: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
-0000ecd0: 2c31 3530 2c70 7572 706c 650a 2020 2020  ,150,purple.    
-0000ece0: 2020 2020 2020 2020 3230 2c32 3030 2c6f          20,200,o
-0000ecf0: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
-0000ed00: 2020 2222 2229 290a 2020 2020 2020 2020    """)).        
-0000ed10: 7461 626c 652e 7072 6573 656e 7428 290a  table.present().
-0000ed20: 2020 2020 2020 2020 7461 626c 652e 7072          table.pr
-0000ed30: 6573 656e 7428 626f 783d 626f 782e 4153  esent(box=box.AS
-0000ed40: 4349 492c 2067 726f 7570 6279 3d22 6465  CII, groupby="de
-0000ed50: 6661 756c 7422 290a 2020 2020 2020 2020  fault").        
-0000ed60: 6f75 7420 3d20 5374 7269 6e67 494f 2829  out = StringIO()
-0000ed70: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
-0000ed80: 7265 7365 6e74 2866 696c 653d 6f75 742c  resent(file=out,
-0000ed90: 2062 6f78 3d62 6f78 2e41 5343 4949 2c20   box=box.ASCII, 
-0000eda0: 6772 6f75 7062 793d 2264 6566 6175 6c74  groupby="default
-0000edb0: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
-0000edc0: 7465 6420 3d20 7465 7874 7772 6170 2e64  ted = textwrap.d
-0000edd0: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
-0000ede0: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-0000edf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ------------+.  
-0000ee00: 2020 2020 2020 2020 2020 7c20 4120 207c            | A  |
-0000ee10: 2042 2020 207c 2044 6566 6175 6c74 207c   B   | Default |
-0000ee20: 0a20 2020 2020 2020 2020 2020 207c 2d2d  .            |--
-0000ee30: 2d2d 2b2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --+-----+-------
-0000ee40: 2d2d 7c0a 2020 2020 2020 2020 2020 2020  --|.            
-0000ee50: 7c20 3130 207c 2031 3030 207c 2070 7572  | 10 | 100 | pur
-0000ee60: 706c 6520 207c 0a20 2020 2020 2020 2020  ple  |.         
-0000ee70: 2020 207c 2031 3520 7c20 3135 3020 7c20     | 15 | 150 | 
-0000ee80: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
-0000ee90: 2020 2020 2020 7c20 3230 207c 2032 3030        | 20 | 200
-0000eea0: 207c 206f 7261 6e67 6520 207c 0a20 2020   | orange  |.   
-0000eeb0: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
-0000eec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-0000eed0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000eee0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000eef0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000ef00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000ef10: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000ef20: 7465 642c 206f 7574 2e67 6574 7661 6c75  ted, out.getvalu
-0000ef30: 6528 2929 0a0a 2020 2020 2020 2020 7461  e())..        ta
-0000ef40: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
-0000ef50: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-0000ef60: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000ef70: 0a20 2020 2020 2020 2020 2020 2061 2c62  .            a,b
-0000ef80: 2c64 6566 6175 6c74 0a20 2020 2020 2020  ,default.       
-0000ef90: 2020 2020 2031 302c 3130 302c 7075 7270       10,100,purp
-0000efa0: 6c65 0a20 2020 2020 2020 2020 2020 2031  le.            1
-0000efb0: 352c 3135 302c 7075 7270 6c65 0a20 2020  5,150,purple.   
-0000efc0: 2020 2020 2020 2020 2031 352c 3230 302c           15,200,
-0000efd0: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
-0000efe0: 2020 2031 352c 3235 302c 6f72 616e 6765     15,250,orange
-0000eff0: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
-0000f000: 3235 302c 6f72 616e 6765 0a20 2020 2020  250,orange.     
-0000f010: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
-0000f020: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
-0000f030: 6e74 2829 0a20 2020 2020 2020 2074 6162  nt().        tab
-0000f040: 6c65 2e70 7265 7365 6e74 2862 6f78 3d62  le.present(box=b
-0000f050: 6f78 2e41 5343 4949 2c20 6772 6f75 7062  ox.ASCII, groupb
-0000f060: 793d 2264 6566 6175 6c74 2061 2229 0a20  y="default a"). 
-0000f070: 2020 2020 2020 206f 7574 203d 2053 7472         out = Str
-0000f080: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
-0000f090: 7461 626c 652e 7072 6573 656e 7428 6669  table.present(fi
-0000f0a0: 6c65 3d6f 7574 2c20 626f 783d 626f 782e  le=out, box=box.
-0000f0b0: 4153 4349 492c 2067 726f 7570 6279 3d22  ASCII, groupby="
-0000f0c0: 6465 6661 756c 7420 6122 290a 2020 2020  default a").    
-0000f0d0: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
-0000f0e0: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
-0000f0f0: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
-0000f100: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-0000f110: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2020  -----+.         
-0000f120: 2020 207c 2041 2020 7c20 4220 2020 7c20     | A  | B   | 
-0000f130: 4465 6661 756c 7420 7c0a 2020 2020 2020  Default |.      
-0000f140: 2020 2020 2020 7c2d 2d2d 2d2b 2d2d 2d2d        |----+----
-0000f150: 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -+---------|.   
-0000f160: 2020 2020 2020 2020 207c 2031 3020 7c20           | 10 | 
-0000f170: 3130 3020 7c20 7075 7270 6c65 2020 7c0a  100 | purple  |.
-0000f180: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
-0000f190: 207c 2031 3530 207c 2020 2020 2020 2020   | 150 |        
-0000f1a0: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
-0000f1b0: 2031 3520 7c20 3230 3020 7c20 6f72 616e   15 | 200 | oran
-0000f1c0: 6765 2020 7c0a 2020 2020 2020 2020 2020  ge  |.          
-0000f1d0: 2020 7c20 2020 207c 2032 3530 207c 2020    |    | 250 |  
-0000f1e0: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
-0000f1f0: 2020 2020 207c 2032 3020 7c20 3235 3020       | 20 | 250 
-0000f200: 7c20 2020 2020 2020 2020 7c0a 2020 2020  |         |.    
-0000f210: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
-0000f220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20  -------------+. 
-0000f230: 2020 2020 2020 2020 2020 2022 2222 290a             """).
-0000f240: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000f250: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000f260: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000f270: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000f280: 6564 2c20 6f75 742e 6765 7476 616c 7565  ed, out.getvalue
-0000f290: 2829 290a 0a20 2020 2020 2020 2074 6162  ())..        tab
-0000f2a0: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-0000f2b0: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000f2c0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000f2d0: 2020 2020 2020 2020 2020 2020 612c 622c              a,b,
-0000f2e0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-0000f2f0: 2020 2020 3130 2c31 3030 2c70 7572 706c      10,100,purpl
-0000f300: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
-0000f310: 2c32 3030 2c6f 7261 6e67 650a 2020 2020  ,200,orange.    
-0000f320: 2020 2020 2020 2020 3135 2c31 3530 2c70          15,150,p
-0000f330: 7572 706c 650a 2020 2020 2020 2020 2020  urple.          
-0000f340: 2020 3230 2c32 3530 2c6f 7261 6e67 650a    20,250,orange.
-0000f350: 2020 2020 2020 2020 2020 2020 3135 2c32              15,2
-0000f360: 3530 2c6f 7261 6e67 650a 2020 2020 2020  50,orange.      
-0000f370: 2020 2020 2020 2222 2229 290a 2020 2020        """)).    
-0000f380: 2020 2020 7461 626c 652e 736f 7274 2822      table.sort("
-0000f390: 6465 6661 756c 7420 6465 7363 2c61 2229  default desc,a")
-0000f3a0: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
-0000f3b0: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-0000f3c0: 2074 6162 6c65 2e70 7265 7365 6e74 2862   table.present(b
-0000f3d0: 6f78 3d62 6f78 2e41 5343 4949 2c20 6772  ox=box.ASCII, gr
-0000f3e0: 6f75 7062 793d 2264 6566 6175 6c74 2061  oupby="default a
-0000f3f0: 2229 0a20 2020 2020 2020 206f 7574 203d  ").        out =
-0000f400: 2053 7472 696e 6749 4f28 290a 2020 2020   StringIO().    
-0000f410: 2020 2020 7461 626c 652e 7072 6573 656e      table.presen
-0000f420: 7428 6669 6c65 3d6f 7574 2c20 626f 783d  t(file=out, box=
-0000f430: 626f 782e 4153 4349 492c 2067 726f 7570  box.ASCII, group
-0000f440: 6279 3d22 6465 6661 756c 7420 6122 290a  by="default a").
-0000f450: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0000f460: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-0000f470: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000f480: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d      +-----------
-0000f490: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
-0000f4a0: 2020 2020 2020 207c 2041 2020 7c20 4220         | A  | B 
-0000f4b0: 2020 7c20 4465 6661 756c 7420 7c0a 2020    | Default |.  
-0000f4c0: 2020 2020 2020 2020 2020 7c2d 2d2d 2d2b            |----+
-0000f4d0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c  -----+---------|
-0000f4e0: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000f4f0: 3020 7c20 3130 3020 7c20 7075 7270 6c65  0 | 100 | purple
-0000f500: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000f510: 7c20 3135 207c 2031 3530 207c 2020 2020  | 15 | 150 |    
-0000f520: 2020 2020 207c 0a20 2020 2020 2020 2020       |.         
-0000f530: 2020 207c 2031 3520 7c20 3230 3020 7c20     | 15 | 200 | 
-0000f540: 6f72 616e 6765 2020 7c0a 2020 2020 2020  orange  |.      
-0000f550: 2020 2020 2020 7c20 2020 207c 2032 3530        |    | 250
-0000f560: 207c 2020 2020 2020 2020 207c 0a20 2020   |         |.   
-0000f570: 2020 2020 2020 2020 207c 2032 3020 7c20           | 20 | 
-0000f580: 3235 3020 7c20 2020 2020 2020 2020 7c0a  250 |         |.
-0000f590: 2020 2020 2020 2020 2020 2020 2b2d 2d2d              +---
-0000f5a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f5b0: 2d2b 0a20 2020 2020 2020 2020 2020 2022  -+.            "
-0000f5c0: 2222 290a 2020 2020 2020 2020 7769 7468  "").        with
-0000f5d0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000f5e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f5f0: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000f600: 7065 6374 6564 2c20 6f75 742e 6765 7476  pected, out.getv
-0000f610: 616c 7565 2829 290a 0a20 2020 2064 6566  alue())..    def
-0000f620: 2074 6573 745f 6d61 726b 646f 776e 2873   test_markdown(s
-0000f630: 656c 6629 3a0a 2020 2020 2020 2020 7461  elf):.        ta
-0000f640: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
-0000f650: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-0000f660: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000f670: 0a20 2020 2020 2020 2020 2020 2061 2c62  .            a,b
-0000f680: 0a20 2020 2020 2020 2020 2020 2031 302c  .            10,
-0000f690: 3130 300a 2020 2020 2020 2020 2020 2020  100.            
-0000f6a0: 3230 2c32 3030 0a20 2020 2020 2020 2020  20,200.         
-0000f6b0: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
-0000f6c0: 206f 7574 5f6d 6172 6b64 6f77 6e20 3d20   out_markdown = 
-0000f6d0: 7461 626c 652e 6173 5f6d 6172 6b64 6f77  table.as_markdow
-0000f6e0: 6e28 290a 2020 2020 2020 2020 7072 696e  n().        prin
-0000f6f0: 7428 6f75 745f 6d61 726b 646f 776e 290a  t(out_markdown).
-0000f700: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0000f710: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-0000f720: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000f730: 2020 2020 7c20 6120 7c20 6220 7c0a 2020      | a | b |.  
-0000f740: 2020 2020 2020 2020 2020 7c2d 2d2d 7c2d            |---|-
-0000f750: 2d2d 7c0a 2020 2020 2020 2020 2020 2020  --|.            
-0000f760: 7c20 3130 207c 2031 3030 207c 0a20 2020  | 10 | 100 |.   
-0000f770: 2020 2020 2020 2020 207c 2032 3020 7c20           | 20 | 
-0000f780: 3230 3020 7c0a 2020 2020 2020 2020 2020  200 |.          
-0000f790: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
-0000f7a0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000f7b0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000f7c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000f7d0: 2865 7870 6563 7465 642c 206f 7574 5f6d  (expected, out_m
-0000f7e0: 6172 6b64 6f77 6e29 0a0a 2020 2020 2020  arkdown)..      
-0000f7f0: 2020 2320 7465 7374 2062 7567 6669 7820    # test bugfix 
-0000f800: 7768 656e 2074 6162 6c65 2068 6173 2061  when table has a
-0000f810: 7474 7269 6275 7465 2022 6465 6661 756c  ttribute "defaul
-0000f820: 7422 0a20 2020 2020 2020 2074 6162 6c65  t".        table
-0000f830: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-0000f840: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
-0000f850: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-0000f860: 2020 2020 2020 2020 2020 612c 622c 6465            a,b,de
-0000f870: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
-0000f880: 2020 3130 2c31 3030 2c70 7572 706c 650a    10,100,purple.
-0000f890: 2020 2020 2020 2020 2020 2020 3135 2c31              15,1
-0000f8a0: 3530 2c0a 2020 2020 2020 2020 2020 2020  50,.            
-0000f8b0: 3230 2c32 3030 2c6f 7261 6e67 650a 2020  20,200,orange.  
-0000f8c0: 2020 2020 2020 2020 2020 2222 2229 290a            """)).
-0000f8d0: 2020 2020 2020 2020 6f75 745f 6d61 726b          out_mark
-0000f8e0: 646f 776e 203d 2074 6162 6c65 2e61 735f  down = table.as_
-0000f8f0: 6d61 726b 646f 776e 2829 0a20 2020 2020  markdown().     
-0000f900: 2020 2070 7269 6e74 286f 7574 5f6d 6172     print(out_mar
-0000f910: 6b64 6f77 6e29 0a20 2020 2020 2020 2065  kdown).        e
-0000f920: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
-0000f930: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000f940: 2020 2020 2020 2020 2020 207c 2061 207c             | a |
-0000f950: 2062 207c 2064 6566 6175 6c74 207c 0a20   b | default |. 
-0000f960: 2020 2020 2020 2020 2020 207c 2d2d 2d7c             |---|
-0000f970: 2d2d 2d7c 2d2d 2d7c 0a20 2020 2020 2020  ---|---|.       
-0000f980: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
-0000f990: 7c20 7075 7270 6c65 207c 0a20 2020 2020  | purple |.     
-0000f9a0: 2020 2020 2020 207c 2031 3520 7c20 3135         | 15 | 15
-0000f9b0: 3020 7c20 207c 0a20 2020 2020 2020 2020  0 |  |.         
-0000f9c0: 2020 207c 2032 3020 7c20 3230 3020 7c20     | 20 | 200 | 
-0000f9d0: 6f72 616e 6765 207c 0a20 2020 2020 2020  orange |.       
-0000f9e0: 2020 2020 2022 2222 290a 2020 2020 2020       """).      
-0000f9f0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000fa00: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-0000fa10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000fa20: 7561 6c28 6578 7065 6374 6564 2c20 6f75  ual(expected, ou
-0000fa30: 745f 6d61 726b 646f 776e 290a 0a20 2020  t_markdown)..   
-0000fa40: 2020 2020 2023 2074 6573 7420 6772 6f75       # test grou
-0000fa50: 7069 6e67 2069 6e20 6173 5f6d 6172 6b64  ping in as_markd
-0000fa60: 6f77 6e0a 2020 2020 2020 2020 7461 626c  own.        tabl
-0000fa70: 6520 3d20 6c74 2e54 6162 6c65 2829 2e63  e = lt.Table().c
-0000fa80: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
-0000fa90: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000faa0: 2020 2020 2020 2020 2020 2061 2c62 2c64             a,b,d
-0000fab0: 6566 6175 6c74 0a20 2020 2020 2020 2020  efault.         
-0000fac0: 2020 2031 302c 3130 302c 7075 7270 6c65     10,100,purple
-0000fad0: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
-0000fae0: 3135 302c 7075 7270 6c65 0a20 2020 2020  150,purple.     
-0000faf0: 2020 2020 2020 2032 302c 3230 302c 6f72         20,200,or
-0000fb00: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
-0000fb10: 2022 2222 2929 0a20 2020 2020 2020 206f   """)).        o
-0000fb20: 7574 5f6d 6172 6b64 6f77 6e20 3d20 7461  ut_markdown = ta
-0000fb30: 626c 652e 6173 5f6d 6172 6b64 6f77 6e28  ble.as_markdown(
-0000fb40: 6772 6f75 7062 793d 2264 6566 6175 6c74  groupby="default
-0000fb50: 2229 0a20 2020 2020 2020 2070 7269 6e74  ").        print
-0000fb60: 286f 7574 5f6d 6172 6b64 6f77 6e29 0a20  (out_markdown). 
-0000fb70: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
-0000fb80: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
-0000fb90: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000fba0: 2020 207c 2061 207c 2062 207c 2064 6566     | a | b | def
-0000fbb0: 6175 6c74 207c 0a20 2020 2020 2020 2020  ault |.         
-0000fbc0: 2020 207c 2d2d 2d7c 2d2d 2d7c 2d2d 2d7c     |---|---|---|
-0000fbd0: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000fbe0: 3020 7c20 3130 3020 7c20 7075 7270 6c65  0 | 100 | purple
-0000fbf0: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
-0000fc00: 2031 3520 7c20 3135 3020 7c20 207c 0a20   15 | 150 |  |. 
-0000fc10: 2020 2020 2020 2020 2020 207c 2032 3020             | 20 
-0000fc20: 7c20 3230 3020 7c20 6f72 616e 6765 207c  | 200 | orange |
-0000fc30: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000fc40: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000fc50: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000fc60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fc70: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-0000fc80: 6374 6564 2c20 6f75 745f 6d61 726b 646f  cted, out_markdo
-0000fc90: 776e 290a 0a20 2020 2020 2020 2074 6162  wn)..        tab
-0000fca0: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-0000fcb0: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000fcc0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000fcd0: 2020 2020 2020 2020 2020 2020 612c 622c              a,b,
-0000fce0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-0000fcf0: 2020 2020 3130 2c31 3030 2c70 7572 706c      10,100,purpl
-0000fd00: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
-0000fd10: 2c32 3030 2c6f 7261 6e67 650a 2020 2020  ,200,orange.    
-0000fd20: 2020 2020 2020 2020 3135 2c31 3530 2c70          15,150,p
-0000fd30: 7572 706c 650a 2020 2020 2020 2020 2020  urple.          
-0000fd40: 2020 3230 2c32 3530 2c6f 7261 6e67 650a    20,250,orange.
-0000fd50: 2020 2020 2020 2020 2020 2020 3135 2c32              15,2
-0000fd60: 3530 2c6f 7261 6e67 650a 2020 2020 2020  50,orange.      
-0000fd70: 2020 2020 2020 2222 2229 290a 2020 2020        """)).    
-0000fd80: 2020 2020 7461 626c 652e 736f 7274 2822      table.sort("
-0000fd90: 6465 6661 756c 7420 6465 7363 2c61 2229  default desc,a")
-0000fda0: 0a20 2020 2020 2020 206f 7574 5f6d 6172  .        out_mar
-0000fdb0: 6b64 6f77 6e20 3d20 7461 626c 652e 6173  kdown = table.as
-0000fdc0: 5f6d 6172 6b64 6f77 6e28 6772 6f75 7062  _markdown(groupb
-0000fdd0: 793d 2264 6566 6175 6c74 2061 2229 0a20  y="default a"). 
-0000fde0: 2020 2020 2020 2070 7269 6e74 286f 7574         print(out
-0000fdf0: 5f6d 6172 6b64 6f77 6e29 0a20 2020 2020  _markdown).     
-0000fe00: 2020 2065 7870 6563 7465 6420 3d20 7465     expected = te
-0000fe10: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
-0000fe20: 225c 0a20 2020 2020 2020 2020 2020 207c  "\.            |
-0000fe30: 2061 207c 2062 207c 2064 6566 6175 6c74   a | b | default
-0000fe40: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
-0000fe50: 2d2d 2d7c 2d2d 2d7c 2d2d 2d7c 0a20 2020  ---|---|---|.   
-0000fe60: 2020 2020 2020 2020 207c 2031 3020 7c20           | 10 | 
-0000fe70: 3130 3020 7c20 7075 7270 6c65 207c 0a20  100 | purple |. 
-0000fe80: 2020 2020 2020 2020 2020 207c 2031 3520             | 15 
-0000fe90: 7c20 3135 3020 7c20 207c 0a20 2020 2020  | 150 |  |.     
-0000fea0: 2020 2020 2020 207c 2031 3520 7c20 3230         | 15 | 20
-0000feb0: 3020 7c20 6f72 616e 6765 207c 0a20 2020  0 | orange |.   
-0000fec0: 2020 2020 2020 2020 207c 2020 7c20 3235           |  | 25
-0000fed0: 3020 7c20 207c 0a20 2020 2020 2020 2020  0 |  |.         
-0000fee0: 2020 207c 2032 3020 7c20 3235 3020 7c20     | 20 | 250 | 
-0000fef0: 207c 0a20 2020 2020 2020 2020 2020 2022   |.            "
-0000ff00: 2222 290a 2020 2020 2020 2020 7769 7468  "").        with
-0000ff10: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000ff20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ff30: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000ff40: 7065 6374 6564 2c20 6f75 745f 6d61 726b  pected, out_mark
-0000ff50: 646f 776e 290a 0a23 2073 616d 706c 6520  down)..# sample 
-0000ff60: 696d 706f 7274 2064 6174 6120 7365 7473  import data sets
-0000ff70: 0a63 7376 5f64 6174 6120 3d20 2222 225c  .csv_data = """\
-0000ff80: 0a61 2c62 2c63 0a30 2c30 2c30 0a30 2c30  .a,b,c.0,0,0.0,0
-0000ff90: 2c31 0a30 2c30 2c32 0a30 2c31 2c30 0a30  ,1.0,0,2.0,1,0.0
-0000ffa0: 2c31 2c31 0a30 2c31 2c32 0a30 2c32 2c30  ,1,1.0,1,2.0,2,0
-0000ffb0: 0a30 2c32 2c31 0a30 2c32 2c32 0a31 2c30  .0,2,1.0,2,2.1,0
-0000ffc0: 2c30 0a31 2c30 2c31 0a31 2c30 2c32 0a31  ,0.1,0,1.1,0,2.1
-0000ffd0: 2c31 2c30 0a31 2c31 2c31 0a31 2c31 2c32  ,1,0.1,1,1.1,1,2
-0000ffe0: 0a31 2c32 2c30 0a31 2c32 2c31 0a31 2c32  .1,2,0.1,2,1.1,2
-0000fff0: 2c32 0a32 2c30 2c30 0a32 2c30 2c31 0a32  ,2.2,0,0.2,0,1.2
-00010000: 2c30 2c32 0a32 2c31 2c30 0a32 2c31 2c31  ,0,2.2,1,0.2,1,1
-00010010: 0a32 2c31 2c32 0a32 2c32 2c30 0a32 2c32  .2,1,2.2,2,0.2,2
-00010020: 2c31 0a32 2c32 2c32 0a0a 2222 220a 0a6a  ,1.2,2,2.."""..j
-00010030: 736f 6e5f 6461 7461 203d 2022 2222 5c0a  son_data = """\.
-00010040: 2020 2020 7b22 6122 3a20 302c 2022 6222      {"a": 0, "b"
-00010050: 3a20 302c 2022 6322 3a20 307d 0a20 2020  : 0, "c": 0}.   
-00010060: 207b 2261 223a 2030 2c20 2262 223a 2030   {"a": 0, "b": 0
-00010070: 2c20 2263 223a 2031 7d0a 2020 2020 7b22  , "c": 1}.    {"
-00010080: 6122 3a20 302c 2022 6222 3a20 302c 2022  a": 0, "b": 0, "
-00010090: 6322 3a20 327d 0a20 2020 207b 2261 223a  c": 2}.    {"a":
-000100a0: 2030 2c20 2262 223a 2031 2c20 2263 223a   0, "b": 1, "c":
-000100b0: 2030 7d0a 2020 2020 7b22 6122 3a20 302c   0}.    {"a": 0,
-000100c0: 2022 6222 3a20 312c 2022 6322 3a20 317d   "b": 1, "c": 1}
-000100d0: 0a20 2020 207b 2261 223a 2030 2c20 2262  .    {"a": 0, "b
-000100e0: 223a 2031 2c20 2263 223a 2032 7d0a 2020  ": 1, "c": 2}.  
-000100f0: 2020 7b22 6122 3a20 302c 2022 6222 3a20    {"a": 0, "b": 
-00010100: 322c 2022 6322 3a20 307d 0a20 2020 207b  2, "c": 0}.    {
-00010110: 2261 223a 2030 2c20 2262 223a 2032 2c20  "a": 0, "b": 2, 
-00010120: 2263 223a 2031 7d0a 2020 2020 7b22 6122  "c": 1}.    {"a"
-00010130: 3a20 302c 2022 6222 3a20 322c 2022 6322  : 0, "b": 2, "c"
-00010140: 3a20 327d 0a20 2020 207b 2261 223a 2031  : 2}.    {"a": 1
-00010150: 2c20 2262 223a 2030 2c20 2263 223a 2030  , "b": 0, "c": 0
-00010160: 7d0a 2020 2020 7b22 6122 3a20 312c 2022  }.    {"a": 1, "
-00010170: 6222 3a20 302c 2022 6322 3a20 317d 0a20  b": 0, "c": 1}. 
-00010180: 2020 207b 2261 223a 2031 2c20 2262 223a     {"a": 1, "b":
-00010190: 2030 2c20 2263 223a 2032 7d0a 2020 2020   0, "c": 2}.    
-000101a0: 7b22 6122 3a20 312c 2022 6222 3a20 312c  {"a": 1, "b": 1,
-000101b0: 2022 6322 3a20 307d 0a20 2020 207b 2261   "c": 0}.    {"a
-000101c0: 223a 2031 2c20 2262 223a 2031 2c20 2263  ": 1, "b": 1, "c
-000101d0: 223a 2031 7d0a 2020 2020 7b22 6122 3a20  ": 1}.    {"a": 
-000101e0: 312c 2022 6222 3a20 312c 2022 6322 3a20  1, "b": 1, "c": 
-000101f0: 327d 0a20 2020 207b 2261 223a 2031 2c20  2}.    {"a": 1, 
-00010200: 2262 223a 2032 2c20 2263 223a 2030 7d0a  "b": 2, "c": 0}.
-00010210: 2020 2020 7b22 6122 3a20 312c 2022 6222      {"a": 1, "b"
-00010220: 3a20 322c 2022 6322 3a20 317d 0a20 2020  : 2, "c": 1}.   
-00010230: 207b 2261 223a 2031 2c20 2262 223a 2032   {"a": 1, "b": 2
-00010240: 2c20 2263 223a 2032 7d0a 2020 2020 7b22  , "c": 2}.    {"
-00010250: 6122 3a20 322c 2022 6222 3a20 302c 2022  a": 2, "b": 0, "
-00010260: 6322 3a20 307d 0a20 2020 207b 2261 223a  c": 0}.    {"a":
-00010270: 2032 2c20 2262 223a 2030 2c20 2263 223a   2, "b": 0, "c":
-00010280: 2031 7d0a 2020 2020 7b22 6122 3a20 322c   1}.    {"a": 2,
-00010290: 2022 6222 3a20 302c 2022 6322 3a20 327d   "b": 0, "c": 2}
-000102a0: 0a20 2020 207b 2261 223a 2032 2c20 2262  .    {"a": 2, "b
-000102b0: 223a 2031 2c20 2263 223a 2030 7d0a 2020  ": 1, "c": 0}.  
-000102c0: 2020 7b22 6122 3a20 322c 2022 6222 3a20    {"a": 2, "b": 
-000102d0: 312c 2022 6322 3a20 317d 0a20 2020 207b  1, "c": 1}.    {
-000102e0: 2261 223a 2032 2c20 2262 223a 2031 2c20  "a": 2, "b": 1, 
-000102f0: 2263 223a 2032 7d0a 2020 2020 7b22 6122  "c": 2}.    {"a"
-00010300: 3a20 322c 2022 6222 3a20 322c 2022 6322  : 2, "b": 2, "c"
-00010310: 3a20 307d 0a20 2020 207b 2261 223a 2032  : 0}.    {"a": 2
-00010320: 2c20 2262 223a 2032 2c20 2263 223a 2031  , "b": 2, "c": 1
-00010330: 7d0a 2020 2020 7b22 6122 3a20 322c 2022  }.    {"a": 2, "
-00010340: 6222 3a20 322c 2022 6322 3a20 327d 0a0a  b": 2, "c": 2}..
-00010350: 2222 220a 0a66 6978 6564 5f77 6964 7468  """..fixed_width
-00010360: 5f64 6174 6120 3d20 2222 225c 0a30 2030  _data = """\.0 0
-00010370: 2030 0a30 2030 2031 0a30 2030 2032 0a30   0.0 0 1.0 0 2.0
-00010380: 2031 2030 0a30 2031 2031 0a30 2031 2032   1 0.0 1 1.0 1 2
-00010390: 0a30 2032 2030 0a30 2032 2031 0a30 2032  .0 2 0.0 2 1.0 2
-000103a0: 2032 0a31 2030 2030 0a31 2030 2031 0a31   2.1 0 0.1 0 1.1
-000103b0: 2030 2032 0a31 2031 2030 0a31 2031 2031   0 2.1 1 0.1 1 1
-000103c0: 0a31 2031 2032 0a31 2032 2030 0a31 2032  .1 1 2.1 2 0.1 2
-000103d0: 2031 0a31 2032 2032 0a32 2030 2030 0a32   1.1 2 2.2 0 0.2
-000103e0: 2030 2031 0a32 2030 2032 0a32 2031 2030   0 1.2 0 2.2 1 0
-000103f0: 0a32 2031 2031 0a32 2031 2032 0a32 2032  .2 1 1.2 1 2.2 2
-00010400: 2030 0a32 2032 2031 0a32 2032 2032 0a0a   0.2 2 1.2 2 2..
-00010410: 2222 220a 0a0a 406d 616b 655f 7465 7374  """...@make_test
-00010420: 5f63 6c61 7373 6573 0a63 6c61 7373 2054  _classes.class T
-00010430: 6162 6c65 496d 706f 7274 4578 706f 7274  ableImportExport
-00010440: 5465 7374 733a 0a20 2020 2022 2222 0a20  Tests:.    """. 
-00010450: 2020 2054 6573 7420 636c 6173 7365 7320     Test classes 
-00010460: 666f 7220 5461 626c 6520 696d 706f 7274  for Table import
-00010470: 2061 6e64 2065 7870 6f72 7420 6d65 7468   and export meth
-00010480: 6f64 732e 0a20 2020 2022 2222 0a20 2020  ods..    """.   
-00010490: 2064 6566 2074 6573 745f 6173 5f64 6174   def test_as_dat
-000104a0: 6166 7261 6d65 2873 656c 6629 3a0a 2020  aframe(self):.  
-000104b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000104c0: 2020 2020 2020 2069 6d70 6f72 7420 7061         import pa
-000104d0: 6e64 6173 2061 7320 7064 0a20 2020 2020  ndas as pd.     
-000104e0: 2020 2065 7863 6570 7420 496d 706f 7274     except Import
-000104f0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00010500: 2020 2070 7269 6e74 2822 7061 6e64 6173     print("pandas
-00010510: 206e 6f74 2069 6e73 7461 6c6c 6564 2c20   not installed, 
-00010520: 736b 6970 7069 6e67 2074 6573 7422 290a  skipping test").
-00010530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010540: 726e 0a0a 2020 2020 2020 2020 696d 706f  rn..        impo
-00010550: 7274 206a 736f 6e0a 0a20 2020 2020 2020  rt json..       
-00010560: 2074 6573 745f 7369 7a65 203d 2033 0a20   test_size = 3. 
-00010570: 2020 2020 2020 2074 3120 3d20 6d61 6b65         t1 = make
-00010580: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
-00010590: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-000105a0: 742c 2074 6573 745f 7369 7a65 290a 0a20  t, test_size).. 
-000105b0: 2020 2020 2020 2064 663a 2070 642e 4461         df: pd.Da
-000105c0: 7461 4672 616d 6520 3d20 7431 2e61 735f  taFrame = t1.as_
-000105d0: 6461 7461 6672 616d 6528 222d 6222 290a  dataframe("-b").
-000105e0: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
-000105f0: 2063 6f6c 756d 6e20 6e61 6d65 730a 2020   column names.  
-00010600: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010610: 7445 7175 616c 285b 2261 222c 2022 6322  tEqual(["a", "c"
-00010620: 5d2c 206c 6973 7428 6466 2e63 6f6c 756d  ], list(df.colum
-00010630: 6e73 2929 0a0a 2020 2020 2020 2020 2320  ns))..        # 
-00010640: 6368 6563 6b20 696d 706f 7274 6564 2076  check imported v
-00010650: 616c 7565 730a 2020 2020 2020 2020 6672  alues.        fr
-00010660: 6f6d 5f64 6620 3d20 6466 2e74 6f5f 6a73  om_df = df.to_js
-00010670: 6f6e 286f 7269 656e 743d 2276 616c 7565  on(orient="value
-00010680: 7322 290a 2020 2020 2020 2020 6578 7065  s").        expe
-00010690: 6374 6564 203d 205b 0a20 2020 2020 2020  cted = [.       
-000106a0: 2020 2020 205b 7265 632e 612c 2072 6563       [rec.a, rec
-000106b0: 2e63 5d20 666f 7220 7265 6320 696e 2074  .c] for rec in t
-000106c0: 310a 2020 2020 2020 2020 5d0a 2020 2020  1.        ].    
-000106d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000106e0: 7175 616c 2865 7870 6563 7465 642c 206a  qual(expected, j
-000106f0: 736f 6e2e 6c6f 6164 7328 6672 6f6d 5f64  son.loads(from_d
-00010700: 6629 290a 0a20 2020 2064 6566 2074 6573  f))..    def tes
-00010710: 745f 6373 765f 6578 706f 7274 2873 656c  t_csv_export(sel
-00010720: 6629 3a0a 2020 2020 2020 2020 6672 6f6d  f):.        from
-00010730: 2069 7465 7274 6f6f 6c73 2069 6d70 6f72   itertools impor
-00010740: 7420 7065 726d 7574 6174 696f 6e73 0a20  t permutations. 
-00010750: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
-00010760: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
-00010770: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-00010780: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00010790: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-000107a0: 7a65 290a 2020 2020 2020 2020 666f 7220  ze).        for 
-000107b0: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
-000107c0: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
-000107d0: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
-000107e0: 2020 2020 206f 7574 203d 2069 6f2e 5374       out = io.St
-000107f0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-00010800: 2020 2020 2074 312e 6373 765f 6578 706f       t1.csv_expo
-00010810: 7274 286f 7574 2c20 6669 656c 646e 616d  rt(out, fieldnam
-00010820: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00010830: 6f75 742e 7365 656b 2830 290a 2020 2020  out.seek(0).    
-00010840: 2020 2020 2020 2020 6f75 746c 696e 6573          outlines
-00010850: 203d 206f 7574 2e72 6561 6428 292e 7370   = out.read().sp
-00010860: 6c69 746c 696e 6573 2829 0a20 2020 2020  litlines().     
-00010870: 2020 2020 2020 206f 7574 2e63 6c6f 7365         out.close
-00010880: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
-00010890: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-000108a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000108b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000108c0: 7175 616c 2827 2c27 2e6a 6f69 6e28 6669  qual(','.join(fi
-000108d0: 656c 646e 616d 6573 292c 206f 7574 6c69  eldnames), outli
-000108e0: 6e65 735b 305d 290a 2020 2020 2020 2020  nes[0]).        
-000108f0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00010900: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-00010910: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00010920: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00010930: 697a 652a 2a33 2b31 2c20 6c65 6e28 6f75  ize**3+1, len(ou
-00010940: 746c 696e 6573 2929 0a20 2020 2020 2020  tlines)).       
-00010950: 2020 2020 2066 6f72 206f 622c 206c 696e       for ob, lin
-00010960: 6520 696e 207a 6970 2874 312c 206f 7574  e in zip(t1, out
-00010970: 6c69 6e65 735b 313a 5d29 3a0a 2020 2020  lines[1:]):.    
-00010980: 2020 2020 2020 2020 2020 2020 6373 765f              csv_
-00010990: 7661 6c73 203d 206c 696e 652e 7370 6c69  vals = line.spli
-000109a0: 7428 272c 2729 0a20 2020 2020 2020 2020  t(',').         
-000109b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-000109c0: 2e73 7562 5465 7374 286f 623d 6f62 2c20  .subTest(ob=ob, 
-000109d0: 6373 765f 7661 6c73 3d63 7376 5f76 616c  csv_vals=csv_val
-000109e0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000109f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010a00: 6572 7454 7275 6528 616c 6c28 0a20 2020  ertTrue(all(.   
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2069 6e74 2863 7376 5f76 616c       int(csv_val
-00010a30: 735b 695d 2920 3d3d 2067 6574 6174 7472  s[i]) == getattr
-00010a40: 286f 622c 2066 6c64 2920 666f 7220 692c  (ob, fld) for i,
-00010a50: 2066 6c64 2069 6e20 656e 756d 6572 6174   fld in enumerat
-00010a60: 6528 6669 656c 646e 616d 6573 290a 2020  e(fieldnames).  
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2929 0a0a 2020 2020 2020 2020 2320    ))..        # 
-00010a90: 7265 7275 6e20 7573 696e 6720 616e 2065  rerun using an e
-00010aa0: 6d70 7479 2074 6162 6c65 0a20 2020 2020  mpty table.     
-00010ab0: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
-00010ac0: 2829 0a20 2020 2020 2020 2066 6f72 2066  ().        for f
-00010ad0: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
-00010ae0: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
-00010af0: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
-00010b00: 2020 2020 6f75 7420 3d20 696f 2e53 7472      out = io.Str
-00010b10: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
-00010b20: 2020 2020 7431 2e63 7376 5f65 7870 6f72      t1.csv_expor
-00010b30: 7428 6f75 742c 2066 6965 6c64 6e61 6d65  t(out, fieldname
-00010b40: 7329 0a20 2020 2020 2020 2020 2020 206f  s).            o
-00010b50: 7574 2e73 6565 6b28 3029 0a20 2020 2020  ut.seek(0).     
-00010b60: 2020 2020 2020 206f 7574 6c69 6e65 7320         outlines 
-00010b70: 3d20 6f75 742e 7265 6164 2829 2e73 706c  = out.read().spl
-00010b80: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
-00010b90: 2020 2020 2020 6f75 742e 636c 6f73 6528        out.close(
-00010ba0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-00010bb0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00010bc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010bd0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00010be0: 7561 6c28 272c 272e 6a6f 696e 2866 6965  ual(','.join(fie
-00010bf0: 6c64 6e61 6d65 7329 2c20 6f75 746c 696e  ldnames), outlin
-00010c00: 6573 5b30 5d29 0a20 2020 2020 2020 2020  es[0]).         
-00010c10: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00010c20: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00010c30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010c40: 6572 7445 7175 616c 2831 2c20 6c65 6e28  ertEqual(1, len(
-00010c50: 6f75 746c 696e 6573 2929 0a0a 2020 2020  outlines))..    
-00010c60: 2020 2020 2320 7265 7275 6e20 7573 696e      # rerun usin
-00010c70: 6720 616e 2065 6d70 7479 2074 6162 6c65  g an empty table
-00010c80: 2c20 7769 7468 2069 6e64 6578 6573 2074  , with indexes t
-00010c90: 6f20 6469 6374 6174 6520 6669 656c 646e  o dictate fieldn
-00010ca0: 616d 6573 0a20 2020 2020 2020 2066 6f72  ames.        for
-00010cb0: 2066 6965 6c64 6e61 6d65 7320 696e 2070   fieldnames in p
-00010cc0: 6572 6d75 7461 7469 6f6e 7328 6c69 7374  ermutations(list
-00010cd0: 2827 6162 6327 2929 3a0a 2020 2020 2020  ('abc')):.      
-00010ce0: 2020 2020 2020 7431 203d 206c 742e 5461        t1 = lt.Ta
-00010cf0: 626c 6528 290a 2020 2020 2020 2020 2020  ble().          
-00010d00: 2020 666f 7220 666c 6420 696e 2066 6965    for fld in fie
-00010d10: 6c64 6e61 6d65 733a 0a20 2020 2020 2020  ldnames:.       
-00010d20: 2020 2020 2020 2020 2074 312e 6372 6561           t1.crea
-00010d30: 7465 5f69 6e64 6578 2866 6c64 290a 2020  te_index(fld).  
-00010d40: 2020 2020 2020 2020 2020 6f75 7420 3d20            out = 
-00010d50: 696f 2e53 7472 696e 6749 4f28 290a 2020  io.StringIO().  
-00010d60: 2020 2020 2020 2020 2020 7431 2e63 7376            t1.csv
-00010d70: 5f65 7870 6f72 7428 6f75 7429 0a20 2020  _export(out).   
-00010d80: 2020 2020 2020 2020 206f 7574 2e73 6565           out.see
-00010d90: 6b28 3029 0a20 2020 2020 2020 2020 2020  k(0).           
-00010da0: 206f 7574 6c69 6e65 7320 3d20 6f75 742e   outlines = out.
-00010db0: 7265 6164 2829 2e73 706c 6974 6c69 6e65  read().splitline
-00010dc0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00010dd0: 6f75 742e 636c 6f73 6528 290a 2020 2020  out.close().    
-00010de0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010df0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00010e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010e10: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
-00010e20: 7428 6669 656c 646e 616d 6573 292c 2073  t(fieldnames), s
-00010e30: 6574 286f 7574 6c69 6e65 735b 305d 2e73  et(outlines[0].s
-00010e40: 706c 6974 2827 2c27 2929 290a 2020 2020  plit(','))).    
-00010e50: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010e60: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00010e70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010e80: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
-00010e90: 206c 656e 286f 7574 6c69 6e65 7329 290a   len(outlines)).
-00010ea0: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
-00010eb0: 765f 6578 706f 7274 5f74 6f5f 7374 7269  v_export_to_stri
-00010ec0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
-00010ed0: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
-00010ee0: 2069 6d70 6f72 7420 7065 726d 7574 6174   import permutat
-00010ef0: 696f 6e73 0a20 2020 2020 2020 2074 6573  ions.        tes
-00010f00: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
-00010f10: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
-00010f20: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00010f30: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00010f40: 6573 745f 7369 7a65 290a 2020 2020 2020  est_size).      
-00010f50: 2020 666f 7220 6669 656c 646e 616d 6573    for fieldnames
-00010f60: 2069 6e20 7065 726d 7574 6174 696f 6e73   in permutations
-00010f70: 286c 6973 7428 2761 6263 2729 293a 0a20  (list('abc')):. 
-00010f80: 2020 2020 2020 2020 2020 206f 7574 5f73             out_s
-00010f90: 7472 696e 6720 3d20 7431 2e63 7376 5f65  tring = t1.csv_e
-00010fa0: 7870 6f72 7428 4e6f 6e65 2c20 6669 656c  xport(None, fiel
-00010fb0: 646e 616d 6573 290a 2020 2020 2020 2020  dnames).        
-00010fc0: 2020 2020 6f75 746c 696e 6573 203d 206f      outlines = o
-00010fd0: 7574 5f73 7472 696e 672e 7370 6c69 746c  ut_string.splitl
-00010fe0: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
-00010ff0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00011000: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00011010: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00011020: 6572 7445 7175 616c 2827 2c27 2e6a 6f69  ertEqual(','.joi
-00011030: 6e28 6669 656c 646e 616d 6573 292c 206f  n(fieldnames), o
-00011040: 7574 6c69 6e65 735b 305d 290a 2020 2020  utlines[0]).    
-00011050: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00011060: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00011070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011080: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00011090: 7374 5f73 697a 6520 2a2a 2033 202b 2031  st_size ** 3 + 1
-000110a0: 2c20 6c65 6e28 6f75 746c 696e 6573 2929  , len(outlines))
-000110b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000110c0: 206f 622c 206c 696e 6520 696e 207a 6970   ob, line in zip
-000110d0: 2874 312c 206f 7574 6c69 6e65 735b 313a  (t1, outlines[1:
-000110e0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-000110f0: 2020 2020 6373 765f 7661 6c73 203d 206c      csv_vals = l
-00011100: 696e 652e 7370 6c69 7428 272c 2729 0a20  ine.split(','). 
-00011110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00011120: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00011130: 286f 623d 6f62 2c20 6373 765f 7661 6c73  (ob=ob, csv_vals
-00011140: 3d63 7376 5f76 616c 7329 3a0a 2020 2020  =csv_vals):.    
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00011170: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
-00011180: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-00011190: 2863 7376 5f76 616c 735b 695d 2920 3d3d  (csv_vals[i]) ==
-000111a0: 2067 6574 6174 7472 286f 622c 2066 6c64   getattr(ob, fld
-000111b0: 2920 666f 7220 692c 2066 6c64 2069 6e20  ) for i, fld in 
-000111c0: 656e 756d 6572 6174 6528 6669 656c 646e  enumerate(fieldn
-000111d0: 616d 6573 290a 2020 2020 2020 2020 2020  ames).          
-000111e0: 2020 2020 2020 2020 2020 2929 0a0a 2020            ))..  
-000111f0: 2020 6465 6620 7465 7374 5f63 7376 5f69    def test_csv_i
-00011200: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
-00011210: 2020 2020 2064 6174 6120 3d20 6373 765f       data = csv_
-00011220: 6461 7461 0a20 2020 2020 2020 2069 6e63  data.        inc
-00011230: 7376 203d 2069 6f2e 5374 7269 6e67 494f  sv = io.StringIO
-00011240: 2864 6174 6129 0a20 2020 2020 2020 2063  (data).        c
-00011250: 7376 7461 626c 6520 3d20 6c74 2e54 6162  svtable = lt.Tab
-00011260: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00011270: 696e 6373 762c 2074 7261 6e73 666f 726d  incsv, transform
-00011280: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
-00011290: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
-000112a0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
-000112b0: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
-000112c0: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
-000112d0: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
-000112e0: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
-000112f0: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-00011300: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00011310: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00011320: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00011330: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
-00011340: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
-00011350: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
-00011360: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
-00011370: 7028 7431 2c20 6373 7674 6162 6c65 2929  p(t1, csvtable))
-00011380: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00011390: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-000113a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000113b0: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
-000113c0: 3120 666f 7220 6c69 6e65 2069 6e20 6461  1 for line in da
-000113d0: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
-000113e0: 6966 206c 696e 652e 7374 7269 7028 2929  if line.strip())
-000113f0: 2d31 2c20 6c65 6e28 6373 7674 6162 6c65  -1, len(csvtable
-00011400: 2929 0a0a 2020 2020 2020 2020 696e 6373  ))..        incs
-00011410: 7620 3d20 696f 2e53 7472 696e 6749 4f28  v = io.StringIO(
-00011420: 6461 7461 290a 2020 2020 2020 2020 726f  data).        ro
-00011430: 775f 7072 6f74 6f74 7970 6520 3d20 7365  w_prototype = se
-00011440: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00011450: 6563 7428 302c 2030 2c20 3029 0a20 2020  ect(0, 0, 0).   
-00011460: 2020 2020 2063 7376 7461 626c 6532 203d       csvtable2 =
-00011470: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00011480: 696d 706f 7274 2869 6e63 7376 2c20 7472  import(incsv, tr
-00011490: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
-000114a0: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
-000114b0: 273a 2069 6e74 7d2c 2072 6f77 5f63 6c61  ': int}, row_cla
-000114c0: 7373 3d74 7970 6528 726f 775f 7072 6f74  ss=type(row_prot
-000114d0: 6f74 7970 6529 295b 3a33 5d0a 0a20 2020  otype))[:3]..   
-000114e0: 2020 2020 2070 7269 6e74 2874 7970 6528       print(type(
-000114f0: 7431 5b30 5d29 2e5f 5f6e 616d 655f 5f2c  t1[0]).__name__,
-00011500: 2074 315b 305d 290a 2020 2020 2020 2020   t1[0]).        
-00011510: 7072 696e 7428 7479 7065 2863 7376 7461  print(type(csvta
-00011520: 626c 6532 5b30 5d29 2e5f 5f6e 616d 655f  ble2[0]).__name_
-00011530: 5f2c 2063 7376 7461 626c 6532 5b30 5d29  _, csvtable2[0])
-00011540: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00011550: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00011560: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00011570: 7373 6572 7445 7175 616c 2874 7970 6528  ssertEqual(type(
-00011580: 7431 5b30 5d29 2c20 7479 7065 2863 7376  t1[0]), type(csv
-00011590: 7461 626c 6532 5b30 5d29 290a 0a20 2020  table2[0]))..   
-000115a0: 2064 6566 2074 6573 745f 6373 765f 636f   def test_csv_co
-000115b0: 6d70 7265 7373 6564 5f69 6d70 6f72 7428  mpressed_import(
-000115c0: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
-000115d0: 6465 6620 7665 7269 6679 5f74 696d 6573  def verify_times
-000115e0: 7461 6d70 7328 7431 2c20 7432 2c20 696e  tamps(t1, t2, in
-000115f0: 666f 5f64 6963 7429 3a0a 2020 2020 2020  fo_dict):.      
-00011600: 2020 2020 2020 666f 7220 7469 6d65 7374        for timest
-00011610: 616d 705f 6174 7472 5f6e 616d 6520 696e  amp_attr_name in
-00011620: 2022 6372 6561 7465 6420 6d6f 6469 6669   "created modifi
-00011630: 6564 206c 6173 745f 696d 706f 7274 222e  ed last_import".
-00011640: 7370 6c69 7428 293a 0a20 2020 2020 2020  split():.       
-00011650: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
-00011660: 6d70 5f76 616c 7565 203d 2069 6e66 6f5f  mp_value = info_
-00011670: 6469 6374 2e70 6f70 2874 696d 6573 7461  dict.pop(timesta
-00011680: 6d70 5f61 7474 725f 6e61 6d65 290a 2020  mp_attr_name).  
-00011690: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-000116a0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-000116b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000116c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000116d0: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 7431 203c 3d20 7469 6d65 7374 616d 705f  t1 <= timestamp_
-00011700: 7661 6c75 6520 3c3d 2074 322c 0a20 2020  value <= t2,.   
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2066 2269 6e63 6f72 7265 6374       f"incorrect
-00011730: 207b 7469 6d65 7374 616d 705f 6174 7472   {timestamp_attr
-00011740: 5f6e 616d 657d 2074 696d 6522 0a20 2020  _name} time".   
-00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011760: 2029 0a0a 2020 2020 2020 2020 7769 7468   )..        with
-00011770: 2074 696d 6573 7461 6d70 5f73 7461 7274   timestamp_start
-00011780: 5f65 6e64 2829 2061 7320 7469 6d69 6e67  _end() as timing
-00011790: 3a0a 2020 2020 2020 2020 2020 2020 7474  :.            tt
-000117a0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-000117b0: 765f 696d 706f 7274 2822 7465 7374 2f61  v_import("test/a
-000117c0: 6263 2e63 7376 222c 2074 7261 6e73 666f  bc.csv", transfo
-000117d0: 726d 733d 6469 6374 2e66 726f 6d6b 6579  rms=dict.fromkey
-000117e0: 7328 2261 6263 222c 2069 6e74 2929 0a0a  s("abc", int))..
-000117f0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00011800: 5f69 6e66 6f5f 6261 7365 203d 2074 742e  _info_base = tt.
-00011810: 696e 666f 2829 0a20 2020 2020 2020 2076  info().        v
-00011820: 6572 6966 795f 7469 6d65 7374 616d 7073  erify_timestamps
-00011830: 2874 696d 696e 672e 7374 6172 742c 2074  (timing.start, t
-00011840: 696d 696e 672e 656e 642c 2065 7870 6563  iming.end, expec
-00011850: 7465 645f 696e 666f 5f62 6173 6529 0a0a  ted_info_base)..
-00011860: 2020 2020 2020 2020 7072 696e 7428 2261          print("a
-00011870: 6263 2e63 7376 222c 2065 7870 6563 7465  bc.csv", expecte
-00011880: 645f 696e 666f 5f62 6173 6529 0a0a 2020  d_info_base)..  
-00011890: 2020 2020 2020 636f 6d70 7265 7373 6564        compressed
-000118a0: 5f66 696c 6573 203d 205b 0a20 2020 2020  _files = [.     
-000118b0: 2020 2020 2020 2022 6162 632e 6373 762e         "abc.csv.
-000118c0: 7a69 7022 2c0a 2020 2020 2020 2020 2020  zip",.          
-000118d0: 2020 2261 6263 2e63 7376 2e67 7a22 2c0a    "abc.csv.gz",.
-000118e0: 2020 2020 2020 2020 2020 2020 2261 6263              "abc
-000118f0: 2e63 7376 2e78 7a22 2c0a 2020 2020 2020  .csv.xz",.      
-00011900: 2020 5d0a 2020 2020 2020 2020 666f 7220    ].        for 
-00011910: 6e61 6d65 2069 6e20 636f 6d70 7265 7373  name in compress
-00011920: 6564 5f66 696c 6573 3a0a 2020 2020 2020  ed_files:.      
-00011930: 2020 2020 2020 696d 706f 7274 5f73 6f75        import_sou
-00011940: 7263 655f 6e61 6d65 203d 2022 7465 7374  rce_name = "test
-00011950: 2f22 202b 206e 616d 650a 2020 2020 2020  /" + name.      
-00011960: 2020 2020 2020 7769 7468 2074 696d 6573        with times
-00011970: 7461 6d70 5f73 7461 7274 5f65 6e64 2829  tamp_start_end()
-00011980: 2061 7320 7469 6d69 6e67 3a0a 2020 2020   as timing:.    
-00011990: 2020 2020 2020 2020 2020 2020 7474 3220              tt2 
-000119a0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-000119b0: 5f69 6d70 6f72 7428 696d 706f 7274 5f73  _import(import_s
-000119c0: 6f75 7263 655f 6e61 6d65 2c20 7472 616e  ource_name, tran
-000119d0: 7366 6f72 6d73 3d64 6963 742e 6672 6f6d  sforms=dict.from
-000119e0: 6b65 7973 2822 6162 6322 2c20 696e 7429  keys("abc", int)
-000119f0: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00011a00: 7432 5f69 6e66 6f20 3d20 7474 322e 696e  t2_info = tt2.in
-00011a10: 666f 2829 0a20 2020 2020 2020 2020 2020  fo().           
-00011a20: 2070 7269 6e74 286e 616d 652c 2074 7432   print(name, tt2
-00011a30: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
-00011a40: 2020 2020 7665 7269 6679 5f74 696d 6573      verify_times
-00011a50: 7461 6d70 7328 7469 6d69 6e67 2e73 7461  tamps(timing.sta
-00011a60: 7274 2c20 7469 6d69 6e67 2e65 6e64 2c20  rt, timing.end, 
-00011a70: 7474 325f 696e 666f 290a 0a20 2020 2020  tt2_info)..     
-00011a80: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
-00011a90: 696e 666f 203d 207b 2a2a 6578 7065 6374  info = {**expect
-00011aa0: 6564 5f69 6e66 6f5f 6261 7365 2c20 226e  ed_info_base, "n
-00011ab0: 616d 6522 3a20 696d 706f 7274 5f73 6f75  ame": import_sou
-00011ac0: 7263 655f 6e61 6d65 7d0a 2020 2020 2020  rce_name}.      
-00011ad0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00011ae0: 7375 6254 6573 7428 6e61 6d65 3d6e 616d  subTest(name=nam
-00011af0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00011b00: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00011b10: 7175 616c 2865 7870 6563 7465 645f 696e  qual(expected_in
-00011b20: 666f 2c20 7474 325f 696e 666f 290a 2020  fo, tt2_info).  
-00011b30: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-00011b40: 656c 662e 7375 6254 6573 7428 6e61 6d65  elf.subTest(name
-00011b50: 3d6e 616d 6529 3a0a 2020 2020 2020 2020  =name):.        
-00011b60: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00011b70: 6572 7445 7175 616c 2873 756d 2874 742e  ertEqual(sum(tt.
-00011b80: 616c 6c2e 6129 2c20 7375 6d28 7474 322e  all.a), sum(tt2.
-00011b90: 616c 6c2e 6129 290a 2020 2020 2020 2020  all.a)).        
-00011ba0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00011bb0: 6254 6573 7428 6e61 6d65 3d6e 616d 6529  bTest(name=name)
-00011bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011bd0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00011be0: 616c 2873 756d 2874 742e 616c 6c2e 6229  al(sum(tt.all.b)
-00011bf0: 2c20 7375 6d28 7474 322e 616c 6c2e 6229  , sum(tt2.all.b)
-00011c00: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-00011c10: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00011c20: 6e61 6d65 3d6e 616d 6529 3a0a 2020 2020  name=name):.    
-00011c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011c40: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
-00011c50: 2874 742e 616c 6c2e 6329 2c20 7375 6d28  (tt.all.c), sum(
-00011c60: 7474 322e 616c 6c2e 6329 290a 0a20 2020  tt2.all.c))..   
-00011c70: 2020 2020 2023 2074 6573 7420 7365 7061       # test sepa
-00011c80: 7261 7465 6c79 2c20 6e6f 2074 7261 6e73  rately, no trans
-00011c90: 666f 726d 7320 666f 7220 4a53 4f4e 2069  forms for JSON i
-00011ca0: 6d70 6f72 7473 0a20 2020 2020 2020 2069  mports.        i
-00011cb0: 6d70 6f72 745f 736f 7572 6365 5f6e 616d  mport_source_nam
-00011cc0: 6520 3d20 2274 6573 742f 6162 632e 6a73  e = "test/abc.js
-00011cd0: 6f6e 2e67 7a22 0a20 2020 2020 2020 2077  on.gz".        w
-00011ce0: 6974 6820 7469 6d65 7374 616d 705f 7374  ith timestamp_st
-00011cf0: 6172 745f 656e 6428 2920 6173 2074 696d  art_end() as tim
-00011d00: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00011d10: 2074 7432 203d 206c 742e 5461 626c 6528   tt2 = lt.Table(
-00011d20: 292e 6a73 6f6e 5f69 6d70 6f72 7428 2274  ).json_import("t
-00011d30: 6573 742f 6162 632e 6a73 6f6e 2e67 7a22  est/abc.json.gz"
-00011d40: 2c20 7374 7265 616d 696e 673d 5472 7565  , streaming=True
-00011d50: 290a 0a20 2020 2020 2020 2074 7432 5f69  )..        tt2_i
-00011d60: 6e66 6f20 3d20 7474 322e 696e 666f 2829  nfo = tt2.info()
-00011d70: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00011d80: 6162 632e 6a73 6f6e 2e67 7a22 2c20 7474  abc.json.gz", tt
-00011d90: 325f 696e 666f 290a 0a20 2020 2020 2020  2_info)..       
-00011da0: 2076 6572 6966 795f 7469 6d65 7374 616d   verify_timestam
-00011db0: 7073 2874 696d 696e 672e 7374 6172 742c  ps(timing.start,
-00011dc0: 2074 696d 696e 672e 656e 642c 2074 7432   timing.end, tt2
-00011dd0: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
-00011de0: 6578 7065 6374 6564 5f69 6e66 6f20 3d20  expected_info = 
-00011df0: 7b2a 2a65 7870 6563 7465 645f 696e 666f  {**expected_info
-00011e00: 5f62 6173 652c 2022 6e61 6d65 223a 2069  _base, "name": i
-00011e10: 6d70 6f72 745f 736f 7572 6365 5f6e 616d  mport_source_nam
-00011e20: 657d 0a20 2020 2020 2020 2077 6974 6820  e}.        with 
-00011e30: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00011e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011e50: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-00011e60: 6563 7465 645f 696e 666f 2c20 7474 325f  ected_info, tt2_
-00011e70: 696e 666f 290a 2020 2020 2020 2020 7769  info).        wi
-00011e80: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00011e90: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00011ea0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00011eb0: 7375 6d28 7474 2e61 6c6c 2e61 292c 2073  sum(tt.all.a), s
-00011ec0: 756d 2874 7432 2e61 6c6c 2e61 2929 0a20  um(tt2.all.a)). 
-00011ed0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00011ee0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00011ef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00011f00: 6572 7445 7175 616c 2873 756d 2874 742e  ertEqual(sum(tt.
-00011f10: 616c 6c2e 6229 2c20 7375 6d28 7474 322e  all.b), sum(tt2.
-00011f20: 616c 6c2e 6229 290a 2020 2020 2020 2020  all.b)).        
-00011f30: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00011f40: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00011f50: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00011f60: 6c28 7375 6d28 7474 2e61 6c6c 2e63 292c  l(sum(tt.all.c),
-00011f70: 2073 756d 2874 7432 2e61 6c6c 2e63 2929   sum(tt2.all.c))
-00011f80: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
-00011f90: 7376 5f69 6d70 6f72 745f 736f 7572 6365  sv_import_source
-00011fa0: 5f69 6e66 6f28 7365 6c66 293a 0a20 2020  _info(self):.   
-00011fb0: 2020 2020 2069 6d70 6f72 7473 203d 205b       imports = [
-00011fc0: 0a20 2020 2020 2020 2020 2020 2028 2261  .            ("a
-00011fd0: 6263 2e63 7376 222c 206c 742e 496d 706f  bc.csv", lt.Impo
-00011fe0: 7274 536f 7572 6365 5479 7065 2e66 696c  rtSourceType.fil
-00011ff0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00012000: 2822 6162 632e 7473 7622 2c20 6c74 2e49  ("abc.tsv", lt.I
-00012010: 6d70 6f72 7453 6f75 7263 6554 7970 652e  mportSourceType.
-00012020: 6669 6c65 292c 0a20 2020 2020 2020 2020  file),.         
-00012030: 2020 2028 2261 6263 2e78 6c73 7822 2c20     ("abc.xlsx", 
-00012040: 6c74 2e49 6d70 6f72 7453 6f75 7263 6554  lt.ImportSourceT
-00012050: 7970 652e 6669 6c65 292c 0a20 2020 2020  ype.file),.     
-00012060: 2020 2020 2020 2028 2261 6263 2e63 7376         ("abc.csv
-00012070: 2e7a 6970 222c 206c 742e 496d 706f 7274  .zip", lt.Import
-00012080: 536f 7572 6365 5479 7065 2e7a 6970 292c  SourceType.zip),
-00012090: 0a20 2020 2020 2020 2020 2020 2028 2261  .            ("a
-000120a0: 6263 2e63 7376 2e67 7a22 2c20 6c74 2e49  bc.csv.gz", lt.I
-000120b0: 6d70 6f72 7453 6f75 7263 6554 7970 652e  mportSourceType.
-000120c0: 677a 6970 292c 0a20 2020 2020 2020 2020  gzip),.         
-000120d0: 2020 2028 2261 6263 2e63 7376 2e78 7a22     ("abc.csv.xz"
-000120e0: 2c20 6c74 2e49 6d70 6f72 7453 6f75 7263  , lt.ImportSourc
-000120f0: 6554 7970 652e 6c7a 6d61 292c 0a20 2020  eType.lzma),.   
-00012100: 2020 2020 2020 2020 2028 2261 2c62 2c63           ("a,b,c
-00012110: 5c6e 312c 322c 3322 2c20 6c74 2e49 6d70  \n1,2,3", lt.Imp
-00012120: 6f72 7453 6f75 7263 6554 7970 652e 7374  ortSourceType.st
-00012130: 7269 6e67 292c 0a20 2020 2020 2020 205d  ring),.        ]
-00012140: 0a20 2020 2020 2020 2066 6f72 2066 6e61  .        for fna
-00012150: 6d65 2c20 6578 7065 6374 6564 5f74 7970  me, expected_typ
-00012160: 6520 696e 2069 6d70 6f72 7473 3a0a 2020  e in imports:.  
-00012170: 2020 2020 2020 2020 2020 6966 2022 5c6e            if "\n
-00012180: 2220 6e6f 7420 696e 2066 6e61 6d65 3a0a  " not in fname:.
-00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121a0: 696d 706f 7274 5f6e 616d 6520 3d20 2274  import_name = "t
-000121b0: 6573 742f 2220 2b20 666e 616d 650a 2020  est/" + fname.  
-000121c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 696d 706f 7274 5f6e 616d 6520 3d20 666e  import_name = fn
-000121f0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00012200: 6966 2069 6d70 6f72 745f 6e61 6d65 2e65  if import_name.e
-00012210: 6e64 7377 6974 6828 222e 6373 7622 293a  ndswith(".csv"):
-00012220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012230: 2074 626c 203d 206c 742e 5461 626c 6528   tbl = lt.Table(
-00012240: 292e 6373 765f 696d 706f 7274 2869 6d70  ).csv_import(imp
-00012250: 6f72 745f 6e61 6d65 290a 2020 2020 2020  ort_name).      
-00012260: 2020 2020 2020 656c 6966 2069 6d70 6f72        elif impor
-00012270: 745f 6e61 6d65 2e65 6e64 7377 6974 6828  t_name.endswith(
-00012280: 222e 786c 7378 2229 3a0a 2020 2020 2020  ".xlsx"):.      
-00012290: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
-000122a0: 6c74 2e54 6162 6c65 2829 2e65 7863 656c  lt.Table().excel
-000122b0: 5f69 6d70 6f72 7428 696d 706f 7274 5f6e  _import(import_n
-000122c0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-000122d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000122e0: 2020 2020 2020 2074 626c 203d 206c 742e         tbl = lt.
-000122f0: 5461 626c 6528 292e 7473 765f 696d 706f  Table().tsv_impo
-00012300: 7274 2869 6d70 6f72 745f 6e61 6d65 290a  rt(import_name).
-00012310: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00012320: 6e74 2872 6570 7228 696d 706f 7274 5f6e  nt(repr(import_n
-00012330: 616d 6529 2c20 7462 6c2e 696d 706f 7274  ame), tbl.import
-00012340: 5f73 6f75 7263 652c 2074 626c 2e69 6d70  _source, tbl.imp
-00012350: 6f72 745f 736f 7572 6365 5f74 7970 6529  ort_source_type)
-00012360: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00012370: 2022 5c6e 2220 6e6f 7420 696e 2066 6e61   "\n" not in fna
-00012380: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-00012390: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000123a0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000123b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000123c0: 662e 6173 7365 7274 4571 7561 6c28 696d  f.assertEqual(im
-000123d0: 706f 7274 5f6e 616d 652c 2074 626c 2e69  port_name, tbl.i
-000123e0: 6d70 6f72 745f 736f 7572 6365 290a 2020  mport_source).  
-000123f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012410: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00012420: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00012430: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00012440: 7365 7274 4571 7561 6c28 4e6f 6e65 2c20  sertEqual(None, 
-00012450: 7462 6c2e 696d 706f 7274 5f73 6f75 7263  tbl.import_sourc
-00012460: 6529 0a20 2020 2020 2020 2020 2020 2077  e).            w
-00012470: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00012480: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012490: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000124a0: 7175 616c 2865 7870 6563 7465 645f 7479  qual(expected_ty
-000124b0: 7065 2c20 7462 6c2e 696d 706f 7274 5f73  pe, tbl.import_s
-000124c0: 6f75 7263 655f 7479 7065 290a 0a20 2020  ource_type)..   
-000124d0: 2064 6566 2074 6573 745f 6373 765f 696d   def test_csv_im
-000124e0: 706f 7274 5f66 726f 6d5f 7572 6c28 7365  port_from_url(se
-000124f0: 6c66 293a 0a20 2020 2020 2020 2066 726f  lf):.        fro
-00012500: 6d20 6874 7470 2e73 6572 7665 7220 696d  m http.server im
-00012510: 706f 7274 2048 5454 5053 6572 7665 722c  port HTTPServer,
-00012520: 2042 6173 6548 5454 5052 6571 7565 7374   BaseHTTPRequest
-00012530: 4861 6e64 6c65 720a 2020 2020 2020 2020  Handler.        
-00012540: 6672 6f6d 2068 7474 7020 696d 706f 7274  from http import
-00012550: 2048 5454 5053 7461 7475 730a 2020 2020   HTTPStatus.    
-00012560: 2020 2020 696d 706f 7274 2074 6872 6561      import threa
-00012570: 6469 6e67 0a20 2020 2020 2020 2069 6d70  ding.        imp
-00012580: 6f72 7420 7469 6d65 0a20 2020 2020 2020  ort time.       
-00012590: 2069 6d70 6f72 7420 7572 6c6c 6962 2e65   import urllib.e
-000125a0: 7272 6f72 0a20 2020 2020 2020 2069 6d70  rror.        imp
-000125b0: 6f72 7420 7572 6c6c 6962 2e72 6571 7565  ort urllib.reque
-000125c0: 7374 0a0a 2020 2020 2020 2020 6966 2053  st..        if S
-000125d0: 4b49 505f 4353 565f 494d 504f 5254 5f55  KIP_CSV_IMPORT_U
-000125e0: 5349 4e47 5f55 524c 5f54 4553 5453 3a0a  SING_URL_TESTS:.
-000125f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012600: 2e73 6b69 7054 6573 7428 2243 5356 2069  .skipTest("CSV i
-00012610: 6d70 6f72 7420 7465 7374 7320 736b 6970  mport tests skip
-00012620: 7065 6422 290a 0a20 2020 2020 2020 2063  ped")..        c
-00012630: 6c61 7373 2043 5356 5465 7374 5265 7175  lass CSVTestRequ
-00012640: 6573 7448 616e 646c 6572 2842 6173 6548  estHandler(BaseH
-00012650: 5454 5052 6571 7565 7374 4861 6e64 6c65  TTPRequestHandle
-00012660: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00012670: 6465 6620 646f 5f47 4554 2873 656c 6629  def do_GET(self)
-00012680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012690: 2020 7365 6c66 2e6c 6f67 5f6d 6573 7361    self.log_messa
-000126a0: 6765 2866 2272 6563 6569 7665 6420 7b73  ge(f"received {s
-000126b0: 656c 662e 636f 6d6d 616e 647d 207b 7365  elf.command} {se
-000126c0: 6c66 2e70 6174 687d 2229 0a20 2020 2020  lf.path}").     
-000126d0: 2020 2020 2020 2020 2020 2070 6174 6820             path 
-000126e0: 3d20 7365 6c66 2e70 6174 680a 2020 2020  = self.path.    
-000126f0: 2020 2020 2020 2020 2020 2020 7365 6e64              send
-00012700: 5f62 7974 6573 203d 2062 2222 0a20 2020  _bytes = b"".   
-00012710: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012720: 7061 7468 203d 3d20 222f 4558 4954 223a  path == "/EXIT":
-00012730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012740: 2020 2020 2073 656c 662e 7365 6e64 5f72       self.send_r
-00012750: 6573 706f 6e73 6528 4854 5450 5374 6174  esponse(HTTPStat
-00012760: 7573 2e4f 4b29 0a20 2020 2020 2020 2020  us.OK).         
-00012770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012780: 656e 645f 6865 6164 6572 7328 290a 2020  end_headers().  
-00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 7365 6c66 2e77 6669 6c65 2e77 7269    self.wfile.wri
-000127b0: 7465 2873 656e 645f 6279 7465 7329 0a20  te(send_bytes). 
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 2020 2074 6872 6561 6469 6e67 2e54 6872     threading.Thr
-000127e0: 6561 6428 7461 7267 6574 3d6c 616d 6264  ead(target=lambd
-000127f0: 613a 2074 696d 652e 736c 6565 7028 3129  a: time.sleep(1)
-00012800: 206f 7220 7365 6c66 2e73 6572 7665 722e   or self.server.
-00012810: 7368 7574 646f 776e 2829 292e 7374 6172  shutdown()).star
-00012820: 7428 290a 0a20 2020 2020 2020 2020 2020  t()..           
-00012830: 2020 2020 2065 6c69 6620 7061 7468 203d       elif path =
-00012840: 3d20 222f 223a 0a20 2020 2020 2020 2020  = "/":.         
-00012850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012860: 7365 6e64 5f72 6573 706f 6e73 6528 4854  send_response(HT
-00012870: 5450 5374 6174 7573 2e4f 4b29 0a20 2020  TPStatus.OK).   
-00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 2073 656c 662e 656e 645f 6865 6164 6572   self.end_header
-000128a0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-000128b0: 2020 2020 2020 2020 7365 6c66 2e77 6669          self.wfi
-000128c0: 6c65 2e77 7269 7465 2873 656e 645f 6279  le.write(send_by
-000128d0: 7465 7329 0a0a 2020 2020 2020 2020 2020  tes)..          
-000128e0: 2020 2020 2020 656c 6966 2070 6174 682e        elif path.
-000128f0: 7374 6172 7473 7769 7468 2822 2f61 6263  startswith("/abc
-00012900: 2e63 7376 2229 3a0a 2020 2020 2020 2020  .csv"):.        
-00012910: 2020 2020 2020 2020 2020 2020 7365 6e64              send
-00012920: 5f62 7974 6573 202b 3d20 6222 612c 622c  _bytes += b"a,b,
-00012930: 635c 6e31 2c32 2c33 5c6e 220a 2020 2020  c\n1,2,3\n".    
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 7365 6c66 2e73 656e 645f 7265 7370 6f6e  self.send_respon
-00012960: 7365 2848 5454 5053 7461 7475 732e 4f4b  se(HTTPStatus.OK
-00012970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012980: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00012990: 6865 6164 6572 2822 436f 6e74 656e 742d  header("Content-
-000129a0: 4c65 6e67 7468 222c 2073 7472 286c 656e  Length", str(len
-000129b0: 2873 656e 645f 6279 7465 7329 2929 0a20  (send_bytes))). 
-000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 2073 656c 662e 656e 645f 6865 6164     self.end_head
-000129e0: 6572 7328 290a 2020 2020 2020 2020 2020  ers().          
-000129f0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00012a00: 6669 6c65 2e77 7269 7465 2873 656e 645f  file.write(send_
-00012a10: 6279 7465 7329 0a0a 2020 2020 2020 2020  bytes)..        
-00012a20: 2020 2020 6465 6620 646f 5f50 4f53 5428      def do_POST(
-00012a30: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-00012a40: 2020 2020 2020 2073 656c 662e 6c6f 675f         self.log_
-00012a50: 6d65 7373 6167 6528 6622 7265 6365 6976  message(f"receiv
-00012a60: 6564 207b 7365 6c66 2e63 6f6d 6d61 6e64  ed {self.command
-00012a70: 7d20 7b73 656c 662e 7061 7468 7d22 290a  } {self.path}").
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 7061 7468 203d 2073 656c 662e 7061 7468  path = self.path
+0000a0b0: 2020 2020 2022 6173 5f68 746d 6c20 646f       "as_html do
+0000a0c0: 6573 206e 6f74 2069 6e63 6c75 6465 2074  es not include t
+0000a0d0: 6865 6164 2061 6e64 2074 626f 6479 2074  head and tbody t
+0000a0e0: 6167 7322 290a 0a20 2020 2020 2020 2068  ags")..        h
+0000a0f0: 746d 6c5f 6c69 6e65 7320 3d20 6874 6d6c  tml_lines = html
+0000a100: 5f6f 7574 7075 742e 7370 6c69 746c 696e  _output.splitlin
+0000a110: 6573 2829 0a20 2020 2020 2020 2068 6472  es().        hdr
+0000a120: 5f6c 696e 6520 3d20 6e65 7874 2868 2066  _line = next(h f
+0000a130: 6f72 2068 2069 6e20 6874 6d6c 5f6c 696e  or h in html_lin
+0000a140: 6573 2069 6620 2263 656e 7465 7222 2069  es if "center" i
+0000a150: 6e20 6829 0a20 2020 2020 2020 2073 656c  n h).        sel
+0000a160: 662e 6173 7365 7274 4571 7561 6c28 273c  f.assertEqual('<
+0000a170: 7472 3e3c 7468 3e3c 6469 7620 616c 6967  tr><th><div alig
+0000a180: 6e3d 2263 656e 7465 7222 3e61 3c2f 6469  n="center">a</di
+0000a190: 763e 3c2f 7468 3e27 0a20 2020 2020 2020  v></th>'.       
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 273c 7468 3e3c 6469 7620 616c 6967    '<th><div alig
+0000a1c0: 6e3d 2263 656e 7465 7222 3e62 3c2f 6469  n="center">b</di
+0000a1d0: 763e 3c2f 7468 3e27 0a20 2020 2020 2020  v></th>'.       
+0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1f0: 2020 273c 7468 3e3c 6469 7620 616c 6967    '<th><div alig
+0000a200: 6e3d 2263 656e 7465 7222 3e63 3c2f 6469  n="center">c</di
+0000a210: 763e 3c2f 7468 3e3c 2f74 723e 272c 0a20  v></th></tr>',. 
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 2020 2020 2020 2020 6864 725f 6c69 6e65          hdr_line
+0000a240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a250: 2020 2020 2020 2020 2020 2022 6661 696c             "fail
+0000a260: 6564 2061 735f 6874 6d6c 2077 6974 6820  ed as_html with 
+0000a270: 616c 6c20 6669 656c 6473 2229 0a0a 2020  all fields")..  
+0000a280: 2020 2020 2020 6874 6d6c 5f6f 7574 7075        html_outpu
+0000a290: 7420 3d20 7365 6c66 2e74 315b 3a31 305d  t = self.t1[:10]
+0000a2a0: 2e61 735f 6874 6d6c 2866 6965 6c64 733d  .as_html(fields=
+0000a2b0: 2261 202d 6220 6322 290a 2020 2020 2020  "a -b c").      
+0000a2c0: 2020 7072 696e 7428 6874 6d6c 5f6f 7574    print(html_out
+0000a2d0: 7075 7429 0a20 2020 2020 2020 2068 746d  put).        htm
+0000a2e0: 6c5f 6c69 6e65 7320 3d20 6874 6d6c 5f6f  l_lines = html_o
+0000a2f0: 7574 7075 742e 7370 6c69 746c 696e 6573  utput.splitlines
+0000a300: 2829 0a20 2020 2020 2020 2068 6472 5f6c  ().        hdr_l
+0000a310: 696e 6520 3d20 6e65 7874 2868 2066 6f72  ine = next(h for
+0000a320: 2068 2069 6e20 6874 6d6c 5f6c 696e 6573   h in html_lines
+0000a330: 2069 6620 2263 656e 7465 7222 2069 6e20   if "center" in 
+0000a340: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+0000a350: 6173 7365 7274 4571 7561 6c28 273c 7472  assertEqual('<tr
+0000a360: 3e3c 7468 3e3c 6469 7620 616c 6967 6e3d  ><th><div align=
+0000a370: 2263 656e 7465 7222 3e61 3c2f 6469 763e  "center">a</div>
+0000a380: 3c2f 7468 3e27 0a20 2020 2020 2020 2020  </th>'.         
+0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3a0: 273c 7468 3e3c 6469 7620 616c 6967 6e3d  '<th><div align=
+0000a3b0: 2263 656e 7465 7222 3e63 3c2f 6469 763e  "center">c</div>
+0000a3c0: 3c2f 7468 3e3c 2f74 723e 272c 0a20 2020  </th></tr>',.   
+0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 2020 2020 2020 6864 725f 6c69 6e65 2c0a        hdr_line,.
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2020 2020 2020 2020 2022 6661 696c 6564           "failed
+0000a410: 2061 735f 6874 6d6c 2077 6974 6820 6e65   as_html with ne
+0000a420: 6761 7465 6420 6669 656c 6422 290a 0a20  gated field").. 
+0000a430: 2020 2020 2020 2068 746d 6c5f 6f75 7470         html_outp
+0000a440: 7574 203d 2073 656c 662e 7431 5b3a 3130  ut = self.t1[:10
+0000a450: 5d2e 6173 5f68 746d 6c28 6669 656c 6473  ].as_html(fields
+0000a460: 3d22 6120 6220 6322 2c20 666f 726d 6174  ="a b c", format
+0000a470: 733d 7b22 6222 3a20 227b 3a30 3364 7d22  s={"b": "{:03d}"
+0000a480: 7d29 0a20 2020 2020 2020 2070 7269 6e74  }).        print
+0000a490: 2868 746d 6c5f 6f75 7470 7574 290a 2020  (html_output).  
+0000a4a0: 2020 2020 2020 6874 6d6c 5f6c 696e 6573        html_lines
+0000a4b0: 203d 2068 746d 6c5f 6f75 7470 7574 2e73   = html_output.s
+0000a4c0: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
+0000a4d0: 2020 2020 6461 7461 5f6c 696e 6520 3d20      data_line = 
+0000a4e0: 6e65 7874 2868 2066 6f72 2068 2069 6e20  next(h for h in 
+0000a4f0: 6874 6d6c 5f6c 696e 6573 2069 6620 223c  html_lines if "<
+0000a500: 7464 3e22 2069 6e20 6829 0a20 2020 2020  td>" in h).     
+0000a510: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000a520: 7561 6c28 273c 7462 6f64 793e 3c74 723e  ual('<tbody><tr>
+0000a530: 3c74 643e 3c64 6976 2061 6c69 676e 3d22  <td><div align="
+0000a540: 7269 6768 7422 3e30 3c2f 6469 763e 3c2f  right">0</div></
+0000a550: 7464 3e27 0a20 2020 2020 2020 2020 2020  td>'.           
+0000a560: 2020 2020 2020 2020 2020 2020 2020 273c                '<
+0000a570: 7464 3e3c 6469 7620 616c 6967 6e3d 2272  td><div align="r
+0000a580: 6967 6874 223e 3030 303c 2f64 6976 3e3c  ight">000</div><
+0000a590: 2f74 643e 270a 2020 2020 2020 2020 2020  /td>'.          
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a5b0: 3c74 643e 3c64 6976 2061 6c69 676e 3d22  <td><div align="
+0000a5c0: 7269 6768 7422 3e30 3c2f 6469 763e 3c2f  right">0</div></
+0000a5d0: 7464 3e3c 2f74 723e 272c 0a20 2020 2020  td></tr>',.     
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 6461 7461 5f6c 696e 652c 0a20      data_line,. 
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 2020 2020 2020 2266 6169 6c65 6420          "failed 
+0000a620: 6173 5f68 746d 6c20 7769 7468 206e 616d  as_html with nam
+0000a630: 6564 2066 6965 6c64 2066 6f72 6d61 7420  ed field format 
+0000a640: 666f 7220 7370 6563 6966 6963 2066 6965  for specific fie
+0000a650: 6c64 2229 0a0a 2020 2020 2020 2020 6874  ld")..        ht
+0000a660: 6d6c 5f6f 7574 7075 7420 3d20 7365 6c66  ml_output = self
+0000a670: 2e74 315b 3a31 305d 2e61 735f 6874 6d6c  .t1[:10].as_html
+0000a680: 2866 6965 6c64 733d 2261 2062 2063 222c  (fields="a b c",
+0000a690: 2066 6f72 6d61 7473 3d7b 696e 743a 2022   formats={int: "
+0000a6a0: 7b3a 3033 647d 227d 290a 2020 2020 2020  {:03d}"}).      
+0000a6b0: 2020 7072 696e 7428 6874 6d6c 5f6f 7574    print(html_out
+0000a6c0: 7075 7429 0a20 2020 2020 2020 2068 746d  put).        htm
+0000a6d0: 6c5f 6c69 6e65 7320 3d20 6874 6d6c 5f6f  l_lines = html_o
+0000a6e0: 7574 7075 742e 7370 6c69 746c 696e 6573  utput.splitlines
+0000a6f0: 2829 0a20 2020 2020 2020 2064 6174 615f  ().        data_
+0000a700: 6c69 6e65 203d 206e 6578 7428 6820 666f  line = next(h fo
+0000a710: 7220 6820 696e 2068 746d 6c5f 6c69 6e65  r h in html_line
+0000a720: 7320 6966 2022 3c74 643e 2220 696e 2068  s if "<td>" in h
+0000a730: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000a740: 7373 6572 7445 7175 616c 2827 3c74 626f  ssertEqual('<tbo
+0000a750: 6479 3e3c 7472 3e3c 7464 3e3c 6469 7620  dy><tr><td><div 
+0000a760: 616c 6967 6e3d 2272 6967 6874 223e 3030  align="right">00
+0000a770: 303c 2f64 6976 3e3c 2f74 643e 270a 2020  0</div></td>'.  
+0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a790: 2020 2020 2020 2027 3c74 643e 3c64 6976         '<td><div
+0000a7a0: 2061 6c69 676e 3d22 7269 6768 7422 3e30   align="right">0
+0000a7b0: 3030 3c2f 6469 763e 3c2f 7464 3e27 0a20  00</div></td>'. 
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 2020 2020 2020 2020 273c 7464 3e3c 6469          '<td><di
+0000a7e0: 7620 616c 6967 6e3d 2272 6967 6874 223e  v align="right">
+0000a7f0: 3030 303c 2f64 6976 3e3c 2f74 643e 3c2f  000</div></td></
+0000a800: 7472 3e27 2c0a 2020 2020 2020 2020 2020  tr>',.          
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000a820: 6174 615f 6c69 6e65 2c0a 2020 2020 2020  ata_line,.      
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 2020 2022 6661 696c 6564 2061 735f 6874     "failed as_ht
+0000a850: 6d6c 2077 6974 6820 6461 7461 2074 7970  ml with data typ
+0000a860: 6520 666f 726d 6174 2066 6f72 2061 6c6c  e format for all
+0000a870: 2066 6965 6c64 7322 290a 0a20 2020 2020   fields")..     
+0000a880: 2020 2068 746d 6c5f 6f75 7470 7574 203d     html_output =
+0000a890: 2073 656c 662e 7431 5b3a 3130 5d2e 6173   self.t1[:10].as
+0000a8a0: 5f68 746d 6c28 6669 656c 6473 3d22 6120  _html(fields="a 
+0000a8b0: 6220 6322 2c20 666f 726d 6174 733d 7b69  b c", formats={i
+0000a8c0: 6e74 3a20 227b 3a30 3364 7d22 7d2c 2067  nt: "{:03d}"}, g
+0000a8d0: 726f 7570 6279 3d22 6122 290a 2020 2020  roupby="a").    
+0000a8e0: 2020 2020 7072 696e 7428 6874 6d6c 5f6f      print(html_o
+0000a8f0: 7574 7075 7429 0a20 2020 2020 2020 2068  utput).        h
+0000a900: 746d 6c5f 6c69 6e65 7320 3d20 6874 6d6c  tml_lines = html
+0000a910: 5f6f 7574 7075 742e 7370 6c69 746c 696e  _output.splitlin
+0000a920: 6573 2829 0a20 2020 2020 2020 2064 6174  es().        dat
+0000a930: 615f 6c69 6e65 203d 206e 6578 7428 6820  a_line = next(h 
+0000a940: 666f 7220 6820 696e 2068 746d 6c5f 6c69  for h in html_li
+0000a950: 6e65 7320 6966 2022 3c74 643e 2220 696e  nes if "<td>" in
+0000a960: 2068 290a 2020 2020 2020 2020 7365 6c66   h).        self
+0000a970: 2e61 7373 6572 7445 7175 616c 2827 3c74  .assertEqual('<t
+0000a980: 626f 6479 3e3c 7472 3e3c 7464 3e3c 6469  body><tr><td><di
+0000a990: 7620 616c 6967 6e3d 2272 6967 6874 223e  v align="right">
+0000a9a0: 3030 303c 2f64 6976 3e3c 2f74 643e 270a  000</div></td>'.
+0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9c0: 2020 2020 2020 2020 2027 3c74 643e 3c64           '<td><d
+0000a9d0: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
+0000a9e0: 3e30 3030 3c2f 6469 763e 3c2f 7464 3e27  >000</div></td>'
+0000a9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aa00: 2020 2020 2020 2020 2020 273c 7464 3e3c            '<td><
+0000aa10: 6469 7620 616c 6967 6e3d 2272 6967 6874  div align="right
+0000aa20: 223e 3030 303c 2f64 6976 3e3c 2f74 643e  ">000</div></td>
+0000aa30: 3c2f 7472 3e27 2c0a 2020 2020 2020 2020  </tr>',.        
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa50: 2064 6174 615f 6c69 6e65 2c0a 2020 2020   data_line,.    
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 2022 6661 696c 6564 2061 735f       "failed as_
+0000aa80: 6874 6d6c 2077 6974 6820 6772 6f75 7062  html with groupb
+0000aa90: 7922 290a 0a20 2020 2020 2020 2068 746d  y")..        htm
+0000aaa0: 6c5f 6f75 7470 7574 203d 2073 656c 662e  l_output = self.
+0000aab0: 7431 5b3a 3130 5d2e 6173 5f68 746d 6c28  t1[:10].as_html(
+0000aac0: 6669 656c 6473 3d22 6120 6220 6322 2c20  fields="a b c", 
+0000aad0: 7461 626c 655f 7072 6f70 6572 7469 6573  table_properties
+0000aae0: 3d7b 2262 6f72 6465 7222 3a20 2232 227d  ={"border": "2"}
+0000aaf0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000ab00: 6874 6d6c 5f6f 7574 7075 7429 0a20 2020  html_output).   
+0000ab10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000ab20: 5472 7565 2822 3c74 6865 6164 3e22 2069  True("<thead>" i
+0000ab30: 6e20 6874 6d6c 5f6f 7574 7075 7420 616e  n html_output an
+0000ab40: 6420 223c 7462 6f64 793e 2220 696e 2068  d "<tbody>" in h
+0000ab50: 746d 6c5f 6f75 7470 7574 2c0a 2020 2020  tml_output,.    
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2261 735f 6874 6d6c 2064 6f65      "as_html doe
+0000ab80: 7320 6e6f 7420 696e 636c 7564 6520 7468  s not include th
+0000ab90: 6561 6420 616e 6420 7462 6f64 7920 7461  ead and tbody ta
+0000aba0: 6773 2229 0a0a 0a20 2020 2064 6566 2074  gs")...    def t
+0000abb0: 6573 745f 6465 6c65 7465 5f73 6c69 6365  est_delete_slice
+0000abc0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0000abd0: 2063 6f6d 7061 7265 5f6c 6973 7420 3d20   compare_list = 
+0000abe0: 6c69 7374 2822 4142 4344 4546 4748 494a  list("ABCDEFGHIJ
+0000abf0: 4b4c 4d4e 4f50 5152 5354 5556 5758 595a  KLMNOPQRSTUVWXYZ
+0000ac00: 3031 3233 3435 3637 3839 6162 6364 6566  0123456789abcdef
+0000ac10: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
+0000ac20: 7778 797a 2229 0a20 2020 2020 2020 2074  wxyz").        t
+0000ac30: 3120 3d20 6c74 2e54 6162 6c65 2829 2e69  1 = lt.Table().i
+0000ac40: 6e73 6572 745f 6d61 6e79 286c 742e 4461  nsert_many(lt.Da
+0000ac50: 7461 4f62 6a65 6374 2841 3d63 2920 666f  taObject(A=c) fo
+0000ac60: 7220 6320 696e 2063 6f6d 7061 7265 5f6c  r c in compare_l
+0000ac70: 6973 7429 0a0a 2020 2020 2020 2020 6465  ist)..        de
+0000ac80: 6620 6d69 6e69 5f74 6573 7428 736c 635f  f mini_test(slc_
+0000ac90: 7475 706c 6529 3a0a 2020 2020 2020 2020  tuple):.        
+0000aca0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000acb0: 6528 736c 635f 7475 706c 652c 2074 7570  e(slc_tuple, tup
+0000acc0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+0000acd0: 2020 2020 206c 6162 656c 203d 2022 5b7b       label = "[{
+0000ace0: 7d3a 7b7d 3a7b 7d5d 222e 666f 726d 6174  }:{}:{}]".format
+0000acf0: 282a 2869 2069 6620 6920 6973 206e 6f74  (*(i if i is not
+0000ad00: 204e 6f6e 6520 656c 7365 2027 2720 666f   None else '' fo
+0000ad10: 7220 6920 696e 2073 6c63 5f74 7570 6c65  r i in slc_tuple
+0000ad20: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000ad30: 2020 2073 6c63 203d 2073 6c69 6365 282a     slc = slice(*
+0000ad40: 736c 635f 7475 706c 6529 0a20 2020 2020  slc_tuple).     
+0000ad50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000ad60: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+0000ad70: 656c 203d 2073 7472 2873 6c63 5f74 7570  el = str(slc_tup
+0000ad80: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
+0000ad90: 2020 2020 736c 6320 3d20 736c 635f 7475      slc = slc_tu
+0000ada0: 706c 650a 0a20 2020 2020 2020 2020 2020  ple..           
+0000adb0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000adc0: 7374 286c 6162 656c 2c20 736c 635f 7475  st(label, slc_tu
+0000add0: 706c 653d 736c 635f 7475 706c 6529 3a0a  ple=slc_tuple):.
+0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adf0: 6465 6c20 636f 6d70 6172 655f 6c69 7374  del compare_list
+0000ae00: 5b73 6c63 5d0a 2020 2020 2020 2020 2020  [slc].          
+0000ae10: 2020 2020 2020 7072 696e 7428 6c61 6265        print(labe
+0000ae20: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
+0000ae30: 2020 2070 7269 6e74 2827 4578 7065 6374     print('Expect
+0000ae40: 6564 272c 2063 6f6d 7061 7265 5f6c 6973  ed', compare_lis
+0000ae50: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0000ae60: 2020 2064 656c 2074 315b 736c 635d 0a20     del t1[slc]. 
+0000ae70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000ae80: 7269 6e74 2827 4f62 7365 7276 6564 272c  rint('Observed',
+0000ae90: 206c 6973 7428 7431 2e61 6c6c 2e41 2929   list(t1.all.A))
+0000aea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aeb0: 2070 7269 6e74 2829 0a20 2020 2020 2020   print().       
+0000aec0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000aed0: 7365 7274 4571 7561 6c28 2727 2e6a 6f69  sertEqual(''.joi
+0000aee0: 6e28 636f 6d70 6172 655f 6c69 7374 292c  n(compare_list),
+0000aef0: 2027 272e 6a6f 696e 2874 312e 616c 6c2e   ''.join(t1.all.
+0000af00: 4129 2c20 2266 6169 6c65 6420 2220 2b20  A), "failed " + 
+0000af10: 6c61 6265 6c29 0a0a 2020 2020 2020 2020  label)..        
+0000af20: 6d69 6e69 5f74 6573 7428 3529 0a20 2020  mini_test(5).   
+0000af30: 2020 2020 206d 696e 695f 7465 7374 282d       mini_test(-
+0000af40: 3529 0a20 2020 2020 2020 206d 696e 695f  5).        mini_
+0000af50: 7465 7374 2828 2d35 2c20 4e6f 6e65 2c20  test((-5, None, 
+0000af60: 4e6f 6e65 2929 0a20 2020 2020 2020 206d  None)).        m
+0000af70: 696e 695f 7465 7374 2828 4e6f 6e65 2c20  ini_test((None, 
+0000af80: 332c 204e 6f6e 6529 290a 2020 2020 2020  3, None)).      
+0000af90: 2020 6d69 6e69 5f74 6573 7428 284e 6f6e    mini_test((Non
+0000afa0: 652c 202d 6c65 6e28 636f 6d70 6172 655f  e, -len(compare_
+0000afb0: 6c69 7374 292b 332c 204e 6f6e 6529 290a  list)+3, None)).
+0000afc0: 2020 2020 2020 2020 6d69 6e69 5f74 6573          mini_tes
+0000afd0: 7428 284e 6f6e 652c 204e 6f6e 652c 2035  t((None, None, 5
+0000afe0: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
+0000aff0: 7465 7374 2828 4e6f 6e65 2c20 4e6f 6e65  test((None, None
+0000b000: 2c20 2d35 2929 0a20 2020 2020 2020 206d  , -5)).        m
+0000b010: 696e 695f 7465 7374 2828 2d35 2c20 2d32  ini_test((-5, -2
+0000b020: 2c20 4e6f 6e65 2929 0a20 2020 2020 2020  , None)).       
+0000b030: 206d 696e 695f 7465 7374 2828 2d32 2c20   mini_test((-2, 
+0000b040: 2d35 2c20 2d31 2929 0a20 2020 2020 2020  -5, -1)).       
+0000b050: 206d 696e 695f 7465 7374 2828 352c 2032   mini_test((5, 2
+0000b060: 302c 2032 2929 0a20 2020 2020 2020 206d  0, 2)).        m
+0000b070: 696e 695f 7465 7374 2828 6c65 6e28 636f  ini_test((len(co
+0000b080: 6d70 6172 655f 6c69 7374 292c 2035 2c20  mpare_list), 5, 
+0000b090: 2d33 2929 0a20 2020 2020 2020 206d 696e  -3)).        min
+0000b0a0: 695f 7465 7374 2828 3230 2c20 3131 2c20  i_test((20, 11, 
+0000b0b0: 2d37 2929 0a20 2020 2020 2020 206d 696e  -7)).        min
+0000b0c0: 695f 7465 7374 2828 352c 2035 2c20 4e6f  i_test((5, 5, No
+0000b0d0: 6e65 2929 0a20 2020 2020 2020 206d 696e  ne)).        min
+0000b0e0: 695f 7465 7374 2828 4e6f 6e65 2c20 2d31  i_test((None, -1
+0000b0f0: 302c 2035 2929 0a20 2020 2020 2020 206d  0, 5)).        m
+0000b100: 696e 695f 7465 7374 2828 4e6f 6e65 2c20  ini_test((None, 
+0000b110: 2d31 302c 202d 3130 2929 0a20 2020 2020  -10, -10)).     
+0000b120: 2020 206d 696e 695f 7465 7374 2828 3130     mini_test((10
+0000b130: 3030 2c20 3230 3030 2c20 4e6f 6e65 2929  00, 2000, None))
+0000b140: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
+0000b150: 7374 2828 4e6f 6e65 2c20 4e6f 6e65 2c20  st((None, None, 
+0000b160: 2d31 2929 0a0a 2020 2020 6465 6620 7465  -1))..    def te
+0000b170: 7374 5f63 6c65 6172 2873 656c 6629 3a0a  st_clear(self):.
+0000b180: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0000b190: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+0000b1a0: 2020 6e75 6d5f 6669 656c 6473 203d 206c    num_fields = l
+0000b1b0: 656e 2873 656c 662e 7431 2e69 6e66 6f28  en(self.t1.info(
+0000b1c0: 295b 2266 6965 6c64 7322 5d29 0a20 2020  )["fields"]).   
+0000b1d0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000b1e0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000b1f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000b200: 7445 7175 616c 2873 656c 662e 7465 7374  tEqual(self.test
+0000b210: 5f73 697a 6520 2a2a 206e 756d 5f66 6965  _size ** num_fie
+0000b220: 6c64 732c 206c 656e 2873 656c 662e 7431  lds, len(self.t1
+0000b230: 292c 2022 696e 7661 6c69 6420 6c65 6e22  ), "invalid len"
+0000b240: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+0000b250: 312e 6372 6561 7465 5f69 6e64 6578 2822  1.create_index("
+0000b260: 6122 290a 0a20 2020 2020 2020 2073 656c  a")..        sel
+0000b270: 662e 7431 2e63 6c65 6172 2829 0a20 2020  f.t1.clear().   
+0000b280: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000b290: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000b2a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000b2b0: 7445 7175 616c 2830 2c20 6c65 6e28 7365  tEqual(0, len(se
+0000b2c0: 6c66 2e74 3129 2c20 2269 6e76 616c 6964  lf.t1), "invalid
+0000b2d0: 206c 656e 2061 6674 6572 2063 6c65 6172   len after clear
+0000b2e0: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+0000b2f0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000b300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b310: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
+0000b320: 6c65 6e28 7365 6c66 2e74 312e 696e 666f  len(self.t1.info
+0000b330: 2829 5b22 696e 6465 7865 7322 5d29 2c20  ()["indexes"]), 
+0000b340: 2269 6e76 616c 6964 2069 6e64 6578 6573  "invalid indexes
+0000b350: 2061 6674 6572 2063 6c65 6172 2229 0a0a   after clear")..
+0000b360: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
+0000b370: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+0000b380: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+0000b390: 7428 290a 2020 2020 2020 2020 6669 656c  t().        fiel
+0000b3a0: 645f 6e61 6d65 7320 3d20 7365 6c66 2e74  d_names = self.t
+0000b3b0: 312e 696e 666f 2829 5b22 6669 656c 6473  1.info()["fields
+0000b3c0: 225d 0a20 2020 2020 2020 206e 756d 5f66  "].        num_f
+0000b3d0: 6965 6c64 7320 3d20 6c65 6e28 6669 656c  ields = len(fiel
+0000b3e0: 645f 6e61 6d65 7329 0a20 2020 2020 2020  d_names).       
+0000b3f0: 2074 315f 7374 6174 7320 3d20 7365 6c66   t1_stats = self
+0000b400: 2e74 312e 7374 6174 7328 292e 7365 6c65  .t1.stats().sele
+0000b410: 6374 2822 6e61 6d65 2063 6f75 6e74 206d  ct("name count m
+0000b420: 696e 206d 6178 206d 6561 6e22 290a 2020  in max mean").  
+0000b430: 2020 2020 2020 666f 7220 6669 656c 646e        for fieldn
+0000b440: 616d 6520 696e 2066 6965 6c64 5f6e 616d  ame in field_nam
+0000b450: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000b460: 7374 6174 5f72 6563 203d 2074 315f 7374  stat_rec = t1_st
+0000b470: 6174 732e 6279 2e6e 616d 655b 6669 656c  ats.by.name[fiel
+0000b480: 646e 616d 655d 0a20 2020 2020 2020 2020  dname].         
+0000b490: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b4a0: 5465 7374 2822 6368 6563 6b20 636f 6d70  Test("check comp
+0000b4b0: 7574 6564 2073 7461 7422 2c20 6669 656c  uted stat", fiel
+0000b4c0: 646e 616d 653d 6669 656c 646e 616d 6529  dname=fieldname)
+0000b4d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b4e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000b4f0: 616c 286c 742e 4461 7461 4f62 6a65 6374  al(lt.DataObject
+0000b500: 286e 616d 653d 6669 656c 646e 616d 652c  (name=fieldname,
+0000b510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 636f 756e 743d 7365 6c66 2e74 6573 745f  count=self.test_
+0000b550: 7369 7a65 202a 2a20 6e75 6d5f 6669 656c  size ** num_fiel
+0000b560: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b590: 2020 206d 696e 3d30 2c0a 2020 2020 2020     min=0,.      
+0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 206d 6178 3d73 656c           max=sel
+0000b5d0: 662e 7465 7374 5f73 697a 6520 2d20 312c  f.test_size - 1,
+0000b5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 6d65 616e 3d28 7365 6c66 2e74 6573 745f  mean=(self.test_
+0000b620: 7369 7a65 202d 2031 2920 2f20 3229 2c0a  size - 1) / 2),.
+0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2073 7461 745f 7265 632c 0a20 2020 2020   stat_rec,.     
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
+0000b680: 7661 6c69 6420 7374 6174 2066 6f72 207b  valid stat for {
+0000b690: 6669 656c 646e 616d 657d 2229 0a0a 2020  fieldname}")..  
+0000b6a0: 2020 6465 6620 7465 7374 5f73 7461 7473    def test_stats
+0000b6b0: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
+0000b6c0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
+0000b6d0: 2829 0a20 2020 2020 2020 2066 6965 6c64  ().        field
+0000b6e0: 5f6e 616d 6573 203d 2073 656c 662e 7431  _names = self.t1
+0000b6f0: 2e69 6e66 6f28 295b 2266 6965 6c64 7322  .info()["fields"
+0000b700: 5d0a 2020 2020 2020 2020 6e75 6d5f 6669  ].        num_fi
+0000b710: 656c 6473 203d 206c 656e 2866 6965 6c64  elds = len(field
+0000b720: 5f6e 616d 6573 290a 2020 2020 2020 2020  _names).        
+0000b730: 7431 5f73 7461 7473 203d 2073 656c 662e  t1_stats = self.
+0000b740: 7431 2e73 7461 7473 2862 795f 6669 656c  t1.stats(by_fiel
+0000b750: 643d 4661 6c73 6529 0a20 2020 2020 2020  d=False).       
+0000b760: 2066 6f72 2073 7461 742c 2076 616c 7565   for stat, value
+0000b770: 2069 6e20 2828 276d 696e 272c 2030 292c   in (('min', 0),
+0000b780: 2028 276d 6178 272c 2073 656c 662e 7465   ('max', self.te
+0000b790: 7374 5f73 697a 6520 2d20 3129 2c20 2827  st_size - 1), ('
+0000b7a0: 636f 756e 7427 2c20 7365 6c66 2e74 6573  count', self.tes
+0000b7b0: 745f 7369 7a65 202a 2a20 6e75 6d5f 6669  t_size ** num_fi
+0000b7c0: 656c 6473 292c 293a 0a20 2020 2020 2020  elds),):.       
+0000b7d0: 2020 2020 2066 6f72 2066 6965 6c64 6e61       for fieldna
+0000b7e0: 6d65 2069 6e20 6669 656c 645f 6e61 6d65  me in field_name
+0000b7f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000b800: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b810: 5465 7374 2822 6368 6563 6b20 636f 6d70  Test("check comp
+0000b820: 7574 6564 2073 7461 7422 2c20 7374 6174  uted stat", stat
+0000b830: 3d73 7461 742c 2066 6965 6c64 6e61 6d65  =stat, fieldname
+0000b840: 3d66 6965 6c64 6e61 6d65 293a 0a20 2020  =fieldname):.   
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000b870: 6c28 7661 6c75 652c 2067 6574 6174 7472  l(value, getattr
+0000b880: 2874 315f 7374 6174 732e 6279 2e73 7461  (t1_stats.by.sta
+0000b890: 745b 7374 6174 5d2c 2066 6965 6c64 6e61  t[stat], fieldna
+0000b8a0: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
+0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8c0: 2020 2020 2020 6622 696e 7661 6c69 6420        f"invalid 
+0000b8d0: 7b73 7461 747d 2073 7461 7420 666f 7220  {stat} stat for 
+0000b8e0: 7b66 6965 6c64 6e61 6d65 7d22 290a 0a20  {fieldname}").. 
+0000b8f0: 2020 2064 6566 2074 6573 745f 7374 6174     def test_stat
+0000b900: 7333 2873 656c 6629 3a0a 2020 2020 2020  s3(self):.      
+0000b910: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+0000b920: 7428 290a 2020 2020 2020 2020 6669 656c  t().        fiel
+0000b930: 645f 6e61 6d65 7320 3d20 7365 6c66 2e74  d_names = self.t
+0000b940: 312e 696e 666f 2829 5b22 6669 656c 6473  1.info()["fields
+0000b950: 225d 0a20 2020 2020 2020 206e 756d 5f66  "].        num_f
+0000b960: 6965 6c64 7320 3d20 6c65 6e28 6669 656c  ields = len(fiel
+0000b970: 645f 6e61 6d65 7329 0a0a 2020 2020 2020  d_names)..      
+0000b980: 2020 2320 7665 7269 6679 2074 6861 7420    # verify that 
+0000b990: 7374 6174 7320 6361 6e20 2273 7465 7020  stats can "step 
+0000b9a0: 6f76 6572 2220 6e6f 6e2d 6e75 6d65 7269  over" non-numeri
+0000b9b0: 6320 6461 7461 0a20 2020 2020 2020 2074  c data.        t
+0000b9c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000b9d0: 7365 6c66 2e74 315b 305d 2e61 203d 2022  self.t1[0].a = "
+0000b9e0: 6e6f 7420 6120 6e75 6d62 6572 220a 2020  not a number".  
+0000b9f0: 2020 2020 2020 6578 6365 7074 2028 4174        except (At
+0000ba00: 7472 6962 7574 6545 7272 6f72 2c20 5479  tributeError, Ty
+0000ba10: 7065 4572 726f 7229 3a0a 2020 2020 2020  peError):.      
+0000ba20: 2020 2020 2020 2320 736f 6d65 2074 6573        # some tes
+0000ba30: 7420 7479 7065 7320 6172 656e 2774 206d  t types aren't m
+0000ba40: 7574 6162 6c65 2c20 6d75 7374 2072 6570  utable, must rep
+0000ba50: 6c61 6365 2072 6563 2077 6974 6820 6120  lace rec with a 
+0000ba60: 6d6f 6469 6669 6564 206f 6e65 0a20 2020  modified one.   
+0000ba70: 2020 2020 2020 2020 206d 6f64 5f72 6563           mod_rec
+0000ba80: 203d 2073 656c 662e 7431 2e70 6f70 2830   = self.t1.pop(0
+0000ba90: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000baa0: 635f 7479 7065 203d 2074 7970 6528 6d6f  c_type = type(mo
+0000bab0: 645f 7265 6329 0a20 2020 2020 2020 2020  d_rec).         
+0000bac0: 2020 206e 6577 5f72 6563 5f64 6963 7420     new_rec_dict 
+0000bad0: 3d20 6c74 2e5f 746f 5f64 6963 7428 6d6f  = lt._to_dict(mo
+0000bae0: 645f 7265 6329 0a20 2020 2020 2020 2020  d_rec).         
+0000baf0: 2020 206e 6577 5f72 6563 5f64 6963 745b     new_rec_dict[
+0000bb00: 2761 275d 203d 2022 6e6f 7420 6120 6e75  'a'] = "not a nu
+0000bb10: 6d62 6572 220a 2020 2020 2020 2020 2020  mber".          
+0000bb20: 2020 6e65 775f 7265 6320 3d20 7265 635f    new_rec = rec_
+0000bb30: 7479 7065 282a 2a6e 6577 5f72 6563 5f64  type(**new_rec_d
+0000bb40: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
+0000bb50: 2073 656c 662e 7431 2e69 6e73 6572 7428   self.t1.insert(
+0000bb60: 6e65 775f 7265 6329 0a0a 2020 2020 2020  new_rec)..      
+0000bb70: 2020 7431 5f73 7461 7473 203d 2073 656c    t1_stats = sel
+0000bb80: 662e 7431 2e73 7461 7473 2829 0a20 2020  f.t1.stats().   
+0000bb90: 2020 2020 2074 315f 7374 6174 7328 2274       t1_stats("t
+0000bba0: 315f 7374 6174 7322 290a 2020 2020 2020  1_stats").      
+0000bbb0: 2020 7431 5f73 7461 7473 2e63 7376 5f65    t1_stats.csv_e
+0000bbc0: 7870 6f72 7428 7379 732e 7374 646f 7574  xport(sys.stdout
+0000bbd0: 290a 2020 2020 2020 2020 7431 5f73 7461  ).        t1_sta
+0000bbe0: 7473 2e70 7265 7365 6e74 2829 0a20 2020  ts.present().   
+0000bbf0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000bc00: 4571 7561 6c28 7365 6c66 2e74 6573 745f  Equal(self.test_
+0000bc10: 7369 7a65 202a 2a20 6e75 6d5f 6669 656c  size ** num_fiel
+0000bc20: 6473 202d 2031 2c20 7431 5f73 7461 7473  ds - 1, t1_stats
+0000bc30: 2e62 792e 6e61 6d65 5b22 6122 5d2e 636f  .by.name["a"].co
+0000bc40: 756e 7429 0a0a 2020 2020 6465 6620 7465  unt)..    def te
+0000bc50: 7374 5f73 7461 7473 3428 7365 6c66 293a  st_stats4(self):
+0000bc60: 0a20 2020 2020 2020 2074 3120 3d20 6c74  .        t1 = lt
+0000bc70: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+0000bc80: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
+0000bc90: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+0000bca0: 2061 2c62 0a20 2020 2020 2020 2031 2c32   a,b.        1,2
+0000bcb0: 0a20 2020 2020 2020 2033 2c0a 2020 2020  .        3,.    
+0000bcc0: 2020 2020 352c 340a 2020 2020 2020 2020      5,4.        
+0000bcd0: 2222 2229 2c20 7472 616e 7366 6f72 6d73  """), transforms
+0000bce0: 3d7b 7d2e 6672 6f6d 6b65 7973 285b 2261  ={}.fromkeys(["a
+0000bcf0: 222c 2022 6222 5d2c 2069 6e74 2929 0a20  ", "b"], int)). 
+0000bd00: 2020 2020 2020 2074 315f 7374 6174 7320         t1_stats 
+0000bd10: 3d20 7431 2e73 7461 7473 2829 0a20 2020  = t1.stats().   
+0000bd20: 2020 2020 2074 315f 7374 6174 732e 7072       t1_stats.pr
+0000bd30: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+0000bd40: 7072 696e 7428 7431 5f73 7461 7473 2e69  print(t1_stats.i
+0000bd50: 6e66 6f28 2929 0a0a 2020 2020 2020 2020  nfo())..        
+0000bd60: 6578 7065 6374 6564 203d 206c 742e 5461  expected = lt.Ta
+0000bd70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+0000bd80: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000bd90: 2822 2222 5c0a 2020 2020 2020 2020 6e61  ("""\.        na
+0000bda0: 6d65 2c6d 6561 6e2c 6d69 6e2c 6d61 782c  me,mean,min,max,
+0000bdb0: 7661 7269 616e 6365 2c73 7464 5f64 6576  variance,std_dev
+0000bdc0: 2c63 6f75 6e74 2c6d 6973 7369 6e67 0a20  ,count,missing. 
+0000bdd0: 2020 2020 2020 2061 2c33 2e30 2c31 2c35         a,3.0,1,5
+0000bde0: 2c34 2c32 2e30 2c33 2c30 0a20 2020 2020  ,4,2.0,3,0.     
+0000bdf0: 2020 2062 2c33 2e30 2c32 2c34 2c32 2c31     b,3.0,2,4,2,1
+0000be00: 2e34 3134 2c32 2c31 0a20 2020 2020 2020  .414,2,1.       
+0000be10: 2022 2222 292c 2074 7261 6e73 666f 726d   """), transform
+0000be20: 733d 7b7d 2e66 726f 6d6b 6579 7328 226d  s={}.fromkeys("m
+0000be30: 6561 6e20 6d69 6e20 6d61 7820 7661 7269  ean min max vari
+0000be40: 616e 6365 2073 7464 5f64 6576 2063 6f75  ance std_dev cou
+0000be50: 6e74 206d 6973 7369 6e67 222e 7370 6c69  nt missing".spli
+0000be60: 7428 292c 2061 7374 2e6c 6974 6572 616c  t(), ast.literal
+0000be70: 5f65 7661 6c29 290a 2020 2020 2020 2020  _eval)).        
+0000be80: 6578 7065 6374 6564 2e70 7265 7365 6e74  expected.present
+0000be90: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
+0000bea0: 2865 7870 6563 7465 642e 696e 666f 2829  (expected.info()
+0000beb0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+0000bec0: 7365 6c66 2e73 7562 5465 7374 2822 6368  self.subTest("ch
+0000bed0: 6563 6b20 636f 6d70 7574 6564 2073 7461  eck computed sta
+0000bee0: 7420 6669 656c 6473 2229 3a0a 2020 2020  t fields"):.    
+0000bef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000bf00: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0000bf10: 642e 696e 666f 2829 5b22 6669 656c 6473  d.info()["fields
+0000bf20: 225d 2c20 7431 5f73 7461 7473 2e69 6e66  "], t1_stats.inf
+0000bf30: 6f28 295b 2266 6965 6c64 7322 5d29 0a0a  o()["fields"])..
+0000bf40: 2020 2020 2020 2020 666f 7220 6578 7065          for expe
+0000bf50: 6374 6564 5f72 6f77 2c20 726f 7720 696e  cted_row, row in
+0000bf60: 207a 6970 2865 7870 6563 7465 642c 2074   zip(expected, t
+0000bf70: 315f 7374 6174 7329 3a0a 2020 2020 2020  1_stats):.      
+0000bf80: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000bf90: 7375 6254 6573 7428 2263 6865 636b 2063  subTest("check c
+0000bfa0: 6f6d 7075 7465 6420 7374 6174 2061 7474  omputed stat att
+0000bfb0: 7269 6275 7465 2028 6e61 6d65 2922 2c20  ribute (name)", 
+0000bfc0: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
+0000bfd0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000bfe0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000bff0: 7465 645f 726f 772e 6e61 6d65 2c20 726f  ted_row.name, ro
+0000c000: 772e 6e61 6d65 290a 2020 2020 2020 2020  w.name).        
+0000c010: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000c020: 6254 6573 7428 2263 6865 636b 2063 6f6d  bTest("check com
+0000c030: 7075 7465 6420 7374 6174 2061 7474 7269  puted stat attri
+0000c040: 6275 7465 2028 6d65 616e 2922 2c20 726f  bute (mean)", ro
+0000c050: 773d 726f 7729 3a0a 2020 2020 2020 2020  w=row):.        
+0000c060: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c070: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0000c080: 645f 726f 772e 6d65 616e 2c20 726f 772e  d_row.mean, row.
+0000c090: 6d65 616e 290a 2020 2020 2020 2020 2020  mean).          
+0000c0a0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000c0b0: 6573 7428 2263 6865 636b 2063 6f6d 7075  est("check compu
+0000c0c0: 7465 6420 7374 6174 2061 7474 7269 6275  ted stat attribu
+0000c0d0: 7465 2028 6d69 6e29 222c 2072 6f77 3d72  te (min)", row=r
+0000c0e0: 6f77 293a 0a20 2020 2020 2020 2020 2020  ow):.           
+0000c0f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c100: 4571 7561 6c28 6578 7065 6374 6564 5f72  Equal(expected_r
+0000c110: 6f77 2e6d 696e 2c20 726f 772e 6d69 6e29  ow.min, row.min)
+0000c120: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000c130: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+0000c140: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
+0000c150: 7461 7420 6174 7472 6962 7574 6520 286d  tat attribute (m
+0000c160: 6178 2922 2c20 726f 773d 726f 7729 3a0a  ax)", row=row):.
+0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c180: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000c190: 2865 7870 6563 7465 645f 726f 772e 6d61  (expected_row.ma
+0000c1a0: 782c 2072 6f77 2e6d 6178 290a 2020 2020  x, row.max).    
+0000c1b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000c1c0: 662e 7375 6254 6573 7428 2263 6865 636b  f.subTest("check
+0000c1d0: 2063 6f6d 7075 7465 6420 7374 6174 2061   computed stat a
+0000c1e0: 7474 7269 6275 7465 2028 7661 7269 616e  ttribute (varian
+0000c1f0: 6365 2922 2c20 726f 773d 726f 7729 3a0a  ce)", row=row):.
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c210: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000c220: 2865 7870 6563 7465 645f 726f 772e 7661  (expected_row.va
+0000c230: 7269 616e 6365 2c20 726f 772e 7661 7269  riance, row.vari
+0000c240: 616e 6365 290a 2020 2020 2020 2020 2020  ance).          
+0000c250: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000c260: 6573 7428 2263 6865 636b 2063 6f6d 7075  est("check compu
+0000c270: 7465 6420 7374 6174 2061 7474 7269 6275  ted stat attribu
+0000c280: 7465 2028 7374 645f 6465 7629 222c 2072  te (std_dev)", r
+0000c290: 6f77 3d72 6f77 293a 0a20 2020 2020 2020  ow=row):.       
+0000c2a0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000c2b0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
+0000c2c0: 6564 5f72 6f77 2e73 7464 5f64 6576 2c20  ed_row.std_dev, 
+0000c2d0: 726f 772e 7374 645f 6465 7629 0a20 2020  row.std_dev).   
+0000c2e0: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+0000c2f0: 6c66 2e73 7562 5465 7374 2822 6368 6563  lf.subTest("chec
+0000c300: 6b20 636f 6d70 7574 6564 2073 7461 7420  k computed stat 
+0000c310: 6174 7472 6962 7574 6520 2863 6f75 6e74  attribute (count
+0000c320: 2922 2c20 726f 773d 726f 7729 3a0a 2020  )", row=row):.  
+0000c330: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c340: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+0000c350: 7870 6563 7465 645f 726f 772e 636f 756e  xpected_row.coun
+0000c360: 742c 2072 6f77 2e63 6f75 6e74 290a 2020  t, row.count).  
+0000c370: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000c380: 656c 662e 7375 6254 6573 7428 2263 6865  elf.subTest("che
+0000c390: 636b 2063 6f6d 7075 7465 6420 7374 6174  ck computed stat
+0000c3a0: 2061 7474 7269 6275 7465 2028 6d69 7373   attribute (miss
+0000c3b0: 696e 6729 222c 2072 6f77 3d72 6f77 293a  ing)", row=row):
+0000c3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c3d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000c3e0: 6c28 6578 7065 6374 6564 5f72 6f77 2e6d  l(expected_row.m
+0000c3f0: 6973 7369 6e67 2c20 726f 772e 6d69 7373  issing, row.miss
+0000c400: 696e 6729 0a0a 2020 2020 6465 6620 7465  ing)..    def te
+0000c410: 7374 5f73 706c 6974 6279 2873 656c 6629  st_splitby(self)
+0000c420: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000c430: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
+0000c440: 2020 2020 6973 5f6f 6464 203d 206c 616d      is_odd = lam
+0000c450: 6264 6120 7265 633a 2072 6563 2e61 2025  bda rec: rec.a %
+0000c460: 2032 0a20 2020 2020 2020 2065 7665 6e73   2.        evens
+0000c470: 2c20 6f64 6473 203d 2073 656c 662e 7431  , odds = self.t1
+0000c480: 2e73 706c 6974 6279 2869 735f 6f64 6429  .splitby(is_odd)
+0000c490: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000c4a0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000c4b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c4c0: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+0000c4d0: 6464 7329 202b 206c 656e 2865 7665 6e73  dds) + len(evens
+0000c4e0: 292c 206c 656e 2873 656c 662e 7431 2929  ), len(self.t1))
+0000c4f0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000c500: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000c510: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c520: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+0000c530: 6464 7329 2c20 6c65 6e28 7365 6c66 2e74  dds), len(self.t
+0000c540: 312e 7768 6572 6528 6973 5f6f 6464 2929  1.where(is_odd))
+0000c550: 290a 0a20 2020 2020 2020 2065 7665 6e5f  )..        even_
+0000c560: 6576 656e 732c 206f 6464 5f65 7665 6e73  evens, odd_evens
+0000c570: 203d 2065 7665 6e73 2e73 706c 6974 6279   = evens.splitby
+0000c580: 2869 735f 6f64 6429 0a20 2020 2020 2020  (is_odd).       
+0000c590: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000c5a0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000c5b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000c5c0: 616c 2830 2c20 6c65 6e28 6f64 645f 6576  al(0, len(odd_ev
+0000c5d0: 656e 7329 290a 2020 2020 2020 2020 7769  ens)).        wi
+0000c5e0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000c5f0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000c600: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000c610: 6c65 6e28 6576 656e 5f65 7665 6e73 292c  len(even_evens),
+0000c620: 206c 656e 2865 7665 6e73 2929 0a0a 2020   len(evens))..  
+0000c630: 2020 2020 2020 2320 6d61 6b65 2073 7572        # make sur
+0000c640: 6520 696e 6465 7865 7320 6172 6520 7072  e indexes are pr
+0000c650: 6573 6572 7665 640a 2020 2020 2020 2020  eserved.        
+0000c660: 7365 6c66 2e74 312e 6372 6561 7465 5f69  self.t1.create_i
+0000c670: 6e64 6578 2822 6122 290a 2020 2020 2020  ndex("a").      
+0000c680: 2020 6576 656e 732c 206f 6464 7320 3d20    evens, odds = 
+0000c690: 7365 6c66 2e74 312e 7370 6c69 7462 7928  self.t1.splitby(
+0000c6a0: 6973 5f6f 6464 290a 2020 2020 2020 2020  is_odd).        
+0000c6b0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000c6c0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000c6d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000c6e0: 6c28 7365 6c66 2e74 312e 696e 666f 2829  l(self.t1.info()
+0000c6f0: 5b22 696e 6465 7865 7322 5d2c 2065 7665  ["indexes"], eve
+0000c700: 6e73 2e69 6e66 6f28 295b 2269 6e64 6578  ns.info()["index
+0000c710: 6573 225d 290a 0a20 2020 2020 2020 2023  es"])..        #
+0000c720: 2074 6573 7420 7061 7373 696e 6720 616e   test passing an
+0000c730: 2061 7474 7269 6275 7465 2061 7320 6120   attribute as a 
+0000c740: 6b65 790a 2020 2020 2020 2020 7a65 726f  key.        zero
+0000c750: 732c 206e 6f6e 5f7a 6572 6f73 203d 2073  s, non_zeros = s
+0000c760: 656c 662e 7431 2e73 706c 6974 6279 2822  elf.t1.splitby("
+0000c770: 6122 290a 2020 2020 2020 2020 7769 7468  a").        with
+0000c780: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000c790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c7a0: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
+0000c7b0: 2872 6563 2e61 203d 3d20 3020 666f 7220  (rec.a == 0 for 
+0000c7c0: 7265 6320 696e 207a 6572 6f73 2929 0a20  rec in zeros)). 
+0000c7d0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000c7e0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000c7f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c800: 6572 7454 7275 6528 616c 6c28 7265 632e  ertTrue(all(rec.
+0000c810: 6120 213d 2030 2066 6f72 2072 6563 2069  a != 0 for rec i
+0000c820: 6e20 6e6f 6e5f 7a65 726f 7329 290a 0a20  n non_zeros)).. 
+0000c830: 2020 2020 2020 2023 2074 6573 7420 7573         # test us
+0000c840: 696e 6720 7072 6564 6963 6174 6520 7468  ing predicate th
+0000c850: 6174 2064 6f65 7320 6e6f 7420 616c 7761  at does not alwa
+0000c860: 7973 2072 6574 7572 6e20 3020 6f72 2031  ys return 0 or 1
+0000c870: 0a20 2020 2020 2020 2069 735f 6e6f 745f  .        is_not_
+0000c880: 6d75 6c74 6970 6c65 5f6f 665f 3320 3d20  multiple_of_3 = 
+0000c890: 6c61 6d62 6461 2072 6563 3a20 7265 632e  lambda rec: rec.
+0000c8a0: 6120 2520 330a 2020 2020 2020 2020 6d75  a % 3.        mu
+0000c8b0: 6c74 735f 6f66 5f33 2c20 6e6f 6e5f 6d75  lts_of_3, non_mu
+0000c8c0: 6c74 735f 6f66 5f33 203d 2073 656c 662e  lts_of_3 = self.
+0000c8d0: 7431 2e73 706c 6974 6279 2869 735f 6e6f  t1.splitby(is_no
+0000c8e0: 745f 6d75 6c74 6970 6c65 5f6f 665f 3329  t_multiple_of_3)
+0000c8f0: 0a20 2020 2020 2020 2070 7269 6e74 286c  .        print(l
+0000c900: 6973 7428 6e6f 6e5f 6d75 6c74 735f 6f66  ist(non_mults_of
+0000c910: 5f33 2e61 6c6c 2e61 2929 0a20 2020 2020  _3.all.a)).     
+0000c920: 2020 2070 7269 6e74 286c 6973 7428 6d75     print(list(mu
+0000c930: 6c74 735f 6f66 5f33 2e61 6c6c 2e61 2929  lts_of_3.all.a))
+0000c940: 0a20 2020 2020 2020 2023 2054 4f44 4f20  .        # TODO 
+0000c950: 2d20 6164 6420 6173 7365 7274 7320 6865  - add asserts he
+0000c960: 7265 0a0a 0a40 6d61 6b65 5f74 6573 745f  re...@make_test_
+0000c970: 636c 6173 7365 730a 636c 6173 7320 5461  classes.class Ta
+0000c980: 626c 654a 6f69 6e54 6573 7473 3a0a 2020  bleJoinTests:.  
+0000c990: 2020 2222 220a 2020 2020 5465 7374 7320    """.    Tests 
+0000c9a0: 666f 7220 5461 626c 6520 6a6f 696e 206f  for Table join o
+0000c9b0: 7065 7261 7469 6f6e 732e 0a20 2020 2022  perations..    "
+0000c9c0: 2222 0a20 2020 2064 6566 2074 6573 745f  "".    def test_
+0000c9d0: 7369 6d70 6c65 5f6a 6f69 6e28 7365 6c66  simple_join(self
+0000c9e0: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+0000c9f0: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+0000ca00: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+0000ca10: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+0000ca20: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+0000ca30: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
+0000ca40: 2074 312e 6372 6561 7465 5f69 6e64 6578   t1.create_index
+0000ca50: 2827 6127 290a 0a20 2020 2020 2020 2074  ('a')..        t
+0000ca60: 3220 3d20 6c74 2e54 6162 6c65 2829 0a20  2 = lt.Table(). 
+0000ca70: 2020 2020 2020 2074 322e 6372 6561 7465         t2.create
+0000ca80: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
+0000ca90: 2020 2020 7432 2e69 6e73 6572 7428 6c74      t2.insert(lt
+0000caa0: 2e44 6174 614f 626a 6563 7428 613d 312c  .DataObject(a=1,
+0000cab0: 2064 3d31 3030 2929 0a0a 2020 2020 2020   d=100))..      
+0000cac0: 2020 6a6f 696e 6564 203d 2028 7431 2e6a    joined = (t1.j
+0000cad0: 6f69 6e5f 6f6e 2827 6127 2920 2b20 7432  oin_on('a') + t2
+0000cae0: 2e6a 6f69 6e5f 6f6e 2827 6127 2929 2829  .join_on('a'))()
+0000caf0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000cb00: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000cb10: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000cb20: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+0000cb30: 7369 7a65 202a 2074 6573 745f 7369 7a65  size * test_size
+0000cb40: 2c20 6c65 6e28 6a6f 696e 6564 2929 0a0a  , len(joined))..
+0000cb50: 2020 2020 2020 2020 6a6f 696e 6564 203d          joined =
+0000cb60: 2028 7431 2e6a 6f69 6e5f 6f6e 2827 6127   (t1.join_on('a'
+0000cb70: 2920 2b20 7432 2928 290a 2020 2020 2020  ) + t2)().      
+0000cb80: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000cb90: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000cba0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000cbb0: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
+0000cbc0: 7465 7374 5f73 697a 652c 206c 656e 286a  test_size, len(j
+0000cbd0: 6f69 6e65 6429 290a 0a20 2020 2020 2020  oined))..       
+0000cbe0: 206a 6f69 6e65 6420 3d20 2874 3120 2b20   joined = (t1 + 
+0000cbf0: 7432 2e6a 6f69 6e5f 6f6e 2827 6127 2929  t2.join_on('a'))
+0000cc00: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
+0000cc10: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000cc20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cc30: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+0000cc40: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
+0000cc50: 7a65 2c20 6c65 6e28 6a6f 696e 6564 2929  ze, len(joined))
+0000cc60: 0a0a 2020 2020 2020 2020 7431 2e64 726f  ..        t1.dro
+0000cc70: 705f 696e 6465 7828 2761 2729 0a20 2020  p_index('a').   
+0000cc80: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000cc90: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000cca0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000ccb0: 6173 7365 7274 5261 6973 6573 2856 616c  assertRaises(Val
+0000ccc0: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
+0000ccd0: 2020 2020 2020 2020 2020 6a6f 696e 6564            joined
+0000cce0: 203d 2028 7431 202b 2074 322e 6a6f 696e   = (t1 + t2.join
+0000ccf0: 5f6f 6e28 2761 2729 2928 290a 0a20 2020  _on('a'))()..   
+0000cd00: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000cd10: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000cd20: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000cd30: 6173 7365 7274 5261 6973 6573 2854 7970  assertRaises(Typ
+0000cd40: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+0000cd50: 2020 2020 2020 2020 2023 2069 6e76 616c           # inval
+0000cd60: 6964 206a 6f69 6e2c 206e 6f20 6b77 6172  id join, no kwar
+0000cd70: 6773 206c 6973 7469 6e67 2061 7474 7269  gs listing attri
+0000cd80: 6275 7465 7320 746f 206a 6f69 6e20 6f6e  butes to join on
+0000cd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cda0: 2074 3320 3d20 7431 2e6a 6f69 6e28 7432   t3 = t1.join(t2
+0000cdb0: 2c20 2761 2c64 2729 0a0a 2020 2020 2020  , 'a,d')..      
+0000cdc0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000cdd0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000cde0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+0000cdf0: 6572 7452 6169 7365 7328 5661 6c75 6545  ertRaises(ValueE
+0000ce00: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+0000ce10: 2020 2020 2020 2023 2069 6e76 616c 6964         # invalid
+0000ce20: 206a 6f69 6e2c 206e 6f20 7375 6368 2061   join, no such a
+0000ce30: 7474 7269 6275 7465 2027 7a27 0a20 2020  ttribute 'z'.   
+0000ce40: 2020 2020 2020 2020 2020 2020 2074 3320               t3 
+0000ce50: 3d20 7431 2e6a 6f69 6e28 7432 2c20 2761  = t1.join(t2, 'a
+0000ce60: 2c64 2c7a 272c 2061 3d27 6127 290a 0a20  ,d,z', a='a').. 
+0000ce70: 2020 2020 2020 2074 3320 3d20 7431 2e6a         t3 = t1.j
+0000ce80: 6f69 6e28 7432 2c20 2761 2c64 272c 2061  oin(t2, 'a,d', a
+0000ce90: 3d27 6127 290a 2020 2020 2020 2020 7769  ='a').        wi
+0000cea0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000ceb0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000cec0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000ced0: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+0000cee0: 5f73 697a 652c 206c 656e 2874 3329 290a  _size, len(t3)).
+0000cef0: 0a20 2020 2020 2020 2074 3420 3d20 7431  .        t4 = t1
+0000cf00: 2e6a 6f69 6e28 7432 2c20 613d 2761 2729  .join(t2, a='a')
+0000cf10: 2e73 656c 6563 7428 2761 2063 2064 272c  .select('a c d',
+0000cf20: 2065 3d6c 616d 6264 6120 7265 633a 2072   e=lambda rec: r
+0000cf30: 6563 2e61 202b 2072 6563 2e63 202b 2072  ec.a + rec.c + r
+0000cf40: 6563 2e64 290a 2020 2020 2020 2020 7769  ec.d).        wi
+0000cf50: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000cf60: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000cf70: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+0000cf80: 6c6c 2872 6563 2e65 203d 3d20 7265 632e  ll(rec.e == rec.
+0000cf90: 612b 7265 632e 632b 7265 632e 6420 666f  a+rec.c+rec.d fo
+0000cfa0: 7220 7265 6320 696e 2074 3429 290a 0a20  r rec in t4)).. 
+0000cfb0: 2020 2020 2020 2023 206a 6f69 6e20 746f         # join to
+0000cfc0: 2065 6d70 7479 206c 6973 742c 2073 686f   empty list, sho
+0000cfd0: 756c 6420 7265 7475 726e 2065 6d70 7479  uld return empty
+0000cfe0: 2074 6162 6c65 0a20 2020 2020 2020 2065   table.        e
+0000cff0: 6d70 7479 5f74 6162 6c65 203d 206c 742e  mpty_table = lt.
+0000d000: 5461 626c 6528 290a 2020 2020 2020 2020  Table().        
+0000d010: 656d 7074 795f 7461 626c 652e 6372 6561  empty_table.crea
+0000d020: 7465 5f69 6e64 6578 2827 6127 290a 2020  te_index('a').  
+0000d030: 2020 2020 2020 7435 203d 2028 7431 2e6a        t5 = (t1.j
+0000d040: 6f69 6e5f 6f6e 2827 6127 2920 2b20 656d  oin_on('a') + em
+0000d050: 7074 795f 7461 626c 6529 2829 0a20 2020  pty_table)().   
+0000d060: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000d070: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000d080: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000d090: 7445 7175 616c 2830 2c20 6c65 6e28 7435  tEqual(0, len(t5
+0000d0a0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+0000d0b0: 5f6f 7574 6572 5f6a 6f69 6e73 2873 656c  _outer_joins(sel
+0000d0c0: 6629 3a0a 2020 2020 2020 2020 7431 203d  f):.        t1 =
+0000d0d0: 206c 742e 5461 626c 6528 2263 6174 616c   lt.Table("catal
+0000d0e0: 6f67 2229 0a20 2020 2020 2020 2074 312e  og").        t1.
+0000d0f0: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
+0000d100: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000d110: 2020 2020 2020 2020 2020 2020 736b 752c              sku,
+0000d120: 636f 6c6f 722c 7369 7a65 2c6d 6174 6572  color,size,mater
+0000d130: 6961 6c0a 2020 2020 2020 2020 2020 2020  ial.            
+0000d140: 3030 312c 7265 642c 584c 2c63 6f74 746f  001,red,XL,cotto
+0000d150: 6e0a 2020 2020 2020 2020 2020 2020 3030  n.            00
+0000d160: 322c 626c 7565 2c58 4c2c 636f 7474 6f6e  2,blue,XL,cotton
+0000d170: 2f70 6f6c 790a 2020 2020 2020 2020 2020  /poly.          
+0000d180: 2020 3030 332c 626c 7565 2c4c 2c6c 696e    003,blue,L,lin
+0000d190: 656e 0a20 2020 2020 2020 2020 2020 2030  en.            0
+0000d1a0: 3034 2c72 6564 2c4d 2c63 6f74 746f 6e0a  04,red,M,cotton.
+0000d1b0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000d1c0: 290a 0a20 2020 2020 2020 2074 3220 3d20  )..        t2 = 
+0000d1d0: 6c74 2e54 6162 6c65 2822 7072 6963 6573  lt.Table("prices
+0000d1e0: 2229 0a20 2020 2020 2020 2074 322e 6373  ").        t2.cs
+0000d1f0: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
+0000d200: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000d210: 2020 2020 2020 2020 2020 736b 752c 756e            sku,un
+0000d220: 6974 5f70 7269 6365 2c73 697a 650a 2020  it_price,size.  
+0000d230: 2020 2020 2020 2020 2020 3030 312c 3130            001,10
+0000d240: 2c4c 0a20 2020 2020 2020 2020 2020 2030  ,L.            0
+0000d250: 3031 2c31 322c 584c 0a20 2020 2020 2020  01,12,XL.       
+0000d260: 2020 2020 2030 3032 2c31 312c 0a20 2020       002,11,.   
+0000d270: 2020 2020 2020 2020 2030 3034 2c39 2c0a           004,9,.
+0000d280: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000d290: 2c20 7472 616e 7366 6f72 6d73 3d7b 2773  , transforms={'s
+0000d2a0: 697a 6527 3a20 6c61 6d62 6461 2078 3a20  ize': lambda x: 
+0000d2b0: 7820 6f72 204e 6f6e 657d 290a 2020 2020  x or None}).    
+0000d2c0: 2020 2020 7072 696e 7428 7431 2e69 6e66      print(t1.inf
+0000d2d0: 6f28 2929 0a0a 2020 2020 2020 2020 7431  o())..        t1
+0000d2e0: 2e70 7265 7365 6e74 2829 0a20 2020 2020  .present().     
+0000d2f0: 2020 2074 322e 7072 6573 656e 7428 290a     t2.present().
+0000d300: 0a20 2020 2020 2020 2074 3320 3d20 7431  .        t3 = t1
+0000d310: 2e6a 6f69 6e28 7432 2c20 6175 746f 5f63  .join(t2, auto_c
+0000d320: 7265 6174 655f 696e 6465 7865 733d 5472  reate_indexes=Tr
+0000d330: 7565 2c20 736b 753d 2273 6b75 2229 0a20  ue, sku="sku"). 
+0000d340: 2020 2020 2020 2070 7269 6e74 2874 332e         print(t3.
+0000d350: 696e 666f 2829 290a 2020 2020 2020 2020  info()).        
+0000d360: 7433 2e70 7265 7365 6e74 2829 0a20 2020  t3.present().   
+0000d370: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000d380: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000d390: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000d3a0: 7445 7175 616c 2834 2c20 6c65 6e28 7433  tEqual(4, len(t3
+0000d3b0: 2929 0a0a 2020 2020 2020 2020 7433 203d  ))..        t3 =
+0000d3c0: 2074 312e 6a6f 696e 2874 322c 2061 7574   t1.join(t2, aut
+0000d3d0: 6f5f 6372 6561 7465 5f69 6e64 6578 6573  o_create_indexes
+0000d3e0: 3d54 7275 652c 2073 6b75 3d22 736b 7522  =True, sku="sku"
+0000d3f0: 2c20 7369 7a65 3d22 7369 7a65 2229 0a20  , size="size"). 
+0000d400: 2020 2020 2020 2074 3328 2269 6e6e 6572         t3("inner
+0000d410: 206a 6f69 6e20 2d20 2220 2b20 7433 2e74   join - " + t3.t
+0000d420: 6162 6c65 5f6e 616d 6529 0a20 2020 2020  able_name).     
+0000d430: 2020 2070 7269 6e74 2874 332e 696e 666f     print(t3.info
+0000d440: 2829 290a 2020 2020 2020 2020 7433 2e70  ()).        t3.p
+0000d450: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
+0000d460: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000d470: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000d480: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000d490: 616c 2831 2c20 6c65 6e28 7433 2929 0a0a  al(1, len(t3))..
+0000d4a0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
+0000d4b0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
+0000d4c0: 626c 652e 5249 4748 545f 4f55 5445 525f  ble.RIGHT_OUTER_
+0000d4d0: 4a4f 494e 2c20 7432 2c20 736b 753d 2273  JOIN, t2, sku="s
+0000d4e0: 6b75 222c 2073 697a 653d 2273 697a 6522  ku", size="size"
+0000d4f0: 290a 2020 2020 2020 2020 7433 2822 7269  ).        t3("ri
+0000d500: 6768 7420 6f75 7465 7220 6a6f 696e 202d  ght outer join -
+0000d510: 2022 202b 2074 332e 7461 626c 655f 6e61   " + t3.table_na
+0000d520: 6d65 290a 2020 2020 2020 2020 7072 696e  me).        prin
+0000d530: 7428 7433 2e69 6e66 6f28 2929 0a20 2020  t(t3.info()).   
+0000d540: 2020 2020 2074 332e 7072 6573 656e 7428       t3.present(
+0000d550: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000d560: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000d570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d580: 6173 7365 7274 4571 7561 6c28 342c 206c  assertEqual(4, l
+0000d590: 656e 2874 3329 290a 0a20 2020 2020 2020  en(t3))..       
+0000d5a0: 2074 3320 3d20 7431 2e6f 7574 6572 5f6a   t3 = t1.outer_j
+0000d5b0: 6f69 6e28 6c74 2e54 6162 6c65 2e4c 4546  oin(lt.Table.LEF
+0000d5c0: 545f 4f55 5445 525f 4a4f 494e 2c20 7432  T_OUTER_JOIN, t2
+0000d5d0: 2c20 736b 753d 2273 6b75 222c 2073 697a  , sku="sku", siz
+0000d5e0: 653d 2273 697a 6522 290a 2020 2020 2020  e="size").      
+0000d5f0: 2020 7433 2822 6c65 6674 206f 7574 6572    t3("left outer
+0000d600: 206a 6f69 6e20 2d20 2220 2b20 7433 2e74   join - " + t3.t
+0000d610: 6162 6c65 5f6e 616d 6529 0a20 2020 2020  able_name).     
+0000d620: 2020 2070 7269 6e74 2874 332e 696e 666f     print(t3.info
+0000d630: 2829 290a 2020 2020 2020 2020 7433 2e70  ()).        t3.p
+0000d640: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
+0000d650: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000d660: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000d670: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000d680: 616c 2832 2c20 6c65 6e28 7433 2929 0a0a  al(2, len(t3))..
+0000d690: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
+0000d6a0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
+0000d6b0: 626c 652e 4655 4c4c 5f4f 5554 4552 5f4a  ble.FULL_OUTER_J
+0000d6c0: 4f49 4e2c 2074 322c 2073 6b75 3d22 736b  OIN, t2, sku="sk
+0000d6d0: 7522 2c20 7369 7a65 3d22 7369 7a65 2229  u", size="size")
+0000d6e0: 0a20 2020 2020 2020 2074 3328 2266 756c  .        t3("ful
+0000d6f0: 6c20 6f75 7465 7220 6a6f 696e 202d 2022  l outer join - "
+0000d700: 202b 2074 332e 7461 626c 655f 6e61 6d65   + t3.table_name
+0000d710: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000d720: 7433 2e69 6e66 6f28 2929 0a20 2020 2020  t3.info()).     
+0000d730: 2020 2074 332e 7072 6573 656e 7428 290a     t3.present().
+0000d740: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000d750: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+0000d760: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000d770: 7365 7274 4571 7561 6c28 3132 2c20 6c65  sertEqual(12, le
+0000d780: 6e28 7433 2929 0a0a 2020 2020 6465 6620  n(t3))..    def 
+0000d790: 7465 7374 5f6f 7574 6572 5f6a 6f69 6e5f  test_outer_join_
+0000d7a0: 6578 616d 706c 6528 7365 6c66 293a 0a20  example(self):. 
+0000d7b0: 2020 2020 2020 2023 2064 6566 696e 6520         # define 
+0000d7c0: 7374 7564 656e 7420 616e 6420 7265 6769  student and regi
+0000d7d0: 7374 7261 7469 6f6e 2064 6174 610a 2020  stration data.  
+0000d7e0: 2020 2020 2020 7374 7564 656e 7473 203d        students =
+0000d7f0: 206c 742e 5461 626c 6528 2273 7475 6465   lt.Table("stude
+0000d800: 6e74 7322 292e 6373 765f 696d 706f 7274  nts").csv_import
+0000d810: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000d820: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000d830: 2020 7374 7564 656e 745f 6964 2c6e 616d    student_id,nam
+0000d840: 650a 2020 2020 2020 2020 2020 2020 3030  e.            00
+0000d850: 3031 2c41 6c69 6365 0a20 2020 2020 2020  01,Alice.       
+0000d860: 2020 2020 2030 3030 322c 426f 620a 2020       0002,Bob.  
+0000d870: 2020 2020 2020 2020 2020 3030 3033 2c43            0003,C
+0000d880: 6861 726c 6965 0a20 2020 2020 2020 2020  harlie.         
+0000d890: 2020 2030 3030 342c 4461 7665 0a20 2020     0004,Dave.   
+0000d8a0: 2020 2020 2020 2020 2030 3030 352c 456e           0005,En
+0000d8b0: 6964 0a20 2020 2020 2020 2020 2020 2022  id.            "
+0000d8c0: 2222 2929 0a0a 2020 2020 2020 2020 7265  ""))..        re
+0000d8d0: 6769 7374 7261 7469 6f6e 7320 3d20 6c74  gistrations = lt
+0000d8e0: 2e54 6162 6c65 2822 7265 6769 7374 7261  .Table("registra
+0000d8f0: 7469 6f6e 7322 292e 6373 765f 696d 706f  tions").csv_impo
+0000d900: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
+0000d910: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000d920: 2020 2020 7374 7564 656e 745f 6964 2c63      student_id,c
+0000d930: 6f75 7273 650a 2020 2020 2020 2020 2020  ourse.          
+0000d940: 2020 3030 3031 2c50 5359 4348 3130 310a    0001,PSYCH101.
+0000d950: 2020 2020 2020 2020 2020 2020 3030 3031              0001
+0000d960: 2c43 414c 4331 0a20 2020 2020 2020 2020  ,CALC1.         
+0000d970: 2020 2030 3030 332c 4249 4f32 3030 0a20     0003,BIO200. 
+0000d980: 2020 2020 2020 2020 2020 2030 3030 352c             0005,
+0000d990: 4348 454d 3130 310a 2020 2020 2020 2020  CHEM101.        
+0000d9a0: 2020 2020 3030 3036 2c50 4859 3130 310a      0006,PHY101.
+0000d9b0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000d9c0: 290a 0a20 2020 2020 2020 2063 6f75 7273  )..        cours
+0000d9d0: 6573 203d 206c 742e 5461 626c 6528 2263  es = lt.Table("c
+0000d9e0: 6f75 7273 6573 2229 2e63 7376 5f69 6d70  ourses").csv_imp
+0000d9f0: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
+0000da00: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+0000da10: 2020 2020 2063 6f75 7273 650a 2020 2020       course.    
+0000da20: 2020 2020 2020 2020 4249 4f32 3030 0a20          BIO200. 
+0000da30: 2020 2020 2020 2020 2020 2043 414c 4331             CALC1
+0000da40: 0a20 2020 2020 2020 2020 2020 2043 4845  .            CHE
+0000da50: 4d31 3031 0a20 2020 2020 2020 2020 2020  M101.           
+0000da60: 2050 5359 4348 3130 310a 2020 2020 2020   PSYCH101.      
+0000da70: 2020 2020 2020 5045 3130 310a 2020 2020        PE101.    
+0000da80: 2020 2020 2020 2020 2222 2229 290a 0a20          """)).. 
+0000da90: 2020 2020 2020 2023 2070 6572 666f 726d         # perform
+0000daa0: 206f 7574 6572 206a 6f69 6e20 616e 6420   outer join and 
+0000dab0: 7368 6f77 2072 6573 756c 7473 3a0a 2020  show results:.  
+0000dac0: 2020 2020 2020 6e6f 6e5f 7265 6720 3d20        non_reg = 
+0000dad0: 7374 7564 656e 7473 2e6f 7574 6572 5f6a  students.outer_j
+0000dae0: 6f69 6e28 6c74 2e54 6162 6c65 2e52 4947  oin(lt.Table.RIG
+0000daf0: 4854 5f4f 5554 4552 5f4a 4f49 4e2c 0a20  HT_OUTER_JOIN,. 
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 2020 2020 2072 6567 6973 7472 6174 696f       registratio
+0000db30: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 2020 2020 2020 2020 2020 7374 7564 656e            studen
+0000db60: 745f 6964 3d22 7374 7564 656e 745f 6964  t_id="student_id
+0000db70: 2229 2e77 6865 7265 2863 6f75 7273 653d  ").where(course=
+0000db80: 4e6f 6e65 290a 2020 2020 2020 2020 6e6f  None).        no
+0000db90: 6e5f 7265 672e 7072 6573 656e 7428 290a  n_reg.present().
+0000dba0: 2020 2020 2020 2020 7072 696e 7428 6c69          print(li
+0000dbb0: 7374 286e 6f6e 5f72 6567 2e61 6c6c 2e6e  st(non_reg.all.n
+0000dbc0: 616d 6529 290a 2020 2020 2020 2020 7769  ame)).        wi
+0000dbd0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000dbe0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000dbf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000dc00: 5b27 426f 6227 2c20 2744 6176 6527 5d2c  ['Bob', 'Dave'],
+0000dc10: 2073 6f72 7465 6428 6e6f 6e5f 7265 672e   sorted(non_reg.
+0000dc20: 616c 6c2e 6e61 6d65 2929 0a0a 2020 2020  all.name))..    
+0000dc30: 2020 2020 2320 636f 7572 7365 7320 7769      # courses wi
+0000dc40: 7468 206e 6f20 7374 7564 656e 7473 0a20  th no students. 
+0000dc50: 2020 2020 2020 206e 6f5f 7374 7564 656e         no_studen
+0000dc60: 7473 203d 2072 6567 6973 7472 6174 696f  ts = registratio
+0000dc70: 6e73 2e6f 7574 6572 5f6a 6f69 6e28 6c74  ns.outer_join(lt
+0000dc80: 2e54 6162 6c65 2e4c 4546 545f 4f55 5445  .Table.LEFT_OUTE
+0000dc90: 525f 4a4f 494e 2c0a 2020 2020 2020 2020  R_JOIN,.        
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2063 6f75 7273 6573 2c0a 2020 2020 2020   courses,.      
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 2020 2063 6f75 7273 653d 2263 6f75 7273     course="cours
+0000dd00: 6522 292e 7768 6572 6528 7374 7564 656e  e").where(studen
+0000dd10: 745f 6964 3d4e 6f6e 6529 0a20 2020 2020  t_id=None).     
+0000dd20: 2020 206e 6f5f 7374 7564 656e 7473 2e70     no_students.p
+0000dd30: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
+0000dd40: 2070 7269 6e74 286c 6973 7428 6e6f 5f73   print(list(no_s
+0000dd50: 7475 6465 6e74 732e 616c 6c2e 636f 7572  tudents.all.cour
+0000dd60: 7365 2929 0a20 2020 2020 2020 2077 6974  se)).        wit
+0000dd70: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000dd80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dd90: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+0000dda0: 2750 4531 3031 275d 2c20 736f 7274 6564  'PE101'], sorted
+0000ddb0: 286e 6f5f 7374 7564 656e 7473 2e61 6c6c  (no_students.all
+0000ddc0: 2e63 6f75 7273 6529 290a 0a0a 2020 2020  .course))...    
+0000ddd0: 2020 2020 6675 6c6c 203d 2020 7374 7564      full =  stud
+0000dde0: 656e 7473 2e6f 7574 6572 5f6a 6f69 6e28  ents.outer_join(
+0000ddf0: 6c74 2e54 6162 6c65 2e46 554c 4c5f 4f55  lt.Table.FULL_OU
+0000de00: 5445 525f 4a4f 494e 2c0a 2020 2020 2020  TER_JOIN,.      
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 7265 6769 7374 7261 7469 6f6e 732c 0a20  registrations,. 
+0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de60: 2020 2020 2073 7475 6465 6e74 5f69 643d       student_id=
+0000de70: 2273 7475 6465 6e74 5f69 6422 292e 7768  "student_id").wh
+0000de80: 6572 6528 6c61 6d62 6461 2072 6563 3a20  ere(lambda rec: 
+0000de90: 7265 632e 636f 7572 7365 2069 7320 4e6f  rec.course is No
+0000dea0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000def0: 2020 2020 6f72 2072 6563 2e6e 616d 6520      or rec.name 
+0000df00: 6973 204e 6f6e 6529 0a20 2020 2020 2020  is None).       
+0000df10: 2066 756c 6c2e 7072 6573 656e 7428 290a   full.present().
+0000df20: 2020 2020 2020 2020 7072 696e 7428 736f          print(so
+0000df30: 7274 6564 2866 756c 6c2e 616c 6c2e 7374  rted(full.all.st
+0000df40: 7564 656e 745f 6964 2929 0a20 2020 2020  udent_id)).     
+0000df50: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000df60: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000df70: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000df80: 7175 616c 285b 2730 3030 3227 2c20 2730  qual(['0002', '0
+0000df90: 3030 3427 2c20 2730 3030 3627 5d2c 2073  004', '0006'], s
+0000dfa0: 6f72 7465 6428 6675 6c6c 2e61 6c6c 2e73  orted(full.all.s
+0000dfb0: 7475 6465 6e74 5f69 6429 290a 0a0a 406d  tudent_id))...@m
+0000dfc0: 616b 655f 7465 7374 5f63 6c61 7373 6573  ake_test_classes
+0000dfd0: 0a63 6c61 7373 2054 6162 6c65 5472 616e  .class TableTran
+0000dfe0: 7366 6f72 6d54 6573 7473 3a0a 2020 2020  sformTests:.    
+0000dff0: 2222 220a 2020 2020 5465 7374 7320 746f  """.    Tests to
+0000e000: 206d 7574 6174 6520 6120 5461 626c 652e   mutate a Table.
+0000e010: 0a20 2020 2022 2222 0a20 2020 2064 6566  .    """.    def
+0000e020: 2074 6573 745f 736f 7274 2873 656c 6629   test_sort(self)
+0000e030: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
+0000e040: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
+0000e050: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
+0000e060: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
+0000e070: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
+0000e080: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+0000e090: 2063 5f67 726f 7570 7320 3d20 300a 2020   c_groups = 0.  
+0000e0a0: 2020 2020 2020 666f 7220 635f 7661 6c75        for c_valu
+0000e0b0: 652c 2072 6563 7320 696e 2069 7465 7274  e, recs in itert
+0000e0c0: 6f6f 6c73 2e67 726f 7570 6279 2874 312c  ools.groupby(t1,
+0000e0d0: 206b 6579 3d6c 616d 6264 6120 7265 633a   key=lambda rec:
+0000e0e0: 2072 6563 2e63 293a 0a20 2020 2020 2020   rec.c):.       
+0000e0f0: 2020 2020 2063 5f67 726f 7570 7320 2b3d       c_groups +=
+0000e100: 2031 0a20 2020 2020 2020 2020 2020 206c   1.            l
+0000e110: 6973 7428 7265 6373 290a 2020 2020 2020  ist(recs).      
+0000e120: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000e130: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000e140: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000e150: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
+0000e160: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+0000e170: 5f73 697a 652c 2063 5f67 726f 7570 7329  _size, c_groups)
+0000e180: 0a0a 2020 2020 2020 2020 7431 2e73 6f72  ..        t1.sor
+0000e190: 7428 2763 2729 0a20 2020 2020 2020 2063  t('c').        c
+0000e1a0: 5f67 726f 7570 7320 3d20 300a 2020 2020  _groups = 0.    
+0000e1b0: 2020 2020 666f 7220 635f 7661 6c75 652c      for c_value,
+0000e1c0: 2072 6563 7320 696e 2069 7465 7274 6f6f   recs in itertoo
+0000e1d0: 6c73 2e67 726f 7570 6279 2874 312c 206b  ls.groupby(t1, k
+0000e1e0: 6579 3d6c 616d 6264 6120 7265 633a 2072  ey=lambda rec: r
+0000e1f0: 6563 2e63 293a 0a20 2020 2020 2020 2020  ec.c):.         
+0000e200: 2020 2063 5f67 726f 7570 7320 2b3d 2031     c_groups += 1
+0000e210: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
+0000e220: 7428 7265 6373 290a 2020 2020 2020 2020  t(recs).        
+0000e230: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000e240: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000e250: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000e260: 6c28 7465 7374 5f73 697a 652c 2063 5f67  l(test_size, c_g
+0000e270: 726f 7570 7329 0a20 2020 2020 2020 2077  roups).        w
+0000e280: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000e290: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e2a0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000e2b0: 2830 2c20 7431 5b30 5d2e 6329 0a0a 2020  (0, t1[0].c)..  
+0000e2c0: 2020 2020 2020 7431 2e73 6f72 7428 2763        t1.sort('c
+0000e2d0: 2064 6573 6327 290a 2020 2020 2020 2020   desc').        
+0000e2e0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000e2f0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000e300: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000e310: 6c28 7465 7374 5f73 697a 652d 312c 2074  l(test_size-1, t
+0000e320: 315b 305d 2e63 290a 0a20 2020 2064 6566  1[0].c)..    def
+0000e330: 2074 6573 745f 736f 7274 3228 7365 6c66   test_sort2(self
+0000e340: 293a 0a0a 2020 2020 2020 2020 726f 775f  ):..        row_
+0000e350: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+0000e360: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+0000e370: 7428 302c 302c 3029 290a 2020 2020 2020  t(0,0,0)).      
+0000e380: 2020 7474 203d 206c 742e 5461 626c 6528    tt = lt.Table(
+0000e390: 292e 6373 765f 696d 706f 7274 2874 6578  ).csv_import(tex
+0000e3a0: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
+0000e3b0: 5c0a 2020 2020 2020 2020 612c 632c 620a  \.        a,c,b.
+0000e3c0: 2020 2020 2020 2020 312c 322c 310a 2020          1,2,1.  
+0000e3d0: 2020 2020 2020 322c 332c 300a 2020 2020        2,3,0.    
+0000e3e0: 2020 2020 352c 352c 2d31 0a20 2020 2020      5,5,-1.     
+0000e3f0: 2020 2033 2c34 2c2d 310a 2020 2020 2020     3,4,-1.      
+0000e400: 2020 322c 342c 2d33 2222 2229 2c20 726f    2,4,-3"""), ro
+0000e410: 775f 636c 6173 733d 726f 775f 7479 7065  w_class=row_type
+0000e420: 2c20 7472 616e 7366 6f72 6d73 3d64 6963  , transforms=dic
+0000e430: 742e 6672 6f6d 6b65 7973 2822 6120 6220  t.fromkeys("a b 
+0000e440: 6322 2e73 706c 6974 2829 2c20 696e 7429  c".split(), int)
+0000e450: 290a 0a20 2020 2020 2020 2064 6566 2074  )..        def t
+0000e460: 6f5f 7475 706c 6573 2874 293a 0a20 2020  o_tuples(t):.   
+0000e470: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e480: 6c69 7374 286d 6170 2861 7474 7267 6574  list(map(attrget
+0000e490: 7465 7228 2a74 2e69 6e66 6f28 295b 2766  ter(*t.info()['f
+0000e4a0: 6965 6c64 7327 5d29 2c20 7429 290a 0a20  ields']), t)).. 
+0000e4b0: 2020 2020 2020 2070 7269 6e74 2874 742e         print(tt.
+0000e4c0: 696e 666f 2829 5b27 6669 656c 6473 275d  info()['fields']
+0000e4d0: 290a 0a20 2020 2020 2020 2073 6f72 745f  )..        sort_
+0000e4e0: 6172 6720 3d20 2263 2062 222e 7370 6c69  arg = "c b".spli
+0000e4f0: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
+0000e500: 7428 6622 536f 7274 696e 6720 6279 207b  t(f"Sorting by {
+0000e510: 736f 7274 5f61 7267 2172 7d22 290a 2020  sort_arg!r}").  
+0000e520: 2020 2020 2020 7474 2e73 6875 6666 6c65        tt.shuffle
+0000e530: 2829 0a20 2020 2020 2020 2074 742e 736f  ().        tt.so
+0000e540: 7274 2873 6f72 745f 6172 6729 0a20 2020  rt(sort_arg).   
+0000e550: 2020 2020 2074 315f 7475 706c 6573 203d       t1_tuples =
+0000e560: 2074 6f5f 7475 706c 6573 2874 7429 0a20   to_tuples(tt). 
+0000e570: 2020 2020 2020 2066 6f72 2074 2069 6e20         for t in 
+0000e580: 7431 5f74 7570 6c65 733a 0a20 2020 2020  t1_tuples:.     
+0000e590: 2020 2020 2020 2070 7269 6e74 2874 290a         print(t).
+0000e5a0: 2020 2020 2020 2020 7072 696e 7428 290a          print().
+0000e5b0: 0a20 2020 2020 2020 2074 742e 7368 7566  .        tt.shuf
+0000e5c0: 666c 6528 290a 2020 2020 2020 2020 7474  fle().        tt
+0000e5d0: 2e73 6f72 7428 2262 2229 0a20 2020 2020  .sort("b").     
+0000e5e0: 2020 2074 742e 736f 7274 2822 6322 290a     tt.sort("c").
+0000e5f0: 2020 2020 2020 2020 7432 5f74 7570 6c65          t2_tuple
+0000e600: 7320 3d20 746f 5f74 7570 6c65 7328 7474  s = to_tuples(tt
+0000e610: 290a 2020 2020 2020 2020 666f 7220 7420  ).        for t 
+0000e620: 696e 2074 325f 7475 706c 6573 3a0a 2020  in t2_tuples:.  
+0000e630: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e640: 7429 0a20 2020 2020 2020 2070 7269 6e74  t).        print
+0000e650: 2829 0a0a 2020 2020 2020 2020 7769 7468  ()..        with
+0000e660: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000e670: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e680: 662e 6173 7365 7274 4571 7561 6c28 7431  f.assertEqual(t1
+0000e690: 5f74 7570 6c65 732c 2074 325f 7475 706c  _tuples, t2_tupl
+0000e6a0: 6573 2c20 2266 6169 6c65 6420 6d75 6c74  es, "failed mult
+0000e6b0: 692d 6174 7472 6962 7574 6520 736f 7274  i-attribute sort
+0000e6c0: 2c20 6769 7665 6e20 6c69 7374 206f 6620  , given list of 
+0000e6d0: 6174 7472 6962 7574 6573 2229 0a0a 2020  attributes")..  
+0000e6e0: 2020 2020 2020 736f 7274 5f61 7267 203d        sort_arg =
+0000e6f0: 2022 632c 6222 0a20 2020 2020 2020 2070   "c,b".        p
+0000e700: 7269 6e74 2866 2253 6f72 7469 6e67 2062  rint(f"Sorting b
+0000e710: 7920 7b73 6f72 745f 6172 6721 727d 2229  y {sort_arg!r}")
+0000e720: 0a20 2020 2020 2020 2074 742e 7368 7566  .        tt.shuf
+0000e730: 666c 6528 290a 2020 2020 2020 2020 7474  fle().        tt
+0000e740: 2e73 6f72 7428 736f 7274 5f61 7267 290a  .sort(sort_arg).
+0000e750: 2020 2020 2020 2020 7431 5f74 7570 6c65          t1_tuple
+0000e760: 7320 3d20 746f 5f74 7570 6c65 7328 7474  s = to_tuples(tt
+0000e770: 290a 2020 2020 2020 2020 666f 7220 7420  ).        for t 
+0000e780: 696e 2074 315f 7475 706c 6573 3a0a 2020  in t1_tuples:.  
+0000e790: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e7a0: 7429 0a20 2020 2020 2020 2070 7269 6e74  t).        print
+0000e7b0: 2829 0a0a 2020 2020 2020 2020 7474 2e73  ()..        tt.s
+0000e7c0: 6875 6666 6c65 2829 0a20 2020 2020 2020  huffle().       
+0000e7d0: 2074 742e 736f 7274 2822 6222 290a 2020   tt.sort("b").  
+0000e7e0: 2020 2020 2020 7474 2e73 6f72 7428 2263        tt.sort("c
+0000e7f0: 2229 0a20 2020 2020 2020 2074 325f 7475  ").        t2_tu
+0000e800: 706c 6573 203d 2074 6f5f 7475 706c 6573  ples = to_tuples
+0000e810: 2874 7429 0a20 2020 2020 2020 2066 6f72  (tt).        for
+0000e820: 2074 2069 6e20 7432 5f74 7570 6c65 733a   t in t2_tuples:
+0000e830: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000e840: 6e74 2874 290a 2020 2020 2020 2020 7072  nt(t).        pr
+0000e850: 696e 7428 290a 0a20 2020 2020 2020 2077  int()..        w
+0000e860: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000e870: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e880: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000e890: 2874 315f 7475 706c 6573 2c20 7432 5f74  (t1_tuples, t2_t
+0000e8a0: 7570 6c65 732c 2022 6661 696c 6564 206d  uples, "failed m
+0000e8b0: 756c 7469 2d61 7474 7269 6275 7465 2073  ulti-attribute s
+0000e8c0: 6f72 742c 2067 6976 656e 2063 6f6d 6d61  ort, given comma
+0000e8d0: 2d73 6570 6172 6174 6564 2061 7474 7269  -separated attri
+0000e8e0: 6275 7465 7320 7374 7269 6e67 2229 0a0a  butes string")..
+0000e8f0: 2020 2020 2020 2020 736f 7274 5f61 7267          sort_arg
+0000e900: 203d 2022 632c 6220 6465 7363 220a 2020   = "c,b desc".  
+0000e910: 2020 2020 2020 7072 696e 7428 6622 536f        print(f"So
+0000e920: 7274 696e 6720 6279 207b 736f 7274 5f61  rting by {sort_a
+0000e930: 7267 2172 7d22 290a 2020 2020 2020 2020  rg!r}").        
+0000e940: 7474 2e73 6875 6666 6c65 2829 0a20 2020  tt.shuffle().   
+0000e950: 2020 2020 2074 742e 736f 7274 2873 6f72       tt.sort(sor
+0000e960: 745f 6172 6729 0a20 2020 2020 2020 2074  t_arg).        t
+0000e970: 315f 7475 706c 6573 203d 2074 6f5f 7475  1_tuples = to_tu
+0000e980: 706c 6573 2874 7429 0a20 2020 2020 2020  ples(tt).       
+0000e990: 2066 6f72 2074 2069 6e20 7431 5f74 7570   for t in t1_tup
+0000e9a0: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
+0000e9b0: 2070 7269 6e74 2874 290a 2020 2020 2020   print(t).      
+0000e9c0: 2020 7072 696e 7428 290a 0a20 2020 2020    print()..     
+0000e9d0: 2020 2074 742e 7368 7566 666c 6528 290a     tt.shuffle().
+0000e9e0: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
+0000e9f0: 2262 2064 6573 6322 290a 2020 2020 2020  "b desc").      
+0000ea00: 2020 7474 2e73 6f72 7428 2263 2229 0a20    tt.sort("c"). 
+0000ea10: 2020 2020 2020 2074 325f 7475 706c 6573         t2_tuples
+0000ea20: 203d 2074 6f5f 7475 706c 6573 2874 7429   = to_tuples(tt)
+0000ea30: 0a20 2020 2020 2020 2066 6f72 2074 2069  .        for t i
+0000ea40: 6e20 7432 5f74 7570 6c65 733a 0a20 2020  n t2_tuples:.   
+0000ea50: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+0000ea60: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000ea70: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+0000ea80: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000ea90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eaa0: 2e61 7373 6572 7445 7175 616c 2874 315f  .assertEqual(t1_
+0000eab0: 7475 706c 6573 2c20 7432 5f74 7570 6c65  tuples, t2_tuple
+0000eac0: 732c 2022 6661 696c 6564 206d 6978 6564  s, "failed mixed
+0000ead0: 2061 7363 656e 6469 6e67 2f64 6573 6365   ascending/desce
+0000eae0: 6e64 696e 6720 6d75 6c74 692d 6174 7472  nding multi-attr
+0000eaf0: 6962 7574 6520 736f 7274 2229 0a0a 2020  ibute sort")..  
+0000eb00: 2020 6465 6620 7465 7374 5f73 6f72 7433    def test_sort3
+0000eb10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000eb20: 656d 706c 6f79 6565 7320 3d20 6c74 2e54  employees = lt.T
+0000eb30: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
+0000eb40: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
+0000eb50: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
+0000eb60: 2020 2065 6d70 5f69 642c 6e61 6d65 2c64     emp_id,name,d
+0000eb70: 6570 742c 7361 6c61 7279 2c63 6f6d 6d69  ept,salary,commi
+0000eb80: 7373 696f 6e0a 2020 2020 2020 2020 2020  ssion.          
+0000eb90: 2020 3030 3031 2c41 6c69 6365 2c53 616c    0001,Alice,Sal
+0000eba0: 6573 2c35 3030 3030 2c30 2e35 0a20 2020  es,50000,0.5.   
+0000ebb0: 2020 2020 2020 2020 2030 3030 322c 426f           0002,Bo
+0000ebc0: 622c 456e 6769 6e65 6572 696e 672c 3130  b,Engineering,10
+0000ebd0: 3030 3030 2c0a 2020 2020 2020 2020 2020  0000,.          
+0000ebe0: 2020 3030 3033 2c43 6861 726c 6573 2c53    0003,Charles,S
+0000ebf0: 616c 6573 2c34 3530 3030 2c30 2e37 0a20  ales,45000,0.7. 
+0000ec00: 2020 2020 2020 2020 2020 2030 3030 342c             0004,
+0000ec10: 4461 7665 2c53 616c 6573 2c34 3530 3030  Dave,Sales,45000
+0000ec20: 2c30 2e36 0a20 2020 2020 2020 2020 2020  ,0.6.           
+0000ec30: 2030 3030 352c 456d 696c 792c 5361 6c65   0005,Emily,Sale
+0000ec40: 732c 3530 3030 302c 302e 340a 2020 2020  s,50000,0.4.    
+0000ec50: 2020 2020 2020 2020 2222 2229 2c20 7472          """), tr
+0000ec60: 616e 7366 6f72 6d73 3d7b 2273 616c 6172  ansforms={"salar
+0000ec70: 7922 3a20 696e 742c 2022 636f 6d6d 6973  y": int, "commis
+0000ec80: 7369 6f6e 223a 2066 6c6f 6174 7d29 0a0a  sion": float})..
+0000ec90: 2020 2020 2020 2020 7361 6c65 735f 656d          sales_em
+0000eca0: 706c 6f79 6565 7320 3d20 656d 706c 6f79  ployees = employ
+0000ecb0: 6565 732e 7768 6572 6528 6465 7074 3d22  ees.where(dept="
+0000ecc0: 5361 6c65 7322 292e 736f 7274 2822 7361  Sales").sort("sa
+0000ecd0: 6c61 7279 2064 6573 632c 636f 6d6d 6973  lary desc,commis
+0000ece0: 7369 6f6e 2229 0a0a 2020 2020 2020 2020  sion")..        
+0000ecf0: 7361 6c65 735f 656d 706c 6f79 6565 732e  sales_employees.
+0000ed00: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000ed10: 2020 7072 696e 7428 6c69 7374 2873 616c    print(list(sal
+0000ed20: 6573 5f65 6d70 6c6f 7965 6573 2e61 6c6c  es_employees.all
+0000ed30: 2e65 6d70 5f69 6429 290a 0a20 2020 2020  .emp_id))..     
+0000ed40: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000ed50: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000ed60: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000ed70: 7175 616c 285b 2730 3030 3527 2c20 2730  qual(['0005', '0
+0000ed80: 3030 3127 2c20 2730 3030 3427 2c20 2730  001', '0004', '0
+0000ed90: 3030 3327 5d2c 0a20 2020 2020 2020 2020  003'],.         
+0000eda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edb0: 2020 2020 6c69 7374 2873 616c 6573 5f65      list(sales_e
+0000edc0: 6d70 6c6f 7965 6573 2e61 6c6c 2e65 6d70  mployees.all.emp
+0000edd0: 5f69 6429 290a 0a20 2020 2064 6566 2074  _id))..    def t
+0000ede0: 6573 745f 756e 6971 7565 2873 656c 6629  est_unique(self)
+0000edf0: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
+0000ee00: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
+0000ee10: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
+0000ee20: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
+0000ee30: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
+0000ee40: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+0000ee50: 2074 3220 3d20 7431 2e75 6e69 7175 6528   t2 = t1.unique(
+0000ee60: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000ee70: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000ee80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ee90: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+0000eea0: 7431 292c 206c 656e 2874 3229 290a 0a20  t1), len(t2)).. 
+0000eeb0: 2020 2020 2020 2074 3320 3d20 7431 2e75         t3 = t1.u
+0000eec0: 6e69 7175 6528 6b65 793d 6c61 6d62 6461  nique(key=lambda
+0000eed0: 2072 6563 3a20 7265 632e 6329 0a20 2020   rec: rec.c).   
+0000eee0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000eef0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000ef00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ef10: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+0000ef20: 2c20 6c65 6e28 7433 2929 0a0a 0a40 6d61  , len(t3))...@ma
+0000ef30: 6b65 5f74 6573 745f 636c 6173 7365 730a  ke_test_classes.
+0000ef40: 636c 6173 7320 5461 626c 654f 7574 7075  class TableOutpu
+0000ef50: 7454 6573 7473 3a0a 2020 2020 2222 220a  tTests:.    """.
+0000ef60: 2020 2020 5465 7374 7320 746f 2076 6572      Tests to ver
+0000ef70: 6966 7920 6f75 7470 7574 2066 6f72 6d73  ify output forms
+0000ef80: 2066 6f72 2061 2054 6162 6c65 2e0a 2020   for a Table..  
+0000ef90: 2020 2222 220a 2020 2020 6465 6620 7465    """.    def te
+0000efa0: 7374 5f62 6173 6963 5f70 7265 7365 6e74  st_basic_present
+0000efb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000efc0: 6966 2072 6963 6820 6973 204e 6f6e 653a  if rich is None:
+0000efd0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+0000efe0: 6f72 7420 7761 726e 696e 6773 0a20 2020  ort warnings.   
+0000eff0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000f000: 732e 7761 726e 2822 7269 6368 206e 6f74  s.warn("rich not
+0000f010: 2069 6e73 7461 6c6c 6564 2c20 6361 6e6e   installed, cann
+0000f020: 6f74 2072 756e 2074 6573 7422 290a 2020  ot run test").  
+0000f030: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f040: 0a0a 2020 2020 2020 2020 6672 6f6d 2072  ..        from r
+0000f050: 6963 6820 696d 706f 7274 2062 6f78 0a20  ich import box. 
+0000f060: 2020 2020 2020 2066 726f 6d20 696f 2069         from io i
+0000f070: 6d70 6f72 7420 5374 7269 6e67 494f 0a20  mport StringIO. 
+0000f080: 2020 2020 2020 2074 6162 6c65 203d 206c         table = l
+0000f090: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+0000f0a0: 706f 7274 2874 6578 7477 7261 702e 6465  port(textwrap.de
+0000f0b0: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
+0000f0c0: 2020 2020 2020 612c 620a 2020 2020 2020        a,b.      
+0000f0d0: 2020 2020 2020 3130 2c31 3030 0a20 2020        10,100.   
+0000f0e0: 2020 2020 2020 2020 2032 302c 3230 300a           20,200.
+0000f0f0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000f100: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+0000f110: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000f120: 2020 6f75 7420 3d20 5374 7269 6e67 494f    out = StringIO
+0000f130: 2829 0a20 2020 2020 2020 2074 6162 6c65  ().        table
+0000f140: 2e70 7265 7365 6e74 2866 696c 653d 6f75  .present(file=ou
+0000f150: 742c 2062 6f78 3d62 6f78 2e41 5343 4949  t, box=box.ASCII
+0000f160: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+0000f170: 6564 203d 2074 6578 7477 7261 702e 6465  ed = textwrap.de
+0000f180: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
+0000f190: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+0000f1a0: 2d2b 0a20 2020 2020 2020 2020 2020 207c  -+.            |
+0000f1b0: 2041 2020 7c20 4220 2020 7c0a 2020 2020   A  | B   |.    
+0000f1c0: 2020 2020 2020 2020 7c2d 2d2d 2d2b 2d2d          |----+--
+0000f1d0: 2d2d 2d7c 0a20 2020 2020 2020 2020 2020  ---|.           
+0000f1e0: 207c 2031 3020 7c20 3130 3020 7c0a 2020   | 10 | 100 |.  
+0000f1f0: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
+0000f200: 2032 3030 207c 0a20 2020 2020 2020 2020   200 |.         
+0000f210: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a     +----------+.
+0000f220: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000f230: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000f240: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000f250: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000f260: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000f270: 7465 642c 206f 7574 2e67 6574 7661 6c75  ted, out.getvalu
+0000f280: 6528 2929 0a0a 2020 2020 2020 2020 2320  e())..        # 
+0000f290: 7465 7374 2062 7567 6669 7820 7768 656e  test bugfix when
+0000f2a0: 2074 6162 6c65 2068 6173 2061 7474 7269   table has attri
+0000f2b0: 6275 7465 2022 6465 6661 756c 7422 0a20  bute "default". 
+0000f2c0: 2020 2020 2020 2074 6162 6c65 203d 206c         table = l
+0000f2d0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+0000f2e0: 706f 7274 2874 6578 7477 7261 702e 6465  port(textwrap.de
+0000f2f0: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
+0000f300: 2020 2020 2020 612c 622c 6465 6661 756c        a,b,defaul
+0000f310: 740a 2020 2020 2020 2020 2020 2020 3130  t.            10
+0000f320: 2c31 3030 2c70 7572 706c 650a 2020 2020  ,100,purple.    
+0000f330: 2020 2020 2020 2020 3135 2c31 3530 2c0a          15,150,.
+0000f340: 2020 2020 2020 2020 2020 2020 3230 2c32              20,2
+0000f350: 3030 2c6f 7261 6e67 650a 2020 2020 2020  00,orange.      
+0000f360: 2020 2020 2020 2222 2229 290a 2020 2020        """)).    
+0000f370: 2020 2020 7461 626c 652e 7072 6573 656e      table.presen
+0000f380: 7428 290a 2020 2020 2020 2020 6f75 7420  t().        out 
+0000f390: 3d20 5374 7269 6e67 494f 2829 0a20 2020  = StringIO().   
+0000f3a0: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
+0000f3b0: 6e74 2866 696c 653d 6f75 742c 2062 6f78  nt(file=out, box
+0000f3c0: 3d62 6f78 2e41 5343 4949 290a 2020 2020  =box.ASCII).    
+0000f3d0: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
+0000f3e0: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+0000f3f0: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
+0000f400: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+0000f410: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2020  -----+.         
+0000f420: 2020 207c 2041 2020 7c20 4220 2020 7c20     | A  | B   | 
+0000f430: 4465 6661 756c 7420 7c0a 2020 2020 2020  Default |.      
+0000f440: 2020 2020 2020 7c2d 2d2d 2d2b 2d2d 2d2d        |----+----
+0000f450: 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -+---------|.   
+0000f460: 2020 2020 2020 2020 207c 2031 3020 7c20           | 10 | 
+0000f470: 3130 3020 7c20 7075 7270 6c65 2020 7c0a  100 | purple  |.
+0000f480: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+0000f490: 207c 2031 3530 207c 2020 2020 2020 2020   | 150 |        
+0000f4a0: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
+0000f4b0: 2032 3020 7c20 3230 3020 7c20 6f72 616e   20 | 200 | oran
+0000f4c0: 6765 2020 7c0a 2020 2020 2020 2020 2020  ge  |.          
+0000f4d0: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    +-------------
+0000f4e0: 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020 2020  -------+.       
+0000f4f0: 2020 2020 2022 2222 290a 2020 2020 2020       """).      
+0000f500: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000f510: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000f520: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000f530: 7561 6c28 6578 7065 6374 6564 2c20 6f75  ual(expected, ou
+0000f540: 742e 6765 7476 616c 7565 2829 290a 0a20  t.getvalue()).. 
+0000f550: 2020 2020 2020 2023 2074 6573 7420 6772         # test gr
+0000f560: 6f75 7062 790a 2020 2020 2020 2020 7461  oupby.        ta
+0000f570: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+0000f580: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
+0000f590: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+0000f5a0: 0a20 2020 2020 2020 2020 2020 2061 2c62  .            a,b
+0000f5b0: 2c64 6566 6175 6c74 0a20 2020 2020 2020  ,default.       
+0000f5c0: 2020 2020 2031 302c 3130 302c 7075 7270       10,100,purp
+0000f5d0: 6c65 0a20 2020 2020 2020 2020 2020 2031  le.            1
+0000f5e0: 352c 3135 302c 7075 7270 6c65 0a20 2020  5,150,purple.   
+0000f5f0: 2020 2020 2020 2020 2032 302c 3230 302c           20,200,
+0000f600: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
+0000f610: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
+0000f620: 2074 6162 6c65 2e70 7265 7365 6e74 2829   table.present()
+0000f630: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
+0000f640: 7265 7365 6e74 2862 6f78 3d62 6f78 2e41  resent(box=box.A
+0000f650: 5343 4949 2c20 6772 6f75 7062 793d 2264  SCII, groupby="d
+0000f660: 6566 6175 6c74 2229 0a20 2020 2020 2020  efault").       
+0000f670: 206f 7574 203d 2053 7472 696e 6749 4f28   out = StringIO(
+0000f680: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+0000f690: 7072 6573 656e 7428 6669 6c65 3d6f 7574  present(file=out
+0000f6a0: 2c20 626f 783d 626f 782e 4153 4349 492c  , box=box.ASCII,
+0000f6b0: 2067 726f 7570 6279 3d22 6465 6661 756c   groupby="defaul
+0000f6c0: 7422 290a 2020 2020 2020 2020 6578 7065  t").        expe
+0000f6d0: 6374 6564 203d 2074 6578 7477 7261 702e  cted = textwrap.
+0000f6e0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+0000f6f0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+0000f700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20  -------------+. 
+0000f710: 2020 2020 2020 2020 2020 207c 2041 2020             | A  
+0000f720: 7c20 4220 2020 7c20 4465 6661 756c 7420  | B   | Default 
+0000f730: 7c0a 2020 2020 2020 2020 2020 2020 7c2d  |.            |-
+0000f740: 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---+-----+------
+0000f750: 2d2d 2d7c 0a20 2020 2020 2020 2020 2020  ---|.           
+0000f760: 207c 2031 3020 7c20 3130 3020 7c20 7075   | 10 | 100 | pu
+0000f770: 7270 6c65 2020 7c0a 2020 2020 2020 2020  rple  |.        
+0000f780: 2020 2020 7c20 3135 207c 2031 3530 207c      | 15 | 150 |
+0000f790: 2020 2020 2020 2020 207c 0a20 2020 2020           |.     
+0000f7a0: 2020 2020 2020 207c 2032 3020 7c20 3230         | 20 | 20
+0000f7b0: 3020 7c20 6f72 616e 6765 2020 7c0a 2020  0 | orange  |.  
+0000f7c0: 2020 2020 2020 2020 2020 2b2d 2d2d 2d2d            +-----
+0000f7d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000f7e0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+0000f7f0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+0000f800: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+0000f810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f820: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+0000f830: 6374 6564 2c20 6f75 742e 6765 7476 616c  cted, out.getval
+0000f840: 7565 2829 290a 0a20 2020 2020 2020 2074  ue())..        t
+0000f850: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+0000f860: 292e 6373 765f 696d 706f 7274 2874 6578  ).csv_import(tex
+0000f870: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
+0000f880: 5c0a 2020 2020 2020 2020 2020 2020 612c  \.            a,
+0000f890: 622c 6465 6661 756c 740a 2020 2020 2020  b,default.      
+0000f8a0: 2020 2020 2020 3130 2c31 3030 2c70 7572        10,100,pur
+0000f8b0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+0000f8c0: 3135 2c31 3530 2c70 7572 706c 650a 2020  15,150,purple.  
+0000f8d0: 2020 2020 2020 2020 2020 3135 2c32 3030            15,200
+0000f8e0: 2c6f 7261 6e67 650a 2020 2020 2020 2020  ,orange.        
+0000f8f0: 2020 2020 3135 2c32 3530 2c6f 7261 6e67      15,250,orang
+0000f900: 650a 2020 2020 2020 2020 2020 2020 3230  e.            20
+0000f910: 2c32 3530 2c6f 7261 6e67 650a 2020 2020  ,250,orange.    
+0000f920: 2020 2020 2020 2020 2222 2229 290a 2020          """)).  
+0000f930: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
+0000f940: 656e 7428 290a 2020 2020 2020 2020 7461  ent().        ta
+0000f950: 626c 652e 7072 6573 656e 7428 626f 783d  ble.present(box=
+0000f960: 626f 782e 4153 4349 492c 2067 726f 7570  box.ASCII, group
+0000f970: 6279 3d22 6465 6661 756c 7420 6122 290a  by="default a").
+0000f980: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
+0000f990: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
+0000f9a0: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
+0000f9b0: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
+0000f9c0: 2e41 5343 4949 2c20 6772 6f75 7062 793d  .ASCII, groupby=
+0000f9d0: 2264 6566 6175 6c74 2061 2229 0a20 2020  "default a").   
+0000f9e0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+0000f9f0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000fa00: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000fa10: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
+0000fa20: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+0000fa30: 2020 2020 7c20 4120 207c 2042 2020 207c      | A  | B   |
+0000fa40: 2044 6566 6175 6c74 207c 0a20 2020 2020   Default |.     
+0000fa50: 2020 2020 2020 207c 2d2d 2d2d 2b2d 2d2d         |----+---
+0000fa60: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  --+---------|.  
+0000fa70: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
+0000fa80: 2031 3030 207c 2070 7572 706c 6520 207c   100 | purple  |
+0000fa90: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000faa0: 3520 7c20 3135 3020 7c20 2020 2020 2020  5 | 150 |       
+0000fab0: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000fac0: 7c20 3135 207c 2032 3030 207c 206f 7261  | 15 | 200 | ora
+0000fad0: 6e67 6520 207c 0a20 2020 2020 2020 2020  nge  |.         
+0000fae0: 2020 207c 2020 2020 7c20 3235 3020 7c20     |    | 250 | 
+0000faf0: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
+0000fb00: 2020 2020 2020 7c20 3230 207c 2032 3530        | 20 | 250
+0000fb10: 207c 2020 2020 2020 2020 207c 0a20 2020   |         |.   
+0000fb20: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
+0000fb30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+0000fb40: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000fb50: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000fb60: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000fb70: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fb80: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000fb90: 7465 642c 206f 7574 2e67 6574 7661 6c75  ted, out.getvalu
+0000fba0: 6528 2929 0a0a 2020 2020 2020 2020 7461  e())..        ta
+0000fbb0: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+0000fbc0: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
+0000fbd0: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+0000fbe0: 0a20 2020 2020 2020 2020 2020 2061 2c62  .            a,b
+0000fbf0: 2c64 6566 6175 6c74 0a20 2020 2020 2020  ,default.       
+0000fc00: 2020 2020 2031 302c 3130 302c 7075 7270       10,100,purp
+0000fc10: 6c65 0a20 2020 2020 2020 2020 2020 2031  le.            1
+0000fc20: 352c 3230 302c 6f72 616e 6765 0a20 2020  5,200,orange.   
+0000fc30: 2020 2020 2020 2020 2031 352c 3135 302c           15,150,
+0000fc40: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
+0000fc50: 2020 2032 302c 3235 302c 6f72 616e 6765     20,250,orange
+0000fc60: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
+0000fc70: 3235 302c 6f72 616e 6765 0a20 2020 2020  250,orange.     
+0000fc80: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
+0000fc90: 2020 2020 2074 6162 6c65 2e73 6f72 7428       table.sort(
+0000fca0: 2264 6566 6175 6c74 2064 6573 632c 6122  "default desc,a"
+0000fcb0: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+0000fcc0: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000fcd0: 2020 7461 626c 652e 7072 6573 656e 7428    table.present(
+0000fce0: 626f 783d 626f 782e 4153 4349 492c 2067  box=box.ASCII, g
+0000fcf0: 726f 7570 6279 3d22 6465 6661 756c 7420  roupby="default 
+0000fd00: 6122 290a 2020 2020 2020 2020 6f75 7420  a").        out 
+0000fd10: 3d20 5374 7269 6e67 494f 2829 0a20 2020  = StringIO().   
+0000fd20: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
+0000fd30: 6e74 2866 696c 653d 6f75 742c 2062 6f78  nt(file=out, box
+0000fd40: 3d62 6f78 2e41 5343 4949 2c20 6772 6f75  =box.ASCII, grou
+0000fd50: 7062 793d 2264 6566 6175 6c74 2061 2229  pby="default a")
+0000fd60: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+0000fd70: 6420 3d20 7465 7874 7772 6170 2e64 6564  d = textwrap.ded
+0000fd80: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+0000fd90: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
+0000fda0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
+0000fdb0: 2020 2020 2020 2020 7c20 4120 207c 2042          | A  | B
+0000fdc0: 2020 207c 2044 6566 6175 6c74 207c 0a20     | Default |. 
+0000fdd0: 2020 2020 2020 2020 2020 207c 2d2d 2d2d             |----
+0000fde0: 2b2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  +-----+---------
+0000fdf0: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000fe00: 3130 207c 2031 3030 207c 2070 7572 706c  10 | 100 | purpl
+0000fe10: 6520 207c 0a20 2020 2020 2020 2020 2020  e  |.           
+0000fe20: 207c 2031 3520 7c20 3135 3020 7c20 2020   | 15 | 150 |   
+0000fe30: 2020 2020 2020 7c0a 2020 2020 2020 2020        |.        
+0000fe40: 2020 2020 7c20 3135 207c 2032 3030 207c      | 15 | 200 |
+0000fe50: 206f 7261 6e67 6520 207c 0a20 2020 2020   orange  |.     
+0000fe60: 2020 2020 2020 207c 2020 2020 7c20 3235         |    | 25
+0000fe70: 3020 7c20 2020 2020 2020 2020 7c0a 2020  0 |         |.  
+0000fe80: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
+0000fe90: 2032 3530 207c 2020 2020 2020 2020 207c   250 |         |
+0000fea0: 0a20 2020 2020 2020 2020 2020 202b 2d2d  .            +--
+0000feb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000fec0: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
+0000fed0: 2222 2229 0a20 2020 2020 2020 2077 6974  """).        wit
+0000fee0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000fef0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ff00: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+0000ff10: 7870 6563 7465 642c 206f 7574 2e67 6574  xpected, out.get
+0000ff20: 7661 6c75 6528 2929 0a0a 2020 2020 6465  value())..    de
+0000ff30: 6620 7465 7374 5f6d 6172 6b64 6f77 6e28  f test_markdown(
+0000ff40: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+0000ff50: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+0000ff60: 292e 6373 765f 696d 706f 7274 2874 6578  ).csv_import(tex
+0000ff70: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
+0000ff80: 5c0a 2020 2020 2020 2020 2020 2020 612c  \.            a,
+0000ff90: 620a 2020 2020 2020 2020 2020 2020 3130  b.            10
+0000ffa0: 2c31 3030 0a20 2020 2020 2020 2020 2020  ,100.           
+0000ffb0: 2032 302c 3230 300a 2020 2020 2020 2020   20,200.        
+0000ffc0: 2020 2020 2222 2229 290a 2020 2020 2020      """)).      
+0000ffd0: 2020 6f75 745f 6d61 726b 646f 776e 203d    out_markdown =
+0000ffe0: 2074 6162 6c65 2e61 735f 6d61 726b 646f   table.as_markdo
+0000fff0: 776e 2829 0a20 2020 2020 2020 2070 7269  wn().        pri
+00010000: 6e74 286f 7574 5f6d 6172 6b64 6f77 6e29  nt(out_markdown)
+00010010: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+00010020: 6420 3d20 7465 7874 7772 6170 2e64 6564  d = textwrap.ded
+00010030: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+00010040: 2020 2020 207c 2061 207c 2062 207c 0a20       | a | b |. 
+00010050: 2020 2020 2020 2020 2020 207c 2d2d 2d7c             |---|
+00010060: 2d2d 2d7c 0a20 2020 2020 2020 2020 2020  ---|.           
+00010070: 207c 2031 3020 7c20 3130 3020 7c0a 2020   | 10 | 100 |.  
+00010080: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
+00010090: 2032 3030 207c 0a20 2020 2020 2020 2020   200 |.         
+000100a0: 2020 2022 2222 290a 2020 2020 2020 2020     """).        
+000100b0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+000100c0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+000100d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000100e0: 6c28 6578 7065 6374 6564 2c20 6f75 745f  l(expected, out_
+000100f0: 6d61 726b 646f 776e 290a 0a20 2020 2020  markdown)..     
+00010100: 2020 2023 2074 6573 7420 6275 6766 6978     # test bugfix
+00010110: 2077 6865 6e20 7461 626c 6520 6861 7320   when table has 
+00010120: 6174 7472 6962 7574 6520 2264 6566 6175  attribute "defau
+00010130: 6c74 220a 2020 2020 2020 2020 7461 626c  lt".        tabl
+00010140: 6520 3d20 6c74 2e54 6162 6c65 2829 2e63  e = lt.Table().c
+00010150: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
+00010160: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+00010170: 2020 2020 2020 2020 2020 2061 2c62 2c64             a,b,d
+00010180: 6566 6175 6c74 0a20 2020 2020 2020 2020  efault.         
+00010190: 2020 2031 302c 3130 302c 7075 7270 6c65     10,100,purple
+000101a0: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
+000101b0: 3135 302c 0a20 2020 2020 2020 2020 2020  150,.           
+000101c0: 2032 302c 3230 302c 6f72 616e 6765 0a20   20,200,orange. 
+000101d0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+000101e0: 0a20 2020 2020 2020 206f 7574 5f6d 6172  .        out_mar
+000101f0: 6b64 6f77 6e20 3d20 7461 626c 652e 6173  kdown = table.as
+00010200: 5f6d 6172 6b64 6f77 6e28 290a 2020 2020  _markdown().    
+00010210: 2020 2020 7072 696e 7428 6f75 745f 6d61      print(out_ma
+00010220: 726b 646f 776e 290a 2020 2020 2020 2020  rkdown).        
+00010230: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
+00010240: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+00010250: 2020 2020 2020 2020 2020 2020 7c20 6120              | a 
+00010260: 7c20 6220 7c20 6465 6661 756c 7420 7c0a  | b | default |.
+00010270: 2020 2020 2020 2020 2020 2020 7c2d 2d2d              |---
+00010280: 7c2d 2d2d 7c2d 2d2d 7c0a 2020 2020 2020  |---|---|.      
+00010290: 2020 2020 2020 7c20 3130 207c 2031 3030        | 10 | 100
+000102a0: 207c 2070 7572 706c 6520 7c0a 2020 2020   | purple |.    
+000102b0: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
+000102c0: 3530 207c 2020 7c0a 2020 2020 2020 2020  50 |  |.        
+000102d0: 2020 2020 7c20 3230 207c 2032 3030 207c      | 20 | 200 |
+000102e0: 206f 7261 6e67 6520 7c0a 2020 2020 2020   orange |.      
+000102f0: 2020 2020 2020 2222 2229 0a20 2020 2020        """).     
+00010300: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00010310: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00010320: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00010330: 7175 616c 2865 7870 6563 7465 642c 206f  qual(expected, o
+00010340: 7574 5f6d 6172 6b64 6f77 6e29 0a0a 2020  ut_markdown)..  
+00010350: 2020 2020 2020 2320 7465 7374 2067 726f        # test gro
+00010360: 7570 696e 6720 696e 2061 735f 6d61 726b  uping in as_mark
+00010370: 646f 776e 0a20 2020 2020 2020 2074 6162  down.        tab
+00010380: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
+00010390: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
+000103a0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+000103b0: 2020 2020 2020 2020 2020 2020 612c 622c              a,b,
+000103c0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
+000103d0: 2020 2020 3130 2c31 3030 2c70 7572 706c      10,100,purpl
+000103e0: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
+000103f0: 2c31 3530 2c70 7572 706c 650a 2020 2020  ,150,purple.    
+00010400: 2020 2020 2020 2020 3230 2c32 3030 2c6f          20,200,o
+00010410: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
+00010420: 2020 2222 2229 290a 2020 2020 2020 2020    """)).        
+00010430: 6f75 745f 6d61 726b 646f 776e 203d 2074  out_markdown = t
+00010440: 6162 6c65 2e61 735f 6d61 726b 646f 776e  able.as_markdown
+00010450: 2867 726f 7570 6279 3d22 6465 6661 756c  (groupby="defaul
+00010460: 7422 290a 2020 2020 2020 2020 7072 696e  t").        prin
+00010470: 7428 6f75 745f 6d61 726b 646f 776e 290a  t(out_markdown).
+00010480: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00010490: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+000104a0: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+000104b0: 2020 2020 7c20 6120 7c20 6220 7c20 6465      | a | b | de
+000104c0: 6661 756c 7420 7c0a 2020 2020 2020 2020  fault |.        
+000104d0: 2020 2020 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d      |---|---|---
+000104e0: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+000104f0: 3130 207c 2031 3030 207c 2070 7572 706c  10 | 100 | purpl
+00010500: 6520 7c0a 2020 2020 2020 2020 2020 2020  e |.            
+00010510: 7c20 3135 207c 2031 3530 207c 2020 7c0a  | 15 | 150 |  |.
+00010520: 2020 2020 2020 2020 2020 2020 7c20 3230              | 20
+00010530: 207c 2032 3030 207c 206f 7261 6e67 6520   | 200 | orange 
+00010540: 7c0a 2020 2020 2020 2020 2020 2020 2222  |.            ""
+00010550: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+00010560: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00010570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010580: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
+00010590: 6563 7465 642c 206f 7574 5f6d 6172 6b64  ected, out_markd
+000105a0: 6f77 6e29 0a0a 2020 2020 2020 2020 7461  own)..        ta
+000105b0: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+000105c0: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
+000105d0: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+000105e0: 0a20 2020 2020 2020 2020 2020 2061 2c62  .            a,b
+000105f0: 2c64 6566 6175 6c74 0a20 2020 2020 2020  ,default.       
+00010600: 2020 2020 2031 302c 3130 302c 7075 7270       10,100,purp
+00010610: 6c65 0a20 2020 2020 2020 2020 2020 2031  le.            1
+00010620: 352c 3230 302c 6f72 616e 6765 0a20 2020  5,200,orange.   
+00010630: 2020 2020 2020 2020 2031 352c 3135 302c           15,150,
+00010640: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
+00010650: 2020 2032 302c 3235 302c 6f72 616e 6765     20,250,orange
+00010660: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
+00010670: 3235 302c 6f72 616e 6765 0a20 2020 2020  250,orange.     
+00010680: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
+00010690: 2020 2020 2074 6162 6c65 2e73 6f72 7428       table.sort(
+000106a0: 2264 6566 6175 6c74 2064 6573 632c 6122  "default desc,a"
+000106b0: 290a 2020 2020 2020 2020 6f75 745f 6d61  ).        out_ma
+000106c0: 726b 646f 776e 203d 2074 6162 6c65 2e61  rkdown = table.a
+000106d0: 735f 6d61 726b 646f 776e 2867 726f 7570  s_markdown(group
+000106e0: 6279 3d22 6465 6661 756c 7420 6122 290a  by="default a").
+000106f0: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
+00010700: 745f 6d61 726b 646f 776e 290a 2020 2020  t_markdown).    
+00010710: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
+00010720: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+00010730: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
+00010740: 7c20 6120 7c20 6220 7c20 6465 6661 756c  | a | b | defaul
+00010750: 7420 7c0a 2020 2020 2020 2020 2020 2020  t |.            
+00010760: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a 2020  |---|---|---|.  
+00010770: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
+00010780: 2031 3030 207c 2070 7572 706c 6520 7c0a   100 | purple |.
+00010790: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+000107a0: 207c 2031 3530 207c 2020 7c0a 2020 2020   | 150 |  |.    
+000107b0: 2020 2020 2020 2020 7c20 3135 207c 2032          | 15 | 2
+000107c0: 3030 207c 206f 7261 6e67 6520 7c0a 2020  00 | orange |.  
+000107d0: 2020 2020 2020 2020 2020 7c20 207c 2032            |  | 2
+000107e0: 3530 207c 2020 7c0a 2020 2020 2020 2020  50 |  |.        
+000107f0: 2020 2020 7c20 3230 207c 2032 3530 207c      | 20 | 250 |
+00010800: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+00010810: 2222 2229 0a20 2020 2020 2020 2077 6974  """).        wit
+00010820: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00010830: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010840: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+00010850: 7870 6563 7465 642c 206f 7574 5f6d 6172  xpected, out_mar
+00010860: 6b64 6f77 6e29 0a0a 2320 7361 6d70 6c65  kdown)..# sample
+00010870: 2069 6d70 6f72 7420 6461 7461 2073 6574   import data set
+00010880: 730a 6373 765f 6461 7461 203d 2022 2222  s.csv_data = """
+00010890: 5c0a 612c 622c 630a 302c 302c 300a 302c  \.a,b,c.0,0,0.0,
+000108a0: 302c 310a 302c 302c 320a 302c 312c 300a  0,1.0,0,2.0,1,0.
+000108b0: 302c 312c 310a 302c 312c 320a 302c 322c  0,1,1.0,1,2.0,2,
+000108c0: 300a 302c 322c 310a 302c 322c 320a 312c  0.0,2,1.0,2,2.1,
+000108d0: 302c 300a 312c 302c 310a 312c 302c 320a  0,0.1,0,1.1,0,2.
+000108e0: 312c 312c 300a 312c 312c 310a 312c 312c  1,1,0.1,1,1.1,1,
+000108f0: 320a 312c 322c 300a 312c 322c 310a 312c  2.1,2,0.1,2,1.1,
+00010900: 322c 320a 322c 302c 300a 322c 302c 310a  2,2.2,0,0.2,0,1.
+00010910: 322c 302c 320a 322c 312c 300a 322c 312c  2,0,2.2,1,0.2,1,
+00010920: 310a 322c 312c 320a 322c 322c 300a 322c  1.2,1,2.2,2,0.2,
+00010930: 322c 310a 322c 322c 320a 0a22 2222 0a0a  2,1.2,2,2.."""..
+00010940: 6a73 6f6e 5f64 6174 6120 3d20 2222 225c  json_data = """\
+00010950: 0a20 2020 207b 2261 223a 2030 2c20 2262  .    {"a": 0, "b
+00010960: 223a 2030 2c20 2263 223a 2030 7d0a 2020  ": 0, "c": 0}.  
+00010970: 2020 7b22 6122 3a20 302c 2022 6222 3a20    {"a": 0, "b": 
+00010980: 302c 2022 6322 3a20 317d 0a20 2020 207b  0, "c": 1}.    {
+00010990: 2261 223a 2030 2c20 2262 223a 2030 2c20  "a": 0, "b": 0, 
+000109a0: 2263 223a 2032 7d0a 2020 2020 7b22 6122  "c": 2}.    {"a"
+000109b0: 3a20 302c 2022 6222 3a20 312c 2022 6322  : 0, "b": 1, "c"
+000109c0: 3a20 307d 0a20 2020 207b 2261 223a 2030  : 0}.    {"a": 0
+000109d0: 2c20 2262 223a 2031 2c20 2263 223a 2031  , "b": 1, "c": 1
+000109e0: 7d0a 2020 2020 7b22 6122 3a20 302c 2022  }.    {"a": 0, "
+000109f0: 6222 3a20 312c 2022 6322 3a20 327d 0a20  b": 1, "c": 2}. 
+00010a00: 2020 207b 2261 223a 2030 2c20 2262 223a     {"a": 0, "b":
+00010a10: 2032 2c20 2263 223a 2030 7d0a 2020 2020   2, "c": 0}.    
+00010a20: 7b22 6122 3a20 302c 2022 6222 3a20 322c  {"a": 0, "b": 2,
+00010a30: 2022 6322 3a20 317d 0a20 2020 207b 2261   "c": 1}.    {"a
+00010a40: 223a 2030 2c20 2262 223a 2032 2c20 2263  ": 0, "b": 2, "c
+00010a50: 223a 2032 7d0a 2020 2020 7b22 6122 3a20  ": 2}.    {"a": 
+00010a60: 312c 2022 6222 3a20 302c 2022 6322 3a20  1, "b": 0, "c": 
+00010a70: 307d 0a20 2020 207b 2261 223a 2031 2c20  0}.    {"a": 1, 
+00010a80: 2262 223a 2030 2c20 2263 223a 2031 7d0a  "b": 0, "c": 1}.
+00010a90: 2020 2020 7b22 6122 3a20 312c 2022 6222      {"a": 1, "b"
+00010aa0: 3a20 302c 2022 6322 3a20 327d 0a20 2020  : 0, "c": 2}.   
+00010ab0: 207b 2261 223a 2031 2c20 2262 223a 2031   {"a": 1, "b": 1
+00010ac0: 2c20 2263 223a 2030 7d0a 2020 2020 7b22  , "c": 0}.    {"
+00010ad0: 6122 3a20 312c 2022 6222 3a20 312c 2022  a": 1, "b": 1, "
+00010ae0: 6322 3a20 317d 0a20 2020 207b 2261 223a  c": 1}.    {"a":
+00010af0: 2031 2c20 2262 223a 2031 2c20 2263 223a   1, "b": 1, "c":
+00010b00: 2032 7d0a 2020 2020 7b22 6122 3a20 312c   2}.    {"a": 1,
+00010b10: 2022 6222 3a20 322c 2022 6322 3a20 307d   "b": 2, "c": 0}
+00010b20: 0a20 2020 207b 2261 223a 2031 2c20 2262  .    {"a": 1, "b
+00010b30: 223a 2032 2c20 2263 223a 2031 7d0a 2020  ": 2, "c": 1}.  
+00010b40: 2020 7b22 6122 3a20 312c 2022 6222 3a20    {"a": 1, "b": 
+00010b50: 322c 2022 6322 3a20 327d 0a20 2020 207b  2, "c": 2}.    {
+00010b60: 2261 223a 2032 2c20 2262 223a 2030 2c20  "a": 2, "b": 0, 
+00010b70: 2263 223a 2030 7d0a 2020 2020 7b22 6122  "c": 0}.    {"a"
+00010b80: 3a20 322c 2022 6222 3a20 302c 2022 6322  : 2, "b": 0, "c"
+00010b90: 3a20 317d 0a20 2020 207b 2261 223a 2032  : 1}.    {"a": 2
+00010ba0: 2c20 2262 223a 2030 2c20 2263 223a 2032  , "b": 0, "c": 2
+00010bb0: 7d0a 2020 2020 7b22 6122 3a20 322c 2022  }.    {"a": 2, "
+00010bc0: 6222 3a20 312c 2022 6322 3a20 307d 0a20  b": 1, "c": 0}. 
+00010bd0: 2020 207b 2261 223a 2032 2c20 2262 223a     {"a": 2, "b":
+00010be0: 2031 2c20 2263 223a 2031 7d0a 2020 2020   1, "c": 1}.    
+00010bf0: 7b22 6122 3a20 322c 2022 6222 3a20 312c  {"a": 2, "b": 1,
+00010c00: 2022 6322 3a20 327d 0a20 2020 207b 2261   "c": 2}.    {"a
+00010c10: 223a 2032 2c20 2262 223a 2032 2c20 2263  ": 2, "b": 2, "c
+00010c20: 223a 2030 7d0a 2020 2020 7b22 6122 3a20  ": 0}.    {"a": 
+00010c30: 322c 2022 6222 3a20 322c 2022 6322 3a20  2, "b": 2, "c": 
+00010c40: 317d 0a20 2020 207b 2261 223a 2032 2c20  1}.    {"a": 2, 
+00010c50: 2262 223a 2032 2c20 2263 223a 2032 7d0a  "b": 2, "c": 2}.
+00010c60: 0a22 2222 0a0a 6669 7865 645f 7769 6474  ."""..fixed_widt
+00010c70: 685f 6461 7461 203d 2022 2222 5c0a 3020  h_data = """\.0 
+00010c80: 3020 300a 3020 3020 310a 3020 3020 320a  0 0.0 0 1.0 0 2.
+00010c90: 3020 3120 300a 3020 3120 310a 3020 3120  0 1 0.0 1 1.0 1 
+00010ca0: 320a 3020 3220 300a 3020 3220 310a 3020  2.0 2 0.0 2 1.0 
+00010cb0: 3220 320a 3120 3020 300a 3120 3020 310a  2 2.1 0 0.1 0 1.
+00010cc0: 3120 3020 320a 3120 3120 300a 3120 3120  1 0 2.1 1 0.1 1 
+00010cd0: 310a 3120 3120 320a 3120 3220 300a 3120  1.1 1 2.1 2 0.1 
+00010ce0: 3220 310a 3120 3220 320a 3220 3020 300a  2 1.1 2 2.2 0 0.
+00010cf0: 3220 3020 310a 3220 3020 320a 3220 3120  2 0 1.2 0 2.2 1 
+00010d00: 300a 3220 3120 310a 3220 3120 320a 3220  0.2 1 1.2 1 2.2 
+00010d10: 3220 300a 3220 3220 310a 3220 3220 320a  2 0.2 2 1.2 2 2.
+00010d20: 0a22 2222 0a0a 0a40 6d61 6b65 5f74 6573  ."""...@make_tes
+00010d30: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
+00010d40: 5461 626c 6549 6d70 6f72 7445 7870 6f72  TableImportExpor
+00010d50: 7454 6573 7473 3a0a 2020 2020 2222 220a  tTests:.    """.
+00010d60: 2020 2020 5465 7374 2063 6c61 7373 6573      Test classes
+00010d70: 2066 6f72 2054 6162 6c65 2069 6d70 6f72   for Table impor
+00010d80: 7420 616e 6420 6578 706f 7274 206d 6574  t and export met
+00010d90: 686f 6473 2e0a 2020 2020 2222 220a 2020  hods..    """.  
+00010da0: 2020 6465 6620 7465 7374 5f61 735f 6461    def test_as_da
+00010db0: 7461 6672 616d 6528 7365 6c66 293a 0a20  taframe(self):. 
+00010dc0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010dd0: 2020 2020 2020 2020 696d 706f 7274 2070          import p
+00010de0: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
+00010df0: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
+00010e00: 7445 7272 6f72 3a0a 2020 2020 2020 2020  tError:.        
+00010e10: 2020 2020 7072 696e 7428 2270 616e 6461      print("panda
+00010e20: 7320 6e6f 7420 696e 7374 616c 6c65 642c  s not installed,
+00010e30: 2073 6b69 7070 696e 6720 7465 7374 2229   skipping test")
+00010e40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010e50: 7572 6e0a 0a20 2020 2020 2020 2069 6d70  urn..        imp
+00010e60: 6f72 7420 6a73 6f6e 0a0a 2020 2020 2020  ort json..      
+00010e70: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
+00010e80: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
+00010e90: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
+00010ea0: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+00010eb0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
+00010ec0: 2020 2020 2020 2020 6466 3a20 7064 2e44          df: pd.D
+00010ed0: 6174 6146 7261 6d65 203d 2074 312e 6173  ataFrame = t1.as
+00010ee0: 5f64 6174 6166 7261 6d65 2822 2d62 2229  _dataframe("-b")
+00010ef0: 0a0a 2020 2020 2020 2020 2320 6368 6563  ..        # chec
+00010f00: 6b20 636f 6c75 6d6e 206e 616d 6573 0a20  k column names. 
+00010f10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010f20: 7274 4571 7561 6c28 5b22 6122 2c20 2263  rtEqual(["a", "c
+00010f30: 225d 2c20 6c69 7374 2864 662e 636f 6c75  "], list(df.colu
+00010f40: 6d6e 7329 290a 0a20 2020 2020 2020 2023  mns))..        #
+00010f50: 2063 6865 636b 2069 6d70 6f72 7465 6420   check imported 
+00010f60: 7661 6c75 6573 0a20 2020 2020 2020 2066  values.        f
+00010f70: 726f 6d5f 6466 203d 2064 662e 746f 5f6a  rom_df = df.to_j
+00010f80: 736f 6e28 6f72 6965 6e74 3d22 7661 6c75  son(orient="valu
+00010f90: 6573 2229 0a20 2020 2020 2020 2065 7870  es").        exp
+00010fa0: 6563 7465 6420 3d20 5b0a 2020 2020 2020  ected = [.      
+00010fb0: 2020 2020 2020 5b72 6563 2e61 2c20 7265        [rec.a, re
+00010fc0: 632e 635d 2066 6f72 2072 6563 2069 6e20  c.c] for rec in 
+00010fd0: 7431 0a20 2020 2020 2020 205d 0a20 2020  t1.        ].   
+00010fe0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00010ff0: 4571 7561 6c28 6578 7065 6374 6564 2c20  Equal(expected, 
+00011000: 6a73 6f6e 2e6c 6f61 6473 2866 726f 6d5f  json.loads(from_
+00011010: 6466 2929 0a0a 2020 2020 6465 6620 7465  df))..    def te
+00011020: 7374 5f63 7376 5f65 7870 6f72 7428 7365  st_csv_export(se
+00011030: 6c66 293a 0a20 2020 2020 2020 2066 726f  lf):.        fro
+00011040: 6d20 6974 6572 746f 6f6c 7320 696d 706f  m itertools impo
+00011050: 7274 2070 6572 6d75 7461 7469 6f6e 730a  rt permutations.
+00011060: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
+00011070: 6520 3d20 330a 2020 2020 2020 2020 7431  e = 3.        t1
+00011080: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00011090: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+000110a0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+000110b0: 697a 6529 0a20 2020 2020 2020 2066 6f72  ize).        for
+000110c0: 2066 6965 6c64 6e61 6d65 7320 696e 2070   fieldnames in p
+000110d0: 6572 6d75 7461 7469 6f6e 7328 6c69 7374  ermutations(list
+000110e0: 2827 6162 6327 2929 3a0a 2020 2020 2020  ('abc')):.      
+000110f0: 2020 2020 2020 6f75 7420 3d20 696f 2e53        out = io.S
+00011100: 7472 696e 6749 4f28 290a 2020 2020 2020  tringIO().      
+00011110: 2020 2020 2020 7431 2e63 7376 5f65 7870        t1.csv_exp
+00011120: 6f72 7428 6f75 742c 2066 6965 6c64 6e61  ort(out, fieldna
+00011130: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
+00011140: 206f 7574 2e73 6565 6b28 3029 0a20 2020   out.seek(0).   
+00011150: 2020 2020 2020 2020 206f 7574 6c69 6e65           outline
+00011160: 7320 3d20 6f75 742e 7265 6164 2829 2e73  s = out.read().s
+00011170: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
+00011180: 2020 2020 2020 2020 6f75 742e 636c 6f73          out.clos
+00011190: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000111a0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+000111b0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+000111c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000111d0: 4571 7561 6c28 272c 272e 6a6f 696e 2866  Equal(','.join(f
+000111e0: 6965 6c64 6e61 6d65 7329 2c20 6f75 746c  ieldnames), outl
+000111f0: 696e 6573 5b30 5d29 0a20 2020 2020 2020  ines[0]).       
+00011200: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00011210: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+00011220: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00011230: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00011240: 7369 7a65 2a2a 332b 312c 206c 656e 286f  size**3+1, len(o
+00011250: 7574 6c69 6e65 7329 290a 2020 2020 2020  utlines)).      
+00011260: 2020 2020 2020 666f 7220 6f62 2c20 6c69        for ob, li
+00011270: 6e65 2069 6e20 7a69 7028 7431 2c20 6f75  ne in zip(t1, ou
+00011280: 746c 696e 6573 5b31 3a5d 293a 0a20 2020  tlines[1:]):.   
+00011290: 2020 2020 2020 2020 2020 2020 2063 7376               csv
+000112a0: 5f76 616c 7320 3d20 6c69 6e65 2e73 706c  _vals = line.spl
+000112b0: 6974 2827 2c27 290a 2020 2020 2020 2020  it(',').        
+000112c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000112d0: 662e 7375 6254 6573 7428 6f62 3d6f 622c  f.subTest(ob=ob,
+000112e0: 2063 7376 5f76 616c 733d 6373 765f 7661   csv_vals=csv_va
+000112f0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+00011300: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011310: 7365 7274 5472 7565 2861 6c6c 280a 2020  sertTrue(all(.  
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 2020 2020 696e 7428 6373 765f 7661        int(csv_va
+00011340: 6c73 5b69 5d29 203d 3d20 6765 7461 7474  ls[i]) == getatt
+00011350: 7228 6f62 2c20 666c 6429 2066 6f72 2069  r(ob, fld) for i
+00011360: 2c20 666c 6420 696e 2065 6e75 6d65 7261  , fld in enumera
+00011370: 7465 2866 6965 6c64 6e61 6d65 7329 0a20  te(fieldnames). 
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2020 2029 290a 0a20 2020 2020 2020 2023     ))..        #
+000113a0: 2072 6572 756e 2075 7369 6e67 2061 6e20   rerun using an 
+000113b0: 656d 7074 7920 7461 626c 650a 2020 2020  empty table.    
+000113c0: 2020 2020 7431 203d 206c 742e 5461 626c      t1 = lt.Tabl
+000113d0: 6528 290a 2020 2020 2020 2020 666f 7220  e().        for 
+000113e0: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
+000113f0: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
+00011400: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
+00011410: 2020 2020 206f 7574 203d 2069 6f2e 5374       out = io.St
+00011420: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
+00011430: 2020 2020 2074 312e 6373 765f 6578 706f       t1.csv_expo
+00011440: 7274 286f 7574 2c20 6669 656c 646e 616d  rt(out, fieldnam
+00011450: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+00011460: 6f75 742e 7365 656b 2830 290a 2020 2020  out.seek(0).    
+00011470: 2020 2020 2020 2020 6f75 746c 696e 6573          outlines
+00011480: 203d 206f 7574 2e72 6561 6428 292e 7370   = out.read().sp
+00011490: 6c69 746c 696e 6573 2829 0a20 2020 2020  litlines().     
+000114a0: 2020 2020 2020 206f 7574 2e63 6c6f 7365         out.close
+000114b0: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
+000114c0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+000114d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000114e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000114f0: 7175 616c 2827 2c27 2e6a 6f69 6e28 6669  qual(','.join(fi
+00011500: 656c 646e 616d 6573 292c 206f 7574 6c69  eldnames), outli
+00011510: 6e65 735b 305d 290a 2020 2020 2020 2020  nes[0]).        
+00011520: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00011530: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00011540: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011550: 7365 7274 4571 7561 6c28 312c 206c 656e  sertEqual(1, len
+00011560: 286f 7574 6c69 6e65 7329 290a 0a20 2020  (outlines))..   
+00011570: 2020 2020 2023 2072 6572 756e 2075 7369       # rerun usi
+00011580: 6e67 2061 6e20 656d 7074 7920 7461 626c  ng an empty tabl
+00011590: 652c 2077 6974 6820 696e 6465 7865 7320  e, with indexes 
+000115a0: 746f 2064 6963 7461 7465 2066 6965 6c64  to dictate field
+000115b0: 6e61 6d65 730a 2020 2020 2020 2020 666f  names.        fo
+000115c0: 7220 6669 656c 646e 616d 6573 2069 6e20  r fieldnames in 
+000115d0: 7065 726d 7574 6174 696f 6e73 286c 6973  permutations(lis
+000115e0: 7428 2761 6263 2729 293a 0a20 2020 2020  t('abc')):.     
+000115f0: 2020 2020 2020 2074 3120 3d20 6c74 2e54         t1 = lt.T
+00011600: 6162 6c65 2829 0a20 2020 2020 2020 2020  able().         
+00011610: 2020 2066 6f72 2066 6c64 2069 6e20 6669     for fld in fi
+00011620: 656c 646e 616d 6573 3a0a 2020 2020 2020  eldnames:.      
+00011630: 2020 2020 2020 2020 2020 7431 2e63 7265            t1.cre
+00011640: 6174 655f 696e 6465 7828 666c 6429 0a20  ate_index(fld). 
+00011650: 2020 2020 2020 2020 2020 206f 7574 203d             out =
+00011660: 2069 6f2e 5374 7269 6e67 494f 2829 0a20   io.StringIO(). 
+00011670: 2020 2020 2020 2020 2020 2074 312e 6373             t1.cs
+00011680: 765f 6578 706f 7274 286f 7574 290a 2020  v_export(out).  
+00011690: 2020 2020 2020 2020 2020 6f75 742e 7365            out.se
+000116a0: 656b 2830 290a 2020 2020 2020 2020 2020  ek(0).          
+000116b0: 2020 6f75 746c 696e 6573 203d 206f 7574    outlines = out
+000116c0: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
+000116d0: 6573 2829 0a20 2020 2020 2020 2020 2020  es().           
+000116e0: 206f 7574 2e63 6c6f 7365 2829 0a20 2020   out.close().   
+000116f0: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00011700: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00011710: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011720: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+00011730: 6574 2866 6965 6c64 6e61 6d65 7329 2c20  et(fieldnames), 
+00011740: 7365 7428 6f75 746c 696e 6573 5b30 5d2e  set(outlines[0].
+00011750: 7370 6c69 7428 272c 2729 2929 0a20 2020  split(','))).   
+00011760: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00011770: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00011780: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011790: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
+000117a0: 2c20 6c65 6e28 6f75 746c 696e 6573 2929  , len(outlines))
+000117b0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+000117c0: 7376 5f65 7870 6f72 745f 746f 5f73 7472  sv_export_to_str
+000117d0: 696e 6728 7365 6c66 293a 0a20 2020 2020  ing(self):.     
+000117e0: 2020 2066 726f 6d20 6974 6572 746f 6f6c     from itertool
+000117f0: 7320 696d 706f 7274 2070 6572 6d75 7461  s import permuta
+00011800: 7469 6f6e 730a 2020 2020 2020 2020 7465  tions.        te
+00011810: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
+00011820: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
+00011830: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+00011840: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00011850: 7465 7374 5f73 697a 6529 0a20 2020 2020  test_size).     
+00011860: 2020 2066 6f72 2066 6965 6c64 6e61 6d65     for fieldname
+00011870: 7320 696e 2070 6572 6d75 7461 7469 6f6e  s in permutation
+00011880: 7328 6c69 7374 2827 6162 6327 2929 3a0a  s(list('abc')):.
+00011890: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
+000118a0: 7374 7269 6e67 203d 2074 312e 6373 765f  string = t1.csv_
+000118b0: 6578 706f 7274 284e 6f6e 652c 2066 6965  export(None, fie
+000118c0: 6c64 6e61 6d65 7329 0a20 2020 2020 2020  ldnames).       
+000118d0: 2020 2020 206f 7574 6c69 6e65 7320 3d20       outlines = 
+000118e0: 6f75 745f 7374 7269 6e67 2e73 706c 6974  out_string.split
+000118f0: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
+00011900: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00011910: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00011920: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011930: 7365 7274 4571 7561 6c28 272c 272e 6a6f  sertEqual(','.jo
+00011940: 696e 2866 6965 6c64 6e61 6d65 7329 2c20  in(fieldnames), 
+00011950: 6f75 746c 696e 6573 5b30 5d29 0a20 2020  outlines[0]).   
+00011960: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00011970: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00011980: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011990: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+000119a0: 6573 745f 7369 7a65 202a 2a20 3320 2b20  est_size ** 3 + 
+000119b0: 312c 206c 656e 286f 7574 6c69 6e65 7329  1, len(outlines)
+000119c0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+000119d0: 7220 6f62 2c20 6c69 6e65 2069 6e20 7a69  r ob, line in zi
+000119e0: 7028 7431 2c20 6f75 746c 696e 6573 5b31  p(t1, outlines[1
+000119f0: 3a5d 293a 0a20 2020 2020 2020 2020 2020  :]):.           
+00011a00: 2020 2020 2063 7376 5f76 616c 7320 3d20       csv_vals = 
+00011a10: 6c69 6e65 2e73 706c 6974 2827 2c27 290a  line.split(',').
+00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a30: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00011a40: 7428 6f62 3d6f 622c 2063 7376 5f76 616c  t(ob=ob, csv_val
+00011a50: 733d 6373 765f 7661 6c73 293a 0a20 2020  s=csv_vals):.   
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00011a80: 2861 6c6c 280a 2020 2020 2020 2020 2020  (all(.          
+00011a90: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00011aa0: 7428 6373 765f 7661 6c73 5b69 5d29 203d  t(csv_vals[i]) =
+00011ab0: 3d20 6765 7461 7474 7228 6f62 2c20 666c  = getattr(ob, fl
+00011ac0: 6429 2066 6f72 2069 2c20 666c 6420 696e  d) for i, fld in
+00011ad0: 2065 6e75 6d65 7261 7465 2866 6965 6c64   enumerate(field
+00011ae0: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
+00011af0: 2020 2020 2020 2020 2020 2029 290a 0a20             )).. 
+00011b00: 2020 2064 6566 2074 6573 745f 6373 765f     def test_csv_
+00011b10: 696d 706f 7274 2873 656c 6629 3a0a 2020  import(self):.  
+00011b20: 2020 2020 2020 6461 7461 203d 2063 7376        data = csv
+00011b30: 5f64 6174 610a 2020 2020 2020 2020 696e  _data.        in
+00011b40: 6373 7620 3d20 696f 2e53 7472 696e 6749  csv = io.StringI
+00011b50: 4f28 6461 7461 290a 2020 2020 2020 2020  O(data).        
+00011b60: 6373 7674 6162 6c65 203d 206c 742e 5461  csvtable = lt.Ta
+00011b70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00011b80: 2869 6e63 7376 2c20 7472 616e 7366 6f72  (incsv, transfor
+00011b90: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
+00011ba0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
+00011bb0: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
+00011bc0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+00011bd0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00011be0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00011bf0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00011c00: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00011c10: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00011c20: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00011c30: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00011c40: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00011c50: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00011c60: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00011c70: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00011c80: 6970 2874 312c 2063 7376 7461 626c 6529  ip(t1, csvtable)
+00011c90: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00011ca0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00011cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011cc0: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
+00011cd0: 2831 2066 6f72 206c 696e 6520 696e 2064  (1 for line in d
+00011ce0: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+00011cf0: 2069 6620 6c69 6e65 2e73 7472 6970 2829   if line.strip()
+00011d00: 292d 312c 206c 656e 2863 7376 7461 626c  )-1, len(csvtabl
+00011d10: 6529 290a 0a20 2020 2020 2020 2069 6e63  e))..        inc
+00011d20: 7376 203d 2069 6f2e 5374 7269 6e67 494f  sv = io.StringIO
+00011d30: 2864 6174 6129 0a20 2020 2020 2020 2072  (data).        r
+00011d40: 6f77 5f70 726f 746f 7479 7065 203d 2073  ow_prototype = s
+00011d50: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+00011d60: 6a65 6374 2830 2c20 302c 2030 290a 2020  ject(0, 0, 0).  
+00011d70: 2020 2020 2020 6373 7674 6162 6c65 3220        csvtable2 
+00011d80: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00011d90: 5f69 6d70 6f72 7428 696e 6373 762c 2074  _import(incsv, t
+00011da0: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
+00011db0: 696e 742c 2027 6227 3a20 696e 742c 2027  int, 'b': int, '
+00011dc0: 6327 3a20 696e 747d 2c20 726f 775f 636c  c': int}, row_cl
+00011dd0: 6173 733d 7479 7065 2872 6f77 5f70 726f  ass=type(row_pro
+00011de0: 746f 7479 7065 2929 5b3a 335d 0a0a 2020  totype))[:3]..  
+00011df0: 2020 2020 2020 7072 696e 7428 7479 7065        print(type
+00011e00: 2874 315b 305d 292e 5f5f 6e61 6d65 5f5f  (t1[0]).__name__
+00011e10: 2c20 7431 5b30 5d29 0a20 2020 2020 2020  , t1[0]).       
+00011e20: 2070 7269 6e74 2874 7970 6528 6373 7674   print(type(csvt
+00011e30: 6162 6c65 325b 305d 292e 5f5f 6e61 6d65  able2[0]).__name
+00011e40: 5f5f 2c20 6373 7674 6162 6c65 325b 305d  __, csvtable2[0]
+00011e50: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00011e60: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00011e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011e80: 6173 7365 7274 4571 7561 6c28 7479 7065  assertEqual(type
+00011e90: 2874 315b 305d 292c 2074 7970 6528 6373  (t1[0]), type(cs
+00011ea0: 7674 6162 6c65 325b 305d 2929 0a0a 2020  vtable2[0]))..  
+00011eb0: 2020 6465 6620 7465 7374 5f63 7376 5f63    def test_csv_c
+00011ec0: 6f6d 7072 6573 7365 645f 696d 706f 7274  ompressed_import
+00011ed0: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
+00011ee0: 2064 6566 2076 6572 6966 795f 7469 6d65   def verify_time
+00011ef0: 7374 616d 7073 2874 312c 2074 322c 2069  stamps(t1, t2, i
+00011f00: 6e66 6f5f 6469 6374 293a 0a20 2020 2020  nfo_dict):.     
+00011f10: 2020 2020 2020 2066 6f72 2074 696d 6573         for times
+00011f20: 7461 6d70 5f61 7474 725f 6e61 6d65 2069  tamp_attr_name i
+00011f30: 6e20 2263 7265 6174 6564 206d 6f64 6966  n "created modif
+00011f40: 6965 6420 6c61 7374 5f69 6d70 6f72 7422  ied last_import"
+00011f50: 2e73 706c 6974 2829 3a0a 2020 2020 2020  .split():.      
+00011f60: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
+00011f70: 616d 705f 7661 6c75 6520 3d20 696e 666f  amp_value = info
+00011f80: 5f64 6963 742e 706f 7028 7469 6d65 7374  _dict.pop(timest
+00011f90: 616d 705f 6174 7472 5f6e 616d 6529 0a20  amp_attr_name). 
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00011fb0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00011fc0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00011fd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00011fe0: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 2074 3120 3c3d 2074 696d 6573 7461 6d70   t1 <= timestamp
+00012010: 5f76 616c 7565 203c 3d20 7432 2c0a 2020  _value <= t2,.  
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2020 2020 2020 6622 696e 636f 7272 6563        f"incorrec
+00012040: 7420 7b74 696d 6573 7461 6d70 5f61 7474  t {timestamp_att
+00012050: 725f 6e61 6d65 7d20 7469 6d65 220a 2020  r_name} time".  
+00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012070: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
+00012080: 6820 7469 6d65 7374 616d 705f 7374 6172  h timestamp_star
+00012090: 745f 656e 6428 2920 6173 2074 696d 696e  t_end() as timin
+000120a0: 673a 0a20 2020 2020 2020 2020 2020 2074  g:.            t
+000120b0: 7420 3d20 6c74 2e54 6162 6c65 2829 2e63  t = lt.Table().c
+000120c0: 7376 5f69 6d70 6f72 7428 2274 6573 742f  sv_import("test/
+000120d0: 6162 632e 6373 7622 2c20 7472 616e 7366  abc.csv", transf
+000120e0: 6f72 6d73 3d64 6963 742e 6672 6f6d 6b65  orms=dict.fromke
+000120f0: 7973 2822 6162 6322 2c20 696e 7429 290a  ys("abc", int)).
+00012100: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+00012110: 645f 696e 666f 5f62 6173 6520 3d20 7474  d_info_base = tt
+00012120: 2e69 6e66 6f28 290a 2020 2020 2020 2020  .info().        
+00012130: 7665 7269 6679 5f74 696d 6573 7461 6d70  verify_timestamp
+00012140: 7328 7469 6d69 6e67 2e73 7461 7274 2c20  s(timing.start, 
+00012150: 7469 6d69 6e67 2e65 6e64 2c20 6578 7065  timing.end, expe
+00012160: 6374 6564 5f69 6e66 6f5f 6261 7365 290a  cted_info_base).
+00012170: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00012180: 6162 632e 6373 7622 2c20 6578 7065 6374  abc.csv", expect
+00012190: 6564 5f69 6e66 6f5f 6261 7365 290a 0a20  ed_info_base).. 
+000121a0: 2020 2020 2020 2063 6f6d 7072 6573 7365         compresse
+000121b0: 645f 6669 6c65 7320 3d20 5b0a 2020 2020  d_files = [.    
+000121c0: 2020 2020 2020 2020 2261 6263 2e63 7376          "abc.csv
+000121d0: 2e7a 6970 222c 0a20 2020 2020 2020 2020  .zip",.         
+000121e0: 2020 2022 6162 632e 6373 762e 677a 222c     "abc.csv.gz",
+000121f0: 0a20 2020 2020 2020 2020 2020 2022 6162  .            "ab
+00012200: 632e 6373 762e 787a 222c 0a20 2020 2020  c.csv.xz",.     
+00012210: 2020 205d 0a20 2020 2020 2020 2066 6f72     ].        for
+00012220: 206e 616d 6520 696e 2063 6f6d 7072 6573   name in compres
+00012230: 7365 645f 6669 6c65 733a 0a20 2020 2020  sed_files:.     
+00012240: 2020 2020 2020 2069 6d70 6f72 745f 736f         import_so
+00012250: 7572 6365 5f6e 616d 6520 3d20 2274 6573  urce_name = "tes
+00012260: 742f 2220 2b20 6e61 6d65 0a20 2020 2020  t/" + name.     
+00012270: 2020 2020 2020 2077 6974 6820 7469 6d65         with time
+00012280: 7374 616d 705f 7374 6172 745f 656e 6428  stamp_start_end(
+00012290: 2920 6173 2074 696d 696e 673a 0a20 2020  ) as timing:.   
+000122a0: 2020 2020 2020 2020 2020 2020 2074 7432               tt2
+000122b0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+000122c0: 765f 696d 706f 7274 2869 6d70 6f72 745f  v_import(import_
+000122d0: 736f 7572 6365 5f6e 616d 652c 2074 7261  source_name, tra
+000122e0: 6e73 666f 726d 733d 6469 6374 2e66 726f  nsforms=dict.fro
+000122f0: 6d6b 6579 7328 2261 6263 222c 2069 6e74  mkeys("abc", int
+00012300: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00012310: 7474 325f 696e 666f 203d 2074 7432 2e69  tt2_info = tt2.i
+00012320: 6e66 6f28 290a 2020 2020 2020 2020 2020  nfo().          
+00012330: 2020 7072 696e 7428 6e61 6d65 2c20 7474    print(name, tt
+00012340: 325f 696e 666f 290a 0a20 2020 2020 2020  2_info)..       
+00012350: 2020 2020 2076 6572 6966 795f 7469 6d65       verify_time
+00012360: 7374 616d 7073 2874 696d 696e 672e 7374  stamps(timing.st
+00012370: 6172 742c 2074 696d 696e 672e 656e 642c  art, timing.end,
+00012380: 2074 7432 5f69 6e66 6f29 0a0a 2020 2020   tt2_info)..    
+00012390: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+000123a0: 5f69 6e66 6f20 3d20 7b2a 2a65 7870 6563  _info = {**expec
+000123b0: 7465 645f 696e 666f 5f62 6173 652c 2022  ted_info_base, "
+000123c0: 6e61 6d65 223a 2069 6d70 6f72 745f 736f  name": import_so
+000123d0: 7572 6365 5f6e 616d 657d 0a20 2020 2020  urce_name}.     
+000123e0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000123f0: 2e73 7562 5465 7374 286e 616d 653d 6e61  .subTest(name=na
+00012400: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
+00012410: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00012420: 4571 7561 6c28 6578 7065 6374 6564 5f69  Equal(expected_i
+00012430: 6e66 6f2c 2074 7432 5f69 6e66 6f29 0a20  nfo, tt2_info). 
+00012440: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00012450: 7365 6c66 2e73 7562 5465 7374 286e 616d  self.subTest(nam
+00012460: 653d 6e61 6d65 293a 0a20 2020 2020 2020  e=name):.       
+00012470: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012480: 7365 7274 4571 7561 6c28 7375 6d28 7474  sertEqual(sum(tt
+00012490: 2e61 6c6c 2e61 292c 2073 756d 2874 7432  .all.a), sum(tt2
+000124a0: 2e61 6c6c 2e61 2929 0a20 2020 2020 2020  .all.a)).       
+000124b0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000124c0: 7562 5465 7374 286e 616d 653d 6e61 6d65  ubTest(name=name
+000124d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000124e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000124f0: 7561 6c28 7375 6d28 7474 2e61 6c6c 2e62  ual(sum(tt.all.b
+00012500: 292c 2073 756d 2874 7432 2e61 6c6c 2e62  ), sum(tt2.all.b
+00012510: 2929 0a20 2020 2020 2020 2020 2020 2077  )).            w
+00012520: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00012530: 286e 616d 653d 6e61 6d65 293a 0a20 2020  (name=name):.   
+00012540: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012550: 662e 6173 7365 7274 4571 7561 6c28 7375  f.assertEqual(su
+00012560: 6d28 7474 2e61 6c6c 2e63 292c 2073 756d  m(tt.all.c), sum
+00012570: 2874 7432 2e61 6c6c 2e63 2929 0a0a 2020  (tt2.all.c))..  
+00012580: 2020 2020 2020 2320 7465 7374 2073 6570        # test sep
+00012590: 6172 6174 656c 792c 206e 6f20 7472 616e  arately, no tran
+000125a0: 7366 6f72 6d73 2066 6f72 204a 534f 4e20  sforms for JSON 
+000125b0: 696d 706f 7274 730a 2020 2020 2020 2020  imports.        
+000125c0: 696d 706f 7274 5f73 6f75 7263 655f 6e61  import_source_na
+000125d0: 6d65 203d 2022 7465 7374 2f61 6263 2e6a  me = "test/abc.j
+000125e0: 736f 6e2e 677a 220a 2020 2020 2020 2020  son.gz".        
+000125f0: 7769 7468 2074 696d 6573 7461 6d70 5f73  with timestamp_s
+00012600: 7461 7274 5f65 6e64 2829 2061 7320 7469  tart_end() as ti
+00012610: 6d69 6e67 3a0a 2020 2020 2020 2020 2020  ming:.          
+00012620: 2020 7474 3220 3d20 6c74 2e54 6162 6c65    tt2 = lt.Table
+00012630: 2829 2e6a 736f 6e5f 696d 706f 7274 2822  ().json_import("
+00012640: 7465 7374 2f61 6263 2e6a 736f 6e2e 677a  test/abc.json.gz
+00012650: 222c 2073 7472 6561 6d69 6e67 3d54 7275  ", streaming=Tru
+00012660: 6529 0a0a 2020 2020 2020 2020 7474 325f  e)..        tt2_
+00012670: 696e 666f 203d 2074 7432 2e69 6e66 6f28  info = tt2.info(
+00012680: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00012690: 2261 6263 2e6a 736f 6e2e 677a 222c 2074  "abc.json.gz", t
+000126a0: 7432 5f69 6e66 6f29 0a0a 2020 2020 2020  t2_info)..      
+000126b0: 2020 7665 7269 6679 5f74 696d 6573 7461    verify_timesta
+000126c0: 6d70 7328 7469 6d69 6e67 2e73 7461 7274  mps(timing.start
+000126d0: 2c20 7469 6d69 6e67 2e65 6e64 2c20 7474  , timing.end, tt
+000126e0: 325f 696e 666f 290a 0a20 2020 2020 2020  2_info)..       
+000126f0: 2065 7870 6563 7465 645f 696e 666f 203d   expected_info =
+00012700: 207b 2a2a 6578 7065 6374 6564 5f69 6e66   {**expected_inf
+00012710: 6f5f 6261 7365 2c20 226e 616d 6522 3a20  o_base, "name": 
+00012720: 696d 706f 7274 5f73 6f75 7263 655f 6e61  import_source_na
+00012730: 6d65 7d0a 2020 2020 2020 2020 7769 7468  me}.        with
+00012740: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00012750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012760: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+00012770: 7065 6374 6564 5f69 6e66 6f2c 2074 7432  pected_info, tt2
+00012780: 5f69 6e66 6f29 0a20 2020 2020 2020 2077  _info).        w
+00012790: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+000127a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000127b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000127c0: 2873 756d 2874 742e 616c 6c2e 6129 2c20  (sum(tt.all.a), 
+000127d0: 7375 6d28 7474 322e 616c 6c2e 6129 290a  sum(tt2.all.a)).
+000127e0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000127f0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00012800: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012810: 7365 7274 4571 7561 6c28 7375 6d28 7474  sertEqual(sum(tt
+00012820: 2e61 6c6c 2e62 292c 2073 756d 2874 7432  .all.b), sum(tt2
+00012830: 2e61 6c6c 2e62 2929 0a20 2020 2020 2020  .all.b)).       
+00012840: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00012850: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00012860: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00012870: 616c 2873 756d 2874 742e 616c 6c2e 6329  al(sum(tt.all.c)
+00012880: 2c20 7375 6d28 7474 322e 616c 6c2e 6329  , sum(tt2.all.c)
+00012890: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000128a0: 6373 765f 696d 706f 7274 5f73 6f75 7263  csv_import_sourc
+000128b0: 655f 696e 666f 2873 656c 6629 3a0a 2020  e_info(self):.  
+000128c0: 2020 2020 2020 696d 706f 7274 7320 3d20        imports = 
+000128d0: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
+000128e0: 6162 632e 6373 7622 2c20 6c74 2e49 6d70  abc.csv", lt.Imp
+000128f0: 6f72 7453 6f75 7263 6554 7970 652e 6669  ortSourceType.fi
+00012900: 6c65 292c 0a20 2020 2020 2020 2020 2020  le),.           
+00012910: 2028 2261 6263 2e74 7376 222c 206c 742e   ("abc.tsv", lt.
+00012920: 496d 706f 7274 536f 7572 6365 5479 7065  ImportSourceType
+00012930: 2e66 696c 6529 2c0a 2020 2020 2020 2020  .file),.        
+00012940: 2020 2020 2822 6162 632e 786c 7378 222c      ("abc.xlsx",
+00012950: 206c 742e 496d 706f 7274 536f 7572 6365   lt.ImportSource
+00012960: 5479 7065 2e66 696c 6529 2c0a 2020 2020  Type.file),.    
+00012970: 2020 2020 2020 2020 2822 6162 632e 6373          ("abc.cs
+00012980: 762e 7a69 7022 2c20 6c74 2e49 6d70 6f72  v.zip", lt.Impor
+00012990: 7453 6f75 7263 6554 7970 652e 7a69 7029  tSourceType.zip)
+000129a0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+000129b0: 6162 632e 6373 762e 677a 222c 206c 742e  abc.csv.gz", lt.
+000129c0: 496d 706f 7274 536f 7572 6365 5479 7065  ImportSourceType
+000129d0: 2e67 7a69 7029 2c0a 2020 2020 2020 2020  .gzip),.        
+000129e0: 2020 2020 2822 6162 632e 6373 762e 787a      ("abc.csv.xz
+000129f0: 222c 206c 742e 496d 706f 7274 536f 7572  ", lt.ImportSour
+00012a00: 6365 5479 7065 2e6c 7a6d 6129 2c0a 2020  ceType.lzma),.  
+00012a10: 2020 2020 2020 2020 2020 2822 612c 622c            ("a,b,
+00012a20: 635c 6e31 2c32 2c33 222c 206c 742e 496d  c\n1,2,3", lt.Im
+00012a30: 706f 7274 536f 7572 6365 5479 7065 2e73  portSourceType.s
+00012a40: 7472 696e 6729 2c0a 2020 2020 2020 2020  tring),.        
+00012a50: 5d0a 2020 2020 2020 2020 666f 7220 666e  ].        for fn
+00012a60: 616d 652c 2065 7870 6563 7465 645f 7479  ame, expected_ty
+00012a70: 7065 2069 6e20 696d 706f 7274 733a 0a20  pe in imports:. 
+00012a80: 2020 2020 2020 2020 2020 2069 6620 225c             if "\
+00012a90: 6e22 206e 6f74 2069 6e20 666e 616d 653a  n" not in fname:
 00012aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ab0: 2061 6464 6564 5f76 616c 7565 203d 2073   added_value = s
-00012ac0: 656c 662e 6865 6164 6572 735b 2256 616c  elf.headers["Val
-00012ad0: 7565 225d 0a20 2020 2020 2020 2020 2020  ue"].           
-00012ae0: 2020 2020 2073 656c 662e 6c6f 675f 6d65       self.log_me
-00012af0: 7373 6167 6528 6622 7265 6365 6976 6564  ssage(f"received
-00012b00: 2068 6561 6465 7220 2756 616c 7565 2720   header 'Value' 
-00012b10: 7b61 6464 6564 5f76 616c 7565 2172 7d22  {added_value!r}"
-00012b20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012b30: 2020 7365 6c66 2e6c 6f67 5f6d 6573 7361    self.log_messa
-00012b40: 6765 2822 6162 6f75 7420 746f 2072 6561  ge("about to rea
-00012b50: 6420 6672 6f6d 2072 6669 6c65 2229 0a20  d from rfile"). 
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00012b70: 6464 6564 5f63 6f6c 756d 6e20 3d20 7365  dded_column = se
-00012b80: 6c66 2e72 6669 6c65 2e72 6561 6428 696e  lf.rfile.read(in
-00012b90: 7428 7365 6c66 2e68 6561 6465 7273 2e67  t(self.headers.g
-00012ba0: 6574 2827 436f 6e74 656e 742d 4c65 6e67  et('Content-Leng
-00012bb0: 7468 272c 2027 3127 2929 290a 2020 2020  th', '1'))).    
-00012bc0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00012bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012be0: 2020 2020 2061 6464 6564 5f63 6f6c 756d       added_colum
-00012bf0: 6e5f 7374 7220 3d20 6164 6465 645f 636f  n_str = added_co
-00012c00: 6c75 6d6e 2e64 6563 6f64 6528 290a 2020  lumn.decode().  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00012c20: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00012c30: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00012c40: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00012c50: 675f 6d65 7373 6167 6528 6622 4572 726f  g_message(f"Erro
-00012c60: 7220 6465 636f 6469 6e67 2061 6464 6564  r decoding added
-00012c70: 2063 6f6c 756d 6e3a 207b 7479 7065 2865   column: {type(e
-00012c80: 292e 5f5f 6e61 6d65 5f5f 7d3a 207b 657d  ).__name__}: {e}
-00012c90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00012ca0: 2020 2020 2020 2061 6464 6564 5f63 6f6c         added_col
-00012cb0: 756d 6e5f 7374 7220 3d20 2265 7272 6f72  umn_str = "error
-00012cc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00012cd0: 2020 7365 6c66 2e6c 6f67 5f6d 6573 7361    self.log_messa
-00012ce0: 6765 2822 7265 6164 2066 726f 6d20 7266  ge("read from rf
-00012cf0: 696c 6520 636f 6d70 6c65 7465 2229 0a20  ile complete"). 
-00012d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012d10: 656c 662e 6c6f 675f 6d65 7373 6167 6528  elf.log_message(
-00012d20: 6622 7265 6365 6976 6564 2062 6f64 7920  f"received body 
-00012d30: 7b61 6464 6564 5f63 6f6c 756d 6e21 727d  {added_column!r}
-00012d40: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00012d50: 2020 2020 7365 6e64 5f62 7974 6573 203d      send_bytes =
-00012d60: 2062 2222 0a20 2020 2020 2020 2020 2020   b"".           
-00012d70: 2020 2020 2069 6620 7061 7468 2e73 7461       if path.sta
-00012d80: 7274 7377 6974 6828 222f 6162 632e 6373  rtswith("/abc.cs
-00012d90: 7622 293a 0a20 2020 2020 2020 2020 2020  v"):.           
-00012da0: 2020 2020 2020 2020 2073 656e 645f 6279           send_by
-00012db0: 7465 7320 2b3d 2066 2261 2c62 2c63 2c7b  tes += f"a,b,c,{
-00012dc0: 6164 6465 645f 636f 6c75 6d6e 5f73 7472  added_column_str
-00012dd0: 7d5c 6e31 2c32 2c33 2c7b 6164 6465 645f  }\n1,2,3,{added_
-00012de0: 7661 6c75 657d 5c6e 222e 656e 636f 6465  value}\n".encode
-00012df0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00012e00: 2020 2020 7365 6c66 2e73 656e 645f 7265      self.send_re
-00012e10: 7370 6f6e 7365 2848 5454 5053 7461 7475  sponse(HTTPStatu
-00012e20: 732e 4f4b 290a 2020 2020 2020 2020 2020  s.OK).          
-00012e30: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00012e40: 6865 6164 6572 2822 436f 6e74 656e 742d  header("Content-
-00012e50: 4c65 6e67 7468 222c 2073 7472 286c 656e  Length", str(len
-00012e60: 2873 656e 645f 6279 7465 7329 2929 0a20  (send_bytes))). 
-00012e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012e80: 656c 662e 656e 645f 6865 6164 6572 7328  elf.end_headers(
-00012e90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012ea0: 2020 7365 6c66 2e77 6669 6c65 2e77 7269    self.wfile.wri
-00012eb0: 7465 2873 656e 645f 6279 7465 7329 0a0a  te(send_bytes)..
-00012ec0: 2020 2020 2020 2020 6465 6620 7275 6e28          def run(
-00012ed0: 7365 7276 6572 5f63 6c61 7373 3d48 5454  server_class=HTT
-00012ee0: 5053 6572 7665 722c 2068 616e 646c 6572  PServer, handler
-00012ef0: 5f63 6c61 7373 3d43 5356 5465 7374 5265  _class=CSVTestRe
-00012f00: 7175 6573 7448 616e 646c 6572 293a 0a20  questHandler):. 
-00012f10: 2020 2020 2020 2020 2020 2073 6572 7665             serve
-00012f20: 725f 6164 6472 6573 7320 3d20 2827 272c  r_address = ('',
-00012f30: 2038 3838 3829 0a20 2020 2020 2020 2020   8888).         
-00012f40: 2020 2068 7474 7064 203d 2073 6572 7665     httpd = serve
-00012f50: 725f 636c 6173 7328 7365 7276 6572 5f61  r_class(server_a
-00012f60: 6464 7265 7373 2c20 6861 6e64 6c65 725f  ddress, handler_
-00012f70: 636c 6173 7329 0a20 2020 2020 2020 2020  class).         
-00012f80: 2020 2068 7474 7064 2e73 6572 7665 5f66     httpd.serve_f
-00012f90: 6f72 6576 6572 2829 0a0a 2020 2020 2020  orever()..      
-00012fa0: 2020 6465 6620 7275 6e5f 6261 636b 6772    def run_backgr
-00012fb0: 6f75 6e64 5f74 6573 745f 7365 7276 6572  ound_test_server
-00012fc0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012fd0: 7020 3d20 7468 7265 6164 696e 672e 5468  p = threading.Th
-00012fe0: 7265 6164 2874 6172 6765 743d 7275 6e29  read(target=run)
-00012ff0: 0a20 2020 2020 2020 2020 2020 2070 2e73  .            p.s
-00013000: 7461 7274 2829 0a0a 2020 2020 2020 2020  tart()..        
-00013010: 2020 2020 666f 7220 7472 6965 735f 7265      for tries_re
-00013020: 6d61 696e 696e 6720 696e 2072 6576 6572  maining in rever
-00013030: 7365 6428 7261 6e67 6528 3230 2929 3a0a  sed(range(20)):.
-00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00013060: 2020 2020 2020 2020 2077 6974 6820 7572           with ur
-00013070: 6c6c 6962 2e72 6571 7565 7374 2e75 726c  llib.request.url
-00013080: 6f70 656e 2822 6874 7470 3a2f 2f6c 6f63  open("http://loc
-00013090: 616c 686f 7374 3a38 3838 382f 2229 3a0a  alhost:8888/"):.
+00012ab0: 2069 6d70 6f72 745f 6e61 6d65 203d 2022   import_name = "
+00012ac0: 7465 7374 2f22 202b 2066 6e61 6d65 0a20  test/" + fname. 
+00012ad0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00012ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012af0: 2069 6d70 6f72 745f 6e61 6d65 203d 2066   import_name = f
+00012b00: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00012b10: 2069 6620 696d 706f 7274 5f6e 616d 652e   if import_name.
+00012b20: 656e 6473 7769 7468 2822 2e63 7376 2229  endswith(".csv")
+00012b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012b40: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00012b50: 2829 2e63 7376 5f69 6d70 6f72 7428 696d  ().csv_import(im
+00012b60: 706f 7274 5f6e 616d 6529 0a20 2020 2020  port_name).     
+00012b70: 2020 2020 2020 2065 6c69 6620 696d 706f         elif impo
+00012b80: 7274 5f6e 616d 652e 656e 6473 7769 7468  rt_name.endswith
+00012b90: 2822 2e78 6c73 7822 293a 0a20 2020 2020  (".xlsx"):.     
+00012ba0: 2020 2020 2020 2020 2020 2074 626c 203d             tbl =
+00012bb0: 206c 742e 5461 626c 6528 292e 6578 6365   lt.Table().exce
+00012bc0: 6c5f 696d 706f 7274 2869 6d70 6f72 745f  l_import(import_
+00012bd0: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00012be0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012bf0: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
+00012c00: 2e54 6162 6c65 2829 2e74 7376 5f69 6d70  .Table().tsv_imp
+00012c10: 6f72 7428 696d 706f 7274 5f6e 616d 6529  ort(import_name)
+00012c20: 0a0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00012c30: 696e 7428 7265 7072 2869 6d70 6f72 745f  int(repr(import_
+00012c40: 6e61 6d65 292c 2074 626c 2e69 6d70 6f72  name), tbl.impor
+00012c50: 745f 736f 7572 6365 2c20 7462 6c2e 696d  t_source, tbl.im
+00012c60: 706f 7274 5f73 6f75 7263 655f 7479 7065  port_source_type
+00012c70: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00012c80: 6620 225c 6e22 206e 6f74 2069 6e20 666e  f "\n" not in fn
+00012c90: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00012ca0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00012cb0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012cd0: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
+00012ce0: 6d70 6f72 745f 6e61 6d65 2c20 7462 6c2e  mport_name, tbl.
+00012cf0: 696d 706f 7274 5f73 6f75 7263 6529 0a20  import_source). 
+00012d00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00012d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d20: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00012d30: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00012d40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00012d50: 7373 6572 7445 7175 616c 284e 6f6e 652c  ssertEqual(None,
+00012d60: 2074 626c 2e69 6d70 6f72 745f 736f 7572   tbl.import_sour
+00012d70: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
+00012d80: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00012d90: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00012da0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00012db0: 4571 7561 6c28 6578 7065 6374 6564 5f74  Equal(expected_t
+00012dc0: 7970 652c 2074 626c 2e69 6d70 6f72 745f  ype, tbl.import_
+00012dd0: 736f 7572 6365 5f74 7970 6529 0a0a 2020  source_type)..  
+00012de0: 2020 6465 6620 7465 7374 5f63 7376 5f69    def test_csv_i
+00012df0: 6d70 6f72 745f 6672 6f6d 5f75 726c 2873  mport_from_url(s
+00012e00: 656c 6629 3a0a 2020 2020 2020 2020 6672  elf):.        fr
+00012e10: 6f6d 2068 7474 702e 7365 7276 6572 2069  om http.server i
+00012e20: 6d70 6f72 7420 4854 5450 5365 7276 6572  mport HTTPServer
+00012e30: 2c20 4261 7365 4854 5450 5265 7175 6573  , BaseHTTPReques
+00012e40: 7448 616e 646c 6572 0a20 2020 2020 2020  tHandler.       
+00012e50: 2066 726f 6d20 6874 7470 2069 6d70 6f72   from http impor
+00012e60: 7420 4854 5450 5374 6174 7573 0a20 2020  t HTTPStatus.   
+00012e70: 2020 2020 2069 6d70 6f72 7420 7468 7265       import thre
+00012e80: 6164 696e 670a 2020 2020 2020 2020 696d  ading.        im
+00012e90: 706f 7274 2074 696d 650a 2020 2020 2020  port time.      
+00012ea0: 2020 696d 706f 7274 2075 726c 6c69 622e    import urllib.
+00012eb0: 6572 726f 720a 2020 2020 2020 2020 696d  error.        im
+00012ec0: 706f 7274 2075 726c 6c69 622e 7265 7175  port urllib.requ
+00012ed0: 6573 740a 0a20 2020 2020 2020 2069 6620  est..        if 
+00012ee0: 534b 4950 5f43 5356 5f49 4d50 4f52 545f  SKIP_CSV_IMPORT_
+00012ef0: 5553 494e 475f 5552 4c5f 5445 5354 533a  USING_URL_TESTS:
+00012f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012f10: 662e 736b 6970 5465 7374 2822 4353 5620  f.skipTest("CSV 
+00012f20: 696d 706f 7274 2074 6573 7473 2073 6b69  import tests ski
+00012f30: 7070 6564 2229 0a0a 2020 2020 2020 2020  pped")..        
+00012f40: 636c 6173 7320 4353 5654 6573 7452 6571  class CSVTestReq
+00012f50: 7565 7374 4861 6e64 6c65 7228 4261 7365  uestHandler(Base
+00012f60: 4854 5450 5265 7175 6573 7448 616e 646c  HTTPRequestHandl
+00012f70: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00012f80: 2064 6566 2064 6f5f 4745 5428 7365 6c66   def do_GET(self
+00012f90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012fa0: 2020 2073 656c 662e 6c6f 675f 6d65 7373     self.log_mess
+00012fb0: 6167 6528 6622 7265 6365 6976 6564 207b  age(f"received {
+00012fc0: 7365 6c66 2e63 6f6d 6d61 6e64 7d20 7b73  self.command} {s
+00012fd0: 656c 662e 7061 7468 7d22 290a 2020 2020  elf.path}").    
+00012fe0: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00012ff0: 203d 2073 656c 662e 7061 7468 0a20 2020   = self.path.   
+00013000: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00013010: 645f 6279 7465 7320 3d20 6222 220a 2020  d_bytes = b"".  
+00013020: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013030: 2070 6174 6820 3d3d 2022 2f45 5849 5422   path == "/EXIT"
+00013040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013050: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
+00013060: 7265 7370 6f6e 7365 2848 5454 5053 7461  response(HTTPSta
+00013070: 7475 732e 4f4b 290a 2020 2020 2020 2020  tus.OK).        
+00013080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013090: 2e65 6e64 5f68 6561 6465 7273 2829 0a20  .end_headers(). 
 000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-000130c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000130d0: 6365 7074 2075 726c 6c69 622e 6572 726f  cept urllib.erro
-000130e0: 722e 5552 4c45 7272 6f72 3a0a 2020 2020  r.URLError:.    
-000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 6966 2074 7269 6573 5f72 656d 6169 6e69  if tries_remaini
-00013110: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00013120: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00013130: 2e73 6c65 6570 2830 2e32 3529 0a0a 2020  .sleep(0.25)..  
-00013140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013150: 2070 0a0a 2020 2020 2020 2020 7765 625f   p..        web_
-00013160: 6164 6472 6573 7320 3d20 2268 7474 703a  address = "http:
-00013170: 2f2f 6c6f 6361 6c68 6f73 743a 3838 3838  //localhost:8888
-00013180: 220a 2020 2020 2020 2020 7020 3d20 7275  ".        p = ru
-00013190: 6e5f 6261 636b 6772 6f75 6e64 5f74 6573  n_background_tes
-000131a0: 745f 7365 7276 6572 2829 0a0a 2020 2020  t_server()..    
-000131b0: 2020 2020 7572 6c20 3d20 7765 625f 6164      url = web_ad
-000131c0: 6472 6573 7320 2b20 222f 6162 632e 6373  dress + "/abc.cs
-000131d0: 7622 0a20 2020 2020 2020 2074 7279 3a0a  v".        try:.
-000131e0: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
-000131f0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00013200: 5f69 6d70 6f72 7428 7572 6c29 0a20 2020  _import(url).   
-00013210: 2020 2020 2020 2020 2074 626c 3220 3d20           tbl2 = 
-00013220: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00013230: 6d70 6f72 7428 0a20 2020 2020 2020 2020  mport(.         
-00013240: 2020 2020 2020 2075 726c 2c0a 2020 2020         url,.    
-00013250: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00013260: 3d62 2265 7874 7261 222c 0a20 2020 2020  =b"extra",.     
-00013270: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00013280: 7273 3d7b 2256 414c 5545 223a 2022 3130  rs={"VALUE": "10
-00013290: 3022 7d2c 0a20 2020 2020 2020 2020 2020  0"},.           
-000132a0: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
-000132b0: 7b7d 2e66 726f 6d6b 6579 7328 2261 2062  {}.fromkeys("a b
-000132c0: 2063 2065 7874 7261 222e 7370 6c69 7428   c extra".split(
-000132d0: 292c 2069 6e74 292c 0a20 2020 2020 2020  ), int),.       
-000132e0: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
-000132f0: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-00013300: 2020 2020 7769 7468 2075 726c 6c69 622e      with urllib.
-00013310: 7265 7175 6573 742e 7572 6c6f 7065 6e28  request.urlopen(
-00013320: 7765 625f 6164 6472 6573 7320 2b20 222f  web_address + "/
-00013330: 4558 4954 2229 3a0a 2020 2020 2020 2020  EXIT"):.        
-00013340: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00013350: 2020 2020 2020 2020 2070 2e6a 6f69 6e28           p.join(
-00013360: 290a 0a20 2020 2020 2020 2074 626c 2e70  )..        tbl.p
-00013370: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-00013380: 2074 626c 322e 7072 6573 656e 7428 290a   tbl2.present().
-00013390: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000133a0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-000133b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000133c0: 7373 6572 7445 7175 616c 2875 726c 2c20  ssertEqual(url, 
-000133d0: 7462 6c2e 696d 706f 7274 5f73 6f75 7263  tbl.import_sourc
-000133e0: 6529 0a20 2020 2020 2020 2077 6974 6820  e).        with 
-000133f0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00013400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013410: 2e61 7373 6572 7445 7175 616c 286c 742e  .assertEqual(lt.
-00013420: 496d 706f 7274 536f 7572 6365 5479 7065  ImportSourceType
-00013430: 2e75 726c 2c20 7462 6c2e 696d 706f 7274  .url, tbl.import
-00013440: 5f73 6f75 7263 655f 7479 7065 290a 0a20  _source_type).. 
-00013450: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00013460: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00013470: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00013480: 6572 7445 7175 616c 2822 6120 6220 6320  ertEqual("a b c 
-00013490: 6578 7472 6122 2e73 706c 6974 2829 2c20  extra".split(), 
-000134a0: 7462 6c32 2e69 6e66 6f28 295b 2266 6965  tbl2.info()["fie
-000134b0: 6c64 7322 5d29 0a20 2020 2020 2020 2077  lds"]).        w
-000134c0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-000134d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000134e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000134f0: 2831 3030 2c20 7462 6c32 5b30 5d2e 6578  (100, tbl2[0].ex
-00013500: 7472 6129 0a0a 2020 2020 6465 6620 7465  tra)..    def te
-00013510: 7374 5f63 7376 5f66 696c 7465 7265 645f  st_csv_filtered_
-00013520: 696d 706f 7274 2873 656c 6629 3a0a 2020  import(self):.  
-00013530: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00013540: 3d20 330a 2020 2020 2020 2020 7474 203d  = 3.        tt =
-00013550: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00013560: 696d 706f 7274 2822 7465 7374 2f61 6263  import("test/abc
-00013570: 2e63 7376 222c 2074 7261 6e73 666f 726d  .csv", transform
-00013580: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
-00013590: 2261 6263 222c 2069 6e74 2929 0a20 2020  "abc", int)).   
-000135a0: 2020 2020 2070 7269 6e74 2822 6162 632e       print("abc.
-000135b0: 6373 7622 2c20 7474 2e69 6e66 6f28 2929  csv", tt.info())
-000135c0: 0a0a 2020 2020 2020 2020 7474 203d 206c  ..        tt = l
-000135d0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-000135e0: 706f 7274 2822 7465 7374 2f61 6263 2e63  port("test/abc.c
-000135f0: 7376 222c 2074 7261 6e73 666f 726d 733d  sv", transforms=
-00013600: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-00013610: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00013640: 6c74 6572 733d 7b22 6322 3a20 6c74 2e54  lters={"c": lt.T
-00013650: 6162 6c65 2e65 7128 3129 7d29 0a20 2020  able.eq(1)}).   
-00013660: 2020 2020 2070 7269 6e74 2874 742e 696e       print(tt.in
-00013670: 666f 2829 290a 2020 2020 2020 2020 7769  fo()).        wi
-00013680: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00013690: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000136a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000136b0: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
-000136c0: 5f73 697a 652c 206c 656e 2874 7429 290a  _size, len(tt)).
-000136d0: 0a20 2020 2020 2020 2074 7420 3d20 6c74  .        tt = lt
-000136e0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-000136f0: 6f72 7428 2274 6573 742f 6162 632e 6373  ort("test/abc.cs
-00013700: 7622 2c20 7472 616e 7366 6f72 6d73 3d64  v", transforms=d
-00013710: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
-00013720: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00013750: 7465 7273 3d7b 2263 223a 2031 7d29 0a20  ters={"c": 1}). 
-00013760: 2020 2020 2020 2070 7269 6e74 2874 742e         print(tt.
-00013770: 696e 666f 2829 290a 2020 2020 2020 2020  info()).        
-00013780: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00013790: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-000137a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000137b0: 6c28 7465 7374 5f73 697a 6520 2a20 7465  l(test_size * te
-000137c0: 7374 5f73 697a 652c 206c 656e 2874 7429  st_size, len(tt)
-000137d0: 290a 0a20 2020 2020 2020 2074 7420 3d20  )..        tt = 
-000137e0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-000137f0: 6d70 6f72 7428 2274 6573 742f 6162 632e  mport("test/abc.
-00013800: 6373 7622 2c20 7472 616e 7366 6f72 6d73  csv", transforms
-00013810: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00013820: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013850: 696c 7465 7273 3d7b 2263 223a 206c 616d  ilters={"c": lam
-00013860: 6264 6120 783a 2030 203c 2078 203c 2032  bda x: 0 < x < 2
-00013870: 7d29 0a20 2020 2020 2020 2070 7269 6e74  }).        print
-00013880: 2874 742e 696e 666f 2829 290a 2020 2020  (tt.info()).    
-00013890: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000138a0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000138b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000138c0: 4571 7561 6c28 7465 7374 5f73 697a 6520  Equal(test_size 
-000138d0: 2a20 7465 7374 5f73 697a 652c 206c 656e  * test_size, len
-000138e0: 2874 7429 290a 0a20 2020 2020 2020 2023  (tt))..        #
-000138f0: 2074 6573 7420 616c 6c20 7370 6563 6961   test all specia
-00013900: 6c20 636f 6d70 6172 6174 6f72 7320 7768  l comparators wh
-00013910: 656e 2075 7365 6420 6173 2066 696c 7465  en used as filte
-00013920: 7273 0a20 2020 2020 2020 2023 2020 2020  rs.        #    
-00013930: 2069 735f 6e6f 6e65 202d 2061 7474 7269   is_none - attri
-00013940: 6275 7465 2076 616c 7565 2069 7320 4e6f  bute value is No
-00013950: 6e65 0a20 2020 2020 2020 2023 2020 2020  ne.        #    
-00013960: 2069 735f 6e6f 745f 6e6f 6e65 202d 2061   is_not_none - a
-00013970: 7474 7269 6275 7465 2076 616c 7565 2069  ttribute value i
-00013980: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00013990: 2020 2023 2020 2020 2069 735f 6e75 6c6c     #     is_null
-000139a0: 202d 2061 7474 7269 6275 7465 2076 616c   - attribute val
-000139b0: 7565 2069 7320 4e6f 6e65 2c20 2222 2c20  ue is None, "", 
-000139c0: 6f72 206e 6f74 2064 6566 696e 6564 0a20  or not defined. 
-000139d0: 2020 2020 2020 2023 2020 2020 2069 735f         #     is_
-000139e0: 6e6f 745f 6e75 6c6c 202d 2061 7474 7269  not_null - attri
-000139f0: 6275 7465 2076 616c 7565 2069 7320 6465  bute value is de
-00013a00: 6669 6e65 642c 2061 6e64 2069 7320 6e6f  fined, and is no
-00013a10: 7420 4e6f 6e65 206f 7220 2222 0a20 2020  t None or "".   
-00013a20: 2020 2020 2023 2020 2020 2073 7461 7274       #     start
-00013a30: 7377 6974 6820 2d20 6174 7472 6962 7574  swith - attribut
-00013a40: 6520 7661 6c75 6520 7374 6172 7473 2077  e value starts w
-00013a50: 6974 6820 6120 6769 7665 6e20 7374 7269  ith a given stri
-00013a60: 6e67 0a20 2020 2020 2020 2023 2020 2020  ng.        #    
-00013a70: 2065 6e64 7377 6974 6820 2d20 6174 7472   endswith - attr
-00013a80: 6962 7574 6520 7661 6c75 6520 656e 6473  ibute value ends
-00013a90: 2077 6974 6820 6120 6769 7665 6e20 7374   with a given st
-00013aa0: 7269 6e67 0a20 2020 2020 2020 2023 2020  ring.        #  
-00013ab0: 2020 2072 655f 6d61 7463 6820 2d20 6174     re_match - at
-00013ac0: 7472 6962 7574 6520 7661 6c75 6520 6d61  tribute value ma
-00013ad0: 7463 6865 7320 6120 7265 6775 6c61 7220  tches a regular 
-00013ae0: 6578 7072 6573 7369 6f6e 0a0a 2020 2020  expression..    
-00013af0: 2020 2020 7072 696e 7428 290a 2020 2020      print().    
-00013b00: 2020 2020 696e 7075 745f 6461 7461 203d      input_data =
-00013b10: 2074 6578 7477 7261 702e 6465 6465 6e74   textwrap.dedent
-00013b20: 2822 2222 5c0a 2020 2020 2020 2020 6e61  ("""\.        na
-00013b30: 6d65 2c61 2c62 2c63 0a20 2020 2020 2020  me,a,b,c.       
-00013b40: 2022 4122 2c31 3030 2c31 3030 2c31 3030   "A",100,100,100
-00013b50: 0a20 2020 2020 2020 2022 4222 2c32 3030  .        "B",200
-00013b60: 2c2c 3230 300a 2020 2020 2020 2020 2241  ,,200.        "A
-00013b70: 3122 2c31 3031 2c31 3031 2c31 3031 0a20  1",101,101,101. 
-00013b80: 2020 2020 2020 2022 4231 222c 3230 312c         "B1",201,
-00013b90: 2c32 3031 0a20 2020 2020 2020 2022 4331  ,201.        "C1
-00013ba0: 222c 3330 312c 2c33 3031 0a20 2020 2020  ",301,,301.     
-00013bb0: 2020 202c 3939 2c39 392c 3939 0a20 2020     ,99,99,99.   
-00013bc0: 2020 2020 2022 2222 290a 2020 2020 2020       """).      
-00013bd0: 2020 6c74 2e54 6162 6c65 2829 2e63 7376    lt.Table().csv
-00013be0: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
-00013bf0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 2020 7472 616e 7366 6f72 6d73 3d64 6963    transforms=dic
-00013c20: 742e 6672 6f6d 6b65 7973 2822 6162 6322  t.fromkeys("abc"
-00013c30: 2c20 696e 7429 2c0a 2020 2020 2020 2020  , int),.        
-00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 2020 2020 2020 292e 7072 6573 656e 7428        ).present(
-00013c60: 290a 0a20 2020 2020 2020 2022 2222 0a20  )..        """. 
-00013c70: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-00013c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013c90: 2d2b 0a20 2020 2020 2020 207c 204e 616d  -+.        | Nam
-00013ca0: 6520 7c20 2020 4120 7c20 2020 2042 207c  e |   A |    B |
-00013cb0: 2020 2043 207c 0a20 2020 2020 2020 207c     C |.        |
-00013cc0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2b2d 2d2d  ------+-----+---
-00013cd0: 2d2d 2d2b 2d2d 2d2d 2d7c 0a20 2020 2020  ---+-----|.     
-00013ce0: 2020 207c 2041 2020 2020 7c20 3130 3020     | A    | 100 
-00013cf0: 7c20 2031 3030 207c 2031 3030 207c 0a20  |  100 | 100 |. 
-00013d00: 2020 2020 2020 207c 2042 2020 2020 7c20         | B    | 
-00013d10: 3230 3020 7c20 4e6f 6e65 207c 2032 3030  200 | None | 200
-00013d20: 207c 0a20 2020 2020 2020 207c 2041 3120   |.        | A1 
-00013d30: 2020 7c20 3130 3120 7c20 2031 3031 207c    | 101 |  101 |
-00013d40: 2031 3031 207c 0a20 2020 2020 2020 207c   101 |.        |
-00013d50: 2042 3120 2020 7c20 3230 3120 7c20 4e6f   B1   | 201 | No
-00013d60: 6e65 207c 2032 3031 207c 0a20 2020 2020  ne | 201 |.     
-00013d70: 2020 207c 2043 3120 2020 7c20 3330 3120     | C1   | 301 
-00013d80: 7c20 4e6f 6e65 207c 2033 3031 207c 0a20  | None | 301 |. 
-00013d90: 2020 2020 2020 207c 2020 2020 2020 7c20         |      | 
-00013da0: 2039 3920 7c20 2020 3939 207c 2020 3939   99 |   99 |  99
-00013db0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
-00013dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013dd0: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2022  -----+.        "
-00013de0: 2222 0a0a 2020 2020 2020 2020 7072 696e  ""..        prin
-00013df0: 7428 2269 735f 6e6f 6e65 2829 2229 0a20  t("is_none()"). 
-00013e00: 2020 2020 2020 2078 203d 206c 742e 5461         x = lt.Ta
-00013e10: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00013e20: 2869 6e70 7574 5f64 6174 612c 0a20 2020  (input_data,.   
-00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e50: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-00013e60: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00013e70: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
-00013e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 2020 2066 696c 7465 7273 3d7b 2262       filters={"b
-00013eb0: 223a 206c 742e 5461 626c 652e 6973 5f6e  ": lt.Table.is_n
-00013ec0: 6f6e 6528 297d 290a 2020 2020 2020 2020  one()}).        
-00013ed0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00013ee0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00013ef0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00013f00: 6c28 332c 206c 656e 2878 2929 0a20 2020  l(3, len(x)).   
-00013f10: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00013f20: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-00013f30: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00013f40: 7454 7275 6528 616c 6c28 6220 6973 204e  tTrue(all(b is N
-00013f50: 6f6e 6520 666f 7220 6220 696e 2078 2e61  one for b in x.a
-00013f60: 6c6c 2e62 2929 0a0a 2020 2020 2020 2020  ll.b))..        
-00013f70: 7072 696e 7428 2269 735f 6e6f 745f 6e6f  print("is_not_no
-00013f80: 6e65 2829 2229 0a20 2020 2020 2020 2078  ne()").        x
-00013f90: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-00013fa0: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
-00013fb0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00013fe0: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
-00013ff0: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
-00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014010: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014020: 696c 7465 7273 3d7b 2262 223a 206c 742e  ilters={"b": lt.
-00014030: 5461 626c 652e 6973 5f6e 6f74 5f6e 6f6e  Table.is_not_non
-00014040: 6528 297d 290a 2020 2020 2020 2020 7769  e()}).        wi
-00014050: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00014060: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00014070: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00014080: 332c 206c 656e 2878 2929 0a20 2020 2020  3, len(x)).     
-00014090: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000140a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000140b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000140c0: 7175 616c 2833 3030 2c20 7375 6d28 782e  qual(300, sum(x.
-000140d0: 616c 6c2e 6229 290a 0a20 2020 2020 2020  all.b))..       
-000140e0: 2070 7269 6e74 2822 6220 6973 5f6e 756c   print("b is_nul
-000140f0: 6c28 2922 290a 2020 2020 2020 2020 7820  l()").        x 
-00014100: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00014110: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
-00014120: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-00014150: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00014160: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00014190: 6c74 6572 733d 7b22 6222 3a20 6c74 2e54  lters={"b": lt.T
-000141a0: 6162 6c65 2e69 735f 6e75 6c6c 2829 7d29  able.is_null()})
-000141b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000141c0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-000141d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000141e0: 7373 6572 7445 7175 616c 2833 2c20 6c65  ssertEqual(3, le
-000141f0: 6e28 7829 290a 2020 2020 2020 2020 7769  n(x)).        wi
-00014200: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00014210: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00014220: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
-00014230: 6c6c 2862 2069 7320 4e6f 6e65 2066 6f72  ll(b is None for
-00014240: 2062 2069 6e20 782e 616c 6c2e 6229 290a   b in x.all.b)).
-00014250: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00014260: 6220 6973 5f6e 6f74 5f6e 756c 6c28 2922  b is_not_null()"
-00014270: 290a 2020 2020 2020 2020 7820 3d20 6c74  ).        x = lt
-00014280: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-00014290: 6f72 7428 696e 7075 745f 6461 7461 2c0a  ort(input_data,.
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142c0: 2020 7472 616e 7366 6f72 6d73 3d64 6963    transforms=dic
-000142d0: 742e 6672 6f6d 6b65 7973 2822 6162 6322  t.fromkeys("abc"
-000142e0: 2c20 696e 7429 2c0a 2020 2020 2020 2020  , int),.        
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014300: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
-00014310: 733d 7b22 6222 3a20 6c74 2e54 6162 6c65  s={"b": lt.Table
-00014320: 2e69 735f 6e6f 745f 6e75 6c6c 2829 7d29  .is_not_null()})
-00014330: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00014340: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00014350: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00014360: 7373 6572 7445 7175 616c 2833 2c20 6c65  ssertEqual(3, le
-00014370: 6e28 7829 290a 2020 2020 2020 2020 7769  n(x)).        wi
-00014380: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00014390: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000143a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000143b0: 3330 302c 2073 756d 2878 2e61 6c6c 2e62  300, sum(x.all.b
-000143c0: 2929 0a0a 2020 2020 2020 2020 7072 696e  ))..        prin
-000143d0: 7428 226e 616d 6520 6973 5f6e 756c 6c28  t("name is_null(
-000143e0: 2922 290a 2020 2020 2020 2020 7820 3d20  )").        x = 
-000143f0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00014400: 6d70 6f72 7428 696e 7075 745f 6461 7461  mport(input_data
-00014410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014430: 2020 2020 7472 616e 7366 6f72 6d73 3d64      transforms=d
-00014440: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
-00014450: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
-00014460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014470: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00014480: 6572 733d 7b22 6e61 6d65 223a 206c 742e  ers={"name": lt.
-00014490: 5461 626c 652e 6973 5f6e 756c 6c28 297d  Table.is_null()}
-000144a0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-000144b0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-000144c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000144d0: 6173 7365 7274 4571 7561 6c28 312c 206c  assertEqual(1, l
-000144e0: 656e 2878 2929 0a20 2020 2020 2020 2077  en(x)).        w
-000144f0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00014500: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014510: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00014520: 2833 2a39 392c 2078 5b30 5d2e 6120 2b20  (3*99, x[0].a + 
-00014530: 785b 305d 2e62 202b 2078 5b30 5d2e 6329  x[0].b + x[0].c)
-00014540: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00014550: 226e 616d 6520 6973 5f6e 6f74 5f6e 756c  "name is_not_nul
-00014560: 6c28 2922 290a 2020 2020 2020 2020 7820  l()").        x 
-00014570: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00014580: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
-00014590: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-000145a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145b0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-000145c0: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-000145d0: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
-000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145f0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00014600: 6c74 6572 733d 7b22 6e61 6d65 223a 206c  lters={"name": l
-00014610: 742e 5461 626c 652e 6973 5f6e 6f74 5f6e  t.Table.is_not_n
-00014620: 756c 6c28 297d 290a 2020 2020 2020 2020  ull()}).        
-00014630: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00014640: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00014650: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00014660: 6c28 352c 206c 656e 2878 2929 0a20 2020  l(5, len(x)).   
-00014670: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00014680: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-00014690: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000146a0: 7445 7175 616c 2822 4120 4220 4131 2042  tEqual("A B A1 B
-000146b0: 3120 4331 222e 7370 6c69 7428 292c 206c  1 C1".split(), l
-000146c0: 6973 7428 782e 616c 6c2e 6e61 6d65 2929  ist(x.all.name))
-000146d0: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-000146e0: 226e 616d 6520 7374 6172 7473 7769 7468  "name startswith
-000146f0: 2827 4227 2922 290a 2020 2020 2020 2020  ('B')").        
-00014700: 7820 3d20 6c74 2e54 6162 6c65 2829 2e63  x = lt.Table().c
-00014710: 7376 5f69 6d70 6f72 7428 696e 7075 745f  sv_import(input_
-00014720: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014740: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00014750: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
-00014760: 2822 6162 6322 2c20 696e 7429 2c0a 2020  ("abc", int),.  
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014790: 6669 6c74 6572 733d 7b22 6e61 6d65 223a  filters={"name":
-000147a0: 206c 742e 5461 626c 652e 7374 6172 7473   lt.Table.starts
-000147b0: 7769 7468 2822 4222 297d 290a 2020 2020  with("B")}).    
-000147c0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000147d0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000147e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000147f0: 4571 7561 6c28 322c 206c 656e 2878 2929  Equal(2, len(x))
-00014800: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00014810: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00014820: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00014830: 7373 6572 7445 7175 616c 2822 4220 4231  ssertEqual("B B1
-00014840: 222e 7370 6c69 7428 292c 206c 6973 7428  ".split(), list(
-00014850: 782e 616c 6c2e 6e61 6d65 2929 0a0a 2020  x.all.name))..  
-00014860: 2020 2020 2020 7072 696e 7428 226e 616d        print("nam
-00014870: 6520 656e 6473 7769 7468 2827 3127 2922  e endswith('1')"
-00014880: 290a 2020 2020 2020 2020 7820 3d20 6c74  ).        x = lt
-00014890: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-000148a0: 6f72 7428 696e 7075 745f 6461 7461 2c0a  ort(input_data,.
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2020 7472 616e 7366 6f72 6d73 3d64 6963    transforms=dic
-000148e0: 742e 6672 6f6d 6b65 7973 2822 6162 6322  t.fromkeys("abc"
-000148f0: 2c20 696e 7429 2c0a 2020 2020 2020 2020  , int),.        
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
-00014920: 733d 7b22 6e61 6d65 223a 206c 742e 5461  s={"name": lt.Ta
-00014930: 626c 652e 656e 6473 7769 7468 2822 3122  ble.endswith("1"
-00014940: 297d 290a 2020 2020 2020 2020 7769 7468  )}).        with
-00014950: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00014960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014970: 662e 6173 7365 7274 4571 7561 6c28 332c  f.assertEqual(3,
-00014980: 206c 656e 2878 2929 0a20 2020 2020 2020   len(x)).       
-00014990: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-000149a0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-000149b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000149c0: 616c 2822 4131 2042 3120 4331 222e 7370  al("A1 B1 C1".sp
-000149d0: 6c69 7428 292c 206c 6973 7428 782e 616c  lit(), list(x.al
-000149e0: 6c2e 6e61 6d65 2929 0a0a 2020 2020 2020  l.name))..      
-000149f0: 2020 7072 696e 7428 7222 6e61 6d65 2072    print(r"name r
-00014a00: 655f 6d61 7463 6828 7227 5b41 425d 5c64  e_match(r'[AB]\d
-00014a10: 2729 2229 0a20 2020 2020 2020 2078 203d  ')").        x =
-00014a20: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00014a30: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
-00014a40: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a60: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
-00014a70: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-00014a80: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014aa0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00014ab0: 7465 7273 3d7b 226e 616d 6522 3a20 6c74  ters={"name": lt
-00014ac0: 2e54 6162 6c65 2e72 655f 6d61 7463 6828  .Table.re_match(
-00014ad0: 7222 5b41 425d 5c64 2229 7d29 0a20 2020  r"[AB]\d")}).   
-00014ae0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00014af0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-00014b00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00014b10: 7445 7175 616c 2832 2c20 6c65 6e28 7829  tEqual(2, len(x)
-00014b20: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00014b30: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00014b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014b50: 6173 7365 7274 4571 7561 6c28 2241 3120  assertEqual("A1 
-00014b60: 4231 222e 7370 6c69 7428 292c 206c 6973  B1".split(), lis
-00014b70: 7428 782e 616c 6c2e 6e61 6d65 2929 0a0a  t(x.all.name))..
-00014b80: 2020 2020 6465 6620 7465 7374 5f63 7376      def test_csv
-00014b90: 5f73 7472 696e 675f 696d 706f 7274 2873  _string_import(s
-00014ba0: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00014bb0: 7461 203d 2063 7376 5f64 6174 610a 2020  ta = csv_data.  
-00014bc0: 2020 2020 2020 6373 7674 6162 6c65 203d        csvtable =
-00014bd0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00014be0: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
-00014bf0: 653d 6461 7461 2c20 7472 616e 7366 6f72  e=data, transfor
-00014c00: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
-00014c10: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
-00014c20: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
-00014c30: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
-00014c40: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
-00014c50: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-00014c60: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00014c70: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-00014c80: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00014c90: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00014ca0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00014cb0: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
-00014cc0: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
-00014cd0: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
-00014ce0: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
-00014cf0: 6970 2874 312c 2063 7376 7461 626c 6529  ip(t1, csvtable)
-00014d00: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-00014d10: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00014d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014d30: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
-00014d40: 2831 2066 6f72 206c 696e 6520 696e 2064  (1 for line in d
-00014d50: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
-00014d60: 2069 6620 6c69 6e65 2e73 7472 6970 2829   if line.strip()
-00014d70: 292d 312c 206c 656e 2863 7376 7461 626c  )-1, len(csvtabl
-00014d80: 6529 290a 0a20 2020 2020 2020 2072 6f77  e))..        row
-00014d90: 5f70 726f 746f 7479 7065 203d 2073 656c  _prototype = sel
-00014da0: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-00014db0: 6374 2830 2c20 302c 2030 290a 2020 2020  ct(0, 0, 0).    
-00014dc0: 2020 2020 6373 7674 6162 6c65 3220 3d20      csvtable2 = 
-00014dd0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00014de0: 6d70 6f72 7428 6461 7461 2c20 7472 616e  mport(data, tran
-00014df0: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
-00014e00: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
-00014e10: 2069 6e74 7d2c 0a20 2020 2020 2020 2020   int},.         
-00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 2072 6f77 5f63 6c61 7373 3d74 7970 6528   row_class=type(
-00014e50: 726f 775f 7072 6f74 6f74 7970 6529 295b  row_prototype))[
-00014e60: 3a33 5d0a 0a20 2020 2020 2020 2070 7269  :3]..        pri
-00014e70: 6e74 2874 7970 6528 7431 5b30 5d29 2e5f  nt(type(t1[0])._
-00014e80: 5f6e 616d 655f 5f2c 2074 315b 305d 290a  _name__, t1[0]).
-00014e90: 2020 2020 2020 2020 7072 696e 7428 7479          print(ty
-00014ea0: 7065 2863 7376 7461 626c 6532 5b30 5d29  pe(csvtable2[0])
-00014eb0: 2e5f 5f6e 616d 655f 5f2c 2063 7376 7461  .__name__, csvta
-00014ec0: 626c 6532 5b30 5d29 0a20 2020 2020 2020  ble2[0]).       
-00014ed0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00014ee0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00014ef0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00014f00: 616c 2874 7970 6528 7431 5b30 5d29 2c20  al(type(t1[0]), 
-00014f10: 7479 7065 2863 7376 7461 626c 6532 5b30  type(csvtable2[0
-00014f20: 5d29 290a 0a20 2020 2064 6566 2074 6573  ]))..    def tes
-00014f30: 745f 6373 765f 6c69 6d69 745f 696d 706f  t_csv_limit_impo
-00014f40: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
-00014f50: 2020 6461 7461 203d 2063 7376 5f64 6174    data = csv_dat
-00014f60: 610a 2020 2020 2020 2020 696d 706f 7274  a.        import
-00014f70: 5f6c 696d 6974 203d 2031 300a 2020 2020  _limit = 10.    
-00014f80: 2020 2020 6373 7674 6162 6c65 203d 206c      csvtable = l
-00014f90: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-00014fa0: 706f 7274 2863 7376 5f73 6f75 7263 653d  port(csv_source=
-00014fb0: 6461 7461 2c20 7472 616e 7366 6f72 6d73  data, transforms
-00014fc0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
-00014fd0: 2069 6e74 2c20 2763 273a 2069 6e74 7d2c   int, 'c': int},
-00014fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015000: 2020 2020 2020 2020 2020 6c69 6d69 743d            limit=
-00015010: 696d 706f 7274 5f6c 696d 6974 290a 0a20  import_limit).. 
-00015020: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00015030: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00015040: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00015050: 6572 7445 7175 616c 2869 6d70 6f72 745f  ertEqual(import_
-00015060: 6c69 6d69 742c 206c 656e 2863 7376 7461  limit, len(csvta
-00015070: 626c 6529 290a 0a20 2020 2020 2020 2063  ble))..        c
-00015080: 7376 7461 626c 6520 3d20 6c74 2e54 6162  svtable = lt.Tab
-00015090: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-000150a0: 6373 765f 736f 7572 6365 3d64 6174 612c  csv_source=data,
-000150b0: 2074 7261 6e73 666f 726d 733d 7b27 6127   transforms={'a'
-000150c0: 3a20 696e 742c 2027 6227 3a20 696e 742c  : int, 'b': int,
-000150d0: 2027 6327 3a20 696e 747d 2c0a 2020 2020   'c': int},.    
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 2020 206c 696d 6974 3d30 290a 0a20       limit=0).. 
-00015110: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00015120: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00015130: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00015140: 6572 7445 7175 616c 2830 2c20 6c65 6e28  ertEqual(0, len(
-00015150: 6373 7674 6162 6c65 2929 0a0a 2020 2020  csvtable))..    
-00015160: 6465 6620 7465 7374 5f63 7376 5f73 7472  def test_csv_str
-00015170: 696e 675f 6c69 7374 5f69 6d70 6f72 7428  ing_list_import(
-00015180: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
-00015190: 6174 6120 3d20 6373 765f 6461 7461 0a20  ata = csv_data. 
-000151a0: 2020 2020 2020 2063 7376 7461 626c 6520         csvtable 
-000151b0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-000151c0: 5f69 6d70 6f72 7428 6373 765f 736f 7572  _import(csv_sour
-000151d0: 6365 3d64 6174 612e 7370 6c69 746c 696e  ce=data.splitlin
-000151e0: 6573 2829 2c20 7472 616e 7366 6f72 6d73  es(), transforms
-000151f0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
-00015200: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
-00015210: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
-00015220: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
-00015230: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
-00015240: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
-00015250: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
-00015260: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
-00015270: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00015280: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00015290: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-000152a0: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
-000152b0: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
-000152c0: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
-000152d0: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
-000152e0: 2874 312c 2063 7376 7461 626c 6529 2929  (t1, csvtable)))
-000152f0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00015300: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00015310: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015320: 7373 6572 7445 7175 616c 2873 756d 2831  ssertEqual(sum(1
-00015330: 2066 6f72 206c 696e 6520 696e 2064 6174   for line in dat
-00015340: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
-00015350: 6620 6c69 6e65 2e73 7472 6970 2829 292d  f line.strip())-
-00015360: 312c 206c 656e 2863 7376 7461 626c 6529  1, len(csvtable)
-00015370: 290a 0a20 2020 2020 2020 2072 6f77 5f70  )..        row_p
-00015380: 726f 746f 7479 7065 203d 2073 656c 662e  rototype = self.
-00015390: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-000153a0: 2830 2c20 302c 2030 290a 2020 2020 2020  (0, 0, 0).      
-000153b0: 2020 6373 7674 6162 6c65 3220 3d20 6c74    csvtable2 = lt
-000153c0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-000153d0: 6f72 7428 6461 7461 2c20 7472 616e 7366  ort(data, transf
-000153e0: 6f72 6d73 3d7b 2761 273a 2069 6e74 2c20  orms={'a': int, 
-000153f0: 2762 273a 2069 6e74 2c20 2763 273a 2069  'b': int, 'c': i
-00015400: 6e74 7d2c 0a20 2020 2020 2020 2020 2020  nt},.           
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00015430: 6f77 5f63 6c61 7373 3d74 7970 6528 726f  ow_class=type(ro
-00015440: 775f 7072 6f74 6f74 7970 6529 295b 3a33  w_prototype))[:3
-00015450: 5d0a 0a20 2020 2020 2020 2070 7269 6e74  ]..        print
-00015460: 2874 7970 6528 7431 5b30 5d29 2e5f 5f6e  (type(t1[0]).__n
-00015470: 616d 655f 5f2c 2074 315b 305d 290a 2020  ame__, t1[0]).  
-00015480: 2020 2020 2020 7072 696e 7428 7479 7065        print(type
-00015490: 2863 7376 7461 626c 6532 5b30 5d29 2e5f  (csvtable2[0])._
-000154a0: 5f6e 616d 655f 5f2c 2063 7376 7461 626c  _name__, csvtabl
-000154b0: 6532 5b30 5d29 0a20 2020 2020 2020 2077  e2[0]).        w
-000154c0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-000154d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000154e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000154f0: 2874 7970 6528 7431 5b30 5d29 2c20 7479  (type(t1[0]), ty
-00015500: 7065 2863 7376 7461 626c 6532 5b30 5d29  pe(csvtable2[0])
-00015510: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00015520: 6373 765f 6e75 6d65 7269 635f 7472 616e  csv_numeric_tran
-00015530: 7366 6f72 6d73 2873 656c 6629 3a0a 2020  sforms(self):.  
-00015540: 2020 2020 2020 6461 7461 203d 2074 6578        data = tex
-00015550: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
-00015560: 5c0a 2020 2020 2020 2020 2020 2020 7479  \.            ty
-00015570: 7065 2c76 616c 7565 0a20 2020 2020 2020  pe,value.       
-00015580: 2020 2020 2069 6e74 2c31 3030 300a 2020       int,1000.  
-00015590: 2020 2020 2020 2020 2020 666c 6f61 742c            float,
-000155a0: 332e 3134 0a20 2020 2020 2020 2020 2020  3.14.           
-000155b0: 2065 6d70 7479 2c0a 2020 2020 2020 2020   empty,.        
-000155c0: 2020 2020 7374 722c e293 a02a 6265 7274      str,...*bert
-000155d0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-000155e0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-000155f0: 7365 6c66 2e73 7562 5465 7374 2822 636f  self.subTest("co
-00015600: 6e76 6572 745f 6e75 6d65 7269 6322 293a  nvert_numeric"):
-00015610: 0a20 2020 2020 2020 2020 2020 2074 626c  .            tbl
-00015620: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-00015630: 765f 696d 706f 7274 2864 6174 612c 2074  v_import(data, t
-00015640: 7261 6e73 666f 726d 733d 7b27 7661 6c75  ransforms={'valu
-00015650: 6527 3a20 6c74 2e54 6162 6c65 2e63 6f6e  e': lt.Table.con
-00015660: 7665 7274 5f6e 756d 6572 6963 7d29 0a20  vert_numeric}). 
-00015670: 2020 2020 2020 2020 2020 2074 626c 2e70             tbl.p
-00015680: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-00015690: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000156a0: 4571 7561 6c28 5b31 3030 302c 2033 2e31  Equal([1000, 3.1
-000156b0: 342c 2027 272c 2027 e293 a02a 6265 7274  4, '', '...*bert
-000156c0: 275d 2c20 6c69 7374 2874 626c 2e61 6c6c  '], list(tbl.all
-000156d0: 2e76 616c 7565 2929 0a0a 2020 2020 2020  .value))..      
-000156e0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-000156f0: 6573 7428 2263 6f6e 7665 7274 5f6e 756d  est("convert_num
-00015700: 6572 6963 2829 2229 3a0a 2020 2020 2020  eric()"):.      
-00015710: 2020 2020 2020 7462 6c20 3d20 6c74 2e54        tbl = lt.T
-00015720: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-00015730: 7428 6461 7461 2c20 7472 616e 7366 6f72  t(data, transfor
-00015740: 6d73 3d7b 2776 616c 7565 273a 206c 742e  ms={'value': lt.
-00015750: 5461 626c 652e 636f 6e76 6572 745f 6e75  Table.convert_nu
-00015760: 6d65 7269 6328 297d 290a 2020 2020 2020  meric()}).      
-00015770: 2020 2020 2020 7462 6c2e 7072 6573 656e        tbl.presen
-00015780: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00015790: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000157a0: 285b 3130 3030 2c20 332e 3134 2c20 2727  ([1000, 3.14, ''
-000157b0: 2c20 27e2 93a0 2a62 6572 7427 5d2c 206c  , '...*bert'], l
-000157c0: 6973 7428 7462 6c2e 616c 6c2e 7661 6c75  ist(tbl.all.valu
-000157d0: 6529 290a 0a20 2020 2020 2020 2077 6974  e))..        wit
-000157e0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-000157f0: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
-00015800: 6e6f 6e5f 6e75 6d65 7269 633d 4e6f 6e65  non_numeric=None
-00015810: 2922 293a 0a20 2020 2020 2020 2020 2020  )"):.           
-00015820: 2074 626c 203d 206c 742e 5461 626c 6528   tbl = lt.Table(
-00015830: 292e 6373 765f 696d 706f 7274 2864 6174  ).csv_import(dat
-00015840: 612c 2074 7261 6e73 666f 726d 733d 7b27  a, transforms={'
-00015850: 7661 6c75 6527 3a20 6c74 2e54 6162 6c65  value': lt.Table
-00015860: 2e63 6f6e 7665 7274 5f6e 756d 6572 6963  .convert_numeric
-00015870: 286e 6f6e 5f6e 756d 6572 6963 3d4e 6f6e  (non_numeric=Non
-00015880: 6529 7d29 0a20 2020 2020 2020 2020 2020  e)}).           
-00015890: 2074 626c 2e70 7265 7365 6e74 2829 0a20   tbl.present(). 
-000158a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000158b0: 6173 7365 7274 4571 7561 6c28 5b31 3030  assertEqual([100
-000158c0: 302c 2033 2e31 342c 2027 272c 204e 6f6e  0, 3.14, '', Non
-000158d0: 655d 2c20 6c69 7374 2874 626c 2e61 6c6c  e], list(tbl.all
-000158e0: 2e76 616c 7565 2929 0a0a 2020 2020 2020  .value))..      
-000158f0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00015900: 6573 7428 2263 6f6e 7665 7274 5f6e 756d  est("convert_num
-00015910: 6572 6963 286e 6f6e 5f6e 756d 6572 6963  eric(non_numeric
-00015920: 3d30 2922 293a 0a20 2020 2020 2020 2020  =0)"):.         
-00015930: 2020 2074 626c 203d 206c 742e 5461 626c     tbl = lt.Tabl
-00015940: 6528 292e 6373 765f 696d 706f 7274 2864  e().csv_import(d
-00015950: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
-00015960: 7b27 7661 6c75 6527 3a20 6c74 2e54 6162  {'value': lt.Tab
-00015970: 6c65 2e63 6f6e 7665 7274 5f6e 756d 6572  le.convert_numer
-00015980: 6963 286e 6f6e 5f6e 756d 6572 6963 3d30  ic(non_numeric=0
-00015990: 297d 290a 2020 2020 2020 2020 2020 2020  )}).            
-000159a0: 7462 6c2e 7072 6573 656e 7428 290a 2020  tbl.present().  
-000159b0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000159c0: 7373 6572 7445 7175 616c 285b 3130 3030  ssertEqual([1000
-000159d0: 2c20 332e 3134 2c20 2727 2c20 305d 2c20  , 3.14, '', 0], 
-000159e0: 6c69 7374 2874 626c 2e61 6c6c 2e76 616c  list(tbl.all.val
-000159f0: 7565 2929 0a0a 2020 2020 2020 2020 7769  ue))..        wi
-00015a00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00015a10: 2263 6f6e 7665 7274 5f6e 756d 6572 6963  "convert_numeric
-00015a20: 2869 6e74 5f74 6f5f 666c 6f61 743d 5472  (int_to_float=Tr
-00015a30: 7565 2922 293a 0a20 2020 2020 2020 2020  ue)"):.         
-00015a40: 2020 2074 626c 203d 206c 742e 5461 626c     tbl = lt.Tabl
-00015a50: 6528 292e 6373 765f 696d 706f 7274 2864  e().csv_import(d
-00015a60: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
-00015a70: 7b27 7661 6c75 6527 3a20 6c74 2e54 6162  {'value': lt.Tab
-00015a80: 6c65 2e63 6f6e 7665 7274 5f6e 756d 6572  le.convert_numer
-00015a90: 6963 2866 6f72 6365 5f66 6c6f 6174 3d54  ic(force_float=T
-00015aa0: 7275 6529 7d29 0a20 2020 2020 2020 2020  rue)}).         
-00015ab0: 2020 2074 626c 2e70 7265 7365 6e74 2829     tbl.present()
-00015ac0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015ad0: 662e 6173 7365 7274 4571 7561 6c28 5b31  f.assertEqual([1
-00015ae0: 3030 302e 302c 2033 2e31 342c 2027 272c  000.0, 3.14, '',
-00015af0: 2027 e293 a02a 6265 7274 275d 2c20 6c69   '...*bert'], li
-00015b00: 7374 2874 626c 2e61 6c6c 2e76 616c 7565  st(tbl.all.value
-00015b10: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-00015b20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00015b30: 5b66 6c6f 6174 2c20 666c 6f61 742c 2073  [float, float, s
-00015b40: 7472 2c20 7374 725d 2c20 6c69 7374 2874  tr, str], list(t
-00015b50: 7970 6528 7629 2066 6f72 2076 2069 6e20  ype(v) for v in 
-00015b60: 7462 6c2e 616c 6c2e 7661 6c75 6529 290a  tbl.all.value)).
-00015b70: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00015b80: 6c66 2e73 7562 5465 7374 2822 636f 6e76  lf.subTest("conv
-00015b90: 6572 745f 6e75 6d65 7269 6328 6e6f 6e5f  ert_numeric(non_
-00015ba0: 6e75 6d65 7269 633d 4e6f 6e65 2c20 656d  numeric=None, em
-00015bb0: 7074 793d 4e6f 6e65 2922 293a 0a20 2020  pty=None)"):.   
-00015bc0: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
-00015bd0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-00015be0: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
-00015bf0: 666f 726d 733d 7b27 7661 6c75 6527 3a20  forms={'value': 
-00015c00: 6c74 2e54 6162 6c65 2e63 6f6e 7665 7274  lt.Table.convert
-00015c10: 5f6e 756d 6572 6963 286e 6f6e 5f6e 756d  _numeric(non_num
-00015c20: 6572 6963 3d4e 6f6e 652c 2065 6d70 7479  eric=None, empty
-00015c30: 3d4e 6f6e 6529 7d29 0a20 2020 2020 2020  =None)}).       
-00015c40: 2020 2020 2074 626c 2e70 7265 7365 6e74       tbl.present
-00015c50: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00015c60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00015c70: 5b31 3030 302c 2033 2e31 342c 204e 6f6e  [1000, 3.14, Non
-00015c80: 652c 204e 6f6e 655d 2c20 6c69 7374 2874  e, None], list(t
-00015c90: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
-00015ca0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00015cb0: 662e 7375 6254 6573 7428 2263 6f6e 7665  f.subTest("conve
-00015cc0: 7274 5f6e 756d 6572 6963 2865 6d70 7479  rt_numeric(empty
-00015cd0: 3d4e 6f6e 6529 2229 3a0a 2020 2020 2020  =None)"):.      
-00015ce0: 2020 2020 2020 7462 6c20 3d20 6c74 2e54        tbl = lt.T
-00015cf0: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
-00015d00: 7428 6461 7461 2c20 7472 616e 7366 6f72  t(data, transfor
-00015d10: 6d73 3d7b 2776 616c 7565 273a 206c 742e  ms={'value': lt.
-00015d20: 5461 626c 652e 636f 6e76 6572 745f 6e75  Table.convert_nu
-00015d30: 6d65 7269 6328 656d 7074 793d 4e6f 6e65  meric(empty=None
-00015d40: 297d 290a 2020 2020 2020 2020 2020 2020  )}).            
-00015d50: 7462 6c2e 7072 6573 656e 7428 290a 2020  tbl.present().  
-00015d60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015d70: 7373 6572 7445 7175 616c 285b 3130 3030  ssertEqual([1000
-00015d80: 2c20 332e 3134 2c20 4e6f 6e65 2c20 27e2  , 3.14, None, '.
-00015d90: 93a0 2a62 6572 7427 5d2c 206c 6973 7428  ..*bert'], list(
-00015da0: 7462 6c2e 616c 6c2e 7661 6c75 6529 290a  tbl.all.value)).
-00015db0: 0a20 2020 2064 6566 2074 6573 745f 6a73  .    def test_js
-00015dc0: 6f6e 5f65 7870 6f72 745f 7374 7265 616d  on_export_stream
-00015dd0: 696e 6728 7365 6c66 293a 0a20 2020 2020  ing(self):.     
-00015de0: 2020 2066 726f 6d20 6974 6572 746f 6f6c     from itertool
-00015df0: 7320 696d 706f 7274 2070 6572 6d75 7461  s import permuta
-00015e00: 7469 6f6e 730a 2020 2020 2020 2020 7465  tions.        te
-00015e10: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
-00015e20: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
-00015e30: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-00015e40: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-00015e50: 7465 7374 5f73 697a 6529 0a20 2020 2020  test_size).     
-00015e60: 2020 2066 6f72 2066 6965 6c64 6e61 6d65     for fieldname
-00015e70: 7320 696e 2070 6572 6d75 7461 7469 6f6e  s in permutation
-00015e80: 7328 6c69 7374 2827 6162 6327 2929 3a0a  s(list('abc')):.
-00015e90: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
-00015ea0: 7374 7269 6e67 203d 2074 312e 6a73 6f6e  string = t1.json
-00015eb0: 5f65 7870 6f72 7428 4e6f 6e65 2c20 6669  _export(None, fi
-00015ec0: 656c 646e 616d 6573 3d66 6965 6c64 6e61  eldnames=fieldna
-00015ed0: 6d65 732c 2073 7472 6561 6d69 6e67 3d54  mes, streaming=T
-00015ee0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00015ef0: 206f 7574 6c69 6e65 7320 3d20 6f75 745f   outlines = out_
-00015f00: 7374 7269 6e67 2e73 706c 6974 6c69 6e65  string.splitline
-00015f10: 7328 290a 0a20 2020 2020 2020 2020 2020  s()..           
-00015f20: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00015f30: 7374 2866 6965 6c64 6e61 6d65 733d 6669  st(fieldnames=fi
-00015f40: 656c 646e 616d 6573 293a 0a20 2020 2020  eldnames):.     
-00015f50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015f60: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-00015f70: 5f73 697a 652a 2a33 2c20 6c65 6e28 6f75  _size**3, len(ou
-00015f80: 746c 696e 6573 2929 0a0a 2020 2020 2020  tlines))..      
-00015f90: 2020 2020 2020 666f 7220 6f62 2c20 6c69        for ob, li
-00015fa0: 6e65 2069 6e20 7a69 7028 7431 2c20 6f75  ne in zip(t1, ou
-00015fb0: 746c 696e 6573 293a 0a20 2020 2020 2020  tlines):.       
-00015fc0: 2020 2020 2020 2020 206a 736f 6e5f 6469           json_di
-00015fd0: 6374 203d 206a 736f 6e2e 6c6f 6164 7328  ct = json.loads(
-00015fe0: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
-00015ff0: 2020 2020 2020 7431 5f64 6174 616f 626a        t1_dataobj
-00016000: 203d 206d 616b 655f 6461 7461 6f62 6a65   = make_dataobje
-00016010: 6374 5f66 726f 6d5f 6f62 286f 6229 0a20  ct_from_ob(ob). 
-00016020: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00016030: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00016040: 286f 623d 6f62 2c20 6c69 6e65 3d6c 696e  (ob=ob, line=lin
-00016050: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00016060: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00016070: 6572 7445 7175 616c 2874 315f 6461 7461  ertEqual(t1_data
-00016080: 6f62 6a2c 206c 742e 4461 7461 4f62 6a65  obj, lt.DataObje
-00016090: 6374 282a 2a6a 736f 6e5f 6469 6374 2929  ct(**json_dict))
-000160a0: 0a0a 2020 2020 6465 6620 7465 7374 5f6a  ..    def test_j
-000160b0: 736f 6e5f 6578 706f 7274 5f6e 6f6e 7374  son_export_nonst
-000160c0: 7265 616d 696e 6728 7365 6c66 293a 0a20  reaming(self):. 
-000160d0: 2020 2020 2020 2066 726f 6d20 6974 6572         from iter
-000160e0: 746f 6f6c 7320 696d 706f 7274 2070 6572  tools import per
-000160f0: 6d75 7461 7469 6f6e 730a 2020 2020 2020  mutations.      
-00016100: 2020 696d 706f 7274 206a 736f 6e0a 2020    import json.  
-00016110: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00016120: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-00016130: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00016140: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00016150: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-00016160: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
-00016170: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
-00016180: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
-00016190: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
-000161a0: 2020 2020 6f75 745f 7374 7269 6e67 203d      out_string =
-000161b0: 2074 312e 6a73 6f6e 5f65 7870 6f72 7428   t1.json_export(
-000161c0: 4e6f 6e65 2c20 6669 656c 646e 616d 6573  None, fieldnames
-000161d0: 3d66 6965 6c64 6e61 6d65 732c 2073 7472  =fieldnames, str
-000161e0: 6561 6d69 6e67 3d46 616c 7365 290a 2020  eaming=False).  
-000161f0: 2020 2020 2020 2020 2020 6f62 7365 7276            observ
-00016200: 6564 5f6a 736f 6e20 3d20 6a73 6f6e 2e6c  ed_json = json.l
-00016210: 6f61 6473 286f 7574 5f73 7472 696e 6729  oads(out_string)
-00016220: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00016230: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00016240: 6669 656c 646e 616d 6573 3d66 6965 6c64  fieldnames=field
-00016250: 6e61 6d65 7329 3a0a 2020 2020 2020 2020  names):.        
-00016260: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00016270: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00016280: 7a65 2a2a 332c 206c 656e 286f 6273 6572  ze**3, len(obser
-00016290: 7665 645f 6a73 6f6e 2929 0a0a 2020 2020  ved_json))..    
-000162a0: 2020 2020 2020 2020 666f 7220 6f62 2c20          for ob, 
-000162b0: 6a73 6f6e 5f64 6963 7420 696e 207a 6970  json_dict in zip
-000162c0: 2874 312c 206f 6273 6572 7665 645f 6a73  (t1, observed_js
-000162d0: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
-000162e0: 2020 2020 2074 315f 6461 7461 6f62 6a20       t1_dataobj 
-000162f0: 3d20 6d61 6b65 5f64 6174 616f 626a 6563  = make_dataobjec
-00016300: 745f 6672 6f6d 5f6f 6228 6f62 290a 2020  t_from_ob(ob).  
-00016310: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00016320: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00016330: 6f62 3d6f 622c 206a 736f 6e5f 6469 6374  ob=ob, json_dict
-00016340: 3d6a 736f 6e5f 6469 6374 293a 0a20 2020  =json_dict):.   
-00016350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016360: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00016370: 6c28 7431 5f64 6174 616f 626a 2c20 6c74  l(t1_dataobj, lt
-00016380: 2e44 6174 614f 626a 6563 7428 2a2a 6a73  .DataObject(**js
-00016390: 6f6e 5f64 6963 7429 290a 0a20 2020 2064  on_dict))..    d
-000163a0: 6566 2074 6573 745f 6a73 6f6e 5f69 6d70  ef test_json_imp
-000163b0: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
-000163c0: 2020 2064 6174 6120 3d20 6a73 6f6e 5f64     data = json_d
-000163d0: 6174 610a 2020 2020 2020 2020 696e 6a73  ata.        injs
-000163e0: 6f6e 203d 2069 6f2e 5374 7269 6e67 494f  on = io.StringIO
-000163f0: 2864 6174 6129 0a20 2020 2020 2020 206a  (data).        j
-00016400: 736f 6e74 6162 6c65 203d 206c 742e 5461  sontable = lt.Ta
-00016410: 626c 6528 292e 6a73 6f6e 5f69 6d70 6f72  ble().json_impor
-00016420: 7428 696e 6a73 6f6e 2c20 7374 7265 616d  t(injson, stream
-00016430: 696e 673d 5472 7565 2c20 7472 616e 7366  ing=True, transf
-00016440: 6f72 6d73 3d7b 2761 273a 2069 6e74 2c20  orms={'a': int, 
-00016450: 2762 273a 2069 6e74 2c20 2763 273a 2069  'b': int, 'c': i
-00016460: 6e74 7d29 0a0a 2020 2020 2020 2020 7465  nt})..        te
-00016470: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
-00016480: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
-00016490: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-000164a0: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-000164b0: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
-000164c0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000164d0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000164e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000164f0: 5472 7565 2861 6c6c 286d 616b 655f 6461  True(all(make_da
-00016500: 7461 6f62 6a65 6374 5f66 726f 6d5f 6f62  taobject_from_ob
-00016510: 2872 6563 3129 203d 3d20 7265 6332 2066  (rec1) == rec2 f
-00016520: 6f72 2072 6563 312c 2072 6563 3220 696e  or rec1, rec2 in
-00016530: 207a 6970 2874 312c 206a 736f 6e74 6162   zip(t1, jsontab
-00016540: 6c65 2929 290a 2020 2020 2020 2020 7769  le))).        wi
-00016550: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00016560: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00016570: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00016580: 6c65 6e28 5b64 2066 6f72 2064 2069 6e20  len([d for d in 
-00016590: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
-000165a0: 2920 6966 2064 2e73 7472 6970 2829 5d29  ) if d.strip()])
-000165b0: 2c20 6c65 6e28 6a73 6f6e 7461 626c 6529  , len(jsontable)
-000165c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000165d0: 6a73 6f6e 5f73 7472 696e 675f 696d 706f  json_string_impo
-000165e0: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
-000165f0: 2020 6461 7461 203d 206a 736f 6e5f 6461    data = json_da
-00016600: 7461 0a20 2020 2020 2020 206a 736f 6e74  ta.        jsont
-00016610: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
-00016620: 292e 6a73 6f6e 5f69 6d70 6f72 7428 6461  ).json_import(da
-00016630: 7461 2c20 7374 7265 616d 696e 673d 5472  ta, streaming=Tr
-00016640: 7565 2c20 7472 616e 7366 6f72 6d73 3d7b  ue, transforms={
-00016650: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
-00016660: 6e74 2c20 2763 273a 2069 6e74 7d29 0a0a  nt, 'c': int})..
-00016670: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-00016680: 6520 3d20 330a 2020 2020 2020 2020 7431  e = 3.        t1
-00016690: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000166a0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000166b0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-000166c0: 697a 6529 0a0a 2020 2020 2020 2020 7769  ize)..        wi
-000166d0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-000166e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000166f0: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
-00016700: 6c6c 286d 616b 655f 6461 7461 6f62 6a65  ll(make_dataobje
-00016710: 6374 5f66 726f 6d5f 6f62 2872 6563 3129  ct_from_ob(rec1)
-00016720: 203d 3d20 7265 6332 2066 6f72 2072 6563   == rec2 for rec
-00016730: 312c 2072 6563 3220 696e 207a 6970 2874  1, rec2 in zip(t
-00016740: 312c 206a 736f 6e74 6162 6c65 2929 290a  1, jsontable))).
-00016750: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00016760: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00016770: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00016780: 7365 7274 4571 7561 6c28 6c65 6e28 5b64  sertEqual(len([d
-00016790: 2066 6f72 2064 2069 6e20 6461 7461 2e73   for d in data.s
-000167a0: 706c 6974 6c69 6e65 7328 2920 6966 2064  plitlines() if d
-000167b0: 2e73 7472 6970 2829 5d29 2c20 6c65 6e28  .strip()]), len(
-000167c0: 6a73 6f6e 7461 626c 6529 290a 0a20 2020  jsontable))..   
-000167d0: 2064 6566 2074 6573 745f 6a73 6f6e 5f73   def test_json_s
-000167e0: 7472 696e 675f 6c69 7374 5f69 6d70 6f72  tring_list_impor
-000167f0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00016800: 2064 6174 6120 3d20 6a73 6f6e 5f64 6174   data = json_dat
-00016810: 610a 2020 2020 2020 2020 6a73 6f6e 7461  a.        jsonta
-00016820: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
-00016830: 2e6a 736f 6e5f 696d 706f 7274 2864 6174  .json_import(dat
-00016840: 612e 7370 6c69 746c 696e 6573 2829 2c20  a.splitlines(), 
-00016850: 7374 7265 616d 696e 673d 5472 7565 2c20  streaming=True, 
-00016860: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
-00016870: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
-00016880: 2763 273a 2069 6e74 7d29 0a0a 2020 2020  'c': int})..    
-00016890: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-000168a0: 330a 2020 2020 2020 2020 7431 203d 206d  3.        t1 = m
-000168b0: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-000168c0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-000168d0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
-000168e0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-000168f0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00016900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016910: 6173 7365 7274 5472 7565 2861 6c6c 286d  assertTrue(all(m
-00016920: 616b 655f 6461 7461 6f62 6a65 6374 5f66  ake_dataobject_f
-00016930: 726f 6d5f 6f62 2872 6563 3129 203d 3d20  rom_ob(rec1) == 
-00016940: 7265 6332 2066 6f72 2072 6563 312c 2072  rec2 for rec1, r
-00016950: 6563 3220 696e 207a 6970 2874 312c 206a  ec2 in zip(t1, j
-00016960: 736f 6e74 6162 6c65 2929 290a 2020 2020  sontable))).    
-00016970: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00016980: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-00016990: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000169a0: 4571 7561 6c28 6c65 6e28 5b64 2066 6f72  Equal(len([d for
-000169b0: 2064 2069 6e20 6461 7461 2e73 706c 6974   d in data.split
-000169c0: 6c69 6e65 7328 2920 6966 2064 2e73 7472  lines() if d.str
-000169d0: 6970 2829 5d29 2c20 6c65 6e28 6a73 6f6e  ip()]), len(json
-000169e0: 7461 626c 6529 290a 0a20 2020 2064 6566  table))..    def
-000169f0: 2074 6573 745f 6a73 6f6e 5f6e 6f6e 7374   test_json_nonst
-00016a00: 7265 616d 696e 675f 7769 7468 5f70 6174  reaming_with_pat
-00016a10: 685f 696d 706f 7274 2873 656c 6629 3a0a  h_import(self):.
-00016a20: 2020 2020 2020 2020 6461 7461 203d 206a          data = j
-00016a30: 736f 6e5f 6461 7461 0a20 2020 2020 2020  son_data.       
-00016a40: 2064 6174 6120 3d20 272c 5c6e 272e 6a6f   data = ',\n'.jo
-00016a50: 696e 2864 6174 612e 7273 7472 6970 2829  in(data.rstrip()
-00016a60: 2e73 706c 6974 6c69 6e65 7328 2929 0a20  .splitlines()). 
-00016a70: 2020 2020 2020 206a 736f 6e5f 696e 7075         json_inpu
-00016a80: 7430 203d 2027 5b27 202b 2064 6174 6120  t0 = '[' + data 
-00016a90: 2b20 275d 270a 2020 2020 2020 2020 6a73  + ']'.        js
-00016aa0: 6f6e 5f69 6e70 7574 3120 3d20 277b 2022  on_input1 = '{ "
-00016ab0: 6461 7461 223a 205b 2720 2b20 6461 7461  data": [' + data
-00016ac0: 202b 2027 5d7d 270a 2020 2020 2020 2020   + ']}'.        
-00016ad0: 6a73 6f6e 5f69 6e70 7574 3220 3d20 277b  json_input2 = '{
-00016ae0: 2022 6461 7461 223a 207b 2022 6974 656d   "data": { "item
-00016af0: 7322 3a20 5b27 202b 2064 6174 6120 2b20  s": [' + data + 
-00016b00: 275d 7d7d 270a 0a20 2020 2020 2020 2066  ']}}'..        f
-00016b10: 6f72 206a 736f 6e5f 696e 7075 742c 2070  or json_input, p
-00016b20: 6174 6820 696e 205b 0a20 2020 2020 2020  ath in [.       
-00016b30: 2020 2020 2028 6a73 6f6e 5f69 6e70 7574       (json_input
-00016b40: 302c 2022 2229 2c0a 2020 2020 2020 2020  0, ""),.        
-00016b50: 2020 2020 286a 736f 6e5f 696e 7075 7431      (json_input1
-00016b60: 2c20 2264 6174 6122 292c 0a20 2020 2020  , "data"),.     
-00016b70: 2020 2020 2020 2028 6a73 6f6e 5f69 6e70         (json_inp
-00016b80: 7574 322c 2022 6461 7461 2e69 7465 6d73  ut2, "data.items
-00016b90: 2229 2c0a 2020 2020 2020 2020 5d3a 0a20  "),.        ]:. 
-00016ba0: 2020 2020 2020 2020 2020 206a 736f 6e74             jsont
-00016bb0: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
-00016bc0: 292e 6a73 6f6e 5f69 6d70 6f72 7428 6a73  ).json_import(js
-00016bd0: 6f6e 5f69 6e70 7574 2c0a 2020 2020 2020  on_input,.      
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 2020 2020 2020 2020 2070 6174 683d 7061           path=pa
-00016c10: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c40: 2020 2074 7261 6e73 666f 726d 733d 7b27     transforms={'
-00016c50: 6127 3a20 696e 742c 2027 6227 3a20 696e  a': int, 'b': in
-00016c60: 742c 2027 6327 3a20 696e 747d 290a 0a20  t, 'c': int}).. 
-00016c70: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-00016c80: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
-00016c90: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
-00016ca0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-00016cb0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-00016cc0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-00016cd0: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-00016ce0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016d00: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-00016d10: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
-00016d20: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
-00016d30: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
-00016d40: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
-00016d50: 2c20 6a73 6f6e 7461 626c 6529 2929 0a20  , jsontable))). 
-00016d60: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00016d70: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d90: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00016da0: 286c 656e 285b 6420 666f 7220 6420 696e  (len([d for d in
-00016db0: 2064 6174 612e 7370 6c69 746c 696e 6573   data.splitlines
-00016dc0: 2829 2069 6620 642e 7374 7269 7028 295d  () if d.strip()]
-00016dd0: 292c 206c 656e 286a 736f 6e74 6162 6c65  ), len(jsontable
-00016de0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-00016df0: 5f6a 736f 6e5f 696d 706f 7274 5f77 6974  _json_import_wit
-00016e00: 685f 6375 7374 6f6d 5f65 6e63 6f64 6572  h_custom_encoder
-00016e10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00016e20: 6672 6f6d 2064 6174 6574 696d 6520 696d  from datetime im
-00016e30: 706f 7274 2064 6174 650a 2020 2020 2020  port date.      
-00016e40: 2020 6461 7461 203d 205b 0a20 2020 2020    data = [.     
-00016e50: 2020 2020 2020 207b 2761 273a 2031 3030         {'a': 100
-00016e60: 2c20 2762 273a 2064 6174 6528 3230 3030  , 'b': date(2000
-00016e70: 2c20 312c 2031 292c 2027 6327 3a20 3230  , 1, 1), 'c': 20
-00016e80: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-00016e90: 7b27 6127 3a20 3130 312c 2027 6227 3a20  {'a': 101, 'b': 
-00016ea0: 6461 7465 2832 3030 312c 2031 2c20 3129  date(2001, 1, 1)
-00016eb0: 2c20 2763 273a 2032 3031 7d2c 0a20 2020  , 'c': 201},.   
-00016ec0: 2020 2020 205d 0a20 2020 2020 2020 2074       ].        t
-00016ed0: 626c 203d 206c 742e 5461 626c 6528 292e  bl = lt.Table().
-00016ee0: 696e 7365 7274 5f6d 616e 7928 6461 7461  insert_many(data
-00016ef0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00016f00: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00016f10: 2854 7970 6545 7272 6f72 293a 0a20 2020  (TypeError):.   
-00016f20: 2020 2020 2020 2020 2078 203d 2074 626c           x = tbl
-00016f30: 2e6a 736f 6e5f 6578 706f 7274 2829 0a0a  .json_export()..
-00016f40: 2020 2020 2020 2020 636c 6173 7320 4a73          class Js
-00016f50: 6f6e 4461 7465 456e 636f 6465 7228 6a73  onDateEncoder(js
-00016f60: 6f6e 2e4a 534f 4e45 6e63 6f64 6572 293a  on.JSONEncoder):
-00016f70: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00016f80: 2064 6566 6175 6c74 2873 656c 662c 206f   default(self, o
-00016f90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016fa0: 2020 2069 6d70 6f72 7420 6461 7465 7469     import dateti
-00016fb0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-00016fc0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00016fd0: 286f 2c20 6461 7465 7469 6d65 2e64 6174  (o, datetime.dat
-00016fe0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00016ff0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00017000: 7472 286f 290a 2020 2020 2020 2020 2020  tr(o).          
-00017010: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00017020: 6572 2829 2e64 6566 6175 6c74 286f 290a  er().default(o).
-00017030: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-00017040: 6420 3d20 7465 7874 7772 6170 2e64 6564  d = textwrap.ded
-00017050: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
-00017060: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00017070: 2020 207b 2261 223a 2031 3030 2c20 2262     {"a": 100, "b
-00017080: 223a 2022 3230 3030 2d30 312d 3031 222c  ": "2000-01-01",
-00017090: 2022 6322 3a20 3230 307d 2c0a 2020 2020   "c": 200},.    
-000170a0: 2020 2020 2020 2020 7b22 6122 3a20 3130          {"a": 10
-000170b0: 312c 2022 6222 3a20 2232 3030 312d 3031  1, "b": "2001-01
-000170c0: 2d30 3122 2c20 2263 223a 2032 3031 7d0a  -01", "c": 201}.
-000170d0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-000170e0: 2020 2020 2020 2020 2020 2222 2229 0a20            """). 
-000170f0: 2020 2020 2020 206a 736f 6e5f 7265 7375         json_resu
-00017100: 6c74 203d 2074 626c 2e6a 736f 6e5f 6578  lt = tbl.json_ex
-00017110: 706f 7274 286a 736f 6e5f 656e 636f 6465  port(json_encode
-00017120: 723d 4a73 6f6e 4461 7465 456e 636f 6465  r=JsonDateEncode
-00017130: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
-00017140: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-00017150: 6374 6564 2c20 6a73 6f6e 5f72 6573 756c  cted, json_resul
-00017160: 7429 0a0a 2020 2020 6465 6620 7465 7374  t)..    def test
-00017170: 5f6a 736f 6e5f 696d 706f 7274 5f77 6974  _json_import_wit
-00017180: 685f 6d75 6c74 6970 6c65 5f63 7573 746f  h_multiple_custo
-00017190: 6d5f 656e 636f 6465 7273 2873 656c 6629  m_encoders(self)
-000171a0: 3a0a 2020 2020 2020 2020 6672 6f6d 2064  :.        from d
-000171b0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-000171c0: 6174 650a 0a20 2020 2020 2020 2063 6c61  ate..        cla
-000171d0: 7373 2041 4141 3a0a 2020 2020 2020 2020  ss AAA:.        
-000171e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000171f0: 2873 656c 662c 206e 616d 6529 3a0a 2020  (self, name):.  
-00017200: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017210: 6c66 2e6e 616d 6520 3d20 6e61 6d65 0a0a  lf.name = name..
-00017220: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-00017230: 0a20 2020 2020 2020 2020 2020 207b 2761  .            {'a
-00017240: 273a 2031 3030 2c20 2762 273a 2064 6174  ': 100, 'b': dat
-00017250: 6528 3230 3030 2c20 312c 2031 292c 2027  e(2000, 1, 1), '
-00017260: 6327 3a20 3230 302c 2027 6427 3a20 4141  c': 200, 'd': AA
-00017270: 4128 2241 6c69 6365 2229 7d2c 0a20 2020  A("Alice")},.   
-00017280: 2020 2020 2020 2020 207b 2761 273a 2031           {'a': 1
-00017290: 3031 2c20 2762 273a 2064 6174 6528 3230  01, 'b': date(20
-000172a0: 3031 2c20 312c 2031 292c 2027 6327 3a20  01, 1, 1), 'c': 
-000172b0: 3230 312c 2027 6427 3a20 4141 4128 2242  201, 'd': AAA("B
-000172c0: 6f62 2229 7d2c 0a20 2020 2020 2020 205d  ob")},.        ]
-000172d0: 0a20 2020 2020 2020 2074 626c 203d 206c  .        tbl = l
-000172e0: 742e 5461 626c 6528 292e 696e 7365 7274  t.Table().insert
-000172f0: 5f6d 616e 7928 6461 7461 290a 2020 2020  _many(data).    
-00017300: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00017310: 7365 7274 5261 6973 6573 2854 7970 6545  sertRaises(TypeE
-00017320: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-00017330: 2020 2078 203d 2074 626c 2e6a 736f 6e5f     x = tbl.json_
-00017340: 6578 706f 7274 2829 0a0a 2020 2020 2020  export()..      
-00017350: 2020 636c 6173 7320 4a73 6f6e 4461 7465    class JsonDate
-00017360: 456e 636f 6465 7228 6a73 6f6e 2e4a 534f  Encoder(json.JSO
-00017370: 4e45 6e63 6f64 6572 293a 0a20 2020 2020  NEncoder):.     
-00017380: 2020 2020 2020 2064 6566 2064 6566 6175         def defau
-00017390: 6c74 2873 656c 662c 206f 293a 0a20 2020  lt(self, o):.   
-000173a0: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
-000173b0: 6f72 7420 6461 7465 7469 6d65 0a20 2020  ort datetime.   
-000173c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000173d0: 6973 696e 7374 616e 6365 286f 2c20 6461  isinstance(o, da
-000173e0: 7465 7469 6d65 2e64 6174 6529 3a0a 2020  tetime.date):.  
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 7265 7475 726e 2073 7472 286f 290a    return str(o).
-00017410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017420: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
-00017430: 6566 6175 6c74 286f 290a 0a20 2020 2020  efault(o)..     
-00017440: 2020 2063 6c61 7373 204a 736f 6e41 4141     class JsonAAA
-00017450: 456e 636f 6465 7228 6a73 6f6e 2e4a 534f  Encoder(json.JSO
-00017460: 4e45 6e63 6f64 6572 293a 0a20 2020 2020  NEncoder):.     
-00017470: 2020 2020 2020 2064 6566 2064 6566 6175         def defau
-00017480: 6c74 2873 656c 662c 206f 293a 0a20 2020  lt(self, o):.   
-00017490: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000174a0: 6973 696e 7374 616e 6365 286f 2c20 4141  isinstance(o, AA
-000174b0: 4129 3a0a 2020 2020 2020 2020 2020 2020  A):.            
-000174c0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000174d0: 2241 4141 286e 616d 653d 7b6f 2e6e 616d  "AAA(name={o.nam
-000174e0: 6521 727d 2922 0a0a 2020 2020 2020 2020  e!r})"..        
-000174f0: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
-00017500: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-00017510: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-00017520: 2020 2020 2020 2020 2020 7b22 6122 3a20            {"a": 
-00017530: 3130 302c 2022 6222 3a20 2232 3030 302d  100, "b": "2000-
-00017540: 3031 2d30 3122 2c20 2263 223a 2032 3030  01-01", "c": 200
-00017550: 2c20 2264 223a 2022 4141 4128 6e61 6d65  , "d": "AAA(name
-00017560: 3d27 416c 6963 6527 2922 7d2c 0a20 2020  ='Alice')"},.   
-00017570: 2020 2020 2020 2020 207b 2261 223a 2031           {"a": 1
-00017580: 3031 2c20 2262 223a 2022 3230 3031 2d30  01, "b": "2001-0
-00017590: 312d 3031 222c 2022 6322 3a20 3230 312c  1-01", "c": 201,
-000175a0: 2022 6422 3a20 2241 4141 286e 616d 653d   "d": "AAA(name=
-000175b0: 2742 6f62 2729 227d 0a20 2020 2020 2020  'Bob')"}.       
-000175c0: 2020 2020 205d 0a20 2020 2020 2020 2022       ].        "
-000175d0: 2222 290a 0a20 2020 2020 2020 206a 736f  "")..        jso
-000175e0: 6e5f 7265 7375 6c74 203d 2074 626c 2e6a  n_result = tbl.j
-000175f0: 736f 6e5f 6578 706f 7274 286a 736f 6e5f  son_export(json_
-00017600: 656e 636f 6465 723d 284a 736f 6e44 6174  encoder=(JsonDat
-00017610: 6545 6e63 6f64 6572 2c20 4a73 6f6e 4141  eEncoder, JsonAA
-00017620: 4145 6e63 6f64 6572 2929 0a20 2020 2020  AEncoder)).     
-00017630: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00017640: 7561 6c28 6578 7065 6374 6564 2c20 6a73  ual(expected, js
-00017650: 6f6e 5f72 6573 756c 7429 0a0a 2020 2020  on_result)..    
-00017660: 6465 6620 7465 7374 5f66 6978 6564 5f77  def test_fixed_w
-00017670: 6964 7468 5f69 6d70 6f72 7428 7365 6c66  idth_import(self
-00017680: 293a 0a20 2020 2020 2020 2064 6174 6120  ):.        data 
-00017690: 3d20 6669 7865 645f 7769 6474 685f 6461  = fixed_width_da
-000176a0: 7461 0a20 2020 2020 2020 2064 6174 615f  ta.        data_
-000176b0: 6669 6c65 203d 2069 6f2e 5374 7269 6e67  file = io.String
-000176c0: 494f 2864 6174 6129 0a20 2020 2020 2020  IO(data).       
-000176d0: 2066 775f 7370 6563 203d 205b 2827 6127   fw_spec = [('a'
-000176e0: 2c20 302c 204e 6f6e 652c 2069 6e74 292c  , 0, None, int),
-000176f0: 2028 2762 272c 2032 2c20 4e6f 6e65 2c20   ('b', 2, None, 
-00017700: 696e 7429 2c20 2827 6327 2c20 342c 204e  int), ('c', 4, N
-00017710: 6f6e 652c 2069 6e74 292c 205d 0a20 2020  one, int), ].   
-00017720: 2020 2020 2074 7420 3d20 6c74 2e54 6162       tt = lt.Tab
-00017730: 6c65 2829 2e69 6e73 6572 745f 6d61 6e79  le().insert_many
-00017740: 286c 742e 4461 7461 4f62 6a65 6374 282a  (lt.DataObject(*
-00017750: 2a72 6563 2920 666f 7220 7265 6320 696e  *rec) for rec in
-00017760: 206c 742e 4669 7865 6457 6964 7468 5265   lt.FixedWidthRe
-00017770: 6164 6572 2866 775f 7370 6563 2c20 6461  ader(fw_spec, da
-00017780: 7461 5f66 696c 6529 290a 0a20 2020 2020  ta_file))..     
-00017790: 2020 2074 6573 745f 7369 7a65 203d 2033     test_size = 3
-000177a0: 0a20 2020 2020 2020 2074 3120 3d20 6d61  .        t1 = ma
-000177b0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-000177c0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000177d0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-000177e0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000177f0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00017800: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00017810: 7373 6572 7454 7275 6528 616c 6c28 6d61  ssertTrue(all(ma
-00017820: 6b65 5f64 6174 616f 626a 6563 745f 6672  ke_dataobject_fr
-00017830: 6f6d 5f6f 6228 7265 6331 2920 3d3d 2072  om_ob(rec1) == r
-00017840: 6563 3220 666f 7220 7265 6331 2c20 7265  ec2 for rec1, re
-00017850: 6332 2069 6e20 7a69 7028 7431 2c20 7474  c2 in zip(t1, tt
-00017860: 2929 290a 2020 2020 2020 2020 7769 7468  ))).        with
-00017870: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00017880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00017890: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-000178a0: 6e28 5b64 2066 6f72 2064 2069 6e20 6461  n([d for d in da
-000178b0: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
-000178c0: 6966 2064 2e73 7472 6970 2829 5d29 2c20  if d.strip()]), 
-000178d0: 6c65 6e28 7474 2929 0a0a 2020 2020 6465  len(tt))..    de
-000178e0: 6620 7465 7374 5f66 6978 6564 5f77 6964  f test_fixed_wid
-000178f0: 7468 5f73 7472 696e 675f 696d 706f 7274  th_string_import
-00017900: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017910: 6461 7461 203d 2066 6978 6564 5f77 6964  data = fixed_wid
-00017920: 7468 5f64 6174 610a 2020 2020 2020 2020  th_data.        
-00017930: 6677 5f73 7065 6320 3d20 5b28 2761 272c  fw_spec = [('a',
-00017940: 2030 2c20 4e6f 6e65 2c20 696e 7429 2c20   0, None, int), 
-00017950: 2827 6227 2c20 322c 204e 6f6e 652c 2069  ('b', 2, None, i
-00017960: 6e74 292c 2028 2763 272c 2034 2c20 4e6f  nt), ('c', 4, No
-00017970: 6e65 2c20 696e 7429 2c20 5d0a 2020 2020  ne, int), ].    
-00017980: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
-00017990: 6528 292e 696e 7365 7274 5f6d 616e 7928  e().insert_many(
-000179a0: 6c74 2e44 6174 614f 626a 6563 7428 2a2a  lt.DataObject(**
-000179b0: 7265 6329 2066 6f72 2072 6563 2069 6e20  rec) for rec in 
-000179c0: 6c74 2e46 6978 6564 5769 6474 6852 6561  lt.FixedWidthRea
-000179d0: 6465 7228 6677 5f73 7065 632c 2064 6174  der(fw_spec, dat
-000179e0: 6129 290a 0a20 2020 2020 2020 2074 6573  a))..        tes
-000179f0: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
-00017a00: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
-00017a10: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00017a20: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00017a30: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
-00017a40: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00017a50: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00017a60: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00017a70: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
-00017a80: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
-00017a90: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
-00017aa0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
-00017ab0: 7a69 7028 7431 2c20 7474 2929 290a 2020  zip(t1, tt))).  
-00017ac0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00017ad0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00017ae0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00017af0: 7274 4571 7561 6c28 6c65 6e28 5b64 2066  rtEqual(len([d f
-00017b00: 6f72 2064 2069 6e20 6461 7461 2e73 706c  or d in data.spl
-00017b10: 6974 6c69 6e65 7328 2920 6966 2064 2e73  itlines() if d.s
-00017b20: 7472 6970 2829 5d29 2c20 6c65 6e28 7474  trip()]), len(tt
-00017b30: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-00017b40: 5f66 6978 6564 5f77 6964 7468 5f73 7472  _fixed_width_str
-00017b50: 696e 675f 6c69 7374 5f69 6d70 6f72 7428  ing_list_import(
-00017b60: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
-00017b70: 6174 6120 3d20 6669 7865 645f 7769 6474  ata = fixed_widt
-00017b80: 685f 6461 7461 0a20 2020 2020 2020 2066  h_data.        f
-00017b90: 775f 7370 6563 203d 205b 2827 6127 2c20  w_spec = [('a', 
-00017ba0: 302c 204e 6f6e 652c 2069 6e74 292c 2028  0, None, int), (
-00017bb0: 2762 272c 2032 2c20 4e6f 6e65 2c20 696e  'b', 2, None, in
-00017bc0: 7429 2c20 2827 6327 2c20 342c 204e 6f6e  t), ('c', 4, Non
-00017bd0: 652c 2069 6e74 292c 5d0a 2020 2020 2020  e, int),].      
-00017be0: 2020 7474 203d 206c 742e 5461 626c 6528    tt = lt.Table(
-00017bf0: 292e 696e 7365 7274 5f6d 616e 7928 6c74  ).insert_many(lt
-00017c00: 2e44 6174 614f 626a 6563 7428 2a2a 7265  .DataObject(**re
-00017c10: 6329 2066 6f72 2072 6563 2069 6e20 6c74  c) for rec in lt
-00017c20: 2e46 6978 6564 5769 6474 6852 6561 6465  .FixedWidthReade
-00017c30: 7228 6677 5f73 7065 632c 2064 6174 612e  r(fw_spec, data.
-00017c40: 7370 6c69 746c 696e 6573 2829 2929 0a0a  splitlines()))..
-00017c50: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-00017c60: 6520 3d20 330a 2020 2020 2020 2020 7431  e = 3.        t1
-00017c70: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00017c80: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-00017c90: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00017ca0: 697a 6529 0a0a 2020 2020 2020 2020 7769  ize)..        wi
-00017cb0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00017cc0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00017cd0: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
-00017ce0: 6c6c 286d 616b 655f 6461 7461 6f62 6a65  ll(make_dataobje
-00017cf0: 6374 5f66 726f 6d5f 6f62 2872 6563 3129  ct_from_ob(rec1)
-00017d00: 203d 3d20 7265 6332 2066 6f72 2072 6563   == rec2 for rec
-00017d10: 312c 2072 6563 3220 696e 207a 6970 2874  1, rec2 in zip(t
-00017d20: 312c 2074 7429 2929 0a20 2020 2020 2020  1, tt))).       
-00017d30: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00017d40: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00017d50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00017d60: 616c 286c 656e 285b 6420 666f 7220 6420  al(len([d for d 
-00017d70: 696e 2064 6174 612e 7370 6c69 746c 696e  in data.splitlin
-00017d80: 6573 2829 2069 6620 642e 7374 7269 7028  es() if d.strip(
-00017d90: 295d 292c 206c 656e 2874 7429 290a 0a20  )]), len(tt)).. 
-00017da0: 2020 2064 6566 2074 6573 745f 6578 6365     def test_exce
-00017db0: 6c5f 696d 706f 7274 2873 656c 6629 3a0a  l_import(self):.
-00017dc0: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
-00017dd0: 6520 3d20 2274 6573 742f 6162 632e 786c  e = "test/abc.xl
-00017de0: 7378 220a 2020 2020 2020 2020 6578 6365  sx".        exce
-00017df0: 6c5f 7461 626c 6520 3d20 6c74 2e54 6162  l_table = lt.Tab
-00017e00: 6c65 2829 2e65 7863 656c 5f69 6d70 6f72  le().excel_impor
-00017e10: 7428 6669 6c65 5f6e 616d 652c 2074 7261  t(file_name, tra
-00017e20: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
-00017e30: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
-00017e40: 3a20 696e 747d 290a 0a20 2020 2020 2020  : int})..       
-00017e50: 2074 6573 745f 7369 7a65 203d 2033 0a20   test_size = 3. 
-00017e60: 2020 2020 2020 2074 3120 3d20 6d61 6b65         t1 = make
-00017e70: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
-00017e80: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00017e90: 742c 2074 6573 745f 7369 7a65 290a 0a20  t, test_size).. 
-00017ea0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00017eb0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00017ec0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00017ed0: 6572 7454 7275 6528 616c 6c28 6d61 6b65  ertTrue(all(make
-00017ee0: 5f64 6174 616f 626a 6563 745f 6672 6f6d  _dataobject_from
-00017ef0: 5f6f 6228 7265 6331 2920 3d3d 2072 6563  _ob(rec1) == rec
-00017f00: 3220 666f 7220 7265 6331 2c20 7265 6332  2 for rec1, rec2
-00017f10: 2069 6e20 7a69 7028 7431 2c20 6578 6365   in zip(t1, exce
-00017f20: 6c5f 7461 626c 6529 2929 0a20 2020 2020  l_table))).     
-00017f30: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00017f40: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00017f50: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00017f60: 7175 616c 2873 756d 2831 2066 6f72 206c  qual(sum(1 for l
-00017f70: 696e 6520 696e 2063 7376 5f64 6174 612e  ine in csv_data.
-00017f80: 7370 6c69 746c 696e 6573 2829 2069 6620  splitlines() if 
-00017f90: 6c69 6e65 2e73 7472 6970 2829 292d 312c  line.strip())-1,
-00017fa0: 206c 656e 2865 7863 656c 5f74 6162 6c65   len(excel_table
-00017fb0: 2929 0a0a 2020 2020 2020 2020 726f 775f  ))..        row_
-00017fc0: 7072 6f74 6f74 7970 6520 3d20 7365 6c66  prototype = self
-00017fd0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00017fe0: 7428 302c 2030 2c20 3029 0a20 2020 2020  t(0, 0, 0).     
-00017ff0: 2020 2063 7376 7461 626c 6532 203d 206c     csvtable2 = l
-00018000: 742e 5461 626c 6528 292e 6578 6365 6c5f  t.Table().excel_
-00018010: 696d 706f 7274 280a 2020 2020 2020 2020  import(.        
-00018020: 2020 2020 6669 6c65 5f6e 616d 652c 2074      file_name, t
-00018030: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
-00018040: 696e 742c 2027 6227 3a20 696e 742c 2027  int, 'b': int, '
-00018050: 6327 3a20 696e 747d 2c20 726f 775f 636c  c': int}, row_cl
-00018060: 6173 733d 7479 7065 2872 6f77 5f70 726f  ass=type(row_pro
-00018070: 746f 7479 7065 290a 2020 2020 2020 2020  totype).        
-00018080: 295b 3a33 5d0a 0a20 2020 2020 2020 2070  )[:3]..        p
-00018090: 7269 6e74 2874 7970 6528 7431 5b30 5d29  rint(type(t1[0])
-000180a0: 2e5f 5f6e 616d 655f 5f2c 2074 315b 305d  .__name__, t1[0]
-000180b0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-000180c0: 7479 7065 2863 7376 7461 626c 6532 5b30  type(csvtable2[0
-000180d0: 5d29 2e5f 5f6e 616d 655f 5f2c 2063 7376  ]).__name__, csv
-000180e0: 7461 626c 6532 5b30 5d29 0a20 2020 2020  table2[0]).     
-000180f0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00018100: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00018110: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00018120: 7175 616c 2874 7970 6528 7431 5b30 5d29  qual(type(t1[0])
-00018130: 2c20 7479 7065 2863 7376 7461 626c 6532  , type(csvtable2
-00018140: 5b30 5d29 290a 0a20 2020 2064 6566 2074  [0]))..    def t
-00018150: 6573 745f 6578 6365 6c5f 6578 706f 7274  est_excel_export
-00018160: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00018170: 6669 6c65 5f6e 616d 6520 3d20 2274 6573  file_name = "tes
-00018180: 742f 6162 632e 786c 7378 220a 2020 2020  t/abc.xlsx".    
-00018190: 2020 2020 6578 6365 6c5f 7461 626c 6520      excel_table 
-000181a0: 3d20 6c74 2e54 6162 6c65 2829 2e65 7863  = lt.Table().exc
-000181b0: 656c 5f69 6d70 6f72 7428 6669 6c65 5f6e  el_import(file_n
-000181c0: 616d 652c 2074 7261 6e73 666f 726d 733d  ame, transforms=
-000181d0: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
-000181e0: 696e 742c 2027 6327 3a20 696e 747d 2c20  int, 'c': int}, 
-000181f0: 6c69 6d69 743d 3129 0a20 2020 2020 2020  limit=1).       
-00018200: 206f 7574 6669 6c65 203d 2069 6f2e 4279   outfile = io.By
-00018210: 7465 7349 4f28 290a 2020 2020 2020 2020  tesIO().        
-00018220: 6578 6365 6c5f 7461 626c 652e 6578 6365  excel_table.exce
-00018230: 6c5f 6578 706f 7274 286f 7574 6669 6c65  l_export(outfile
-00018240: 290a 2020 2020 2020 2020 6578 706f 7274  ).        export
-00018250: 6564 5f74 6162 6c65 203d 206c 742e 5461  ed_table = lt.Ta
-00018260: 626c 6528 292e 6578 6365 6c5f 696d 706f  ble().excel_impo
-00018270: 7274 286f 7574 6669 6c65 2c20 7472 616e  rt(outfile, tran
-00018280: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
-00018290: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
-000182a0: 2069 6e74 7d29 0a0a 2020 2020 2020 2020   int})..        
-000182b0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-000182c0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-000182d0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-000182e0: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
-000182f0: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
-00018300: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
-00018310: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
-00018320: 2865 7870 6f72 7465 645f 7461 626c 652c  (exported_table,
-00018330: 2065 7863 656c 5f74 6162 6c65 2929 290a   excel_table))).
-00018340: 0a20 2020 2064 6566 2074 6573 745f 6d6f  .    def test_mo
-00018350: 6475 6c65 5f6c 6576 656c 5f63 7376 5f69  dule_level_csv_i
-00018360: 6d70 6f72 7465 7228 7365 6c66 293a 0a20  mporter(self):. 
-00018370: 2020 2020 2020 2064 6174 6120 3d20 6373         data = cs
-00018380: 765f 6461 7461 0a20 2020 2020 2020 2063  v_data.        c
-00018390: 7376 7461 626c 6520 3d20 6c74 2e63 7376  svtable = lt.csv
-000183a0: 5f69 6d70 6f72 7428 6373 765f 736f 7572  _import(csv_sour
-000183b0: 6365 3d64 6174 612c 2074 7261 6e73 666f  ce=data, transfo
-000183c0: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
-000183d0: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
-000183e0: 747d 290a 0a20 2020 2020 2020 2074 6573  t})..        tes
-000183f0: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
-00018400: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
-00018410: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00018420: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00018430: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
-00018440: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00018450: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00018460: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00018470: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
-00018480: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
-00018490: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
-000184a0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
-000184b0: 7a69 7028 7431 2c20 6373 7674 6162 6c65  zip(t1, csvtable
-000184c0: 2929 290a 2020 2020 2020 2020 7769 7468  ))).        with
-000184d0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-000184e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000184f0: 662e 6173 7365 7274 4571 7561 6c28 7375  f.assertEqual(su
-00018500: 6d28 3120 666f 7220 6c69 6e65 2069 6e20  m(1 for line in 
-00018510: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
-00018520: 2920 6966 206c 696e 652e 7374 7269 7028  ) if line.strip(
-00018530: 2929 2d31 2c20 6c65 6e28 6373 7674 6162  ))-1, len(csvtab
-00018540: 6c65 2929 0a0a 2020 2020 6465 6620 7465  le))..    def te
-00018550: 7374 5f6d 6f64 756c 655f 6c65 7665 6c5f  st_module_level_
-00018560: 6a73 6f6e 5f69 6d70 6f72 7465 7228 7365  json_importer(se
-00018570: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
-00018580: 6120 3d20 6a73 6f6e 5f64 6174 610a 2020  a = json_data.  
-00018590: 2020 2020 2020 6a73 6f6e 7461 626c 6520        jsontable 
-000185a0: 3d20 6c74 2e6a 736f 6e5f 696d 706f 7274  = lt.json_import
-000185b0: 2864 6174 612c 2073 7472 6561 6d69 6e67  (data, streaming
-000185c0: 3d54 7275 652c 2074 7261 6e73 666f 726d  =True, transform
-000185d0: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
-000185e0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
-000185f0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
-00018600: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
-00018610: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
-00018620: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
-00018630: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
-00018640: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-00018650: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00018660: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00018670: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00018680: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
-00018690: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
-000186a0: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
-000186b0: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
-000186c0: 7028 7431 2c20 6a73 6f6e 7461 626c 6529  p(t1, jsontable)
-000186d0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-000186e0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-000186f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018700: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00018710: 285b 6420 666f 7220 6420 696e 2064 6174  ([d for d in dat
-00018720: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
-00018730: 6620 642e 7374 7269 7028 295d 292c 206c  f d.strip()]), l
-00018740: 656e 286a 736f 6e74 6162 6c65 2929 0a0a  en(jsontable))..
-00018750: 2020 2020 6465 6620 7465 7374 5f6d 6f64      def test_mod
-00018760: 756c 655f 6c65 7665 6c5f 6578 6365 6c5f  ule_level_excel_
-00018770: 696d 706f 7274 2873 656c 6629 3a0a 2020  import(self):.  
-00018780: 2020 2020 2020 6669 6c65 5f6e 616d 6520        file_name 
-00018790: 3d20 2274 6573 742f 6162 632e 786c 7378  = "test/abc.xlsx
-000187a0: 220a 2020 2020 2020 2020 6578 6365 6c5f  ".        excel_
-000187b0: 7461 626c 6520 3d20 6c74 2e65 7863 656c  table = lt.excel
-000187c0: 5f69 6d70 6f72 7428 6669 6c65 5f6e 616d  _import(file_nam
-000187d0: 652c 2074 7261 6e73 666f 726d 733d 7b27  e, transforms={'
-000187e0: 6127 3a20 696e 742c 2027 6227 3a20 696e  a': int, 'b': in
-000187f0: 742c 2027 6327 3a20 696e 747d 290a 0a20  t, 'c': int}).. 
-00018800: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
-00018810: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
-00018820: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-00018830: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00018840: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-00018850: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
-00018860: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00018870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00018880: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-00018890: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
-000188a0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
-000188b0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
-000188c0: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
-000188d0: 2c20 6578 6365 6c5f 7461 626c 6529 2929  , excel_table)))
-000188e0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000188f0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00018900: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018910: 7373 6572 7445 7175 616c 2873 756d 2831  ssertEqual(sum(1
-00018920: 2066 6f72 206c 696e 6520 696e 2063 7376   for line in csv
-00018930: 5f64 6174 612e 7370 6c69 746c 696e 6573  _data.splitlines
-00018940: 2829 2069 6620 6c69 6e65 2e73 7472 6970  () if line.strip
-00018950: 2829 292d 312c 206c 656e 2865 7863 656c  ())-1, len(excel
-00018960: 5f74 6162 6c65 2929 0a0a 0a40 6d61 6b65  _table))...@make
-00018970: 5f74 6573 745f 636c 6173 7365 730a 636c  _test_classes.cl
-00018980: 6173 7320 5461 626c 6550 6976 6f74 5465  ass TablePivotTe
-00018990: 7374 733a 0a20 2020 2022 2222 0a20 2020  sts:.    """.   
-000189a0: 2054 6573 7420 636c 6173 7320 666f 7220   Test class for 
-000189b0: 5461 626c 6520 7069 766f 7420 6f70 6572  Table pivot oper
-000189c0: 6174 696f 6e73 2e0a 2020 2020 2222 220a  ations..    """.
-000189d0: 2020 2020 6465 6620 7465 7374 5f70 6976      def test_piv
-000189e0: 6f74 2873 656c 6629 3a0a 2020 2020 2020  ot(self):.      
-000189f0: 2020 7465 7374 5f73 697a 6520 3d20 350a    test_size = 5.
-00018a00: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
-00018a10: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
-00018a20: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-00018a30: 6374 2c20 7465 7374 5f73 697a 6529 0a20  ct, test_size). 
-00018a40: 2020 2020 2020 2074 312e 6372 6561 7465         t1.create
-00018a50: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
-00018a60: 2020 2020 7431 2e63 7265 6174 655f 696e      t1.create_in
-00018a70: 6465 7828 2762 2729 0a20 2020 2020 2020  dex('b').       
-00018a80: 2074 3170 6976 6f74 203d 2074 312e 7069   t1pivot = t1.pi
-00018a90: 766f 7428 2761 2729 0a20 2020 2020 2020  vot('a').       
-00018aa0: 2074 3170 6976 6f74 2e64 756d 7028 290a   t1pivot.dump().
-00018ab0: 2020 2020 2020 2020 7431 7069 766f 742e          t1pivot.
-00018ac0: 6475 6d70 5f63 6f75 6e74 7328 290a 2020  dump_counts().  
-00018ad0: 2020 2020 2020 7431 7069 766f 742e 7375        t1pivot.su
-00018ae0: 6d6d 6172 795f 636f 756e 7473 2829 0a0a  mmary_counts()..
-00018af0: 2020 2020 2020 2020 7432 7069 766f 7420          t2pivot 
-00018b00: 3d20 7431 2e70 6976 6f74 2827 6120 6227  = t1.pivot('a b'
-00018b10: 290a 2020 2020 2020 2020 7432 7069 766f  ).        t2pivo
-00018b20: 742e 6475 6d70 2829 0a20 2020 2020 2020  t.dump().       
-00018b30: 2074 3270 6976 6f74 2e64 756d 705f 636f   t2pivot.dump_co
-00018b40: 756e 7473 2829 0a20 2020 2020 2020 2074  unts().        t
-00018b50: 3270 6976 6f74 2e73 756d 6d61 7279 5f63  2pivot.summary_c
-00018b60: 6f75 6e74 7328 290a 0a20 2020 2020 2020  ounts()..       
-00018b70: 2023 2054 4f44 4f20 2d20 6164 6420 6173   # TODO - add as
-00018b80: 7365 7274 730a 0a0a 636c 6173 7320 5461  serts...class Ta
-00018b90: 626c 6553 6561 7263 6854 6573 7473 2875  bleSearchTests(u
-00018ba0: 6e69 7474 6573 742e 5465 7374 4361 7365  nittest.TestCase
-00018bb0: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-00018bc0: 6573 7420 636c 6173 7320 666f 7220 6675  est class for fu
-00018bd0: 6c6c 2d74 6578 7420 7365 6172 6368 206d  ll-text search m
-00018be0: 6574 686f 6473 2e0a 2020 2020 2222 220a  ethods..    """.
-00018bf0: 2020 2020 7265 6369 7065 5f64 6174 6120      recipe_data 
-00018c00: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
-00018c10: 7428 2222 225c 0a20 2020 2020 2020 2069  t("""\.        i
-00018c20: 642c 7469 746c 652c 696e 6772 6564 6965  d,title,ingredie
-00018c30: 6e74 730a 2020 2020 2020 2020 312c 5475  nts.        1,Tu
-00018c40: 6e61 2063 6173 7365 726f 6c65 2c22 7475  na casserole,"tu
-00018c50: 6e61 2c20 6e6f 6f64 6c65 732c 2043 7265  na, noodles, Cre
-00018c60: 616d 206f 6620 4d75 7368 726f 6f6d 2053  am of Mushroom S
-00018c70: 6f75 7022 0a20 2020 2020 2020 2032 2c48  oup".        2,H
-00018c80: 6177 6169 6961 6e20 7069 7a7a 612c 7069  awaiian pizza,pi
-00018c90: 7a7a 6120 646f 7567 6820 7069 6e65 6170  zza dough pineap
-00018ca0: 706c 6520 6861 6d20 746f 6d61 746f 2073  ple ham tomato s
-00018cb0: 6175 6365 0a20 2020 2020 2020 2033 2c4d  auce.        3,M
-00018cc0: 6172 6768 6572 6974 6120 7069 7a7a 612c  argherita pizza,
-00018cd0: 7069 7a7a 6120 646f 7567 6820 6368 6565  pizza dough chee
-00018ce0: 7365 2070 6573 746f 2061 7274 6963 686f  se pesto articho
-00018cf0: 6b65 2068 6561 7274 730a 2020 2020 2020  ke hearts.      
-00018d00: 2020 342c 5065 7070 6572 6f6e 6920 7069    4,Pepperoni pi
-00018d10: 7a7a 612c 7069 7a7a 6120 646f 7567 6820  zza,pizza dough 
-00018d20: 6368 6565 7365 2074 6f6d 6174 6f20 7361  cheese tomato sa
-00018d30: 7563 6520 7065 7070 6572 6f6e 690a 2020  uce pepperoni.  
-00018d40: 2020 2020 2020 352c 4772 696c 6c65 6420        5,Grilled 
-00018d50: 6368 6565 7365 2073 616e 6477 6963 682c  cheese sandwich,
-00018d60: 6272 6561 6420 6368 6565 7365 2062 7574  bread cheese but
-00018d70: 7465 720a 2020 2020 2020 2020 362c 5475  ter.        6,Tu
-00018d80: 6e61 206d 656c 742c 7475 6e61 206d 6179  na melt,tuna may
-00018d90: 6f6e 6e61 6973 6520 746f 6d61 746f 2062  onnaise tomato b
-00018da0: 7265 6164 2063 6865 6573 650a 2020 2020  read cheese.    
-00018db0: 2020 2020 372c 4368 696c 6920 646f 672c      7,Chili dog,
-00018dc0: 686f 7420 646f 6720 6368 696c 6920 6f6e  hot dog chili on
-00018dd0: 696f 6e20 6275 6e0a 2020 2020 2020 2020  ion bun.        
-00018de0: 382c 4672 656e 6368 2074 6f61 7374 2c65  8,French toast,e
-00018df0: 6767 206d 696c 6b20 7661 6e69 6c6c 6120  gg milk vanilla 
-00018e00: 6272 6561 6420 6d61 706c 6520 7379 7275  bread maple syru
-00018e10: 700a 2020 2020 2020 2020 392c 424c 542c  p.        9,BLT,
-00018e20: 6272 6561 6420 6261 636f 6e20 6c65 7474  bread bacon lett
-00018e30: 7563 6520 746f 6d61 746f 206d 6179 6f6e  uce tomato mayon
-00018e40: 6e61 6973 650a 2020 2020 2020 2020 3130  naise.        10
-00018e50: 2c52 6575 6265 6e20 7361 6e64 7769 6368  ,Reuben sandwich
-00018e60: 2c72 7965 2062 7265 6164 2073 6175 6572  ,rye bread sauer
-00018e70: 6b72 6175 7420 636f 726e 6564 2062 6565  kraut corned bee
-00018e80: 6620 7377 6973 7320 6368 6565 7365 2072  f swiss cheese r
-00018e90: 7573 7369 616e 2064 7265 7373 696e 6720  ussian dressing 
-00018ea0: 7468 6f75 7361 6e64 2069 736c 616e 640a  thousand island.
-00018eb0: 2020 2020 2020 2020 3131 2c48 616d 6275          11,Hambu
-00018ec0: 7267 6572 2c67 726f 756e 6420 6265 6566  rger,ground beef
-00018ed0: 2062 756e 206c 6574 7475 6365 206b 6574   bun lettuce ket
-00018ee0: 6368 7570 206d 7573 7461 7264 2070 6963  chup mustard pic
-00018ef0: 6b6c 650a 2020 2020 2020 2020 3132 2c43  kle.        12,C
-00018f00: 6865 6573 6562 7572 6765 722c 6772 6f75  heeseburger,grou
-00018f10: 6e64 2062 6565 6620 6275 6e20 6c65 7474  nd beef bun lett
-00018f20: 7563 6520 6b65 7463 6875 7020 6d75 7374  uce ketchup must
-00018f30: 6172 6420 7069 636b 6c65 2063 6865 6573  ard pickle chees
-00018f40: 650a 2020 2020 2020 2020 3133 2c42 6163  e.        13,Bac
-00018f50: 6f6e 2063 6865 6573 6562 7572 6765 722c  on cheeseburger,
-00018f60: 6772 6f75 6e64 2062 6565 6620 6275 6e20  ground beef bun 
-00018f70: 6c65 7474 7563 6520 6b65 7463 6875 7020  lettuce ketchup 
-00018f80: 6d75 7374 6172 6420 7069 636b 6c65 2063  mustard pickle c
-00018f90: 6865 6573 6520 6261 636f 6e0a 2020 2020  heese bacon.    
-00018fa0: 2020 2020 2222 2229 0a0a 2020 2020 6465      """)..    de
-00018fb0: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
-00018fc0: 2020 2020 2020 2073 656c 662e 7265 6369         self.reci
-00018fd0: 7065 7320 3d20 6c74 2e54 6162 6c65 2829  pes = lt.Table()
-00018fe0: 2e63 7376 5f69 6d70 6f72 7428 7365 6c66  .csv_import(self
-00018ff0: 2e72 6563 6970 655f 6461 7461 2c20 7472  .recipe_data, tr
-00019000: 616e 7366 6f72 6d73 3d64 6963 7428 6964  ansforms=dict(id
-00019010: 3d69 6e74 2929 0a20 2020 2020 2020 2073  =int)).        s
-00019020: 656c 662e 7265 6369 7065 732e 6372 6561  elf.recipes.crea
-00019030: 7465 5f69 6e64 6578 2822 6964 222c 2075  te_index("id", u
-00019040: 6e69 7175 653d 5472 7565 290a 2020 2020  nique=True).    
-00019050: 2020 2020 7365 6c66 2e72 6563 6970 6573      self.recipes
-00019060: 2e63 7265 6174 655f 7365 6172 6368 5f69  .create_search_i
-00019070: 6e64 6578 2822 696e 6772 6564 6965 6e74  ndex("ingredient
-00019080: 7322 290a 0a20 2020 2040 616e 6e6f 756e  s")..    @announ
-00019090: 6365 5f74 6573 740a 2020 2020 6465 6620  ce_test.    def 
-000190a0: 7465 7374 5f61 6363 6573 735f 6e6f 6e5f  test_access_non_
-000190b0: 6578 6973 7465 6e74 5f73 6561 7263 685f  existent_search_
-000190c0: 6174 7472 6962 7574 6528 7365 6c66 293a  attribute(self):
-000190d0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000190e0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-000190f0: 5661 6c75 6545 7272 6f72 2c20 6d73 673d  ValueError, msg=
-00019100: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
-00019110: 2056 616c 7565 4572 726f 7220 7768 656e   ValueError when
-00019120: 2061 6363 6573 7369 6e67 206e 6f6e 2d65   accessing non-e
-00019130: 7869 7374 656e 7420 7365 6172 6368 2069  xistent search i
-00019140: 6e64 6578 2229 3a0a 2020 2020 2020 2020  ndex"):.        
-00019150: 2020 2020 7365 6c66 2e72 6563 6970 6573      self.recipes
-00019160: 2e73 6561 7263 682e 7469 746c 6528 2278  .search.title("x
-00019170: 797a 2229 0a0a 2020 2020 4061 6e6e 6f75  yz")..    @annou
-00019180: 6e63 655f 7465 7374 0a20 2020 2064 6566  nce_test.    def
-00019190: 2074 6573 745f 7365 6172 6368 5f64 6972   test_search_dir
-000191a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000191b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000191c0: 285b 2769 6e67 7265 6469 656e 7473 275d  (['ingredients']
-000191d0: 2c20 6469 7228 7365 6c66 2e72 6563 6970  , dir(self.recip
-000191e0: 6573 2e73 6561 7263 6829 2c20 2266 6169  es.search), "fai
-000191f0: 6c65 6420 746f 2067 656e 6572 6174 6520  led to generate 
-00019200: 636f 7272 6563 7420 6469 7228 2920 7265  correct dir() re
-00019210: 7370 6f6e 7365 2229 0a0a 2020 2020 4061  sponse")..    @a
-00019220: 6e6e 6f75 6e63 655f 7465 7374 0a20 2020  nnounce_test.   
-00019230: 2064 6566 2074 6573 745f 7465 7874 5f73   def test_text_s
-00019240: 6561 7263 6828 7365 6c66 293a 0a20 2020  earch(self):.   
-00019250: 2020 2020 2066 6f72 2071 7565 7279 2c20       for query, 
-00019260: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
-00019270: 2020 2020 2020 2020 2020 2822 222c 205b            ("", [
-00019280: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019290: 2822 7475 6e61 222c 205b 312c 2036 5d29  ("tuna", [1, 6])
-000192a0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000192b0: 7475 6e61 202b 6368 6565 7365 222c 205b  tuna +cheese", [
-000192c0: 362c 2033 2c20 342c 2035 2c20 3130 2c20  6, 3, 4, 5, 10, 
-000192d0: 3132 2c20 3133 2c20 315d 292c 0a20 2020  12, 13, 1]),.   
-000192e0: 2020 2020 2020 2020 2028 2270 696e 6561           ("pinea
-000192f0: 7070 6c65 202b 6261 636f 6e20 6c65 7474  pple +bacon lett
-00019300: 7563 6520 6265 6566 202d 7361 7565 726b  uce beef -sauerk
-00019310: 7261 7574 2074 6f6d 6174 6f22 2c20 5b39  raut tomato", [9
-00019320: 2c20 3133 2c20 322c 2031 312c 2031 322c  , 13, 2, 11, 12,
-00019330: 2034 2c20 362c 2031 305d 292c 0a20 2020   4, 6, 10]),.   
-00019340: 2020 2020 2020 2020 2028 2270 697a 7a61           ("pizza
-00019350: 2064 6f75 6768 202d 7069 6e65 6170 706c   dough -pineappl
-00019360: 6522 2c20 5b33 2c20 342c 2032 5d29 2c0a  e", [3, 4, 2]),.
-00019370: 2020 2020 2020 2020 2020 2020 2822 7069              ("pi
-00019380: 7a7a 6120 646f 7567 6820 2d2d 7069 6e65  zza dough --pine
-00019390: 6170 706c 6522 2c20 5b33 2c20 345d 292c  apple", [3, 4]),
-000193a0: 0a20 2020 2020 2020 2020 2020 2028 2262  .            ("b
-000193b0: 7265 6164 2062 6163 6f6e 222c 205b 392c  read bacon", [9,
-000193c0: 2035 2c20 362c 2038 2c20 3130 2c20 3133   5, 6, 8, 10, 13
-000193d0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000193e0: 2822 6272 6561 6420 2b2b 6261 636f 6e22  ("bread ++bacon"
-000193f0: 2c20 5b39 2c20 3133 5d29 2c0a 2020 2020  , [9, 13]),.    
-00019400: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-00019410: 2b2b 616e 6368 6f76 6965 7322 2c20 5b5d  ++anchovies", []
-00019420: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00019430: 2262 7265 6164 202b 2b62 6163 6f6e 202b  "bread ++bacon +
-00019440: 2b61 6e63 686f 7669 6573 222c 205b 5d29  +anchovies", [])
-00019450: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00019460: 6272 6561 6420 6261 636f 6e20 2d2d 616e  bread bacon --an
-00019470: 6368 6f76 6965 7322 2c20 5b39 2c20 352c  chovies", [9, 5,
-00019480: 2036 2c20 382c 2031 302c 2031 335d 292c   6, 8, 10, 13]),
-00019490: 0a20 2020 2020 2020 205d 3a0a 2020 2020  .        ]:.    
-000194a0: 2020 2020 2020 2020 6d61 7463 6865 7320          matches 
-000194b0: 3d20 7365 6c66 2e72 6563 6970 6573 2e73  = self.recipes.s
-000194c0: 6561 7263 682e 696e 6772 6564 6965 6e74  earch.ingredient
-000194d0: 7328 7175 6572 792c 2061 735f 7461 626c  s(query, as_tabl
-000194e0: 653d 4661 6c73 652c 206d 696e 5f73 636f  e=False, min_sco
-000194f0: 7265 3d2d 3130 3030 3029 0a20 2020 2020  re=-10000).     
-00019500: 2020 2020 2020 206d 6174 6368 5f69 6473         match_ids
-00019510: 203d 205b 7265 6369 7065 2e69 6420 666f   = [recipe.id fo
-00019520: 7220 7265 6369 7065 2c20 5f20 696e 206d  r recipe, _ in m
-00019530: 6174 6368 6573 5d0a 2020 2020 2020 2020  atches].        
-00019540: 2020 2020 7072 696e 7428 7265 7072 2871      print(repr(q
-00019550: 7565 7279 292c 2027 2d3e 272c 205b 2872  uery), '->', [(r
-00019560: 6563 6970 652e 6964 2c20 7363 6f72 6529  ecipe.id, score)
-00019570: 2066 6f72 2072 6563 6970 652c 2073 636f   for recipe, sco
-00019580: 7265 2069 6e20 6d61 7463 6865 735d 290a  re in matches]).
-00019590: 2020 2020 2020 2020 2020 2020 7769 7468              with
-000195a0: 2073 656c 662e 7375 6254 6573 7428 7175   self.subTest(qu
-000195b0: 6572 793d 7175 6572 7929 3a0a 2020 2020  ery=query):.    
-000195c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000195d0: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-000195e0: 6563 7465 642c 206d 6174 6368 5f69 6473  ected, match_ids
-000195f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019610: 2020 2066 2269 6e76 616c 6964 2072 6573     f"invalid res
-00019620: 756c 7473 2066 6f72 2071 7565 7279 207b  ults for query {
-00019630: 7175 6572 7921 727d 2c20 6578 7065 6374  query!r}, expect
-00019640: 6564 207b 6578 7065 6374 6564 7d2c 2067  ed {expected}, g
-00019650: 6f74 207b 6d61 7463 685f 6964 737d 2229  ot {match_ids}")
-00019660: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
-00019670: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
-00019680: 745f 696e 7661 6c69 6461 7465 5f69 6e64  t_invalidate_ind
-00019690: 6578 2873 656c 6629 3a0a 2020 2020 2020  ex(self):.      
-000196a0: 2020 7365 6c66 2e72 6563 6970 6573 2e70    self.recipes.p
-000196b0: 6f70 2830 290a 2020 2020 2020 2020 7769  op(0).        wi
-000196c0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-000196d0: 6973 6573 286c 742e 5365 6172 6368 496e  ises(lt.SearchIn
-000196e0: 6465 7849 6e63 6f6e 7369 7374 656e 7445  dexInconsistentE
-000196f0: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
-00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2020 206d 7367 3d22 6661 696c 6564       msg="failed
-00019720: 2074 6f20 7261 6973 6520 6578 6365 7074   to raise except
-00019730: 696f 6e20 7768 656e 2073 6561 7263 6869  ion when searchi
-00019740: 6e67 206d 6f64 6966 6965 6420 7461 626c  ng modified tabl
-00019750: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-00019760: 2073 656c 662e 7265 6369 7065 732e 7365   self.recipes.se
-00019770: 6172 6368 2e69 6e67 7265 6469 656e 7473  arch.ingredients
-00019780: 2822 6261 636f 6e22 290a 0a20 2020 2040  ("bacon")..    @
-00019790: 616e 6e6f 756e 6365 5f74 6573 740a 2020  announce_test.  
-000197a0: 2020 6465 6620 7465 7374 5f73 6561 7263    def test_searc
-000197b0: 685f 7769 7468 5f6b 6579 776f 7264 7328  h_with_keywords(
-000197c0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-000197d0: 6f72 2071 7565 7279 2c20 6578 7065 6374  or query, expect
-000197e0: 6564 2c20 6578 7065 6374 6564 5f77 6f72  ed, expected_wor
-000197f0: 6473 2069 6e20 5b0a 2020 2020 2020 2020  ds in [.        
-00019800: 2020 2020 2020 2020 2822 7475 6e61 222c          ("tuna",
-00019810: 205b 312c 2036 5d2c 205b 7b27 6e6f 6f64   [1, 6], [{'nood
-00019820: 6c65 7327 2c20 276e 6f6f 646c 6527 2c20  les', 'noodle', 
-00019830: 2774 756e 6127 2c20 2773 6f75 7027 2c20  'tuna', 'soup', 
-00019840: 2763 7265 616d 272c 2027 6d75 7368 726f  'cream', 'mushro
-00019850: 6f6d 277d 2c0a 2020 2020 2020 2020 2020  om'},.          
-00019860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019870: 2020 2020 2020 2020 7b27 746f 6d61 746f          {'tomato
-00019880: 272c 2027 7475 6e61 272c 2027 6d61 796f  ', 'tuna', 'mayo
-00019890: 6e6e 6169 7365 272c 2027 6272 6561 6427  nnaise', 'bread'
-000198a0: 2c20 2763 6865 6573 6527 7d5d 292c 0a20  , 'cheese'}]),. 
-000198b0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-000198c0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-000198d0: 7463 6865 7320 3d20 7365 6c66 2e72 6563  tches = self.rec
-000198e0: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
-000198f0: 6564 6965 6e74 7328 7175 6572 792c 206d  edients(query, m
-00019900: 696e 5f73 636f 7265 3d2d 3130 3030 302c  in_score=-10000,
-00019910: 2061 735f 7461 626c 653d 4661 6c73 652c   as_table=False,
-00019920: 2069 6e63 6c75 6465 5f77 6f72 6473 3d54   include_words=T
-00019930: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00019940: 206d 6174 6368 5f69 6473 203d 205b 7265   match_ids = [re
-00019950: 6369 7065 2e69 6420 666f 7220 7265 6369  cipe.id for reci
-00019960: 7065 2c20 7363 6f72 652c 2077 6f72 6473  pe, score, words
-00019970: 2069 6e20 6d61 7463 6865 735d 0a20 2020   in matches].   
-00019980: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
-00019990: 6570 7228 7175 6572 7929 2c20 272d 3e27  epr(query), '->'
-000199a0: 2c20 5b28 7265 6369 7065 2e69 642c 2073  , [(recipe.id, s
-000199b0: 636f 7265 2c20 776f 7264 7329 2066 6f72  core, words) for
-000199c0: 2072 6563 6970 652c 2073 636f 7265 2c20   recipe, score, 
-000199d0: 776f 7264 7320 696e 206d 6174 6368 6573  words in matches
-000199e0: 5d29 0a20 2020 2020 2020 2020 2020 2077  ]).            w
-000199f0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00019a00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00019a10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00019a20: 7175 616c 2865 7870 6563 7465 642c 206d  qual(expected, m
-00019a30: 6174 6368 5f69 6473 2c0a 2020 2020 2020  atch_ids,.      
-00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a50: 2020 2020 2020 2020 2020 2066 2269 6e76             f"inv
-00019a60: 616c 6964 2072 6573 756c 7473 2066 6f72  alid results for
-00019a70: 2071 7565 7279 207b 7175 6572 7921 727d   query {query!r}
-00019a80: 2c20 6578 7065 6374 6564 207b 6578 7065  , expected {expe
-00019a90: 6374 6564 7d2c 2067 6f74 207b 6d61 7463  cted}, got {matc
-00019aa0: 685f 6964 737d 2229 0a20 2020 2020 2020  h_ids}").       
-00019ab0: 2020 2020 206d 6174 6368 5f77 6f72 6473       match_words
-00019ac0: 203d 205b 7365 7428 776f 7264 7329 2066   = [set(words) f
-00019ad0: 6f72 2072 6563 6970 652c 2073 636f 7265  or recipe, score
-00019ae0: 2c20 776f 7264 7320 696e 206d 6174 6368  , words in match
-00019af0: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
-00019b00: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00019b10: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00019b20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00019b30: 4571 7561 6c28 6578 7065 6374 6564 5f77  Equal(expected_w
-00019b40: 6f72 6473 2c20 6d61 7463 685f 776f 7264  ords, match_word
-00019b50: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00019b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b70: 2020 2020 2269 6e76 616c 6964 206d 6174      "invalid mat
-00019b80: 6368 2077 6f72 6473 2066 6f72 2071 7565  ch words for que
-00019b90: 7279 207b 2172 7d2c 2065 7870 6563 7465  ry {!r}, expecte
-00019ba0: 6420 7b7d 2c20 676f 7420 7b7d 222e 666f  d {}, got {}".fo
-00019bb0: 726d 6174 2871 7565 7279 2c0a 2020 2020  rmat(query,.    
-00019bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c10: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00019c20: 7065 6374 6564 5f77 6f72 6473 2c0a 2020  pected_words,.  
-00019c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c90: 6d61 7463 685f 776f 7264 7329 290a 0a20  match_words)).. 
-00019ca0: 2020 2040 616e 6e6f 756e 6365 5f74 6573     @announce_tes
-00019cb0: 740a 2020 2020 6465 6620 7465 7374 5f73  t.    def test_s
-00019cc0: 6561 7263 685f 7769 7468 5f6c 696d 6974  earch_with_limit
-00019cd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00019ce0: 666f 7220 7175 6572 792c 2065 7870 6563  for query, expec
-00019cf0: 7465 6420 696e 205b 0a20 2020 2020 2020  ted in [.       
-00019d00: 2020 2020 2028 2222 2c20 5b5d 292c 0a20       ("", []),. 
-00019d10: 2020 2020 2020 2020 2020 2028 2274 756e             ("tun
-00019d20: 6122 2c20 5b31 2c20 365d 292c 0a20 2020  a", [1, 6]),.   
-00019d30: 2020 2020 2020 2020 2028 2274 756e 6120           ("tuna 
-00019d40: 2b63 6865 6573 6522 2c20 5b36 2c20 332c  +cheese", [6, 3,
-00019d50: 2034 5d29 2c0a 2020 2020 2020 2020 2020   4]),.          
-00019d60: 2020 2822 7069 6e65 6170 706c 6520 2b62    ("pineapple +b
-00019d70: 6163 6f6e 206c 6574 7475 6365 2062 6565  acon lettuce bee
-00019d80: 6620 2d73 6175 6572 6b72 6175 7420 746f  f -sauerkraut to
-00019d90: 6d61 746f 222c 205b 392c 2031 332c 2032  mato", [9, 13, 2
-00019da0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019db0: 2822 7069 7a7a 6120 646f 7567 6820 2d70  ("pizza dough -p
-00019dc0: 696e 6561 7070 6c65 222c 205b 332c 2034  ineapple", [3, 4
-00019dd0: 2c20 325d 292c 0a20 2020 2020 2020 2020  , 2]),.         
-00019de0: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
-00019df0: 202d 2d70 696e 6561 7070 6c65 222c 205b   --pineapple", [
-00019e00: 332c 2034 5d29 2c0a 2020 2020 2020 2020  3, 4]),.        
-00019e10: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
-00019e20: 6e22 2c20 5b39 2c20 352c 2036 5d29 2c0a  n", [9, 5, 6]),.
-00019e30: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
-00019e40: 6561 6420 2b2b 6261 636f 6e22 2c20 5b39  ead ++bacon", [9
-00019e50: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
-00019e60: 2020 2020 2822 6272 6561 6420 2b2b 616e      ("bread ++an
-00019e70: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
-00019e80: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-00019e90: 6164 202b 2b62 6163 6f6e 202b 2b61 6e63  ad ++bacon ++anc
-00019ea0: 686f 7669 6573 222c 205b 5d29 2c0a 2020  hovies", []),.  
-00019eb0: 2020 2020 2020 2020 2020 2822 6272 6561            ("brea
-00019ec0: 6420 6261 636f 6e20 2d2d 616e 6368 6f76  d bacon --anchov
-00019ed0: 6965 7322 2c20 5b39 2c20 352c 2036 5d29  ies", [9, 5, 6])
-00019ee0: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
-00019ef0: 2020 2020 2020 2020 206d 6174 6368 6573           matches
-00019f00: 203d 2073 656c 662e 7265 6369 7065 732e   = self.recipes.
-00019f10: 7365 6172 6368 2e69 6e67 7265 6469 656e  search.ingredien
-00019f20: 7473 2871 7565 7279 2c20 6173 5f74 6162  ts(query, as_tab
-00019f30: 6c65 3d46 616c 7365 2c20 6d69 6e5f 7363  le=False, min_sc
-00019f40: 6f72 653d 2d31 3030 3030 2c20 6c69 6d69  ore=-10000, limi
-00019f50: 743d 3329 0a20 2020 2020 2020 2020 2020  t=3).           
-00019f60: 206d 6174 6368 5f69 6473 203d 205b 7265   match_ids = [re
-00019f70: 6369 7065 2e69 6420 666f 7220 7265 6369  cipe.id for reci
-00019f80: 7065 2c20 5f20 696e 206d 6174 6368 6573  pe, _ in matches
-00019f90: 5d0a 2020 2020 2020 2020 2020 2020 7072  ].            pr
-00019fa0: 696e 7428 7265 7072 2871 7565 7279 292c  int(repr(query),
-00019fb0: 2027 2d3e 272c 205b 2872 6563 6970 652e   '->', [(recipe.
-00019fc0: 6964 2c20 7363 6f72 6529 2066 6f72 2072  id, score) for r
-00019fd0: 6563 6970 652c 2073 636f 7265 2069 6e20  ecipe, score in 
-00019fe0: 6d61 7463 6865 735d 290a 2020 2020 2020  matches]).      
-00019ff0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0001a000: 7375 6254 6573 7428 7175 6572 793d 7175  subTest(query=qu
-0001a010: 6572 7929 3a0a 2020 2020 2020 2020 2020  ery):.          
-0001a020: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001a030: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
-0001a040: 206d 6174 6368 5f69 6473 2c0a 2020 2020   match_ids,.    
-0001a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a060: 2020 2020 2020 2020 2020 2020 2066 2269               f"i
-0001a070: 6e76 616c 6964 2072 6573 756c 7473 2066  nvalid results f
-0001a080: 6f72 2071 7565 7279 207b 7175 6572 7921  or query {query!
-0001a090: 727d 2c20 6578 7065 6374 6564 207b 6578  r}, expected {ex
-0001a0a0: 7065 6374 6564 7d2c 2067 6f74 207b 6d61  pected}, got {ma
-0001a0b0: 7463 685f 6964 737d 2229 0a0a 2020 2020  tch_ids}")..    
-0001a0c0: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-0001a0d0: 2020 2064 6566 2074 6573 745f 7365 6172     def test_sear
-0001a0e0: 6368 5f77 6974 685f 6d69 6e5f 7363 6f72  ch_with_min_scor
-0001a0f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0001a100: 2066 6f72 2071 7565 7279 2c20 6578 7065   for query, expe
-0001a110: 6374 6564 2069 6e20 5b0a 2020 2020 2020  cted in [.      
-0001a120: 2020 2020 2020 2822 222c 205b 5d29 2c0a        ("", []),.
-0001a130: 2020 2020 2020 2020 2020 2020 2822 7475              ("tu
-0001a140: 6e61 222c 205b 5d29 2c0a 2020 2020 2020  na", []),.      
-0001a150: 2020 2020 2020 2822 7475 6e61 202b 6368        ("tuna +ch
-0001a160: 6565 7365 222c 205b 362c 5d29 2c0a 2020  eese", [6,]),.  
-0001a170: 2020 2020 2020 2020 2020 2822 7069 6e65            ("pine
-0001a180: 6170 706c 6520 2b62 6163 6f6e 206c 6574  apple +bacon let
-0001a190: 7475 6365 2062 6565 6620 2d73 6175 6572  tuce beef -sauer
-0001a1a0: 6b72 6175 7420 746f 6d61 746f 222c 205b  kraut tomato", [
-0001a1b0: 392c 2031 335d 292c 0a20 2020 2020 2020  9, 13]),.       
-0001a1c0: 2020 2020 2028 2270 697a 7a61 2064 6f75       ("pizza dou
-0001a1d0: 6768 202d 7069 6e65 6170 706c 6522 2c20  gh -pineapple", 
-0001a1e0: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-0001a1f0: 2028 2270 697a 7a61 2064 6f75 6768 202d   ("pizza dough -
-0001a200: 2d70 696e 6561 7070 6c65 222c 205b 5d29  -pineapple", [])
-0001a210: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-0001a220: 6272 6561 6420 6261 636f 6e22 2c20 5b5d  bread bacon", []
-0001a230: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001a240: 2262 7265 6164 202b 2b62 6163 6f6e 222c  "bread ++bacon",
-0001a250: 205b 392c 5d29 2c0a 2020 2020 2020 2020   [9,]),.        
-0001a260: 2020 2020 2822 6272 6561 6420 2b2b 616e      ("bread ++an
-0001a270: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
-0001a280: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-0001a290: 6164 202b 2b62 6163 6f6e 202b 2b61 6e63  ad ++bacon ++anc
-0001a2a0: 686f 7669 6573 222c 205b 5d29 2c0a 2020  hovies", []),.  
-0001a2b0: 2020 2020 2020 2020 2020 2822 6272 6561            ("brea
-0001a2c0: 6420 6261 636f 6e20 2d2d 616e 6368 6f76  d bacon --anchov
-0001a2d0: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-0001a2e0: 2020 205d 3a0a 2020 2020 2020 2020 2020     ]:.          
-0001a2f0: 2020 6d61 7463 6865 7320 3d20 7365 6c66    matches = self
-0001a300: 2e72 6563 6970 6573 2e73 6561 7263 682e  .recipes.search.
-0001a310: 696e 6772 6564 6965 6e74 7328 7175 6572  ingredients(quer
-0001a320: 792c 2061 735f 7461 626c 653d 4661 6c73  y, as_table=Fals
-0001a330: 652c 206d 696e 5f73 636f 7265 3d31 3030  e, min_score=100
-0001a340: 3029 0a20 2020 2020 2020 2020 2020 206d  0).            m
-0001a350: 6174 6368 5f69 6473 203d 205b 7265 6369  atch_ids = [reci
-0001a360: 7065 2e69 6420 666f 7220 7265 6369 7065  pe.id for recipe
-0001a370: 2c20 5f20 696e 206d 6174 6368 6573 5d0a  , _ in matches].
-0001a380: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0001a390: 7428 7265 7072 2871 7565 7279 292c 2027  t(repr(query), '
-0001a3a0: 2d3e 272c 205b 2872 6563 6970 652e 6964  ->', [(recipe.id
-0001a3b0: 2c20 7363 6f72 6529 2066 6f72 2072 6563  , score) for rec
-0001a3c0: 6970 652c 2073 636f 7265 2069 6e20 6d61  ipe, score in ma
-0001a3d0: 7463 6865 735d 290a 2020 2020 2020 2020  tches]).        
-0001a3e0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0001a3f0: 6254 6573 7428 7175 6572 793d 7175 6572  bTest(query=quer
-0001a400: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
-0001a410: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001a420: 7175 616c 2865 7870 6563 7465 642c 206d  qual(expected, m
-0001a430: 6174 6368 5f69 6473 2c0a 2020 2020 2020  atch_ids,.      
-0001a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a450: 2020 2020 2020 2020 2020 2066 2269 6e76             f"inv
-0001a460: 616c 6964 2072 6573 756c 7473 2066 6f72  alid results for
-0001a470: 2071 7565 7279 207b 7175 6572 7921 727d   query {query!r}
-0001a480: 2c20 6578 7065 6374 6564 207b 6578 7065  , expected {expe
-0001a490: 6374 6564 7d2c 2067 6f74 207b 6d61 7463  cted}, got {matc
-0001a4a0: 685f 6964 737d 2229 0a0a 2020 2020 4061  h_ids}")..    @a
-0001a4b0: 6e6e 6f75 6e63 655f 7465 7374 0a20 2020  nnounce_test.   
-0001a4c0: 2064 6566 2074 6573 745f 7365 6172 6368   def test_search
-0001a4d0: 5f77 6974 685f 6173 5f74 6162 6c65 2873  _with_as_table(s
-0001a4e0: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
-0001a4f0: 7220 7175 6572 792c 2065 7870 6563 7465  r query, expecte
-0001a500: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
-0001a510: 2020 2028 2222 2c20 5b5d 292c 0a20 2020     ("", []),.   
-0001a520: 2020 2020 2020 2020 2028 2274 756e 6122           ("tuna"
-0001a530: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
-0001a540: 2020 2028 2274 756e 6120 2b63 6865 6573     ("tuna +chees
-0001a550: 6522 2c20 5b36 2c5d 292c 0a20 2020 2020  e", [6,]),.     
-0001a560: 2020 2020 2020 2028 2270 696e 6561 7070         ("pineapp
-0001a570: 6c65 202b 6261 636f 6e20 6c65 7474 7563  le +bacon lettuc
-0001a580: 6520 6265 6566 202d 7361 7565 726b 7261  e beef -sauerkra
-0001a590: 7574 2074 6f6d 6174 6f22 2c20 5b39 2c20  ut tomato", [9, 
-0001a5a0: 3133 5d29 2c0a 2020 2020 2020 2020 2020  13]),.          
-0001a5b0: 2020 2822 7069 7a7a 6120 646f 7567 6820    ("pizza dough 
-0001a5c0: 2d70 696e 6561 7070 6c65 222c 205b 5d29  -pineapple", [])
-0001a5d0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-0001a5e0: 7069 7a7a 6120 646f 7567 6820 2d2d 7069  pizza dough --pi
-0001a5f0: 6e65 6170 706c 6522 2c20 5b5d 292c 0a20  neapple", []),. 
-0001a600: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-0001a610: 6164 2062 6163 6f6e 222c 205b 5d29 2c0a  ad bacon", []),.
-0001a620: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
-0001a630: 6561 6420 2b2b 6261 636f 6e22 2c20 5b39  ead ++bacon", [9
-0001a640: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
-0001a650: 2028 2262 7265 6164 202b 2b61 6e63 686f   ("bread ++ancho
-0001a660: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
-0001a670: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-0001a680: 2b2b 6261 636f 6e20 2b2b 616e 6368 6f76  ++bacon ++anchov
-0001a690: 6965 7322 2c20 5b5d 292c 0a20 2020 2020  ies", []),.     
-0001a6a0: 2020 2020 2020 2028 2262 7265 6164 2062         ("bread b
-0001a6b0: 6163 6f6e 202d 2d61 6e63 686f 7669 6573  acon --anchovies
-0001a6c0: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
-0001a6d0: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
-0001a6e0: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
-0001a6f0: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
-0001a700: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-0001a710: 6d69 6e5f 7363 6f72 653d 3130 3030 2c20  min_score=1000, 
-0001a720: 6173 5f74 6162 6c65 3d54 7275 6529 0a20  as_table=True). 
-0001a730: 2020 2020 2020 2020 2020 206d 6174 6368             match
-0001a740: 5f69 6473 203d 205b 7265 6369 7065 2e69  _ids = [recipe.i
-0001a750: 6420 666f 7220 7265 6369 7065 2069 6e20  d for recipe in 
-0001a760: 6d61 7463 6865 735d 0a20 2020 2020 2020  matches].       
-0001a770: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
-0001a780: 7175 6572 7929 2c20 272d 3e27 2c20 5b28  query), '->', [(
-0001a790: 7265 6369 7065 2e69 642c 2072 6563 6970  recipe.id, recip
-0001a7a0: 652e 696e 6772 6564 6965 6e74 735f 7365  e.ingredients_se
-0001a7b0: 6172 6368 5f73 636f 7265 2920 666f 7220  arch_score) for 
-0001a7c0: 7265 6369 7065 2069 6e20 6d61 7463 6865  recipe in matche
-0001a7d0: 735d 290a 2020 2020 2020 2020 2020 2020  s]).            
-0001a7e0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0001a7f0: 7428 7175 6572 793d 7175 6572 7929 3a0a  t(query=query):.
-0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0001a820: 2865 7870 6563 7465 642c 206d 6174 6368  (expected, match
-0001a830: 5f69 6473 2c0a 2020 2020 2020 2020 2020  _ids,.          
-0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a850: 2020 2020 2020 2066 2269 6e76 616c 6964         f"invalid
-0001a860: 2072 6573 756c 7473 2066 6f72 2071 7565   results for que
-0001a870: 7279 207b 7175 6572 7921 727d 2c20 6578  ry {query!r}, ex
-0001a880: 7065 6374 6564 207b 6578 7065 6374 6564  pected {expected
-0001a890: 7d2c 2067 6f74 207b 6d61 7463 685f 6964  }, got {match_id
-0001a8a0: 737d 2229 0a0a 2020 2020 2020 2020 2020  s}")..          
-0001a8b0: 2020 7363 6f72 655f 6174 7472 203d 2022    score_attr = "
-0001a8c0: 696e 6772 6564 6965 6e74 735f 7365 6172  ingredients_sear
-0001a8d0: 6368 5f73 636f 7265 220a 2020 2020 2020  ch_score".      
-0001a8e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001a8f0: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
-0001a900: 2020 2020 2020 2061 6c6c 280a 2020 2020         all(.    
-0001a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a920: 6861 7361 7474 7228 6d61 7463 6865 732e  hasattr(matches.
-0001a930: 6279 2e69 645b 6d69 645d 2c20 7363 6f72  by.id[mid], scor
-0001a940: 655f 6174 7472 290a 2020 2020 2020 2020  e_attr).        
-0001a950: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a960: 6d69 6420 696e 206d 6174 6368 5f69 6473  mid in match_ids
-0001a970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a980: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-0001a990: 2020 2020 6622 6173 5f74 6162 6c65 2064      f"as_table d
-0001a9a0: 6964 206e 6f74 2070 6f70 756c 6174 6520  id not populate 
-0001a9b0: 736f 6d65 2073 6561 7263 6820 7265 636f  some search reco
-0001a9c0: 7264 7320 7769 7468 207b 7363 6f72 655f  rds with {score_
-0001a9d0: 6174 7472 2172 7d22 0a20 2020 2020 2020  attr!r}".       
-0001a9e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001a9f0: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-0001aa00: 616c 7365 280a 2020 2020 2020 2020 2020  alse(.          
-0001aa10: 2020 2020 2020 616e 7928 0a20 2020 2020        any(.     
-0001aa20: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0001aa30: 6173 6174 7472 2873 656c 662e 7265 6369  asattr(self.reci
-0001aa40: 7065 732e 6279 2e69 645b 6d69 645d 2c20  pes.by.id[mid], 
-0001aa50: 7363 6f72 655f 6174 7472 290a 2020 2020  score_attr).    
-0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa70: 666f 7220 6d69 6420 696e 206d 6174 6368  for mid in match
-0001aa80: 5f69 6473 0a20 2020 2020 2020 2020 2020  _ids.           
-0001aa90: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-0001aaa0: 2020 2020 2020 2020 6622 6173 5f74 6162          f"as_tab
-0001aab0: 6c65 2070 6f70 756c 6174 6564 2073 6f6d  le populated som
-0001aac0: 6520 6f72 6967 696e 616c 2072 6563 6f72  e original recor
-0001aad0: 6473 2077 6974 6820 7b73 636f 7265 5f61  ds with {score_a
-0001aae0: 7474 7221 727d 220a 2020 2020 2020 2020  ttr!r}".        
-0001aaf0: 2020 2020 290a 0a63 6c61 7373 2054 6162      )..class Tab
-0001ab00: 6c65 5365 6172 6368 5465 7374 735f 4461  leSearchTests_Da
-0001ab10: 7461 4f62 6a65 6374 7328 5461 626c 6553  taObjects(TableS
-0001ab20: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
-0001ab30: 6744 6174 614f 626a 6563 7473 293a 0a20  gDataObjects):. 
-0001ab40: 2020 2070 6173 730a 0a63 6c61 7373 2054     pass..class T
-0001ab50: 6162 6c65 5365 6172 6368 5465 7374 735f  ableSearchTests_
-0001ab60: 4e61 6d65 6474 7570 6c65 7328 5461 626c  Namedtuples(Tabl
-0001ab70: 6553 6561 7263 6854 6573 7473 2c20 5573  eSearchTests, Us
-0001ab80: 696e 674e 616d 6564 7475 706c 6573 293a  ingNamedtuples):
-0001ab90: 0a20 2020 2070 6173 730a 0a63 6c61 7373  .    pass..class
-0001aba0: 2054 6162 6c65 5365 6172 6368 5465 7374   TableSearchTest
-0001abb0: 735f 5479 7069 6e67 4e61 6d65 6474 7570  s_TypingNamedtup
-0001abc0: 6c65 7328 5461 626c 6553 6561 7263 6854  les(TableSearchT
-0001abd0: 6573 7473 2c20 5573 696e 6754 7970 696e  ests, UsingTypin
-0001abe0: 674e 616d 6564 5475 706c 6529 3a0a 2020  gNamedTuple):.  
-0001abf0: 2020 7061 7373 0a0a 636c 6173 7320 5461    pass..class Ta
-0001ac00: 626c 6553 6561 7263 6854 6573 7473 5f54  bleSearchTests_T
-0001ac10: 7970 696e 6754 7970 6564 4469 6374 2854  ypingTypedDict(T
-0001ac20: 6162 6c65 5365 6172 6368 5465 7374 732c  ableSearchTests,
-0001ac30: 2055 7369 6e67 5479 7069 6e67 5479 7065   UsingTypingType
-0001ac40: 6444 6963 7429 3a0a 2020 2020 7061 7373  dDict):.    pass
-0001ac50: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
-0001ac60: 7263 6854 6573 7473 5f53 6c6f 7474 6564  rchTests_Slotted
-0001ac70: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
-0001ac80: 732c 2055 7369 6e67 536c 6f74 7465 644f  s, UsingSlottedO
-0001ac90: 626a 6563 7473 293a 0a20 2020 2070 6173  bjects):.    pas
-0001aca0: 730a 0a63 6c61 7373 2054 6162 6c65 5365  s..class TableSe
-0001acb0: 6172 6368 5465 7374 735f 5369 6d70 6c65  archTests_Simple
-0001acc0: 4e61 6d65 7370 6163 6528 5461 626c 6553  Namespace(TableS
-0001acd0: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
-0001ace0: 6753 696d 706c 654e 616d 6573 7061 6365  gSimpleNamespace
-0001acf0: 293a 0a20 2020 2070 6173 730a 0a69 6620  ):.    pass..if 
-0001ad00: 6461 7461 636c 6173 7365 7320 6973 206e  dataclasses is n
-0001ad10: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
-0001ad20: 7373 2054 6162 6c65 5365 6172 6368 5465  ss TableSearchTe
-0001ad30: 7374 735f 4461 7461 636c 6173 7365 7328  sts_Dataclasses(
-0001ad40: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-0001ad50: 2c20 5573 696e 6744 6174 6163 6c61 7373  , UsingDataclass
-0001ad60: 6573 293a 0a20 2020 2020 2020 2070 6173  es):.        pas
-0001ad70: 730a 0a69 6620 7079 6461 6e74 6963 2069  s..if pydantic i
-0001ad80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001ad90: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-0001ada0: 6854 6573 7473 5f50 7964 616e 7469 634d  hTests_PydanticM
-0001adb0: 6f64 656c 7328 5461 626c 6553 6561 7263  odels(TableSearc
-0001adc0: 6854 6573 7473 2c20 5573 696e 6750 7964  hTests, UsingPyd
-0001add0: 616e 7469 634d 6f64 656c 293a 0a20 2020  anticModel):.   
-0001ade0: 2020 2020 2070 6173 730a 0a20 2020 2063       pass..    c
-0001adf0: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
-0001ae00: 5465 7374 735f 5079 6461 6e74 6963 496d  Tests_PydanticIm
-0001ae10: 6d75 7461 626c 654d 6f64 656c 7328 5461  mutableModels(Ta
-0001ae20: 626c 6553 6561 7263 6854 6573 7473 2c20  bleSearchTests, 
-0001ae30: 5573 696e 6750 7964 616e 7469 6349 6d6d  UsingPydanticImm
-0001ae40: 7574 6162 6c65 4d6f 6465 6c29 3a0a 2020  utableModel):.  
-0001ae50: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0001ae60: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-0001ae70: 6854 6573 7473 5f50 7964 616e 7469 634f  hTests_PydanticO
-0001ae80: 524d 4d6f 6465 6c73 2854 6162 6c65 5365  RMModels(TableSe
-0001ae90: 6172 6368 5465 7374 732c 2055 7369 6e67  archTests, Using
-0001aea0: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-0001aeb0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0001aec0: 0a69 6620 6174 7472 2069 7320 6e6f 7420  .if attr is not 
-0001aed0: 4e6f 6e65 3a0a 2020 2020 636c 6173 7320  None:.    class 
-0001aee0: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-0001aef0: 5f41 7474 7243 6c61 7373 6573 2854 6162  _AttrClasses(Tab
-0001af00: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
-0001af10: 7369 6e67 4174 7472 436c 6173 7329 3a0a  singAttrClass):.
-0001af20: 2020 2020 2020 2020 7061 7373 0a0a 6966          pass..if
-0001af30: 2074 7261 6974 6c65 7473 2069 7320 6e6f   traitlets is no
-0001af40: 7420 4e6f 6e65 3a0a 2020 2020 636c 6173  t None:.    clas
-0001af50: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
-0001af60: 7473 5f54 7261 6974 6c65 7473 436c 6173  ts_TraitletsClas
-0001af70: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
-0001af80: 6573 7473 2c20 5573 696e 6754 7261 6974  ests, UsingTrait
-0001af90: 6c65 7473 436c 6173 7329 3a0a 2020 2020  letsClass):.    
-0001afa0: 2020 2020 7061 7373 0a0a 6966 2053 6c6f      pass..if Slo
-0001afb0: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
-0001afc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 636c  not None:.    cl
-0001afd0: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
-0001afe0: 6573 7473 5f53 6c6f 7474 6564 5769 7468  ests_SlottedWith
-0001aff0: 4469 6374 2854 6162 6c65 5365 6172 6368  Dict(TableSearch
-0001b000: 5465 7374 732c 2055 7369 6e67 536c 6f74  Tests, UsingSlot
-0001b010: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
-0001b020: 7473 293a 0a20 2020 2020 2020 2070 6173  ts):.        pas
-0001b030: 730a 0a0a 636c 6173 7320 496e 6974 6961  s...class Initia
-0001b040: 6c54 6573 7428 756e 6974 7465 7374 2e54  lTest(unittest.T
-0001b050: 6573 7443 6173 6529 3a0a 2020 2020 6672  estCase):.    fr
-0001b060: 6f6d 206c 6974 746c 6574 6162 6c65 2069  om littletable i
-0001b070: 6d70 6f72 7420 280a 2020 2020 2020 2020  mport (.        
-0001b080: 5f5f 7665 7273 696f 6e5f 5f20 6173 206c  __version__ as l
-0001b090: 6974 746c 6574 6162 6c65 5f76 6572 7369  ittletable_versi
-0001b0a0: 6f6e 2c0a 2020 2020 2020 2020 5f5f 7665  on,.        __ve
-0001b0b0: 7273 696f 6e5f 7469 6d65 5f5f 2061 7320  rsion_time__ as 
-0001b0c0: 6c69 7474 6c65 7461 626c 655f 7665 7273  littletable_vers
-0001b0d0: 696f 6e5f 7469 6d65 2c0a 2020 2020 2020  ion_time,.      
-0001b0e0: 2020 5f5f 7665 7273 696f 6e5f 696e 666f    __version_info
-0001b0f0: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
-0001b100: 655f 7665 7273 696f 6e5f 696e 666f 2c0a  e_version_info,.
-0001b110: 2020 2020 290a 0a20 2020 2070 7269 6e74      )..    print
-0001b120: 280a 2020 2020 2020 2020 6622 4265 6769  (.        f"Begi
-0001b130: 6e6e 696e 6720 7465 7374 206f 6620 6c69  nning test of li
-0001b140: 7474 6c65 7461 626c 652c 2076 6572 7369  ttletable, versi
-0001b150: 6f6e 207b 6c69 7474 6c65 7461 626c 655f  on {littletable_
-0001b160: 7665 7273 696f 6e7d 2c20 7b6c 6974 746c  version}, {littl
-0001b170: 6574 6162 6c65 5f76 6572 7369 6f6e 5f74  etable_version_t
-0001b180: 696d 657d 222c 0a20 2020 2029 0a20 2020  ime}",.    ).   
-0001b190: 2070 7269 6e74 286c 6974 746c 6574 6162   print(littletab
-0001b1a0: 6c65 5f76 6572 7369 6f6e 5f69 6e66 6f29  le_version_info)
-0001b1b0: 0a20 2020 2070 7269 6e74 2822 5079 7468  .    print("Pyth
-0001b1c0: 6f6e 2076 6572 7369 6f6e 222c 2073 7973  on version", sys
-0001b1d0: 2e76 6572 7369 6f6e 290a 2020 2020 7072  .version).    pr
-0001b1e0: 696e 7428 290a 0a0a 636c 6173 7320 5374  int()...class St
-0001b1f0: 6f72 6167 6549 6e64 6570 656e 6465 6e74  orageIndependent
-0001b200: 5465 7374 7328 756e 6974 7465 7374 2e54  Tests(unittest.T
-0001b210: 6573 7443 6173 6529 3a0a 2020 2020 4061  estCase):.    @a
-0001b220: 6e6e 6f75 6e63 655f 7465 7374 0a20 2020  nnounce_test.   
-0001b230: 2064 6566 2074 6573 745f 6e6f 726d 616c   def test_normal
-0001b240: 697a 655f 7374 7228 7365 6c66 293a 0a20  ize_str(self):. 
-0001b250: 2020 2020 2020 2066 6f72 2069 6e5f 776f         for in_wo
-0001b260: 7264 2c20 6578 7065 6374 6564 5f77 6f72  rd, expected_wor
-0001b270: 6420 696e 205b 0a20 2020 2020 2020 2020  d in [.         
-0001b280: 2020 2028 226e 6f63 6861 6e67 6522 2c20     ("nochange", 
-0001b290: 226e 6f63 6861 6e67 6522 292c 0a20 2020  "nochange"),.   
-0001b2a0: 2020 2020 2020 2020 2028 2254 6f4c 6f77           ("ToLow
-0001b2b0: 6572 222c 2022 746f 6c6f 7765 7222 292c  er", "tolower"),
-0001b2c0: 0a20 2020 2020 2020 2020 2020 2028 2249  .            ("I
-0001b2d0: 2e42 2e4d 2e22 2c20 2269 626d 2229 2c0a  .B.M.", "ibm"),.
-0001b2e0: 2020 2020 2020 2020 2020 2020 2822 472e              ("G.
-0001b2f0: 452e 222c 2022 6765 2229 2c0a 2020 2020  E.", "ge"),.    
-0001b300: 2020 2020 2020 2020 2822 4d2e 222c 2022          ("M.", "
-0001b310: 6d22 292c 0a20 2020 2020 2020 2020 2020  m"),.           
-0001b320: 2028 224d 2e78 797a 222c 2022 6d22 292c   ("M.xyz", "m"),
-0001b330: 0a20 2020 2020 2020 2020 2020 2028 222a  .            ("*
-0001b340: 7878 782d 6868 6822 2c20 2278 7878 2d68  xxx-hhh", "xxx-h
-0001b350: 6868 2229 2c0a 2020 2020 2020 2020 2020  hh"),.          
-0001b360: 2020 2822 2b62 6c61 6846 6f6f 222c 2022    ("+blahFoo", "
-0001b370: 626c 6168 666f 6f22 292c 0a20 2020 2020  blahfoo"),.     
-0001b380: 2020 2020 2020 2023 2028 2266 6f78 6573         # ("foxes
-0001b390: 222c 2022 666f 7822 292c 0a20 2020 2020  ", "fox"),.     
-0001b3a0: 2020 2020 2020 2023 2028 2263 6875 7263         # ("churc
-0001b3b0: 6865 7322 2c20 2263 6875 7263 6822 292c  hes", "church"),
-0001b3c0: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
-0001b3d0: 2264 7265 7373 6573 222c 2022 6472 6573  "dresses", "dres
-0001b3e0: 7322 292c 0a20 2020 2020 2020 205d 3a0a  s"),.        ]:.
-0001b3f0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0001b400: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
-0001b410: 5f77 6f72 6429 3a0a 2020 2020 2020 2020  _word):.        
-0001b420: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001b430: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
-0001b440: 645f 776f 7264 2c20 6c74 2e54 6162 6c65  d_word, lt.Table
-0001b450: 2e5f 6e6f 726d 616c 697a 655f 776f 7264  ._normalize_word
-0001b460: 2869 6e5f 776f 7264 2929 0a0a 2020 2020  (in_word))..    
-0001b470: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
-0001b480: 7a65 5f73 7472 5f67 656e 2873 656c 6629  ze_str_gen(self)
-0001b490: 3a0a 2020 2020 2020 2020 666f 7220 696e  :.        for in
-0001b4a0: 5f77 6f72 642c 2065 7870 6563 7465 645f  _word, expected_
-0001b4b0: 776f 7264 7320 696e 205b 0a20 2020 2020  words in [.     
-0001b4c0: 2020 2020 2020 2028 226e 6f63 6861 6e67         ("nochang
-0001b4d0: 6522 2c20 5b22 6e6f 6368 616e 6765 225d  e", ["nochange"]
-0001b4e0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001b4f0: 2254 6f4c 6f77 6572 222c 205b 2274 6f6c  "ToLower", ["tol
-0001b500: 6f77 6572 225d 292c 0a20 2020 2020 2020  ower"]),.       
-0001b510: 2020 2020 2028 2249 2e42 2e4d 2e22 2c20       ("I.B.M.", 
-0001b520: 5b22 692e 622e 6d2e 222c 2022 6962 6d22  ["i.b.m.", "ibm"
-0001b530: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0001b540: 2822 472e 452e 222c 205b 2267 2e65 2e22  ("G.E.", ["g.e."
-0001b550: 2c20 2267 6522 5d29 2c0a 2020 2020 2020  , "ge"]),.      
-0001b560: 2020 2020 2020 2822 412e 492e 222c 205b        ("A.I.", [
-0001b570: 2261 2e69 2e22 2c20 2261 6922 5d29 2c0a  "a.i.", "ai"]),.
-0001b580: 2020 2020 2020 2020 2020 2020 2822 4149              ("AI
-0001b590: 222c 205b 2261 6922 5d29 2c0a 2020 2020  ", ["ai"]),.    
-0001b5a0: 2020 2020 2020 2020 2822 4d2e 222c 205b          ("M.", [
-0001b5b0: 226d 225d 292c 0a20 2020 2020 2020 2020  "m"]),.         
-0001b5c0: 2020 2028 226d 6d2e 7879 7a22 2c20 5b22     ("mm.xyz", ["
-0001b5d0: 6d6d 222c 2022 6d6d 2e78 797a 222c 2022  mm", "mm.xyz", "
-0001b5e0: 7879 7a22 5d29 2c0a 2020 2020 2020 2020  xyz"]),.        
-0001b5f0: 2020 2020 2822 4d4d 2e78 797a 222c 205b      ("MM.xyz", [
-0001b600: 226d 6d22 2c20 226d 6d2e 7879 7a22 2c20  "mm", "mm.xyz", 
-0001b610: 2278 797a 225d 292c 0a20 2020 2020 2020  "xyz"]),.       
-0001b620: 2020 2020 2028 2254 6872 6561 6469 6e67       ("Threading
-0001b630: 2e69 7341 6c69 7665 2829 222c 205b 2769  .isAlive()", ['i
-0001b640: 7361 6c69 7665 272c 2027 7468 7265 6164  salive', 'thread
-0001b650: 696e 6727 2c20 2774 6872 6561 6469 6e67  ing', 'threading
-0001b660: 2e69 7361 6c69 7665 275d 292c 0a20 2020  .isalive']),.   
-0001b670: 2020 2020 2020 2020 2028 222a 7878 782d           ("*xxx-
-0001b680: 6868 6822 2c20 5b27 6868 6827 2c20 2778  hhh", ['hhh', 'x
-0001b690: 7878 272c 2027 7878 782d 6868 6827 5d29  xx', 'xxx-hhh'])
-0001b6a0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-0001b6b0: 2b62 6c61 6846 6f6f 222c 205b 2262 6c61  +blahFoo", ["bla
-0001b6c0: 6866 6f6f 225d 292c 0a20 2020 2020 2020  hfoo"]),.       
-0001b6d0: 2020 2020 2028 2273 7472 2e6c 7374 7269       ("str.lstri
-0001b6e0: 7022 2c20 5b22 6c73 7472 6970 222c 2022  p", ["lstrip", "
-0001b6f0: 7374 7222 2c20 2273 7472 2e6c 7374 7269  str", "str.lstri
-0001b700: 7022 5d29 2c0a 2020 2020 2020 2020 2020  p"]),.          
-0001b710: 2020 2822 7374 722e 6c73 7472 6970 2829    ("str.lstrip()
-0001b720: 222c 205b 226c 7374 7269 7022 2c20 2273  ", ["lstrip", "s
-0001b730: 7472 222c 2022 7374 722e 6c73 7472 6970  tr", "str.lstrip
-0001b740: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0001b750: 2028 2273 656c 662e 6173 7365 7274 4571   ("self.assertEq
-0001b760: 7561 6c73 222c 205b 2261 7373 6572 7465  uals", ["asserte
-0001b770: 7175 616c 7322 2c20 2273 656c 6622 2c20  quals", "self", 
-0001b780: 2273 656c 662e 6173 7365 7274 6571 7561  "self.assertequa
-0001b790: 6c73 225d 292c 0a20 2020 2020 2020 2020  ls"]),.         
-0001b7a0: 2020 2028 2254 6573 7443 6173 652e 6173     ("TestCase.as
-0001b7b0: 7365 7274 4571 7561 6c73 222c 205b 2261  sertEquals", ["a
-0001b7c0: 7373 6572 7465 7175 616c 7322 2c20 2274  ssertequals", "t
-0001b7d0: 6573 7463 6173 6522 2c20 2274 6573 7463  estcase", "testc
-0001b7e0: 6173 652e 6173 7365 7274 6571 7561 6c73  ase.assertequals
-0001b7f0: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0001b800: 2028 2275 6e69 7474 6573 742e 5465 7374   ("unittest.Test
-0001b810: 4361 7365 2e61 7373 6572 7445 7175 616c  Case.assertEqual
-0001b820: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-0001b830: 205b 2261 7373 6572 7465 7175 616c 7322   ["assertequals"
-0001b840: 2c20 2274 6573 7463 6173 6522 2c20 2275  , "testcase", "u
-0001b850: 6e69 7474 6573 7422 2c20 2275 6e69 7474  nittest", "unitt
-0001b860: 6573 742e 7465 7374 6361 7365 2e61 7373  est.testcase.ass
-0001b870: 6572 7465 7175 616c 7322 5d29 2c0a 2020  ertequals"]),.  
-0001b880: 2020 2020 2020 2020 2020 2822 666f 7865            ("foxe
-0001b890: 7322 2c20 5b22 666f 7822 2c20 2266 6f78  s", ["fox", "fox
-0001b8a0: 6573 225d 292c 0a20 2020 2020 2020 2020  es"]),.         
-0001b8b0: 2020 2028 2263 6875 7263 6865 7322 2c20     ("churches", 
-0001b8c0: 5b22 6368 7572 6368 222c 2022 6368 7572  ["church", "chur
-0001b8d0: 6368 6573 225d 292c 0a20 2020 2020 2020  ches"]),.       
-0001b8e0: 2020 2020 2028 2264 7265 7373 6573 222c       ("dresses",
-0001b8f0: 205b 2264 7265 7373 222c 2022 6472 6573   ["dress", "dres
-0001b900: 7365 7322 5d29 2c0a 2020 2020 2020 2020  ses"]),.        
-0001b910: 2020 2020 2822 6472 6573 7322 2c20 5b22      ("dress", ["
-0001b920: 6472 6573 7322 2c20 5d29 2c0a 2020 2020  dress", ]),.    
-0001b930: 2020 2020 2020 2020 2822 6269 6173 222c          ("bias",
-0001b940: 205b 2262 6961 7322 2c20 5d29 2c0a 2020   ["bias", ]),.  
-0001b950: 2020 2020 2020 2020 2020 2822 746f 7973            ("toys
-0001b960: 222c 205b 2274 6f79 222c 2022 746f 7973  ", ["toy", "toys
-0001b970: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0001b980: 2028 2262 6162 6965 7322 2c20 5b22 6261   ("babies", ["ba
-0001b990: 6269 6573 222c 2022 6261 6279 225d 292c  bies", "baby"]),
-0001b9a0: 0a20 2020 2020 2020 2020 2020 2028 2261  .            ("a
-0001b9b0: 6464 656e 6461 222c 205b 2261 6464 656e  ddenda", ["adden
-0001b9c0: 6461 222c 2022 6164 6465 6e64 756d 225d  da", "addendum"]
-0001b9d0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001b9e0: 2272 6162 6965 7322 2c20 5b22 7261 6269  "rabies", ["rabi
-0001b9f0: 6573 225d 292c 0a20 2020 2020 2020 2020  es"]),.         
-0001ba00: 2020 2028 226c 617a 696e 6573 7322 2c20     ("laziness", 
-0001ba10: 5b22 6c61 7a69 6e65 7373 225d 292c 0a20  ["laziness"]),. 
-0001ba20: 2020 2020 2020 2020 2020 2028 2270 6879             ("phy
-0001ba30: 7369 6373 222c 205b 2270 6879 7369 6373  sics", ["physics
-0001ba40: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0001ba50: 2028 2250 7974 686f 6e27 7322 2c20 5b22   ("Python's", ["
-0001ba60: 7079 7468 6f6e 225d 292c 0a20 2020 2020  python"]),.     
-0001ba70: 2020 2020 2020 2028 2756 616c 7565 4572         ('ValueEr
-0001ba80: 726f 7227 2c20 5b27 6572 726f 7227 2c20  ror', ['error', 
-0001ba90: 2776 616c 7565 6572 726f 7227 5d29 2c0a  'valueerror']),.
-0001baa0: 2020 2020 2020 2020 2020 2020 2827 4465              ('De
-0001bab0: 7072 6563 6174 696f 6e57 6172 6e69 6e67  precationWarning
-0001bac0: 272c 205b 2764 6570 7265 6361 7469 6f6e  ', ['deprecation
-0001bad0: 7761 726e 696e 6727 2c20 2777 6172 6e69  warning', 'warni
-0001bae0: 6e67 275d 292c 0a20 2020 2020 2020 2020  ng']),.         
-0001baf0: 2020 2028 2743 7573 746f 6d45 7863 6570     ('CustomExcep
-0001bb00: 7469 6f6e 272c 205b 2763 7573 746f 6d65  tion', ['custome
-0001bb10: 7863 6570 7469 6f6e 272c 2027 6578 6365  xception', 'exce
-0001bb20: 7074 696f 6e27 5d29 2c0a 2020 2020 2020  ption']),.      
-0001bb30: 2020 2020 2020 2827 7465 7272 6f72 272c        ('terror',
-0001bb40: 205b 2774 6572 726f 7227 5d29 2c0a 2020   ['terror']),.  
-0001bb50: 2020 2020 2020 2020 2020 2827 6572 726f            ('erro
-0001bb60: 7227 2c20 5b27 6572 726f 7227 5d29 2c0a  r', ['error']),.
-0001bb70: 2020 2020 2020 2020 5d3a 0a20 2020 2020          ]:.     
-0001bb80: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0001bb90: 2e73 7562 5465 7374 2869 6e5f 776f 7264  .subTest(in_word
-0001bba0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001bbb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001bbc0: 7561 6c28 6578 7065 6374 6564 5f77 6f72  ual(expected_wor
-0001bbd0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbf0: 2020 2020 2073 6f72 7465 6428 6c69 7374       sorted(list
-0001bc00: 286c 742e 5461 626c 652e 5f6e 6f72 6d61  (lt.Table._norma
-0001bc10: 6c69 7a65 5f77 6f72 645f 6765 6e28 696e  lize_word_gen(in
-0001bc20: 5f77 6f72 642c 2066 726f 7a65 6e73 6574  _word, frozenset
-0001bc30: 2829 2929 2929 0a0a 2020 2020 4061 6e6e  ()))))..    @ann
-0001bc40: 6f75 6e63 655f 7465 7374 0a20 2020 2064  ounce_test.    d
-0001bc50: 6566 2074 6573 745f 6e6f 726d 616c 697a  ef test_normaliz
-0001bc60: 655f 7370 6c69 7428 7365 6c66 293a 0a20  e_split(self):. 
-0001bc70: 2020 2020 2020 2066 6f72 2069 6e5f 7374         for in_st
-0001bc80: 722c 2065 7870 6563 7465 645f 7374 725f  r, expected_str_
-0001bc90: 7365 7420 696e 205b 0a20 2020 2020 2020  set in [.       
-0001bca0: 2020 2020 2028 2273 7472 2e6c 7374 7269       ("str.lstri
-0001bcb0: 7028 2922 2c20 5b22 6c73 7472 6970 222c  p()", ["lstrip",
-0001bcc0: 2022 7374 7222 2c20 2273 7472 2e6c 7374   "str", "str.lst
-0001bcd0: 7269 7022 5d29 2c0a 2020 2020 2020 2020  rip"]),.        
-0001bce0: 2020 2020 2822 7374 722e 6c73 7472 6970      ("str.lstrip
-0001bcf0: 2829 2073 7472 2e72 7374 7269 7028 2922  () str.rstrip()"
-0001bd00: 2c20 5b22 6c73 7472 6970 222c 2022 7273  , ["lstrip", "rs
-0001bd10: 7472 6970 222c 2022 7374 7222 2c20 2273  trip", "str", "s
-0001bd20: 7472 2e6c 7374 7269 7022 2c20 2273 7472  tr.lstrip", "str
-0001bd30: 2e72 7374 7269 7022 5d29 2c0a 2020 2020  .rstrip"]),.    
-0001bd40: 2020 2020 2020 2020 2320 2822 222c 205b          # ("", [
-0001bd50: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0001bd60: 2320 2822 222c 205b 5d29 2c0a 2020 2020  # ("", []),.    
-0001bd70: 2020 2020 2020 2020 2320 2822 222c 205b          # ("", [
-0001bd80: 5d29 2c0a 2020 2020 2020 2020 5d3a 0a20  ]),.        ]:. 
-0001bd90: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0001bda0: 7365 6c66 2e73 7562 5465 7374 2869 6e5f  self.subTest(in_
-0001bdb0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0001bdc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001bdd0: 7445 7175 616c 2865 7870 6563 7465 645f  tEqual(expected_
-0001bde0: 7374 725f 7365 742c 0a20 2020 2020 2020  str_set,.       
-0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be00: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-0001be10: 2873 6574 286c 742e 5461 626c 652e 5f6e  (set(lt.Table._n
-0001be20: 6f72 6d61 6c69 7a65 5f73 706c 6974 2869  ormalize_split(i
-0001be30: 6e5f 7374 7229 2929 290a 0a20 2020 2040  n_str))))..    @
-0001be40: 616e 6e6f 756e 6365 5f74 6573 740a 2020  announce_test.  
-0001be50: 2020 6465 6620 7465 7374 5f70 6c75 7261    def test_plura
-0001be60: 6c73 5f77 6974 685f 7472 6169 6c69 6e67  ls_with_trailing
-0001be70: 5f70 756e 6374 7561 7469 6f6e 2873 656c  _punctuation(sel
-0001be80: 6629 3a0a 2020 2020 2020 2020 666f 7220  f):.        for 
-0001be90: 286c 696e 652c 2065 7870 6563 7465 6429  (line, expected)
-0001bea0: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-0001beb0: 2020 2827 4920 636f 756c 6420 6865 6172    ('I could hear
-0001bec0: 2074 6865 2062 6162 6965 7320 6372 6965   the babies crie
-0001bed0: 732e 272c 205b 2762 6162 6965 7327 2c20  s.', ['babies', 
-0001bee0: 2762 6162 7927 2c20 2763 6f75 6c64 272c  'baby', 'could',
-0001bef0: 2027 6372 6965 7327 2c20 2763 7279 272c   'cries', 'cry',
-0001bf00: 2027 6865 6172 272c 2027 6927 2c20 2774   'hear', 'i', 't
-0001bf10: 6865 275d 292c 0a20 2020 2020 2020 2020  he']),.         
-0001bf20: 2020 2028 2757 686f 2061 7265 2074 686f     ('Who are tho
-0001bf30: 7365 2062 6162 6965 733f 272c 205b 2761  se babies?', ['a
-0001bf40: 7265 272c 2027 6261 6269 6573 272c 2027  re', 'babies', '
-0001bf50: 6261 6279 272c 2027 7468 6f73 6527 2c20  baby', 'those', 
-0001bf60: 2777 686f 275d 292c 0a20 2020 2020 2020  'who']),.       
-0001bf70: 2020 2020 2028 2257 686f 2074 6f6f 6b20       ("Who took 
-0001bf80: 7468 6520 6261 6269 6573 2720 7261 7474  the babies' ratt
-0001bf90: 6c65 7320 7468 6973 2074 696d 653f 222c  les this time?",
-0001bfa0: 0a20 2020 2020 2020 2020 2020 2020 5b27  .             ['
-0001bfb0: 6261 6269 6573 272c 2027 6261 6279 272c  babies', 'baby',
-0001bfc0: 2027 7261 7474 6c65 272c 2027 7261 7474   'rattle', 'ratt
-0001bfd0: 6c65 7327 2c20 2774 6865 272c 2027 7468  les', 'the', 'th
-0001bfe0: 6973 272c 2027 7469 6d65 272c 2027 746f  is', 'time', 'to
-0001bff0: 6f6b 272c 2027 7768 6f27 5d29 2c0a 2020  ok', 'who']),.  
-0001c000: 2020 2020 2020 2020 2020 2827 4920 6c6f            ('I lo
-0001c010: 7665 2074 6865 7365 2063 616b 6573 2127  ve these cakes!'
-0001c020: 2c20 5b27 6361 6b65 272c 2027 6361 6b65  , ['cake', 'cake
-0001c030: 7327 2c20 2769 272c 2027 6c6f 7665 272c  s', 'i', 'love',
-0001c040: 2027 7468 6573 6527 5d29 2c0a 2020 2020   'these']),.    
-0001c050: 2020 2020 2020 2020 2827 5768 656e 206d          ('When m
-0001c060: 7920 7769 6665 2063 6f6f 6b73 2c20 7368  y wife cooks, sh
-0001c070: 6520 6261 6b65 732e 272c 205b 2762 616b  e bakes.', ['bak
-0001c080: 6527 2c20 2762 616b 6573 272c 2027 636f  e', 'bakes', 'co
-0001c090: 6f6b 272c 2027 636f 6f6b 7327 2c20 276d  ok', 'cooks', 'm
-0001c0a0: 7927 2c20 2773 6865 272c 2027 7768 656e  y', 'she', 'when
-0001c0b0: 272c 2027 7769 6665 275d 292c 0a20 2020  ', 'wife']),.   
-0001c0c0: 2020 2020 2020 2020 2028 224c 6574 2773           ("Let's
-0001c0d0: 2067 6f20 7368 6f70 7069 6e67 2066 6f72   go shopping for
-0001c0e0: 2061 6e74 6971 7565 7321 222c 205b 2761   antiques!", ['a
-0001c0f0: 6e74 6971 7565 272c 2027 616e 7469 7175  ntique', 'antiqu
-0001c100: 6573 272c 2027 666f 7227 2c20 2767 6f27  es', 'for', 'go'
-0001c110: 2c20 276c 6574 272c 2027 7368 6f70 7069  , 'let', 'shoppi
-0001c120: 6e67 275d 292c 0a20 2020 2020 2020 2020  ng']),.         
-0001c130: 2020 2028 2754 6869 7320 6973 2061 6e20     ('This is an 
-0001c140: 616e 7469 7175 6520 7661 7365 2c20 776f  antique vase, wo
-0001c150: 7274 6820 7468 6f75 7361 6e64 7321 272c  rth thousands!',
-0001c160: 0a20 2020 2020 2020 2020 2020 2020 5b27  .             ['
-0001c170: 616e 272c 2027 616e 7469 7175 6527 2c20  an', 'antique', 
-0001c180: 2769 7327 2c20 2774 6869 7327 2c20 2774  'is', 'this', 't
-0001c190: 686f 7573 616e 6427 2c20 2774 686f 7573  housand', 'thous
-0001c1a0: 616e 6473 272c 2027 7661 7365 272c 2027  ands', 'vase', '
-0001c1b0: 776f 7274 6827 5d29 2c0a 2020 2020 2020  worth']),.      
-0001c1c0: 2020 2020 2020 2827 5768 656e 2077 6520        ('When we 
-0001c1d0: 6d65 6574 2c20 796f 7520 6172 6520 6120  meet, you are a 
-0001c1e0: 6769 616e 7420 616d 6f6e 6720 6d65 6e2e  giant among men.
-0001c1f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0001c200: 5b27 6127 2c20 2761 6d6f 6e67 272c 2027  ['a', 'among', '
-0001c210: 6172 6527 2c20 2767 6961 6e74 272c 2027  are', 'giant', '
-0001c220: 6d61 6e27 2c20 276d 6565 7427 2c20 276d  man', 'meet', 'm
-0001c230: 656e 272c 2027 7765 272c 2027 7768 656e  en', 'we', 'when
-0001c240: 272c 2027 796f 7527 5d29 2c0a 2020 2020  ', 'you']),.    
-0001c250: 2020 2020 2020 2020 2827 5768 656e 2077          ('When w
-0001c260: 6520 6172 6520 616d 6f6e 6720 6d65 6e2c  e are among men,
-0001c270: 2079 6f75 2061 7265 2061 2067 6961 6e74   you are a giant
-0001c280: 206d 6561 7462 616c 6c2e 272c 0a20 2020   meatball.',.   
-0001c290: 2020 2020 2020 2020 2020 5b27 6127 2c20            ['a', 
-0001c2a0: 2761 6d6f 6e67 272c 2027 6172 6527 2c20  'among', 'are', 
-0001c2b0: 2761 7265 272c 2027 6769 616e 7427 2c20  'are', 'giant', 
-0001c2c0: 276d 616e 272c 2027 6d65 6174 6261 6c6c  'man', 'meatball
-0001c2d0: 272c 2027 6d65 6e27 2c20 2777 6527 2c20  ', 'men', 'we', 
-0001c2e0: 2777 6865 6e27 2c20 2779 6f75 275d 292c  'when', 'you']),
-0001c2f0: 0a20 2020 2020 2020 205d 3a0a 2020 2020  .        ]:.    
-0001c300: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0001c310: 662e 7375 6254 6573 7428 6c69 6e65 293a  f.subTest(line):
-0001c320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c330: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001c340: 6c28 6578 7065 6374 6564 2c20 736f 7274  l(expected, sort
-0001c350: 6564 286c 742e 5461 626c 652e 5f6e 6f72  ed(lt.Table._nor
-0001c360: 6d61 6c69 7a65 5f73 706c 6974 286c 696e  malize_split(lin
-0001c370: 6529 2929 0a0a 0a69 6620 5f5f 6e61 6d65  e)))...if __name
-0001c380: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
-0001c390: 3a0a 2020 2020 756e 6974 7465 7374 2e6d  :.    unittest.m
-0001c3a0: 6169 6e28 290a                           ain().
+000130b0: 2020 2073 656c 662e 7766 696c 652e 7772     self.wfile.wr
+000130c0: 6974 6528 7365 6e64 5f62 7974 6573 290a  ite(send_bytes).
+000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130e0: 2020 2020 7468 7265 6164 696e 672e 5468      threading.Th
+000130f0: 7265 6164 2874 6172 6765 743d 6c61 6d62  read(target=lamb
+00013100: 6461 3a20 7469 6d65 2e73 6c65 6570 2831  da: time.sleep(1
+00013110: 2920 6f72 2073 656c 662e 7365 7276 6572  ) or self.server
+00013120: 2e73 6875 7464 6f77 6e28 2929 2e73 7461  .shutdown()).sta
+00013130: 7274 2829 0a0a 2020 2020 2020 2020 2020  rt()..          
+00013140: 2020 2020 2020 656c 6966 2070 6174 6820        elif path 
+00013150: 3d3d 2022 2f22 3a0a 2020 2020 2020 2020  == "/":.        
+00013160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013170: 2e73 656e 645f 7265 7370 6f6e 7365 2848  .send_response(H
+00013180: 5454 5053 7461 7475 732e 4f4b 290a 2020  TTPStatus.OK).  
+00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131a0: 2020 7365 6c66 2e65 6e64 5f68 6561 6465    self.end_heade
+000131b0: 7273 2829 0a20 2020 2020 2020 2020 2020  rs().           
+000131c0: 2020 2020 2020 2020 2073 656c 662e 7766           self.wf
+000131d0: 696c 652e 7772 6974 6528 7365 6e64 5f62  ile.write(send_b
+000131e0: 7974 6573 290a 0a20 2020 2020 2020 2020  ytes)..         
+000131f0: 2020 2020 2020 2065 6c69 6620 7061 7468         elif path
+00013200: 2e73 7461 7274 7377 6974 6828 222f 6162  .startswith("/ab
+00013210: 632e 6373 7622 293a 0a20 2020 2020 2020  c.csv"):.       
+00013220: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00013230: 645f 6279 7465 7320 2b3d 2062 2261 2c62  d_bytes += b"a,b
+00013240: 2c63 5c6e 312c 322c 335c 6e22 0a20 2020  ,c\n1,2,3\n".   
+00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013260: 2073 656c 662e 7365 6e64 5f72 6573 706f   self.send_respo
+00013270: 6e73 6528 4854 5450 5374 6174 7573 2e4f  nse(HTTPStatus.O
+00013280: 4b29 0a20 2020 2020 2020 2020 2020 2020  K).             
+00013290: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+000132a0: 5f68 6561 6465 7228 2243 6f6e 7465 6e74  _header("Content
+000132b0: 2d4c 656e 6774 6822 2c20 7374 7228 6c65  -Length", str(le
+000132c0: 6e28 7365 6e64 5f62 7974 6573 2929 290a  n(send_bytes))).
+000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132e0: 2020 2020 7365 6c66 2e65 6e64 5f68 6561      self.end_hea
+000132f0: 6465 7273 2829 0a20 2020 2020 2020 2020  ders().         
+00013300: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013310: 7766 696c 652e 7772 6974 6528 7365 6e64  wfile.write(send
+00013320: 5f62 7974 6573 290a 0a20 2020 2020 2020  _bytes)..       
+00013330: 2020 2020 2064 6566 2064 6f5f 504f 5354       def do_POST
+00013340: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013350: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00013360: 5f6d 6573 7361 6765 2866 2272 6563 6569  _message(f"recei
+00013370: 7665 6420 7b73 656c 662e 636f 6d6d 616e  ved {self.comman
+00013380: 647d 207b 7365 6c66 2e70 6174 687d 2229  d} {self.path}")
+00013390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000133a0: 2070 6174 6820 3d20 7365 6c66 2e70 6174   path = self.pat
+000133b0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+000133c0: 2020 6164 6465 645f 7661 6c75 6520 3d20    added_value = 
+000133d0: 7365 6c66 2e68 6561 6465 7273 5b22 5661  self.headers["Va
+000133e0: 6c75 6522 5d0a 2020 2020 2020 2020 2020  lue"].          
+000133f0: 2020 2020 2020 7365 6c66 2e6c 6f67 5f6d        self.log_m
+00013400: 6573 7361 6765 2866 2272 6563 6569 7665  essage(f"receive
+00013410: 6420 6865 6164 6572 2027 5661 6c75 6527  d header 'Value'
+00013420: 207b 6164 6465 645f 7661 6c75 6521 727d   {added_value!r}
+00013430: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00013440: 2020 2073 656c 662e 6c6f 675f 6d65 7373     self.log_mess
+00013450: 6167 6528 2261 626f 7574 2074 6f20 7265  age("about to re
+00013460: 6164 2066 726f 6d20 7266 696c 6522 290a  ad from rfile").
+00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013480: 6164 6465 645f 636f 6c75 6d6e 203d 2073  added_column = s
+00013490: 656c 662e 7266 696c 652e 7265 6164 2869  elf.rfile.read(i
+000134a0: 6e74 2873 656c 662e 6865 6164 6572 732e  nt(self.headers.
+000134b0: 6765 7428 2743 6f6e 7465 6e74 2d4c 656e  get('Content-Len
+000134c0: 6774 6827 2c20 2731 2729 2929 0a20 2020  gth', '1'))).   
+000134d0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+000134e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000134f0: 2020 2020 2020 6164 6465 645f 636f 6c75        added_colu
+00013500: 6d6e 5f73 7472 203d 2061 6464 6564 5f63  mn_str = added_c
+00013510: 6f6c 756d 6e2e 6465 636f 6465 2829 0a20  olumn.decode(). 
+00013520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00013530: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00013540: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00013550: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00013560: 6f67 5f6d 6573 7361 6765 2866 2245 7272  og_message(f"Err
+00013570: 6f72 2064 6563 6f64 696e 6720 6164 6465  or decoding adde
+00013580: 6420 636f 6c75 6d6e 3a20 7b74 7970 6528  d column: {type(
+00013590: 6529 2e5f 5f6e 616d 655f 5f7d 3a20 7b65  e).__name__}: {e
+000135a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000135b0: 2020 2020 2020 2020 6164 6465 645f 636f          added_co
+000135c0: 6c75 6d6e 5f73 7472 203d 2022 6572 726f  lumn_str = "erro
+000135d0: 7222 0a20 2020 2020 2020 2020 2020 2020  r".             
+000135e0: 2020 2073 656c 662e 6c6f 675f 6d65 7373     self.log_mess
+000135f0: 6167 6528 2272 6561 6420 6672 6f6d 2072  age("read from r
+00013600: 6669 6c65 2063 6f6d 706c 6574 6522 290a  file complete").
+00013610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013620: 7365 6c66 2e6c 6f67 5f6d 6573 7361 6765  self.log_message
+00013630: 2866 2272 6563 6569 7665 6420 626f 6479  (f"received body
+00013640: 207b 6164 6465 645f 636f 6c75 6d6e 2172   {added_column!r
+00013650: 7d22 290a 0a20 2020 2020 2020 2020 2020  }")..           
+00013660: 2020 2020 2073 656e 645f 6279 7465 7320       send_bytes 
+00013670: 3d20 6222 220a 2020 2020 2020 2020 2020  = b"".          
+00013680: 2020 2020 2020 6966 2070 6174 682e 7374        if path.st
+00013690: 6172 7473 7769 7468 2822 2f61 6263 2e63  artswith("/abc.c
+000136a0: 7376 2229 3a0a 2020 2020 2020 2020 2020  sv"):.          
+000136b0: 2020 2020 2020 2020 2020 7365 6e64 5f62            send_b
+000136c0: 7974 6573 202b 3d20 6622 612c 622c 632c  ytes += f"a,b,c,
+000136d0: 7b61 6464 6564 5f63 6f6c 756d 6e5f 7374  {added_column_st
+000136e0: 727d 5c6e 312c 322c 332c 7b61 6464 6564  r}\n1,2,3,{added
+000136f0: 5f76 616c 7565 7d5c 6e22 2e65 6e63 6f64  _value}\n".encod
+00013700: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
+00013710: 2020 2020 2073 656c 662e 7365 6e64 5f72       self.send_r
+00013720: 6573 706f 6e73 6528 4854 5450 5374 6174  esponse(HTTPStat
+00013730: 7573 2e4f 4b29 0a20 2020 2020 2020 2020  us.OK).         
+00013740: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+00013750: 5f68 6561 6465 7228 2243 6f6e 7465 6e74  _header("Content
+00013760: 2d4c 656e 6774 6822 2c20 7374 7228 6c65  -Length", str(le
+00013770: 6e28 7365 6e64 5f62 7974 6573 2929 290a  n(send_bytes))).
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 7365 6c66 2e65 6e64 5f68 6561 6465 7273  self.end_headers
+000137a0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000137b0: 2020 2073 656c 662e 7766 696c 652e 7772     self.wfile.wr
+000137c0: 6974 6528 7365 6e64 5f62 7974 6573 290a  ite(send_bytes).
+000137d0: 0a20 2020 2020 2020 2064 6566 2072 756e  .        def run
+000137e0: 2873 6572 7665 725f 636c 6173 733d 4854  (server_class=HT
+000137f0: 5450 5365 7276 6572 2c20 6861 6e64 6c65  TPServer, handle
+00013800: 725f 636c 6173 733d 4353 5654 6573 7452  r_class=CSVTestR
+00013810: 6571 7565 7374 4861 6e64 6c65 7229 3a0a  equestHandler):.
+00013820: 2020 2020 2020 2020 2020 2020 7365 7276              serv
+00013830: 6572 5f61 6464 7265 7373 203d 2028 2727  er_address = (''
+00013840: 2c20 3838 3838 290a 2020 2020 2020 2020  , 8888).        
+00013850: 2020 2020 6874 7470 6420 3d20 7365 7276      httpd = serv
+00013860: 6572 5f63 6c61 7373 2873 6572 7665 725f  er_class(server_
+00013870: 6164 6472 6573 732c 2068 616e 646c 6572  address, handler
+00013880: 5f63 6c61 7373 290a 2020 2020 2020 2020  _class).        
+00013890: 2020 2020 6874 7470 642e 7365 7276 655f      httpd.serve_
+000138a0: 666f 7265 7665 7228 290a 0a20 2020 2020  forever()..     
+000138b0: 2020 2064 6566 2072 756e 5f62 6163 6b67     def run_backg
+000138c0: 726f 756e 645f 7465 7374 5f73 6572 7665  round_test_serve
+000138d0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+000138e0: 2070 203d 2074 6872 6561 6469 6e67 2e54   p = threading.T
+000138f0: 6872 6561 6428 7461 7267 6574 3d72 756e  hread(target=run
+00013900: 290a 2020 2020 2020 2020 2020 2020 702e  ).            p.
+00013910: 7374 6172 7428 290a 0a20 2020 2020 2020  start()..       
+00013920: 2020 2020 2066 6f72 2074 7269 6573 5f72       for tries_r
+00013930: 656d 6169 6e69 6e67 2069 6e20 7265 7665  emaining in reve
+00013940: 7273 6564 2872 616e 6765 2832 3029 293a  rsed(range(20)):
+00013950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013960: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00013970: 2020 2020 2020 2020 2020 7769 7468 2075            with u
+00013980: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
+00013990: 6c6f 7065 6e28 2268 7474 703a 2f2f 6c6f  lopen("http://lo
+000139a0: 6361 6c68 6f73 743a 3838 3838 2f22 293a  calhost:8888/"):
+000139b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000139c0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000139e0: 7863 6570 7420 7572 6c6c 6962 2e65 7272  xcept urllib.err
+000139f0: 6f72 2e55 524c 4572 726f 723a 0a20 2020  or.URLError:.   
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a10: 2069 6620 7472 6965 735f 7265 6d61 696e   if tries_remain
+00013a20: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00013a30: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+00013a40: 652e 736c 6565 7028 302e 3235 290a 0a20  e.sleep(0.25).. 
+00013a50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00013a60: 6e20 700a 0a20 2020 2020 2020 2077 6562  n p..        web
+00013a70: 5f61 6464 7265 7373 203d 2022 6874 7470  _address = "http
+00013a80: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3838  ://localhost:888
+00013a90: 3822 0a20 2020 2020 2020 2070 203d 2072  8".        p = r
+00013aa0: 756e 5f62 6163 6b67 726f 756e 645f 7465  un_background_te
+00013ab0: 7374 5f73 6572 7665 7228 290a 0a20 2020  st_server()..   
+00013ac0: 2020 2020 2075 726c 203d 2077 6562 5f61       url = web_a
+00013ad0: 6464 7265 7373 202b 2022 2f61 6263 2e63  ddress + "/abc.c
+00013ae0: 7376 220a 2020 2020 2020 2020 7472 793a  sv".        try:
+00013af0: 0a20 2020 2020 2020 2020 2020 2074 626c  .            tbl
+00013b00: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+00013b10: 765f 696d 706f 7274 2875 726c 290a 2020  v_import(url).  
+00013b20: 2020 2020 2020 2020 2020 7462 6c32 203d            tbl2 =
+00013b30: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00013b40: 696d 706f 7274 280a 2020 2020 2020 2020  import(.        
+00013b50: 2020 2020 2020 2020 7572 6c2c 0a20 2020          url,.   
+00013b60: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00013b70: 613d 6222 6578 7472 6122 2c0a 2020 2020  a=b"extra",.    
+00013b80: 2020 2020 2020 2020 2020 2020 6865 6164              head
+00013b90: 6572 733d 7b22 5641 4c55 4522 3a20 2231  ers={"VALUE": "1
+00013ba0: 3030 227d 2c0a 2020 2020 2020 2020 2020  00"},.          
+00013bb0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+00013bc0: 3d7b 7d2e 6672 6f6d 6b65 7973 2822 6120  ={}.fromkeys("a 
+00013bd0: 6220 6320 6578 7472 6122 2e73 706c 6974  b c extra".split
+00013be0: 2829 2c20 696e 7429 2c0a 2020 2020 2020  (), int),.      
+00013bf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00013c00: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+00013c10: 2020 2020 2077 6974 6820 7572 6c6c 6962       with urllib
+00013c20: 2e72 6571 7565 7374 2e75 726c 6f70 656e  .request.urlopen
+00013c30: 2877 6562 5f61 6464 7265 7373 202b 2022  (web_address + "
+00013c40: 2f45 5849 5422 293a 0a20 2020 2020 2020  /EXIT"):.       
+00013c50: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00013c60: 2020 2020 2020 2020 2020 702e 6a6f 696e            p.join
+00013c70: 2829 0a0a 2020 2020 2020 2020 7462 6c2e  ()..        tbl.
+00013c80: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+00013c90: 2020 7462 6c32 2e70 7265 7365 6e74 2829    tbl2.present()
+00013ca0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00013cb0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00013cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013cd0: 6173 7365 7274 4571 7561 6c28 7572 6c2c  assertEqual(url,
+00013ce0: 2074 626c 2e69 6d70 6f72 745f 736f 7572   tbl.import_sour
+00013cf0: 6365 290a 2020 2020 2020 2020 7769 7468  ce).        with
+00013d00: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00013d10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013d20: 662e 6173 7365 7274 4571 7561 6c28 6c74  f.assertEqual(lt
+00013d30: 2e49 6d70 6f72 7453 6f75 7263 6554 7970  .ImportSourceTyp
+00013d40: 652e 7572 6c2c 2074 626c 2e69 6d70 6f72  e.url, tbl.impor
+00013d50: 745f 736f 7572 6365 5f74 7970 6529 0a0a  t_source_type)..
+00013d60: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00013d70: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00013d80: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013d90: 7365 7274 4571 7561 6c28 2261 2062 2063  sertEqual("a b c
+00013da0: 2065 7874 7261 222e 7370 6c69 7428 292c   extra".split(),
+00013db0: 2074 626c 322e 696e 666f 2829 5b22 6669   tbl2.info()["fi
+00013dc0: 656c 6473 225d 290a 2020 2020 2020 2020  elds"]).        
+00013dd0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00013de0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00013df0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00013e00: 6c28 3130 302c 2074 626c 325b 305d 2e65  l(100, tbl2[0].e
+00013e10: 7874 7261 290a 0a20 2020 2064 6566 2074  xtra)..    def t
+00013e20: 6573 745f 6373 765f 6669 6c74 6572 6564  est_csv_filtered
+00013e30: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+00013e40: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00013e50: 203d 2033 0a20 2020 2020 2020 2074 7420   = 3.        tt 
+00013e60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00013e70: 5f69 6d70 6f72 7428 2274 6573 742f 6162  _import("test/ab
+00013e80: 632e 6373 7622 2c20 7472 616e 7366 6f72  c.csv", transfor
+00013e90: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
+00013ea0: 2822 6162 6322 2c20 696e 7429 290a 2020  ("abc", int)).  
+00013eb0: 2020 2020 2020 7072 696e 7428 2261 6263        print("abc
+00013ec0: 2e63 7376 222c 2074 742e 696e 666f 2829  .csv", tt.info()
+00013ed0: 290a 0a20 2020 2020 2020 2074 7420 3d20  )..        tt = 
+00013ee0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00013ef0: 6d70 6f72 7428 2274 6573 742f 6162 632e  mport("test/abc.
+00013f00: 6373 7622 2c20 7472 616e 7366 6f72 6d73  csv", transforms
+00013f10: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00013f20: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
+00013f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013f50: 696c 7465 7273 3d7b 2263 223a 206c 742e  ilters={"c": lt.
+00013f60: 5461 626c 652e 6571 2831 297d 290a 2020  Table.eq(1)}).  
+00013f70: 2020 2020 2020 7072 696e 7428 7474 2e69        print(tt.i
+00013f80: 6e66 6f28 2929 0a20 2020 2020 2020 2077  nfo()).        w
+00013f90: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00013fa0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00013fb0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013fc0: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+00013fd0: 745f 7369 7a65 2c20 6c65 6e28 7474 2929  t_size, len(tt))
+00013fe0: 0a0a 2020 2020 2020 2020 7474 203d 206c  ..        tt = l
+00013ff0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00014000: 706f 7274 2822 7465 7374 2f61 6263 2e63  port("test/abc.c
+00014010: 7376 222c 2074 7261 6e73 666f 726d 733d  sv", transforms=
+00014020: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00014030: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00014060: 6c74 6572 733d 7b22 6322 3a20 317d 290a  lters={"c": 1}).
+00014070: 2020 2020 2020 2020 7072 696e 7428 7474          print(tt
+00014080: 2e69 6e66 6f28 2929 0a20 2020 2020 2020  .info()).       
+00014090: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000140a0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+000140b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000140c0: 616c 2874 6573 745f 7369 7a65 202a 2074  al(test_size * t
+000140d0: 6573 745f 7369 7a65 2c20 6c65 6e28 7474  est_size, len(tt
+000140e0: 2929 0a0a 2020 2020 2020 2020 7474 203d  ))..        tt =
+000140f0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00014100: 696d 706f 7274 2822 7465 7374 2f61 6263  import("test/abc
+00014110: 2e63 7376 222c 2074 7261 6e73 666f 726d  .csv", transform
+00014120: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00014130: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 6669 6c74 6572 733d 7b22 6322 3a20 6c61  filters={"c": la
+00014170: 6d62 6461 2078 3a20 3020 3c20 7820 3c20  mbda x: 0 < x < 
+00014180: 327d 290a 2020 2020 2020 2020 7072 696e  2}).        prin
+00014190: 7428 7474 2e69 6e66 6f28 2929 0a20 2020  t(tt.info()).   
+000141a0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000141b0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+000141c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000141d0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+000141e0: 202a 2074 6573 745f 7369 7a65 2c20 6c65   * test_size, le
+000141f0: 6e28 7474 2929 0a0a 2020 2020 2020 2020  n(tt))..        
+00014200: 2320 7465 7374 2061 6c6c 2073 7065 6369  # test all speci
+00014210: 616c 2063 6f6d 7061 7261 746f 7273 2077  al comparators w
+00014220: 6865 6e20 7573 6564 2061 7320 6669 6c74  hen used as filt
+00014230: 6572 730a 2020 2020 2020 2020 2320 2020  ers.        #   
+00014240: 2020 6973 5f6e 6f6e 6520 2d20 6174 7472    is_none - attr
+00014250: 6962 7574 6520 7661 6c75 6520 6973 204e  ibute value is N
+00014260: 6f6e 650a 2020 2020 2020 2020 2320 2020  one.        #   
+00014270: 2020 6973 5f6e 6f74 5f6e 6f6e 6520 2d20    is_not_none - 
+00014280: 6174 7472 6962 7574 6520 7661 6c75 6520  attribute value 
+00014290: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+000142a0: 2020 2020 2320 2020 2020 6973 5f6e 756c      #     is_nul
+000142b0: 6c20 2d20 6174 7472 6962 7574 6520 7661  l - attribute va
+000142c0: 6c75 6520 6973 204e 6f6e 652c 2022 222c  lue is None, "",
+000142d0: 206f 7220 6e6f 7420 6465 6669 6e65 640a   or not defined.
+000142e0: 2020 2020 2020 2020 2320 2020 2020 6973          #     is
+000142f0: 5f6e 6f74 5f6e 756c 6c20 2d20 6174 7472  _not_null - attr
+00014300: 6962 7574 6520 7661 6c75 6520 6973 2064  ibute value is d
+00014310: 6566 696e 6564 2c20 616e 6420 6973 206e  efined, and is n
+00014320: 6f74 204e 6f6e 6520 6f72 2022 220a 2020  ot None or "".  
+00014330: 2020 2020 2020 2320 2020 2020 7374 6172        #     star
+00014340: 7473 7769 7468 202d 2061 7474 7269 6275  tswith - attribu
+00014350: 7465 2076 616c 7565 2073 7461 7274 7320  te value starts 
+00014360: 7769 7468 2061 2067 6976 656e 2073 7472  with a given str
+00014370: 696e 670a 2020 2020 2020 2020 2320 2020  ing.        #   
+00014380: 2020 656e 6473 7769 7468 202d 2061 7474    endswith - att
+00014390: 7269 6275 7465 2076 616c 7565 2065 6e64  ribute value end
+000143a0: 7320 7769 7468 2061 2067 6976 656e 2073  s with a given s
+000143b0: 7472 696e 670a 2020 2020 2020 2020 2320  tring.        # 
+000143c0: 2020 2020 7265 5f6d 6174 6368 202d 2061      re_match - a
+000143d0: 7474 7269 6275 7465 2076 616c 7565 206d  ttribute value m
+000143e0: 6174 6368 6573 2061 2072 6567 756c 6172  atches a regular
+000143f0: 2065 7870 7265 7373 696f 6e0a 0a20 2020   expression..   
+00014400: 2020 2020 2070 7269 6e74 2829 0a20 2020       print().   
+00014410: 2020 2020 2069 6e70 7574 5f64 6174 6120       input_data 
+00014420: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
+00014430: 7428 2222 225c 0a20 2020 2020 2020 206e  t("""\.        n
+00014440: 616d 652c 612c 622c 630a 2020 2020 2020  ame,a,b,c.      
+00014450: 2020 2241 222c 3130 302c 3130 302c 3130    "A",100,100,10
+00014460: 300a 2020 2020 2020 2020 2242 222c 3230  0.        "B",20
+00014470: 302c 2c32 3030 0a20 2020 2020 2020 2022  0,,200.        "
+00014480: 4131 222c 3130 312c 3130 312c 3130 310a  A1",101,101,101.
+00014490: 2020 2020 2020 2020 2242 3122 2c32 3031          "B1",201
+000144a0: 2c2c 3230 310a 2020 2020 2020 2020 2243  ,,201.        "C
+000144b0: 3122 2c33 3031 2c2c 3330 310a 2020 2020  1",301,,301.    
+000144c0: 2020 2020 2c39 392c 3939 2c39 390a 2020      ,99,99,99.  
+000144d0: 2020 2020 2020 2222 2229 0a20 2020 2020        """).     
+000144e0: 2020 206c 742e 5461 626c 6528 292e 6373     lt.Table().cs
+000144f0: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
+00014500: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00014510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014520: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
+00014530: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+00014540: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014560: 2020 2020 2020 2029 2e70 7265 7365 6e74         ).present
+00014570: 2829 0a0a 2020 2020 2020 2020 2222 220a  ()..        """.
+00014580: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+00014590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000145a0: 2d2d 2b0a 2020 2020 2020 2020 7c20 4e61  --+.        | Na
+000145b0: 6d65 207c 2020 2041 207c 2020 2020 4220  me |   A |    B 
+000145c0: 7c20 2020 4320 7c0a 2020 2020 2020 2020  |   C |.        
+000145d0: 7c2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d  |------+-----+--
+000145e0: 2d2d 2d2d 2b2d 2d2d 2d2d 7c0a 2020 2020  ----+-----|.    
+000145f0: 2020 2020 7c20 4120 2020 207c 2031 3030      | A    | 100
+00014600: 207c 2020 3130 3020 7c20 3130 3020 7c0a   |  100 | 100 |.
+00014610: 2020 2020 2020 2020 7c20 4220 2020 207c          | B    |
+00014620: 2032 3030 207c 204e 6f6e 6520 7c20 3230   200 | None | 20
+00014630: 3020 7c0a 2020 2020 2020 2020 7c20 4131  0 |.        | A1
+00014640: 2020 207c 2031 3031 207c 2020 3130 3120     | 101 |  101 
+00014650: 7c20 3130 3120 7c0a 2020 2020 2020 2020  | 101 |.        
+00014660: 7c20 4231 2020 207c 2032 3031 207c 204e  | B1   | 201 | N
+00014670: 6f6e 6520 7c20 3230 3120 7c0a 2020 2020  one | 201 |.    
+00014680: 2020 2020 7c20 4331 2020 207c 2033 3031      | C1   | 301
+00014690: 207c 204e 6f6e 6520 7c20 3330 3120 7c0a   | None | 301 |.
+000146a0: 2020 2020 2020 2020 7c20 2020 2020 207c          |      |
+000146b0: 2020 3939 207c 2020 2039 3920 7c20 2039    99 |   99 |  9
+000146c0: 3920 7c0a 2020 2020 2020 2020 2b2d 2d2d  9 |.        +---
+000146d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000146e0: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+000146f0: 2222 220a 0a20 2020 2020 2020 2070 7269  """..        pri
+00014700: 6e74 2822 6973 5f6e 6f6e 6528 2922 290a  nt("is_none()").
+00014710: 2020 2020 2020 2020 7820 3d20 6c74 2e54          x = lt.T
+00014720: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
+00014730: 7428 696e 7075 745f 6461 7461 2c0a 2020  t(input_data,.  
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014760: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00014770: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00014780: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147b0: 2020 2020 2020 6669 6c74 6572 733d 7b22        filters={"
+000147c0: 6222 3a20 6c74 2e54 6162 6c65 2e69 735f  b": lt.Table.is_
+000147d0: 6e6f 6e65 2829 7d29 0a20 2020 2020 2020  none()}).       
+000147e0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000147f0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00014800: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00014810: 616c 2833 2c20 6c65 6e28 7829 290a 2020  al(3, len(x)).  
+00014820: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00014830: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00014840: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014850: 7274 5472 7565 2861 6c6c 2862 2069 7320  rtTrue(all(b is 
+00014860: 4e6f 6e65 2066 6f72 2062 2069 6e20 782e  None for b in x.
+00014870: 616c 6c2e 6229 290a 0a20 2020 2020 2020  all.b))..       
+00014880: 2070 7269 6e74 2822 6973 5f6e 6f74 5f6e   print("is_not_n
+00014890: 6f6e 6528 2922 290a 2020 2020 2020 2020  one()").        
+000148a0: 7820 3d20 6c74 2e54 6162 6c65 2829 2e63  x = lt.Table().c
+000148b0: 7376 5f69 6d70 6f72 7428 696e 7075 745f  sv_import(input_
+000148c0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148e0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+000148f0: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
+00014900: 2822 6162 6322 2c20 696e 7429 2c0a 2020  ("abc", int),.  
+00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014930: 6669 6c74 6572 733d 7b22 6222 3a20 6c74  filters={"b": lt
+00014940: 2e54 6162 6c65 2e69 735f 6e6f 745f 6e6f  .Table.is_not_no
+00014950: 6e65 2829 7d29 0a20 2020 2020 2020 2077  ne()}).        w
+00014960: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014970: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014980: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014990: 2833 2c20 6c65 6e28 7829 290a 2020 2020  (3, len(x)).    
+000149a0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+000149b0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+000149c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000149d0: 4571 7561 6c28 3330 302c 2073 756d 2878  Equal(300, sum(x
+000149e0: 2e61 6c6c 2e62 2929 0a0a 2020 2020 2020  .all.b))..      
+000149f0: 2020 7072 696e 7428 2262 2069 735f 6e75    print("b is_nu
+00014a00: 6c6c 2829 2229 0a20 2020 2020 2020 2078  ll()").        x
+00014a10: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+00014a20: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
+00014a30: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a50: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00014a60: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00014a70: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014aa0: 696c 7465 7273 3d7b 2262 223a 206c 742e  ilters={"b": lt.
+00014ab0: 5461 626c 652e 6973 5f6e 756c 6c28 297d  Table.is_null()}
+00014ac0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00014ad0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00014ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014af0: 6173 7365 7274 4571 7561 6c28 332c 206c  assertEqual(3, l
+00014b00: 656e 2878 2929 0a20 2020 2020 2020 2077  en(x)).        w
+00014b10: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014b20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014b30: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00014b40: 616c 6c28 6220 6973 204e 6f6e 6520 666f  all(b is None fo
+00014b50: 7220 6220 696e 2078 2e61 6c6c 2e62 2929  r b in x.all.b))
+00014b60: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00014b70: 2262 2069 735f 6e6f 745f 6e75 6c6c 2829  "b is_not_null()
+00014b80: 2229 0a20 2020 2020 2020 2078 203d 206c  ").        x = l
+00014b90: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00014ba0: 706f 7274 2869 6e70 7574 5f64 6174 612c  port(input_data,
+00014bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bd0: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
+00014be0: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+00014bf0: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c10: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00014c20: 7273 3d7b 2262 223a 206c 742e 5461 626c  rs={"b": lt.Tabl
+00014c30: 652e 6973 5f6e 6f74 5f6e 756c 6c28 297d  e.is_not_null()}
+00014c40: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00014c50: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00014c60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014c70: 6173 7365 7274 4571 7561 6c28 332c 206c  assertEqual(3, l
+00014c80: 656e 2878 2929 0a20 2020 2020 2020 2077  en(x)).        w
+00014c90: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014ca0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014cb0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014cc0: 2833 3030 2c20 7375 6d28 782e 616c 6c2e  (300, sum(x.all.
+00014cd0: 6229 290a 0a20 2020 2020 2020 2070 7269  b))..        pri
+00014ce0: 6e74 2822 6e61 6d65 2069 735f 6e75 6c6c  nt("name is_null
+00014cf0: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
+00014d00: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00014d10: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+00014d20: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d40: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00014d50: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00014d60: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d80: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00014d90: 7465 7273 3d7b 226e 616d 6522 3a20 6c74  ters={"name": lt
+00014da0: 2e54 6162 6c65 2e69 735f 6e75 6c6c 2829  .Table.is_null()
+00014db0: 7d29 0a20 2020 2020 2020 2077 6974 6820  }).        with 
+00014dc0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00014dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014de0: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
+00014df0: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
+00014e00: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00014e10: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00014e20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00014e30: 6c28 332a 3939 2c20 785b 305d 2e61 202b  l(3*99, x[0].a +
+00014e40: 2078 5b30 5d2e 6220 2b20 785b 305d 2e63   x[0].b + x[0].c
+00014e50: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00014e60: 2822 6e61 6d65 2069 735f 6e6f 745f 6e75  ("name is_not_nu
+00014e70: 6c6c 2829 2229 0a20 2020 2020 2020 2078  ll()").        x
+00014e80: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+00014e90: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
+00014ea0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ec0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00014ed0: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00014ee0: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014f10: 696c 7465 7273 3d7b 226e 616d 6522 3a20  ilters={"name": 
+00014f20: 6c74 2e54 6162 6c65 2e69 735f 6e6f 745f  lt.Table.is_not_
+00014f30: 6e75 6c6c 2829 7d29 0a20 2020 2020 2020  null()}).       
+00014f40: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00014f50: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00014f60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00014f70: 616c 2835 2c20 6c65 6e28 7829 290a 2020  al(5, len(x)).  
+00014f80: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00014f90: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00014fa0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014fb0: 7274 4571 7561 6c28 2241 2042 2041 3120  rtEqual("A B A1 
+00014fc0: 4231 2043 3122 2e73 706c 6974 2829 2c20  B1 C1".split(), 
+00014fd0: 6c69 7374 2878 2e61 6c6c 2e6e 616d 6529  list(x.all.name)
+00014fe0: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00014ff0: 2822 6e61 6d65 2073 7461 7274 7377 6974  ("name startswit
+00015000: 6828 2742 2729 2229 0a20 2020 2020 2020  h('B')").       
+00015010: 2078 203d 206c 742e 5461 626c 6528 292e   x = lt.Table().
+00015020: 6373 765f 696d 706f 7274 2869 6e70 7574  csv_import(input
+00015030: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
+00015060: 726d 733d 6469 6374 2e66 726f 6d6b 6579  rms=dict.fromkey
+00015070: 7328 2261 6263 222c 2069 6e74 292c 0a20  s("abc", int),. 
+00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150a0: 2066 696c 7465 7273 3d7b 226e 616d 6522   filters={"name"
+000150b0: 3a20 6c74 2e54 6162 6c65 2e73 7461 7274  : lt.Table.start
+000150c0: 7377 6974 6828 2242 2229 7d29 0a20 2020  swith("B")}).   
+000150d0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000150e0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+000150f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00015100: 7445 7175 616c 2832 2c20 6c65 6e28 7829  tEqual(2, len(x)
+00015110: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00015120: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00015130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015140: 6173 7365 7274 4571 7561 6c28 2242 2042  assertEqual("B B
+00015150: 3122 2e73 706c 6974 2829 2c20 6c69 7374  1".split(), list
+00015160: 2878 2e61 6c6c 2e6e 616d 6529 290a 0a20  (x.all.name)).. 
+00015170: 2020 2020 2020 2070 7269 6e74 2822 6e61         print("na
+00015180: 6d65 2065 6e64 7377 6974 6828 2731 2729  me endswith('1')
+00015190: 2229 0a20 2020 2020 2020 2078 203d 206c  ").        x = l
+000151a0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+000151b0: 706f 7274 2869 6e70 7574 5f64 6174 612c  port(input_data,
+000151c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
+000151f0: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+00015200: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015220: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00015230: 7273 3d7b 226e 616d 6522 3a20 6c74 2e54  rs={"name": lt.T
+00015240: 6162 6c65 2e65 6e64 7377 6974 6828 2231  able.endswith("1
+00015250: 2229 7d29 0a20 2020 2020 2020 2077 6974  ")}).        wit
+00015260: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00015270: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015280: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00015290: 2c20 6c65 6e28 7829 290a 2020 2020 2020  , len(x)).      
+000152a0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+000152b0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+000152c0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000152d0: 7561 6c28 2241 3120 4231 2043 3122 2e73  ual("A1 B1 C1".s
+000152e0: 706c 6974 2829 2c20 6c69 7374 2878 2e61  plit(), list(x.a
+000152f0: 6c6c 2e6e 616d 6529 290a 0a20 2020 2020  ll.name))..     
+00015300: 2020 2070 7269 6e74 2872 226e 616d 6520     print(r"name 
+00015310: 7265 5f6d 6174 6368 2872 275b 4142 5d5c  re_match(r'[AB]\
+00015320: 6427 2922 290a 2020 2020 2020 2020 7820  d')").        x 
+00015330: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00015340: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
+00015350: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015370: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+00015380: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00015390: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
+000153a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153b0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000153c0: 6c74 6572 733d 7b22 6e61 6d65 223a 206c  lters={"name": l
+000153d0: 742e 5461 626c 652e 7265 5f6d 6174 6368  t.Table.re_match
+000153e0: 2872 225b 4142 5d5c 6422 297d 290a 2020  (r"[AB]\d")}).  
+000153f0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00015400: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00015410: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00015420: 7274 4571 7561 6c28 322c 206c 656e 2878  rtEqual(2, len(x
+00015430: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00015440: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00015450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015460: 2e61 7373 6572 7445 7175 616c 2822 4131  .assertEqual("A1
+00015470: 2042 3122 2e73 706c 6974 2829 2c20 6c69   B1".split(), li
+00015480: 7374 2878 2e61 6c6c 2e6e 616d 6529 290a  st(x.all.name)).
+00015490: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
+000154a0: 765f 7374 7269 6e67 5f69 6d70 6f72 7428  v_string_import(
+000154b0: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
+000154c0: 6174 6120 3d20 6373 765f 6461 7461 0a20  ata = csv_data. 
+000154d0: 2020 2020 2020 2063 7376 7461 626c 6520         csvtable 
+000154e0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+000154f0: 5f69 6d70 6f72 7428 6373 765f 736f 7572  _import(csv_sour
+00015500: 6365 3d64 6174 612c 2074 7261 6e73 666f  ce=data, transfo
+00015510: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
+00015520: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
+00015530: 747d 290a 0a20 2020 2020 2020 2074 6573  t})..        tes
+00015540: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
+00015550: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+00015560: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+00015570: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+00015580: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
+00015590: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000155a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000155b0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000155c0: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
+000155d0: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
+000155e0: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
+000155f0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
+00015600: 7a69 7028 7431 2c20 6373 7674 6162 6c65  zip(t1, csvtable
+00015610: 2929 290a 2020 2020 2020 2020 7769 7468  ))).        with
+00015620: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00015630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015640: 662e 6173 7365 7274 4571 7561 6c28 7375  f.assertEqual(su
+00015650: 6d28 3120 666f 7220 6c69 6e65 2069 6e20  m(1 for line in 
+00015660: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
+00015670: 2920 6966 206c 696e 652e 7374 7269 7028  ) if line.strip(
+00015680: 2929 2d31 2c20 6c65 6e28 6373 7674 6162  ))-1, len(csvtab
+00015690: 6c65 2929 0a0a 2020 2020 2020 2020 726f  le))..        ro
+000156a0: 775f 7072 6f74 6f74 7970 6520 3d20 7365  w_prototype = se
+000156b0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000156c0: 6563 7428 302c 2030 2c20 3029 0a20 2020  ect(0, 0, 0).   
+000156d0: 2020 2020 2063 7376 7461 626c 6532 203d       csvtable2 =
+000156e0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+000156f0: 696d 706f 7274 2864 6174 612c 2074 7261  import(data, tra
+00015700: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
+00015710: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
+00015720: 3a20 696e 747d 2c0a 2020 2020 2020 2020  : int},.        
+00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015750: 2020 726f 775f 636c 6173 733d 7479 7065    row_class=type
+00015760: 2872 6f77 5f70 726f 746f 7479 7065 2929  (row_prototype))
+00015770: 5b3a 335d 0a0a 2020 2020 2020 2020 7072  [:3]..        pr
+00015780: 696e 7428 7479 7065 2874 315b 305d 292e  int(type(t1[0]).
+00015790: 5f5f 6e61 6d65 5f5f 2c20 7431 5b30 5d29  __name__, t1[0])
+000157a0: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
+000157b0: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+000157c0: 292e 5f5f 6e61 6d65 5f5f 2c20 6373 7674  ).__name__, csvt
+000157d0: 6162 6c65 325b 305d 290a 2020 2020 2020  able2[0]).      
+000157e0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+000157f0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00015800: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00015810: 7561 6c28 7479 7065 2874 315b 305d 292c  ual(type(t1[0]),
+00015820: 2074 7970 6528 6373 7674 6162 6c65 325b   type(csvtable2[
+00015830: 305d 2929 0a0a 2020 2020 6465 6620 7465  0]))..    def te
+00015840: 7374 5f63 7376 5f6c 696d 6974 5f69 6d70  st_csv_limit_imp
+00015850: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
+00015860: 2020 2064 6174 6120 3d20 6373 765f 6461     data = csv_da
+00015870: 7461 0a20 2020 2020 2020 2069 6d70 6f72  ta.        impor
+00015880: 745f 6c69 6d69 7420 3d20 3130 0a20 2020  t_limit = 10.   
+00015890: 2020 2020 2063 7376 7461 626c 6520 3d20       csvtable = 
+000158a0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+000158b0: 6d70 6f72 7428 6373 765f 736f 7572 6365  mport(csv_source
+000158c0: 3d64 6174 612c 2074 7261 6e73 666f 726d  =data, transform
+000158d0: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
+000158e0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
+000158f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015910: 2020 2020 2020 2020 2020 206c 696d 6974             limit
+00015920: 3d69 6d70 6f72 745f 6c69 6d69 7429 0a0a  =import_limit)..
+00015930: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00015940: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00015950: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00015960: 7365 7274 4571 7561 6c28 696d 706f 7274  sertEqual(import
+00015970: 5f6c 696d 6974 2c20 6c65 6e28 6373 7674  _limit, len(csvt
+00015980: 6162 6c65 2929 0a0a 2020 2020 2020 2020  able))..        
+00015990: 6373 7674 6162 6c65 203d 206c 742e 5461  csvtable = lt.Ta
+000159a0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+000159b0: 2863 7376 5f73 6f75 7263 653d 6461 7461  (csv_source=data
+000159c0: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
+000159d0: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
+000159e0: 2c20 2763 273a 2069 6e74 7d2c 0a20 2020  , 'c': int},.   
+000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a10: 2020 2020 2020 6c69 6d69 743d 3029 0a0a        limit=0)..
+00015a20: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00015a30: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00015a40: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00015a50: 7365 7274 4571 7561 6c28 302c 206c 656e  sertEqual(0, len
+00015a60: 2863 7376 7461 626c 6529 290a 0a20 2020  (csvtable))..   
+00015a70: 2064 6566 2074 6573 745f 6373 765f 7374   def test_csv_st
+00015a80: 7269 6e67 5f6c 6973 745f 696d 706f 7274  ring_list_import
+00015a90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00015aa0: 6461 7461 203d 2063 7376 5f64 6174 610a  data = csv_data.
+00015ab0: 2020 2020 2020 2020 6373 7674 6162 6c65          csvtable
+00015ac0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+00015ad0: 765f 696d 706f 7274 2863 7376 5f73 6f75  v_import(csv_sou
+00015ae0: 7263 653d 6461 7461 2e73 706c 6974 6c69  rce=data.splitli
+00015af0: 6e65 7328 292c 2074 7261 6e73 666f 726d  nes(), transform
+00015b00: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
+00015b10: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
+00015b20: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
+00015b30: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
+00015b40: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
+00015b50: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
+00015b60: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
+00015b70: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+00015b80: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00015b90: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00015ba0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00015bb0: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
+00015bc0: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
+00015bd0: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
+00015be0: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
+00015bf0: 7028 7431 2c20 6373 7674 6162 6c65 2929  p(t1, csvtable))
+00015c00: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00015c10: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00015c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015c30: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00015c40: 3120 666f 7220 6c69 6e65 2069 6e20 6461  1 for line in da
+00015c50: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
+00015c60: 6966 206c 696e 652e 7374 7269 7028 2929  if line.strip())
+00015c70: 2d31 2c20 6c65 6e28 6373 7674 6162 6c65  -1, len(csvtable
+00015c80: 2929 0a0a 2020 2020 2020 2020 726f 775f  ))..        row_
+00015c90: 7072 6f74 6f74 7970 6520 3d20 7365 6c66  prototype = self
+00015ca0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00015cb0: 7428 302c 2030 2c20 3029 0a20 2020 2020  t(0, 0, 0).     
+00015cc0: 2020 2063 7376 7461 626c 6532 203d 206c     csvtable2 = l
+00015cd0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00015ce0: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
+00015cf0: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+00015d00: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+00015d10: 696e 747d 2c0a 2020 2020 2020 2020 2020  int},.          
+00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d40: 726f 775f 636c 6173 733d 7479 7065 2872  row_class=type(r
+00015d50: 6f77 5f70 726f 746f 7479 7065 2929 5b3a  ow_prototype))[:
+00015d60: 335d 0a0a 2020 2020 2020 2020 7072 696e  3]..        prin
+00015d70: 7428 7479 7065 2874 315b 305d 292e 5f5f  t(type(t1[0]).__
+00015d80: 6e61 6d65 5f5f 2c20 7431 5b30 5d29 0a20  name__, t1[0]). 
+00015d90: 2020 2020 2020 2070 7269 6e74 2874 7970         print(typ
+00015da0: 6528 6373 7674 6162 6c65 325b 305d 292e  e(csvtable2[0]).
+00015db0: 5f5f 6e61 6d65 5f5f 2c20 6373 7674 6162  __name__, csvtab
+00015dc0: 6c65 325b 305d 290a 2020 2020 2020 2020  le2[0]).        
+00015dd0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00015de0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00015df0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00015e00: 6c28 7479 7065 2874 315b 305d 292c 2074  l(type(t1[0]), t
+00015e10: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+00015e20: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00015e30: 5f63 7376 5f6e 756d 6572 6963 5f74 7261  _csv_numeric_tra
+00015e40: 6e73 666f 726d 7328 7365 6c66 293a 0a20  nsforms(self):. 
+00015e50: 2020 2020 2020 2064 6174 6120 3d20 7465         data = te
+00015e60: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
+00015e70: 225c 0a20 2020 2020 2020 2020 2020 2074  "\.            t
+00015e80: 7970 652c 7661 6c75 650a 2020 2020 2020  ype,value.      
+00015e90: 2020 2020 2020 696e 742c 3130 3030 0a20        int,1000. 
+00015ea0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00015eb0: 2c33 2e31 340a 2020 2020 2020 2020 2020  ,3.14.          
+00015ec0: 2020 656d 7074 792c 0a20 2020 2020 2020    empty,.       
+00015ed0: 2020 2020 2073 7472 2ce2 93a0 2a62 6572       str,...*ber
+00015ee0: 740a 2020 2020 2020 2020 2020 2020 2222  t.            ""
+00015ef0: 2229 0a0a 2020 2020 2020 2020 7769 7468  ")..        with
+00015f00: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+00015f10: 6f6e 7665 7274 5f6e 756d 6572 6963 2229  onvert_numeric")
+00015f20: 3a0a 2020 2020 2020 2020 2020 2020 7462  :.            tb
+00015f30: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e63  l = lt.Table().c
+00015f40: 7376 5f69 6d70 6f72 7428 6461 7461 2c20  sv_import(data, 
+00015f50: 7472 616e 7366 6f72 6d73 3d7b 2776 616c  transforms={'val
+00015f60: 7565 273a 206c 742e 5461 626c 652e 636f  ue': lt.Table.co
+00015f70: 6e76 6572 745f 6e75 6d65 7269 637d 290a  nvert_numeric}).
+00015f80: 2020 2020 2020 2020 2020 2020 7462 6c2e              tbl.
+00015f90: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+00015fa0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00015fb0: 7445 7175 616c 285b 3130 3030 2c20 332e  tEqual([1000, 3.
+00015fc0: 3134 2c20 2727 2c20 27e2 93a0 2a62 6572  14, '', '...*ber
+00015fd0: 7427 5d2c 206c 6973 7428 7462 6c2e 616c  t'], list(tbl.al
+00015fe0: 6c2e 7661 6c75 6529 290a 0a20 2020 2020  l.value))..     
+00015ff0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00016000: 5465 7374 2822 636f 6e76 6572 745f 6e75  Test("convert_nu
+00016010: 6d65 7269 6328 2922 293a 0a20 2020 2020  meric()"):.     
+00016020: 2020 2020 2020 2074 626c 203d 206c 742e         tbl = lt.
+00016030: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00016040: 7274 2864 6174 612c 2074 7261 6e73 666f  rt(data, transfo
+00016050: 726d 733d 7b27 7661 6c75 6527 3a20 6c74  rms={'value': lt
+00016060: 2e54 6162 6c65 2e63 6f6e 7665 7274 5f6e  .Table.convert_n
+00016070: 756d 6572 6963 2829 7d29 0a20 2020 2020  umeric()}).     
+00016080: 2020 2020 2020 2074 626c 2e70 7265 7365         tbl.prese
+00016090: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
+000160a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000160b0: 6c28 5b31 3030 302c 2033 2e31 342c 2027  l([1000, 3.14, '
+000160c0: 272c 2027 e293 a02a 6265 7274 275d 2c20  ', '...*bert'], 
+000160d0: 6c69 7374 2874 626c 2e61 6c6c 2e76 616c  list(tbl.all.val
+000160e0: 7565 2929 0a0a 2020 2020 2020 2020 7769  ue))..        wi
+000160f0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00016100: 2263 6f6e 7665 7274 5f6e 756d 6572 6963  "convert_numeric
+00016110: 286e 6f6e 5f6e 756d 6572 6963 3d4e 6f6e  (non_numeric=Non
+00016120: 6529 2229 3a0a 2020 2020 2020 2020 2020  e)"):.          
+00016130: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00016140: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
+00016150: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
+00016160: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
+00016170: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
+00016180: 6328 6e6f 6e5f 6e75 6d65 7269 633d 4e6f  c(non_numeric=No
+00016190: 6e65 297d 290a 2020 2020 2020 2020 2020  ne)}).          
+000161a0: 2020 7462 6c2e 7072 6573 656e 7428 290a    tbl.present().
+000161b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000161c0: 2e61 7373 6572 7445 7175 616c 285b 3130  .assertEqual([10
+000161d0: 3030 2c20 332e 3134 2c20 2727 2c20 4e6f  00, 3.14, '', No
+000161e0: 6e65 5d2c 206c 6973 7428 7462 6c2e 616c  ne], list(tbl.al
+000161f0: 6c2e 7661 6c75 6529 290a 0a20 2020 2020  l.value))..     
+00016200: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00016210: 5465 7374 2822 636f 6e76 6572 745f 6e75  Test("convert_nu
+00016220: 6d65 7269 6328 6e6f 6e5f 6e75 6d65 7269  meric(non_numeri
+00016230: 633d 3029 2229 3a0a 2020 2020 2020 2020  c=0)"):.        
+00016240: 2020 2020 7462 6c20 3d20 6c74 2e54 6162      tbl = lt.Tab
+00016250: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+00016260: 6461 7461 2c20 7472 616e 7366 6f72 6d73  data, transforms
+00016270: 3d7b 2776 616c 7565 273a 206c 742e 5461  ={'value': lt.Ta
+00016280: 626c 652e 636f 6e76 6572 745f 6e75 6d65  ble.convert_nume
+00016290: 7269 6328 6e6f 6e5f 6e75 6d65 7269 633d  ric(non_numeric=
+000162a0: 3029 7d29 0a20 2020 2020 2020 2020 2020  0)}).           
+000162b0: 2074 626c 2e70 7265 7365 6e74 2829 0a20   tbl.present(). 
+000162c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000162d0: 6173 7365 7274 4571 7561 6c28 5b31 3030  assertEqual([100
+000162e0: 302c 2033 2e31 342c 2027 272c 2030 5d2c  0, 3.14, '', 0],
+000162f0: 206c 6973 7428 7462 6c2e 616c 6c2e 7661   list(tbl.all.va
+00016300: 6c75 6529 290a 0a20 2020 2020 2020 2077  lue))..        w
+00016310: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00016320: 2822 636f 6e76 6572 745f 6e75 6d65 7269  ("convert_numeri
+00016330: 6328 696e 745f 746f 5f66 6c6f 6174 3d54  c(int_to_float=T
+00016340: 7275 6529 2229 3a0a 2020 2020 2020 2020  rue)"):.        
+00016350: 2020 2020 7462 6c20 3d20 6c74 2e54 6162      tbl = lt.Tab
+00016360: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+00016370: 6461 7461 2c20 7472 616e 7366 6f72 6d73  data, transforms
+00016380: 3d7b 2776 616c 7565 273a 206c 742e 5461  ={'value': lt.Ta
+00016390: 626c 652e 636f 6e76 6572 745f 6e75 6d65  ble.convert_nume
+000163a0: 7269 6328 666f 7263 655f 666c 6f61 743d  ric(force_float=
+000163b0: 5472 7565 297d 290a 2020 2020 2020 2020  True)}).        
+000163c0: 2020 2020 7462 6c2e 7072 6573 656e 7428      tbl.present(
+000163d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000163e0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+000163f0: 3130 3030 2e30 2c20 332e 3134 2c20 2727  1000.0, 3.14, ''
+00016400: 2c20 27e2 93a0 2a62 6572 7427 5d2c 206c  , '...*bert'], l
+00016410: 6973 7428 7462 6c2e 616c 6c2e 7661 6c75  ist(tbl.all.valu
+00016420: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00016430: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00016440: 285b 666c 6f61 742c 2066 6c6f 6174 2c20  ([float, float, 
+00016450: 7374 722c 2073 7472 5d2c 206c 6973 7428  str, str], list(
+00016460: 7479 7065 2876 2920 666f 7220 7620 696e  type(v) for v in
+00016470: 2074 626c 2e61 6c6c 2e76 616c 7565 2929   tbl.all.value))
+00016480: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00016490: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
+000164a0: 7665 7274 5f6e 756d 6572 6963 286e 6f6e  vert_numeric(non
+000164b0: 5f6e 756d 6572 6963 3d4e 6f6e 652c 2065  _numeric=None, e
+000164c0: 6d70 7479 3d4e 6f6e 6529 2229 3a0a 2020  mpty=None)"):.  
+000164d0: 2020 2020 2020 2020 2020 7462 6c20 3d20            tbl = 
+000164e0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+000164f0: 6d70 6f72 7428 6461 7461 2c20 7472 616e  mport(data, tran
+00016500: 7366 6f72 6d73 3d7b 2776 616c 7565 273a  sforms={'value':
+00016510: 206c 742e 5461 626c 652e 636f 6e76 6572   lt.Table.conver
+00016520: 745f 6e75 6d65 7269 6328 6e6f 6e5f 6e75  t_numeric(non_nu
+00016530: 6d65 7269 633d 4e6f 6e65 2c20 656d 7074  meric=None, empt
+00016540: 793d 4e6f 6e65 297d 290a 2020 2020 2020  y=None)}).      
+00016550: 2020 2020 2020 7462 6c2e 7072 6573 656e        tbl.presen
+00016560: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00016570: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00016580: 285b 3130 3030 2c20 332e 3134 2c20 4e6f  ([1000, 3.14, No
+00016590: 6e65 2c20 4e6f 6e65 5d2c 206c 6973 7428  ne, None], list(
+000165a0: 7462 6c2e 616c 6c2e 7661 6c75 6529 290a  tbl.all.value)).
+000165b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+000165c0: 6c66 2e73 7562 5465 7374 2822 636f 6e76  lf.subTest("conv
+000165d0: 6572 745f 6e75 6d65 7269 6328 656d 7074  ert_numeric(empt
+000165e0: 793d 4e6f 6e65 2922 293a 0a20 2020 2020  y=None)"):.     
+000165f0: 2020 2020 2020 2074 626c 203d 206c 742e         tbl = lt.
+00016600: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00016610: 7274 2864 6174 612c 2074 7261 6e73 666f  rt(data, transfo
+00016620: 726d 733d 7b27 7661 6c75 6527 3a20 6c74  rms={'value': lt
+00016630: 2e54 6162 6c65 2e63 6f6e 7665 7274 5f6e  .Table.convert_n
+00016640: 756d 6572 6963 2865 6d70 7479 3d4e 6f6e  umeric(empty=Non
+00016650: 6529 7d29 0a20 2020 2020 2020 2020 2020  e)}).           
+00016660: 2074 626c 2e70 7265 7365 6e74 2829 0a20   tbl.present(). 
+00016670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016680: 6173 7365 7274 4571 7561 6c28 5b31 3030  assertEqual([100
+00016690: 302c 2033 2e31 342c 204e 6f6e 652c 2027  0, 3.14, None, '
+000166a0: e293 a02a 6265 7274 275d 2c20 6c69 7374  ...*bert'], list
+000166b0: 2874 626c 2e61 6c6c 2e76 616c 7565 2929  (tbl.all.value))
+000166c0: 0a0a 2020 2020 6465 6620 7465 7374 5f6a  ..    def test_j
+000166d0: 736f 6e5f 6578 706f 7274 5f73 7472 6561  son_export_strea
+000166e0: 6d69 6e67 2873 656c 6629 3a0a 2020 2020  ming(self):.    
+000166f0: 2020 2020 6672 6f6d 2069 7465 7274 6f6f      from itertoo
+00016700: 6c73 2069 6d70 6f72 7420 7065 726d 7574  ls import permut
+00016710: 6174 696f 6e73 0a20 2020 2020 2020 2074  ations.        t
+00016720: 6573 745f 7369 7a65 203d 2033 0a20 2020  est_size = 3.   
+00016730: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
+00016740: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00016750: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00016760: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
+00016770: 2020 2020 666f 7220 6669 656c 646e 616d      for fieldnam
+00016780: 6573 2069 6e20 7065 726d 7574 6174 696f  es in permutatio
+00016790: 6e73 286c 6973 7428 2761 6263 2729 293a  ns(list('abc')):
+000167a0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000167b0: 5f73 7472 696e 6720 3d20 7431 2e6a 736f  _string = t1.jso
+000167c0: 6e5f 6578 706f 7274 284e 6f6e 652c 2066  n_export(None, f
+000167d0: 6965 6c64 6e61 6d65 733d 6669 656c 646e  ieldnames=fieldn
+000167e0: 616d 6573 2c20 7374 7265 616d 696e 673d  ames, streaming=
+000167f0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00016800: 2020 6f75 746c 696e 6573 203d 206f 7574    outlines = out
+00016810: 5f73 7472 696e 672e 7370 6c69 746c 696e  _string.splitlin
+00016820: 6573 2829 0a0a 2020 2020 2020 2020 2020  es()..          
+00016830: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00016840: 6573 7428 6669 656c 646e 616d 6573 3d66  est(fieldnames=f
+00016850: 6965 6c64 6e61 6d65 7329 3a0a 2020 2020  ieldnames):.    
+00016860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016870: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00016880: 745f 7369 7a65 2a2a 332c 206c 656e 286f  t_size**3, len(o
+00016890: 7574 6c69 6e65 7329 290a 0a20 2020 2020  utlines))..     
+000168a0: 2020 2020 2020 2066 6f72 206f 622c 206c         for ob, l
+000168b0: 696e 6520 696e 207a 6970 2874 312c 206f  ine in zip(t1, o
+000168c0: 7574 6c69 6e65 7329 3a0a 2020 2020 2020  utlines):.      
+000168d0: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
+000168e0: 6963 7420 3d20 6a73 6f6e 2e6c 6f61 6473  ict = json.loads
+000168f0: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
+00016900: 2020 2020 2020 2074 315f 6461 7461 6f62         t1_dataob
+00016910: 6a20 3d20 6d61 6b65 5f64 6174 616f 626a  j = make_dataobj
+00016920: 6563 745f 6672 6f6d 5f6f 6228 6f62 290a  ect_from_ob(ob).
+00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016940: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00016950: 7428 6f62 3d6f 622c 206c 696e 653d 6c69  t(ob=ob, line=li
+00016960: 6e65 293a 0a20 2020 2020 2020 2020 2020  ne):.           
+00016970: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00016980: 7365 7274 4571 7561 6c28 7431 5f64 6174  sertEqual(t1_dat
+00016990: 616f 626a 2c20 6c74 2e44 6174 614f 626a  aobj, lt.DataObj
+000169a0: 6563 7428 2a2a 6a73 6f6e 5f64 6963 7429  ect(**json_dict)
+000169b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000169c0: 6a73 6f6e 5f65 7870 6f72 745f 6e6f 6e73  json_export_nons
+000169d0: 7472 6561 6d69 6e67 2873 656c 6629 3a0a  treaming(self):.
+000169e0: 2020 2020 2020 2020 6672 6f6d 2069 7465          from ite
+000169f0: 7274 6f6f 6c73 2069 6d70 6f72 7420 7065  rtools import pe
+00016a00: 726d 7574 6174 696f 6e73 0a20 2020 2020  rmutations.     
+00016a10: 2020 2069 6d70 6f72 7420 6a73 6f6e 0a20     import json. 
+00016a20: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00016a30: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
+00016a40: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00016a50: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00016a60: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00016a70: 7a65 290a 2020 2020 2020 2020 666f 7220  ze).        for 
+00016a80: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
+00016a90: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
+00016aa0: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
+00016ab0: 2020 2020 206f 7574 5f73 7472 696e 6720       out_string 
+00016ac0: 3d20 7431 2e6a 736f 6e5f 6578 706f 7274  = t1.json_export
+00016ad0: 284e 6f6e 652c 2066 6965 6c64 6e61 6d65  (None, fieldname
+00016ae0: 733d 6669 656c 646e 616d 6573 2c20 7374  s=fieldnames, st
+00016af0: 7265 616d 696e 673d 4661 6c73 6529 0a20  reaming=False). 
+00016b00: 2020 2020 2020 2020 2020 206f 6273 6572             obser
+00016b10: 7665 645f 6a73 6f6e 203d 206a 736f 6e2e  ved_json = json.
+00016b20: 6c6f 6164 7328 6f75 745f 7374 7269 6e67  loads(out_string
+00016b30: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00016b40: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00016b50: 2866 6965 6c64 6e61 6d65 733d 6669 656c  (fieldnames=fiel
+00016b60: 646e 616d 6573 293a 0a20 2020 2020 2020  dnames):.       
+00016b70: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00016b80: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00016b90: 697a 652a 2a33 2c20 6c65 6e28 6f62 7365  ize**3, len(obse
+00016ba0: 7276 6564 5f6a 736f 6e29 290a 0a20 2020  rved_json))..   
+00016bb0: 2020 2020 2020 2020 2066 6f72 206f 622c           for ob,
+00016bc0: 206a 736f 6e5f 6469 6374 2069 6e20 7a69   json_dict in zi
+00016bd0: 7028 7431 2c20 6f62 7365 7276 6564 5f6a  p(t1, observed_j
+00016be0: 736f 6e29 3a0a 2020 2020 2020 2020 2020  son):.          
+00016bf0: 2020 2020 2020 7431 5f64 6174 616f 626a        t1_dataobj
+00016c00: 203d 206d 616b 655f 6461 7461 6f62 6a65   = make_dataobje
+00016c10: 6374 5f66 726f 6d5f 6f62 286f 6229 0a20  ct_from_ob(ob). 
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00016c30: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00016c40: 286f 623d 6f62 2c20 6a73 6f6e 5f64 6963  (ob=ob, json_dic
+00016c50: 743d 6a73 6f6e 5f64 6963 7429 3a0a 2020  t=json_dict):.  
+00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00016c80: 616c 2874 315f 6461 7461 6f62 6a2c 206c  al(t1_dataobj, l
+00016c90: 742e 4461 7461 4f62 6a65 6374 282a 2a6a  t.DataObject(**j
+00016ca0: 736f 6e5f 6469 6374 2929 0a0a 2020 2020  son_dict))..    
+00016cb0: 6465 6620 7465 7374 5f6a 736f 6e5f 696d  def test_json_im
+00016cc0: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
+00016cd0: 2020 2020 6461 7461 203d 206a 736f 6e5f      data = json_
+00016ce0: 6461 7461 0a20 2020 2020 2020 2069 6e6a  data.        inj
+00016cf0: 736f 6e20 3d20 696f 2e53 7472 696e 6749  son = io.StringI
+00016d00: 4f28 6461 7461 290a 2020 2020 2020 2020  O(data).        
+00016d10: 6a73 6f6e 7461 626c 6520 3d20 6c74 2e54  jsontable = lt.T
+00016d20: 6162 6c65 2829 2e6a 736f 6e5f 696d 706f  able().json_impo
+00016d30: 7274 2869 6e6a 736f 6e2c 2073 7472 6561  rt(injson, strea
+00016d40: 6d69 6e67 3d54 7275 652c 2074 7261 6e73  ming=True, trans
+00016d50: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+00016d60: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+00016d70: 696e 747d 290a 0a20 2020 2020 2020 2074  int})..        t
+00016d80: 6573 745f 7369 7a65 203d 2033 0a20 2020  est_size = 3.   
+00016d90: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
+00016da0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00016db0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00016dc0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+00016dd0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00016de0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+00016df0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00016e00: 7454 7275 6528 616c 6c28 6d61 6b65 5f64  tTrue(all(make_d
+00016e10: 6174 616f 626a 6563 745f 6672 6f6d 5f6f  ataobject_from_o
+00016e20: 6228 7265 6331 2920 3d3d 2072 6563 3220  b(rec1) == rec2 
+00016e30: 666f 7220 7265 6331 2c20 7265 6332 2069  for rec1, rec2 i
+00016e40: 6e20 7a69 7028 7431 2c20 6a73 6f6e 7461  n zip(t1, jsonta
+00016e50: 626c 6529 2929 0a20 2020 2020 2020 2077  ble))).        w
+00016e60: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00016e70: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00016e80: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00016e90: 286c 656e 285b 6420 666f 7220 6420 696e  (len([d for d in
+00016ea0: 2064 6174 612e 7370 6c69 746c 696e 6573   data.splitlines
+00016eb0: 2829 2069 6620 642e 7374 7269 7028 295d  () if d.strip()]
+00016ec0: 292c 206c 656e 286a 736f 6e74 6162 6c65  ), len(jsontable
+00016ed0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00016ee0: 5f6a 736f 6e5f 7374 7269 6e67 5f69 6d70  _json_string_imp
+00016ef0: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
+00016f00: 2020 2064 6174 6120 3d20 6a73 6f6e 5f64     data = json_d
+00016f10: 6174 610a 2020 2020 2020 2020 6a73 6f6e  ata.        json
+00016f20: 7461 626c 6520 3d20 6c74 2e54 6162 6c65  table = lt.Table
+00016f30: 2829 2e6a 736f 6e5f 696d 706f 7274 2864  ().json_import(d
+00016f40: 6174 612c 2073 7472 6561 6d69 6e67 3d54  ata, streaming=T
+00016f50: 7275 652c 2074 7261 6e73 666f 726d 733d  rue, transforms=
+00016f60: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
+00016f70: 696e 742c 2027 6327 3a20 696e 747d 290a  int, 'c': int}).
+00016f80: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00016f90: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
+00016fa0: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
+00016fb0: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+00016fc0: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+00016fd0: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
+00016fe0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00016ff0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00017000: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00017010: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+00017020: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+00017030: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+00017040: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+00017050: 7431 2c20 6a73 6f6e 7461 626c 6529 2929  t1, jsontable)))
+00017060: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00017070: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00017080: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017090: 7373 6572 7445 7175 616c 286c 656e 285b  ssertEqual(len([
+000170a0: 6420 666f 7220 6420 696e 2064 6174 612e  d for d in data.
+000170b0: 7370 6c69 746c 696e 6573 2829 2069 6620  splitlines() if 
+000170c0: 642e 7374 7269 7028 295d 292c 206c 656e  d.strip()]), len
+000170d0: 286a 736f 6e74 6162 6c65 2929 0a0a 2020  (jsontable))..  
+000170e0: 2020 6465 6620 7465 7374 5f6a 736f 6e5f    def test_json_
+000170f0: 7374 7269 6e67 5f6c 6973 745f 696d 706f  string_list_impo
+00017100: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+00017110: 2020 6461 7461 203d 206a 736f 6e5f 6461    data = json_da
+00017120: 7461 0a20 2020 2020 2020 206a 736f 6e74  ta.        jsont
+00017130: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+00017140: 292e 6a73 6f6e 5f69 6d70 6f72 7428 6461  ).json_import(da
+00017150: 7461 2e73 706c 6974 6c69 6e65 7328 292c  ta.splitlines(),
+00017160: 2073 7472 6561 6d69 6e67 3d54 7275 652c   streaming=True,
+00017170: 2074 7261 6e73 666f 726d 733d 7b27 6127   transforms={'a'
+00017180: 3a20 696e 742c 2027 6227 3a20 696e 742c  : int, 'b': int,
+00017190: 2027 6327 3a20 696e 747d 290a 0a20 2020   'c': int})..   
+000171a0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+000171b0: 2033 0a20 2020 2020 2020 2074 3120 3d20   3.        t1 = 
+000171c0: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+000171d0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+000171e0: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+000171f0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00017200: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00017210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017220: 2e61 7373 6572 7454 7275 6528 616c 6c28  .assertTrue(all(
+00017230: 6d61 6b65 5f64 6174 616f 626a 6563 745f  make_dataobject_
+00017240: 6672 6f6d 5f6f 6228 7265 6331 2920 3d3d  from_ob(rec1) ==
+00017250: 2072 6563 3220 666f 7220 7265 6331 2c20   rec2 for rec1, 
+00017260: 7265 6332 2069 6e20 7a69 7028 7431 2c20  rec2 in zip(t1, 
+00017270: 6a73 6f6e 7461 626c 6529 2929 0a20 2020  jsontable))).   
+00017280: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00017290: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+000172a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000172b0: 7445 7175 616c 286c 656e 285b 6420 666f  tEqual(len([d fo
+000172c0: 7220 6420 696e 2064 6174 612e 7370 6c69  r d in data.spli
+000172d0: 746c 696e 6573 2829 2069 6620 642e 7374  tlines() if d.st
+000172e0: 7269 7028 295d 292c 206c 656e 286a 736f  rip()]), len(jso
+000172f0: 6e74 6162 6c65 2929 0a0a 2020 2020 6465  ntable))..    de
+00017300: 6620 7465 7374 5f6a 736f 6e5f 6e6f 6e73  f test_json_nons
+00017310: 7472 6561 6d69 6e67 5f77 6974 685f 7061  treaming_with_pa
+00017320: 7468 5f69 6d70 6f72 7428 7365 6c66 293a  th_import(self):
+00017330: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00017340: 6a73 6f6e 5f64 6174 610a 2020 2020 2020  json_data.      
+00017350: 2020 6461 7461 203d 2027 2c5c 6e27 2e6a    data = ',\n'.j
+00017360: 6f69 6e28 6461 7461 2e72 7374 7269 7028  oin(data.rstrip(
+00017370: 292e 7370 6c69 746c 696e 6573 2829 290a  ).splitlines()).
+00017380: 2020 2020 2020 2020 6a73 6f6e 5f69 6e70          json_inp
+00017390: 7574 3020 3d20 275b 2720 2b20 6461 7461  ut0 = '[' + data
+000173a0: 202b 2027 5d27 0a20 2020 2020 2020 206a   + ']'.        j
+000173b0: 736f 6e5f 696e 7075 7431 203d 2027 7b20  son_input1 = '{ 
+000173c0: 2264 6174 6122 3a20 5b27 202b 2064 6174  "data": [' + dat
+000173d0: 6120 2b20 275d 7d27 0a20 2020 2020 2020  a + ']}'.       
+000173e0: 206a 736f 6e5f 696e 7075 7432 203d 2027   json_input2 = '
+000173f0: 7b20 2264 6174 6122 3a20 7b20 2269 7465  { "data": { "ite
+00017400: 6d73 223a 205b 2720 2b20 6461 7461 202b  ms": [' + data +
+00017410: 2027 5d7d 7d27 0a0a 2020 2020 2020 2020   ']}}'..        
+00017420: 666f 7220 6a73 6f6e 5f69 6e70 7574 2c20  for json_input, 
+00017430: 7061 7468 2069 6e20 5b0a 2020 2020 2020  path in [.      
+00017440: 2020 2020 2020 286a 736f 6e5f 696e 7075        (json_inpu
+00017450: 7430 2c20 2222 292c 0a20 2020 2020 2020  t0, ""),.       
+00017460: 2020 2020 2028 6a73 6f6e 5f69 6e70 7574       (json_input
+00017470: 312c 2022 6461 7461 2229 2c0a 2020 2020  1, "data"),.    
+00017480: 2020 2020 2020 2020 286a 736f 6e5f 696e          (json_in
+00017490: 7075 7432 2c20 2264 6174 612e 6974 656d  put2, "data.item
+000174a0: 7322 292c 0a20 2020 2020 2020 205d 3a0a  s"),.        ]:.
+000174b0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+000174c0: 7461 626c 6520 3d20 6c74 2e54 6162 6c65  table = lt.Table
+000174d0: 2829 2e6a 736f 6e5f 696d 706f 7274 286a  ().json_import(j
+000174e0: 736f 6e5f 696e 7075 742c 0a20 2020 2020  son_input,.     
+000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2020 2020 2020 2020 2020 7061 7468 3d70            path=p
+00017520: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
+00017560: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
+00017570: 6e74 2c20 2763 273a 2069 6e74 7d29 0a0a  nt, 'c': int})..
+00017580: 2020 2020 2020 2020 2020 2020 7465 7374              test
+00017590: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+000175a0: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
+000175b0: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
+000175c0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+000175d0: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
+000175e0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+000175f0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00017600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017610: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+00017620: 6c6c 286d 616b 655f 6461 7461 6f62 6a65  ll(make_dataobje
+00017630: 6374 5f66 726f 6d5f 6f62 2872 6563 3129  ct_from_ob(rec1)
+00017640: 203d 3d20 7265 6332 2066 6f72 2072 6563   == rec2 for rec
+00017650: 312c 2072 6563 3220 696e 207a 6970 2874  1, rec2 in zip(t
+00017660: 312c 206a 736f 6e74 6162 6c65 2929 290a  1, jsontable))).
+00017670: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00017680: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00017690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000176a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000176b0: 6c28 6c65 6e28 5b64 2066 6f72 2064 2069  l(len([d for d i
+000176c0: 6e20 6461 7461 2e73 706c 6974 6c69 6e65  n data.splitline
+000176d0: 7328 2920 6966 2064 2e73 7472 6970 2829  s() if d.strip()
+000176e0: 5d29 2c20 6c65 6e28 6a73 6f6e 7461 626c  ]), len(jsontabl
+000176f0: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
+00017700: 745f 6a73 6f6e 5f69 6d70 6f72 745f 7769  t_json_import_wi
+00017710: 7468 5f63 7573 746f 6d5f 656e 636f 6465  th_custom_encode
+00017720: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00017730: 2066 726f 6d20 6461 7465 7469 6d65 2069   from datetime i
+00017740: 6d70 6f72 7420 6461 7465 0a20 2020 2020  mport date.     
+00017750: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00017760: 2020 2020 2020 2020 7b27 6127 3a20 3130          {'a': 10
+00017770: 302c 2027 6227 3a20 6461 7465 2832 3030  0, 'b': date(200
+00017780: 302c 2031 2c20 3129 2c20 2763 273a 2032  0, 1, 1), 'c': 2
+00017790: 3030 7d2c 0a20 2020 2020 2020 2020 2020  00},.           
+000177a0: 207b 2761 273a 2031 3031 2c20 2762 273a   {'a': 101, 'b':
+000177b0: 2064 6174 6528 3230 3031 2c20 312c 2031   date(2001, 1, 1
+000177c0: 292c 2027 6327 3a20 3230 317d 2c0a 2020  ), 'c': 201},.  
+000177d0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+000177e0: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
+000177f0: 2e69 6e73 6572 745f 6d61 6e79 2864 6174  .insert_many(dat
+00017800: 6129 0a20 2020 2020 2020 2077 6974 6820  a).        with 
+00017810: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00017820: 7328 5479 7065 4572 726f 7229 3a0a 2020  s(TypeError):.  
+00017830: 2020 2020 2020 2020 2020 7820 3d20 7462            x = tb
+00017840: 6c2e 6a73 6f6e 5f65 7870 6f72 7428 290a  l.json_export().
+00017850: 0a20 2020 2020 2020 2063 6c61 7373 204a  .        class J
+00017860: 736f 6e44 6174 6545 6e63 6f64 6572 286a  sonDateEncoder(j
+00017870: 736f 6e2e 4a53 4f4e 456e 636f 6465 7229  son.JSONEncoder)
+00017880: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00017890: 6620 6465 6661 756c 7428 7365 6c66 2c20  f default(self, 
+000178a0: 6f29 3a0a 2020 2020 2020 2020 2020 2020  o):.            
+000178b0: 2020 2020 696d 706f 7274 2064 6174 6574      import datet
+000178c0: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
+000178d0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000178e0: 6528 6f2c 2064 6174 6574 696d 652e 6461  e(o, datetime.da
+000178f0: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
+00017900: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00017910: 7374 7228 6f29 0a20 2020 2020 2020 2020  str(o).         
+00017920: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+00017930: 7065 7228 292e 6465 6661 756c 7428 6f29  per().default(o)
+00017940: 0a0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
+00017950: 6564 203d 2074 6578 7477 7261 702e 6465  ed = textwrap.de
+00017960: 6465 6e74 2822 2222 5c0a 2020 2020 2020  dent("""\.      
+00017970: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00017980: 2020 2020 7b22 6122 3a20 3130 302c 2022      {"a": 100, "
+00017990: 6222 3a20 2232 3030 302d 3031 2d30 3122  b": "2000-01-01"
+000179a0: 2c20 2263 223a 2032 3030 7d2c 0a20 2020  , "c": 200},.   
+000179b0: 2020 2020 2020 2020 207b 2261 223a 2031           {"a": 1
+000179c0: 3031 2c20 2262 223a 2022 3230 3031 2d30  01, "b": "2001-0
+000179d0: 312d 3031 222c 2022 6322 3a20 3230 317d  1-01", "c": 201}
+000179e0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+000179f0: 2020 2020 2020 2020 2020 2022 2222 290a             """).
+00017a00: 2020 2020 2020 2020 6a73 6f6e 5f72 6573          json_res
+00017a10: 756c 7420 3d20 7462 6c2e 6a73 6f6e 5f65  ult = tbl.json_e
+00017a20: 7870 6f72 7428 6a73 6f6e 5f65 6e63 6f64  xport(json_encod
+00017a30: 6572 3d4a 736f 6e44 6174 6545 6e63 6f64  er=JsonDateEncod
+00017a40: 6572 290a 2020 2020 2020 2020 7365 6c66  er).        self
+00017a50: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
+00017a60: 6563 7465 642c 206a 736f 6e5f 7265 7375  ected, json_resu
+00017a70: 6c74 290a 0a20 2020 2064 6566 2074 6573  lt)..    def tes
+00017a80: 745f 6a73 6f6e 5f69 6d70 6f72 745f 7769  t_json_import_wi
+00017a90: 7468 5f6d 756c 7469 706c 655f 6375 7374  th_multiple_cust
+00017aa0: 6f6d 5f65 6e63 6f64 6572 7328 7365 6c66  om_encoders(self
+00017ab0: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
+00017ac0: 6461 7465 7469 6d65 2069 6d70 6f72 7420  datetime import 
+00017ad0: 6461 7465 0a0a 2020 2020 2020 2020 636c  date..        cl
+00017ae0: 6173 7320 4141 413a 0a20 2020 2020 2020  ass AAA:.       
+00017af0: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
+00017b00: 5f28 7365 6c66 2c20 6e61 6d65 293a 0a20  _(self, name):. 
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017b20: 656c 662e 6e61 6d65 203d 206e 616d 650a  elf.name = name.
+00017b30: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00017b40: 5b0a 2020 2020 2020 2020 2020 2020 7b27  [.            {'
+00017b50: 6127 3a20 3130 302c 2027 6227 3a20 6461  a': 100, 'b': da
+00017b60: 7465 2832 3030 302c 2031 2c20 3129 2c20  te(2000, 1, 1), 
+00017b70: 2763 273a 2032 3030 2c20 2764 273a 2041  'c': 200, 'd': A
+00017b80: 4141 2822 416c 6963 6522 297d 2c0a 2020  AA("Alice")},.  
+00017b90: 2020 2020 2020 2020 2020 7b27 6127 3a20            {'a': 
+00017ba0: 3130 312c 2027 6227 3a20 6461 7465 2832  101, 'b': date(2
+00017bb0: 3030 312c 2031 2c20 3129 2c20 2763 273a  001, 1, 1), 'c':
+00017bc0: 2032 3031 2c20 2764 273a 2041 4141 2822   201, 'd': AAA("
+00017bd0: 426f 6222 297d 2c0a 2020 2020 2020 2020  Bob")},.        
+00017be0: 5d0a 2020 2020 2020 2020 7462 6c20 3d20  ].        tbl = 
+00017bf0: 6c74 2e54 6162 6c65 2829 2e69 6e73 6572  lt.Table().inser
+00017c00: 745f 6d61 6e79 2864 6174 6129 0a20 2020  t_many(data).   
+00017c10: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00017c20: 7373 6572 7452 6169 7365 7328 5479 7065  ssertRaises(Type
+00017c30: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+00017c40: 2020 2020 7820 3d20 7462 6c2e 6a73 6f6e      x = tbl.json
+00017c50: 5f65 7870 6f72 7428 290a 0a20 2020 2020  _export()..     
+00017c60: 2020 2063 6c61 7373 204a 736f 6e44 6174     class JsonDat
+00017c70: 6545 6e63 6f64 6572 286a 736f 6e2e 4a53  eEncoder(json.JS
+00017c80: 4f4e 456e 636f 6465 7229 3a0a 2020 2020  ONEncoder):.    
+00017c90: 2020 2020 2020 2020 6465 6620 6465 6661          def defa
+00017ca0: 756c 7428 7365 6c66 2c20 6f29 3a0a 2020  ult(self, o):.  
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 696d                im
+00017cc0: 706f 7274 2064 6174 6574 696d 650a 2020  port datetime.  
+00017cd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017ce0: 2069 7369 6e73 7461 6e63 6528 6f2c 2064   isinstance(o, d
+00017cf0: 6174 6574 696d 652e 6461 7465 293a 0a20  atetime.date):. 
+00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d10: 2020 2072 6574 7572 6e20 7374 7228 6f29     return str(o)
+00017d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d30: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00017d40: 6465 6661 756c 7428 6f29 0a0a 2020 2020  default(o)..    
+00017d50: 2020 2020 636c 6173 7320 4a73 6f6e 4141      class JsonAA
+00017d60: 4145 6e63 6f64 6572 286a 736f 6e2e 4a53  AEncoder(json.JS
+00017d70: 4f4e 456e 636f 6465 7229 3a0a 2020 2020  ONEncoder):.    
+00017d80: 2020 2020 2020 2020 6465 6620 6465 6661          def defa
+00017d90: 756c 7428 7365 6c66 2c20 6f29 3a0a 2020  ult(self, o):.  
+00017da0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017db0: 2069 7369 6e73 7461 6e63 6528 6f2c 2041   isinstance(o, A
+00017dc0: 4141 293a 0a20 2020 2020 2020 2020 2020  AA):.           
+00017dd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00017de0: 6622 4141 4128 6e61 6d65 3d7b 6f2e 6e61  f"AAA(name={o.na
+00017df0: 6d65 2172 7d29 220a 0a20 2020 2020 2020  me!r})"..       
+00017e00: 2065 7870 6563 7465 6420 3d20 7465 7874   expected = text
+00017e10: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+00017e20: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+00017e30: 2020 2020 2020 2020 2020 207b 2261 223a             {"a":
+00017e40: 2031 3030 2c20 2262 223a 2022 3230 3030   100, "b": "2000
+00017e50: 2d30 312d 3031 222c 2022 6322 3a20 3230  -01-01", "c": 20
+00017e60: 302c 2022 6422 3a20 2241 4141 286e 616d  0, "d": "AAA(nam
+00017e70: 653d 2741 6c69 6365 2729 227d 2c0a 2020  e='Alice')"},.  
+00017e80: 2020 2020 2020 2020 2020 7b22 6122 3a20            {"a": 
+00017e90: 3130 312c 2022 6222 3a20 2232 3030 312d  101, "b": "2001-
+00017ea0: 3031 2d30 3122 2c20 2263 223a 2032 3031  01-01", "c": 201
+00017eb0: 2c20 2264 223a 2022 4141 4128 6e61 6d65  , "d": "AAA(name
+00017ec0: 3d27 426f 6227 2922 7d0a 2020 2020 2020  ='Bob')"}.      
+00017ed0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00017ee0: 2222 2229 0a0a 2020 2020 2020 2020 6a73  """)..        js
+00017ef0: 6f6e 5f72 6573 756c 7420 3d20 7462 6c2e  on_result = tbl.
+00017f00: 6a73 6f6e 5f65 7870 6f72 7428 6a73 6f6e  json_export(json
+00017f10: 5f65 6e63 6f64 6572 3d28 4a73 6f6e 4461  _encoder=(JsonDa
+00017f20: 7465 456e 636f 6465 722c 204a 736f 6e41  teEncoder, JsonA
+00017f30: 4141 456e 636f 6465 7229 290a 2020 2020  AAEncoder)).    
+00017f40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00017f50: 7175 616c 2865 7870 6563 7465 642c 206a  qual(expected, j
+00017f60: 736f 6e5f 7265 7375 6c74 290a 0a20 2020  son_result)..   
+00017f70: 2064 6566 2074 6573 745f 6669 7865 645f   def test_fixed_
+00017f80: 7769 6474 685f 696d 706f 7274 2873 656c  width_import(sel
+00017f90: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
+00017fa0: 203d 2066 6978 6564 5f77 6964 7468 5f64   = fixed_width_d
+00017fb0: 6174 610a 2020 2020 2020 2020 6461 7461  ata.        data
+00017fc0: 5f66 696c 6520 3d20 696f 2e53 7472 696e  _file = io.Strin
+00017fd0: 6749 4f28 6461 7461 290a 2020 2020 2020  gIO(data).      
+00017fe0: 2020 6677 5f73 7065 6320 3d20 5b28 2761    fw_spec = [('a
+00017ff0: 272c 2030 2c20 4e6f 6e65 2c20 696e 7429  ', 0, None, int)
+00018000: 2c20 2827 6227 2c20 322c 204e 6f6e 652c  , ('b', 2, None,
+00018010: 2069 6e74 292c 2028 2763 272c 2034 2c20   int), ('c', 4, 
+00018020: 4e6f 6e65 2c20 696e 7429 2c20 5d0a 2020  None, int), ].  
+00018030: 2020 2020 2020 7474 203d 206c 742e 5461        tt = lt.Ta
+00018040: 626c 6528 292e 696e 7365 7274 5f6d 616e  ble().insert_man
+00018050: 7928 6c74 2e44 6174 614f 626a 6563 7428  y(lt.DataObject(
+00018060: 2a2a 7265 6329 2066 6f72 2072 6563 2069  **rec) for rec i
+00018070: 6e20 6c74 2e46 6978 6564 5769 6474 6852  n lt.FixedWidthR
+00018080: 6561 6465 7228 6677 5f73 7065 632c 2064  eader(fw_spec, d
+00018090: 6174 615f 6669 6c65 2929 0a0a 2020 2020  ata_file))..    
+000180a0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+000180b0: 330a 2020 2020 2020 2020 7431 203d 206d  3.        t1 = m
+000180c0: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
+000180d0: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
+000180e0: 6a65 6374 2c20 7465 7374 5f73 697a 6529  ject, test_size)
+000180f0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00018100: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00018110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018120: 6173 7365 7274 5472 7565 2861 6c6c 286d  assertTrue(all(m
+00018130: 616b 655f 6461 7461 6f62 6a65 6374 5f66  ake_dataobject_f
+00018140: 726f 6d5f 6f62 2872 6563 3129 203d 3d20  rom_ob(rec1) == 
+00018150: 7265 6332 2066 6f72 2072 6563 312c 2072  rec2 for rec1, r
+00018160: 6563 3220 696e 207a 6970 2874 312c 2074  ec2 in zip(t1, t
+00018170: 7429 2929 0a20 2020 2020 2020 2077 6974  t))).        wit
+00018180: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00018190: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000181a0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+000181b0: 656e 285b 6420 666f 7220 6420 696e 2064  en([d for d in d
+000181c0: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+000181d0: 2069 6620 642e 7374 7269 7028 295d 292c   if d.strip()]),
+000181e0: 206c 656e 2874 7429 290a 0a20 2020 2064   len(tt))..    d
+000181f0: 6566 2074 6573 745f 6669 7865 645f 7769  ef test_fixed_wi
+00018200: 6474 685f 7374 7269 6e67 5f69 6d70 6f72  dth_string_impor
+00018210: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00018220: 2064 6174 6120 3d20 6669 7865 645f 7769   data = fixed_wi
+00018230: 6474 685f 6461 7461 0a20 2020 2020 2020  dth_data.       
+00018240: 2066 775f 7370 6563 203d 205b 2827 6127   fw_spec = [('a'
+00018250: 2c20 302c 204e 6f6e 652c 2069 6e74 292c  , 0, None, int),
+00018260: 2028 2762 272c 2032 2c20 4e6f 6e65 2c20   ('b', 2, None, 
+00018270: 696e 7429 2c20 2827 6327 2c20 342c 204e  int), ('c', 4, N
+00018280: 6f6e 652c 2069 6e74 292c 205d 0a20 2020  one, int), ].   
+00018290: 2020 2020 2074 7420 3d20 6c74 2e54 6162       tt = lt.Tab
+000182a0: 6c65 2829 2e69 6e73 6572 745f 6d61 6e79  le().insert_many
+000182b0: 286c 742e 4461 7461 4f62 6a65 6374 282a  (lt.DataObject(*
+000182c0: 2a72 6563 2920 666f 7220 7265 6320 696e  *rec) for rec in
+000182d0: 206c 742e 4669 7865 6457 6964 7468 5265   lt.FixedWidthRe
+000182e0: 6164 6572 2866 775f 7370 6563 2c20 6461  ader(fw_spec, da
+000182f0: 7461 2929 0a0a 2020 2020 2020 2020 7465  ta))..        te
+00018300: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
+00018310: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
+00018320: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+00018330: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00018340: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+00018350: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00018360: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00018370: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00018380: 5472 7565 2861 6c6c 286d 616b 655f 6461  True(all(make_da
+00018390: 7461 6f62 6a65 6374 5f66 726f 6d5f 6f62  taobject_from_ob
+000183a0: 2872 6563 3129 203d 3d20 7265 6332 2066  (rec1) == rec2 f
+000183b0: 6f72 2072 6563 312c 2072 6563 3220 696e  or rec1, rec2 in
+000183c0: 207a 6970 2874 312c 2074 7429 2929 0a20   zip(t1, tt))). 
+000183d0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000183e0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+000183f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00018400: 6572 7445 7175 616c 286c 656e 285b 6420  ertEqual(len([d 
+00018410: 666f 7220 6420 696e 2064 6174 612e 7370  for d in data.sp
+00018420: 6c69 746c 696e 6573 2829 2069 6620 642e  litlines() if d.
+00018430: 7374 7269 7028 295d 292c 206c 656e 2874  strip()]), len(t
+00018440: 7429 290a 0a20 2020 2064 6566 2074 6573  t))..    def tes
+00018450: 745f 6669 7865 645f 7769 6474 685f 7374  t_fixed_width_st
+00018460: 7269 6e67 5f6c 6973 745f 696d 706f 7274  ring_list_import
+00018470: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00018480: 6461 7461 203d 2066 6978 6564 5f77 6964  data = fixed_wid
+00018490: 7468 5f64 6174 610a 2020 2020 2020 2020  th_data.        
+000184a0: 6677 5f73 7065 6320 3d20 5b28 2761 272c  fw_spec = [('a',
+000184b0: 2030 2c20 4e6f 6e65 2c20 696e 7429 2c20   0, None, int), 
+000184c0: 2827 6227 2c20 322c 204e 6f6e 652c 2069  ('b', 2, None, i
+000184d0: 6e74 292c 2028 2763 272c 2034 2c20 4e6f  nt), ('c', 4, No
+000184e0: 6e65 2c20 696e 7429 2c5d 0a20 2020 2020  ne, int),].     
+000184f0: 2020 2074 7420 3d20 6c74 2e54 6162 6c65     tt = lt.Table
+00018500: 2829 2e69 6e73 6572 745f 6d61 6e79 286c  ().insert_many(l
+00018510: 742e 4461 7461 4f62 6a65 6374 282a 2a72  t.DataObject(**r
+00018520: 6563 2920 666f 7220 7265 6320 696e 206c  ec) for rec in l
+00018530: 742e 4669 7865 6457 6964 7468 5265 6164  t.FixedWidthRead
+00018540: 6572 2866 775f 7370 6563 2c20 6461 7461  er(fw_spec, data
+00018550: 2e73 706c 6974 6c69 6e65 7328 2929 290a  .splitlines())).
+00018560: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00018570: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
+00018580: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
+00018590: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+000185a0: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+000185b0: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
+000185c0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+000185d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000185e0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+000185f0: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+00018600: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+00018610: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+00018620: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+00018630: 7431 2c20 7474 2929 290a 2020 2020 2020  t1, tt))).      
+00018640: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00018650: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00018660: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00018670: 7561 6c28 6c65 6e28 5b64 2066 6f72 2064  ual(len([d for d
+00018680: 2069 6e20 6461 7461 2e73 706c 6974 6c69   in data.splitli
+00018690: 6e65 7328 2920 6966 2064 2e73 7472 6970  nes() if d.strip
+000186a0: 2829 5d29 2c20 6c65 6e28 7474 2929 0a0a  ()]), len(tt))..
+000186b0: 2020 2020 6465 6620 7465 7374 5f65 7863      def test_exc
+000186c0: 656c 5f69 6d70 6f72 7428 7365 6c66 293a  el_import(self):
+000186d0: 0a20 2020 2020 2020 2066 696c 655f 6e61  .        file_na
+000186e0: 6d65 203d 2022 7465 7374 2f61 6263 2e78  me = "test/abc.x
+000186f0: 6c73 7822 0a20 2020 2020 2020 2065 7863  lsx".        exc
+00018700: 656c 5f74 6162 6c65 203d 206c 742e 5461  el_table = lt.Ta
+00018710: 626c 6528 292e 6578 6365 6c5f 696d 706f  ble().excel_impo
+00018720: 7274 2866 696c 655f 6e61 6d65 2c20 7472  rt(file_name, tr
+00018730: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
+00018740: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
+00018750: 273a 2069 6e74 7d29 0a0a 2020 2020 2020  ': int})..      
+00018760: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
+00018770: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
+00018780: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
+00018790: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+000187a0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
+000187b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000187c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000187d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000187e0: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
+000187f0: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
+00018800: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
+00018810: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
+00018820: 3220 696e 207a 6970 2874 312c 2065 7863  2 in zip(t1, exc
+00018830: 656c 5f74 6162 6c65 2929 290a 2020 2020  el_table))).    
+00018840: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00018850: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00018860: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00018870: 4571 7561 6c28 7375 6d28 3120 666f 7220  Equal(sum(1 for 
+00018880: 6c69 6e65 2069 6e20 6373 765f 6461 7461  line in csv_data
+00018890: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
+000188a0: 206c 696e 652e 7374 7269 7028 2929 2d31   line.strip())-1
+000188b0: 2c20 6c65 6e28 6578 6365 6c5f 7461 626c  , len(excel_tabl
+000188c0: 6529 290a 0a20 2020 2020 2020 2072 6f77  e))..        row
+000188d0: 5f70 726f 746f 7479 7065 203d 2073 656c  _prototype = sel
+000188e0: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+000188f0: 6374 2830 2c20 302c 2030 290a 2020 2020  ct(0, 0, 0).    
+00018900: 2020 2020 6373 7674 6162 6c65 3220 3d20      csvtable2 = 
+00018910: 6c74 2e54 6162 6c65 2829 2e65 7863 656c  lt.Table().excel
+00018920: 5f69 6d70 6f72 7428 0a20 2020 2020 2020  _import(.       
+00018930: 2020 2020 2066 696c 655f 6e61 6d65 2c20       file_name, 
+00018940: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
+00018950: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
+00018960: 2763 273a 2069 6e74 7d2c 2072 6f77 5f63  'c': int}, row_c
+00018970: 6c61 7373 3d74 7970 6528 726f 775f 7072  lass=type(row_pr
+00018980: 6f74 6f74 7970 6529 0a20 2020 2020 2020  ototype).       
+00018990: 2029 5b3a 335d 0a0a 2020 2020 2020 2020   )[:3]..        
+000189a0: 7072 696e 7428 7479 7065 2874 315b 305d  print(type(t1[0]
+000189b0: 292e 5f5f 6e61 6d65 5f5f 2c20 7431 5b30  ).__name__, t1[0
+000189c0: 5d29 0a20 2020 2020 2020 2070 7269 6e74  ]).        print
+000189d0: 2874 7970 6528 6373 7674 6162 6c65 325b  (type(csvtable2[
+000189e0: 305d 292e 5f5f 6e61 6d65 5f5f 2c20 6373  0]).__name__, cs
+000189f0: 7674 6162 6c65 325b 305d 290a 2020 2020  vtable2[0]).    
+00018a00: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00018a10: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00018a20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00018a30: 4571 7561 6c28 7479 7065 2874 315b 305d  Equal(type(t1[0]
+00018a40: 292c 2074 7970 6528 6373 7674 6162 6c65  ), type(csvtable
+00018a50: 325b 305d 2929 0a0a 2020 2020 6465 6620  2[0]))..    def 
+00018a60: 7465 7374 5f65 7863 656c 5f65 7870 6f72  test_excel_expor
+00018a70: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00018a80: 2066 696c 655f 6e61 6d65 203d 2022 7465   file_name = "te
+00018a90: 7374 2f61 6263 2e78 6c73 7822 0a20 2020  st/abc.xlsx".   
+00018aa0: 2020 2020 2065 7863 656c 5f74 6162 6c65       excel_table
+00018ab0: 203d 206c 742e 5461 626c 6528 292e 6578   = lt.Table().ex
+00018ac0: 6365 6c5f 696d 706f 7274 2866 696c 655f  cel_import(file_
+00018ad0: 6e61 6d65 2c20 7472 616e 7366 6f72 6d73  name, transforms
+00018ae0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
+00018af0: 2069 6e74 2c20 2763 273a 2069 6e74 7d2c   int, 'c': int},
+00018b00: 206c 696d 6974 3d31 290a 2020 2020 2020   limit=1).      
+00018b10: 2020 6f75 7466 696c 6520 3d20 696f 2e42    outfile = io.B
+00018b20: 7974 6573 494f 2829 0a20 2020 2020 2020  ytesIO().       
+00018b30: 2065 7863 656c 5f74 6162 6c65 2e65 7863   excel_table.exc
+00018b40: 656c 5f65 7870 6f72 7428 6f75 7466 696c  el_export(outfil
+00018b50: 6529 0a20 2020 2020 2020 2065 7870 6f72  e).        expor
+00018b60: 7465 645f 7461 626c 6520 3d20 6c74 2e54  ted_table = lt.T
+00018b70: 6162 6c65 2829 2e65 7863 656c 5f69 6d70  able().excel_imp
+00018b80: 6f72 7428 6f75 7466 696c 652c 2074 7261  ort(outfile, tra
+00018b90: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
+00018ba0: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
+00018bb0: 3a20 696e 747d 290a 0a20 2020 2020 2020  : int})..       
+00018bc0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00018bd0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00018be0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00018bf0: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
+00018c00: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
+00018c10: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
+00018c20: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
+00018c30: 7028 6578 706f 7274 6564 5f74 6162 6c65  p(exported_table
+00018c40: 2c20 6578 6365 6c5f 7461 626c 6529 2929  , excel_table)))
+00018c50: 0a0a 2020 2020 6465 6620 7465 7374 5f6d  ..    def test_m
+00018c60: 6f64 756c 655f 6c65 7665 6c5f 6373 765f  odule_level_csv_
+00018c70: 696d 706f 7274 6572 2873 656c 6629 3a0a  importer(self):.
+00018c80: 2020 2020 2020 2020 6461 7461 203d 2063          data = c
+00018c90: 7376 5f64 6174 610a 2020 2020 2020 2020  sv_data.        
+00018ca0: 6373 7674 6162 6c65 203d 206c 742e 6373  csvtable = lt.cs
+00018cb0: 765f 696d 706f 7274 2863 7376 5f73 6f75  v_import(csv_sou
+00018cc0: 7263 653d 6461 7461 2c20 7472 616e 7366  rce=data, transf
+00018cd0: 6f72 6d73 3d7b 2761 273a 2069 6e74 2c20  orms={'a': int, 
+00018ce0: 2762 273a 2069 6e74 2c20 2763 273a 2069  'b': int, 'c': i
+00018cf0: 6e74 7d29 0a0a 2020 2020 2020 2020 7465  nt})..        te
+00018d00: 7374 5f73 697a 6520 3d20 330a 2020 2020  st_size = 3.    
+00018d10: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
+00018d20: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+00018d30: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00018d40: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+00018d50: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00018d60: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00018d70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00018d80: 5472 7565 2861 6c6c 286d 616b 655f 6461  True(all(make_da
+00018d90: 7461 6f62 6a65 6374 5f66 726f 6d5f 6f62  taobject_from_ob
+00018da0: 2872 6563 3129 203d 3d20 7265 6332 2066  (rec1) == rec2 f
+00018db0: 6f72 2072 6563 312c 2072 6563 3220 696e  or rec1, rec2 in
+00018dc0: 207a 6970 2874 312c 2063 7376 7461 626c   zip(t1, csvtabl
+00018dd0: 6529 2929 0a20 2020 2020 2020 2077 6974  e))).        wit
+00018de0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00018df0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018e00: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+00018e10: 756d 2831 2066 6f72 206c 696e 6520 696e  um(1 for line in
+00018e20: 2064 6174 612e 7370 6c69 746c 696e 6573   data.splitlines
+00018e30: 2829 2069 6620 6c69 6e65 2e73 7472 6970  () if line.strip
+00018e40: 2829 292d 312c 206c 656e 2863 7376 7461  ())-1, len(csvta
+00018e50: 626c 6529 290a 0a20 2020 2064 6566 2074  ble))..    def t
+00018e60: 6573 745f 6d6f 6475 6c65 5f6c 6576 656c  est_module_level
+00018e70: 5f6a 736f 6e5f 696d 706f 7274 6572 2873  _json_importer(s
+00018e80: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
+00018e90: 7461 203d 206a 736f 6e5f 6461 7461 0a20  ta = json_data. 
+00018ea0: 2020 2020 2020 206a 736f 6e74 6162 6c65         jsontable
+00018eb0: 203d 206c 742e 6a73 6f6e 5f69 6d70 6f72   = lt.json_impor
+00018ec0: 7428 6461 7461 2c20 7374 7265 616d 696e  t(data, streamin
+00018ed0: 673d 5472 7565 2c20 7472 616e 7366 6f72  g=True, transfor
+00018ee0: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
+00018ef0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
+00018f00: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
+00018f10: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+00018f20: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00018f30: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00018f40: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00018f50: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00018f60: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00018f70: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00018f80: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00018f90: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00018fa0: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00018fb0: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00018fc0: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00018fd0: 6970 2874 312c 206a 736f 6e74 6162 6c65  ip(t1, jsontable
+00018fe0: 2929 290a 2020 2020 2020 2020 7769 7468  ))).        with
+00018ff0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00019000: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019010: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+00019020: 6e28 5b64 2066 6f72 2064 2069 6e20 6461  n([d for d in da
+00019030: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
+00019040: 6966 2064 2e73 7472 6970 2829 5d29 2c20  if d.strip()]), 
+00019050: 6c65 6e28 6a73 6f6e 7461 626c 6529 290a  len(jsontable)).
+00019060: 0a20 2020 2064 6566 2074 6573 745f 6d6f  .    def test_mo
+00019070: 6475 6c65 5f6c 6576 656c 5f65 7863 656c  dule_level_excel
+00019080: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+00019090: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+000190a0: 203d 2022 7465 7374 2f61 6263 2e78 6c73   = "test/abc.xls
+000190b0: 7822 0a20 2020 2020 2020 2065 7863 656c  x".        excel
+000190c0: 5f74 6162 6c65 203d 206c 742e 6578 6365  _table = lt.exce
+000190d0: 6c5f 696d 706f 7274 2866 696c 655f 6e61  l_import(file_na
+000190e0: 6d65 2c20 7472 616e 7366 6f72 6d73 3d7b  me, transforms={
+000190f0: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
+00019100: 6e74 2c20 2763 273a 2069 6e74 7d29 0a0a  nt, 'c': int})..
+00019110: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
+00019120: 6520 3d20 330a 2020 2020 2020 2020 7431  e = 3.        t1
+00019130: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
+00019140: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
+00019150: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
+00019160: 697a 6529 0a0a 2020 2020 2020 2020 7769  ize)..        wi
+00019170: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00019180: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00019190: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+000191a0: 6c6c 286d 616b 655f 6461 7461 6f62 6a65  ll(make_dataobje
+000191b0: 6374 5f66 726f 6d5f 6f62 2872 6563 3129  ct_from_ob(rec1)
+000191c0: 203d 3d20 7265 6332 2066 6f72 2072 6563   == rec2 for rec
+000191d0: 312c 2072 6563 3220 696e 207a 6970 2874  1, rec2 in zip(t
+000191e0: 312c 2065 7863 656c 5f74 6162 6c65 2929  1, excel_table))
+000191f0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00019200: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00019210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019220: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00019230: 3120 666f 7220 6c69 6e65 2069 6e20 6373  1 for line in cs
+00019240: 765f 6461 7461 2e73 706c 6974 6c69 6e65  v_data.splitline
+00019250: 7328 2920 6966 206c 696e 652e 7374 7269  s() if line.stri
+00019260: 7028 2929 2d31 2c20 6c65 6e28 6578 6365  p())-1, len(exce
+00019270: 6c5f 7461 626c 6529 290a 0a0a 406d 616b  l_table))...@mak
+00019280: 655f 7465 7374 5f63 6c61 7373 6573 0a63  e_test_classes.c
+00019290: 6c61 7373 2054 6162 6c65 5069 766f 7454  lass TablePivotT
+000192a0: 6573 7473 3a0a 2020 2020 2222 220a 2020  ests:.    """.  
+000192b0: 2020 5465 7374 2063 6c61 7373 2066 6f72    Test class for
+000192c0: 2054 6162 6c65 2070 6976 6f74 206f 7065   Table pivot ope
+000192d0: 7261 7469 6f6e 732e 0a20 2020 2022 2222  rations..    """
+000192e0: 0a20 2020 2064 6566 2074 6573 745f 7069  .    def test_pi
+000192f0: 766f 7428 7365 6c66 293a 0a20 2020 2020  vot(self):.     
+00019300: 2020 2074 6573 745f 7369 7a65 203d 2035     test_size = 5
+00019310: 0a20 2020 2020 2020 2074 3120 3d20 6d61  .        t1 = ma
+00019320: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+00019330: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00019340: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+00019350: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
+00019360: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
+00019370: 2020 2020 2074 312e 6372 6561 7465 5f69       t1.create_i
+00019380: 6e64 6578 2827 6227 290a 2020 2020 2020  ndex('b').      
+00019390: 2020 7431 7069 766f 7420 3d20 7431 2e70    t1pivot = t1.p
+000193a0: 6976 6f74 2827 6127 290a 2020 2020 2020  ivot('a').      
+000193b0: 2020 7431 7069 766f 742e 6475 6d70 2829    t1pivot.dump()
+000193c0: 0a20 2020 2020 2020 2074 3170 6976 6f74  .        t1pivot
+000193d0: 2e64 756d 705f 636f 756e 7473 2829 0a20  .dump_counts(). 
+000193e0: 2020 2020 2020 2074 3170 6976 6f74 2e73         t1pivot.s
+000193f0: 756d 6d61 7279 5f63 6f75 6e74 7328 290a  ummary_counts().
+00019400: 0a20 2020 2020 2020 2074 3270 6976 6f74  .        t2pivot
+00019410: 203d 2074 312e 7069 766f 7428 2761 2062   = t1.pivot('a b
+00019420: 2729 0a20 2020 2020 2020 2074 3270 6976  ').        t2piv
+00019430: 6f74 2e64 756d 7028 290a 2020 2020 2020  ot.dump().      
+00019440: 2020 7432 7069 766f 742e 6475 6d70 5f63    t2pivot.dump_c
+00019450: 6f75 6e74 7328 290a 2020 2020 2020 2020  ounts().        
+00019460: 7432 7069 766f 742e 7375 6d6d 6172 795f  t2pivot.summary_
+00019470: 636f 756e 7473 2829 0a0a 2020 2020 2020  counts()..      
+00019480: 2020 2320 544f 444f 202d 2061 6464 2061    # TODO - add a
+00019490: 7373 6572 7473 0a0a 0a63 6c61 7373 2054  sserts...class T
+000194a0: 6162 6c65 5365 6172 6368 5465 7374 7328  ableSearchTests(
+000194b0: 756e 6974 7465 7374 2e54 6573 7443 6173  unittest.TestCas
+000194c0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+000194d0: 5465 7374 2063 6c61 7373 2066 6f72 2066  Test class for f
+000194e0: 756c 6c2d 7465 7874 2073 6561 7263 6820  ull-text search 
+000194f0: 6d65 7468 6f64 732e 0a20 2020 2022 2222  methods..    """
+00019500: 0a20 2020 2072 6563 6970 655f 6461 7461  .    recipe_data
+00019510: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+00019520: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+00019530: 6964 2c74 6974 6c65 2c69 6e67 7265 6469  id,title,ingredi
+00019540: 656e 7473 0a20 2020 2020 2020 2031 2c54  ents.        1,T
+00019550: 756e 6120 6361 7373 6572 6f6c 652c 2274  una casserole,"t
+00019560: 756e 612c 206e 6f6f 646c 6573 2c20 4372  una, noodles, Cr
+00019570: 6561 6d20 6f66 204d 7573 6872 6f6f 6d20  eam of Mushroom 
+00019580: 536f 7570 220a 2020 2020 2020 2020 322c  Soup".        2,
+00019590: 4861 7761 6969 616e 2070 697a 7a61 2c70  Hawaiian pizza,p
+000195a0: 697a 7a61 2064 6f75 6768 2070 696e 6561  izza dough pinea
+000195b0: 7070 6c65 2068 616d 2074 6f6d 6174 6f20  pple ham tomato 
+000195c0: 7361 7563 650a 2020 2020 2020 2020 332c  sauce.        3,
+000195d0: 4d61 7267 6865 7269 7461 2070 697a 7a61  Margherita pizza
+000195e0: 2c70 697a 7a61 2064 6f75 6768 2063 6865  ,pizza dough che
+000195f0: 6573 6520 7065 7374 6f20 6172 7469 6368  ese pesto artich
+00019600: 6f6b 6520 6865 6172 7473 0a20 2020 2020  oke hearts.     
+00019610: 2020 2034 2c50 6570 7065 726f 6e69 2070     4,Pepperoni p
+00019620: 697a 7a61 2c70 697a 7a61 2064 6f75 6768  izza,pizza dough
+00019630: 2063 6865 6573 6520 746f 6d61 746f 2073   cheese tomato s
+00019640: 6175 6365 2070 6570 7065 726f 6e69 0a20  auce pepperoni. 
+00019650: 2020 2020 2020 2035 2c47 7269 6c6c 6564         5,Grilled
+00019660: 2063 6865 6573 6520 7361 6e64 7769 6368   cheese sandwich
+00019670: 2c62 7265 6164 2063 6865 6573 6520 6275  ,bread cheese bu
+00019680: 7474 6572 0a20 2020 2020 2020 2036 2c54  tter.        6,T
+00019690: 756e 6120 6d65 6c74 2c74 756e 6120 6d61  una melt,tuna ma
+000196a0: 796f 6e6e 6169 7365 2074 6f6d 6174 6f20  yonnaise tomato 
+000196b0: 6272 6561 6420 6368 6565 7365 0a20 2020  bread cheese.   
+000196c0: 2020 2020 2037 2c43 6869 6c69 2064 6f67       7,Chili dog
+000196d0: 2c68 6f74 2064 6f67 2063 6869 6c69 206f  ,hot dog chili o
+000196e0: 6e69 6f6e 2062 756e 0a20 2020 2020 2020  nion bun.       
+000196f0: 2038 2c46 7265 6e63 6820 746f 6173 742c   8,French toast,
+00019700: 6567 6720 6d69 6c6b 2076 616e 696c 6c61  egg milk vanilla
+00019710: 2062 7265 6164 206d 6170 6c65 2073 7972   bread maple syr
+00019720: 7570 0a20 2020 2020 2020 2039 2c42 4c54  up.        9,BLT
+00019730: 2c62 7265 6164 2062 6163 6f6e 206c 6574  ,bread bacon let
+00019740: 7475 6365 2074 6f6d 6174 6f20 6d61 796f  tuce tomato mayo
+00019750: 6e6e 6169 7365 0a20 2020 2020 2020 2031  nnaise.        1
+00019760: 302c 5265 7562 656e 2073 616e 6477 6963  0,Reuben sandwic
+00019770: 682c 7279 6520 6272 6561 6420 7361 7565  h,rye bread saue
+00019780: 726b 7261 7574 2063 6f72 6e65 6420 6265  rkraut corned be
+00019790: 6566 2073 7769 7373 2063 6865 6573 6520  ef swiss cheese 
+000197a0: 7275 7373 6961 6e20 6472 6573 7369 6e67  russian dressing
+000197b0: 2074 686f 7573 616e 6420 6973 6c61 6e64   thousand island
+000197c0: 0a20 2020 2020 2020 2031 312c 4861 6d62  .        11,Hamb
+000197d0: 7572 6765 722c 6772 6f75 6e64 2062 6565  urger,ground bee
+000197e0: 6620 6275 6e20 6c65 7474 7563 6520 6b65  f bun lettuce ke
+000197f0: 7463 6875 7020 6d75 7374 6172 6420 7069  tchup mustard pi
+00019800: 636b 6c65 0a20 2020 2020 2020 2031 322c  ckle.        12,
+00019810: 4368 6565 7365 6275 7267 6572 2c67 726f  Cheeseburger,gro
+00019820: 756e 6420 6265 6566 2062 756e 206c 6574  und beef bun let
+00019830: 7475 6365 206b 6574 6368 7570 206d 7573  tuce ketchup mus
+00019840: 7461 7264 2070 6963 6b6c 6520 6368 6565  tard pickle chee
+00019850: 7365 0a20 2020 2020 2020 2031 332c 4261  se.        13,Ba
+00019860: 636f 6e20 6368 6565 7365 6275 7267 6572  con cheeseburger
+00019870: 2c67 726f 756e 6420 6265 6566 2062 756e  ,ground beef bun
+00019880: 206c 6574 7475 6365 206b 6574 6368 7570   lettuce ketchup
+00019890: 206d 7573 7461 7264 2070 6963 6b6c 6520   mustard pickle 
+000198a0: 6368 6565 7365 2062 6163 6f6e 0a20 2020  cheese bacon.   
+000198b0: 2020 2020 2022 2222 290a 0a20 2020 2064       """)..    d
+000198c0: 6566 2073 6574 5570 2873 656c 6629 3a0a  ef setUp(self):.
+000198d0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+000198e0: 6970 6573 203d 206c 742e 5461 626c 6528  ipes = lt.Table(
+000198f0: 292e 6373 765f 696d 706f 7274 2873 656c  ).csv_import(sel
+00019900: 662e 7265 6369 7065 5f64 6174 612c 2074  f.recipe_data, t
+00019910: 7261 6e73 666f 726d 733d 6469 6374 2869  ransforms=dict(i
+00019920: 643d 696e 7429 290a 2020 2020 2020 2020  d=int)).        
+00019930: 7365 6c66 2e72 6563 6970 6573 2e63 7265  self.recipes.cre
+00019940: 6174 655f 696e 6465 7828 2269 6422 2c20  ate_index("id", 
+00019950: 756e 6971 7565 3d54 7275 6529 0a20 2020  unique=True).   
+00019960: 2020 2020 2073 656c 662e 7265 6369 7065       self.recipe
+00019970: 732e 6372 6561 7465 5f73 6561 7263 685f  s.create_search_
+00019980: 696e 6465 7828 2269 6e67 7265 6469 656e  index("ingredien
+00019990: 7473 2229 0a0a 2020 2020 4061 6e6e 6f75  ts")..    @annou
+000199a0: 6e63 655f 7465 7374 0a20 2020 2064 6566  nce_test.    def
+000199b0: 2074 6573 745f 6163 6365 7373 5f6e 6f6e   test_access_non
+000199c0: 5f65 7869 7374 656e 745f 7365 6172 6368  _existent_search
+000199d0: 5f61 7474 7269 6275 7465 2873 656c 6629  _attribute(self)
+000199e0: 3a0a 2020 2020 2020 2020 7769 7468 2073  :.        with s
+000199f0: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00019a00: 2856 616c 7565 4572 726f 722c 206d 7367  (ValueError, msg
+00019a10: 3d22 6661 696c 6564 2074 6f20 7261 6973  ="failed to rais
+00019a20: 6520 5661 6c75 6545 7272 6f72 2077 6865  e ValueError whe
+00019a30: 6e20 6163 6365 7373 696e 6720 6e6f 6e2d  n accessing non-
+00019a40: 6578 6973 7465 6e74 2073 6561 7263 6820  existent search 
+00019a50: 696e 6465 7822 293a 0a20 2020 2020 2020  index"):.       
+00019a60: 2020 2020 2073 656c 662e 7265 6369 7065       self.recipe
+00019a70: 732e 7365 6172 6368 2e74 6974 6c65 2822  s.search.title("
+00019a80: 7879 7a22 290a 0a20 2020 2040 616e 6e6f  xyz")..    @anno
+00019a90: 756e 6365 5f74 6573 740a 2020 2020 6465  unce_test.    de
+00019aa0: 6620 7465 7374 5f73 6561 7263 685f 6469  f test_search_di
+00019ab0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00019ac0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00019ad0: 6c28 5b27 696e 6772 6564 6965 6e74 7327  l(['ingredients'
+00019ae0: 5d2c 2064 6972 2873 656c 662e 7265 6369  ], dir(self.reci
+00019af0: 7065 732e 7365 6172 6368 292c 2022 6661  pes.search), "fa
+00019b00: 696c 6564 2074 6f20 6765 6e65 7261 7465  iled to generate
+00019b10: 2063 6f72 7265 6374 2064 6972 2829 2072   correct dir() r
+00019b20: 6573 706f 6e73 6522 290a 0a20 2020 2040  esponse")..    @
+00019b30: 616e 6e6f 756e 6365 5f74 6573 740a 2020  announce_test.  
+00019b40: 2020 6465 6620 7465 7374 5f74 6578 745f    def test_text_
+00019b50: 7365 6172 6368 2873 656c 6629 3a0a 2020  search(self):.  
+00019b60: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
+00019b70: 2065 7870 6563 7465 6420 696e 205b 0a20   expected in [. 
+00019b80: 2020 2020 2020 2020 2020 2028 2222 2c20             ("", 
+00019b90: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00019ba0: 2028 2274 756e 6122 2c20 5b31 2c20 365d   ("tuna", [1, 6]
+00019bb0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00019bc0: 2274 756e 6120 2b63 6865 6573 6522 2c20  "tuna +cheese", 
+00019bd0: 5b36 2c20 332c 2034 2c20 352c 2031 302c  [6, 3, 4, 5, 10,
+00019be0: 2031 322c 2031 332c 2031 5d29 2c0a 2020   12, 13, 1]),.  
+00019bf0: 2020 2020 2020 2020 2020 2822 7069 6e65            ("pine
+00019c00: 6170 706c 6520 2b62 6163 6f6e 206c 6574  apple +bacon let
+00019c10: 7475 6365 2062 6565 6620 2d73 6175 6572  tuce beef -sauer
+00019c20: 6b72 6175 7420 746f 6d61 746f 222c 205b  kraut tomato", [
+00019c30: 392c 2031 332c 2032 2c20 3131 2c20 3132  9, 13, 2, 11, 12
+00019c40: 2c20 342c 2036 2c20 3130 5d29 2c0a 2020  , 4, 6, 10]),.  
+00019c50: 2020 2020 2020 2020 2020 2822 7069 7a7a            ("pizz
+00019c60: 6120 646f 7567 6820 2d70 696e 6561 7070  a dough -pineapp
+00019c70: 6c65 222c 205b 332c 2034 2c20 325d 292c  le", [3, 4, 2]),
+00019c80: 0a20 2020 2020 2020 2020 2020 2028 2270  .            ("p
+00019c90: 697a 7a61 2064 6f75 6768 202d 2d70 696e  izza dough --pin
+00019ca0: 6561 7070 6c65 222c 205b 332c 2034 5d29  eapple", [3, 4])
+00019cb0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+00019cc0: 6272 6561 6420 6261 636f 6e22 2c20 5b39  bread bacon", [9
+00019cd0: 2c20 352c 2036 2c20 382c 2031 302c 2031  , 5, 6, 8, 10, 1
+00019ce0: 335d 292c 0a20 2020 2020 2020 2020 2020  3]),.           
+00019cf0: 2028 2262 7265 6164 202b 2b62 6163 6f6e   ("bread ++bacon
+00019d00: 222c 205b 392c 2031 335d 292c 0a20 2020  ", [9, 13]),.   
+00019d10: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
+00019d20: 202b 2b61 6e63 686f 7669 6573 222c 205b   ++anchovies", [
+00019d30: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019d40: 2822 6272 6561 6420 2b2b 6261 636f 6e20  ("bread ++bacon 
+00019d50: 2b2b 616e 6368 6f76 6965 7322 2c20 5b5d  ++anchovies", []
+00019d60: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00019d70: 2262 7265 6164 2062 6163 6f6e 202d 2d61  "bread bacon --a
+00019d80: 6e63 686f 7669 6573 222c 205b 392c 2035  nchovies", [9, 5
+00019d90: 2c20 362c 2038 2c20 3130 2c20 3133 5d29  , 6, 8, 10, 13])
+00019da0: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+00019db0: 2020 2020 2020 2020 206d 6174 6368 6573           matches
+00019dc0: 203d 2073 656c 662e 7265 6369 7065 732e   = self.recipes.
+00019dd0: 7365 6172 6368 2e69 6e67 7265 6469 656e  search.ingredien
+00019de0: 7473 2871 7565 7279 2c20 6173 5f74 6162  ts(query, as_tab
+00019df0: 6c65 3d46 616c 7365 2c20 6d69 6e5f 7363  le=False, min_sc
+00019e00: 6f72 653d 2d31 3030 3030 290a 2020 2020  ore=-10000).    
+00019e10: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+00019e20: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+00019e30: 6f72 2072 6563 6970 652c 205f 2069 6e20  or recipe, _ in 
+00019e40: 6d61 7463 6865 735d 0a20 2020 2020 2020  matches].       
+00019e50: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
+00019e60: 7175 6572 7929 2c20 272d 3e27 2c20 5b28  query), '->', [(
+00019e70: 7265 6369 7065 2e69 642c 2073 636f 7265  recipe.id, score
+00019e80: 2920 666f 7220 7265 6369 7065 2c20 7363  ) for recipe, sc
+00019e90: 6f72 6520 696e 206d 6174 6368 6573 5d29  ore in matches])
+00019ea0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00019eb0: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
+00019ec0: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
+00019ed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019ee0: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+00019ef0: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
+00019f00: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00019f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f20: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
+00019f30: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
+00019f40: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
+00019f50: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
+00019f60: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
+00019f70: 290a 0a20 2020 2040 616e 6e6f 756e 6365  )..    @announce
+00019f80: 5f74 6573 740a 2020 2020 6465 6620 7465  _test.    def te
+00019f90: 7374 5f69 6e76 616c 6964 6174 655f 696e  st_invalidate_in
+00019fa0: 6465 7828 7365 6c66 293a 0a20 2020 2020  dex(self):.     
+00019fb0: 2020 2073 656c 662e 7265 6369 7065 732e     self.recipes.
+00019fc0: 706f 7028 3029 0a20 2020 2020 2020 2077  pop(0).        w
+00019fd0: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00019fe0: 6169 7365 7328 6c74 2e53 6561 7263 6849  aises(lt.SearchI
+00019ff0: 6e64 6578 496e 636f 6e73 6973 7465 6e74  ndexInconsistent
+0001a000: 4572 726f 722c 0a20 2020 2020 2020 2020  Error,.         
+0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a020: 2020 2020 2020 6d73 673d 2266 6169 6c65        msg="faile
+0001a030: 6420 746f 2072 6169 7365 2065 7863 6570  d to raise excep
+0001a040: 7469 6f6e 2077 6865 6e20 7365 6172 6368  tion when search
+0001a050: 696e 6720 6d6f 6469 6669 6564 2074 6162  ing modified tab
+0001a060: 6c65 2229 3a0a 2020 2020 2020 2020 2020  le"):.          
+0001a070: 2020 7365 6c66 2e72 6563 6970 6573 2e73    self.recipes.s
+0001a080: 6561 7263 682e 696e 6772 6564 6965 6e74  earch.ingredient
+0001a090: 7328 2262 6163 6f6e 2229 0a0a 2020 2020  s("bacon")..    
+0001a0a0: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+0001a0b0: 2020 2064 6566 2074 6573 745f 7365 6172     def test_sear
+0001a0c0: 6368 5f77 6974 685f 6b65 7977 6f72 6473  ch_with_keywords
+0001a0d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001a0e0: 666f 7220 7175 6572 792c 2065 7870 6563  for query, expec
+0001a0f0: 7465 642c 2065 7870 6563 7465 645f 776f  ted, expected_wo
+0001a100: 7264 7320 696e 205b 0a20 2020 2020 2020  rds in [.       
+0001a110: 2020 2020 2020 2020 2028 2274 756e 6122           ("tuna"
+0001a120: 2c20 5b31 2c20 365d 2c20 5b7b 276e 6f6f  , [1, 6], [{'noo
+0001a130: 646c 6573 272c 2027 6e6f 6f64 6c65 272c  dles', 'noodle',
+0001a140: 2027 7475 6e61 272c 2027 736f 7570 272c   'tuna', 'soup',
+0001a150: 2027 6372 6561 6d27 2c20 276d 7573 6872   'cream', 'mushr
+0001a160: 6f6f 6d27 7d2c 0a20 2020 2020 2020 2020  oom'},.         
+0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a180: 2020 2020 2020 2020 207b 2774 6f6d 6174           {'tomat
+0001a190: 6f27 2c20 2774 756e 6127 2c20 276d 6179  o', 'tuna', 'may
+0001a1a0: 6f6e 6e61 6973 6527 2c20 2762 7265 6164  onnaise', 'bread
+0001a1b0: 272c 2027 6368 6565 7365 277d 5d29 2c0a  ', 'cheese'}]),.
+0001a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1d0: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
+0001a1e0: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
+0001a1f0: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
+0001a200: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
+0001a210: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
+0001a220: 2c20 6173 5f74 6162 6c65 3d46 616c 7365  , as_table=False
+0001a230: 2c20 696e 636c 7564 655f 776f 7264 733d  , include_words=
+0001a240: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0001a250: 2020 6d61 7463 685f 6964 7320 3d20 5b72    match_ids = [r
+0001a260: 6563 6970 652e 6964 2066 6f72 2072 6563  ecipe.id for rec
+0001a270: 6970 652c 2073 636f 7265 2c20 776f 7264  ipe, score, word
+0001a280: 7320 696e 206d 6174 6368 6573 5d0a 2020  s in matches].  
+0001a290: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0001a2a0: 7265 7072 2871 7565 7279 292c 2027 2d3e  repr(query), '->
+0001a2b0: 272c 205b 2872 6563 6970 652e 6964 2c20  ', [(recipe.id, 
+0001a2c0: 7363 6f72 652c 2077 6f72 6473 2920 666f  score, words) fo
+0001a2d0: 7220 7265 6369 7065 2c20 7363 6f72 652c  r recipe, score,
+0001a2e0: 2077 6f72 6473 2069 6e20 6d61 7463 6865   words in matche
+0001a2f0: 735d 290a 2020 2020 2020 2020 2020 2020  s]).            
+0001a300: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0001a310: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0001a320: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001a330: 4571 7561 6c28 6578 7065 6374 6564 2c20  Equal(expected, 
+0001a340: 6d61 7463 685f 6964 732c 0a20 2020 2020  match_ids,.     
+0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a360: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
+0001a370: 7661 6c69 6420 7265 7375 6c74 7320 666f  valid results fo
+0001a380: 7220 7175 6572 7920 7b71 7565 7279 2172  r query {query!r
+0001a390: 7d2c 2065 7870 6563 7465 6420 7b65 7870  }, expected {exp
+0001a3a0: 6563 7465 647d 2c20 676f 7420 7b6d 6174  ected}, got {mat
+0001a3b0: 6368 5f69 6473 7d22 290a 2020 2020 2020  ch_ids}").      
+0001a3c0: 2020 2020 2020 6d61 7463 685f 776f 7264        match_word
+0001a3d0: 7320 3d20 5b73 6574 2877 6f72 6473 2920  s = [set(words) 
+0001a3e0: 666f 7220 7265 6369 7065 2c20 7363 6f72  for recipe, scor
+0001a3f0: 652c 2077 6f72 6473 2069 6e20 6d61 7463  e, words in matc
+0001a400: 6865 735d 0a20 2020 2020 2020 2020 2020  hes].           
+0001a410: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0001a420: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0001a430: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001a440: 7445 7175 616c 2865 7870 6563 7465 645f  tEqual(expected_
+0001a450: 776f 7264 732c 206d 6174 6368 5f77 6f72  words, match_wor
+0001a460: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a480: 2020 2020 2022 696e 7661 6c69 6420 6d61       "invalid ma
+0001a490: 7463 6820 776f 7264 7320 666f 7220 7175  tch words for qu
+0001a4a0: 6572 7920 7b21 727d 2c20 6578 7065 6374  ery {!r}, expect
+0001a4b0: 6564 207b 7d2c 2067 6f74 207b 7d22 2e66  ed {}, got {}".f
+0001a4c0: 6f72 6d61 7428 7175 6572 792c 0a20 2020  ormat(query,.   
+0001a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001a530: 7870 6563 7465 645f 776f 7264 732c 0a20  xpected_words,. 
+0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5a0: 206d 6174 6368 5f77 6f72 6473 2929 0a0a   match_words))..
+0001a5b0: 2020 2020 4061 6e6e 6f75 6e63 655f 7465      @announce_te
+0001a5c0: 7374 0a20 2020 2064 6566 2074 6573 745f  st.    def test_
+0001a5d0: 7365 6172 6368 5f77 6974 685f 6c69 6d69  search_with_limi
+0001a5e0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001a5f0: 2066 6f72 2071 7565 7279 2c20 6578 7065   for query, expe
+0001a600: 6374 6564 2069 6e20 5b0a 2020 2020 2020  cted in [.      
+0001a610: 2020 2020 2020 2822 222c 205b 5d29 2c0a        ("", []),.
+0001a620: 2020 2020 2020 2020 2020 2020 2822 7475              ("tu
+0001a630: 6e61 222c 205b 312c 2036 5d29 2c0a 2020  na", [1, 6]),.  
+0001a640: 2020 2020 2020 2020 2020 2822 7475 6e61            ("tuna
+0001a650: 202b 6368 6565 7365 222c 205b 362c 2033   +cheese", [6, 3
+0001a660: 2c20 345d 292c 0a20 2020 2020 2020 2020  , 4]),.         
+0001a670: 2020 2028 2270 696e 6561 7070 6c65 202b     ("pineapple +
+0001a680: 6261 636f 6e20 6c65 7474 7563 6520 6265  bacon lettuce be
+0001a690: 6566 202d 7361 7565 726b 7261 7574 2074  ef -sauerkraut t
+0001a6a0: 6f6d 6174 6f22 2c20 5b39 2c20 3133 2c20  omato", [9, 13, 
+0001a6b0: 325d 292c 0a20 2020 2020 2020 2020 2020  2]),.           
+0001a6c0: 2028 2270 697a 7a61 2064 6f75 6768 202d   ("pizza dough -
+0001a6d0: 7069 6e65 6170 706c 6522 2c20 5b33 2c20  pineapple", [3, 
+0001a6e0: 342c 2032 5d29 2c0a 2020 2020 2020 2020  4, 2]),.        
+0001a6f0: 2020 2020 2822 7069 7a7a 6120 646f 7567      ("pizza doug
+0001a700: 6820 2d2d 7069 6e65 6170 706c 6522 2c20  h --pineapple", 
+0001a710: 5b33 2c20 345d 292c 0a20 2020 2020 2020  [3, 4]),.       
+0001a720: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
+0001a730: 6f6e 222c 205b 392c 2035 2c20 365d 292c  on", [9, 5, 6]),
+0001a740: 0a20 2020 2020 2020 2020 2020 2028 2262  .            ("b
+0001a750: 7265 6164 202b 2b62 6163 6f6e 222c 205b  read ++bacon", [
+0001a760: 392c 2031 335d 292c 0a20 2020 2020 2020  9, 13]),.       
+0001a770: 2020 2020 2028 2262 7265 6164 202b 2b61       ("bread ++a
+0001a780: 6e63 686f 7669 6573 222c 205b 5d29 2c0a  nchovies", []),.
+0001a790: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
+0001a7a0: 6561 6420 2b2b 6261 636f 6e20 2b2b 616e  ead ++bacon ++an
+0001a7b0: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
+0001a7c0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+0001a7d0: 6164 2062 6163 6f6e 202d 2d61 6e63 686f  ad bacon --ancho
+0001a7e0: 7669 6573 222c 205b 392c 2035 2c20 365d  vies", [9, 5, 6]
+0001a7f0: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
+0001a800: 2020 2020 2020 2020 2020 6d61 7463 6865            matche
+0001a810: 7320 3d20 7365 6c66 2e72 6563 6970 6573  s = self.recipes
+0001a820: 2e73 6561 7263 682e 696e 6772 6564 6965  .search.ingredie
+0001a830: 6e74 7328 7175 6572 792c 2061 735f 7461  nts(query, as_ta
+0001a840: 626c 653d 4661 6c73 652c 206d 696e 5f73  ble=False, min_s
+0001a850: 636f 7265 3d2d 3130 3030 302c 206c 696d  core=-10000, lim
+0001a860: 6974 3d33 290a 2020 2020 2020 2020 2020  it=3).          
+0001a870: 2020 6d61 7463 685f 6964 7320 3d20 5b72    match_ids = [r
+0001a880: 6563 6970 652e 6964 2066 6f72 2072 6563  ecipe.id for rec
+0001a890: 6970 652c 205f 2069 6e20 6d61 7463 6865  ipe, _ in matche
+0001a8a0: 735d 0a20 2020 2020 2020 2020 2020 2070  s].            p
+0001a8b0: 7269 6e74 2872 6570 7228 7175 6572 7929  rint(repr(query)
+0001a8c0: 2c20 272d 3e27 2c20 5b28 7265 6369 7065  , '->', [(recipe
+0001a8d0: 2e69 642c 2073 636f 7265 2920 666f 7220  .id, score) for 
+0001a8e0: 7265 6369 7065 2c20 7363 6f72 6520 696e  recipe, score in
+0001a8f0: 206d 6174 6368 6573 5d29 0a20 2020 2020   matches]).     
+0001a900: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0001a910: 2e73 7562 5465 7374 2871 7565 7279 3d71  .subTest(query=q
+0001a920: 7565 7279 293a 0a20 2020 2020 2020 2020  uery):.         
+0001a930: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001a940: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0001a950: 2c20 6d61 7463 685f 6964 732c 0a20 2020  , match_ids,.   
+0001a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a970: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0001a980: 696e 7661 6c69 6420 7265 7375 6c74 7320  invalid results 
+0001a990: 666f 7220 7175 6572 7920 7b71 7565 7279  for query {query
+0001a9a0: 2172 7d2c 2065 7870 6563 7465 6420 7b65  !r}, expected {e
+0001a9b0: 7870 6563 7465 647d 2c20 676f 7420 7b6d  xpected}, got {m
+0001a9c0: 6174 6368 5f69 6473 7d22 290a 0a20 2020  atch_ids}")..   
+0001a9d0: 2040 616e 6e6f 756e 6365 5f74 6573 740a   @announce_test.
+0001a9e0: 2020 2020 6465 6620 7465 7374 5f73 6561      def test_sea
+0001a9f0: 7263 685f 7769 7468 5f6d 696e 5f73 636f  rch_with_min_sco
+0001aa00: 7265 2873 656c 6629 3a0a 2020 2020 2020  re(self):.      
+0001aa10: 2020 666f 7220 7175 6572 792c 2065 7870    for query, exp
+0001aa20: 6563 7465 6420 696e 205b 0a20 2020 2020  ected in [.     
+0001aa30: 2020 2020 2020 2028 2222 2c20 5b5d 292c         ("", []),
+0001aa40: 0a20 2020 2020 2020 2020 2020 2028 2274  .            ("t
+0001aa50: 756e 6122 2c20 5b5d 292c 0a20 2020 2020  una", []),.     
+0001aa60: 2020 2020 2020 2028 2274 756e 6120 2b63         ("tuna +c
+0001aa70: 6865 6573 6522 2c20 5b36 2c5d 292c 0a20  heese", [6,]),. 
+0001aa80: 2020 2020 2020 2020 2020 2028 2270 696e             ("pin
+0001aa90: 6561 7070 6c65 202b 6261 636f 6e20 6c65  eapple +bacon le
+0001aaa0: 7474 7563 6520 6265 6566 202d 7361 7565  ttuce beef -saue
+0001aab0: 726b 7261 7574 2074 6f6d 6174 6f22 2c20  rkraut tomato", 
+0001aac0: 5b39 2c20 3133 5d29 2c0a 2020 2020 2020  [9, 13]),.      
+0001aad0: 2020 2020 2020 2822 7069 7a7a 6120 646f        ("pizza do
+0001aae0: 7567 6820 2d70 696e 6561 7070 6c65 222c  ugh -pineapple",
+0001aaf0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+0001ab00: 2020 2822 7069 7a7a 6120 646f 7567 6820    ("pizza dough 
+0001ab10: 2d2d 7069 6e65 6170 706c 6522 2c20 5b5d  --pineapple", []
+0001ab20: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001ab30: 2262 7265 6164 2062 6163 6f6e 222c 205b  "bread bacon", [
+0001ab40: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001ab50: 2822 6272 6561 6420 2b2b 6261 636f 6e22  ("bread ++bacon"
+0001ab60: 2c20 5b39 2c5d 292c 0a20 2020 2020 2020  , [9,]),.       
+0001ab70: 2020 2020 2028 2262 7265 6164 202b 2b61       ("bread ++a
+0001ab80: 6e63 686f 7669 6573 222c 205b 5d29 2c0a  nchovies", []),.
+0001ab90: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
+0001aba0: 6561 6420 2b2b 6261 636f 6e20 2b2b 616e  ead ++bacon ++an
+0001abb0: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
+0001abc0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+0001abd0: 6164 2062 6163 6f6e 202d 2d61 6e63 686f  ad bacon --ancho
+0001abe0: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
+0001abf0: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
+0001ac00: 2020 206d 6174 6368 6573 203d 2073 656c     matches = sel
+0001ac10: 662e 7265 6369 7065 732e 7365 6172 6368  f.recipes.search
+0001ac20: 2e69 6e67 7265 6469 656e 7473 2871 7565  .ingredients(que
+0001ac30: 7279 2c20 6173 5f74 6162 6c65 3d46 616c  ry, as_table=Fal
+0001ac40: 7365 2c20 6d69 6e5f 7363 6f72 653d 3130  se, min_score=10
+0001ac50: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+0001ac60: 6d61 7463 685f 6964 7320 3d20 5b72 6563  match_ids = [rec
+0001ac70: 6970 652e 6964 2066 6f72 2072 6563 6970  ipe.id for recip
+0001ac80: 652c 205f 2069 6e20 6d61 7463 6865 735d  e, _ in matches]
+0001ac90: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0001aca0: 6e74 2872 6570 7228 7175 6572 7929 2c20  nt(repr(query), 
+0001acb0: 272d 3e27 2c20 5b28 7265 6369 7065 2e69  '->', [(recipe.i
+0001acc0: 642c 2073 636f 7265 2920 666f 7220 7265  d, score) for re
+0001acd0: 6369 7065 2c20 7363 6f72 6520 696e 206d  cipe, score in m
+0001ace0: 6174 6368 6573 5d29 0a20 2020 2020 2020  atches]).       
+0001acf0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0001ad00: 7562 5465 7374 2871 7565 7279 3d71 7565  ubTest(query=que
+0001ad10: 7279 293a 0a20 2020 2020 2020 2020 2020  ry):.           
+0001ad20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001ad30: 4571 7561 6c28 6578 7065 6374 6564 2c20  Equal(expected, 
+0001ad40: 6d61 7463 685f 6964 732c 0a20 2020 2020  match_ids,.     
+0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad60: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
+0001ad70: 7661 6c69 6420 7265 7375 6c74 7320 666f  valid results fo
+0001ad80: 7220 7175 6572 7920 7b71 7565 7279 2172  r query {query!r
+0001ad90: 7d2c 2065 7870 6563 7465 6420 7b65 7870  }, expected {exp
+0001ada0: 6563 7465 647d 2c20 676f 7420 7b6d 6174  ected}, got {mat
+0001adb0: 6368 5f69 6473 7d22 290a 0a20 2020 2040  ch_ids}")..    @
+0001adc0: 616e 6e6f 756e 6365 5f74 6573 740a 2020  announce_test.  
+0001add0: 2020 6465 6620 7465 7374 5f73 6561 7263    def test_searc
+0001ade0: 685f 7769 7468 5f61 735f 7461 626c 6528  h_with_as_table(
+0001adf0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+0001ae00: 6f72 2071 7565 7279 2c20 6578 7065 6374  or query, expect
+0001ae10: 6564 2069 6e20 5b0a 2020 2020 2020 2020  ed in [.        
+0001ae20: 2020 2020 2822 222c 205b 5d29 2c0a 2020      ("", []),.  
+0001ae30: 2020 2020 2020 2020 2020 2822 7475 6e61            ("tuna
+0001ae40: 222c 205b 5d29 2c0a 2020 2020 2020 2020  ", []),.        
+0001ae50: 2020 2020 2822 7475 6e61 202b 6368 6565      ("tuna +chee
+0001ae60: 7365 222c 205b 362c 5d29 2c0a 2020 2020  se", [6,]),.    
+0001ae70: 2020 2020 2020 2020 2822 7069 6e65 6170          ("pineap
+0001ae80: 706c 6520 2b62 6163 6f6e 206c 6574 7475  ple +bacon lettu
+0001ae90: 6365 2062 6565 6620 2d73 6175 6572 6b72  ce beef -sauerkr
+0001aea0: 6175 7420 746f 6d61 746f 222c 205b 392c  aut tomato", [9,
+0001aeb0: 2031 335d 292c 0a20 2020 2020 2020 2020   13]),.         
+0001aec0: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
+0001aed0: 202d 7069 6e65 6170 706c 6522 2c20 5b5d   -pineapple", []
+0001aee0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001aef0: 2270 697a 7a61 2064 6f75 6768 202d 2d70  "pizza dough --p
+0001af00: 696e 6561 7070 6c65 222c 205b 5d29 2c0a  ineapple", []),.
+0001af10: 2020 2020 2020 2020 2020 2020 2822 6272              ("br
+0001af20: 6561 6420 6261 636f 6e22 2c20 5b5d 292c  ead bacon", []),
+0001af30: 0a20 2020 2020 2020 2020 2020 2028 2262  .            ("b
+0001af40: 7265 6164 202b 2b62 6163 6f6e 222c 205b  read ++bacon", [
+0001af50: 392c 5d29 2c0a 2020 2020 2020 2020 2020  9,]),.          
+0001af60: 2020 2822 6272 6561 6420 2b2b 616e 6368    ("bread ++anch
+0001af70: 6f76 6965 7322 2c20 5b5d 292c 0a20 2020  ovies", []),.   
+0001af80: 2020 2020 2020 2020 2028 2262 7265 6164           ("bread
+0001af90: 202b 2b62 6163 6f6e 202b 2b61 6e63 686f   ++bacon ++ancho
+0001afa0: 7669 6573 222c 205b 5d29 2c0a 2020 2020  vies", []),.    
+0001afb0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+0001afc0: 6261 636f 6e20 2d2d 616e 6368 6f76 6965  bacon --anchovie
+0001afd0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
+0001afe0: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
+0001aff0: 6d61 7463 6865 7320 3d20 7365 6c66 2e72  matches = self.r
+0001b000: 6563 6970 6573 2e73 6561 7263 682e 696e  ecipes.search.in
+0001b010: 6772 6564 6965 6e74 7328 7175 6572 792c  gredients(query,
+0001b020: 206d 696e 5f73 636f 7265 3d31 3030 302c   min_score=1000,
+0001b030: 2061 735f 7461 626c 653d 5472 7565 290a   as_table=True).
+0001b040: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+0001b050: 685f 6964 7320 3d20 5b72 6563 6970 652e  h_ids = [recipe.
+0001b060: 6964 2066 6f72 2072 6563 6970 6520 696e  id for recipe in
+0001b070: 206d 6174 6368 6573 5d0a 2020 2020 2020   matches].      
+0001b080: 2020 2020 2020 7072 696e 7428 7265 7072        print(repr
+0001b090: 2871 7565 7279 292c 2027 2d3e 272c 205b  (query), '->', [
+0001b0a0: 2872 6563 6970 652e 6964 2c20 7265 6369  (recipe.id, reci
+0001b0b0: 7065 2e69 6e67 7265 6469 656e 7473 5f73  pe.ingredients_s
+0001b0c0: 6561 7263 685f 7363 6f72 6529 2066 6f72  earch_score) for
+0001b0d0: 2072 6563 6970 6520 696e 206d 6174 6368   recipe in match
+0001b0e0: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
+0001b0f0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0001b100: 7374 2871 7565 7279 3d71 7565 7279 293a  st(query=query):
+0001b110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b120: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001b130: 6c28 6578 7065 6374 6564 2c20 6d61 7463  l(expected, matc
+0001b140: 685f 6964 732c 0a20 2020 2020 2020 2020  h_ids,.         
+0001b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b160: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
+0001b170: 6420 7265 7375 6c74 7320 666f 7220 7175  d results for qu
+0001b180: 6572 7920 7b71 7565 7279 2172 7d2c 2065  ery {query!r}, e
+0001b190: 7870 6563 7465 6420 7b65 7870 6563 7465  xpected {expecte
+0001b1a0: 647d 2c20 676f 7420 7b6d 6174 6368 5f69  d}, got {match_i
+0001b1b0: 6473 7d22 290a 0a20 2020 2020 2020 2020  ds}")..         
+0001b1c0: 2020 2073 636f 7265 5f61 7474 7220 3d20     score_attr = 
+0001b1d0: 2269 6e67 7265 6469 656e 7473 5f73 6561  "ingredients_sea
+0001b1e0: 7263 685f 7363 6f72 6522 0a20 2020 2020  rch_score".     
+0001b1f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001b200: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
+0001b210: 2020 2020 2020 2020 616c 6c28 0a20 2020          all(.   
+0001b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b230: 2068 6173 6174 7472 286d 6174 6368 6573   hasattr(matches
+0001b240: 2e62 792e 6964 5b6d 6964 5d2c 2073 636f  .by.id[mid], sco
+0001b250: 7265 5f61 7474 7229 0a20 2020 2020 2020  re_attr).       
+0001b260: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001b270: 206d 6964 2069 6e20 6d61 7463 685f 6964   mid in match_id
+0001b280: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001b290: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0001b2a0: 2020 2020 2066 2261 735f 7461 626c 6520       f"as_table 
+0001b2b0: 6469 6420 6e6f 7420 706f 7075 6c61 7465  did not populate
+0001b2c0: 2073 6f6d 6520 7365 6172 6368 2072 6563   some search rec
+0001b2d0: 6f72 6473 2077 6974 6820 7b73 636f 7265  ords with {score
+0001b2e0: 5f61 7474 7221 727d 220a 2020 2020 2020  _attr!r}".      
+0001b2f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001b300: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001b310: 4661 6c73 6528 0a20 2020 2020 2020 2020  False(.         
+0001b320: 2020 2020 2020 2061 6e79 280a 2020 2020         any(.    
+0001b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b340: 6861 7361 7474 7228 7365 6c66 2e72 6563  hasattr(self.rec
+0001b350: 6970 6573 2e62 792e 6964 5b6d 6964 5d2c  ipes.by.id[mid],
+0001b360: 2073 636f 7265 5f61 7474 7229 0a20 2020   score_attr).   
+0001b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b380: 2066 6f72 206d 6964 2069 6e20 6d61 7463   for mid in matc
+0001b390: 685f 6964 730a 2020 2020 2020 2020 2020  h_ids.          
+0001b3a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0001b3b0: 2020 2020 2020 2020 2066 2261 735f 7461           f"as_ta
+0001b3c0: 626c 6520 706f 7075 6c61 7465 6420 736f  ble populated so
+0001b3d0: 6d65 206f 7269 6769 6e61 6c20 7265 636f  me original reco
+0001b3e0: 7264 7320 7769 7468 207b 7363 6f72 655f  rds with {score_
+0001b3f0: 6174 7472 2172 7d22 0a20 2020 2020 2020  attr!r}".       
+0001b400: 2020 2020 2029 0a0a 636c 6173 7320 5461       )..class Ta
+0001b410: 626c 6553 6561 7263 6854 6573 7473 5f44  bleSearchTests_D
+0001b420: 6174 614f 626a 6563 7473 2854 6162 6c65  ataObjects(Table
+0001b430: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+0001b440: 6e67 4461 7461 4f62 6a65 6374 7329 3a0a  ngDataObjects):.
+0001b450: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
+0001b460: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+0001b470: 5f4e 616d 6564 7475 706c 6573 2854 6162  _Namedtuples(Tab
+0001b480: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
+0001b490: 7369 6e67 4e61 6d65 6474 7570 6c65 7329  singNamedtuples)
+0001b4a0: 3a0a 2020 2020 7061 7373 0a0a 636c 6173  :.    pass..clas
+0001b4b0: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
+0001b4c0: 7473 5f54 7970 696e 674e 616d 6564 7475  ts_TypingNamedtu
+0001b4d0: 706c 6573 2854 6162 6c65 5365 6172 6368  ples(TableSearch
+0001b4e0: 5465 7374 732c 2055 7369 6e67 5479 7069  Tests, UsingTypi
+0001b4f0: 6e67 4e61 6d65 6454 7570 6c65 293a 0a20  ngNamedTuple):. 
+0001b500: 2020 2070 6173 730a 0a63 6c61 7373 2054     pass..class T
+0001b510: 6162 6c65 5365 6172 6368 5465 7374 735f  ableSearchTests_
+0001b520: 5479 7069 6e67 5479 7065 6444 6963 7428  TypingTypedDict(
+0001b530: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+0001b540: 2c20 5573 696e 6754 7970 696e 6754 7970  , UsingTypingTyp
+0001b550: 6564 4469 6374 293a 0a20 2020 2070 6173  edDict):.    pas
+0001b560: 730a 0a63 6c61 7373 2054 6162 6c65 5365  s..class TableSe
+0001b570: 6172 6368 5465 7374 735f 536c 6f74 7465  archTests_Slotte
+0001b580: 6428 5461 626c 6553 6561 7263 6854 6573  d(TableSearchTes
+0001b590: 7473 2c20 5573 696e 6753 6c6f 7474 6564  ts, UsingSlotted
+0001b5a0: 4f62 6a65 6374 7329 3a0a 2020 2020 7061  Objects):.    pa
+0001b5b0: 7373 0a0a 636c 6173 7320 5461 626c 6553  ss..class TableS
+0001b5c0: 6561 7263 6854 6573 7473 5f53 696d 706c  earchTests_Simpl
+0001b5d0: 654e 616d 6573 7061 6365 2854 6162 6c65  eNamespace(Table
+0001b5e0: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+0001b5f0: 6e67 5369 6d70 6c65 4e61 6d65 7370 6163  ngSimpleNamespac
+0001b600: 6529 3a0a 2020 2020 7061 7373 0a0a 6966  e):.    pass..if
+0001b610: 2064 6174 6163 6c61 7373 6573 2069 7320   dataclasses is 
+0001b620: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 636c  not None:.    cl
+0001b630: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
+0001b640: 6573 7473 5f44 6174 6163 6c61 7373 6573  ests_Dataclasses
+0001b650: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+0001b660: 732c 2055 7369 6e67 4461 7461 636c 6173  s, UsingDataclas
+0001b670: 7365 7329 3a0a 2020 2020 2020 2020 7061  ses):.        pa
+0001b680: 7373 0a0a 6966 2070 7964 616e 7469 6320  ss..if pydantic 
+0001b690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001b6a0: 2063 6c61 7373 2054 6162 6c65 5365 6172   class TableSear
+0001b6b0: 6368 5465 7374 735f 5079 6461 6e74 6963  chTests_Pydantic
+0001b6c0: 4d6f 6465 6c73 2854 6162 6c65 5365 6172  Models(TableSear
+0001b6d0: 6368 5465 7374 732c 2055 7369 6e67 5079  chTests, UsingPy
+0001b6e0: 6461 6e74 6963 4d6f 6465 6c29 3a0a 2020  danticModel):.  
+0001b6f0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0001b700: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
+0001b710: 6854 6573 7473 5f50 7964 616e 7469 6349  hTests_PydanticI
+0001b720: 6d6d 7574 6162 6c65 4d6f 6465 6c73 2854  mmutableModels(T
+0001b730: 6162 6c65 5365 6172 6368 5465 7374 732c  ableSearchTests,
+0001b740: 2055 7369 6e67 5079 6461 6e74 6963 496d   UsingPydanticIm
+0001b750: 6d75 7461 626c 654d 6f64 656c 293a 0a20  mutableModel):. 
+0001b760: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0001b770: 2063 6c61 7373 2054 6162 6c65 5365 6172   class TableSear
+0001b780: 6368 5465 7374 735f 5079 6461 6e74 6963  chTests_Pydantic
+0001b790: 4f52 4d4d 6f64 656c 7328 5461 626c 6553  ORMModels(TableS
+0001b7a0: 6561 7263 6854 6573 7473 2c20 5573 696e  earchTests, Usin
+0001b7b0: 6750 7964 616e 7469 634f 524d 4d6f 6465  gPydanticORMMode
+0001b7c0: 6c29 3a0a 2020 2020 2020 2020 7061 7373  l):.        pass
+0001b7d0: 0a0a 6966 2061 7474 7220 6973 206e 6f74  ..if attr is not
+0001b7e0: 204e 6f6e 653a 0a20 2020 2063 6c61 7373   None:.    class
+0001b7f0: 2054 6162 6c65 5365 6172 6368 5465 7374   TableSearchTest
+0001b800: 735f 4174 7472 436c 6173 7365 7328 5461  s_AttrClasses(Ta
+0001b810: 626c 6553 6561 7263 6854 6573 7473 2c20  bleSearchTests, 
+0001b820: 5573 696e 6741 7474 7243 6c61 7373 293a  UsingAttrClass):
+0001b830: 0a20 2020 2020 2020 2070 6173 730a 0a69  .        pass..i
+0001b840: 6620 7472 6169 746c 6574 7320 6973 206e  f traitlets is n
+0001b850: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
+0001b860: 7373 2054 6162 6c65 5365 6172 6368 5465  ss TableSearchTe
+0001b870: 7374 735f 5472 6169 746c 6574 7343 6c61  sts_TraitletsCla
+0001b880: 7373 6573 2854 6162 6c65 5365 6172 6368  sses(TableSearch
+0001b890: 5465 7374 732c 2055 7369 6e67 5472 6169  Tests, UsingTrai
+0001b8a0: 746c 6574 7343 6c61 7373 293a 0a20 2020  tletsClass):.   
+0001b8b0: 2020 2020 2070 6173 730a 0a69 6620 536c       pass..if Sl
+0001b8c0: 6f74 7465 6457 6974 6844 6963 7420 6973  ottedWithDict is
+0001b8d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2063   not None:.    c
+0001b8e0: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
+0001b8f0: 5465 7374 735f 536c 6f74 7465 6457 6974  Tests_SlottedWit
+0001b900: 6844 6963 7428 5461 626c 6553 6561 7263  hDict(TableSearc
+0001b910: 6854 6573 7473 2c20 5573 696e 6753 6c6f  hTests, UsingSlo
+0001b920: 7474 6564 5769 7468 4469 6374 4f62 6a65  ttedWithDictObje
+0001b930: 6374 7329 3a0a 2020 2020 2020 2020 7061  cts):.        pa
+0001b940: 7373 0a0a 0a63 6c61 7373 2049 6e69 7469  ss...class Initi
+0001b950: 616c 5465 7374 2875 6e69 7474 6573 742e  alTest(unittest.
+0001b960: 5465 7374 4361 7365 293a 0a20 2020 2066  TestCase):.    f
+0001b970: 726f 6d20 6c69 7474 6c65 7461 626c 6520  rom littletable 
+0001b980: 696d 706f 7274 2028 0a20 2020 2020 2020  import (.       
+0001b990: 205f 5f76 6572 7369 6f6e 5f5f 2061 7320   __version__ as 
+0001b9a0: 6c69 7474 6c65 7461 626c 655f 7665 7273  littletable_vers
+0001b9b0: 696f 6e2c 0a20 2020 2020 2020 205f 5f76  ion,.        __v
+0001b9c0: 6572 7369 6f6e 5f74 696d 655f 5f20 6173  ersion_time__ as
+0001b9d0: 206c 6974 746c 6574 6162 6c65 5f76 6572   littletable_ver
+0001b9e0: 7369 6f6e 5f74 696d 652c 0a20 2020 2020  sion_time,.     
+0001b9f0: 2020 205f 5f76 6572 7369 6f6e 5f69 6e66     __version_inf
+0001ba00: 6f5f 5f20 6173 206c 6974 746c 6574 6162  o__ as littletab
+0001ba10: 6c65 5f76 6572 7369 6f6e 5f69 6e66 6f2c  le_version_info,
+0001ba20: 0a20 2020 2029 0a0a 2020 2020 7072 696e  .    )..    prin
+0001ba30: 7428 0a20 2020 2020 2020 2066 2242 6567  t(.        f"Beg
+0001ba40: 696e 6e69 6e67 2074 6573 7420 6f66 206c  inning test of l
+0001ba50: 6974 746c 6574 6162 6c65 2c20 7665 7273  ittletable, vers
+0001ba60: 696f 6e20 7b6c 6974 746c 6574 6162 6c65  ion {littletable
+0001ba70: 5f76 6572 7369 6f6e 7d2c 207b 6c69 7474  _version}, {litt
+0001ba80: 6c65 7461 626c 655f 7665 7273 696f 6e5f  letable_version_
+0001ba90: 7469 6d65 7d22 2c0a 2020 2020 290a 2020  time}",.    ).  
+0001baa0: 2020 7072 696e 7428 6c69 7474 6c65 7461    print(littleta
+0001bab0: 626c 655f 7665 7273 696f 6e5f 696e 666f  ble_version_info
+0001bac0: 290a 2020 2020 7072 696e 7428 2250 7974  ).    print("Pyt
+0001bad0: 686f 6e20 7665 7273 696f 6e22 2c20 7379  hon version", sy
+0001bae0: 732e 7665 7273 696f 6e29 0a20 2020 2070  s.version).    p
+0001baf0: 7269 6e74 2829 0a0a 0a63 6c61 7373 2053  rint()...class S
+0001bb00: 746f 7261 6765 496e 6465 7065 6e64 656e  torageIndependen
+0001bb10: 7454 6573 7473 2875 6e69 7474 6573 742e  tTests(unittest.
+0001bb20: 5465 7374 4361 7365 293a 0a20 2020 2040  TestCase):.    @
+0001bb30: 616e 6e6f 756e 6365 5f74 6573 740a 2020  announce_test.  
+0001bb40: 2020 6465 6620 7465 7374 5f6e 6f72 6d61    def test_norma
+0001bb50: 6c69 7a65 5f73 7472 2873 656c 6629 3a0a  lize_str(self):.
+0001bb60: 2020 2020 2020 2020 666f 7220 696e 5f77          for in_w
+0001bb70: 6f72 642c 2065 7870 6563 7465 645f 776f  ord, expected_wo
+0001bb80: 7264 2069 6e20 5b0a 2020 2020 2020 2020  rd in [.        
+0001bb90: 2020 2020 2822 6e6f 6368 616e 6765 222c      ("nochange",
+0001bba0: 2022 6e6f 6368 616e 6765 2229 2c0a 2020   "nochange"),.  
+0001bbb0: 2020 2020 2020 2020 2020 2822 546f 4c6f            ("ToLo
+0001bbc0: 7765 7222 2c20 2274 6f6c 6f77 6572 2229  wer", "tolower")
+0001bbd0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+0001bbe0: 492e 422e 4d2e 222c 2022 6962 6d22 292c  I.B.M.", "ibm"),
+0001bbf0: 0a20 2020 2020 2020 2020 2020 2028 2247  .            ("G
+0001bc00: 2e45 2e22 2c20 2267 6522 292c 0a20 2020  .E.", "ge"),.   
+0001bc10: 2020 2020 2020 2020 2028 224d 2e22 2c20           ("M.", 
+0001bc20: 226d 2229 2c0a 2020 2020 2020 2020 2020  "m"),.          
+0001bc30: 2020 2822 4d2e 7879 7a22 2c20 226d 2229    ("M.xyz", "m")
+0001bc40: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+0001bc50: 2a78 7878 2d68 6868 222c 2022 7878 782d  *xxx-hhh", "xxx-
+0001bc60: 6868 6822 292c 0a20 2020 2020 2020 2020  hhh"),.         
+0001bc70: 2020 2028 222b 626c 6168 466f 6f22 2c20     ("+blahFoo", 
+0001bc80: 2262 6c61 6866 6f6f 2229 2c0a 2020 2020  "blahfoo"),.    
+0001bc90: 2020 2020 2020 2020 2320 2822 666f 7865          # ("foxe
+0001bca0: 7322 2c20 2266 6f78 2229 2c0a 2020 2020  s", "fox"),.    
+0001bcb0: 2020 2020 2020 2020 2320 2822 6368 7572          # ("chur
+0001bcc0: 6368 6573 222c 2022 6368 7572 6368 2229  ches", "church")
+0001bcd0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0001bce0: 2822 6472 6573 7365 7322 2c20 2264 7265  ("dresses", "dre
+0001bcf0: 7373 2229 2c0a 2020 2020 2020 2020 5d3a  ss"),.        ]:
+0001bd00: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0001bd10: 6820 7365 6c66 2e73 7562 5465 7374 2869  h self.subTest(i
+0001bd20: 6e5f 776f 7264 293a 0a20 2020 2020 2020  n_word):.       
+0001bd30: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0001bd40: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
+0001bd50: 6564 5f77 6f72 642c 206c 742e 5461 626c  ed_word, lt.Tabl
+0001bd60: 652e 5f6e 6f72 6d61 6c69 7a65 5f77 6f72  e._normalize_wor
+0001bd70: 6428 696e 5f77 6f72 6429 290a 0a20 2020  d(in_word))..   
+0001bd80: 2064 6566 2074 6573 745f 6e6f 726d 616c   def test_normal
+0001bd90: 697a 655f 7374 725f 6765 6e28 7365 6c66  ize_str_gen(self
+0001bda0: 293a 0a20 2020 2020 2020 2066 6f72 2069  ):.        for i
+0001bdb0: 6e5f 776f 7264 2c20 6578 7065 6374 6564  n_word, expected
+0001bdc0: 5f77 6f72 6473 2069 6e20 5b0a 2020 2020  _words in [.    
+0001bdd0: 2020 2020 2020 2020 2822 6e6f 6368 616e          ("nochan
+0001bde0: 6765 222c 205b 226e 6f63 6861 6e67 6522  ge", ["nochange"
+0001bdf0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001be00: 2822 546f 4c6f 7765 7222 2c20 5b22 746f  ("ToLower", ["to
+0001be10: 6c6f 7765 7222 5d29 2c0a 2020 2020 2020  lower"]),.      
+0001be20: 2020 2020 2020 2822 492e 422e 4d2e 222c        ("I.B.M.",
+0001be30: 205b 2269 2e62 2e6d 2e22 2c20 2269 626d   ["i.b.m.", "ibm
+0001be40: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
+0001be50: 2028 2247 2e45 2e22 2c20 5b22 672e 652e   ("G.E.", ["g.e.
+0001be60: 222c 2022 6765 225d 292c 0a20 2020 2020  ", "ge"]),.     
+0001be70: 2020 2020 2020 2028 2241 2e49 2e22 2c20         ("A.I.", 
+0001be80: 5b22 612e 692e 222c 2022 6169 225d 292c  ["a.i.", "ai"]),
+0001be90: 0a20 2020 2020 2020 2020 2020 2028 2241  .            ("A
+0001bea0: 4922 2c20 5b22 6169 225d 292c 0a20 2020  I", ["ai"]),.   
+0001beb0: 2020 2020 2020 2020 2028 224d 2e22 2c20           ("M.", 
+0001bec0: 5b22 6d22 5d29 2c0a 2020 2020 2020 2020  ["m"]),.        
+0001bed0: 2020 2020 2822 6d6d 2e78 797a 222c 205b      ("mm.xyz", [
+0001bee0: 226d 6d22 2c20 226d 6d2e 7879 7a22 2c20  "mm", "mm.xyz", 
+0001bef0: 2278 797a 225d 292c 0a20 2020 2020 2020  "xyz"]),.       
+0001bf00: 2020 2020 2028 224d 4d2e 7879 7a22 2c20       ("MM.xyz", 
+0001bf10: 5b22 6d6d 222c 2022 6d6d 2e78 797a 222c  ["mm", "mm.xyz",
+0001bf20: 2022 7879 7a22 5d29 2c0a 2020 2020 2020   "xyz"]),.      
+0001bf30: 2020 2020 2020 2822 5468 7265 6164 696e        ("Threadin
+0001bf40: 672e 6973 416c 6976 6528 2922 2c20 5b27  g.isAlive()", ['
+0001bf50: 6973 616c 6976 6527 2c20 2774 6872 6561  isalive', 'threa
+0001bf60: 6469 6e67 272c 2027 7468 7265 6164 696e  ding', 'threadin
+0001bf70: 672e 6973 616c 6976 6527 5d29 2c0a 2020  g.isalive']),.  
+0001bf80: 2020 2020 2020 2020 2020 2822 2a78 7878            ("*xxx
+0001bf90: 2d68 6868 222c 205b 2768 6868 272c 2027  -hhh", ['hhh', '
+0001bfa0: 7878 7827 2c20 2778 7878 2d68 6868 275d  xxx', 'xxx-hhh']
+0001bfb0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001bfc0: 222b 626c 6168 466f 6f22 2c20 5b22 626c  "+blahFoo", ["bl
+0001bfd0: 6168 666f 6f22 5d29 2c0a 2020 2020 2020  ahfoo"]),.      
+0001bfe0: 2020 2020 2020 2822 7374 722e 6c73 7472        ("str.lstr
+0001bff0: 6970 222c 205b 226c 7374 7269 7022 2c20  ip", ["lstrip", 
+0001c000: 2273 7472 222c 2022 7374 722e 6c73 7472  "str", "str.lstr
+0001c010: 6970 225d 292c 0a20 2020 2020 2020 2020  ip"]),.         
+0001c020: 2020 2028 2273 7472 2e6c 7374 7269 7028     ("str.lstrip(
+0001c030: 2922 2c20 5b22 6c73 7472 6970 222c 2022  )", ["lstrip", "
+0001c040: 7374 7222 2c20 2273 7472 2e6c 7374 7269  str", "str.lstri
+0001c050: 7022 5d29 2c0a 2020 2020 2020 2020 2020  p"]),.          
+0001c060: 2020 2822 7365 6c66 2e61 7373 6572 7445    ("self.assertE
+0001c070: 7175 616c 7322 2c20 5b22 6173 7365 7274  quals", ["assert
+0001c080: 6571 7561 6c73 222c 2022 7365 6c66 222c  equals", "self",
+0001c090: 2022 7365 6c66 2e61 7373 6572 7465 7175   "self.assertequ
+0001c0a0: 616c 7322 5d29 2c0a 2020 2020 2020 2020  als"]),.        
+0001c0b0: 2020 2020 2822 5465 7374 4361 7365 2e61      ("TestCase.a
+0001c0c0: 7373 6572 7445 7175 616c 7322 2c20 5b22  ssertEquals", ["
+0001c0d0: 6173 7365 7274 6571 7561 6c73 222c 2022  assertequals", "
+0001c0e0: 7465 7374 6361 7365 222c 2022 7465 7374  testcase", "test
+0001c0f0: 6361 7365 2e61 7373 6572 7465 7175 616c  case.assertequal
+0001c100: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
+0001c110: 2020 2822 756e 6974 7465 7374 2e54 6573    ("unittest.Tes
+0001c120: 7443 6173 652e 6173 7365 7274 4571 7561  tCase.assertEqua
+0001c130: 6c73 222c 0a20 2020 2020 2020 2020 2020  ls",.           
+0001c140: 2020 5b22 6173 7365 7274 6571 7561 6c73    ["assertequals
+0001c150: 222c 2022 7465 7374 6361 7365 222c 2022  ", "testcase", "
+0001c160: 756e 6974 7465 7374 222c 2022 756e 6974  unittest", "unit
+0001c170: 7465 7374 2e74 6573 7463 6173 652e 6173  test.testcase.as
+0001c180: 7365 7274 6571 7561 6c73 225d 292c 0a20  sertequals"]),. 
+0001c190: 2020 2020 2020 2020 2020 2028 2266 6f78             ("fox
+0001c1a0: 6573 222c 205b 2266 6f78 222c 2022 666f  es", ["fox", "fo
+0001c1b0: 7865 7322 5d29 2c0a 2020 2020 2020 2020  xes"]),.        
+0001c1c0: 2020 2020 2822 6368 7572 6368 6573 222c      ("churches",
+0001c1d0: 205b 2263 6875 7263 6822 2c20 2263 6875   ["church", "chu
+0001c1e0: 7263 6865 7322 5d29 2c0a 2020 2020 2020  rches"]),.      
+0001c1f0: 2020 2020 2020 2822 6472 6573 7365 7322        ("dresses"
+0001c200: 2c20 5b22 6472 6573 7322 2c20 2264 7265  , ["dress", "dre
+0001c210: 7373 6573 225d 292c 0a20 2020 2020 2020  sses"]),.       
+0001c220: 2020 2020 2028 2264 7265 7373 222c 205b       ("dress", [
+0001c230: 2264 7265 7373 222c 205d 292c 0a20 2020  "dress", ]),.   
+0001c240: 2020 2020 2020 2020 2028 2262 6961 7322           ("bias"
+0001c250: 2c20 5b22 6269 6173 222c 205d 292c 0a20  , ["bias", ]),. 
+0001c260: 2020 2020 2020 2020 2020 2028 2274 6f79             ("toy
+0001c270: 7322 2c20 5b22 746f 7922 2c20 2274 6f79  s", ["toy", "toy
+0001c280: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
+0001c290: 2020 2822 6261 6269 6573 222c 205b 2262    ("babies", ["b
+0001c2a0: 6162 6965 7322 2c20 2262 6162 7922 5d29  abies", "baby"])
+0001c2b0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+0001c2c0: 6164 6465 6e64 6122 2c20 5b22 6164 6465  addenda", ["adde
+0001c2d0: 6e64 6122 2c20 2261 6464 656e 6475 6d22  nda", "addendum"
+0001c2e0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001c2f0: 2822 7261 6269 6573 222c 205b 2272 6162  ("rabies", ["rab
+0001c300: 6965 7322 5d29 2c0a 2020 2020 2020 2020  ies"]),.        
+0001c310: 2020 2020 2822 6c61 7a69 6e65 7373 222c      ("laziness",
+0001c320: 205b 226c 617a 696e 6573 7322 5d29 2c0a   ["laziness"]),.
+0001c330: 2020 2020 2020 2020 2020 2020 2822 7068              ("ph
+0001c340: 7973 6963 7322 2c20 5b22 7068 7973 6963  ysics", ["physic
+0001c350: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
+0001c360: 2020 2822 5079 7468 6f6e 2773 222c 205b    ("Python's", [
+0001c370: 2270 7974 686f 6e22 5d29 2c0a 2020 2020  "python"]),.    
+0001c380: 2020 2020 2020 2020 2827 5661 6c75 6545          ('ValueE
+0001c390: 7272 6f72 272c 205b 2765 7272 6f72 272c  rror', ['error',
+0001c3a0: 2027 7661 6c75 6565 7272 6f72 275d 292c   'valueerror']),
+0001c3b0: 0a20 2020 2020 2020 2020 2020 2028 2744  .            ('D
+0001c3c0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+0001c3d0: 6727 2c20 5b27 6465 7072 6563 6174 696f  g', ['deprecatio
+0001c3e0: 6e77 6172 6e69 6e67 272c 2027 7761 726e  nwarning', 'warn
+0001c3f0: 696e 6727 5d29 2c0a 2020 2020 2020 2020  ing']),.        
+0001c400: 2020 2020 2827 4375 7374 6f6d 4578 6365      ('CustomExce
+0001c410: 7074 696f 6e27 2c20 5b27 6375 7374 6f6d  ption', ['custom
+0001c420: 6578 6365 7074 696f 6e27 2c20 2765 7863  exception', 'exc
+0001c430: 6570 7469 6f6e 275d 292c 0a20 2020 2020  eption']),.     
+0001c440: 2020 2020 2020 2028 2774 6572 726f 7227         ('terror'
+0001c450: 2c20 5b27 7465 7272 6f72 275d 292c 0a20  , ['terror']),. 
+0001c460: 2020 2020 2020 2020 2020 2028 2765 7272             ('err
+0001c470: 6f72 272c 205b 2765 7272 6f72 275d 292c  or', ['error']),
+0001c480: 0a20 2020 2020 2020 205d 3a0a 2020 2020  .        ]:.    
+0001c490: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0001c4a0: 662e 7375 6254 6573 7428 696e 5f77 6f72  f.subTest(in_wor
+0001c4b0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+0001c4c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001c4d0: 7175 616c 2865 7870 6563 7465 645f 776f  qual(expected_wo
+0001c4e0: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
+0001c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c500: 2020 2020 2020 736f 7274 6564 286c 6973        sorted(lis
+0001c510: 7428 6c74 2e54 6162 6c65 2e5f 6e6f 726d  t(lt.Table._norm
+0001c520: 616c 697a 655f 776f 7264 5f67 656e 2869  alize_word_gen(i
+0001c530: 6e5f 776f 7264 2c20 6672 6f7a 656e 7365  n_word, frozense
+0001c540: 7428 2929 2929 290a 0a20 2020 2040 616e  t()))))..    @an
+0001c550: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+0001c560: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
+0001c570: 7a65 5f73 706c 6974 2873 656c 6629 3a0a  ze_split(self):.
+0001c580: 2020 2020 2020 2020 666f 7220 696e 5f73          for in_s
+0001c590: 7472 2c20 6578 7065 6374 6564 5f73 7472  tr, expected_str
+0001c5a0: 5f73 6574 2069 6e20 5b0a 2020 2020 2020  _set in [.      
+0001c5b0: 2020 2020 2020 2822 7374 722e 6c73 7472        ("str.lstr
+0001c5c0: 6970 2829 222c 205b 226c 7374 7269 7022  ip()", ["lstrip"
+0001c5d0: 2c20 2273 7472 222c 2022 7374 722e 6c73  , "str", "str.ls
+0001c5e0: 7472 6970 225d 292c 0a20 2020 2020 2020  trip"]),.       
+0001c5f0: 2020 2020 2028 2273 7472 2e6c 7374 7269       ("str.lstri
+0001c600: 7028 2920 7374 722e 7273 7472 6970 2829  p() str.rstrip()
+0001c610: 222c 205b 226c 7374 7269 7022 2c20 2272  ", ["lstrip", "r
+0001c620: 7374 7269 7022 2c20 2273 7472 222c 2022  strip", "str", "
+0001c630: 7374 722e 6c73 7472 6970 222c 2022 7374  str.lstrip", "st
+0001c640: 722e 7273 7472 6970 225d 292c 0a20 2020  r.rstrip"]),.   
+0001c650: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
+0001c660: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+0001c670: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
+0001c680: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
+0001c690: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
+0001c6a0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001c6b0: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
+0001c6c0: 5f73 7472 293a 0a20 2020 2020 2020 2020  _str):.         
+0001c6d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001c6e0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0001c6f0: 5f73 7472 5f73 6574 2c0a 2020 2020 2020  _str_set,.      
+0001c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c710: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0001c720: 6428 7365 7428 6c74 2e54 6162 6c65 2e5f  d(set(lt.Table._
+0001c730: 6e6f 726d 616c 697a 655f 7370 6c69 7428  normalize_split(
+0001c740: 696e 5f73 7472 2929 2929 0a0a 2020 2020  in_str))))..    
+0001c750: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+0001c760: 2020 2064 6566 2074 6573 745f 706c 7572     def test_plur
+0001c770: 616c 735f 7769 7468 5f74 7261 696c 696e  als_with_trailin
+0001c780: 675f 7075 6e63 7475 6174 696f 6e28 7365  g_punctuation(se
+0001c790: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
+0001c7a0: 2028 6c69 6e65 2c20 6578 7065 6374 6564   (line, expected
+0001c7b0: 2920 696e 205b 0a20 2020 2020 2020 2020  ) in [.         
+0001c7c0: 2020 2028 2749 2063 6f75 6c64 2068 6561     ('I could hea
+0001c7d0: 7220 7468 6520 6261 6269 6573 2063 7269  r the babies cri
+0001c7e0: 6573 2e27 2c20 5b27 6261 6269 6573 272c  es.', ['babies',
+0001c7f0: 2027 6261 6279 272c 2027 636f 756c 6427   'baby', 'could'
+0001c800: 2c20 2763 7269 6573 272c 2027 6372 7927  , 'cries', 'cry'
+0001c810: 2c20 2768 6561 7227 2c20 2769 272c 2027  , 'hear', 'i', '
+0001c820: 7468 6527 5d29 2c0a 2020 2020 2020 2020  the']),.        
+0001c830: 2020 2020 2827 5768 6f20 6172 6520 7468      ('Who are th
+0001c840: 6f73 6520 6261 6269 6573 3f27 2c20 5b27  ose babies?', ['
+0001c850: 6172 6527 2c20 2762 6162 6965 7327 2c20  are', 'babies', 
+0001c860: 2762 6162 7927 2c20 2774 686f 7365 272c  'baby', 'those',
+0001c870: 2027 7768 6f27 5d29 2c0a 2020 2020 2020   'who']),.      
+0001c880: 2020 2020 2020 2822 5768 6f20 746f 6f6b        ("Who took
+0001c890: 2074 6865 2062 6162 6965 7327 2072 6174   the babies' rat
+0001c8a0: 746c 6573 2074 6869 7320 7469 6d65 3f22  tles this time?"
+0001c8b0: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
+0001c8c0: 2762 6162 6965 7327 2c20 2762 6162 7927  'babies', 'baby'
+0001c8d0: 2c20 2772 6174 746c 6527 2c20 2772 6174  , 'rattle', 'rat
+0001c8e0: 746c 6573 272c 2027 7468 6527 2c20 2774  tles', 'the', 't
+0001c8f0: 6869 7327 2c20 2774 696d 6527 2c20 2774  his', 'time', 't
+0001c900: 6f6f 6b27 2c20 2777 686f 275d 292c 0a20  ook', 'who']),. 
+0001c910: 2020 2020 2020 2020 2020 2028 2749 206c             ('I l
+0001c920: 6f76 6520 7468 6573 6520 6361 6b65 7321  ove these cakes!
+0001c930: 272c 205b 2763 616b 6527 2c20 2763 616b  ', ['cake', 'cak
+0001c940: 6573 272c 2027 6927 2c20 276c 6f76 6527  es', 'i', 'love'
+0001c950: 2c20 2774 6865 7365 275d 292c 0a20 2020  , 'these']),.   
+0001c960: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
+0001c970: 6d79 2077 6966 6520 636f 6f6b 732c 2073  my wife cooks, s
+0001c980: 6865 2062 616b 6573 2e27 2c20 5b27 6261  he bakes.', ['ba
+0001c990: 6b65 272c 2027 6261 6b65 7327 2c20 2763  ke', 'bakes', 'c
+0001c9a0: 6f6f 6b27 2c20 2763 6f6f 6b73 272c 2027  ook', 'cooks', '
+0001c9b0: 6d79 272c 2027 7368 6527 2c20 2777 6865  my', 'she', 'whe
+0001c9c0: 6e27 2c20 2777 6966 6527 5d29 2c0a 2020  n', 'wife']),.  
+0001c9d0: 2020 2020 2020 2020 2020 2822 4c65 7427            ("Let'
+0001c9e0: 7320 676f 2073 686f 7070 696e 6720 666f  s go shopping fo
+0001c9f0: 7220 616e 7469 7175 6573 2122 2c20 5b27  r antiques!", ['
+0001ca00: 616e 7469 7175 6527 2c20 2761 6e74 6971  antique', 'antiq
+0001ca10: 7565 7327 2c20 2766 6f72 272c 2027 676f  ues', 'for', 'go
+0001ca20: 272c 2027 6c65 7427 2c20 2773 686f 7070  ', 'let', 'shopp
+0001ca30: 696e 6727 5d29 2c0a 2020 2020 2020 2020  ing']),.        
+0001ca40: 2020 2020 2827 5468 6973 2069 7320 616e      ('This is an
+0001ca50: 2061 6e74 6971 7565 2076 6173 652c 2077   antique vase, w
+0001ca60: 6f72 7468 2074 686f 7573 616e 6473 2127  orth thousands!'
+0001ca70: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
+0001ca80: 2761 6e27 2c20 2761 6e74 6971 7565 272c  'an', 'antique',
+0001ca90: 2027 6973 272c 2027 7468 6973 272c 2027   'is', 'this', '
+0001caa0: 7468 6f75 7361 6e64 272c 2027 7468 6f75  thousand', 'thou
+0001cab0: 7361 6e64 7327 2c20 2776 6173 6527 2c20  sands', 'vase', 
+0001cac0: 2777 6f72 7468 275d 292c 0a20 2020 2020  'worth']),.     
+0001cad0: 2020 2020 2020 2028 2757 6865 6e20 7765         ('When we
+0001cae0: 206d 6565 742c 2079 6f75 2061 7265 2061   meet, you are a
+0001caf0: 2067 6961 6e74 2061 6d6f 6e67 206d 656e   giant among men
+0001cb00: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+0001cb10: 205b 2761 272c 2027 616d 6f6e 6727 2c20   ['a', 'among', 
+0001cb20: 2761 7265 272c 2027 6769 616e 7427 2c20  'are', 'giant', 
+0001cb30: 276d 616e 272c 2027 6d65 6574 272c 2027  'man', 'meet', '
+0001cb40: 6d65 6e27 2c20 2777 6527 2c20 2777 6865  men', 'we', 'whe
+0001cb50: 6e27 2c20 2779 6f75 275d 292c 0a20 2020  n', 'you']),.   
+0001cb60: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
+0001cb70: 7765 2061 7265 2061 6d6f 6e67 206d 656e  we are among men
+0001cb80: 2c20 796f 7520 6172 6520 6120 6769 616e  , you are a gian
+0001cb90: 7420 6d65 6174 6261 6c6c 2e27 2c0a 2020  t meatball.',.  
+0001cba0: 2020 2020 2020 2020 2020 205b 2761 272c             ['a',
+0001cbb0: 2027 616d 6f6e 6727 2c20 2761 7265 272c   'among', 'are',
+0001cbc0: 2027 6172 6527 2c20 2767 6961 6e74 272c   'are', 'giant',
+0001cbd0: 2027 6d61 6e27 2c20 276d 6561 7462 616c   'man', 'meatbal
+0001cbe0: 6c27 2c20 276d 656e 272c 2027 7765 272c  l', 'men', 'we',
+0001cbf0: 2027 7768 656e 272c 2027 796f 7527 5d29   'when', 'you'])
+0001cc00: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+0001cc10: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+0001cc20: 6c66 2e73 7562 5465 7374 286c 696e 6529  lf.subTest(line)
+0001cc30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001cc40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001cc50: 616c 2865 7870 6563 7465 642c 2073 6f72  al(expected, sor
+0001cc60: 7465 6428 6c74 2e54 6162 6c65 2e5f 6e6f  ted(lt.Table._no
+0001cc70: 726d 616c 697a 655f 7370 6c69 7428 6c69  rmalize_split(li
+0001cc80: 6e65 2929 290a 0a0a 6966 205f 5f6e 616d  ne)))...if __nam
+0001cc90: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
+0001cca0: 273a 0a20 2020 2075 6e69 7474 6573 742e  ':.    unittest.
+0001ccb0: 6d61 696e 2829 0a                        main().
```

