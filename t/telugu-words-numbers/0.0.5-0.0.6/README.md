# Comparing `tmp/telugu_words_numbers-0.0.5.tar.gz` & `tmp/telugu_words_numbers-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telugu_words_numbers-0.0.5.tar", last modified: Tue Apr  9 17:51:26 2024, max compression
+gzip compressed data, was "telugu_words_numbers-0.0.6.tar", last modified: Tue Apr  9 18:31:49 2024, max compression
```

## Comparing `telugu_words_numbers-0.0.5.tar` & `telugu_words_numbers-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 17:51:26.373532 telugu_words_numbers-0.0.5/
--rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3363 2024-04-09 17:51:25.955049 telugu_words_numbers-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2735 2024-04-09 17:50:43.000000 telugu_words_numbers-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 17:51:26.373532 telugu_words_numbers-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1306 2024-04-09 17:37:19.000000 telugu_words_numbers-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:51:25.955049 telugu_words_numbers-0.0.5/telugu_words_numbers/
--rw-rw-rw-   0        0        0      122 2024-04-09 17:46:35.000000 telugu_words_numbers-0.0.5/telugu_words_numbers/__init__.py
--rw-rw-rw-   0        0        0     7806 2024-04-09 17:46:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers/telugu_word_to_number.py
-drwxrwxrwx   0        0        0        0 2024-04-09 17:51:25.955049 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/
--rw-rw-rw-   0        0        0     3363 2024-04-09 17:51:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-09 17:51:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:51:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 17:51:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-09 17:51:25.000000 telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3372 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2695 2024-04-09 18:04:30.000000 telugu_words_numbers-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2024-04-09 18:31:41.000000 telugu_words_numbers-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.104223 telugu_words_numbers-0.0.6/telugu_words_numbers/
+-rw-rw-rw-   0        0        0      122 2024-04-09 17:46:35.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/
+-rw-rw-rw-   0        0        0      214 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/telugu_currency_units.json
+-rw-rw-rw-   0        0        0    11500 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/telugu_numbers.json
+-rw-rw-rw-   0        0        0     7806 2024-04-09 18:28:11.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/telugu_word_to_number.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.104223 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/
+-rw-rw-rw-   0        0        0     3372 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/top_level.txt
```

### Comparing `telugu_words_numbers-0.0.5/LICENSE` & `telugu_words_numbers-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.5/PKG-INFO` & `telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telugu_words_numbers
-Version: 0.0.5
+Name: telugu-words-numbers
+Version: 0.0.6
 Summary: Telugu words to numbers conversion
 Home-page: https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main
 Author: Sandeep Panchal
 Author-email: sandeep.panchal545@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues
 Keywords: telugu,words,numbers,conversion,words to number,words to number conversion,telugu words number conversion
@@ -25,81 +25,70 @@
 ### Features
 - Convert Telugu number-words to numerical values.
 - Supports a wide range of Telugu numerical representations.
 
 ### Create a virtual environment if require with the python version 3.8 or more
 ```
 conda create -n telugu_num_env python=3.8
-
 # Replace "telugu_num_env" with other name according to you
 ```
 
 ### Supporting packages to be installed (Additional packages can be installed if require)
 ```
 text2digits
 numpy
 ```
 
 ### Installation with `pip'
 ```
 # From CMD terminal
 pip install telugu-words-numbers
 
-
 # From IPYNB notebook
 !pip install telugu-words-numbers
 ```
 
-### Usage
-
+### Usage for single text conversion
 ```
-# For single text conversion
 from telugu_words_numbers import TeluguWordsToNumber
-
 # creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
-
 text = "దీపిక కి అరవై పంపండి"
 number, converted_text = converter.word_number_conversion(text)
 print('Number: ', number)
 print('Original Text: ', text)
 print('Converted Text: ', converted_text)
+```
 
-
-# Output
-
+### Out of single text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 ```
+### Usage for multiple text conversion
 ```
-# For multiple texts conversion loop over list of Telugu texts
 from telugu_words_numbers import TeluguWordsToNumber
-
 # creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
-
 texts = [
             "దీపిక కి అరవై పంపండి",
             "భరత్ కి ఏడు వందలు పంపు"
     ]
-
 for text in texts:
     number, converted_text = converter.word_number_conversion(text)
     print('Number: ', number)
     print('Original Text: ', text)
     print('Converted Text: ', converted_text)
     print('-'*20, '\n')
-
-# Output
-
+```
+### Output of multiple text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 -------------------- 
-
 Number:  700.0
 Original Text:  భరత్ కి ఏడు వందలు పంపు
 Converted Text:  భరత్ కి 700 పంపు
-```
-
+```
```

### Comparing `telugu_words_numbers-0.0.5/README.md` & `telugu_words_numbers-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -35,64 +35,58 @@
 # In the CMD terminal, go to the home where inference.py is present and run it as below
 
 $ python3 inference.py
 
 # Note: Comment/uncomment as mentioned in the inference.py script
 ```
 
-### Usage
 
+### Usage for single text conversion
 ```
