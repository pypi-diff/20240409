# Comparing `tmp/liblet-1.7.3.tar.gz` & `tmp/liblet-1.7.4.tar.gz`

## Comparing `liblet-1.7.3.tar` & `liblet-1.7.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/api.rst
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/conf.py
--rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples.ipynb
--rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples.rst
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/index.rst
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/installation.rst
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/stg.svg
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/tree.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_static/custom.css
--rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_static/logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_templates/project.html
--rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_70_0.svg
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_71_0.svg
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_82_0.svg
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_83_0.svg
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_8_0.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.3/src/scripts.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/__init__.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/antlr.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/automaton.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/const.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/decorators.py
--rw-r--r--   0        0        0    20499 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/display.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/grammar.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/llvm.py
--rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/antlr_test.py
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/automaton_test.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/decorators_test.py
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/grammar_test.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/run.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/utils_test.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.3/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.3/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.3/LICENSE-GPL.txt
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.3/README.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/api.rst
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/conf.py
+-rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples.ipynb
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples.rst
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/index.rst
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/installation.rst
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/stg.svg
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/tree.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_static/custom.css
+-rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_static/logo.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_templates/project.html
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_70_0.svg
+-rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_71_0.svg
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_82_0.svg
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_83_0.svg
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_8_0.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.4/src/scripts.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/__init__.py
+-rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/antlr.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/automaton.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/const.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/decorators.py
+-rw-r--r--   0        0        0    20902 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/display.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/grammar.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/llvm.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/antlr_test.py
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/automaton_test.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/decorators_test.py
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/grammar_test.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/run.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/utils_test.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.4/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.4/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.4/LICENSE-GPL.txt
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.4/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.4/PKG-INFO
```

### Comparing `liblet-1.7.3/docs/api.rst` & `liblet-1.7.4/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -197,21 +197,25 @@
 
 This module provides a commodity class to deal with `ANTLR <https://www.antlr.org/>`_ for the Python 3 *target*.
 
 .. currentmodule:: liblet.antlr
 
 .. autoclass:: ANTLR
 
+   .. automethod:: load
+   .. automethod:: save
    .. automethod:: print_grammar
    .. automethod:: context
    .. automethod:: tokens
    .. automethod:: tree
 
 .. autoclass:: AnnotatedTreeWalker
 
+   .. automethod:: load
+   .. automethod:: save
    .. automethod:: catchall
    .. automethod:: register
    .. automethod:: RECOURSE_CHILDREN
    .. automethod:: TREE_CATCHALL
    .. automethod:: TEXT_CATCHALL
 
 LLVM support
```

### Comparing `liblet-1.7.3/docs/conf.py` & `liblet-1.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples.ipynb` & `liblet-1.7.4/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples.rst` & `liblet-1.7.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/index.rst` & `liblet-1.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/installation.rst` & `liblet-1.7.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/stg.svg` & `liblet-1.7.4/docs/stg.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/tree.svg` & `liblet-1.7.4/docs/tree.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/_static/logo.png` & `liblet-1.7.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/_templates/project.html` & `liblet-1.7.4/docs/_templates/project.html`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples_files/examples_70_0.svg` & `liblet-1.7.4/docs/examples_files/examples_70_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples_files/examples_71_0.svg` & `liblet-1.7.4/docs/examples_files/examples_71_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples_files/examples_82_0.svg` & `liblet-1.7.4/docs/examples_files/examples_82_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples_files/examples_83_0.svg` & `liblet-1.7.4/docs/examples_files/examples_83_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/docs/examples_files/examples_8_0.svg` & `liblet-1.7.4/docs/examples_files/examples_8_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/liblet/__init__.py` & `liblet-1.7.4/src/liblet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.7.3'
+__version__ = '1.7.4'
 
 from liblet.antlr import ANTLR, AnnotatedTreeWalker
 from liblet.automaton import (
   Automaton,
   BottomUpInstantaneousDescription,
   InstantaneousDescription,
   TopDownInstantaneousDescription,
@@ -40,14 +40,15 @@
   peek,
   suffixes,
   uc,
   union_of,
   warn,
 )
 
+
 __all__ = [
   '__version__',
   'animate_derivation',
   'AnnotatedTreeWalker',
   'ANTLR',
   'AttrDict',
   'Automaton',
```

