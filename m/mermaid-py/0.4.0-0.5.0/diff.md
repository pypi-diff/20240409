# Comparing `tmp/mermaid_py-0.4.0.tar.gz` & `tmp/mermaid_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mermaid_py-0.4.0.tar", max compression
+gzip compressed data, was "mermaid_py-0.5.0.tar", max compression
```

## Comparing `mermaid_py-0.4.0.tar` & `mermaid_py-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1093 2024-03-31 17:23:46.983748 mermaid_py-0.4.0/LICENSE
--rw-r--r--   0        0        0     4814 2024-03-31 17:23:46.983748 mermaid_py-0.4.0/README.md
--rw-r--r--   0        0        0      881 2024-03-31 17:24:21.123647 mermaid_py-0.4.0/mermaid/__init__.py
--rw-r--r--   0        0        0     3538 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/_main.py
--rw-r--r--   0        0        0     1286 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/_utils.py
--rw-r--r--   0        0        0        0 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/classdiagram/__init__.py
--rw-r--r--   0        0        0     3167 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/configuration.py
--rw-r--r--   0        0        0     2180 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/erdiagram/__init__.py
--rw-r--r--   0        0        0     3000 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/erdiagram/entity.py
--rw-r--r--   0        0        0     2191 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/erdiagram/link.py
--rw-r--r--   0        0        0     2673 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/flowchart/__init__.py
--rw-r--r--   0        0        0     3592 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/flowchart/link.py
--rw-r--r--   0        0        0     4424 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/flowchart/node.py
--rw-r--r--   0        0        0     1827 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/graph/__init__.py
--rw-r--r--   0        0        0      341 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/icon.py
--rw-r--r--   0        0        0     1888 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/mindmap/__init__.py
--rw-r--r--   0        0        0     3917 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/mindmap/level.py
--rw-r--r--   0        0        0     1868 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/piechart.py
--rw-r--r--   0        0        0     2774 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/reqdiagram/__init__.py
--rw-r--r--   0        0        0     1414 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/reqdiagram/element.py
--rw-r--r--   0        0        0     1285 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/reqdiagram/link.py
--rw-r--r--   0        0        0     2831 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/reqdiagram/requirement.py
--rw-r--r--   0        0        0     2403 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/sequence/__init__.py
--rw-r--r--   0        0        0     4875 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/sequence/element.py
--rw-r--r--   0        0        0     2137 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/sequence/link.py
--rw-r--r--   0        0        0     6100 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/sequence/logic.py
--rw-r--r--   0        0        0     3093 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/statediagram/__init__.py
--rw-r--r--   0        0        0       31 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/statediagram/base.py
--rw-r--r--   0        0        0     5702 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/statediagram/state.py
--rw-r--r--   0        0        0     5483 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/statediagram/transition.py
--rw-r--r--   0        0        0     1547 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/style.py
--rw-r--r--   0        0        0     2007 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/userjourney/__init__.py
--rw-r--r--   0        0        0      233 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/userjourney/actor.py
--rw-r--r--   0        0        0      935 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/userjourney/section.py
--rw-r--r--   0        0        0     1023 2024-03-31 17:23:46.987748 mermaid_py-0.4.0/mermaid/userjourney/task.py
--rw-r--r--   0        0        0      998 2024-03-31 17:24:21.123647 mermaid_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5469 1970-01-01 00:00:00.000000 mermaid_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-09 15:35:48.191144 mermaid_py-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4819 2024-04-09 15:35:48.191144 mermaid_py-0.5.0/README.md
+-rw-r--r--   0        0        0      913 2024-04-09 15:36:25.047381 mermaid_py-0.5.0/mermaid/__init__.py
+-rw-r--r--   0        0        0     4528 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/_main.py
+-rw-r--r--   0        0        0     1286 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/classdiagram/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/configuration.py
+-rw-r--r--   0        0        0     2180 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/erdiagram/__init__.py
+-rw-r--r--   0        0        0     3000 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/erdiagram/entity.py
+-rw-r--r--   0        0        0     2191 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/erdiagram/link.py
+-rw-r--r--   0        0        0     2673 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/flowchart/__init__.py
+-rw-r--r--   0        0        0     3592 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/flowchart/link.py
+-rw-r--r--   0        0        0     4424 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/flowchart/node.py
+-rw-r--r--   0        0        0     1827 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/graph/__init__.py
+-rw-r--r--   0        0        0      341 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/icon.py
+-rw-r--r--   0        0        0     1888 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/mindmap/__init__.py
+-rw-r--r--   0        0        0     3917 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/mindmap/level.py
+-rw-r--r--   0        0        0     1868 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/piechart.py
+-rw-r--r--   0        0        0     2774 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/reqdiagram/__init__.py
+-rw-r--r--   0        0        0     1414 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/reqdiagram/element.py
+-rw-r--r--   0        0        0     1285 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/reqdiagram/link.py
+-rw-r--r--   0        0        0     2831 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/reqdiagram/requirement.py
+-rw-r--r--   0        0        0     2403 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/sequence/__init__.py
+-rw-r--r--   0        0        0     4875 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/sequence/element.py
+-rw-r--r--   0        0        0     2137 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/sequence/link.py
+-rw-r--r--   0        0        0     6100 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/sequence/logic.py
+-rw-r--r--   0        0        0     3093 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/statediagram/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/statediagram/base.py
+-rw-r--r--   0        0        0     5702 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/statediagram/state.py
+-rw-r--r--   0        0        0     5483 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/statediagram/transition.py
+-rw-r--r--   0        0        0     1547 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/style.py
+-rw-r--r--   0        0        0     2007 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/userjourney/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/userjourney/actor.py
+-rw-r--r--   0        0        0      935 2024-04-09 15:35:48.195144 mermaid_py-0.5.0/mermaid/userjourney/section.py
+-rw-r--r--   0        0        0     1023 2024-04-09 15:35:48.199144 mermaid_py-0.5.0/mermaid/userjourney/task.py
+-rw-r--r--   0        0        0      998 2024-04-09 15:36:25.047381 mermaid_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 mermaid_py-0.5.0/PKG-INFO
```

### Comparing `mermaid_py-0.4.0/LICENSE` & `mermaid_py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/README.md` & `mermaid_py-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     <a href="https://pypistats.org/packages/mermaid-py">
         <img src="https://img.shields.io/pypi/dm/mermaid-py"
             alt="Mounthly Download" /></a>
     <a href="https://pypi.org/project/mermaid-py/">
         <img src="https://img.shields.io/pypi/v/mermaid-py.svg?style=flat"
             alt="latest version" /></a>
     <a href="https://pypi.org/project/mermaid-py/">
