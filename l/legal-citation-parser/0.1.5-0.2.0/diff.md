# Comparing `tmp/legal_citation_parser-0.1.5.tar.gz` & `tmp/legal_citation_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.1.5.tar", last modified: Sun Apr  7 01:26:01 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.2.0.tar", last modified: Tue Apr  9 03:12:41 2024, max compression
```

## Comparing `legal_citation_parser-0.1.5.tar` & `legal_citation_parser-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.5/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1940 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1606 2024-04-07 00:44:19.000000 legal_citation_parser-0.1.5/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/legal_citation_parser/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2024-04-06 23:11:08.000000 legal_citation_parser-0.1.5/legal_citation_parser/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.5/legal_citation_parser/canlii_constants.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6799 2024-04-06 23:56:27.000000 legal_citation_parser-0.1.5/legal_citation_parser/canlii_rules.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2024-04-07 01:23:43.000000 legal_citation_parser-0.1.5/legal_citation_parser/citation_parser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.5/legal_citation_parser/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1940 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      702 2024-04-07 01:25:55.000000 legal_citation_parser-0.1.5/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.2.0/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4756 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4421 2024-04-09 02:49:51.000000 legal_citation_parser-0.2.0/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/legal_citation_parser/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2024-04-07 01:51:59.000000 legal_citation_parser-0.2.0/legal_citation_parser/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    32481 2024-04-07 18:00:32.000000 legal_citation_parser-0.2.0/legal_citation_parser/canlii_constants.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8379 2024-04-09 02:03:30.000000 legal_citation_parser-0.2.0/legal_citation_parser/canlii_rules.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1023 2024-04-08 17:41:14.000000 legal_citation_parser-0.2.0/legal_citation_parser/citation_parser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3705 2024-04-09 02:09:14.000000 legal_citation_parser-0.2.0/legal_citation_parser/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4756 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      703 2024-04-07 18:00:32.000000 legal_citation_parser-0.2.0/setup.py
```

### Comparing `legal_citation_parser-0.1.5/LICENSE` & `legal_citation_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.5/legal_citation_parser/canlii_constants.py` & `legal_citation_parser-0.2.0/legal_citation_parser/canlii_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,8 +645,9 @@
     "ontario": "on",
     "prince edward island": "pe",
     "québec": "qc",
     "saskatchewan": "sk",
     "yukon": "yt",
     "northwest territories": "nt",
     "nunavut": "nu",
+    "federal": "ca",
 }
```

### Comparing `legal_citation_parser-0.1.5/legal_citation_parser/citation_parser.py` & `legal_citation_parser-0.2.0/legal_citation_parser/citation_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
-This Python module provides tools for extracting metadata information from legal citation strings.
+Extracts metadata information from legal citation strings.
 
 """
 
 from .canlii_rules import canlii_citation_parser
 
 def parse_citation(
-    citation: str, citation_type: str = "canlii", include_url: bool = False
+    citation: str, citation_type: str = "canlii", **kwargs
 ) -> dict:
     """
     Parses a citation string to extract key information about the court case.
 
     Args:
         citation (str): The citation string to parse.
         type (str): The type of citation to parse. Default is "canlii".
 
+    Keyword Args:
+        include_url (bool): A flag to determine whether to include the CanLII URL in the output.
+        
+
     Returns:
         dict: A dictionary containing the parsed information, including the style of cause,
         citation, citation type (neutral or CanLII), year, court code, decision number,
         jurisdiction, court name, and court level.
     """
 
     if citation_type == "canlii":
-        return canlii_citation_parser(citation, include_url=include_url)
+        return canlii_citation_parser(citation, **kwargs)
 
     elif "CanLII" in citation:
-        return canlii_citation_parser(citation)
+        return canlii_citation_parser(citation **kwargs)
 
     else:
         return None
```

### Comparing `legal_citation_parser-0.1.5/setup.py` & `legal_citation_parser-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='legal_citation_parser',
-    version='0.1.5',
-    description='Extract metadata from legal citations',
+    version='0.2.0',
+    description='Extracts metadata from legal citations',
     author='Daniel Nathan Booy',
     url='https://github.com/646e62/legal_citation_parser',
     author_email='444e42@protonmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

