# Comparing `tmp/yamld-0.0.22.tar.gz` & `tmp/yamld-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamld-0.0.22.tar", last modified: Fri Mar 15 13:27:29 2024, max compression
+gzip compressed data, was "yamld-0.0.3.tar", last modified: Mon Apr  8 16:53:23 2024, max compression
```

## Comparing `yamld-0.0.22.tar` & `yamld-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,24 @@
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-03-15 13:27:29.748070 yamld-0.0.22/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1069 2024-02-04 15:37:23.000000 yamld-0.0.22/LICENSE
--rw-r--r--   0 hunter    (1000) hunter    (1000)      412 2024-03-15 13:27:29.748070 yamld-0.0.22/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2472 2024-02-21 10:22:48.000000 yamld-0.0.22/README.md
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-03-15 13:27:29.744072 yamld-0.0.22/bin/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3096 2024-03-15 13:26:30.000000 yamld-0.0.22/bin/csv2yamld
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2148 2024-02-13 15:56:45.000000 yamld-0.0.22/bin/yamld
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1582 2024-02-10 20:22:37.000000 yamld-0.0.22/bin/yamld2csv
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       81 2024-02-04 17:15:45.000000 yamld-0.0.22/pyproject.toml
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2024-03-15 13:27:29.748070 yamld-0.0.22/setup.cfg
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      659 2024-03-15 13:26:10.000000 yamld-0.0.22/setup.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-03-15 13:27:29.744072 yamld-0.0.22/tests/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        0 2024-02-06 15:52:18.000000 yamld-0.0.22/tests/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2103 2024-02-20 15:25:57.000000 yamld-0.0.22/tests/test_read.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2079 2024-02-12 14:31:14.000000 yamld-0.0.22/tests/test_read_mini.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1381 2024-02-10 12:57:05.000000 yamld-0.0.22/tests/test_read_with_nulls.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1368 2024-02-12 13:49:34.000000 yamld-0.0.22/tests/test_write.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1322 2024-02-12 13:50:36.000000 yamld-0.0.22/tests/test_write_mini.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1183 2024-02-07 12:53:32.000000 yamld-0.0.22/tests/test_write_with_nulls.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-03-15 13:27:29.744072 yamld-0.0.22/yamld/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      328 2024-03-01 14:45:22.000000 yamld-0.0.22/yamld/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1769 2024-02-20 13:09:22.000000 yamld-0.0.22/yamld/common.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)    10357 2024-02-12 14:28:41.000000 yamld-0.0.22/yamld/read.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     4598 2024-03-01 14:45:22.000000 yamld-0.0.22/yamld/write.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-03-15 13:27:29.748070 yamld-0.0.22/yamld.egg-info/
--rw-r--r--   0 hunter    (1000) hunter    (1000)      412 2024-03-15 13:27:29.000000 yamld-0.0.22/yamld.egg-info/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      453 2024-03-15 13:27:29.000000 yamld-0.0.22/yamld.egg-info/SOURCES.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2024-03-15 13:27:29.000000 yamld-0.0.22/yamld.egg-info/dependency_links.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       14 2024-03-15 13:27:29.000000 yamld-0.0.22/yamld.egg-info/requires.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        6 2024-03-15 13:27:29.000000 yamld-0.0.22/yamld.egg-info/top_level.txt
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/
+-rw-r--r--   0 hunter    (1000) hunter    (1000)      395 2024-04-08 16:53:23.101043 yamld-0.0.3/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2187 2024-04-08 16:48:54.000000 yamld-0.0.3/README.md
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/bin/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3233 2024-04-08 11:42:17.000000 yamld-0.0.3/bin/csv2yamld
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2202 2024-04-08 11:48:25.000000 yamld-0.0.3/bin/yamld
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1659 2024-04-08 11:08:12.000000 yamld-0.0.3/bin/yamld2csv
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2024-04-08 16:53:23.101043 yamld-0.0.3/setup.cfg
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      652 2024-04-08 16:51:00.000000 yamld-0.0.3/setup.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/tests/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1077 2024-04-06 15:40:32.000000 yamld-0.0.3/tests/test_basic_parse_test.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/yamld/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      534 2024-04-06 19:00:33.000000 yamld-0.0.3/yamld/__init__.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      332 2024-04-08 11:36:44.000000 yamld-0.0.3/yamld/common.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3394 2024-04-08 14:47:35.000000 yamld-0.0.3/yamld/parser.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1814 2024-04-08 14:49:37.000000 yamld-0.0.3/yamld/with_iofile.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1433 2024-04-08 14:40:39.000000 yamld-0.0.3/yamld/with_pandas.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2660 2024-04-08 11:28:42.000000 yamld-0.0.3/yamld/writer.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/yamld.egg-info/
+-rw-r--r--   0 hunter    (1000) hunter    (1000)      395 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      339 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       14 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/requires.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        6 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/top_level.txt
```

### Comparing `yamld-0.0.22/README.md` & `yamld-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# YAMLd
+# yaml-datasets (YAMLd)
 