-        <img src="https://img.shields.io/badge/Python-%E2%89%A53.8-blue"
-            alt="latest version" /></a>
+        <img src="https://img.shields.io/pypi/pyversions/mermaid-py"
+            alt="suported python version" /></a>
 </p>
 
 ## Description
 
 mermaid-py is a dynamic Python library designed to serve as a seamless interface for
 the renowned Mermaid library. Built upon the powerful capabilities of Python, mermaid-py
 empowers developers and data enthusiasts to effortlessly create stunning diagrams, flowcharts,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # Mermaid-py this package works as an interface for the famous mermaid-js
 library that uses scripts to create diagrams.
-   _[_C_o_d_e_ _C_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _L_I_C_E_N_S_E_]_[_M_o_u_n_t_h_l_y_ _D_o_w_n_l_o_a_d_]_[_l_a_t_e_s_t_ _v_e_r_s_i_o_n_]_[_l_a_t_e_s_t
-                                   _v_e_r_s_i_o_n_]
+  _[_C_o_d_e_ _C_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _L_I_C_E_N_S_E_]_[_M_o_u_n_t_h_l_y_ _D_o_w_n_l_o_a_d_]_[_l_a_t_e_s_t_ _v_e_r_s_i_o_n_]_[_s_u_p_o_r_t_e_d
+                                _p_y_t_h_o_n_ _v_e_r_s_i_o_n_]
 ## Description mermaid-py is a dynamic Python library designed to serve as a
 seamless interface for the renowned Mermaid library. Built upon the powerful
 capabilities of Python, mermaid-py empowers developers and data enthusiasts to
 effortlessly create stunning diagrams, flowcharts, and visualizations directly
 within their Python environments. ## Examples first install `mermaid-py` by
 `pip install mermaid-py`. - using `Mermaid` and `Graph` classes: ```python
 import mermaid as md from mermaid.graph import Graph graph: Graph = Graph
```