### Comparing `liblet-1.7.3/src/liblet/antlr.py` & `liblet-1.7.4/src/liblet/antlr.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,33 +91,33 @@
           self.source[suffix] = inf.read()
         spec = imputil.spec_from_file_location(qn, src_path)
         module = imputil.module_from_spec(spec)
         spec.loader.exec_module(module)
         modules[qn] = module
         setattr(self, suffix, getattr(module, qn))
 
-  def save(self, path):
-    """Saves this grammar to file.
-
-    Args:
-      path (str): the path of the file where to save the grammar.
-    """
-    with open(path, 'w') as ouf:
-      ouf.write(self.grammar)
-
   @classmethod
   def load(cls, path):
     """Loads a grammar from file.
 
     Args:
       path (str): the path of the file where the grammar was saved.
     """
     with open(path) as inf:
       return cls(inf.read())
 
+  def save(self, path):
+    """Saves this grammar to file.
+
+    Args:
+      path (str): the path of the file where to save the grammar.
+    """
+    with open(path, 'w') as ouf:
+      ouf.write(self.grammar)
+
   def print_grammar(self, number_lines=True):  # pragma: nocover
     """Prints the grammar (with line numbers)
 
     Args:
       number_lines (bool): if ``False`` line numbers will not be printed.
     """
     print(  # noqa: T201
```

### Comparing `liblet-1.7.3/src/liblet/automaton.py` & `liblet-1.7.4/src/liblet/automaton.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/liblet/decorators.py` & `liblet-1.7.4/src/liblet/decorators.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/liblet/display.py` & `liblet-1.7.4/src/liblet/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from warnings import warn as wwarn
 
 import svgutils.transform as svg_ttransform
 from graphviz import Digraph
 from IPython.display import HTML, SVG, display
 from ipywidgets import IntSlider, interactive
 
-from liblet.const import ε
+
+from liblet.const import ε, FONT_NAME
 from liblet.grammar import HAIR_SPACE, Derivation, Productions
 from liblet.utils import AttrDict, CYKTable, compose, letstr
 
 
 def _escape(label):
   return sub(r'\]', '&#93;', sub(r'\[', '&#91;', escape(str(label))))
 
@@ -41,101 +42,111 @@
       )
     return other_str(obj)
 
   return mapping_aware_label
 
 
 def mapping_aware_gv_args(obj):
-  return {'shape': 'none', 'margin': '0'} if isinstance(obj, Mapping) else {'margin': '.05'}
+  return (
+    {'shape': 'none', 'margin': '0', 'height': '0', 'width': '0'} if isinstance(obj, Mapping) else {'margin': '.05'}
+  )
 
 
 def make_node_wrapper(
   node_label=None,  # how to produce the node label from the node object
   node_eq='obj',  # how to decide equality between nodes
-  default_gv_args=None,  # how to produce the default gv args from the node object
+  node_gv_args=None,  # how to produce the default gv args from the node object
 ):
   if node_label is None:
     node_label = make_mapping_aware_label()
   elif not callable(node_label):
     raise ValueError('node_label must be either None or a callable')
 
   if node_eq == 'obj':
     node_eq = lambda x, y: x == y
   elif node_eq == 'label':
     node_eq = lambda x, y: node_label(x) == node_label(y)
   elif not callable(node_eq):
     raise ValueError('node_eq must be either "obj", "label" or a callable')
 
-  if default_gv_args is None:
-    default_gv_args = mapping_aware_gv_args
-  elif not callable(default_gv_args):
-    raise ValueError('default_gv_args must be either None or a callable')
+  if node_gv_args is None:
+    node_gv_args = mapping_aware_gv_args
+  elif not callable(node_gv_args):
+    raise ValueError('node_gv_args must be either None or a callable')
 
-  class NodeWrapper:
+  class EHW:
     def __init__(self, obj):
       self.obj = obj
 
     def __eq__(self, other):
+      if not isinstance(other, EHW):
+        return False
       return node_eq(self.obj, other.obj)
 
     def __hash__(self):
       return hash(node_label(self.obj))
 
+  class NodeWrapper(EHW):
+    _wn2gid = {}  # noqa: RUF012
+
+    def __new__(cls, obj):
+      ehw = EHW(obj)
+      if ehw not in cls._wn2gid:
+        intsance = cls._wn2gid[ehw] = super().__new__(cls)
+        intsance._gid = f'N{len(cls._wn2gid)}'
+      return cls._wn2gid[ehw]
+
     def gid(self):
       return self._gid
 
     def label(self):
       return node_label(self.obj)
 
