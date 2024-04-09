# Comparing `tmp/telugu_words_numbers-0.0.2.tar.gz` & `tmp/telugu_words_numbers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telugu_words_numbers-0.0.2.tar", last modified: Tue Apr  9 15:23:21 2024, max compression
+gzip compressed data, was "telugu_words_numbers-0.0.3.tar", last modified: Tue Apr  9 15:36:10 2024, max compression
```

## Comparing `telugu_words_numbers-0.0.2.tar` & `telugu_words_numbers-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:23:21.410726 telugu_words_numbers-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3895 2024-04-09 15:23:21.402686 telugu_words_numbers-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2958 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 15:23:21.410726 telugu_words_numbers-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1333 2024-04-09 15:18:59.000000 telugu_words_numbers-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:23:21.402686 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/
--rw-rw-rw-   0        0        0     3895 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 15:36:10.775710 telugu_words_numbers-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3895 2024-04-09 15:36:10.767753 telugu_words_numbers-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2958 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:36:10.775710 telugu_words_numbers-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1305 2024-04-09 15:33:25.000000 telugu_words_numbers-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:36:10.337329 telugu_words_numbers-0.0.3/telugu_words_numbers/
+-rw-rw-rw-   0        0        0      102 2024-04-09 15:34:40.000000 telugu_words_numbers-0.0.3/telugu_words_numbers/__init__.py
+-rw-rw-rw-   0        0        0     8027 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.3/telugu_words_numbers/telugu_word_to_number.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:36:10.354173 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/
+-rw-rw-rw-   0        0        0     3895 2024-04-09 15:36:10.000000 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-04-09 15:36:10.000000 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:36:10.000000 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 15:36:10.000000 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 15:36:10.000000 telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/top_level.txt
```

### Comparing `telugu_words_numbers-0.0.2/LICENSE` & `telugu_words_numbers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.2/PKG-INFO` & `telugu_words_numbers-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telugu_words_numbers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Telugu words to numbers conversion
 Home-page: https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main
 Author: Sandeep Panchal
 Author-email: sandeep.panchal545@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues
 Keywords: telugu,words,numbers,conversion,words to number,words to number conversion,telugu words number conversion
```

### Comparing `telugu_words_numbers-0.0.2/README.md` & `telugu_words_numbers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.2/setup.py` & `telugu_words_numbers-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setting up
 setup(
     name="telugu_words_numbers",
-    packages=find_packages(where="telugu_words_numbers"),
-    version='0.0.2',
+    packages=find_packages(),
+    version='0.0.3',
     license='MIT',
     author="Sandeep Panchal",
     author_email="sandeep.panchal545@gmail.com",
     description='Telugu words to numbers conversion',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main",
```

### Comparing `telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/PKG-INFO` & `telugu_words_numbers-0.0.3/telugu_words_numbers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telugu-words-numbers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Telugu words to numbers conversion
 Home-page: https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main
 Author: Sandeep Panchal
 Author-email: sandeep.panchal545@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues
 Keywords: telugu,words,numbers,conversion,words to number,words to number conversion,telugu words number conversion
```

