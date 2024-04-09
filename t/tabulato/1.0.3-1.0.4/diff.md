# Comparing `tmp/tabulato-1.0.3.tar.gz` & `tmp/tabulato-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulato-1.0.3.tar", last modified: Thu Mar  7 12:47:58 2024, max compression
+gzip compressed data, was "tabulato-1.0.4.tar", last modified: Tue Apr  9 15:04:52 2024, max compression
```

## Comparing `tabulato-1.0.3.tar` & `tabulato-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.334721 tabulato-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.330721 tabulato-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:47.000000 tabulato-1.0.3/.github/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.330721 tabulato-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-07 12:47:47.000000 tabulato-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-07 12:47:47.000000 tabulato-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-07 12:47:47.000000 tabulato-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-07 12:47:47.000000 tabulato-1.0.3/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 12:47:47.000000 tabulato-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-03-07 12:47:58.334721 tabulato-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-03-07 12:47:47.000000 tabulato-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-07 12:47:47.000000 tabulato-1.0.3/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.330721 tabulato-1.0.3/images/
--rw-r--r--   0 runner    (1001) docker     (127)   144746 2024-03-07 12:47:47.000000 tabulato-1.0.3/images/0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   175038 2024-03-07 12:47:47.000000 tabulato-1.0.3/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-07 12:47:47.000000 tabulato-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-07 12:47:47.000000 tabulato-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:47:58.334721 tabulato-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.330721 tabulato-1.0.3/tabulato/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-07 12:47:47.000000 tabulato-1.0.3/tabulato/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-03-07 12:47:47.000000 tabulato-1.0.3/tabulato/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.334721 tabulato-1.0.3/tabulato/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-07 12:47:47.000000 tabulato-1.0.3/tabulato/tests/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-07 12:47:47.000000 tabulato-1.0.3/tabulato/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:47:58.334721 tabulato-1.0.3/tabulato.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-03-07 12:47:58.000000 tabulato-1.0.3/tabulato.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-07 12:47:58.000000 tabulato-1.0.3/tabulato.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:47:58.000000 tabulato-1.0.3/tabulato.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-07 12:47:58.000000 tabulato-1.0.3/tabulato.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.839227 tabulato-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:46.000000 tabulato-1.0.4/.github/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.839227 tabulato-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-09 15:04:46.000000 tabulato-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 15:04:46.000000 tabulato-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 15:04:46.000000 tabulato-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 15:04:46.000000 tabulato-1.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 15:04:46.000000 tabulato-1.0.4/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:04:46.000000 tabulato-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-09 15:04:52.843227 tabulato-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-09 15:04:46.000000 tabulato-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.839227 tabulato-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.839227 tabulato-1.0.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.839227 tabulato-1.0.4/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/_static/css/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/docs/source/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/github/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/github/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-09 15:04:46.000000 tabulato-1.0.4/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-09 15:04:46.000000 tabulato-1.0.4/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   144746 2024-04-09 15:04:46.000000 tabulato-1.0.4/images/0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   175038 2024-04-09 15:04:46.000000 tabulato-1.0.4/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 15:04:46.000000 tabulato-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 15:04:46.000000 tabulato-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:04:52.843227 tabulato-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/tabulato/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 15:04:46.000000 tabulato-1.0.4/tabulato/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-09 15:04:46.000000 tabulato-1.0.4/tabulato/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/tabulato/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-09 15:04:46.000000 tabulato-1.0.4/tabulato/tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-09 15:04:46.000000 tabulato-1.0.4/tabulato/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:52.843227 tabulato-1.0.4/tabulato.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-09 15:04:52.000000 tabulato-1.0.4/tabulato.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 15:04:52.000000 tabulato-1.0.4/tabulato.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:04:52.000000 tabulato-1.0.4/tabulato.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 15:04:52.000000 tabulato-1.0.4/tabulato.egg-info/top_level.txt
```

### Comparing `tabulato-1.0.3/.github/workflows/ci.yml` & `tabulato-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/.gitignore` & `tabulato-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/LICENSE` & `tabulato-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/PKG-INFO` & `tabulato-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabulato
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a Python package that provides functionality for generating tabulated representations of data with customizable colors and formatting options. It offers a user-friendly interface for creating visually appealing tables in terminal output.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -68,24 +68,25 @@
 - [tabulato](#tabulato)
 - [Table of Contents](#table-of-contents)
 - [Key features of tabulato include:](#key-features-of-tabulato-include)
 - [Installation](#installation)
 - [Python Version](#python-version)
 - [Example](#example)
 - [What's missing on this package?](#whats-missing-on-this-package)
+- [Docs](#docs)
 - [License](#license)
 
 ### Key features of tabulato include:
 
 - Generating tables with customizable colors for headers, even rows, and odd rows.
 - Specifying required columns to ensure important data is always displayed.
 - Option to make headers bold for emphasis.
 - User-friendly API for straightforward integration into your Python projects.
 
-> tabulato simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
+> `tabulato` simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
 
 ### Installation
 
 To install tabulato, you can use pip:
 
 ```bash
 pip install tabulato
@@ -269,10 +270,14 @@
 | `"BG_WHITE"`  | White background  |
 | `"BG_YELLOW"` | Yellow background |
 
 ### What's missing on this package?
 
 This package lacks `wrapping` of text for long lines. This `version` only support small tables. Long column data might not end up displayed well, however with small column data like this package is the best.
 
+### Docs
+
+You can read the full documentation [here](https://tabulato.readthedocs.io/en/latest/).
+
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tabulato Version: 1.0.3 Summary: This is a Python
+Metadata-Version: 2.1 Name: tabulato Version: 1.0.4 Summary: This is a Python
 package that provides functionality for generating tabulated representations of
 data with customizable colors and formatting options. It offers a user-friendly
 interface for creating visually appealing tables in terminal output. Author-
 email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
@@ -47,19 +47,19 @@
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_t_a_b_u_l_a_t_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_r_i_s_p_e_n_g_a_r_i_/
   _t_a_b_u_l_a_t_o_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_a_b_u_l_a_t_o_._s_v_g_]
 ### Table of Contents - [tabulato](#tabulato) - [Table of Contents](#table-of-
 contents) - [Key features of tabulato include:](#key-features-of-tabulato-
 include) - [Installation](#installation) - [Python Version](#python-version) -
 [Example](#example) - [What's missing on this package?](#whats-missing-on-this-
-package) - [License](#license) ### Key features of tabulato include: -
-Generating tables with customizable colors for headers, even rows, and odd
-rows. - Specifying required columns to ensure important data is always
+package) - [Docs](#docs) - [License](#license) ### Key features of tabulato
+include: - Generating tables with customizable colors for headers, even rows,
+and odd rows. - Specifying required columns to ensure important data is always
 displayed. - Option to make headers bold for emphasis. - User-friendly API for
-straightforward integration into your Python projects. > tabulato simplifies
+straightforward integration into your Python projects. > `tabulato` simplifies
 the task of formatting and presenting tabular data in terminal environments,
 making it an essential tool for developers and data scientists working with
 command-line interfaces. ### Installation To install tabulato, you can use pip:
 ```bash pip install tabulato ``` ### Python Version This package support python
 version `>=3.10` ### Example In the following examples shows you how you can
 use ```py from tabulato import colorful_tabulate, TableRowStyle headers =
 ["Name", "Student Number", "DOB", "Email Address"] data = [ ["John Doe",
@@ -130,9 +130,10 @@
 ----- | | `"BG_BLACK"` | Black background | | `"BG_RED"` | Red background | |
 `"BG_GREEN"` | Green background | | `"BG_BLUE"` | Blue background | |
 `"BG_PURPLE"` | Purple background | | `"BG_CYAN"` | Cyan background | |
 `"BG_WHITE"` | White background | | `"BG_YELLOW"` | Yellow background | ###
 What's missing on this package? This package lacks `wrapping` of text for long
 lines. This `version` only support small tables. Long column data might not end
 up displayed well, however with small column data like this package is the
-best. ### License This project is licensed under the MIT License - see the
-[LICENSE](/LISENSE) file for details.
+best. ### Docs You can read the full documentation [here](https://
+tabulato.readthedocs.io/en/latest/). ### License This project is licensed under
+the MIT License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `tabulato-1.0.3/README.md` & `tabulato-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 - [tabulato](#tabulato)
 - [Table of Contents](#table-of-contents)
 - [Key features of tabulato include:](#key-features-of-tabulato-include)
 - [Installation](#installation)
 - [Python Version](#python-version)
 - [Example](#example)
 - [What's missing on this package?](#whats-missing-on-this-package)
+- [Docs](#docs)
 - [License](#license)
 
 ### Key features of tabulato include:
 
 - Generating tables with customizable colors for headers, even rows, and odd rows.
 - Specifying required columns to ensure important data is always displayed.
 - Option to make headers bold for emphasis.
 - User-friendly API for straightforward integration into your Python projects.
 
-> tabulato simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
+> `tabulato` simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
 
 ### Installation
 
 To install tabulato, you can use pip:
 
 ```bash
 pip install tabulato
@@ -217,10 +218,14 @@
 | `"BG_WHITE"`  | White background  |
 | `"BG_YELLOW"` | Yellow background |
 
 ### What's missing on this package?
 
 This package lacks `wrapping` of text for long lines. This `version` only support small tables. Long column data might not end up displayed well, however with small column data like this package is the best.
 
+### Docs
+
+You can read the full documentation [here](https://tabulato.readthedocs.io/en/latest/).
+
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -10,19 +10,19 @@
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_t_a_b_u_l_a_t_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_r_i_s_p_e_n_g_a_r_i_/
   _t_a_b_u_l_a_t_o_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_a_b_u_l_a_t_o_._s_v_g_]
 ### Table of Contents - [tabulato](#tabulato) - [Table of Contents](#table-of-
 contents) - [Key features of tabulato include:](#key-features-of-tabulato-
 include) - [Installation](#installation) - [Python Version](#python-version) -
 [Example](#example) - [What's missing on this package?](#whats-missing-on-this-
-package) - [License](#license) ### Key features of tabulato include: -
-Generating tables with customizable colors for headers, even rows, and odd
-rows. - Specifying required columns to ensure important data is always
+package) - [Docs](#docs) - [License](#license) ### Key features of tabulato
+include: - Generating tables with customizable colors for headers, even rows,
+and odd rows. - Specifying required columns to ensure important data is always
 displayed. - Option to make headers bold for emphasis. - User-friendly API for
-straightforward integration into your Python projects. > tabulato simplifies
+straightforward integration into your Python projects. > `tabulato` simplifies
 the task of formatting and presenting tabular data in terminal environments,
 making it an essential tool for developers and data scientists working with
 command-line interfaces. ### Installation To install tabulato, you can use pip:
 ```bash pip install tabulato ``` ### Python Version This package support python
 version `>=3.10` ### Example In the following examples shows you how you can
 use ```py from tabulato import colorful_tabulate, TableRowStyle headers =
 ["Name", "Student Number", "DOB", "Email Address"] data = [ ["John Doe",
@@ -93,9 +93,10 @@
 ----- | | `"BG_BLACK"` | Black background | | `"BG_RED"` | Red background | |
 `"BG_GREEN"` | Green background | | `"BG_BLUE"` | Blue background | |
 `"BG_PURPLE"` | Purple background | | `"BG_CYAN"` | Cyan background | |
 `"BG_WHITE"` | White background | | `"BG_YELLOW"` | Yellow background | ###
 What's missing on this package? This package lacks `wrapping` of text for long
 lines. This `version` only support small tables. Long column data might not end
 up displayed well, however with small column data like this package is the
-best. ### License This project is licensed under the MIT License - see the
-[LICENSE](/LISENSE) file for details.
+best. ### Docs You can read the full documentation [here](https://
+tabulato.readthedocs.io/en/latest/). ### License This project is licensed under
+the MIT License - see the [LICENSE](/LISENSE) file for details.
```

### Comparing `tabulato-1.0.3/example.py` & `tabulato-1.0.4/example.py`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/images/0.jpg` & `tabulato-1.0.4/images/0.jpg`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/images/1.jpg` & `tabulato-1.0.4/images/1.jpg`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/pyproject.toml` & `tabulato-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tabulato"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Crispen Gari", email = "crispengari@gmail.com"},
 ]
 description = "This is a Python package that provides functionality for generating tabulated representations of data with customizable colors and formatting options. It offers a user-friendly interface for creating visually appealing tables in terminal output."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `tabulato-1.0.3/tabulato/table.py` & `tabulato-1.0.4/tabulato/table.py`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/tabulato/tests/test_tables.py` & `tabulato-1.0.4/tabulato/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/tabulato/utils.py` & `tabulato-1.0.4/tabulato/utils.py`

 * *Files identical despite different names*

### Comparing `tabulato-1.0.3/tabulato.egg-info/PKG-INFO` & `tabulato-1.0.4/tabulato.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabulato
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is a Python package that provides functionality for generating tabulated representations of data with customizable colors and formatting options. It offers a user-friendly interface for creating visually appealing tables in terminal output.
 Author-email: Crispen Gari <crispengari@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 crispengari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -68,24 +68,25 @@
 - [tabulato](#tabulato)
 - [Table of Contents](#table-of-contents)
 - [Key features of tabulato include:](#key-features-of-tabulato-include)
 - [Installation](#installation)
 - [Python Version](#python-version)
 - [Example](#example)
 - [What's missing on this package?](#whats-missing-on-this-package)
+- [Docs](#docs)
 - [License](#license)
 
 ### Key features of tabulato include:
 
 - Generating tables with customizable colors for headers, even rows, and odd rows.
 - Specifying required columns to ensure important data is always displayed.
 - Option to make headers bold for emphasis.
 - User-friendly API for straightforward integration into your Python projects.
 
-> tabulato simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
+> `tabulato` simplifies the task of formatting and presenting tabular data in terminal environments, making it an essential tool for developers and data scientists working with command-line interfaces.
 
 ### Installation
 
 To install tabulato, you can use pip:
 
 ```bash
 pip install tabulato
@@ -269,10 +270,14 @@
 | `"BG_WHITE"`  | White background  |
 | `"BG_YELLOW"` | Yellow background |
 
 ### What's missing on this package?
 
 This package lacks `wrapping` of text for long lines. This `version` only support small tables. Long column data might not end up displayed well, however with small column data like this package is the best.
 
+### Docs
+
+You can read the full documentation [here](https://tabulato.readthedocs.io/en/latest/).
+
 ### License
 
 This project is licensed under the MIT License - see the [LICENSE](/LISENSE) file for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tabulato Version: 1.0.3 Summary: This is a Python
+Metadata-Version: 2.1 Name: tabulato Version: 1.0.4 Summary: This is a Python
 package that provides functionality for generating tabulated representations of
 data with customizable colors and formatting options. It offers a user-friendly
 interface for creating visually appealing tables in terminal output. Author-
 email: Crispen Gari
 gmail.com> License: MIT License Copyright (c) 2024 crispengari Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
@@ -47,19 +47,19 @@
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_t_a_b_u_l_a_t_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_r_i_s_p_e_n_g_a_r_i_/
   _t_a_b_u_l_a_t_o_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_a_b_u_l_a_t_o_._s_v_g_]
 ### Table of Contents - [tabulato](#tabulato) - [Table of Contents](#table-of-
 contents) - [Key features of tabulato include:](#key-features-of-tabulato-
 include) - [Installation](#installation) - [Python Version](#python-version) -
 [Example](#example) - [What's missing on this package?](#whats-missing-on-this-
-package) - [License](#license) ### Key features of tabulato include: -
-Generating tables with customizable colors for headers, even rows, and odd
-rows. - Specifying required columns to ensure important data is always
+package) - [Docs](#docs) - [License](#license) ### Key features of tabulato
+include: - Generating tables with customizable colors for headers, even rows,
+and odd rows. - Specifying required columns to ensure important data is always
 displayed. - Option to make headers bold for emphasis. - User-friendly API for
-straightforward integration into your Python projects. > tabulato simplifies
+straightforward integration into your Python projects. > `tabulato` simplifies
 the task of formatting and presenting tabular data in terminal environments,
 making it an essential tool for developers and data scientists working with
 command-line interfaces. ### Installation To install tabulato, you can use pip:
 ```bash pip install tabulato ``` ### Python Version This package support python
 version `>=3.10` ### Example In the following examples shows you how you can
 use ```py from tabulato import colorful_tabulate, TableRowStyle headers =
 ["Name", "Student Number", "DOB", "Email Address"] data = [ ["John Doe",
@@ -130,9 +130,10 @@
 ----- | | `"BG_BLACK"` | Black background | | `"BG_RED"` | Red background | |
 `"BG_GREEN"` | Green background | | `"BG_BLUE"` | Blue background | |
 `"BG_PURPLE"` | Purple background | | `"BG_CYAN"` | Cyan background | |
 `"BG_WHITE"` | White background | | `"BG_YELLOW"` | Yellow background | ###
 What's missing on this package? This package lacks `wrapping` of text for long
 lines. This `version` only support small tables. Long column data might not end
 up displayed well, however with small column data like this package is the
-best. ### License This project is licensed under the MIT License - see the
-[LICENSE](/LISENSE) file for details.
+best. ### Docs You can read the full documentation [here](https://
+tabulato.readthedocs.io/en/latest/). ### License This project is licensed under
+the MIT License - see the [LICENSE](/LISENSE) file for details.
```

