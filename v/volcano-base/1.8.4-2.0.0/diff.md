# Comparing `tmp/volcano_base-1.8.4.tar.gz` & `tmp/volcano_base-2.0.0.tar.gz`

## Comparing `volcano_base-1.8.4.tar` & `volcano_base-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.mise.local.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.mise.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.release-please-manifest.json
--rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 volcano_base-1.8.4/CHANGELOG.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.4/release-please-config.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-1.8.4/requirements-dev.lock
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-1.8.4/requirements.lock
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/dependabot.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/release-please/release-please-config.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/release-please/release-please-manifest.json
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/__init__.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/config.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/cesm2.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/historic_so2.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/down/ob16.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/__init__.py
--rw-r--r--   0        0        0    22142 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/load_c2w_files.py
--rw-r--r--   0        0        0    31469 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/load/load_ob16.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/manipulate/__init__.py
--rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-1.8.4/src/volcano_base/manipulate/time_series.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-1.8.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-1.8.4/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-1.8.4/README.md
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.mise.local.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.mise.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.release-please-manifest.json
+-rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 volcano_base-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.0/release-please-config.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-2.0.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-2.0.0/requirements.lock
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/release-please/release-please-config.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/release-please/release-please-manifest.json
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 volcano_base-2.0.0/assets/examples.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/__init__.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/config.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/cesm2.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/historic_so2.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/ob16.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/__init__.py
+-rw-r--r--   0        0        0    24171 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/load_c2w_files.py
+-rw-r--r--   0        0        0    31469 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/load_ob16.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/manipulate/__init__.py
+-rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/manipulate/time_series.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-2.0.0/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-2.0.0/README.md
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-2.0.0/PKG-INFO
```

### Comparing `volcano_base-1.8.4/.mise.toml` & `volcano_base-2.0.0/.mise.toml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/.pre-commit-config.yaml` & `volcano_base-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/CHANGELOG.md` & `volcano_base-2.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## [2.0.0](https://github.com/engeir/volcano-base/compare/v1.8.4...v2.0.0) (2024-04-09)
+
+
+### ⚠ BREAKING CHANGES
+
+* **cesm load:** use a regex class object to specify files to find
+
+### Features
+
+* **cesm load:** use a regex class object to specify files to find ([793c0a9](https://github.com/engeir/volcano-base/commit/793c0a90b8536eb8b299c12ad0bf692f633d51e7))
+
 ## [1.8.4](https://github.com/engeir/volcano-base/compare/v1.8.3...v1.8.4) (2024-04-08)
 
 
 ### Bug Fixes
 
 * **ob16:** scale colum SO2 so unit adjusts from kg/m2 to Tg (per Earth surface) ([7c82515](https://github.com/engeir/volcano-base/commit/7c8251584e8787d18bc964ead685e86efc5a3ef8))
```

### Comparing `volcano_base-1.8.4/release-please-config.json` & `volcano_base-2.0.0/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/requirements-dev.lock` & `volcano_base-2.0.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/requirements.lock` & `volcano_base-2.0.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/.github/release-please/release-please-config.json` & `volcano_base-2.0.0/.github/release-please/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/.github/workflows/release.yml` & `volcano_base-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/config.py` & `volcano_base-2.0.0/src/volcano_base/config.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/down/cesm2.py` & `volcano_base-2.0.0/src/volcano_base/down/cesm2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/down/historic_so2.py` & `volcano_base-2.0.0/src/volcano_base/down/historic_so2.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/down/ob16.py` & `volcano_base-2.0.0/src/volcano_base/down/ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/load/load_c2w_files.py` & `volcano_base-2.0.0/src/volcano_base/load/load_c2w_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,41 +24,184 @@
             if args
             else "Cannot find the necessary CESM2 files."
         )
         self.message = f"{msg} I went looking in {file.resolve()}. Please run the `save_cesm_files` function within `down.cesm2` to see what files are missing."
         super().__init__(self.message)
 
 
+class RegexLookup:
+    """Create a regex for the files you want to find with FindFiles.
+
+    Parameters
+    ----------
+    ft : str
+        File type that should be found. Default is '.nc'.
+    group_names : dict[str, str]
+        Dictionary with the group names and the corresponding regex group names.
+    reverse_search_query : pathlib.Path
+        Path to the file that should be found using the regex groups.
+    regex : str
+        Regular expression that should be used to find the files.
+
+    Raises
+    ------
+    CESM2FileNotFound
+        If the files cannot be found the hard disk might not be mounted
+    """
+
+    def __init__(
+        self,
+        ft: str,
+        group_names: dict[str, str],
+        reverse_search_query: pathlib.Path,
+        regex: str,
+    ) -> None:
+        self.ft = ft if ft.startswith(".") else f".{ft}"
+        for name in group_names.values():
+            name_ = f"<{name}>"
+            if name_ not in str(reverse_search_query.resolve()):
+                raise ValueError(
+                    "The reverse_search must contain all group_name values and the file type ft."
+                )
+            setattr(self, f"_{name}", set())
+        self.groups = group_names
+        self.reverse_search_query = reverse_search_query
+        self.regex = regex
+        self._combined: set = set()
+        self._bad_files: set[pathlib.Path] = set()
+
+    def search(self) -> None:
+        """Search for files in the root path that match the regular expression."""
+        pattern = re.compile(self.regex + self.ft, re.X)
+        self.root_path = volcano_base.config.DATA_PATH
+        if not self.root_path.exists():
+            raise CESM2FileNotFound()
+        files = self.root_path.rglob(f"**/*{self.ft}")
+        self._initial_file_lookup(files, pattern)
+
+    def reverse_search(self, file_tuple: tuple[str, ...], ft: str) -> pathlib.Path:
+        """Look for file paths using the regex match groups."""
+        # Substitute all instances of group values in the reverse search string
+        this_search = self.reverse_search_query
+        for i, v in enumerate(file_tuple):
+            this_search = pathlib.Path(
+                str(this_search).replace(f"<{list(self.groups.values())[i]}>", v)
+            )
+        this_search = pathlib.Path(str(this_search).replace("<ft>", ft))
+        return self.root_path / this_search
+
+    def _initial_file_lookup(self, files, pattern) -> None:
+        for file in files:
+            if isinstance(search := pattern.search(str(file)), re.Match):
+                for i, v in enumerate(search.groups()):
+                    getattr(self, f"_{list(self.groups.values())[i]}").add(v)
+                self._combined.add(tuple(search.groups()))
+            else:
+                self._bad_files.add(file)
+
+
+def default_regex() -> RegexLookup:
+    """Return a regex object that looks for files using the initial directory hierarchy."""
+    regex = r"""# Match everything up to "ensemble-simulations"
+        .*ensemble-simulations/
+        # Match for compset (group 1)
+        # Create a group of as many charaters as you can find that are in a-z or A-Z
+        # or _ or -, but stop (?, non-greedy) as soon as another character shows up
+        ([a-z,A-Z,0-9,_,-]+?)
+        # Look for forward slash and some number of characters, then a -
+        /\w+-
+        # Match for ensemble (group 2)
+        # Create a group with any number of characters
+        (\w+)
+        # Match a -
+        -
+        # Match for simulation type (group 3)
+        # Same group as above
+        ([a-z,A-Z,0-9,_,-]+?)
+        # Match a /, then any number of special or non-special characters, then a /
+        /.*/
+        # Match for attribute / variable (group 4)
+        # Create a group of some non-zero number of non-special characters
+        (\w+)
+        # Match a -
+        -
+        # Match for frequency (group 5)
+        # Create a group of exactly two characters of any type
+        (..)
+        # Match a -
+        -
+        # Match for date (group 6)
+        # Match exactly 8 digits
+        (\d{8})"""
+    group_names = {
+        "Compsets": "compset",
+        "Ensembles": "ens",
+        "Simulations": "sim",
+        "Attributes": "attr",
+        "Frequencies": "freq",
+        "Dates": "date",
+    }
+    reverse_search = (
+        pathlib.Path("ensemble-simulations")
+        / "<compset>"
+        / "<compset>-<ens>-<sim>"
+        / "aggregate"
+        / "<attr>-<freq>-<date><ft>"
+    )
+    return RegexLookup(".nc", group_names, reverse_search, regex)
+
+
+def nird_archive_regex() -> RegexLookup:
+    """Return a regex object that looks for files using the NIRD archive directory hierarchy."""
+    regex = r"""# Match everything up to "nird-archive"
+        .*nird-archive/
+        (.*)
+        -
+        (.*)
+        -
+        (.*)
+        -
+        (.*)
+        -
+        (.*)
+        -
+        (.*)
+        -
+        (\d{8})"""
+    group_names = {
+        "Compsets": "compset",
+        "Latutude": "latitude",
+        "Simulations": "sim",
+        "Ensembles": "ens",
+        "Attributes": "attr",
+        "Frequencies": "freq",
+        "Dates": "date",
+    }
+    reverse_search = (
+        pathlib.Path("nird-archive")
+        / "<compset>-<latitude>-<sim>-<ens>-<attr>-<freq>-<date><ft>"
+    )
+    return RegexLookup(".nc", group_names, reverse_search, regex)
+
+
 class FindFiles:
     """Find files that match a pre-defined regular expression.
 
     Parameters
     ----------
-    ft : str
-        file type to look for
+    regex : RegexLookup | None
+        A RegexLookup object that contains the regular expression and the groups that
+        should be found.
 
     Attributes
     ----------
-    _compset : set containing all component setups
-    _sim : set containing all simulations
-    _ens : set containing all ensembles
-    _attr : set containing all attributes
-    _freq : set containing all frequencies
-    _date : set containing all dates
-    _combined : set containing all combinations of the above sets that were found
-    _bad_files : files that were candidates but that did not match the regex
     _matched_files : files that have been looked up among the files found with the regex
     _sort_order : tuple with the sorting that is applied to the files
     _sort_reverse : bool stating if the sorting of the files should be reversed
 
-    Raises
-    ------
-    CESM2FileNotFound
-        If the files cannot be found the hard disk might not be mounted
-
     Examples
     --------
     >>> ff = FindFiles()
 
     You find nothing since the date is wrong.
 
     >>> files = ff.find(
@@ -111,62 +254,18 @@
 
     Or print the true file paths
 
     >>> found_paths = matches._re_create_file_paths(*matches.get_files().unwrap())
     >>> # [print(found_path) for found_path in found_paths]
     """
 
-    def __init__(self, ft: str = ".nc"):
-        self._compset: set[str] = set()
-        self._sim: set = set()
-        self._ens: set = set()
-        self._attr: set = set()
-        self._freq: set = set()
-        self._date: set = set()
-        self._combined: set = set()
-        self._bad_files: set[pathlib.Path] = set()
-        self.ft = ft
-        regex = r"""# Match everything up to "ensemble-simulations"
-            .*ensemble-simulations/
-            # Match for compset
-            # Create a group of as many charaters as you can find that are in a-z or A-Z
-            # or _ or -, but stop (?, non-greedy) as soon as another character shows up
-            ([a-z,A-Z,0-9,_,-]+?)
-            # Look for forward slash and some number of characters, then a -
-            /\w+-
-            # Match for ensemble
-            # Create a group with any number of characters
-            (\w+)
-            # Match a -
-            -
-            # Match for simulation type
-            # Same group as above, but we do not accept _ this time
-            ([a-z,A-Z,0-9,_,-]+?)
-            # Match a /, then any number of special or non-special characters, then a /
-            /.*/
-            # Match for attribute / variable
-            # Create a group or some non-zero number of non-special characters
-            (\w+)
-            # Match a -
-            -
-            # Match for frequency
-            # Create a group of exactly two characters of any type
-            (..)
-            # Match a -
-            -
-            # Match for date
-            # Match exactly 8 digits
-            (\d{8})"""
-        pattern = re.compile(regex + self.ft, re.X)
-        self.root_path = pathlib.Path(volcano_base.config.DATA_PATH)
-        if not self.root_path.exists():
-            raise CESM2FileNotFound()
-        files = self.root_path.rglob(f"**/*{self.ft}")
-        self._initial_file_lookup(files, pattern)
-        self._matched_files: list[tuple[str, str, str, str, str, str]] | None = None
+    def __init__(self, regex: RegexLookup | None = None):
+        self.regex = default_regex() if regex is None else regex
+        self.regex.search()
+        self._matched_files: list[tuple[str, ...]] | None = None
         self._sort_order: tuple[str, ...] | None = None
         self._sort_reverse: bool = False
 
     def copy(self) -> Self:
         """Create a shallow copy of this object."""
         # https://stackoverflow.com/a/15774013/10642998
         cls = self.__class__
@@ -188,59 +287,34 @@
         match self.get_files():
             case Success(value):
                 files.extend(str(i) for i in value)
             case Failure(value):
                 files.append(value)
         return f"{head}\n\t{"\n\t".join(files)}"
 
-    def _initial_file_lookup(self, files, pattern) -> None:
-        for file in files:
-            if isinstance(search := pattern.search(str(file)), re.Match):
-                compset, ens, sim, attr, freq, date = search.groups()
-                self._compset.add(compset)
-                self._sim.add(sim)
-                self._ens.add(ens)
-                self._attr.add(attr)
-                self._freq.add(freq)
-                self._date.add(date)
-                self._combined.add((compset, sim, ens, attr, freq, date))
-            else:
-                self._bad_files.add(file)
-
     def avail(self) -> None:
         """Print out all available combinations."""
+        dict_list = [f"{key} ({value})" for key, value in self.regex.groups.items()]
+        longest = max(len(i) + 1 for i in dict_list) // 8 + 1
         for h, s_ in zip(
-            [
-                "Compsets (compset)",
-                "Ensembles (ensemble)",
-                "Simulations (sim)",
-                "Attributes (attr)",
-                "Frequencies (freq)",
-                "Dates (date)",
-            ],
-            [
-                self._compset,
-                self._ens,
-                self._sim,
-                self._attr,
-                self._freq,
-                self._date,
-            ],
+            dict_list,
+            [getattr(self.regex, f"_{name}") for name in self.regex.groups.values()],
             strict=True,
         ):
             s = sorted(s_)
             print(f"{h}:", end="\r")
-            [print(f"\t\t\t{i}") for i in s]
+            tab = "\t" * longest
+            [print(f"{tab}{i}") for i in s]
 
-    def get_files(self) -> Result[list[tuple[str, str, str, str, str, str]], str]:
+    def get_files(self) -> Result[list[tuple[str, ...]], str]:
         """Return the list of matched files.
 
         Returns
         -------
-        Result[list[tuple[str, str, str, str, str, str]], str]
+        Result[list[tuple[str, ...]], str]
             A result type that is a Success or a Failure. Match against it to safely
             obtain the correct output (also see the `print_files()` method)::
 
                 match get_files():
                     case Success(value):
                         [print(v) for v in value]
                     case Failure(value):
@@ -330,22 +404,15 @@
         return ac
 
     def _sort_tup(self, *attributes: str) -> Self:
         """Sort the matched files in the order of their attributes."""
         if self._matched_files is None:
             return self
         # Check that the attributes are valid.
-        lookup = {
-            "compset": 0,
-            "sim": 1,
-            "ensemble": 2,
-            "attr": 3,
-            "freq": 4,
-            "date": 5,
-        }
+        lookup = {v: i for i, v in enumerate(self.regex.groups.values())}
         for a in attributes:
             if a not in lookup.keys():
                 raise AttributeError(
                     "Sorting cannot be done since the sorting parameter is not an"
                     " attribute of all the arrays. Available attributes are\n"
                     f"{list(lookup.keys())}"
                 )
@@ -391,36 +458,33 @@
         for elem in args:
             if isinstance(elem, str):
                 combinations.append([elem])
             else:  # Maaaybe check in an elif for an instance of an iterable, but nahh
                 combinations.append(elem)
         # Find all combinations of the variations of elements we want to find
         prod = list(product(*combinations))
-        out: list[tuple[str, str, str, str, str, str]] = []
+        out: list[tuple[str, ...]] = []
         for prod_tup in prod:
             if found_tups := [
-                tup for tup in self._combined if all(elem in tup for elem in prod_tup)
+                tup
+                for tup in self.regex._combined
+                if all(elem in tup for elem in prod_tup)
             ]:
                 out.extend(iter(found_tups))
         if out:
             self._matched_files = out
             return self
         err_msg = (
             "I could not find any matches for your search, but here are the individual"
             " sets. Try to specify one at the time, of decreasing importance, to narrow"
             " down what files you have available for your use case."
         )
         raise AttributeError(
             err_msg,
-            self._compset,
-            self._ens,
-            self._sim,
-            self._attr,
-            self._freq,
-            self._date,
+            *[getattr(self.regex, f"_{name}") for name in self.regex.groups.values()],
         )
 
     def remove(self, *args: str) -> Self:
         """Remove all files that contain any of the specified groups.
 
         Parameters
         ----------
@@ -468,61 +532,63 @@
         for elem in args:
             if isinstance(elem, str):
                 combinations.append([elem])
             else:  # Maaaybe check in an elif for an instance of an iterable, but nahh
                 combinations.append(elem)
         # Find all combinations of the variations of elements we want to find
         prod = list(product(*combinations))
-        out: list[tuple[str, str, str, str, str, str]] = []
+        out: list[tuple[str, ...]] = []
         for prod_tup in prod:
             if found_tups := [
                 tup
                 for tup in self._matched_files
                 if all(elem in tup for elem in prod_tup)
             ]:
                 out.extend(iter(found_tups))
         self._matched_files = out
         # Make sure we keep the sorting order after the refined selection has been made.
         return self if self._sort_order is None else self._sort_tup(*self._sort_order)
 
     def keep_most_recent(self) -> Self:
-        """Keep only the latest file among identical files."""
+        """Keep only the latest file among identical files.
+
+        This assumes that there is a sorting attribute named 'date' that is available.
+        """
         if self._matched_files is None:
             return self
         sorting = self._sort_order
         reverse = self._sort_reverse
-        self = self.sort(
-            "compset", "ensemble", "sim", "attr", "freq", "date", reverse=True
-        )
+        self = self.sort("date", reverse=True)
         only_recent = []
-        last_file = ("",) * 6
+        last_file = ("",) * len(self.regex.groups)
         if self._matched_files is None:
             return self
         for file in self._matched_files:
             if last_file[:-1] != file[:-1]:
                 only_recent.append(file)
                 last_file = file
         self._matched_files = only_recent
         return self if sorting is None else self.sort(*sorting, reverse=reverse)
 
     def _re_create_file_paths(
         self,
-        *found_files: tuple[str, str, str, str, str, str],
+        *found_files: tuple[str, ...],
         ft: str | None = None,
         check_existance: bool = True,
     ) -> list[pathlib.Path]:
         """Re-create complete file paths based on tuples made from regex groups.
 
         Parameters
         ----------
-        *found_files : tuple[str, str, str, str, str, str]
+        *found_files : tuple[str, ...]
             Any number of tuples that were the output of the
             ``self.find`` method.
         ft : str | None
-            File type that should be returned. Default is '.nc'.
+            File type that should be returned. Default is to use the file type of the
+            regex object.
         check_existance : bool
             Whether to check if the files exists or not
 
         Returns
         -------
         list[pathlib.Path]
             Files that were re-created and that exists are placed in a list and
@@ -530,95 +596,88 @@
 
         Raises
         ------
         FileNotFoundError
             If a file is not found
         """
         if ft is None:
-            ft = self.ft
+            ft = self.regex.ft
         paths: list[pathlib.Path] = []
         for file_tup in found_files:
-            compset, sim, ens, attr, freq, date = file_tup
-            path = pathlib.Path(
-                self.root_path
-                / "ensemble-simulations"
-                / compset
-                / f"{compset}-{ens}-{sim}"
-                / "aggregate"
-                / f"{attr}-{freq}-{date}{ft}"
-            )
+            path = self.regex.reverse_search(file_tup, ft)
             if not path.exists() and check_existance:
                 raise FileNotFoundError(
                     "For some reason, re-creating the file from the regex groups did"
                     " not work! Track this issue down immedeately! The incorrect file"
                     f" path was {path}."
                 )
             paths.append(path)
         return paths
 
     def load(
-        self, *files: tuple[str, str, str, str, str, str], ft: str | None = None
+        self, *files: tuple[str, ...], ft: str | None = None
     ) -> list[xr.DataArray]:
         """Load files into xr.DataArray objects.
 
         Parameters
         ----------
-        *files : tuple[str, str, str, str, str, str]
+        *files : tuple[str, ...]
             Any number of files, represented as tuples with six elements that uniquely
             specify the file path.
         ft : str | None
-            File type that should be returned. Default is '.nc'.
+            File type that should be returned. Default is to use the file type of the
+            regex object.
 
         Returns
         -------
         list[xr.DataArray]
             The same number of objects are returned as was given, but loaded as
             xr.DataArray objects.
 
         Raises
         ------
         ValueError
             If no files have been matched yet, there is no point in loading
         """
         if ft is None:
-            ft = self.ft
-        if not files and self._matched_files is None:
-            raise ValueError("No files have been matched yet.")
-        elif not files and self._matched_files is not None:
-            _files = self._matched_files
-        elif files:
-            _files = list(files)
+            ft = self.regex.ft
+        match files, self._matched_files:
+            case ([], None):
+                raise ValueError("No files have been matched yet.")
+            case ([], list(match_files)):
+                _files = match_files
+            case (files, _):
+                _files = list(files)
         xr_arrs: list[xr.DataArray] = []
         for file in _files:
+            attr_idx = list(self.regex.groups.values()).index("attr")
+            attr = file[attr_idx]
             fp = self._re_create_file_paths(file, ft=ft)[0].resolve()
-            xarr = self._open_xr(fp, file) if ft == ".nc" else self._open_np(fp, file)
-            file_set = {
-                "compset": file[0],
-                "sim": file[1],
-                "ensemble": file[2],
-                "attr": file[3],
-                "freq": file[4],
-                "date": file[5],
-                "file_id": file,
-            }
+            xarr = (
+                self._open_xr(fp, attr)
+                if ft == ".nc"
+                else self._open_np(fp, file, attr)
+            )
+            file_set = {v: file[i] for i, v in enumerate(self.regex.groups.values())}
+            file_set["file_id"] = str(file)
             xarr = xarr.assign_attrs(file_set)
             xr_arrs.append(xarr.chunk({"time": 100}))
         return xr_arrs
 
     @staticmethod
     def _open_xr(fp, file) -> xr.DataArray:
         xset = xr.open_dataset(fp)
-        xarr = getattr(xset, file[3]).assign_attrs(xset.attrs)
+        xarr = getattr(xset, file).assign_attrs(xset.attrs)
         xset.close()
         return xarr
 
     @staticmethod
-    def _open_np(fp, file) -> xr.DataArray:
+    def _open_np(fp, file, attr) -> xr.DataArray:
         with np.load(fp) as f:
             xarr = xr.DataArray(f["data"], dims=["time"], coords={"time": f["times"]})
             file_set = {
-                "long_name": volcano_base.config.DATA_ATTRS[file[3]][0],
-                "units": volcano_base.config.DATA_ATTRS[file[3]][1],
+                "long_name": volcano_base.config.DATA_ATTRS[attr][0],
+                "units": volcano_base.config.DATA_ATTRS[attr][1],
                 "file_id": file,
             }
             xarr = xarr.assign_attrs(file_set)
         return xarr
```

### Comparing `volcano_base-1.8.4/src/volcano_base/load/load_ob16.py` & `volcano_base-2.0.0/src/volcano_base/load/load_ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/manipulate/__init__.py` & `volcano_base-2.0.0/src/volcano_base/manipulate/__init__.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/src/volcano_base/manipulate/time_series.py` & `volcano_base-2.0.0/src/volcano_base/manipulate/time_series.py`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/.gitignore` & `volcano_base-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/LICENSE` & `volcano_base-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_base-1.8.4/README.md` & `volcano_base-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.4</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.0</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

### Comparing `volcano_base-1.8.4/pyproject.toml` & `volcano_base-2.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "volcano-base"
-version = "1.8.4"
+version = "2.0.0"
 description = "Download, find and manipulate volcano and climate related time series"
 authors = [{ name = "engeir", email = "engeir@pm.me" }]
 license = "MIT"
 readme = "README.md"
 requires-python = ">= 3.12"
 dependencies = [
     "returns>=0.22.0",
```

### Comparing `volcano_base-1.8.4/PKG-INFO` & `volcano_base-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: volcano-base
-Version: 1.8.4
+Version: 2.0.0
 Summary: Download, find and manipulate volcano and climate related time series
 Author-email: engeir <engeir@pm.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: cftime>=1.6.3
@@ -19,15 +19,15 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: xarray>=2024.1.1
 Description-Content-Type: text/markdown
 
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v1.8.4</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.0</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

