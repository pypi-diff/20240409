# Comparing `tmp/geodynamic-0.0.2.tar.gz` & `tmp/geodynamic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.2.tar", last modified: Fri Apr  5 15:04:12 2024, max compression
+gzip compressed data, was "geodynamic-0.0.3.tar", last modified: Tue Apr  9 12:59:21 2024, max compression
```

## Comparing `geodynamic-0.0.2.tar` & `geodynamic-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.316134 geodynamic-0.0.2/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.2/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 15:04:12.315837 geodynamic-0.0.2/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      272 2024-04-05 12:38:51.000000 geodynamic-0.0.2/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.307218 geodynamic-0.0.2/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.2/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.311744 geodynamic-0.0.2/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.2/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10257 2024-02-21 13:25:22.000000 geodynamic-0.0.2/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    23251 2024-03-01 12:40:39.000000 geodynamic-0.0.2/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12689 2024-03-01 18:21:15.000000 geodynamic-0.0.2/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.2/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    25110 2024-04-05 14:53:52.000000 geodynamic-0.0.2/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.314370 geodynamic-0.0.2/geodynamic/parsers/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:33.000000 geodynamic-0.0.2/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.2/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     5939 2024-04-05 14:57:27.000000 geodynamic-0.0.2/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.2/geodynamic/parsers/short_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-05 15:04:12.315021 geodynamic-0.0.2/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      953 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      542 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       70 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-05 15:04:12.000000 geodynamic-0.0.2/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-05 15:04:12.317354 geodynamic-0.0.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      961 2024-04-05 15:03:53.000000 geodynamic-0.0.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.494100 geodynamic-0.0.3/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.3/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-09 12:59:21.494015 geodynamic-0.0.3/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.481637 geodynamic-0.0.3/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.3/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.491118 geodynamic-0.0.3/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.3/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10290 2024-04-08 16:47:18.000000 geodynamic-0.0.3/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    23251 2024-03-01 12:40:39.000000 geodynamic-0.0.3/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12689 2024-03-01 18:21:15.000000 geodynamic-0.0.3/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.3/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    29798 2024-04-09 12:54:44.000000 geodynamic-0.0.3/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.492970 geodynamic-0.0.3/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.3/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.3/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     6740 2024-04-09 12:40:41.000000 geodynamic-0.0.3/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.3/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.3/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-09 12:59:21.493688 geodynamic-0.0.3/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-09 12:59:21.000000 geodynamic-0.0.3/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-09 12:59:21.494724 geodynamic-0.0.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-08 16:25:07.000000 geodynamic-0.0.3/setup.py
```

### Comparing `geodynamic-0.0.2/PKG-INFO` & `geodynamic-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: manim>=0.18.0
-Requires-Dist: manim-mobject-svg>=0.5.0
+Requires-Dist: pycairo>=1.0.0
 
 # GeoDynamic
 
 ## Installation
 
-```
+```bash
 pip install --upgrade geodynamic
 ```
 
 ## Using
 
-```
+1. Preparing code `test.py`:
+
+```python
 from geodynamic.manim_dynamic import *
 
-class Test(GeoDynamic):
+class TestScene(GeoDynamic):
     def construct(self):       
-        self.loadGeoGebra('./test.ggb')    
-        self.exportSVG('./test_ggb.svg')
+        self.loadGeoGebra('test.ggb', scheme = 'pandora', px_size = [400, 300])    
+        self.exportSVG('test_ggb.svg')
+```
+
+2. Run compilation:
+
+```bash
+manim 'test.py' TestScene
 ```
```

### Comparing `geodynamic-0.0.2/geodynamic/geo/construction.py` & `geodynamic-0.0.3/geodynamic/geo/construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         self.vars = []
         self.elements = [
             Element("xAxis", Line((0, 1), 0), visible=False),
             Element("yAxis", Line((1, 0), 0), visible=False)
         ]
         self.commands = []
         self.state = {} #статус элементов и связи (state[elem_name] = {level, inputs, outputs, built})