-**YAMLd** is a tiny subset of *YAML* designed specifically for representing tabular data (for now, only *CSV*). It is particularly useful for datasets with numerous features or lengthy sequences that are hard to read. The **D** stands for data!
+YAML datasets (**YAMLd**) is a tiny subset of *YAML* designed specifically for representing tabular data (such as **CSV**). It is particularly useful for datasets with numerous features or lengthy sequences that are hard to read.
 
 ### YAMLd Rules:
 
-- The hyphen symbol (`-`) is  only used to list the dataset. Other use cases are not permited.
-- Each file contains only one dataset and optional meta data.
-- Meta data are listed before the dataset.
-- Meta data does not contain nested dictionaries, only key-value maps.
+- The file ends with a top-level key *data* or *dataset* that contain the list of entries in the dataset
+- Everything before is considered meta-data
     
 ### Example
 
 ``` yaml
 features_description:
   name: 'embloyee name'
   age: 'age'
   city: 'closest city to adress'
 
 extra: 3.4
 
-whatever_name_for_your_data:
+dataset:
   - name: 'John Doe'
     age: 30
     city: 'New York'
   - name: 'Jane Smith'
     age: 25
     city: 'San Francisco'
   - name: 'Bob Johnson'
@@ -31,28 +29,27 @@
     city: 'Chicago'
 ```
 
 Using a 'mini' version of this, you can remove the feature names from each line as follows.
 
 ``` yaml
 data:
-  - - name:
-    - age: 
-    - city:
-  - - 'John Doe'
-    - 30
-    - 'New York'
+  - name: 'John Doe'
+    age: 30
+    city: 'New York'
   - - 'Jane Smith'
     - 25
     - 'San Francisco'
   - - 'Bob Johnson'
     - 35
     - 'Chicago'
 ```
 
+You can also remove feature names completly.
+
 **Note:** It is still experimental, use it with caution.
 
 ## Convert CSV to YAMLd and vice versa:
 ```console
 csv2yamld <your-csv-file>
 ```
 
@@ -73,21 +70,18 @@
 
 
 ## Setup
 ```console 
 pip install -U yamld
 ```
 