-# For single text conversion
-# Go to the path where telugu_word_to_number.py is present
+from telugu_words_numbers import TeluguWordsToNumber
 
-from telugu_word_to_number import TeluguWordsToNumber
-
-# create an object instance
+# creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
 
 text = "దీపిక కి అరవై పంపండి"
 number, converted_text = converter.word_number_conversion(text)
 print('Number: ', number)
 print('Original Text: ', text)
 print('Converted Text: ', converted_text)
+```
 
-
-# Output
-
+### Out of single text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 ```
 
+### Usage for multiple text conversion
 ```
-# For multiple texts conversion loop over list of Telugu texts
-# Go to the path where telugu_word_to_number.py is present
-
-from telugu_word_to_number import TeluguWordsToNumber
+from telugu_words_numbers import TeluguWordsToNumber
 
-# create an object instance
+# creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
-
 texts = [
             "దీపిక కి అరవై పంపండి",
             "భరత్ కి ఏడు వందలు పంపు"
     ]
 
 for text in texts:
     number, converted_text = converter.word_number_conversion(text)
     print('Number: ', number)
     print('Original Text: ', text)
     print('Converted Text: ', converted_text)
     print('-'*20, '\n')
+```
 
-# Output
-
+### Output of multiple text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 -------------------- 
-
 Number:  700.0
 Original Text:  భరత్ కి ఏడు వందలు పంపు
 Converted Text:  భరత్ కి 700 పంపు
 ```
```

### Comparing `telugu_words_numbers-0.0.5/setup.py` & `telugu_words_numbers-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 with codecs.open(os.path.join(here, "README.srt"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setting up
 setup(
     name="telugu_words_numbers",
     packages=find_packages(),
-    version='0.0.5',
+    package_data={'telugu_words_numbers': ['json_files/*.json']},
+    version='0.0.6',
     license='MIT',
     author="Sandeep Panchal",
     author_email="sandeep.panchal545@gmail.com",
     description='Telugu words to numbers conversion',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main",
```

### Comparing `telugu_words_numbers-0.0.5/telugu_words_numbers/telugu_word_to_number.py` & `telugu_words_numbers-0.0.6/telugu_words_numbers/telugu_word_to_number.py`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.5/telugu_words_numbers.egg-info/PKG-INFO` & `telugu_words_numbers-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: telugu-words-numbers
-Version: 0.0.5
+Name: telugu_words_numbers
+Version: 0.0.6
 Summary: Telugu words to numbers conversion
 Home-page: https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main
 Author: Sandeep Panchal
 Author-email: sandeep.panchal545@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/issues
 Keywords: telugu,words,numbers,conversion,words to number,words to number conversion,telugu words number conversion
@@ -25,81 +25,70 @@
 ### Features
 - Convert Telugu number-words to numerical values.
 - Supports a wide range of Telugu numerical representations.
 
 ### Create a virtual environment if require with the python version 3.8 or more
 ```
 conda create -n telugu_num_env python=3.8
-
 # Replace "telugu_num_env" with other name according to you
 ```
 
 ### Supporting packages to be installed (Additional packages can be installed if require)
 ```
 text2digits
 numpy
 ```
 
 ### Installation with `pip'
 ```
 # From CMD terminal
 pip install telugu-words-numbers
 
-
 # From IPYNB notebook
 !pip install telugu-words-numbers
 ```
 
-### Usage
-
+### Usage for single text conversion
 ```
-# For single text conversion
 from telugu_words_numbers import TeluguWordsToNumber
-
 # creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
-
 text = "దీపిక కి అరవై పంపండి"
 number, converted_text = converter.word_number_conversion(text)
 print('Number: ', number)
 print('Original Text: ', text)
 print('Converted Text: ', converted_text)
+```
 
-
-# Output
-
+### Out of single text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 ```
+### Usage for multiple text conversion
 ```
-# For multiple texts conversion loop over list of Telugu texts
 from telugu_words_numbers import TeluguWordsToNumber
-
 # creating and object of the class TeluguWordsToNum
 converter = TeluguWordsToNumber()
-
 texts = [
             "దీపిక కి అరవై పంపండి",
             "భరత్ కి ఏడు వందలు పంపు"
     ]
-
 for text in texts:
     number, converted_text = converter.word_number_conversion(text)
     print('Number: ', number)
     print('Original Text: ', text)
     print('Converted Text: ', converted_text)
     print('-'*20, '\n')
-
-# Output
-
+```
+### Output of multiple text conversion
+```
 Number:  60.0
 Original Text:  దీపిక కి అరవై పంపండి
 Converted Text:  దీపిక కి 60 పంపండి
 -------------------- 
-
 Number:  700.0
 Original Text:  భరత్ కి ఏడు వందలు పంపు
 Converted Text:  భరత్ కి 700 పంపు
-```
-
+```
```