+        
+        self.style = {}
 
     def __repr__(self):
         str_out = "-------------------\n[[construction]]:\n"
 
         str_out += "\n[{} phantoms]:".format(len(self.phantoms)) + '\n'
         for key in self.phantoms: str_out += str(key) + ': ' + str(self.phantoms[key]) + '\n'
```

### Comparing `geodynamic-0.0.2/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.3/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.2/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.3/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.2/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.3/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.2/geodynamic/manim_dynamic.py` & `geodynamic-0.0.3/geodynamic/manim_dynamic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,156 @@
 import re
 import numpy as np
 
 from .geo import construction as geo
 from manim import *
-from manim_mobject_svg import *
+from .parsers.svg_parser import *
 from .parsers import short_parser, ggb_parser
 
+import xml.etree.ElementTree as ET
+
 #--------------------------------------------------------------------------
 
-class GeoStyle:
-    def __init__(self, color = 'blue', theme = 'light'):
-        #self.green_light = 'rgb(227, 239, 219)'
-        #self.green = 'rgb(128, 190, 140)'
-
-        if theme == 'dark':
-            self.background = BLACK
-            self.strong = WHITE
-            self.col_gray = '#282828'
-
-            if color == 'white':
-                self.col = '#ffffff'
-                self.col_light = '#333333'
-                self.col_accent = '#db4251'
-                self.col_accent_light = '#68383f'
-            elif color == 'purple':
-                self.background = '#151324'
-                self.col = '#9f9fdd'
-                self.col_light = '#3c3766'
-                self.col_accent = '#db4251'
-                self.col_accent_light = '#542f36'
-                self.col_gray = '#211f2f'
+#стилевик от Пандоры
+style_pandora = {}
 
-        else:
-            self.background = WHITE
-            self.strong = BLACK
+style_pandora['dot'] = {}
+style_pandora['line'] = {}
+style_pandora['angle'] = {}
+style_pandora['strich'] = {}
+style_pandora['color'] = {}
+
+style_pandora['dot']['main'] = 7
+style_pandora['dot']['bold'] = 9
+style_pandora['dot']['aux'] = 5
+
+style_pandora['line']['main'] = 2
+style_pandora['line']['bold'] = 2.5
+style_pandora['line']['aux'] = 1.5
+
+style_pandora['angle']['line'] = 1
+style_pandora['angle']['r_default'] = 12.5
+style_pandora['angle']['r_shift'] = 1.5
+style_pandora['angle']['r_right'] = 10
+
+style_pandora['strich']['len'] = 0.45
+style_pandora['strich']['shift'] = 0.14
+
+style_pandora['color']['black'] = '#000000'
+style_pandora['color']['main'] = '#2581b5'
+style_pandora['color']['light'] = '#bef3fc'
+style_pandora['color']['aux'] = '#000000'
+style_pandora['color']['acc'] = '#ef60ab'
+style_pandora['color']['acc_light'] = '#ffd2ee'
 
-            if color == 'green':
-                self.col = '#80be8c'
-                self.col_light = '#e3efdb'
-                self.col_accent = '#d05456'
-                self.col_accent_light = '#f6e0db'
-            elif color == 'orange':
-                self.col = '#d97c2c'
-                self.col_light = '#fae7ca'
-                self.col_accent = '#72a6d9'
-                self.col_accent_light = '#d8edfb'
-            elif color == 'purple':
-                self.col = '#8670ac'
-                self.col_light = '#e8e3f0'
-                self.col_accent = '#d05456'
-                self.col_accent_light = '#f6e0db'
-            else: #blue
-                self.col = '#6688c2'
-                self.col_light = '#dee7f5'
-                self.col_accent = '#d05456'
-                self.col_accent_light = '#f6e0db'
+def CorrectSVG(svg_path):
+    #tree = ET.parse(svg_path)
 
-            self.col_gray = '#eeeeee'
-            
+    #for elem in tree.findall(f'.//{xmlns}text'):
+    #    elem.set('font-style', 'italic')
 
-        self.dot_size = 0.085
-        self.line_width = 6
+    #tree.write(svg_path, encoding = "UTF-8", xml_declaration = False)
+    return
+
+class GeoStyle:
+    def __init__(self, scheme = 'book', color = 'blue', theme = 'light', px_size = [1920, 1080]):
+        self.dot_size = 0.17   
+        self.line_width = 6   
         self.ang_width = 0.75 * self.line_width
         self.strich_rshift = 0.14
         self.ang_rshift = 0.75 * self.strich_rshift
         self.strich_len = 0.45