-To install without virtual environments, you can use [*pipx*](https://github.com/pypa/pipx). Another option is to pass `--break-system-packages` to *pip*, but it's not advisable.
+To install without virtual environments, you can use [*pipx*](https://github.com/pypa/pipx).
 
 ## Details
-The main goal is to edit and view your data files with nothing but your text editor. Consequently, a lot of YAML features are not supported, as their inclusion could either introduce clutter or hinder the parsing efficiency for datasets.
+The main goal is to edit and view your data files with nothing but your text editor. Consequently, a lot of YAML features are not parsed after the top-level key-word `data` or `dataset`, as their inclusion could either introduce clutter or hinder the parsing efficiency for dataset. For example, YAML explicit types markings and comments are not supported.
+
 
 ### Data Types:
 - Dataset data types:
     - List: surrounded with `[]`
     - String: surrounded with `""` or `''` 
-    - Number
-- Meta data has one extra data type:
-    - key-value maps: value can only be one of the other types used for the dataset.
-    
- **Note:** YAML explicit types marking and comments are not supported.
+    - Number
```

### Comparing `yamld-0.0.22/bin/csv2yamld` & `yamld-0.0.3/bin/csv2yamld`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/env python
 
 import pandas as pd
 import argparse
 from pathlib import Path
 import sys
 
-from yamld.write import write_dataframe
+from yamld.with_iofile import write_dataframe
 
 
-def df2yaml(df, inpath, outpath, is_mini, stdout=False):
+def df2yaml(df, inpath, outpath, is_min, stdout=False):
     inpath = Path(inpath)
     suffix = inpath.suffix
     if stdout:
-        write_dataframe(sys.stdout, df, name='data', is_mini=is_mini)
+        write_dataframe(sys.stdout, df, name='data', is_min=is_min)
     else:
         if outpath:
             outpath = Path(outpath)
         else:
             outpath = inpath.with_suffix('.yaml')
+            
+        if Path(outpath).exists():
+            raise Exception("Output file already exist: " + str(outpath))
+            
         with open(outpath, 'w') as f:
-            write_dataframe(f, df, name='data', is_mini=is_mini)
+            write_dataframe(f, df, is_min=is_min)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Read CSV file using Pandas read_csv() function.')
 
     parser.add_argument('file_path', type=str, help='Path to the CSV file')
 
@@ -61,16 +65,16 @@
     # Read CSV file using Pandas read_csv() function
     try:
         separator = args.separator if not args.table else '\t'
         df = pd.read_csv(args.file_path, sep=separator, nrows= args.nrows,
                          skiprows= args.skiprows, header=0 if args.header else None,
                          usecols=args.columns, comment=args.comment, encoding=args.encoding)
         df2yaml(df, args.file_path, args.output_file, args.mini, args.stdout)
-    except FileNotFoundError:
-        print(f"Error: File not found at {args.file_path}")
-    except pd.errors.EmptyDataError:
-        print(f"Error: The CSV file at {args.file_path} is empty")
+    except FileNotFoundError as e:
+        raise type(e)(f"File not found: {args.file_path}")
+    except pd.errors.EmptyDataError as e:
+        raise type(e)(f"The input CSV file is empty: {args.file_path}")
 
 
 # Run the main function
 if __name__ == "__main__":
     main()
```

### Comparing `yamld-0.0.22/bin/yamld` & `yamld-0.0.3/bin/yamld`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #!/usr/bin/env python
 
 import argparse
 from pathlib import Path
 import pandas as pd
 
-from yamld.read import read_onelist_dataframe_from_file
-from yamld.write import write_dataframe_from_path
+from yamld.with_iofile import read_dataframe
+from yamld.with_iofile import write_dataframe
 
 
-def yaml2yaml(inpath, outpath=None, skiprows=None, nrows=None, is_mini=False, encoding='utf-8'):
+def yaml2yaml(inpath, outpath=None, skiprows=None, nrows=None, is_min=False, encoding='utf-8'):
     inpath = Path(inpath)
     suffix = inpath.suffix
     if outpath:
         outpath = Path(outpath)
     else:
         outpath = inpath.with_suffix('.mini.yaml')
 
-    df = read_onelist_dataframe_from_file(inpath)
-    write_dataframe_from_path(outpath, df.iloc[skiprows:nrows], is_mini=is_mini, encoding=encoding)
+    if Path(outpath).exists():
+        raise Exception("Output file already exist: " + str(outpath))
+
+    df = read_dataframe(inpath)
+    write_dataframe(outpath, df.iloc[skiprows:nrows], is_min=is_min, encoding=encoding)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Read CSV file using Pandas read_csv() function.')
 
     parser.add_argument('file_path', type=str, help='Path to the CSV file')
 
-
     # Optional arguments
     parser.add_argument('-o', '--output', type=str, default=None,
                         help='Character indicating the start of a comment line in the CSV file')
 
     parser.add_argument('-m', '--mini', action='store_true',
                         help='Specify if the CSV file has a header row')
 
@@ -44,15 +46,15 @@
 def main():
     # Check if the script is being run as the main program
     # Parse command line arguments
     args = parse_arguments()
 
     # Read CSV file using Pandas read_csv() function
     try:
-        yaml2yaml(args.file_path, args.output, skiprows=args.skiprows, nrows=args.nrows, is_mini=args.mini, encoding=args.encoding)
+        yaml2yaml(args.file_path, args.output, skiprows=args.skiprows, nrows=args.nrows, is_min=args.mini, encoding=args.encoding)
     except FileNotFoundError:
         print(f"Error: File not found at {args.file_path}")
     except pd.errors.EmptyDataError:
         print(f"Error: The CSV file at {args.file_path} is empty")
 
 
 # Run the main function
```

### Comparing `yamld-0.0.22/bin/yamld2csv` & `yamld-0.0.3/bin/yamld2csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python
 
 import argparse
 from pathlib import Path
 import pandas as pd
 
-from yamld.read import read_onelist_dataframe
+from yamld.with_iofile import read_dataframe
 
 
 def yaml2csv(inpath, outpath=None, encoding='utf-8'):
     inpath = Path(inpath)
     suffix = inpath.suffix
     if outpath:
         outpath = Path(outpath)
     else:
-        outpath = inpath.with_suffix('.yaml')
+        outpath = inpath.with_suffix('.csv')
+        
+    if Path(outpath).exists():
+        raise Exception("Output file already exist: " + str(outpath))
 
-    with open(inpath, 'r') as f:
-        df = read_onelist_dataframe(f)
+    df = read_dataframe(inpath)
     df.to_csv(outpath, encoding=encoding, index=False)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Read CSV file using Pandas read_csv() function.')
 
     parser.add_argument('file_path', type=str, help='Path to the CSV file')
@@ -38,16 +40,16 @@
     # Check if the script is being run as the main program
     # Parse command line arguments
     args = parse_arguments()
 
     # Read CSV file using Pandas read_csv() function
     try:
         yaml2csv(args.file_path, args.output, args.encoding)
-    except FileNotFoundError:
-        print(f"Error: File not found at {args.file_path}")
-    except pd.errors.EmptyDataError:
-        print(f"Error: The CSV file at {args.file_path} is empty")
+    except FileNotFoundError as e:
+        raise type(e)(f"File not found: {args.file_path}")
+    except pd.errors.EmptyDataError as e:
+        raise type(e)(f"The YAML file is empty: {args.file_path}")
 
 
 # Run the main function
 if __name__ == "__main__":
     main()
```

### Comparing `yamld-0.0.22/setup.py` & `yamld-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# setup.py
-
 from setuptools import setup, find_packages
 
 setup(
     name='yamld',
-    version='0.0.22',
+    version='0.0.3',
     author='Yahya Badran',
     author_email='techtweaking@gmail.com',
     description='parser of YAMLd, a tiny subset of YAML',
-    url='https://github.com/badranx/YAML-2D',
+    url='https://github.com/badranx/yaml-datasets',
     install_requires=['pandas >= 1.0.0'],
     packages = [package for package in find_packages() if package.startswith("yamld")],
     scripts=['bin/csv2yamld', 'bin/yamld2csv', 'bin/yamld'],
     license='MIT',
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

