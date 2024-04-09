# Comparing `tmp/gradio_cofoldinginput-0.0.2.tar.gz` & `tmp/gradio_cofoldinginput-0.0.3.tar.gz`

## Comparing `gradio_cofoldinginput-0.0.2.tar` & `gradio_cofoldinginput-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/heme.sdf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/__init__.py
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/cofoldinginput.py
--rw-r--r--   0        0        0    35656 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/cofoldinginput.pyi
--rw-r--r--   0        0        0  1297566 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/component/index.js
--rw-r--r--   0        0        0    57524 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/css.css
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/heme.json
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/heme.sdf
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/Example.svelte
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/Index.svelte
--rw-r--r--   0        0        0    65457 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/package-lock.json
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/package.json
--rw-r--r--   0        0        0    42621 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/Accordion.svelte
--rw-r--r--   0        0        0    28539 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/Button.svelte
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/Molecule.svelte
--rw-r--r--   0        0        0    28898 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/SearchInput.svelte
--rw-r--r--   0        0        0    26063 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/Sequence.svelte
--rw-r--r--   0        0        0    35882 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/SequenceInput.svelte
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/frontend/shared/style.css
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/.gitignore
--rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/heme.sdf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/__init__.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/cofoldinginput.py
+-rw-r--r--   0        0        0    35656 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/cofoldinginput.pyi
+-rw-r--r--   0        0        0  1297586 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/component/index.js
+-rw-r--r--   0        0        0    57524 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/css.css
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/heme.json
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/heme.sdf
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/Example.svelte
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/Index.svelte
+-rw-r--r--   0        0        0    65457 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/package-lock.json
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/package.json
+-rw-r--r--   0        0        0    42621 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/Accordion.svelte
+-rw-r--r--   0        0        0    28539 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/Button.svelte
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/Molecule.svelte
+-rw-r--r--   0        0        0    28898 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/SearchInput.svelte
+-rw-r--r--   0        0        0    26063 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/Sequence.svelte
+-rw-r--r--   0        0        0    35916 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/SequenceInput.svelte
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/frontend/shared/style.css
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/.gitignore
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 gradio_cofoldinginput-0.0.3/PKG-INFO
```

### Comparing `gradio_cofoldinginput-0.0.2/heme.sdf` & `gradio_cofoldinginput-0.0.3/heme.sdf`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/cofoldinginput.py` & `gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/cofoldinginput.py`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/cofoldinginput.pyi` & `gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/cofoldinginput.pyi`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/component/index.js` & `gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/component/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30518,15 +30518,15 @@
             sequence: "",
             open: !0,
             chain: b
         }), e(0, o);
     }
 
     function C(n) {
-        o.splice(n.detail, 1), e(0, o);
+        o.splice(n.detail, 1), e(0, o), g("updateVals", o);
     }
 
     function L(n) {
         let b = o.find((t) => t.class === "protein").chain;
         if (b === void 0) {
             alert("Please add a protein chain first");
             return;
```

### Comparing `gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/component/style.css` & `gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/backend/gradio_cofoldinginput/templates/example/index.js` & `gradio_cofoldinginput-0.0.3/backend/gradio_cofoldinginput/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/demo/app.py` & `gradio_cofoldinginput-0.0.3/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/demo/css.css` & `gradio_cofoldinginput-0.0.3/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/demo/heme.json` & `gradio_cofoldinginput-0.0.3/demo/heme.json`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/demo/heme.sdf` & `gradio_cofoldinginput-0.0.3/demo/heme.sdf`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/demo/space.py` & `gradio_cofoldinginput-0.0.3/demo/space.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_cofoldinginput`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.2%20-%20orange">  
+<a href="https://pypi.org/project/gradio_cofoldinginput/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_cofoldinginput"></a>  
 </div>
 
 Component to enter protein and DNA sequences + small molecules for cofolding
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
```

### Comparing `gradio_cofoldinginput-0.0.2/frontend/Example.svelte` & `gradio_cofoldinginput-0.0.3/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/Index.svelte` & `gradio_cofoldinginput-0.0.3/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/package-lock.json` & `gradio_cofoldinginput-0.0.3/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/package.json` & `gradio_cofoldinginput-0.0.3/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/Accordion.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/Accordion.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/Button.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/Button.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/Molecule.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/Molecule.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/SearchInput.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/SearchInput.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/Sequence.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/Sequence.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/SequenceInput.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/SequenceInput.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
     vals = vals;
     // console.log(vals);
   }
 
   function remove(event) {
     vals.splice(event.detail, 1);
     vals = vals;
+    dispatch("updateVals", vals);
   }
 
   async function fetchMolecules(pdbId) {
     const url = `https://www.ebi.ac.uk/pdbe/api/pdb/entry/molecules/${pdbId}`;
     try {
       const response = await fetch(url);
       if (!response.ok) {
```

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/Textbox.svelte` & `gradio_cofoldinginput-0.0.3/frontend/shared/Textbox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/frontend/shared/style.css` & `gradio_cofoldinginput-0.0.3/frontend/shared/style.css`

 * *Files identical despite different names*

### Comparing `gradio_cofoldinginput-0.0.2/README.md` & `gradio_cofoldinginput-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # `gradio_cofoldinginput`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.2%20-%20orange">  
+<a href="https://pypi.org/project/gradio_cofoldinginput/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_cofoldinginput"></a>  
 
 Component to enter protein and DNA sequences + small molecules for cofolding
 
 ## Installation
 
 ```bash
 pip install gradio_cofoldinginput
```

### Comparing `gradio_cofoldinginput-0.0.2/pyproject.toml` & `gradio_cofoldinginput-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_cofoldinginput"
-version = "0.0.2"
+version = "0.0.3"
 description = "Component to enter protein and DNA sequences + small molecules for cofolding"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_cofoldinginput/templates", "*.pyi", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates"]
+artifacts = ["/backend/gradio_cofoldinginput/templates", "*.pyi", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates", "backend/gradio_cofoldinginput/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_cofoldinginput"]
```

### Comparing `gradio_cofoldinginput-0.0.2/PKG-INFO` & `gradio_cofoldinginput-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_cofoldinginput
-Version: 0.0.2
+Version: 0.0.3
 Summary: Component to enter protein and DNA sequences + small molecules for cofolding
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: MIT
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 
 # `gradio_cofoldinginput`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.2%20-%20orange">  
+<a href="https://pypi.org/project/gradio_cofoldinginput/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_cofoldinginput"></a>  
 
 Component to enter protein and DNA sequences + small molecules for cofolding
 
 ## Installation
 
 ```bash
 pip install gradio_cofoldinginput
```