+        self.ang_rdefault = 0.8
+        self.ang_right = 0.65
+        
+        self.background = WHITE
+        self.strong = BLACK
+
+        if scheme == 'pandora':            
+            self.convert_pandora_to_manim()
+            
+        else:
+            if theme == 'dark':
+                self.background = BLACK
+                self.strong = WHITE
+                self.col_gray = '#282828'
+
+                if color == 'white':
+                    self.col = '#ffffff'
+                    self.col_light = '#333333'
+                    self.col_accent = '#db4251'
+                    self.col_accent_light = '#68383f'
+                elif color == 'purple':
+                    self.background = '#151324'
+                    self.col = '#9f9fdd'
+                    self.col_light = '#3c3766'
+                    self.col_accent = '#db4251'
+                    self.col_accent_light = '#542f36'
+                    self.col_gray = '#211f2f'
+
+            else:
+                self.background = WHITE
+                self.strong = BLACK
+
+                if color == 'green':
+                    self.col = '#80be8c'
+                    self.col_light = '#e3efdb'
+                    self.col_accent = '#d05456'
+                    self.col_accent_light = '#f6e0db'
+                elif color == 'orange':
+                    self.col = '#d97c2c'
+                    self.col_light = '#fae7ca'
+                    self.col_accent = '#72a6d9'
+                    self.col_accent_light = '#d8edfb'
+                elif color == 'purple':
+                    self.col = '#8670ac'
+                    self.col_light = '#e8e3f0'
+                    self.col_accent = '#d05456'
+                    self.col_accent_light = '#f6e0db'
+                else: #blue
+                    self.col = '#6688c2'
+                    self.col_light = '#dee7f5'
+                    self.col_accent = '#d05456'
+                    self.col_accent_light = '#f6e0db'
+
+                self.col_gray = '#eeeeee'
+        
+        #параметры окна отображения 
+        # размеры width и height в px
+        # положение начала координат xZero и yZero
+        # масштаб scale в px для 0.5 unit
+        self.view = {}
+        if px_size is not None:
+            self.view['width'], self.view['height'] = px_size[0], px_size[1]
+
+    def convert_pandora_to_manim(self):
+        self.dot_size = 0.02 * style_pandora['dot']['main']
+        self.line_width = 2 * style_pandora['line']['main']
+        self.ang_width = 2 * style_pandora['angle']['line']
+        self.ang_rshift = 2 * style_pandora['angle']['r_shift']
+        self.ang_rdefault = 0.02 * style_pandora['angle']['r_default']
+        self.ang_right = 0.02 * style_pandora['angle']['r_right']
+        self.strich_len = 2 * style_pandora['strich']['len']
+        self.strich_rshift = 2 * style_pandora['strich']['shift']
+        
+        self.background = '#ffffff'
+        self.col = style_pandora['color']['main']
+        self.col_light = style_pandora['color']['light']
+        self.col_accent = style_pandora['color']['acc']
+        self.col_accent_light = style_pandora['color']['acc_light']
+        self.col_gray = '#eeeeee'
+        
+    def setViewByGeo(self, geoView):
+        w0, h0 = self.view['width'], self.view['height']
+        w, h = geoView['width'], geoView['height']
+        q = min(w0/w, h0/h)
+        
+        self.view['scale'] = geoView['scale'] * q
+        self.view['xZero'] = geoView['xZero'] * q + (w0 - q * w) / 2
+        self.view['yZero'] = geoView['yZero'] * q + (h0 - q * h) / 2
 
 #--------------------------------------------------------------------------
 
 class GeoDynamic(MovingCameraScene):
     style_default = GeoStyle('purple', 'dark')
 
     def __init__(self):
@@ -157,19 +239,37 @@
             else: continue
             if not el.visible: 
                 mobj.set_opacity(0)
 
     def loadGeometry(self, filepath, update = False, debug = False):
         short_parser.loadCode(self.geo, filepath, update = update, debug = debug)
         self.geo.rebuild(debug = debug)