### Comparing `mermaid_py-0.4.0/mermaid/__init__.py` & `mermaid_py-0.5.0/mermaid/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 
 Functions:
     load(file_path): Load data from a file.
     text_to_snake_case(text): Convert a string of text to snake case.
 """
 from enum import Enum
 
-from ._main import Mermaid
+from ._main import Mermaid, Position
 from ._utils import load, text_to_snake_case
 from .configuration import Config
 from .graph import Graph
 from .icon import Icon
 from .style import Style
 
-__version__: str = '0.4.0'
+__version__: str = '0.5.0'
 
 
 class Direction(Enum):
     """Enum for representing the direction of a Mermaid diagram."""
     LEFT_TO_RIGHT = 'LR'
     RIGHT_TO_LEFT = 'RL'
     TOP_TO_BOTTOM = 'TB'
     BOTTOM_TO_TOP = 'BT'
 
 
-__all__ = ['Mermaid', 'load', 'Direction', 'Graph', 'Style', 'Config', 'Icon']
+__all__ = [
+    'Mermaid', 'load', 'Direction', 'Graph', 'Style', 'Config', 'Icon',
+    'Position'
+]
```

### Comparing `mermaid_py-0.4.0/mermaid/_main.py` & `mermaid_py-0.5.0/mermaid/_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,61 @@
 import base64
+from enum import Enum
 from pathlib import Path
 from typing import Union
 
 import requests
 from requests import Response
 
 from .graph import Graph
 
 
+class Position(Enum):
+    """
+    This class represents the position of the node in a Mermaid diagram.
+    """
+    LEFT = 'left'
+    RIGHT = 'right'
+    CENTER = 'center'
+    NONE = 'none'
+
+
 class Mermaid:
     """
     This class represents a Mermaid diagram.
 
     Attributes:
         _diagram (str): The base64 encoded string of the Mermaid diagram script.
         svg_response (Response): The response from the GET request to the Mermaid SVG API.
         img_response (Response): The response from the GET request to the Mermaid IMG API.
     """
-    def __init__(self, graph: Graph):
+    def __init__(self,
+                 graph: Graph,
+                 position: Union[Position, str] = Position.NONE):
         """
         The constructor for the Mermaid class.
 
         Parameters:
             graph (Graph): The Graph object containing the Mermaid diagram script.
         """
+        self.__position: str = position if isinstance(position,
+                                                      str) else position.value
         self._diagram = self._process_diagram(graph.script)
         self._make_request_to_mermaid()
 
+    def set_position(self, position: Union[Position, str]) -> None:
+        """
+        Set the position of the node in the Mermaid diagram.
+
+        Parameters:
+            position (Union[Position, str]): The position of the node.
+        """
+        self.__position = position if isinstance(position,
+                                                 str) else position.value
+
     @staticmethod
     def _process_diagram(diagram: str) -> str:
         """
         Process the Mermaid diagram script into a base64 encoded string.
 
         Parameters:
             diagram (str): The Mermaid diagram script.
@@ -46,15 +71,17 @@
     def _repr_html_(self) -> str:
         """
         Return the text of the SVG response.
 
         Returns:
             str: The text of the SVG response.
         """
-        return self.svg_response.text
+        if self.__position == Position.NONE.value:
+            return self.svg_response.text
+        return f'<div style="text-align:{self.__position}">{self.svg_response.text}</div>'
 
     def _make_request_to_mermaid(self) -> None:
         """
         Make GET requests to the Mermaid SVG and IMG APIs using
         the base64 encoded string of the Mermaid diagram script.
         """
         self.svg_response: Response = requests.get('https://mermaid.ink/svg/' +
```

### Comparing `mermaid_py-0.4.0/mermaid/_utils.py` & `mermaid_py-0.5.0/mermaid/_utils.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/configuration.py` & `mermaid_py-0.5.0/mermaid/configuration.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/erdiagram/__init__.py` & `mermaid_py-0.5.0/mermaid/erdiagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/erdiagram/entity.py` & `mermaid_py-0.5.0/mermaid/erdiagram/entity.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/erdiagram/link.py` & `mermaid_py-0.5.0/mermaid/erdiagram/link.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/flowchart/__init__.py` & `mermaid_py-0.5.0/mermaid/flowchart/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/flowchart/link.py` & `mermaid_py-0.5.0/mermaid/flowchart/link.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/flowchart/node.py` & `mermaid_py-0.5.0/mermaid/flowchart/node.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/graph/__init__.py` & `mermaid_py-0.5.0/mermaid/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/mindmap/__init__.py` & `mermaid_py-0.5.0/mermaid/mindmap/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/mindmap/level.py` & `mermaid_py-0.5.0/mermaid/mindmap/level.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/piechart.py` & `mermaid_py-0.5.0/mermaid/piechart.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/reqdiagram/__init__.py` & `mermaid_py-0.5.0/mermaid/reqdiagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/reqdiagram/element.py` & `mermaid_py-0.5.0/mermaid/reqdiagram/element.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/reqdiagram/link.py` & `mermaid_py-0.5.0/mermaid/reqdiagram/link.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/reqdiagram/requirement.py` & `mermaid_py-0.5.0/mermaid/reqdiagram/requirement.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/sequence/__init__.py` & `mermaid_py-0.5.0/mermaid/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/sequence/element.py` & `mermaid_py-0.5.0/mermaid/sequence/element.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/sequence/link.py` & `mermaid_py-0.5.0/mermaid/sequence/link.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/sequence/logic.py` & `mermaid_py-0.5.0/mermaid/sequence/logic.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/statediagram/__init__.py` & `mermaid_py-0.5.0/mermaid/statediagram/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/statediagram/state.py` & `mermaid_py-0.5.0/mermaid/statediagram/state.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/statediagram/transition.py` & `mermaid_py-0.5.0/mermaid/statediagram/transition.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/style.py` & `mermaid_py-0.5.0/mermaid/style.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/userjourney/__init__.py` & `mermaid_py-0.5.0/mermaid/userjourney/__init__.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/userjourney/section.py` & `mermaid_py-0.5.0/mermaid/userjourney/section.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/mermaid/userjourney/task.py` & `mermaid_py-0.5.0/mermaid/userjourney/task.py`

 * *Files identical despite different names*

### Comparing `mermaid_py-0.4.0/pyproject.toml` & `mermaid_py-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mermaid-py"
-version = "0.4.0"
+version = "0.5.0"
 description = "A simple interface for the the famous lib mermaid-js to create diagrams."
 authors = ["ouhammmourachid <rachidouhammou21@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mermaid"}]
 exclude = ["mermaid/tests/*.py"]
 repository = "https://github.com/ouhammmourachid/mermaid-py"
 license = "MIT"
