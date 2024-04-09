# Comparing `tmp/precice-config-visualizer-0.2.0.tar.gz` & `tmp/precice-config-visualizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice-config-visualizer-0.2.0.tar", last modified: Thu Mar 14 13:23:03 2024, max compression
+gzip compressed data, was "precice-config-visualizer-0.2.1.tar", last modified: Tue Apr  9 10:07:45 2024, max compression
```

## Comparing `precice-config-visualizer-0.2.0.tar` & `precice-config-visualizer-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 simonifc (20067) simonifc  (1000)        0 2024-03-14 13:23:03.596766 precice-config-visualizer-0.2.0/
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)    35149 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/LICENSE
--rw-r--r--   0 simonifc (20067) simonifc  (1000)     2921 2024-03-14 13:23:03.596766 precice-config-visualizer-0.2.0/PKG-INFO
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)     1785 2024-03-14 12:49:34.000000 precice-config-visualizer-0.2.0/README.md
-drwxrwxr-x   0 simonifc (20067) simonifc  (1000)        0 2024-03-14 13:23:03.592765 precice-config-visualizer-0.2.0/data/
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)      305 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/data/org.precice.configvisualizer.desktop
-drwxrwxr-x   0 simonifc (20067) simonifc  (1000)        0 2024-03-14 13:23:03.596766 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/
--rw-r--r--   0 simonifc (20067) simonifc  (1000)     2921 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/PKG-INFO
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)      509 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/SOURCES.txt
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)        1 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/dependency_links.txt
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)      159 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/entry_points.txt
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)       26 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/requires.txt
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)       24 2024-03-14 13:23:03.000000 precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/top_level.txt
-drwxrwxr-x   0 simonifc (20067) simonifc  (1000)        0 2024-03-14 13:23:03.596766 precice-config-visualizer-0.2.0/preciceconfigvisualizer/
--rwxrwxr-x   0 simonifc (20067) simonifc  (1000)     1956 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/preciceconfigvisualizer/cli.py
--rwxrwxr-x   0 simonifc (20067) simonifc  (1000)    15688 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/preciceconfigvisualizer/common.py
--rwxrwxr-x   0 simonifc (20067) simonifc  (1000)      633 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/preciceconfigvisualizer/gui.py
--rwxrwxr-x   0 simonifc (20067) simonifc  (1000)    13494 2024-03-12 13:56:24.000000 precice-config-visualizer-0.2.0/preciceconfigvisualizer/window.py
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)     1586 2024-03-12 16:32:51.000000 precice-config-visualizer-0.2.0/pyproject.toml
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)       38 2024-03-14 13:23:03.596766 precice-config-visualizer-0.2.0/setup.cfg
--rw-rw-r--   0 simonifc (20067) simonifc  (1000)       38 2024-03-12 16:02:41.000000 precice-config-visualizer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/data/org.precice.config_visualizer.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 10:07:45.000000 precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15928 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13494 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/preciceconfigvisualizer/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:07:45.196506 precice-config-visualizer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:07:34.000000 precice-config-visualizer-0.2.1/setup.py
```

### Comparing `precice-config-visualizer-0.2.0/LICENSE` & `precice-config-visualizer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.0/PKG-INFO` & `precice-config-visualizer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice-config-visualizer-0.2.0/README.md` & `precice-config-visualizer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.0/precice_config_visualizer.egg-info/PKG-INFO` & `precice-config-visualizer-0.2.1/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice-config-visualizer-0.2.0/preciceconfigvisualizer/cli.py` & `precice-config-visualizer-0.2.1/preciceconfigvisualizer/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     parser.add_argument(
         "--no-watchpoints", action="store_true", help="Do not display watchpoints."
     )
     parser.add_argument(
         "--no-colors", action="store_true", help="Disable colors in the output."
     )
     parser.add_argument(
-        "--margin", default=8, type=int, help="Margin around cluster borders in points."
+        "--margin", default=0, type=int, help="Margin around cluster borders in points."
     )
     parser.add_argument("infile", type=str, help="The XML configuration file.")
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
```

### Comparing `precice-config-visualizer-0.2.0/preciceconfigvisualizer/common.py` & `precice-config-visualizer-0.2.1/preciceconfigvisualizer/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,66 +9,68 @@
 if sys.version_info < (3, 6):
     raise RuntimeError(
         "This program requires python 3.6 or later but you attempted to run it"
         " with python {}.{}".format(sys.version_info.major.sys.version_info.minor)
     )
 
 
-def isTrue(text):
+def isTrue(text: str) -> bool:
     return text.lower() in ["yes", "1", "true", "on"]
 
 
-def quote(text):
+def quote(text: str) -> str:
     return f'"{text}"'
 
 
-def parseXML(content):
+def parseXML(content) -> etree._Element:
     p = etree.XMLParser(recover=True, remove_comments=True)
     return etree.fromstring(content, p)
 
 