-        
-    def loadGeoGebra(self, filepath, update = False, debug = False):
+
+    def loadGeoGebra(self, filepath, scheme = 'pandora', px_size = None, update = False, debug = False):
         self.geo = ggb_parser.load(filepath, debug = debug) 
         self.geo.rebuild(debug = debug)
-        self.setStyle(GeoStyle('blue', 'light'))
+        
+        style = GeoStyle(scheme = scheme, px_size = px_size)
+        
+        if px_size is not None:
+            style.setViewByGeo(self.geo.style['view'])
+        else:
+            style.view = self.geo.style['view']
+
+        view = style.view
+        scale = view['scale']
+        for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_rshift', 'strich_len']:
+            style.__setattr__(key, getattr(style, key) * 50 / scale)
+
+        self.camera.frame.set(width = view['width'] / scale)
+        dx = self.camera.frame.width / 2 - view['xZero'] / scale
+        dy = view['height'] / (2 * scale) - view['yZero'] / scale      
+        self.camera.frame.shift(dx * RIGHT + dy * DOWN)
+
+        self.setStyle(style)
         self.addAllGeometry(show = True)
 
     def updateGeoVar(self, x, var_name):
         self.geo.update(var_name, float(x.get_value()))
         updates = self.geo.rebuild()
         #print(updates)
         #if np.isclose(self.geo.var(var_name).data, float(x.get_value())): return
@@ -194,20 +294,22 @@
     def playGrayStyle(self, names, mode = None, **kwargs):
         self.play(*GrayStyleObjs(self, names, mode, **kwargs))
 
     def playBackStyle(self, names, mode = None, **kwargs):
         self.play(*BackStyleObjs(self, names, mode, **kwargs))
 
     #----------------------------------
-        
+
     def exportSVG(self, filepath):
