# Comparing `tmp/gpti-1.4.tar.gz` & `tmp/gpti-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpti-1.4.tar", last modified: Sun Apr  7 00:19:54 2024, max compression
+gzip compressed data, was "gpti-1.5.tar", last modified: Tue Apr  9 19:54:13 2024, max compression
```

## Comparing `gpti-1.4.tar` & `gpti-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.488304 gpti-1.4/
--rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.4/LICENSE
--rw-rw-rw-   0        0        0    63532 2024-04-07 00:19:54.488304 gpti-1.4/PKG-INFO
--rw-rw-rw-   0        0        0    61477 2024-04-07 00:16:22.000000 gpti-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.462589 gpti-1.4/gpti/
--rw-rw-rw-   0        0        0   109640 2024-04-06 23:08:54.000000 gpti-1.4/gpti/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 00:19:54.478531 gpti-1.4/gpti.egg-info/
--rw-rw-rw-   0        0        0    63532 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-07 00:19:54.000000 gpti-1.4/gpti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 00:19:54.488304 gpti-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1180 2024-04-06 23:14:17.000000 gpti-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:54:13.819434 gpti-1.5/
+-rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.5/LICENSE
+-rw-rw-rw-   0        0        0    63532 2024-04-09 19:54:13.815993 gpti-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    61477 2024-04-09 19:49:42.000000 gpti-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 19:54:13.787743 gpti-1.5/gpti/
+-rw-rw-rw-   0        0        0   109640 2024-04-06 23:08:54.000000 gpti-1.5/gpti/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:54:13.808262 gpti-1.5/gpti.egg-info/
+-rw-rw-rw-   0        0        0    63532 2024-04-09 19:54:13.000000 gpti-1.5/gpti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-09 19:54:13.000000 gpti-1.5/gpti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:54:13.000000 gpti-1.5/gpti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 19:54:13.000000 gpti-1.5/gpti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-09 19:54:13.000000 gpti-1.5/gpti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:54:13.819434 gpti-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2024-04-09 19:51:45.000000 gpti-1.5/setup.py
```

### Comparing `gpti-1.4/LICENSE` & `gpti-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpti-1.4/PKG-INFO` & `gpti-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.4
+Version: 1.5
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -624,15 +624,15 @@
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
 | Parameter       | Default                          | Description                           |
 |-----------------|----------------------------------|---------------------------------------|
-| prompt_negative |                                  | Indicates what the AI should not do   |
+| negative_prompt |                                  | Indicates what the AI should not do   |
 | model           | absolutereality_V16.safetensors [37db0fc3] | Select from the list of models |
 | cfg_scale       | 7                                | Min: 0, Max: 20                       |
 | steps           | 25                               | Min: 1, Max: 30                       |
 | sampler         | DPM++ 2M Karras                  | Select from these: "Euler","Euler a","Heun","DPM++ 2M Karras","DPM++ SDE Karras","DDIM" |
 
 <a id="prodia-stablediffusion"></a>
 ## Usage Prodia Stable-Diffusion
```

### Comparing `gpti-1.4/README.md` & `gpti-1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,15 @@
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
 | Parameter       | Default                          | Description                           |
 |-----------------|----------------------------------|---------------------------------------|
-| prompt_negative |                                  | Indicates what the AI should not do   |
+| negative_prompt |                                  | Indicates what the AI should not do   |
 | model           | absolutereality_V16.safetensors [37db0fc3] | Select from the list of models |
 | cfg_scale       | 7                                | Min: 0, Max: 20                       |
 | steps           | 25                               | Min: 1, Max: 30                       |
 | sampler         | DPM++ 2M Karras                  | Select from these: "Euler","Euler a","Heun","DPM++ 2M Karras","DPM++ SDE Karras","DDIM" |
 
 <a id="prodia-stablediffusion"></a>
 ## Usage Prodia Stable-Diffusion
```

### Comparing `gpti-1.4/gpti/__init__.py` & `gpti-1.5/gpti/__init__.py`

 * *Files identical despite different names*

### Comparing `gpti-1.4/gpti.egg-info/PKG-INFO` & `gpti-1.5/gpti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.4
+Version: 1.5
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -624,15 +624,15 @@
 - timeless-1.0.ckpt [7c4971d4]
 - toonyou_beta6.safetensors [980f6b15]
 
 #### Parameters
 
 | Parameter       | Default                          | Description                           |
 |-----------------|----------------------------------|---------------------------------------|
-| prompt_negative |                                  | Indicates what the AI should not do   |
+| negative_prompt |                                  | Indicates what the AI should not do   |
 | model           | absolutereality_V16.safetensors [37db0fc3] | Select from the list of models |
 | cfg_scale       | 7                                | Min: 0, Max: 20                       |
 | steps           | 25                               | Min: 1, Max: 30                       |
 | sampler         | DPM++ 2M Karras                  | Select from these: "Euler","Euler a","Heun","DPM++ 2M Karras","DPM++ SDE Karras","DDIM" |
 
 <a id="prodia-stablediffusion"></a>
 ## Usage Prodia Stable-Diffusion
```

### Comparing `gpti-1.4/setup.py` & `gpti-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as f:
         _long_description = f.read()
 except Exception as e:
     _long_description = ''
 
 setup(
     name='gpti',
-    version='1.4',
+    version='1.5',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='yandricr',
     author_email='yandribret@gmail.com',
     description='This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT',
```