-    def default_gv_args(self):
-      return default_gv_args(self.obj)
+    def gv_args(self):
+      return node_gv_args(self.obj)
 
     def __repr__(self):
       return f'NodeWrapper[obj = {self.obj}, label = {self.label()}, hash = {hash(self)}]'
 
   return NodeWrapper
 
 
 class GVWrapper:
   def __init__(self, gv_graph_args=None, node_wrapper=None):
-    if gv_graph_args is None:
-      gv_graph_args = {}
-    if node_wrapper is None:
-      node_wrapper = make_node_wrapper()
+    gv_graph_args = gv_graph_args or {}
+    gv_graph_args['node_attr'] = {'fontname': f"'{FONT_NAME}'"} | (
+      gv_graph_args['node_attr'] if 'node_attr' in gv_graph_args else {}
+    )
+    gv_graph_args['edge_attr'] = {'fontname': f"'{FONT_NAME}'"} | (
+      gv_graph_args['edge_attr'] if 'edge_attr' in gv_graph_args else {}
+    )
+    node_wrapper = node_wrapper or make_node_wrapper()
     self.G = Digraph(**gv_graph_args)
     self.node_wrapper = node_wrapper
-    self.wn2gid = {}
+    self.nodes = set()
 
   def wrapped_graph(self):
     return self.G
 
-  def _obj2wn(self, obj):
-    wn = self.node_wrapper(obj)
-    if wn not in self.wn2gid:
-      wn._gid = f'N{len(self.wn2gid)}'
-      self.wn2gid[wn] = wn._gid
-      return (wn, True)
-    wn._gid = self.wn2gid[wn]
-    return (wn, False)
-
   def subgraph(self, **args):
     return self.G.subgraph(**args)
 
   def node(self, obj, G=None, gv_args=None):
     if G is None:
       G = self.G
-    wn, new = self._obj2wn(obj)
-    if new:
-      G.node(wn.gid(), wn.label(), **({'fontname': 'Fira Code'} | wn.default_gv_args() | (gv_args or {})))
-    return wn.gid()
+    wn = self.node_wrapper(obj)
+    if wn.gid() not in self.nodes:
+      G.node(wn.gid(), wn.label(), **(wn.gv_args() | (gv_args or {})))
+      self.nodes.add(wn.gid())
+    return wn
 
   def edge(self, objsrc, objdst, G=None, gv_args=None):
     if G is None:
       G = self.G
-    G.edge(self.node(objsrc), self.node(objdst), **({'fontname': 'Fira Code'} | (gv_args or {})))
+    G.edge(self.node(objsrc).gid(), self.node(objdst).gid(), **(gv_args or {}))
 
   def __repr__(self):
     return 'GVWrapper[\n' + indent(str(self.G), '\t') + ']'
 
   def _repr_svg_(self):
     return self.G._repr_image_svg_xml()
 
@@ -212,15 +223,15 @@
   def __init__(self, root, children=None):
     self.root = root
     self.children = list(children) if children else []
     if isinstance(root, Mapping):
       self.attr = AttrDict(root)
 
   def __iter__(self):