-        config.frame_height = self.camera.frame.get_height()
-        config.frame_width = self.camera.frame.get_width()
-        #print(config)
-        config.__setattr__('frame_center', self.camera.frame.get_center())
+        #config.frame_height = self.camera.frame.get_height()
+        #config.frame_width = self.camera.frame.get_width()
+        #scale = 2 * self.style['view']['scale']
+        #config.frame_width, config.frame_height = self.style['view']['width'] / scale, self.style['view']['height'] / scale
+        #config.__setattr__('frame_center', self.camera.frame.get_center())
+        config.__setattr__('ggb_view', self.style.view)
         VGroup(*self.mobjects).to_svg(filepath)
     
     def addGrid(self, x_range=(-10, 10, 1), y_range=(-10, 10, 1)):
         grid = NumberPlane(
             x_range = x_range,
             y_range = y_range,
             x_length = x_range[1] - x_range[0],
@@ -445,14 +547,29 @@
     for tex in texsymb:
         label = re.sub(texsymb[tex], re.sub(r'\\', r'\\\\', tex), label)
 
     #print('AFTER: ', label)
 
     return label
 
+def getAngRadius(ang: geo.Angle, style = None):
+    if style is None: style = GeoDynamic.style_default
+    r = style.ang_rdefault
+    max_r = min(np.linalg.norm(ang.v1), np.linalg.norm(ang.v2))*0.65
+    if ang.angle > 0.01:
+        return min(max_r, r / ang.angle**0.25)
+    else:
+        return min(max_r, r / 0.01**0.25)
+        
+def getRightAngSize(ang: geo.Angle, style = None):
+    if style is None: style = GeoDynamic.style_default
+    r = style.ang_right
+    max_r = min(np.linalg.norm(ang.v1), np.linalg.norm(ang.v2))*0.65
+    return min(max_r, r)
+
 def CreateMObject(elem, z_auto = False, style = None, debug = False):
     try:
         if style is None: style = GeoDynamic.style_default
 
         dash = getParamFromDict(elem.style, 'stroke_dash', None)
 
         col_s = getParamFromDict(elem.style, 'stroke', style.strong)
@@ -483,23 +600,23 @@
             poly_fill = Polygon(*pp, color = col_s, fill_color = col_f, fill_opacity = op_f, stroke_width = 0, stroke_opacity = 0).set_z_index(zz)
             poly_stroke = Polygon(*pp, joint_type = LineJointType.ROUND, color = col_s, fill_opacity = 0, stroke_width = lw, stroke_opacity = op_s).set_z_index(max(zz_stroke, zz + 0.1))
             
             return VGroup(poly_fill, poly_stroke, name = elem.name)
             
         if type(elem.data) == geo.Angle: 
             arr = []
-            r = elem.data.r + elem.style['r_offset'] + (elem.style['lines'] - 1) * style.ang_rshift
+            r = getAngRadius(elem.data, style) + elem.style['r_offset'] + (elem.style['lines'] - 1) * style.ang_rshift
             p = [elem.data.p[0], elem.data.p[1], 0]
             line1 = Line([p[0], p[1], 0], [p[0] + elem.data.v1[0], p[1] + elem.data.v1[1], 0])
             line2 = Line([p[0], p[1], 0], [p[0] + elem.data.v2[0], p[1] + elem.data.v2[1], 0])    
-            
+
             right_mark = np.isclose(elem.data.angle, PI/2) if 'right_mark' not in elem.style else elem.style['right_mark']
 
             if right_mark:
-                r *= 0.7
+                r = getRightAngSize(elem.data, style)
                 n1 = elem.data.v1 * (r / np.linalg.norm(elem.data.v1))
                 n2 = elem.data.v2 * (r / np.linalg.norm(elem.data.v2))
                 p1 = [p[0] + n1[0], p[1] + n1[1], 0]
                 p2 = [p1[0] + n2[0], p1[1] + n2[1], 0]
                 p3 = [p[0] + n2[0], p[1] + n2[1], 0]
                 arr.append(Polygon(p, p1, p2, p3, 
                                     color = col_f, stroke_width = 0, fill_opacity = op_f).set_z_index(zz))
@@ -584,15 +701,15 @@
                 arr.append(tex)
                 if hasParam(elem.style, 'offset'):
                     tex.shift([elem.style['offset'][0], elem.style['offset'][1], 0])
 
             return VGroup(*arr, name = elem.name)
 
         if type(elem.data) == geo.Point:  
-            arr = [Dot([elem.data.a[0], elem.data.a[1], 0], radius = style.dot_size,
+            arr = [Dot([elem.data.a[0], elem.data.a[1], 0], radius = style.dot_size / 2,
                     color = col_f, fill_opacity = op_f).set_z_index(zz)]
             if hasParam(elem.style, 'show_label'):
                 label = elem.style['label'] if hasParam(elem.style, 'label') else '$' + elem.name + '$'
                 tex = Tex(correctedLabel(label), color = col_label).set_z_index(zz_label).scale(1.12).move_to(arr[0])
                 arr.append(tex)
                 if hasParam(elem.style, 'offset'):
                     tex.shift([elem.style['offset'][0], elem.style['offset'][1], 0])
```

### Comparing `geodynamic-0.0.2/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.3/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.2/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.3/geodynamic/parsers/ggb_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 temp_path = os.path.join(os.getcwd(), "temp")
 
 #--------------------------------------------------------------------------
 
 def rgb_to_hex(r, g, b):
     return '#{:02x}{:02x}{:02x}'.format(r, g, b)
 
-def get_constr_xelem(ggb_path: str): # -> XElement:
+def get_xelems(ggb_path: str): # -> XElement:
     try:    
         os.mkdir(temp_path)
     except FileExistsError:
         pass
     shutil.copyfile(ggb_path, os.path.join(temp_path, "temp.ggb"))
     
     ggb = ZipFile(os.path.join(temp_path, "temp.ggb"))
@@ -28,23 +28,22 @@
     os.remove(os.path.join(temp_path, "temp.ggb"))
     
     tree = ElementTree.parse(os.path.join(temp_path, "geogebra.xml"))
     root = tree.getroot()
     
     shutil.rmtree(temp_path)
     
-    return root.find("construction")
+    return root.find("construction"), root.find("euclidianView")
 
-def parse(constr_xelem: XElement, debug = False): # -> Construction:
-    constr = Construction()
+def parse_constr(constr: Construction, constr_xelem: XElement, debug = False):
     xelems_left_to_pass = 0
 
     style = {}
     
-    for xelem in constr_xelem:
+    for xelem in constr_xelem:            
         if xelem.tag == "element":
             name = xelem.attrib['label']
             #print(f'ELEMENT {name}')
             if xelem.attrib["type"] != "numeric":
                 style[name] = {}
 
                 elem = xelem.find("decoration")
@@ -134,14 +133,29 @@
         for key in style[name]:
             #print(f'STYLE >> {name} >> {key} = {style[name][key]}')
             if key == 'show_element':
                 constr.element(name).visible = style[name][key]
                 continue
             constr.element(name).style[key] = style[name][key]
 
-    return constr
+def FloatOrNone(txt):
+    return float(txt) if txt is not None else None
+
+def parse_view(constr: Construction, view_xelem: XElement, debug = False):
+    constr.style['view'] = {}
+    
+    for xelem in view_xelem:            
+        if xelem.tag == "size":
+            constr.style['view']['width'], constr.style['view']['height'] = FloatOrNone(xelem.attrib['width']), FloatOrNone(xelem.attrib['height'])
+
+        if xelem.tag == "coordSystem":
+            constr.style['view']['xZero'], constr.style['view']['yZero'] = FloatOrNone(xelem.attrib['xZero']), FloatOrNone(xelem.attrib['yZero'])
+            constr.style['view']['scale'] = FloatOrNone(xelem.attrib['scale'])       
 
 def load(ggb_path: str, debug = False): # -> Construction:
-    constr_xelem = get_constr_xelem(ggb_path)
-    constr = parse(constr_xelem, debug = debug)
+    constr_xelem, view_xelem = get_xelems(ggb_path)
+    print(constr_xelem, view_xelem)
+    constr = Construction()
+    parse_constr(constr, constr_xelem, debug = debug)
+    parse_view(constr, view_xelem, debug = debug)
     
     return constr
```

### Comparing `geodynamic-0.0.2/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.3/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.2/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.3/geodynamic.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: manim>=0.18.0
-Requires-Dist: manim-mobject-svg>=0.5.0
+Requires-Dist: pycairo>=1.0.0
 
 # GeoDynamic
 
 ## Installation
 
-```
+```bash
 pip install --upgrade geodynamic
 ```
 
 ## Using
 
-```
+1. Preparing code `test.py`:
+
+```python
 from geodynamic.manim_dynamic import *
 
-class Test(GeoDynamic):
+class TestScene(GeoDynamic):
     def construct(self):       
-        self.loadGeoGebra('./test.ggb')    
-        self.exportSVG('./test_ggb.svg')
+        self.loadGeoGebra('test.ggb', scheme = 'pandora', px_size = [400, 300])    
+        self.exportSVG('test_ggb.svg')
+```
+
+2. Run compilation:
+
+```bash
+manim 'test.py' TestScene
 ```
```

### Comparing `geodynamic-0.0.2/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.3/geodynamic.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 geodynamic/geo/construction.py
 geodynamic/geo/lib_commands.py
 geodynamic/geo/lib_elements.py
 geodynamic/geo/lib_vars.py
 geodynamic/parsers/__init__.py
 geodynamic/parsers/ggb_generator.py
 geodynamic/parsers/ggb_parser.py
-geodynamic/parsers/short_parser.py
+geodynamic/parsers/short_parser.py
+geodynamic/parsers/svg_parser.py
```

### Comparing `geodynamic-0.0.2/setup.py` & `geodynamic-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.2',
+  version='0.0.3',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
   install_requires=[
       'requests>=2.25.1',
       'numpy>=1.26.0',
       'manim>=0.18.0',
-      'manim-mobject-svg>=0.5.0',
+      'pycairo>=1.0.0',
       ],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='geometry dynamic geogebra manim animation svg python',
   #project_urls={
   #  'Documentation': 'https://gitlab.mathem.ru/'
   #},
-  python_requires='>=3.7'
+  python_requires='>=3.9'
 )
 
 print(find_packages())
```