@@ -27,15 +27,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [bumpver]
-current_version = "0.4.0"
+current_version = "0.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"$'
 ]
 "mermaid/__init__.py" = [
```

### Comparing `mermaid_py-0.4.0/PKG-INFO` & `mermaid_py-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mermaid-py
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple interface for the the famous lib mermaid-js to create diagrams.
 Home-page: https://mermaidpy.vercel.app
 License: MIT
 Author: ouhammmourachid
 Author-email: rachidouhammou21@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,16 +32,16 @@
     <a href="https://pypistats.org/packages/mermaid-py">
         <img src="https://img.shields.io/pypi/dm/mermaid-py"
             alt="Mounthly Download" /></a>
     <a href="https://pypi.org/project/mermaid-py/">
         <img src="https://img.shields.io/pypi/v/mermaid-py.svg?style=flat"
             alt="latest version" /></a>
     <a href="https://pypi.org/project/mermaid-py/">
-        <img src="https://img.shields.io/badge/Python-%E2%89%A53.8-blue"
-            alt="latest version" /></a>
+        <img src="https://img.shields.io/pypi/pyversions/mermaid-py"
+            alt="suported python version" /></a>
 </p>
 
 ## Description
 
 mermaid-py is a dynamic Python library designed to serve as a seamless interface for
 the renowned Mermaid library. Built upon the powerful capabilities of Python, mermaid-py
 empowers developers and data enthusiasts to effortlessly create stunning diagrams, flowcharts,
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: mermaid-py Version: 0.4.0 Summary: A simple
+Metadata-Version: 2.1 Name: mermaid-py Version: 0.5.0 Summary: A simple
 interface for the the famous lib mermaid-js to create diagrams. Home-page:
 https://mermaidpy.vercel.app License: MIT Author: ouhammmourachid Author-email:
 rachidouhammou21@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: ipython
 (>=8.17.2,<9.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Project-URL:
 Repository, https://github.com/ouhammmourachid/mermaid-py Description-Content-
 Type: text/markdown # Mermaid-py this package works as an interface for the
 famous mermaid-js library that uses scripts to create diagrams.
-   _[_C_o_d_e_ _C_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _L_I_C_E_N_S_E_]_[_M_o_u_n_t_h_l_y_ _D_o_w_n_l_o_a_d_]_[_l_a_t_e_s_t_ _v_e_r_s_i_o_n_]_[_l_a_t_e_s_t
-                                   _v_e_r_s_i_o_n_]
+  _[_C_o_d_e_ _C_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _L_I_C_E_N_S_E_]_[_M_o_u_n_t_h_l_y_ _D_o_w_n_l_o_a_d_]_[_l_a_t_e_s_t_ _v_e_r_s_i_o_n_]_[_s_u_p_o_r_t_e_d
+                                _p_y_t_h_o_n_ _v_e_r_s_i_o_n_]
 ## Description mermaid-py is a dynamic Python library designed to serve as a
 seamless interface for the renowned Mermaid library. Built upon the powerful
 capabilities of Python, mermaid-py empowers developers and data enthusiasts to
 effortlessly create stunning diagrams, flowcharts, and visualizations directly
 within their Python environments. ## Examples first install `mermaid-py` by
 `pip install mermaid-py`. - using `Mermaid` and `Graph` classes: ```python
 import mermaid as md from mermaid.graph import Graph graph: Graph = Graph
```

