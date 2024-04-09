# Comparing `tmp/pyaogmaneo-2.4.3.tar.gz` & `tmp/pyaogmaneo-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.3.tar", last modified: Sat Apr  6 18:43:07 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.4.4.tar", last modified: Tue Apr  9 00:50:36 2024, max compression
```

## Comparing `pyaogmaneo-2.4.3.tar` & `pyaogmaneo-2.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:50:36.653925 pyaogmaneo-2.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:50:36.649925 pyaogmaneo-2.4.4/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 00:50:36.653925 pyaogmaneo-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:50:36.653925 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 00:50:36.000000 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 00:50:36.000000 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:50:36.000000 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:50:36.000000 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 00:50:36.000000 pyaogmaneo-2.4.4/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:50:36.653925 pyaogmaneo-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:50:36.649925 pyaogmaneo-2.4.4/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:50:36.653925 pyaogmaneo-2.4.4/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-04-09 00:50:23.000000 pyaogmaneo-2.4.4/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.4.3/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.4.4/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/CMakeLists.txt` & `pyaogmaneo-2.4.4/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 3a2ad0f486b83587237789922fe9326ba9b6b03f
+        GIT_TAG 6a9c378e11c57d01ee9d56c746979f057b3383d9
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.4.3/LICENSE.md` & `pyaogmaneo-2.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/PKG-INFO` & `pyaogmaneo-2.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.3/README.md` & `pyaogmaneo-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.4.4/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.3/setup.py` & `pyaogmaneo-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.4.3",
+    version="2.4.4",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
     if (std::get<2>(size) < 1)
         throw std::runtime_error("error: size[2] < 1 is not allowed!");
 
     if (num_dendrites_per_cell < 1)
         throw std::runtime_error("error: num_dendrites_per_cell < 1 is not allowed!");
 
+    if (value_num_dendrites_per_cell < 2)
+        throw std::runtime_error("error: value_num_dendrites_per_cell < 2 is not allowed!");
+
     if (up_radius < 0)
         throw std::runtime_error("error: up_radius < 0 is not allowed!");
 
     if (down_radius < 0)
         throw std::runtime_error("error: down_radius < 0 is not allowed!");
 
     if (history_capacity < 2)
@@ -107,14 +110,15 @@
     for (int i = 0; i < io_descs.size(); i++) {
         io_descs[i].check_in_range();
 
         c_io_descs[i] = aon::Hierarchy::IO_Desc(
             aon::Int3(std::get<0>(io_descs[i].size), std::get<1>(io_descs[i].size), std::get<2>(io_descs[i].size)),
             static_cast<aon::IO_Type>(io_descs[i].type),
             io_descs[i].num_dendrites_per_cell,
+            io_descs[i].value_num_dendrites_per_cell,
             io_descs[i].up_radius,
             io_descs[i].down_radius,
             io_descs[i].history_capacity
         );
     }
     
     aon::Array<aon::Hierarchy::Layer_Desc> c_layer_descs(layer_descs.size());
```

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_hierarchy.h`

 * *Files 2% similar despite different names*

```diff
@@ -10,45 +10,48 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int hierarchy_magic = 3141858;
+const int hierarchy_magic = 1249818;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
 struct IO_Desc {
     std::tuple<int, int, int> size;
     IO_Type type;
 
     int num_dendrites_per_cell;
+    int value_num_dendrites_per_cell;
 
     int up_radius;
     int down_radius;
 
     int history_capacity;
 
     IO_Desc(
         const std::tuple<int, int, int> &size,
         IO_Type type,
         int num_dendrites_per_cell,
+        int value_num_dendrites_per_cell,
         int up_radius,
         int down_radius,
         int history_capacity
     )
     :
     size(size),
     type(type),
     num_dendrites_per_cell(num_dendrites_per_cell),
+    value_num_dendrites_per_cell(value_num_dendrites_per_cell),
     up_radius(up_radius),
     down_radius(down_radius),
     history_capacity(history_capacity)
     {}
 
     void check_in_range() const;
 };
```

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.3/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.4.4/source/pyaogmaneo/py_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -32,26 +32,29 @@
     py::class_<pyaon::IO_Desc>(m, "IODesc")
         .def(py::init<
                 std::tuple<int, int, int>,
                 pyaon::IO_Type,
                 int,
                 int,
                 int,
+                int,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
             py::arg("io_type") = pyaon::prediction,
             py::arg("num_dendrites_per_cell") = 4,
+            py::arg("value_num_dendrites_per_cell") = 8,
             py::arg("up_radius") = 2,
             py::arg("down_radius") = 2,
             py::arg("history_capacity") = 256
         )
         .def_readwrite("size", &pyaon::IO_Desc::size)
         .def_readwrite("io_type", &pyaon::IO_Desc::type)
         .def_readwrite("num_dendrites_per_cell", &pyaon::IO_Desc::num_dendrites_per_cell)
+        .def_readwrite("value_num_dendrites_per_cell", &pyaon::IO_Desc::value_num_dendrites_per_cell)
         .def_readwrite("up_radius", &pyaon::IO_Desc::up_radius)
         .def_readwrite("down_radius", &pyaon::IO_Desc::down_radius)
         .def_readwrite("history_capacity", &pyaon::IO_Desc::history_capacity)
         .def("__copy__", 
             [](const pyaon::IO_Desc &other) {
                 return other;
             }
```