-def parseXMLFile(file):
+def parseXMLFile(file: str) -> etree._Element:
     return parseXML(open(file, "rb").read())
 
 
-def addNode(g, name, **attrs):
+def addNode(g: pydot.Graph, name: str, **attrs) -> pydot.Node:
     n = pydot.Node(quote(name), **attrs)
     g.add_node(n)
     return n
 
 
-def addEdge(g, src, dst, **attrs):
+def addEdge(g: pydot.Graph, src: str, dst: str, **attrs) -> pydot.Edge:
     e = pydot.Edge(quote(src), quote(dst), **attrs)
     g.add_edge(e)
     return e
 
 
-def addUniqueEdge(g, src, dst, **attrs):
+def addUniqueEdge(g: pydot.Graph, src: str, dst: str, **attrs) -> pydot.Edge:
     for e in g.get_edge_list():
         es, ed = e.get_source().strip('"'), e.get_destination().strip('"')
         if es == src and ed == dst:
             return e
     e = pydot.Edge(quote(src), quote(dst), **attrs)
     g.add_edge(e)
     return e
 
 
-def getEdge(g, src, dst):
+def getEdge(g: pydot.Graph, src: str, dst: str) -> pydot.Edge | None:
     for e in g.get_edge_list():
         es, ed = e.get_source().strip('"'), e.get_destination().strip('"')
         if es == src and ed == dst:
             return e
     return None
 
 
-def getParticipantNames(solverinterface):
+def getParticipantNames(solverinterface: etree._Element) -> list[str]:
     return [p.attrib["name"] for p in solverinterface.findall("participant")]
 
 
-def getParticipantColor(solverinterface, blackOnly=False):
+def getParticipantColor(
+    solverinterface: str, blackOnly: bool = False
+) -> dict[str, str]:
     names = getParticipantNames(solverinterface)
     colors = None
     if blackOnly:
         colors = cycle(["black"])
     else:
         colorblind = [
             "#0173B2",
@@ -82,15 +84,15 @@
             "#ECE133",
             "#56B4E9",
         ]
         colors = cycle(colorblind)
     return dict(zip(names, colors))
 
 
-def configToGraph(ast, args):
+def configToGraph(ast: etree._Element, args) -> pydot.Graph:
     assert ast.tag == "precice-configuration"
 
     solverinterfaces = ast.findall("solver-interface")
     precice_version = -1
     si_dims = None  # precice v2
 
     assert len(solverinterfaces) in [0, 1]
@@ -253,22 +255,20 @@
                         shape="note",
                         label=quote(f"{wpname}\nat ({wpcoord})"),
                         color=color,
                     )
                     addEdge(participant, wpnode, name, color=color)
 
             # other children
-            mappings = []
             for child in elem.iterchildren():
                 # register mappings
                 if child.tag.startswith("mapping:"):
                     mkind = child.tag[child.tag.find(":") + 1 :]
                     mfrom = name + "-" + child.attrib["from"]
                     mto = name + "-" + child.attrib["to"]
-                    # mappings.append((mfrom, mto, mkind))
                     if args.mappings == "full":
                         addEdge(
                             participant, mfrom, mto, label=quote(mkind), color=color
                         )
                     elif args.mappings == "merged":
                         e = getEdge(participant, mto, mfrom)
                         if e is None:
@@ -428,11 +428,11 @@
     """
     try:
         return streamlike.buffer.read()
     except:
         return streamlike.read()
 
 
-def configFileToDotCode(filename, args):
+def configFileToDotCode(filename: str, args) -> str:
     xml = parseXML(readBinary(open(filename, "rb")))
     g = configToGraph(xml, args)
     return g.to_string()
```

### Comparing `precice-config-visualizer-0.2.0/preciceconfigvisualizer/gui.py` & `precice-config-visualizer-0.2.1/preciceconfigvisualizer/gui.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.0/preciceconfigvisualizer/window.py` & `precice-config-visualizer-0.2.1/preciceconfigvisualizer/window.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-0.2.0/pyproject.toml` & `precice-config-visualizer-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -37,12 +37,19 @@
 [project.scripts]
 precice-config-visualizer = "preciceconfigvisualizer.cli:main"
 
 [project.gui-scripts]
 precice-config-visualizer-gui = "preciceconfigvisualizer.gui:main"
 
 [tool.setuptools]
-data-files = { "share/applications" = ["data/org.precice.configvisualizer.desktop"] }
 packages=["preciceconfigvisualizer"]
 
+[tool.setuptools.data-files]
+"share/applications" = ["data/org.precice.config_visualizer.desktop"]
+"share/metainfo" = ["data/org.precice.config_visualizer.metainfo.xml"]
+"share/icons/hicolor/scalable/apps/" = ["data/org.precice.config_visualizer.svg"]
+
 [tool.setuptools-git-versioning]
 enabled = true
+
+[tool.mypy]
+disable_error_code = "import-untyped"
```

