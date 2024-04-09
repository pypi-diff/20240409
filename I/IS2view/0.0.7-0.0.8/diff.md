# Comparing `tmp/IS2view-0.0.7.tar.gz` & `tmp/IS2view-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IS2view-0.0.7.tar", last modified: Sat Apr  6 18:00:33 2024, max compression
+gzip compressed data, was "IS2view-0.0.8.tar", last modified: Tue Apr  9 16:34:12 2024, max compression
```

## Comparing `IS2view-0.0.7.tar` & `IS2view-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-06 18:00:23.000000 IS2view-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-06 18:00:23.000000 IS2view-0.0.7/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-06 18:00:23.000000 IS2view-0.0.7/CONTRIBUTORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/IS2view/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69246 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-06 18:00:23.000000 IS2view-0.0.7/IS2view/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:00:33.866410 IS2view-0.0.7/IS2view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 18:00:33.000000 IS2view-0.0.7/IS2view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-06 18:00:23.000000 IS2view-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 18:00:23.000000 IS2view-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-06 18:00:33.866410 IS2view-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-06 18:00:23.000000 IS2view-0.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-06 18:00:23.000000 IS2view-0.0.7/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:00:23.000000 IS2view-0.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 18:00:23.000000 IS2view-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:00:33.866410 IS2view-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-06 18:00:23.000000 IS2view-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 18:00:23.000000 IS2view-0.0.7/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:34:12.950367 IS2view-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-09 16:34:03.000000 IS2view-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-09 16:34:03.000000 IS2view-0.0.8/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 16:34:03.000000 IS2view-0.0.8/CONTRIBUTORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:34:12.946367 IS2view-0.0.8/IS2view/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75917 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 16:34:03.000000 IS2view-0.0.8/IS2view/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:34:12.946367 IS2view-0.0.8/IS2view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-09 16:34:12.000000 IS2view-0.0.8/IS2view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 16:34:12.000000 IS2view-0.0.8/IS2view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:34:12.000000 IS2view-0.0.8/IS2view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:34:12.000000 IS2view-0.0.8/IS2view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 16:34:12.000000 IS2view-0.0.8/IS2view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 16:34:03.000000 IS2view-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 16:34:03.000000 IS2view-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-09 16:34:12.946367 IS2view-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-09 16:34:03.000000 IS2view-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 16:34:03.000000 IS2view-0.0.8/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 16:34:03.000000 IS2view-0.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:34:03.000000 IS2view-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:34:12.950367 IS2view-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-09 16:34:03.000000 IS2view-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 16:34:03.000000 IS2view-0.0.8/version.txt
```

### Comparing `IS2view-0.0.7/.gitignore` & `IS2view-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/CODE_OF_CONDUCT.rst` & `IS2view-0.0.8/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view/__init__.py` & `IS2view-0.0.8/IS2view/__init__.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view/api.py` & `IS2view-0.0.8/IS2view/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 api.py
-Written by Tyler Sutterley (03/2024)
+Written by Tyler Sutterley (04/2024)
 Plotting tools for visualizing rioxarray variables on leaflet maps
 
 PYTHON DEPENDENCIES:
     geopandas: Python tools for geographic data
         http://geopandas.readthedocs.io/
     ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython
         https://ipywidgets.readthedocs.io/en/latest/
@@ -24,14 +24,16 @@
         https://rasterio.readthedocs.io
     xarray: N-D labeled arrays and datasets in Python
         https://docs.xarray.dev/en/stable/
     xyzservices: Source of XYZ tiles providers
         https://xyzservices.readthedocs.io/en/stable/
 
 UPDATE HISTORY:
+    Updated 04/2024: add connections and functions for changing variables
+        and other attributes of the leaflet map visualization
     Updated 03/2024: add fix for broken xyzservice links
         fix deprecation of copying ipyleaflet layers
     Updated 11/2023: setting dynamic colormap with float64 min and max
         rather than nans due to future deprecation of JSON serialization
     Updated 08/2023: add option for viewing full screen leaflet map
     Updated 07/2023: renamed module from IS2view.py to api.py
         add plot functions for map basemaps and added geometries
@@ -69,14 +71,17 @@
     logging.debug("ipyleaflet not available")
 try:
     import matplotlib
     import matplotlib.cm as cm
     import matplotlib.colorbar
     import matplotlib.pyplot as plt
     import matplotlib.colors as colors
