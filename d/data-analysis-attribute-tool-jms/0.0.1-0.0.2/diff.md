# Comparing `tmp/data-analysis-attribute-tool-jms-0.0.1.tar.gz` & `tmp/data-analysis-attribute-tool-jms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-analysis-attribute-tool-jms-0.0.1.tar", last modified: Fri Mar 15 11:44:29 2024, max compression
+gzip compressed data, was "data-analysis-attribute-tool-jms-0.0.2.tar", last modified: Tue Apr  9 13:56:37 2024, max compression
```

## Comparing `data-analysis-attribute-tool-jms-0.0.1.tar` & `data-analysis-attribute-tool-jms-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.452492 data-analysis-attribute-tool-jms-0.0.1/
--rw-r--r--   0 jms        (501) staff       (20)     1067 2024-03-15 11:24:26.000000 data-analysis-attribute-tool-jms-0.0.1/LICENSE
--rw-r--r--   0 jms        (501) staff       (20)     1091 2024-03-15 11:44:29.451835 data-analysis-attribute-tool-jms-0.0.1/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)       86 2024-03-15 11:38:15.000000 data-analysis-attribute-tool-jms-0.0.1/README.md
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.440795 data-analysis-attribute-tool-jms-0.0.1/data/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 11:28:30.000000 data-analysis-attribute-tool-jms-0.0.1/data/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.441361 data-analysis-attribute-tool-jms-0.0.1/data/analysis/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 11:28:30.000000 data-analysis-attribute-tool-jms-0.0.1/data/analysis/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.441986 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 11:28:30.000000 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.442784 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/tool/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 11:28:30.000000 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/tool/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.444065 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/tool/jms/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 11:28:30.000000 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/tool/jms/__init__.py
--rw-r--r--   0 jms        (501) staff       (20)      512 2024-03-15 11:36:05.000000 data-analysis-attribute-tool-jms-0.0.1/data/analysis/attribute/tool/jms/data_attribute_obtain_tool.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 11:44:29.450036 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/
--rw-r--r--   0 jms        (501) staff       (20)     1091 2024-03-15 11:44:29.000000 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)      558 2024-03-15 11:44:29.000000 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/SOURCES.txt
--rw-r--r--   0 jms        (501) staff       (20)        1 2024-03-15 11:44:29.000000 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/dependency_links.txt
--rw-r--r--   0 jms        (501) staff       (20)      283 2024-03-15 11:44:29.000000 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/requires.txt
--rw-r--r--   0 jms        (501) staff       (20)        5 2024-03-15 11:44:29.000000 data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/top_level.txt
--rw-r--r--   0 jms        (501) staff       (20)      317 2024-03-15 11:38:28.000000 data-analysis-attribute-tool-jms-0.0.1/pyproject.toml
--rw-r--r--   0 jms        (501) staff       (20)      847 2024-03-15 11:44:29.454508 data-analysis-attribute-tool-jms-0.0.1/setup.cfg
--rw-r--r--   0 jms        (501) staff       (20)      147 2024-03-15 11:42:05.000000 data-analysis-attribute-tool-jms-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:56:37.330805 data-analysis-attribute-tool-jms-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-09 13:54:04.000000 data-analysis-attribute-tool-jms-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1123 2024-04-09 13:56:37.328829 data-analysis-attribute-tool-jms-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-04-09 13:54:50.000000 data-analysis-attribute-tool-jms-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 13:56:37.326823 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/
+-rw-rw-rw-   0        0        0     1123 2024-04-09 13:56:37.000000 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-04-09 13:56:37.000000 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:56:37.000000 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2024-04-09 13:56:37.000000 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:56:37.000000 data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      331 2024-04-09 13:54:04.000000 data-analysis-attribute-tool-jms-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      881 2024-04-09 13:56:37.332804 data-analysis-attribute-tool-jms-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      153 2024-04-09 13:54:04.000000 data-analysis-attribute-tool-jms-0.0.2/setup.py
```

### Comparing `data-analysis-attribute-tool-jms-0.0.1/PKG-INFO` & `data-analysis-attribute-tool-jms-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: data-analysis-attribute-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: jieba>=0.42.1
-Requires-Dist: setuptools>=42
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-attribute-tool-jms
-
-使用jieba工具，实现简单词性抽取接口
+Metadata-Version: 2.1
+Name: data-analysis-attribute-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: jieba>=0.42.1
+Requires-Dist: setuptools>=42
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+
+# data-analysis-attribute-tool-jms
+
+使用jieba工具，实现简单词性抽取接口。
```

### Comparing `data-analysis-attribute-tool-jms-0.0.1/data_analysis_attribute_tool_jms.egg-info/PKG-INFO` & `data-analysis-attribute-tool-jms-0.0.2/data_analysis_attribute_tool_jms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: data-analysis-attribute-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: jieba>=0.42.1
-Requires-Dist: setuptools>=42
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-attribute-tool-jms
-
-使用jieba工具，实现简单词性抽取接口
+Metadata-Version: 2.1
+Name: data-analysis-attribute-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-attribute-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: jieba>=0.42.1
+Requires-Dist: setuptools>=42
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+
+# data-analysis-attribute-tool-jms
+
+使用jieba工具，实现简单词性抽取接口。
```

