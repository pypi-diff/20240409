# Comparing `tmp/telugu_words_numbers-0.0.1.tar.gz` & `tmp/telugu_words_numbers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telugu_words_numbers-0.0.1.tar", last modified: Tue Apr  9 08:42:31 2024, max compression
+gzip compressed data, was "telugu_words_numbers-0.0.2.tar", last modified: Tue Apr  9 15:23:21 2024, max compression
```

## Comparing `telugu_words_numbers-0.0.1.tar` & `telugu_words_numbers-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 sandeep.panchal (302844481) domain users (302800513)        0 2024-04-09 08:42:31.654644 telugu_words_numbers-0.0.1/
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)     4475 2024-04-09 08:42:31.650644 telugu_words_numbers-0.0.1/PKG-INFO
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)     2856 2024-04-09 06:16:24.000000 telugu_words_numbers-0.0.1/README.md
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)       38 2024-04-09 08:42:31.654644 telugu_words_numbers-0.0.1/setup.cfg
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)     1297 2024-04-09 06:14:16.000000 telugu_words_numbers-0.0.1/setup.py
-drwxr-xr-x   0 sandeep.panchal (302844481) domain users (302800513)        0 2024-04-09 08:42:31.650644 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)     4475 2024-04-09 08:42:31.000000 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/PKG-INFO
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)      237 2024-04-09 08:42:31.000000 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/SOURCES.txt
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)        1 2024-04-09 08:42:31.000000 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/dependency_links.txt
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)       18 2024-04-09 08:42:31.000000 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/requires.txt
--rw-r--r--   0 sandeep.panchal (302844481) domain users (302800513)        1 2024-04-09 08:42:31.000000 telugu_words_numbers-0.0.1/telugu_words_numbers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 15:23:21.410726 telugu_words_numbers-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3895 2024-04-09 15:23:21.402686 telugu_words_numbers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2958 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:23:21.410726 telugu_words_numbers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2024-04-09 15:18:59.000000 telugu_words_numbers-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:23:21.402686 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/
+-rw-rw-rw-   0        0        0     3895 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:23:21.000000 telugu_words_numbers-0.0.2/telugu_words_numbers.egg-info/top_level.txt
```

### Comparing `telugu_words_numbers-0.0.1/README.md` & `telugu_words_numbers-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-## Telugu Number-Words To Numbers Conversion
-
-### Overview
-- The Telugu Number-Words to Numbers Conversion package is a Python library that enables developers to convert numerical representations written in Telugu language text (using words) into their equivalent numerical values.
-
-### Features
-- Convert Telugu number-words to numerical values.
-- Supports a wide range of Telugu numerical representations.
-
-### Create a virtual environment if require with the python version 3.8 or more
-```
-conda create -n telugu_num_env python=3.8
-
-# Replace "telugu_num_env" with other name according to you
-```
-
-### Supporting packages to be installed (Additional packages can be installed if require)
-```
-text2digits
-numpy
-```
-
-### Installation with `pip'
-```
-# From CMD terminal
-pip install telugu-words-to-number
-
-
-# From IPYNB notebook
-!pip install telugu-words-to-number
-```
-
-### Inference
-```
-# In the CMD terminal, go to the home where inference.py is present and run it as below
-
-$ python3 inference.py
-
-# Note: Comment/uncomment as mentioned in the inference.py script
-```
-
-### Usage
-
-```
-# For single text conversion
-# Go to the path where telugu_word_to_number.py is present
-
-from telugu_word_to_number import TeluguWordsToNumber as tel_word_num
-
-# create an object instance
-obj = tel_word_num()
-
-text = "దీపిక కి అరవై పంపండి"
-number, converted_text = obj.word_number_conversion(text)
-print('Number: ', number)
-print('Original Text: ', text)
-print('Converted Text: ', converted_text)
-
-
-# Output
-
-Number:  60.0
-Original Text:  దీపిక కి అరవై పంపండి
-Converted Text:  దీపిక కి 60 పంపండి
-```
-```
-# For multiple texts conversion loop over list of Telugu texts
-# Go to the path where telugu_word_to_number.py is present
-
-from telugu_word_to_number import TeluguWordsToNumber as tel_word_num
-
-# create an object instance
-obj = tel_word_num()
-
-texts = [
-            "దీపిక కి అరవై పంపండి",
-            "భరత్ కి ఏడు వందలు పంపు"
-    ]
-
-for text in texts:
-    number, converted_text = obj.word_number_conversion(text)
-    print('Number: ', number)
-    print('Original Text: ', text)
-    print('Converted Text: ', converted_text)
-    print('-'*20, '\n')
-
-# Output
-
-Number:  60.0
-Original Text:  దీపిక కి అరవై పంపండి
-Converted Text:  దీపిక కి 60 పంపండి
--------------------- 
-
-Number:  700.0
-Original Text:  భరత్ కి ఏడు వందలు పంపు
-Converted Text:  భరత్ కి 700 పంపు
-
-```
-
-### Issues and Contributions
-If you encounter any issues or would like to contribute to this project, please visit the [GitHub repository](https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main).
-
+## Telugu Number-Words To Numbers Conversion
+
+### Overview
+- The Telugu Number-Words to Numbers Conversion package is a Python library that enables developers to convert numerical representations written in Telugu language text (using words) into their equivalent numerical values.
+
+### Features
+- Convert Telugu number-words to numerical values.
+- Supports a wide range of Telugu numerical representations.
+
+### Create a virtual environment if require with the python version 3.8 or more
+```
+conda create -n telugu_num_env python=3.8
+
+# Replace "telugu_num_env" with other name according to you
+```
+
+### Supporting packages to be installed (Additional packages can be installed if require)
+```
+text2digits
+numpy
+```
+
+### Installation with `pip'
+```
+# From CMD terminal
+pip install telugu-words-to-number
+
+
+# From IPYNB notebook
+!pip install telugu-words-to-number
+```
+
+### Inference
+```
+# In the CMD terminal, go to the home where inference.py is present and run it as below
+
+$ python3 inference.py
+
+# Note: Comment/uncomment as mentioned in the inference.py script
+```
+
+### Usage
+
+```
+# For single text conversion
+# Go to the path where telugu_word_to_number.py is present
+
+from telugu_word_to_number import TeluguWordsToNumber as tel_word_num
+
+# create an object instance
+obj = tel_word_num()
+
+text = "దీపిక కి అరవై పంపండి"
+number, converted_text = obj.word_number_conversion(text)
+print('Number: ', number)
+print('Original Text: ', text)
+print('Converted Text: ', converted_text)
+
+
+# Output
+
+Number:  60.0
+Original Text:  దీపిక కి అరవై పంపండి
+Converted Text:  దీపిక కి 60 పంపండి
+```
+```
+# For multiple texts conversion loop over list of Telugu texts
+# Go to the path where telugu_word_to_number.py is present
+
+from telugu_word_to_number import TeluguWordsToNumber as tel_word_num
+
+# create an object instance
+obj = tel_word_num()
+
+texts = [
+            "దీపిక కి అరవై పంపండి",
+            "భరత్ కి ఏడు వందలు పంపు"
+    ]
+
+for text in texts:
+    number, converted_text = obj.word_number_conversion(text)
+    print('Number: ', number)
+    print('Original Text: ', text)
+    print('Converted Text: ', converted_text)
+    print('-'*20, '\n')
+
+# Output
+
+Number:  60.0
+Original Text:  దీపిక కి అరవై పంపండి
+Converted Text:  దీపిక కి 60 పంపండి
+-------------------- 
+
+Number:  700.0
+Original Text:  భరత్ కి ఏడు వందలు పంపు
+Converted Text:  భరత్ కి 700 పంపు
+
+```
+
+### Issues and Contributions
+If you encounter any issues or would like to contribute to this project, please visit the [GitHub repository](https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main).
+
```

### Comparing `telugu_words_numbers-0.0.1/setup.py` & `telugu_words_numbers-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = fh.read()
-
-# Setting up
-setup(
-    name="telugu_words_numbers",
-    packages=find_packages(where="telugu_words_numbers"),
-    version='0.0.1',
-    license='MIT',
-    author="Sandeep Panchal",
-    author_email="sandeep.panchal545@gmail.com",
-    description='Telugu words to numbers conversion',
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    url="https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main",
-    project_urls ={
-            "Bug Tracker" : "https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues"
-        },
-    install_requires=["text2digits", "numpy"],
-    keywords=[
-        "telugu", "words", "numbers", "conversion", "words to number",
-        "words to number conversion", "telugu words number conversion",
-    ], 
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent"
-    ]
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = fh.read()
+
+# Setting up
+setup(
+    name="telugu_words_numbers",
+    packages=find_packages(where="telugu_words_numbers"),
+    version='0.0.2',
+    license='MIT',
+    author="Sandeep Panchal",
+    author_email="sandeep.panchal545@gmail.com",
+    description='Telugu words to numbers conversion',
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    url="https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main",
+    project_urls ={
+            "Bug Tracker" : "https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues"
+        },
+    install_requires=["text2digits", "numpy"],
+    keywords=[
+        "telugu", "words", "numbers", "conversion", "words to number",
+        "words to number conversion", "telugu words number conversion",
+    ], 
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent"
+    ]
 )
```