-    return iter([self.root * self.children])
+    return iter([self.root, *self.children])
 
   @classmethod
   def from_lol(cls, lol):
     """Builds a tree from a *list of lists*.
 
     A list of lists (lol) is a list recursively defined such that the first element of a lol
     is the tree node content and the following elements are lols.
@@ -258,15 +269,15 @@
       dict(  # noqa: C408
         graph_attr={'nodesep': '.25', 'ranksep': '.25'},
         node_attr={'shape': 'box', 'width': '0', 'height': '0', 'style': 'rounded, setlinewidth(.25)'},
         edge_attr={'dir': 'none'},
       ),
       make_node_wrapper(
         node_label=compose(make_mapping_aware_label(), itemgetter(0)),
-        default_gv_args=compose(mapping_aware_gv_args, itemgetter(0)),
+        node_gv_args=compose(mapping_aware_gv_args, itemgetter(0)),
       ),
     )
 
     def walk(T):
       curr = (T.root, T)
       G.node(curr)
       for child in T.children:
@@ -513,19 +524,19 @@
       dict(  # noqa: C408
         graph_attr={'rankdir': 'LR', 'size': '32'},
         node_attr={'margin': '.05'} if self.large_labels else {},
         engine='dot',
       ),
       make_node_wrapper(
         node_label=make_mapping_aware_label(other_str=partial(letstr, sep=sep)),
-        default_gv_args=lambda X: {'peripheries': '2' if X in self.F else '1'},
+        node_gv_args=lambda X: {'peripheries': '2' if X in self.F else '1'},
       ),
     )
     if self.S is not None:
-      (G.node('', gv_args={'shape': 'point'}),)
+      G.node('', gv_args={'shape': 'point'})
       G.edge('', self.S)
     for X, x, Y in self.transitions:
       G.edge(X, Y, gv_args={'xlabel' if self.large_labels else 'label': x})
     self.G = G
     return G
 
   def _repr_svg_(self):
@@ -561,15 +572,15 @@
   return ui
 
 
 # HTML/SVG stuff
 
 
 def __bordered_table__(content):  # noqa: N807
-  return HTML('<style>td, th {border: 1pt solid lightgray !important ;}</style><table>' + content + '</table>')
+  return HTML(f'<style>td, th {{border: 1pt solid lightgray !important;}} * {{font-family: "{FONT_NAME}";}}</style><table>' + content + '</table>')
 
 
 def resized_svg_repr(obj, width=800, height=600):
   if hasattr(obj, '_repr_image_svg_xml'):
     svg_str = obj._repr_image_svg_xml()
   elif hasattr(obj, '_repr_svg_'):
     svg_str = obj._repr_svg_()
```

### Comparing `liblet-1.7.3/src/liblet/grammar.py` & `liblet-1.7.4/src/liblet/grammar.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/liblet/llvm.py` & `liblet-1.7.4/src/liblet/llvm.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/liblet/utils.py` & `liblet-1.7.4/src/liblet/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections.abc import MutableMapping, Set  #  noqa: PYI025
 from functools import partial, reduce
 from html import escape
 from itertools import chain
 from sys import stderr
 from warnings import warn as wwarn
 
+from liblet.const import FONT_NAME
 
 def suffixes(α):
   for i in range(len(α)):
     yield α[i:]
 
 
 def warn(msg):
@@ -155,14 +156,17 @@
     del self.__store[key]
 
   def __iter__(self):
     return iter(self.__store)
 
   def __len__(self):
     return len(self.__store)
+  
+  def __repr__(self):
+    return f'AttrDict({self.__store})'
 
 
 class Table:
   """A one or two-dimensional *table* able to detect conflicts and with a nice HTML representation, based on :obj:`~collections.defaultdict`."""
 
   DEFAULT_FORMAT = {  # noqa: RUF012
     'cols_sort': False,
@@ -248,15 +252,15 @@
           if c in self.data[r]:
             R.data[r][c] = self.data[r][c]
     return R
 
   def _repr_html_(self):
     def _table(content):
       return (
-        '<style>td, th {border: 1pt solid lightgray !important; text-align: left !important;}</style><table>'
+        f'<style>td, th {{border: 1pt solid lightgray !important; text-align: left !important;}} * {{font-family: "{FONT_NAME}";}}</style><table>'
         + content
         + '</table>'
       )
 
     def _fmt(r, c):
       if c not in self.data[r]:
         return '&nbsp;'
```

### Comparing `liblet-1.7.3/src/tests/antlr_test.py` & `liblet-1.7.4/src/tests/antlr_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/tests/automaton_test.py` & `liblet-1.7.4/src/tests/automaton_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/tests/decorators_test.py` & `liblet-1.7.4/src/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/tests/grammar_test.py` & `liblet-1.7.4/src/tests/grammar_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/src/tests/utils_test.py` & `liblet-1.7.4/src/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/LICENSE-CC.txt` & `liblet-1.7.4/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/LICENSE-GPL.txt` & `liblet-1.7.4/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/README.md` & `liblet-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/pyproject.toml` & `liblet-1.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liblet-1.7.3/PKG-INFO` & `liblet-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liblet
-Version: 1.7.3
+Version: 1.7.4
 Summary: A teaching aid library for formal languages and compiler courses.
 Project-URL: Documentation, https://liblet.readthedocs.io/
 Project-URL: Source code, https://github.com/let-unimi/liblet
 Project-URL: Changelog, https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt
 Project-URL: Bug Tracker, https://github.com/let-unimi/liblet/issues
 Author-email: Massimo Santini <massimo.santini@unimi.it>
 License-File: LICENSE-CC.txt
```

