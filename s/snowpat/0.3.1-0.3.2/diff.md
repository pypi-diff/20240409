# Comparing `tmp/snowpat-0.3.1.tar.gz` & `tmp/snowpat-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowpat-0.3.1.tar", max compression
+gzip compressed data, was "snowpat-0.3.2.tar", max compression
```

## Comparing `snowpat-0.3.1.tar` & `snowpat-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     4706 2024-03-11 10:05:41.864304 snowpat-0.3.1/README.md
--rw-r--r--   0        0        0      451 2024-03-11 13:47:01.256809 snowpat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5553 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/Utils.py
--rw-r--r--   0        0        0      217 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/__init__.py
--rw-r--r--   0        0        0     5961 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/plot_helpers_snowpack.py
--rw-r--r--   0        0        0    14883 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/plot_snowpack.py
--rw-r--r--   0        0        0     5025 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/plotting.py
--rw-r--r--   0        0        0     8884 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/SnowLens/snowlens.py
--rw-r--r--   0        0        0      124 2024-03-11 13:47:01.260809 snowpat-0.3.1/snowpat/__init__.py
--rw-r--r--   0        0        0     3497 2024-03-01 12:47:20.304690 snowpat-0.3.1/snowpat/pysmet/ACDD.py
--rw-r--r--   0        0        0     6642 2024-03-01 12:46:16.651908 snowpat-0.3.1/snowpat/pysmet/MetaData.py
--rw-r--r--   0        0        0    16293 2024-03-11 13:46:15.724125 snowpat-0.3.1/snowpat/pysmet/SMET.py
--rw-r--r--   0        0        0       81 2024-03-01 13:25:13.396701 snowpat-0.3.1/snowpat/pysmet/__init__.py
--rw-r--r--   0        0        0     3434 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/pysmet/pySMET.py
--rw-r--r--   0        0        0     7043 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/snowpackreader/Snowpack.py
--rw-r--r--   0        0        0      103 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/snowpackreader/__init__.py
--rw-r--r--   0        0        0    16984 2024-03-11 09:34:03.280864 snowpat-0.3.1/snowpat/snowpackreader/snowpackreader.py
--rw-r--r--   0        0        0     5290 1970-01-01 00:00:00.000000 snowpat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4818 2024-03-25 16:50:06.259366 snowpat-0.3.2/README.md
+-rw-r--r--   0        0        0      451 2024-04-09 14:03:14.009609 snowpat-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5580 2024-04-09 12:46:08.457422 snowpat-0.3.2/snowpat/SnowLens/Utils.py
+-rw-r--r--   0        0        0      217 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/SnowLens/__init__.py
+-rw-r--r--   0        0        0     6575 2024-04-09 13:46:24.733339 snowpat-0.3.2/snowpat/SnowLens/plot_helpers_snowpack.py
+-rw-r--r--   0        0        0    15924 2024-04-09 13:44:38.712173 snowpat-0.3.2/snowpat/SnowLens/plot_snowpack.py
+-rw-r--r--   0        0        0     5193 2024-04-03 14:37:46.233673 snowpat-0.3.2/snowpat/SnowLens/plotting.py
+-rw-r--r--   0        0        0     9053 2024-04-03 14:24:45.399491 snowpat-0.3.2/snowpat/SnowLens/snowlens.py
+-rw-r--r--   0        0        0      124 2024-04-09 14:03:14.013609 snowpat-0.3.2/snowpat/__init__.py
+-rw-r--r--   0        0        0    26470 2024-04-03 14:58:35.674461 snowpat-0.3.2/snowpat/msgs.py
+-rw-r--r--   0        0        0     3497 2024-03-01 12:47:20.304690 snowpat-0.3.2/snowpat/pysmet/ACDD.py
+-rw-r--r--   0        0        0     6886 2024-04-03 14:33:30.994355 snowpat-0.3.2/snowpat/pysmet/MetaData.py
+-rw-r--r--   0        0        0    16663 2024-04-03 14:34:38.847241 snowpat-0.3.2/snowpat/pysmet/SMET.py
+-rw-r--r--   0        0        0       81 2024-03-01 13:25:13.396701 snowpat-0.3.2/snowpat/pysmet/__init__.py
+-rw-r--r--   0        0        0     3434 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/pysmet/pySMET.py
+-rw-r--r--   0        0        0     7785 2024-04-09 13:50:01.031827 snowpat-0.3.2/snowpat/snowpackreader/Snowpack.py
+-rw-r--r--   0        0        0      103 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/snowpackreader/__init__.py
+-rw-r--r--   0        0        0    16984 2024-03-11 09:34:03.280864 snowpat-0.3.2/snowpat/snowpackreader/snowpackreader.py
+-rw-r--r--   0        0        0     5402 1970-01-01 00:00:00.000000 snowpat-0.3.2/PKG-INFO
```

### Comparing `snowpat-0.3.1/README.md` & `snowpat-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,31 @@
 There are two submodules:
 pysmet: Used to read and write SMET files
 snowpackreader: Used to read SNOWPACK output files (.pro) and handle profiles easily (soon also with visualization)
 SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](https://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/indexplot/))
 
 ## News
 
+2024-03-25: Installation via PyPi now possible
+
 2024-03-08: Plotting of Snow Profiles is available with SnowLense module
 
 2024-03-01: A simple merge function is now available to join to SMET Files: merge(SMETFile, override) and mergeFromFile(filename, override)
 
 ## Installation
 
 Installation via pip and poetry is supported. 
 
-The easiest way to is to directly install from git (needs git to be installed):
+It is as easy as:
+
+```bash
+pip install snowpat
+```
+
+You can also install from git (needs git to be installed) to always get the latest release:
 
 ```bash
 pip install [--user] git+https://gitlabext.wsl.ch/patrick.leibersperger/snowpat.git
 ```
 
 the --user option might be needed if you do not have admin rights.
```

### Comparing `snowpat-0.3.1/snowpat/SnowLens/Utils.py` & `snowpat-0.3.2/snowpat/SnowLens/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     "vmin": Union[int, Dict[str, int]],
     "vmax": Union[int, Dict[str, int]],
     "adjust_data": Callable[[str, ndarray], ndarray],
     "single_ticks": bool,
     "set_ylabel": bool,
     "colorbar": bool,
     "ind_mfcrust": bool,
+    "mfcrust_color": bool,
     "profile_on": datetime,
 }
 
 SNOWPACK_HELP_TEXT = {
     "start": "The start time of the plot",
     "stop": "The stop time of the plot",
     "resolution": "The resolution of dates of the plot",
```

### Comparing `snowpat-0.3.1/snowpat/SnowLens/plot_helpers_snowpack.py` & `snowpat-0.3.2/snowpat/SnowLens/plot_helpers_snowpack.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import datetime
 
 from typing import List, Dict, Optional, Callable, Union
 
 
 grain_type_color = ['greenyellow', 'darkgreen', 'pink', 'lightblue', 'blue', 'magenta', 'red', 'cyan', 'lightblue']
 
+# the default mapping to color maps
 def getColorMap(var_code) -> mcolors.Colormap:
     if var_code == "0513":
         cmap = mcolors.ListedColormap(grain_type_color)
     elif var_code == "0503":
         cmap = "coolwarm"
         cmap = cm.get_cmap(cmap)
     elif var_code == "0502":
@@ -30,14 +31,15 @@
         cmap = "viridis"
         cmap = cm.get_cmap(cmap)
     else:
         cmap = "viridis"
         cmap = cm.get_cmap(cmap)
     return cmap
 
+# the default mapping to normalizations
 def getNorm(var_code) -> mcolors.Normalize:
     if var_code == "0513":
         norm = mcolors.BoundaryNorm([0.5,1.5,2.5,3.5,4.5,5.5,6.5,7.5,8.5,9.5], 9)
     elif var_code == "0503":
         norm = mcolors.Normalize(vmin=-20, vmax=0)
     elif var_code == "0506":
         norm = mcolors.Normalize(vmin=0, vmax=5)
@@ -45,34 +47,37 @@
         norm = mcolors.Normalize(vmin=0, vmax=600)
     elif var_code == "0535":
         norm = mcolors.Normalize(vmin=0, vmax=60)
     else:
         norm = mcolors.LogNorm(vmin=10 ** -1, vmax=1)
     return norm
 
+# the default handling of special var codes
 def adjustData(var_code:str, data:np.ndarray)->np.ndarray:
     new_data = data.copy()
     new_data = np.where(np.isnan(new_data), -999, new_data)
     if var_code == "0513":
         new_data = np.where(new_data == 772, -100, new_data)
         new_data = (divmod(new_data, 100)[0]).astype(int)
         new_data = np.where(new_data == -10, -999, new_data)
         new_data = np.where(new_data == -1, 7.2, new_data)
     if var_code == "0535": # TODO: is this needed?
         ice_density = 917
         new_data = 6 / (ice_density * new_data/1000)   
     return new_data
         
+# contains all the kwargs, and options for the plot
 @dataclass
 class PlotHelper:
     set_ylabel : bool = True
     single_ticks : bool = True
     colorbar : bool = True
     set_cbar_label : bool = True
     ind_mfcrust : bool = True
+    mfcrust_color : bool = False
     n_cols : int = 1
     start : Optional[datetime.datetime] = None
     stop : Optional[datetime.datetime] = None
     resolution : Optional[str] = None
     num_ticks : Optional[int] = None
     cmap : Optional[mcolors.Colormap] = None
     norm : Optional[mcolors.Normalize] = None
@@ -138,14 +143,15 @@
             if var_code == "0513" or var_code == "0503":
                 if np.array_equal(res, data): 
                     res = adjustData(var_code, data) 
         else:
             res = adjustData(var_code, data)
         return res
 
+# formats, so that months and years are only printed, when they change
 class CustomFormatter(mdates.DateFormatter):
     def __init__(self, month_fmt, year_fmt):
         self.month_fmt = month_fmt
         self.year_fmt = year_fmt
         super().__init__(month_fmt)
 
     def __call__(self, x, pos=0):
@@ -165,10 +171,17 @@
                 self.prev_date = current_date
                 return current_date.strftime(self.month_fmt)
 
         # Otherwise, update the previous date and return the year format
         self.prev_date = current_date
         return current_date.strftime(self.year_fmt)
     
-def _add_crust_lines(ax:plt.Axes, x:list, h:np.ndarray, mesh:np.ndarray):
+def _add_crust_lines(ax:plt.Axes, x:list, h:np.ndarray, mesh:np.ndarray, ind_mfcrust:bool = True,new_color:bool = False):
     crust_mesh = np.ma.masked_where(mesh != 7.2, mesh)
-    ax.pcolor(x, h, crust_mesh.transpose(), hatch='///', alpha=0.)
+    if new_color and not ind_mfcrust:
+        ax.pcolor(x,h, crust_mesh.transpose(), color='orange')
+    elif ind_mfcrust and not new_color:
+        ax.pcolor(x,h, crust_mesh.transpose(), hatch="///", alpha=0.)
+    elif new_color and ind_mfcrust:
+        ax.pcolor(x, h, crust_mesh.transpose(), color='orange', hatch='///', alpha=0.)
+    else:
+        pass
```

### Comparing `snowpat-0.3.1/snowpat/SnowLens/plot_snowpack.py` & `snowpat-0.3.2/snowpat/SnowLens/plot_snowpack.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,91 +58,111 @@
         - norm (Union[mcolors.Normalize, Dict[str, mcolors.Normalize]]): The normalization for the plot.
         - cbar_label (Union[str, Dict[str,str]]): The colorbar label for the plot.
         - n_cols (int): The number of columns for the subplots.
         - title (str): The title for the plot.
         - vmin (Union[int, Dict[str,int]]): The minimum value for the colormap.
         - vmax (Union[int, Dict[str,int]]): The maximum value for the colormap.
         - adjust_data (Callable[[str,np.ndarray],np.ndarray]): A function for adjusting the data.
-        - single_ticks (bool): Whether to use a single x-axis/y-axis for all subplots.
-        - set_ylabel (bool): Whether to set the y-axis label.
-        - colorbar (bool): Whether to display the colorbar.
-        - ind_mfcrust (bool): Whether to indicate the MFCrust specifically.
+        - single_ticks (bool): Whether to use a single x-axis/y-axis for all subplots. (default: True)
+        - set_ylabel (bool): Whether to set the y-axis label. (default: True)
+        - colorbar (bool): Whether to display the colorbar. (default: True)
+        - ind_mfcrust (bool): Whether to indicate the MFCrust specifically. (default: True)
+        - mfcrust_color (bool): Plot the meltcrust in orange instead of read. (default: False)
         - subtitle (Dict[str,str]): A dictionary with subtitles for each variable code.
 
         All other keyword arguments are passed to the pcolormesh function.
 
 
         Raises:
             ValueError: If any of the variable codes are not valid.
             RuntimeError: If there is a problem during plotting.
         """
-        plot_data, dates = self._init_data(var_codes)
+        dates = self._init_data(var_codes)
         
         kwargs = self._parse_kwargs(**kwargs)
 
-        plot_dates, tick_dates, plot_data = self._aggregateData(var_codes, dates, plot_data)
+        plot_dates, tick_dates = self._aggregateData(var_codes, dates)
 
 
+        # calculate the number of rows and cols for the subplots
         n_subplots = len(var_codes)
         n_rows = n_subplots // self.plot_helper.n_cols
         if n_subplots % self.plot_helper.n_cols != 0:
             n_rows += 1
-            
+        
+        # adjust the figure size so it stays nicely looking within a grid
         fig_x = 6.4 * (1+ 2.0 * (self.plot_helper.n_cols-1)) if self.plot_helper.n_cols > 1 else 6.4
         fig_y = 4.8 * (1 + 1.0* (n_rows - 1)) if n_rows > 1 and self.plot_helper.n_cols > 1 else 4.8 * (1 + 0.2* (n_rows - 1))
         fig, axes = plt.subplots(n_rows, self.plot_helper.n_cols, figsize=(fig_x,fig_y), sharex=self.plot_helper.single_ticks, sharey=self.plot_helper.single_ticks)
         
+        # add some space between the subplots, to make space for ticks and cbars
         wspace = 0.4 if self.plot_helper.n_cols > 1 and not self.plot_helper.single_ticks else 0.3
         hspace = 0.4 if n_rows > 1 else 0.2
         fig.subplots_adjust(hspace=hspace, wspace=wspace)
         
         if self.plot_helper.title:
             fig.suptitle(self.plot_helper.title, fontsize=16)
         
+        # set the indexes at which subplot the x/y labels should be set
         if self.plot_helper.n_cols > 1 and n_rows > 1:
             ids_ylabels = [i for i in range(1, n_subplots+1) if i % self.plot_helper.n_cols == 1]
             ids_xlabels = [i for i in range(n_subplots-self.plot_helper.n_cols+1, n_subplots+1)]
         elif self.plot_helper.n_cols == 1 and n_rows > 1:
             ids_ylabels = [i for i in range(1, n_subplots+1)]
             ids_xlabels = [n_subplots]
         elif self.plot_helper.n_cols > 1 and n_rows == 1:
             ids_ylabels = [1]
             ids_xlabels = [i for i in range(1, n_subplots+1)]
+        else:
+            ids_xlabels = [1]
+            ids_ylabels = [1]
 
         row = 0
         col = 0
         for sub_id in range(1, n_subplots+1):
             var_code = var_codes[sub_id-1]
 
-            ax = axes[row, col] if self.plot_helper.n_cols > 1 and n_rows > 1 else axes[row]
+            # if it is only one subplot, axes is not an array
+            if isinstance(axes, mpl.axes.Axes):
+                ax = axes
+            else:
+                # we need to get the correct axes object, whether it is a 1D or 2D array
+                ax = axes[row, col] if self.plot_helper.n_cols > 1 and n_rows > 1 else axes[row]            
             row += 1 if (sub_id % self.plot_helper.n_cols == 1) or (self.plot_helper.n_cols == 1 or n_rows == 1) else 0
             col = (col+1) % self.plot_helper.n_cols           
             
             cmap = self.plot_helper.getCmap(var_code)
             norm = self.plot_helper.getNorm(var_code)
             cmap.set_bad(ax.get_facecolor())
             
             mpl.rcParams['hatch.linewidth'] = 3.0
             plot_dates_len = len(plot_dates)
 
             for date_id, plot_date in enumerate(plot_dates):
+                # set the bar to the correct date, i.e. the x boundaries
                 x = [plot_date, plot_dates[date_id+1]] if date_id < plot_dates_len-1 else [plot_date, plot_date + pd.Timedelta(days=1)]
-                h = self.snowpack.get_profile_on(plot_date).get_param("0501") # "0501" are the layer boundaries
-                data = plot_data[var_code][date_id]
+                profile = self.snowpack.get_profile_on(plot_date)
+                # get the layer boundaries, which will be the y boundaries
+                h = profile.get_param("0501") # "0501" are the layer boundaries
+                # the data in the cells
+                data = profile.get_param(var_code)
                 data = self.plot_helper.handleData(var_code, data)
                 if h.size == 1: continue
 
+                # we need to handle missing values
                 mesh = np.array([data,])
                 conditions = mesh== -999
                 masked_mesh = np.ma.masked_where(conditions, mesh)     
 
                 cplot = ax.pcolormesh(x, h, masked_mesh.transpose(), norm=norm, cmap=cmap, **kwargs)
-                if self.plot_helper.ind_mfcrust and var_code == "0513":
-                    _add_crust_lines(ax, x, h, mesh)
+                if var_code == "0513":
+                    # this function will add the crust lines to the plot, if it any is set to true
+                    _add_crust_lines(ax, x, h, mesh, self.plot_helper.ind_mfcrust, self.plot_helper.mfcrust_color)
            
+            # set the x and y limits, for better visualization
             ax.set_xlim(self.plot_helper.start, self.plot_helper.stop)
             hmax = self.snowpack.get_profile_on(self.plot_helper.stop).get_param("0501")[-1]
             ymax = hmax if hmax > 250 else 250
             ymin,_ = ax.get_ylim()
             ax.set_ylim(ymin, ymax)            
             
                 
@@ -266,53 +286,50 @@
         if "subtitle" in kwargs:
             self.plot_helper.subtitle = kwargs.pop("subtitle")
             
         self.plot_helper.single_ticks = kwargs.pop("single_ticks", True)
         self.plot_helper.set_ylabel = kwargs.pop("set_ylabel", True)
         self.plot_helper.colorbar = kwargs.pop("colorbar", True)
         self.plot_helper.ind_mfcrust = kwargs.pop("ind_mfcrust", True)
+        self.plot_helper.mfcrust_color = kwargs.pop("mfcrust_color", False)
         
         return kwargs
                    
     
     def _init_data(self, var_codes):
         for var_code in var_codes:
             if not self.snowpack.DataCodes.get(var_code):
                 raise ValueError(f"Invalid variable code: {var_code}")
-        plot_data = {var_code:[] for var_code in var_codes}
         dates = self.snowpack.get_all_dates()
         self.plot_helper.start = dates[0]
         self.plot_helper.stop = dates[-1]
-        return plot_data, dates
+        return dates
         
-    def _aggregateData(self, var_codes, dates, plot_data):
+    def _aggregateData(self, var_codes, dates):
         start = self.plot_helper.start
         stop = self.plot_helper.stop
         if self.plot_helper.resolution:
             dates = pd.date_range(start, stop, freq=self.plot_helper.resolution)
             
         plot_dates = []
         for date in dates:
             profile = self.snowpack.get_profile_on(date)
             if profile:
                 plot_dates.append(date)
-                for var_code in var_codes: 
-                    data = profile.get_param(var_code)
-                    plot_data[var_code].append(data)
 
                     
         tick_dates = None
         if self.plot_helper.num_ticks:
             tick_dates = pd.date_range(start, stop, freq=(stop-start)/self.plot_helper.num_ticks)
             if (stop-start) > pd.Timedelta(days=1):
                 tick_dates = tick_dates.floor("D")
             else:
                 tick_dates = tick_dates.floor("H")
         
-        return plot_dates, tick_dates, plot_data
+        return plot_dates, tick_dates
 
     def _setColorbar(self, ax:plt.Axes, cplot:QuadMesh, var_code:str, fig:plt.Figure):
         if self.plot_helper.colorbar:
             ax_pos = ax.get_position()
             cax = fig.add_axes([ax_pos.x1+0.01, ax_pos.y0, 0.02, ax_pos.height])
             cbar = plt.colorbar(cplot, cax=cax)
```

### Comparing `snowpat-0.3.1/snowpat/SnowLens/plotting.py` & `snowpat-0.3.2/snowpat/SnowLens/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,8 +137,17 @@
                 horizontalalignment='left', verticalalignment='center',
                 zorder=1)  # Add this line here
 
     # Add sk38 value below the arrow
     ax.annotate("sk38: "+str(sk38), xy=(1.1, z_sk38), xytext=(1.1, z_sk38-0.03),
                 xycoords='axes fraction', textcoords='axes fraction',
                 horizontalalignment='left', verticalalignment='center',
-                zorder=1)  # Add this line here
+                zorder=1)  # Add this line here
+    
+from os import getcwd
+def show_logo():
+    print(getcwd())
+    path = "resources/snowpat.png"
+    logo = plt.imread(path)
+    plt.imshow(logo)
+    plt.show()
+
```

### Comparing `snowpat-0.3.1/snowpat/SnowLens/snowlens.py` & `snowpat-0.3.2/snowpat/SnowLens/snowlens.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .. import pysmet as smet
 from typing import Optional, List
 import matplotlib.pyplot as plt
 
 from .plot_snowpack import SnowpackPlotter, plotProfile
 from .Utils import PlotType, SNOWPACK_KWARGS, SNOWPACK_HELP_TEXT, _type_to_string, PROFILE_HELP_TEXT, PROFILE_KWARGS, GENERAL_HELP_TEXT, GENERAL_KWARGS, _is_of_type
 
+from .plotting import show_logo
 
 def plot(snowpack_file: Optional[spr.SnowpackReader] = None, smetfile: Optional[smet.SMETFile] = None, profile:Optional[spr.Snowpack] = None, **kwargs):
     """
     Plot function for visualizing Snowpack or SMET data.
     Only one of snowpack, smet, or profile should be provided.
 
     Parameters:
@@ -18,15 +19,21 @@
     - profile: Optional[spr.Snowpack], the snowpack profile to plot.
     - **kwargs: Additional keyword arguments for customizing the plot.
 
     Returns:
     - fig: matplotlib.figure.Figure, the generated plot figure.
     - plotter: SnowpackPlotter, the plotter object used for generating the plot. (None if profile is provided)
 
+
+    use plot("snowpat") to show the snowpat logo
     """
+    if snowpack_file == "snowpat": 
+        show_logo()
+        return None, None
+    
     def assign_arg(arg):
         nonlocal snowpack_file, smetfile, profile
         if isinstance(arg, spr.SnowpackReader):
             snowpack_file = arg
             smetfile = None
             profile = None            
         elif isinstance(arg, smet.SMETFile):
```

### Comparing `snowpat-0.3.1/snowpat/pysmet/ACDD.py` & `snowpat-0.3.2/snowpat/pysmet/ACDD.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.1/snowpat/pysmet/MetaData.py` & `snowpat-0.3.2/snowpat/pysmet/MetaData.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, List
 import pandas as pd
 
+from ..msgs import *
 class MetaData:
     """A class used to represent the metadata of a SMET file.
 
     Attributes:
         station_id (str): The ID of the station.
         location (Location): The location of the station, which includes:
             latitude (float): The latitude of the location.
@@ -51,22 +52,27 @@
         d.update(self.location.adjusted_dict)
         del d["location"]
         if d.get('fields') is not None:
                 d['fields'] = ' '.join(d['fields'])
         return d    
     
         
-    def checkValidity(self) -> bool:
+    def checkValidity(self, fun:bool=False) -> bool:
         nodata_set = self.nodata is not None
-        return (
-            self.station_id
-            and self.location.checkValidity()
-            and nodata_set
-            and self.fields
-        )
+        valid =  self.station_id and self.location.checkValidity() and nodata_set and self.fields
+        if not valid:
+            if fun:
+                print(bad())
+                print(empire())
+            raise f"Invalid metadata: {self}"
+        else :
+            if fun:
+                print(way())
+                print(mando())
+        return valid
 
 
 class Location:
     def __init__(self) -> None:
         self.latitude: Optional[float] = None
         self.longitude: Optional[float] = None
         self.altitude: Optional[float] = None
```

### Comparing `snowpat-0.3.1/snowpat/pysmet/SMET.py` & `snowpat-0.3.2/snowpat/pysmet/SMET.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import pandas as pd
 import numpy as np
 import os
 
 from .MetaData import *
 from .ACDD import ACDDMetadata
 
+from ..msgs import *
 
 class SMETFile:
     """A class used to represent a SMET file.
 
     Attributes:
         identifier (str): A string that represents the identifier of the SMET data.
         meta_data (MetaData): An instance of the MetaData class that stores the mandatory metadata of the SMET data.
         data (pd.DataFrame): A pandas DataFrame that stores the SMET data.
         optional_meta_data (OptionalMetadata): A dictionary that stores the optional metadata of the SMET data.
         acdd_meta_data (ACDDMetadata): An instance of the ACDDMetadata class that stores the ACDD metadata of the SMET data.
         other_meta_data(dict): A dictionary that stores the other metadata of the SMET data.
     """
 
-    def __init__(self, filename, read: bool, num_header_lines: int = None) -> None:
+    def __init__(self, filename, read: bool, num_header_lines: int = None, fun:bool = False) -> None:
         if not os.path.isfile(filename) and read:
             raise FileNotFoundError(f"The file {filename} does not exist.")
 
         self.num_header_lines = num_header_lines if read else 1
         self.identifier = None if read else self.getIdentifier()
         self.optional_meta_data = None if read else dict()
         self.filename = filename
         self.data_header = None if read else ""
         self.acdd_meta_data = ACDDMetadata()
         self.other_meta_data = dict()
         self.meta_data = self.read_meta_data() if read else MetaData()
         self.data = self.read_data() if read else pd.DataFrame()
 
+        self.fun = fun
+
     def read_data(self) -> pd.DataFrame:
         if not self.meta_data:
             print(
                 "Something went wrong reading MetaData, in the worst case please contact patrick.leibersperger@slf.ch"
             )
         if self.meta_data.fields:
             self.data_header = self.meta_data.fields
@@ -103,16 +106,19 @@
                 elif "acdd" in line:
                     key, value = line.split("=")
                     self.acdd_meta_data.set_attribute(key.strip(), value.strip())
                 else:
                     self.other_meta_data[line.split("=")[0].strip()] = line.split("=")[1].strip()
         unknown_metadata = [key for key in self.other_meta_data.keys()]
         if unknown_metadata:
+            if self.fun:
+                print(bad())
+                print(empire())
             print(f"Unknown metadata: {unknown_metadata}")
-        meta_data.checkValidity()
+        meta_data.checkValidity(self.fun)
         self.optional_meta_data = optional_meta_data
         return meta_data
 
     def __parseFields(self, fields: List[str]):
         possible_fields = [
             "P",
             "TA",
@@ -132,18 +138,24 @@
             "julian",
         ]
         non_conforming_fields = [
             field for field in fields if field not in possible_fields
         ]
 
         if non_conforming_fields:
-            print(
+            if self.fun:
+                print(not_way())
+                print(yoda())
+            print(                    
                 "The following fields do not conform to the SMET standard:",
                 non_conforming_fields,
             )
+        elif self.fun and not non_conforming_fields:
+            print(way())
+            print(mando())
 
         return fields
 
     def __str__(self):
         return (
             f"SMETFile:\n"
             f"{self.meta_data}\n"
```

### Comparing `snowpat-0.3.1/snowpat/pysmet/pySMET.py` & `snowpat-0.3.2/snowpat/pysmet/pySMET.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.1/snowpat/snowpackreader/Snowpack.py` & `snowpat-0.3.2/snowpat/snowpackreader/Snowpack.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         Returns:
             The parameter associated with the given code.
 
         Raises:
             KeyError: If the code is not found in the data.
 
         """
+        # need to add these, because they were handled seperately and can also be called through different means
         possible_codes = list(self.data.keys()) + ["0501", "0530", "0514"]
         if not code in possible_codes:
             print(f"{code} is invalid")
             print("available codes are:")
             print(f"{self.data.keys()}")
             
         if code == "0501":
@@ -105,24 +106,34 @@
 
         Returns:
             None
         """
         self._above_ground = discard
 
     def _parse_data(self, old_hardness:bool):
-        n_layers = self.num_nodes - 1
+        # snowpack sometimes does not explicitly put a boundary at 0, so we need to append that
+        if self.layer_boundaries[0] > 0:
+            self.num_nodes += 1
+            self.layer_boundaries = np.insert(self.layer_boundaries, 0, 0)
+            self._height_mask = np.insert(self._height_mask, 0, True)
+        
+        # nodes give the boundaries, but values are valid for the whole layer
+        n_layers = self.num_nodes -1
         for key, val in self.data.items():
-            if key == "0513": #TODO: hadnle this shit properly
+            # grain types has surface hoar as 0, and is specified with a dfferent code
+            if key == "0513": 
                 self.data[key] = np.delete(val, -1)
+            # fill missing layers with nans
             if self.data[key].size != n_layers:
                 self.data[key] = np.insert(
                     self.data[key], 0, [np.nan for _ in range(n_layers - self.data[key].size)]
                 )
 
 
+        # make new fields, so it is clearer, where the layers actually are
         layer_middle = [
             (self.layer_boundaries[i + 1] + self.layer_boundaries[i]) / 2
             for i in range(self.layer_boundaries.size - 1)
         ]
         layer_thicknes = [
             (self.layer_boundaries[i + 1] - self.layer_boundaries[i]) / 2
             for i in range(self.layer_boundaries.size - 1)
@@ -132,14 +143,16 @@
         layer_thicknes = np.array(layer_thicknes)
 
         self.data["layer middle"] = layer_middle
         self.data["layer thickness"] = layer_thicknes
         if len(self._height_mask) > n_layers:
             self._height_mask = np.delete(self._height_mask, -1)
         
+        
+        # check how the hardness is specified
         if old_hardness:
             self.isNewton = all(self.data["0534"] > 0)
             self.old_hardness = True
         else:
             self.isNewton = any(self.data["0534"] > 6) 
             self.old_hardness = False
```

### Comparing `snowpat-0.3.1/snowpat/snowpackreader/snowpackreader.py` & `snowpat-0.3.2/snowpat/snowpackreader/snowpackreader.py`

 * *Files identical despite different names*

### Comparing `snowpat-0.3.1/PKG-INFO` & `snowpat-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowpat
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: leibersp
 Author-email: patrick.leibersperger@slf.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,23 +23,31 @@
 There are two submodules:
 pysmet: Used to read and write SMET files
 snowpackreader: Used to read SNOWPACK output files (.pro) and handle profiles easily (soon also with visualization)
 SnowLense: Plotting Framework for files that can be read with this module (SMET not yet available) ([see Documentation](https://snowpat-patrick-leibersperger-c7ec84b7d2c6ab235482777a3905915fe.gitlab-pages.wsl.ch/indexplot/))
 
 ## News
 
+2024-03-25: Installation via PyPi now possible
+
 2024-03-08: Plotting of Snow Profiles is available with SnowLense module
 
 2024-03-01: A simple merge function is now available to join to SMET Files: merge(SMETFile, override) and mergeFromFile(filename, override)
 
 ## Installation
 
 Installation via pip and poetry is supported. 
 
-The easiest way to is to directly install from git (needs git to be installed):
+It is as easy as:
+
+```bash
+pip install snowpat
+```
+
+You can also install from git (needs git to be installed) to always get the latest release:
 
 ```bash
 pip install [--user] git+https://gitlabext.wsl.ch/patrick.leibersperger/snowpat.git
 ```
 
 the --user option might be needed if you do not have admin rights.
```