+    matplotlib.rcParams['font.family'] = 'sans-serif'
+    matplotlib.rcParams['font.sans-serif'] = ['Arial', 'Helvetica', 'DejaVu Sans']
+    matplotlib.rcParams['mathtext.default'] = 'regular'
 except (AttributeError, ImportError, ModuleNotFoundError) as exc:
     logging.critical("matplotlib not available")
 try:
     import owslib.wms
 except (AttributeError, ImportError, ModuleNotFoundError) as exc:
     logging.debug("owslib not available")
 try:
@@ -312,15 +317,15 @@
         if kwargs['scale_control']:
             self.scale_control = ipyleaflet.ScaleControl(position='topright')
             self.map.add(self.scale_control)
         # add control for cursor position
         if kwargs['cursor_control']:
             self.cursor = ipywidgets.Label()
             cursor_control = ipyleaflet.WidgetControl(widget=self.cursor,
-                position='bottomright')
+                position='bottomleft')
             self.map.add(cursor_control)
             # keep track of cursor position
             self.map.on_interaction(self.handle_interaction)
         # add draw control
         if kwargs['draw_control']:
             # add control for drawing features on map
             draw_control = ipyleaflet.DrawControl(
@@ -667,52 +672,52 @@
 
     bounds = Tuple(Tuple(Float(), Float()), Tuple(Float(), Float()))
     @observe('bounds')
     def boundary_change(self, change):
         """Update image on boundary change
         """
         # add image object to map
-        if self.image is not None:
+        if self._image is not None:
             # attempt to remove layer
-            self.remove(self.image)
+            self.remove(self._image)
             # create new image service layer
-            self.image = ipyleaflet.ImageService(
+            self._image = ipyleaflet.ImageService(
                 name=self._variable,
                 crs=self.crs,
                 interactive=True,
                 update_interval=100,
                 endpoint='local')
         # add click handler for popups
         if self.enable_popups:
-            self.image.on_click(self.handle_click)
+            self._image.on_click(self.handle_click)
         # set the image url
         self.set_image_url()
-        self.add(self.image)
+        self.add(self._image)
 
     def __init__(self, ds):
         # initialize map
         self.map = None
         self.crs = None
         self.left, self.top = (None, None)
         self.right, self.bottom = (None, None)
         self.sw = {}
         self.ne = {}
         # initialize dataset
         self._ds = ds
         self._ds_selected = None
         self._variable = None
         # initialize image and colorbars
-        self.image = None
+        self._image = None
         self.cmap = None
         self.norm = None
         self.opacity = None
-        self.colorbar = None
+        self._colorbar = None
         # initialize attributes for popup
         self.enable_popups = False
-        self.popup = None
+        self._popup = None
         self._data = None
         self._units = None
 
     # add imagery data to leaflet map
     def plot(self, m, **kwargs):
         """Creates image plots on leaflet maps
 
@@ -763,59 +768,50 @@
         self.lag = int(kwargs['lag'])
         if (self._ds[self._variable].ndim == 3) and ('time' in self._ds[self._variable].dims):
             self._ds_selected = self._ds[self._variable].sel(time=self._ds.time[self.lag])
         elif (self._ds[self._variable].ndim == 3) and ('band' in self._ds[self._variable].dims):
             self._ds_selected = self._ds[self._variable].sel(band=1)
         else:
             self._ds_selected = self._ds[self._variable]
-        # set colorbar limits to 2-98 percentile
-        # if not using a defined plot range
-        clim = self._ds_selected.chunk(dict(y=-1,x=-1)).quantile((0.02, 0.98)).values
-        fmin = np.finfo(np.float64).min
-        if (kwargs['vmin'] is None) or np.isclose(kwargs['vmin'], fmin):
-            vmin = clim[0]
-        else:
-            vmin = np.copy(kwargs['vmin'])
-        fmax = np.finfo(np.float64).max
-        if (kwargs['vmax'] is None) or np.isclose(kwargs['vmax'], fmax):
-            vmax = clim[-1]
-        else:
-            vmax = np.copy(kwargs['vmax'])
+        # get the normalization bounds
+        self.get_norm_bounds(**kwargs)
         # create matplotlib normalization
         if kwargs['norm'] is None:
-            self.norm = colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
+            self.norm = colors.Normalize(vmin=self.vmin, vmax=self.vmax, clip=True)
         else:
             self.norm = copy.copy(kwargs['norm'])
         # get colormap
         self.cmap = copy.copy(cm.get_cmap(kwargs['cmap']))
         # get opacity
         self.opacity = float(kwargs['opacity'])
         # wait for changes
         asyncio.ensure_future(self.async_wait_for_bounds())
-        self.image = ipyleaflet.ImageService(
+        self._image = ipyleaflet.ImageService(
             name=self._variable,
             crs=self.crs,
             interactive=True,
             update_interval=100,
             endpoint='local')
         # add click handler for popups
         if self.enable_popups:
-            self.image.on_click(self.handle_click)
+            self._image.on_click(self.handle_click)
         # set the image url
         self.set_image_url()
         # add image object to map
-        self.add(self.image)
+        self.add(self._image)
         # add colorbar
-        if kwargs['colorbar']:
+        self.colorbar = kwargs['colorbar']
+        self.colorbar_position = kwargs['position']
+        if self.colorbar:
             self.add_colorbar(
                 label=self._variable,
                 cmap=self.cmap,
                 opacity=self.opacity,
                 norm=self.norm,
-                position=kwargs['position']
+                position=self.colorbar_position
             )
 
     def wait_for_change(self, widget, value):
         future = asyncio.Future()
         def get_value(change):
             future.set_result(change.new)
             widget.unobserve(get_value, value)
@@ -879,17 +875,17 @@
             elif (layer._model_name == 'LeafletPopupModel'):
                 self.remove(layer)
         for control in self.map.controls:
             if (control._model_name == 'LeafletWidgetControlModel') and \
                 (control.widget._model_name == 'ImageModel'):
                 self.remove(control)
         # reset layers and controls
-        self.image = None
-        self.popup = None
-        self.colorbar = None
+        self._image = None
+        self._popup = None
+        self._colorbar = None
 
     # get map bounding box in projected coordinates
     def get_bbox(self):
         """get the bounding box of the leaflet map in projected coordinates
         """
         # get SW and NE corners in map coordinates
         (self.left, self.top), (self.right, self.bottom) = self.map.pixel_bounds
@@ -934,14 +930,61 @@
         except Exception as exc:
             pass
         else:
             self._ds.rio.set_crs(ds_crs)
             return
         # raise exception
         raise Exception('Unknown coordinate reference system')
+    
+    def get_norm_bounds(self, **kwargs):
+        """
+        Get the colorbar normalization bounds
+
+        Parameters
+        ----------
+        vmin : float or NoneType
+            Minimum value for normalization
+        vmax : float or NoneType
+            Maximum value for normalization
+        """
+        # set default keyword arguments
+        kwargs.setdefault('vmin', None)
+        kwargs.setdefault('vmax', None)
+        # set colorbar limits to 2-98 percentile
+        # if not using a defined plot range
+        clim = self._ds_selected.chunk(dict(y=-1,x=-1)).quantile((0.02, 0.98)).values
+        # set minimum for normalization
+        fmin = np.finfo(np.float64).min
+        if (kwargs['vmin'] is None) or np.isclose(kwargs['vmin'], fmin):
+            self.vmin = clim[0]
+            self._dynamic = True
+        else:
+            self.vmin = np.copy(kwargs['vmin'])
+            self._dynamic = False
+        # set maximum for normalization
+        fmax = np.finfo(np.float64).max
+        if (kwargs['vmax'] is None) or np.isclose(kwargs['vmax'], fmax):
+            self.vmax = clim[-1]
+            self._dynamic = True
+        else:
+            self.vmax = np.copy(kwargs['vmax'])
+            self._dynamic = False
+
+    def validate_norm(self):
+        """
+        Validate the colorbar normalization bounds
+        """
+        fmin = np.finfo(np.float64).min
+        fmax = np.finfo(np.float64).max
+        if np.isclose(self.vmin, fmin):
+            self.vmin = -5
+            self._dynamic = False
+        if np.isclose(self.vmax, fmax):
+            self.vmax = 5
+            self._dynamic = False
 
     def clip_image(self, ds):
         """clip or warp xarray image to bounds of leaflet map
         """
         self.get_bbox()
         # attempt to get the coordinate reference system of the dataset
         self.get_crs()
@@ -1026,45 +1069,189 @@
         return self
 
     def set_image_url(self, *args, **kwargs):
         """set the url for the imageservice
         """
         self.get_bounds()
         self.get_image_url()
-        self.image.url = self.url
+        self._image.url = self.url
+
+    def redraw(self, *args, **kwargs):
+        """
+        Redraw the image on the map
+        """
+        # try to update the selected dataset
+        try:
+            self.get_image_url()
+        except Exception as exc:
+            pass
+        else:
+            # update image url
+            self._image.url = self.url
+            # force redrawing of map by removing and adding layer
+            self.remove(self._image)
+            self.add(self._image)
+
+    def redraw_colorbar(self, *args, **kwargs):
+        """
+        Redraw the colorbar on the map
+        """
+        try:
+            if self.colorbar:
+                self.add_colorbar(
+                    label=self._variable,
+                    cmap=self.cmap,
+                    opacity=self.opacity,
+                    norm=self.norm,
+                    position=self.colorbar_position
+                )
+        except Exception as exc:
+            pass
+
+    # observe changes in widget parameters
+    def observe_widget(self, widget, **kwargs):
+        """observe changes in widget parameters
+        """
+        # connect variable widget to set function
+        try:
+            widget.variable.observe(self.set_variable)
+        except AttributeError:
+            pass
+        # connect time lag widget to time slice function
+        try:
+            widget.timelag.observe(self.set_lag)
+        except AttributeError:
+            pass
+        # connect normalization widget to set function
+        try:
+            widget.range.observe(self.set_norm)
+        except AttributeError:
+            pass
+        # connect dynamic normalization widget to set function
+        try:
+            widget.dynamic.observe(self.set_dynamic)
+        except AttributeError:
+            pass
+        # connect colormap widget to set function
+        try:
+            widget.cmap.observe(self.set_colormap)
+        except AttributeError:
+            pass
+        # connect reverse colormap widget to set function
+        try:
+            widget.reverse.observe(self.set_colormap)
+        except AttributeError:
+            pass
+
+    def set_variable(self, sender):
+        """update the dataframe variable for a new selected variable
+        """
+        # only update variable if a new final
+        if isinstance(sender['new'], str):
+            self._variable = sender['new']
+        else:
+            return
+        # reduce to variable and lag
+        if (self._ds[self._variable].ndim == 3) and ('time' in self._ds[self._variable].dims):
+            self._ds_selected = self._ds[self._variable].sel(time=self._ds.time[self.lag])
+        elif (self._ds[self._variable].ndim == 3) and ('band' in self._ds[self._variable].dims):
+            self._ds_selected = self._ds[self._variable].sel(band=1)
+        else:
+            self._ds_selected = self._ds[self._variable]
+        # check if dynamic normalization is enabled
+        if self._dynamic:
+            self.get_norm_bounds()
+            self.norm.vmin = self.vmin
+            self.norm.vmax = self.vmax
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
 
     def set_lag(self, sender):
         """update the time lag for the selected variable
         """
         # only update lag if a new final
         if isinstance(sender['new'], int):
             self.lag = sender['new'] - 1
         else:
             return
         # try to update the selected dataset
-        try:
-            self._ds_selected = self._ds[self._variable].sel(time=self._ds.time[self.lag])
-            self.get_image_url()
-        except Exception as exc:
-            pass
+        self._ds_selected = self._ds[self._variable].sel(time=self._ds.time[self.lag])
+        # check if dynamic normalization is enabled
+        if self._dynamic:
+            self.get_norm_bounds()
+            self.norm.vmin = self.vmin
+            self.norm.vmax = self.vmax
+        # try to redraw the selected dataset
+        self.redraw()
+        if self._dynamic:
+            self.redraw_colorbar()
+
+    def set_dynamic(self, sender):
+        """set dynamic normalization for the selected variable
+        """
+        # only update dynamic norm if a new final
+        if isinstance(sender['new'], bool) and sender['new']:
+            self.get_norm_bounds()
+            self._dynamic = True
+        elif isinstance(sender['new'], bool):
+            self.vmin, self.vmax = (-5, 5)
+            self._dynamic = False
         else:
-            # update image url
-            self.image.url = self.url
-            # force redrawing of map by removing and adding layer
-            self.remove(self.image)
-            self.add(self.image)
+            return
+        # set the normalization bounds
+        self.validate_norm()
+        self.norm.vmin = self.vmin
+        self.norm.vmax = self.vmax
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
+
+    def set_norm(self, sender):
+        """update the normalization for the selected variable
+        """
+        # only update norm if a new final
+        if isinstance(sender['new'], (tuple, list)):
+            self.vmin, self.vmax = sender['new']
+        else:
+            return
+        # set the normalization bounds
+        self.validate_norm()
+        self.norm.vmin = self.vmin
+        self.norm.vmax = self.vmax
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
+
+    def set_colormap(self, sender):
+        """update the colormap for the selected variable
+        """
+        # only update colormap if a new final
+        if isinstance(sender['new'], str):
+            cmap_name = self.cmap.name
+            cmap_reverse_flag = '_r' if cmap_name.endswith('_r') else ''
+            self.cmap = cm.get_cmap(sender['new'] + cmap_reverse_flag)
+        elif isinstance(sender['new'], bool):
+            cmap_name = self.cmap.name.strip('_r')
+            cmap_reverse_flag = '_r' if sender['new'] else ''
+            self.cmap = cm.get_cmap(cmap_name + cmap_reverse_flag)
+        else:
+            return
+        # try to redraw the selected dataset
+        self.redraw()
+        self.redraw_colorbar()
 
     # functional calls for click events
     def handle_click(self, **kwargs):
         """callback for handling mouse clicks
         """
         lat, lon = kwargs.get('coordinates')
         # remove any prior instances of popup
-        if self.popup is not None:
-            self.remove(self.popup)
+        if self._popup is not None:
+            self.remove(self._popup)
         # attempt to get the coordinate reference system of the dataset
         try:
             grid_mapping = self._ds[self._variable].attrs['grid_mapping']
             crs = self._ds[grid_mapping].attrs['crs_wkt']
         except Exception as exc:
             crs = self._ds.rio.crs.to_wkt()
         else:
@@ -1076,17 +1263,17 @@
         self._units = self._ds[self._variable].attrs['units']
         # only create popup if valid
         if np.isnan(self._data):
             return
         # create contextual popup
         child = ipywidgets.HTML()
         child.value = '{0:0.1f} {1}'.format(np.squeeze(self._data), self._units)
-        self.popup = ipyleaflet.Popup(location=(lat, lon),
+        self._popup = ipyleaflet.Popup(location=(lat, lon),
             child=child, name='popup')
-        self.add(self.popup)
+        self.add(self._popup)
 
     # add colorbar widget to leaflet map
     def add_colorbar(self, **kwargs):
         """Creates colorbars on leaflet maps
 
         Parameters
         ----------
@@ -1098,42 +1285,43 @@
         position : str, position of colorbar on leaflet map
         width : float, width of colorbar
         height : float, height of colorbar
         """
         kwargs.setdefault('cmap', 'viridis')
         kwargs.setdefault('norm', None)
         kwargs.setdefault('opacity', 1.0)
-        kwargs.setdefault('orientation', 'horizontal')
+        kwargs.setdefault('orientation', 'vertical')
         kwargs.setdefault('label', 'delta_h')
         kwargs.setdefault('position', 'topright')
-        kwargs.setdefault('width', 6.0)
-        kwargs.setdefault('height', 0.4)
+        kwargs.setdefault('width', 0.2)
+        kwargs.setdefault('height', 3.0)
         # remove any prior instances of a colorbar
-        if self.colorbar is not None:
-            self.remove(self.colorbar)
+        if self._colorbar is not None:
+            self.remove(self._colorbar)
         # create matplotlib colorbar
         _, ax = plt.subplots(figsize=(kwargs['width'], kwargs['height']))
         cbar = matplotlib.colorbar.ColorbarBase(ax,
             cmap=kwargs['cmap'],
             norm=kwargs['norm'],
             alpha=kwargs['opacity'],
             orientation=kwargs['orientation'],
             label=kwargs['label'])
         cbar.solids.set_rasterized(True)
         cbar.ax.tick_params(which='both', width=1, direction='in')
         # save colorbar to in-memory png object
         png = io.BytesIO()
-        plt.savefig(png, bbox_inches='tight', format='png', transparent=True)
+        plt.savefig(png, bbox_inches='tight', pad_inches=0.075,
+            format='png', transparent=True)
         png.seek(0)
         # create output widget
         output = ipywidgets.Image(value=png.getvalue(), format='png')
-        self.colorbar = ipyleaflet.WidgetControl(widget=output,
-            transparent_bg=True, position=kwargs['position'])
+        self._colorbar = ipyleaflet.WidgetControl(widget=output,
+            transparent_bg=False, position=kwargs['position'])
         # add colorbar
-        self.add(self.colorbar)
+        self.add(self._colorbar)
         plt.close()
 
     # save the current map as an image
     def imshow(self, ax=None, **kwargs):
         """Save the current map as a static image
 
         Parameters
```

### Comparing `IS2view-0.0.7/IS2view/convert.py` & `IS2view-0.0.8/IS2view/convert.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view/io.py` & `IS2view-0.0.8/IS2view/io.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view/tools.py` & `IS2view-0.0.8/IS2view/tools.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view/utilities.py` & `IS2view-0.0.8/IS2view/utilities.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/IS2view.egg-info/PKG-INFO` & `IS2view-0.0.8/IS2view.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.7/LICENSE` & `IS2view-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/PKG-INFO` & `IS2view-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.7/README.rst` & `IS2view-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.7/setup.py` & `IS2view-0.0.8/setup.py`

 * *Files identical despite different names*

