# Comparing `tmp/coronagraphoto-1.0.0.tar.gz` & `tmp/coronagraphoto-1.0.1.tar.gz`

## Comparing `coronagraphoto-1.0.0.tar` & `coronagraphoto-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/README.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/sim_star_cor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/input/settings/example.toml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/__init__.py
--rwxr-xr-x   0        0        0    20640 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/coronagraph.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/logger.py
--rw-r--r--   0        0        0    36095 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/observation.py
--rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/observations.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/observing_scenario.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/render_engine.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/settings.py
--rwxr-xr-x   0        0        0    11832 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/src/coronagraphoto/util.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/LICENSE
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 coronagraphoto-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.zenodo.json
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/README.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/sim_star_cor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/input/settings/example.toml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/_version.py
+-rwxr-xr-x   0        0        0    20640 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/coronagraph.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/logger.py
+-rw-r--r--   0        0        0    36095 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/observation.py
+-rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/observations.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/observing_scenario.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/render_engine.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/settings.py
+-rwxr-xr-x   0        0        0    11832 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/src/coronagraphoto/util.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 coronagraphoto-1.0.1/PKG-INFO
```

### Comparing `coronagraphoto-1.0.0/.pre-commit-config.yaml` & `coronagraphoto-1.0.1/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.5.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
-      - id: no-commit-to-branch
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.3.4
     hooks:
       # Run the linter.
       - id: ruff
-        args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
     rev: v3.1.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
         args: []
+  -   repo: https://github.com/pre-commit/mirrors-mypy
+      rev: 'v1.9.0'
+      hooks:
+      -   id: mypy
```

### Comparing `coronagraphoto-1.0.0/CHANGELOG.md` & `coronagraphoto-1.0.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [1.0.1](https://github.com/CoreySpohn/coronagraphoto/compare/v1.0.0...v1.0.1) (2024-04-09)
+
+
+### Bug Fixes
+
+* **main:** Adding zenodo information ([26837e6](https://github.com/CoreySpohn/coronagraphoto/commit/26837e6b894d0380d0dd529506da1cd35d1ccc1d))
+
 ## 1.0.0 (2024-03-22)
 
 
 ### Bug Fixes
 
 * adding dependabot ([5a7fe8e](https://github.com/CoreySpohn/coronagraphoto/commit/5a7fe8e613a436155293495a44fb121d98819f16))
 * Adding workflow ([4f020b2](https://github.com/CoreySpohn/coronagraphoto/commit/4f020b26ce70578127a3560af6947c1d43b1dfaf))
```

### Comparing `coronagraphoto-1.0.0/sim_star_cor.py` & `coronagraphoto-1.0.1/sim_star_cor.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/.github/workflows/publish-to-pypi.yml` & `coronagraphoto-1.0.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/.github/workflows/release-please.yml` & `coronagraphoto-1.0.1/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/input/settings/example.toml` & `coronagraphoto-1.0.1/input/settings/example.toml`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/coronagraph.py` & `coronagraphoto-1.0.1/src/coronagraphoto/coronagraph.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/logger.py` & `coronagraphoto-1.0.1/src/coronagraphoto/logger.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/observation.py` & `coronagraphoto-1.0.1/src/coronagraphoto/observation.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/observations.py` & `coronagraphoto-1.0.1/src/coronagraphoto/observations.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/observing_scenario.py` & `coronagraphoto-1.0.1/src/coronagraphoto/observing_scenario.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/render_engine.py` & `coronagraphoto-1.0.1/src/coronagraphoto/render_engine.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/settings.py` & `coronagraphoto-1.0.1/src/coronagraphoto/settings.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/src/coronagraphoto/util.py` & `coronagraphoto-1.0.1/src/coronagraphoto/util.py`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/.gitignore` & `coronagraphoto-1.0.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -157,7 +157,9 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 input/
 !input/settings/example.toml
+*_version.py
+.DS_Store
```

### Comparing `coronagraphoto-1.0.0/LICENSE` & `coronagraphoto-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coronagraphoto-1.0.0/pyproject.toml` & `coronagraphoto-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -25,20 +25,42 @@
   "numba",
   "pandas",
   "photutils",
   "synphot",
   "tqdm",
   "xarray",
 ]
-
-[tool.hatch.version]
-source = "vcs"
+[project.optional-dependencies]
+dev = ["mypy", "ruff", "pre-comi"]
+docs = [
+  "sphinx",
+  "myst-parser",
+  "sphinx-book-theme",
+  "sphinx-autoapi",
+  "sphinx_autodoc_typehints",
+]
+test = ["nox", "pytest", "hypothesis", "pytest-cov"]
 
 [project.urls]
 Homepage = "https://github.com/CoreySpohn/coronagraphoto"
 Issues = "https://github.com/CoreySpohn/coronagraphoto/issues"
 
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/coronagraphoto/_version.py"
+
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
+
+[tool.ruff]
+select = ["D", "I"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.mypy]
+overrides = [{ module = "toml.*", ignore_missing_imports = true }]
```

