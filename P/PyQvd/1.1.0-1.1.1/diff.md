# Comparing `tmp/PyQvd-1.1.0.tar.gz` & `tmp/PyQvd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQvd-1.1.0.tar", last modified: Sun Apr  7 10:49:23 2024, max compression
+gzip compressed data, was "PyQvd-1.1.1.tar", last modified: Tue Apr  9 12:29:24 2024, max compression
```

## Comparing `PyQvd-1.1.0.tar` & `PyQvd-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.544315 PyQvd-1.1.0/
--rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 PyQvd-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0    12492 2024-04-07 10:49:23.543112 PyQvd-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.540811 PyQvd-1.1.0/PyQvd.egg-info/
--rw-rw-rw-   0        0        0    12492 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 PyQvd-1.1.0/README.md
--rw-rw-rw-   0        0        0     1288 2024-04-07 10:48:28.000000 PyQvd-1.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.534321 PyQvd-1.1.0/pyqvd/
--rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 PyQvd-1.1.0/pyqvd/__init__.py
--rw-rw-rw-   0        0        0    37372 2024-04-07 10:48:20.000000 PyQvd-1.1.0/pyqvd/qvd.py
--rw-rw-rw-   0        0        0       42 2024-04-07 10:49:23.545661 PyQvd-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 12:29:24.249535 PyQvd-1.1.1/
+-rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 PyQvd-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    12492 2024-04-09 12:29:24.247620 PyQvd-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 12:29:24.246020 PyQvd-1.1.1/PyQvd.egg-info/
+-rw-rw-rw-   0        0        0    12492 2024-04-09 12:29:24.000000 PyQvd-1.1.1/PyQvd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-09 12:29:24.000000 PyQvd-1.1.1/PyQvd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 12:29:24.000000 PyQvd-1.1.1/PyQvd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-09 12:29:24.000000 PyQvd-1.1.1/PyQvd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 12:29:24.000000 PyQvd-1.1.1/PyQvd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 PyQvd-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1288 2024-04-09 12:27:38.000000 PyQvd-1.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-09 12:29:24.243890 PyQvd-1.1.1/pyqvd/
+-rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 PyQvd-1.1.1/pyqvd/__init__.py
+-rw-rw-rw-   0        0        0    37738 2024-04-09 12:27:08.000000 PyQvd-1.1.1/pyqvd/qvd.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 12:29:24.249535 PyQvd-1.1.1/setup.cfg
```

### Comparing `PyQvd-1.1.0/LICENSE.md` & `PyQvd-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyQvd-1.1.0/PKG-INFO` & `PyQvd-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyQvd-1.1.0/PyQvd.egg-info/PKG-INFO` & `PyQvd-1.1.1/PyQvd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyQvd-1.1.0/README.md` & `PyQvd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PyQvd-1.1.0/pyproject.toml` & `PyQvd-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyQvd"
-version = "1.1.0"
+version = "1.1.1"
 description = "Utility library for reading/writing Qlik View Data (QVD) files in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.md"}
 authors = [
     {name = "Constantin Müller", email = "info@mueller-constantin.de"},
 ]
 keywords = ["qlik", "qvd", "qlik sense", "qlik view", "pandas"]
```

### Comparing `PyQvd-1.1.0/pyqvd/qvd.py` & `PyQvd-1.1.1/pyqvd/qvd.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,28 +81,29 @@
         Converts the symbol to its byte representation.
 
         :return: The byte representation of the symbol.
         """
         if self._int_value is not None and self._string_value is not None:
             return (b"\05" +
                     self._int_value.to_bytes(4, byteorder="little", signed=True) +
-                    str.encode(self._string_value) +
+                    str.encode(self._string_value, encoding="utf-8") +
                     b"\0")
 
         if self._double_value is not None and self._string_value is not None:
-            return b"\06" + struct.pack("<d", self._double_value) + str.encode(self._string_value) + b"\0"
+            return (b"\06" + struct.pack("<d", self._double_value) +
+                    str.encode(self._string_value, encoding="utf-8") + b"\0")
 
         if self._int_value is not None:
             return b"\01" + self._int_value.to_bytes(4, byteorder="little", signed=True)
 
         if self._double_value is not None:
             return b"\02" + struct.pack("<d", self._double_value)
 
         if self._string_value is not None:
-            return b"\04" + str.encode(self._string_value) + b"\0"
+            return b"\04" + str.encode(self._string_value, encoding="utf-8") + b"\0"
 
         raise ValueError("The symbol does not contain any value.")
 
     def __eq__(self, __value: object) -> bool:
         """
         Determines whether this symbol is equal to another object.
 
@@ -427,44 +428,47 @@
                     symbols.append(QvdSymbol.from_int_value(value))
                 elif type_byte == 2:
                     byte_data = symbol_buffer[pointer:pointer + 8]
                     value = struct.unpack("<d", byte_data)[0]
                     pointer += 8
                     symbols.append(QvdSymbol.from_double_value(value))
                 elif type_byte == 4:
-                    value = ""
+                    byte_data = bytearray()
 
                     while symbol_buffer[pointer] != 0:
-                        value += chr(symbol_buffer[pointer])
+                        byte_data.append(symbol_buffer[pointer])
                         pointer += 1
 
+                    value = byte_data.decode(encoding="utf-8")
                     pointer += 1
                     symbols.append(QvdSymbol.from_string_value(value))
                 elif type_byte == 5:
-                    byte_data = symbol_buffer[pointer:pointer + 4]
-                    int_value = int.from_bytes(byte_data, byteorder="little", signed=True)
+                    int_byte_data = symbol_buffer[pointer:pointer + 4]
+                    int_value = int.from_bytes(int_byte_data, byteorder="little", signed=True)
                     pointer += 4
 
-                    string_value = ""
+                    string_byte_data = bytearray()
                     while symbol_buffer[pointer] != 0:
-                        string_value += chr(symbol_buffer[pointer])
+                        string_byte_data.append(symbol_buffer[pointer])
                         pointer += 1
 
+                    string_value = string_byte_data.decode(encoding="utf-8")
                     pointer += 1
                     symbols.append(QvdSymbol.from_dual_int_value(int_value, string_value))
                 elif type_byte == 6:
-                    byte_data = symbol_buffer[pointer:pointer + 8]
-                    double_value = struct.unpack("<d", byte_data)[0]
+                    double_byte_data = symbol_buffer[pointer:pointer + 8]
+                    double_value = struct.unpack("<d", double_byte_data)[0]
                     pointer += 8
 
-                    string_value = ""
+                    string_byte_data = bytearray()
                     while symbol_buffer[pointer] != 0:
                         string_value += chr(symbol_buffer[pointer])
                         pointer += 1
 
+                    string_value = string_byte_data.decode(encoding="utf-8")
                     pointer += 1
                     symbols.append(QvdSymbol.from_dual_double_value(double_value, string_value))
                 else:
                     raise ValueError("The symbol type byte is not recognized. Unknown data type: " + hex(type_byte))
 
             self._symbol_table[index] = symbols
```

