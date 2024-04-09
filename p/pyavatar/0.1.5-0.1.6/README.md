# Comparing `tmp/pyavatar-0.1.5.tar.gz` & `tmp/pyavatar-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyavatar-0.1.5.tar", last modified: Tue Oct 24 17:56:29 2023, max compression
+gzip compressed data, was "pyavatar-0.1.6.tar", last modified: Tue Apr  9 21:13:43 2024, max compression
```

## Comparing `pyavatar-0.1.5.tar` & `pyavatar-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2023-10-24 17:56:29.411204 pyavatar-0.1.5/
--rw-r--r--   0 smallwat3r   (501) staff       (20)     1074 2023-09-01 14:41:43.000000 pyavatar-0.1.5/LICENSE
--rw-r--r--   0 smallwat3r   (501) staff       (20)      114 2023-09-01 14:41:43.000000 pyavatar-0.1.5/MANIFEST.in
--rw-r--r--   0 smallwat3r   (501) staff       (20)     3424 2023-10-24 17:56:29.411069 pyavatar-0.1.5/PKG-INFO
--rw-r--r--   0 smallwat3r   (501) staff       (20)     2833 2023-09-07 21:36:03.000000 pyavatar-0.1.5/README.md
-drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2023-10-24 17:56:29.409266 pyavatar-0.1.5/pyavatar/
--rw-r--r--   0 smallwat3r   (501) staff       (20)     7947 2023-10-24 17:56:25.000000 pyavatar-0.1.5/pyavatar/__init__.py
--rw-r--r--   0 smallwat3r   (501) staff       (20)       22 2023-10-24 17:56:25.000000 pyavatar-0.1.5/pyavatar/_version.py
-drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2023-10-24 17:56:29.410005 pyavatar-0.1.5/pyavatar/font/
--rwxr-xr-x   0 smallwat3r   (501) staff       (20)   124204 2023-09-01 14:41:43.000000 pyavatar-0.1.5/pyavatar/font/Lora.ttf
-drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2023-10-24 17:56:29.409878 pyavatar-0.1.5/pyavatar.egg-info/
--rw-r--r--   0 smallwat3r   (501) staff       (20)     3424 2023-10-24 17:56:29.000000 pyavatar-0.1.5/pyavatar.egg-info/PKG-INFO
--rw-r--r--   0 smallwat3r   (501) staff       (20)      317 2023-10-24 17:56:29.000000 pyavatar-0.1.5/pyavatar.egg-info/SOURCES.txt
--rw-r--r--   0 smallwat3r   (501) staff       (20)        1 2023-10-24 17:56:29.000000 pyavatar-0.1.5/pyavatar.egg-info/dependency_links.txt
--rw-r--r--   0 smallwat3r   (501) staff       (20)       15 2023-10-24 17:56:29.000000 pyavatar-0.1.5/pyavatar.egg-info/requires.txt
--rw-r--r--   0 smallwat3r   (501) staff       (20)        9 2023-10-24 17:56:29.000000 pyavatar-0.1.5/pyavatar.egg-info/top_level.txt
--rw-r--r--   0 smallwat3r   (501) staff       (20)     1089 2023-10-23 19:46:56.000000 pyavatar-0.1.5/pyproject.toml
--rw-r--r--   0 smallwat3r   (501) staff       (20)       15 2023-10-24 17:56:25.000000 pyavatar-0.1.5/requirements.txt
--rw-r--r--   0 smallwat3r   (501) staff       (20)       38 2023-10-24 17:56:29.411251 pyavatar-0.1.5/setup.cfg
--rw-r--r--   0 smallwat3r   (501) staff       (20)     1144 2023-09-01 19:42:10.000000 pyavatar-0.1.5/setup.py
-drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2023-10-24 17:56:29.410757 pyavatar-0.1.5/tests/
--rw-r--r--   0 smallwat3r   (501) staff       (20)     4143 2023-09-07 21:34:59.000000 pyavatar-0.1.5/tests/test_pyavatar.py
+drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2024-04-09 21:13:43.987370 pyavatar-0.1.6/
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     1074 2023-09-01 14:41:43.000000 pyavatar-0.1.6/LICENSE
+-rw-r--r--   0 smallwat3r   (501) staff       (20)      114 2023-09-01 14:41:43.000000 pyavatar-0.1.6/MANIFEST.in
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     3454 2024-04-09 21:13:43.987171 pyavatar-0.1.6/PKG-INFO
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     2833 2023-09-07 21:36:03.000000 pyavatar-0.1.6/README.md
+drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2024-04-09 21:13:43.984326 pyavatar-0.1.6/pyavatar/
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     7953 2024-04-09 21:12:37.000000 pyavatar-0.1.6/pyavatar/__init__.py
+-rw-r--r--   0 smallwat3r   (501) staff       (20)       22 2024-04-09 21:12:43.000000 pyavatar-0.1.6/pyavatar/_version.py
+drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2024-04-09 21:13:43.985105 pyavatar-0.1.6/pyavatar/font/
+-rwxr-xr-x   0 smallwat3r   (501) staff       (20)   124204 2023-09-01 14:41:43.000000 pyavatar-0.1.6/pyavatar/font/Lora.ttf
+drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2024-04-09 21:13:43.984982 pyavatar-0.1.6/pyavatar.egg-info/
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     3454 2024-04-09 21:13:43.000000 pyavatar-0.1.6/pyavatar.egg-info/PKG-INFO
+-rw-r--r--   0 smallwat3r   (501) staff       (20)      317 2024-04-09 21:13:43.000000 pyavatar-0.1.6/pyavatar.egg-info/SOURCES.txt
+-rw-r--r--   0 smallwat3r   (501) staff       (20)        1 2024-04-09 21:13:43.000000 pyavatar-0.1.6/pyavatar.egg-info/dependency_links.txt
+-rw-r--r--   0 smallwat3r   (501) staff       (20)       15 2024-04-09 21:13:43.000000 pyavatar-0.1.6/pyavatar.egg-info/requires.txt
+-rw-r--r--   0 smallwat3r   (501) staff       (20)        9 2024-04-09 21:13:43.000000 pyavatar-0.1.6/pyavatar.egg-info/top_level.txt
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     1089 2023-10-23 19:46:56.000000 pyavatar-0.1.6/pyproject.toml
+-rw-r--r--   0 smallwat3r   (501) staff       (20)       15 2024-04-09 21:12:37.000000 pyavatar-0.1.6/requirements.txt
+-rw-r--r--   0 smallwat3r   (501) staff       (20)       38 2024-04-09 21:13:43.987413 pyavatar-0.1.6/setup.cfg
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     1144 2023-09-01 19:42:10.000000 pyavatar-0.1.6/setup.py
+drwxr-xr-x   0 smallwat3r   (501) staff       (20)        0 2024-04-09 21:13:43.986678 pyavatar-0.1.6/tests/
+-rw-r--r--   0 smallwat3r   (501) staff       (20)     4143 2023-09-07 21:34:59.000000 pyavatar-0.1.6/tests/test_pyavatar.py
```

### Comparing `pyavatar-0.1.5/LICENSE` & `pyavatar-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyavatar-0.1.5/PKG-INFO` & `pyavatar-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyavatar
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate simple user avatars from an input string.
 Home-page: https://github.com/smallwat3r/pyavatar
 Author: Matthieu Petiteau
 Author-email: mpetiteau.pro@gmail.com
 License: MIT
 Keywords: avatar
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow==10.3.0
 
 <h3 align="center">pyavatar</h3>
 <p align="center">Create default user avatars from a given string</p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/1.png" />
   <img src="https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/2.png" />
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: pyavatar Version: 0.1.5 Summary: Generate simple
+Metadata-Version: 2.1 Name: pyavatar Version: 0.1.6 Summary: Generate simple
 user avatars from an input string. Home-page: https://github.com/smallwat3r/
 pyavatar Author: Matthieu Petiteau Author-email: mpetiteau.pro@gmail.com
 License: MIT Keywords: avatar Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Pillow==10.3.0
                               ******** ppyyaavvaattaarr ********
                 Create default user avatars from a given string
 [https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/1.png][https:
   //raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/2.png][https://
         raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/3.png]
    _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_s_m_a_l_l_w_a_t_3_r_/_p_y_a_v_a_t_a_r_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_w_h_e_e_l_/_p_y_a_v_a_t_a_r_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
```

### Comparing `pyavatar-0.1.5/README.md` & `pyavatar-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyavatar-0.1.5/pyavatar/__init__.py` & `pyavatar-0.1.6/pyavatar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     @staticmethod
     def _random_color() -> _RGBColor:
         return (random.randint(0, 255),
                 random.randint(0, 255),
                 random.randint(0, 255))
 
-    def __generate_avatar(self) -> Image:
+    def __generate_avatar(self) -> Image.Image:
         image = Image.new(mode="RGB",
                           size=(self.size, self.size),
                           color=self.color)
         font = ImageFont.truetype(self.fontpath, size=int(0.6 * self.size))
         draw = ImageDraw.Draw(image)
         _, _, w_txt, h_txt = draw.textbbox((0, 0), self.text, font)
         off_x, off_y, _, _ = font.getbbox(self.text)
```

### Comparing `pyavatar-0.1.5/pyavatar/font/Lora.ttf` & `pyavatar-0.1.6/pyavatar/font/Lora.ttf`

 * *Files identical despite different names*

### Comparing `pyavatar-0.1.5/pyavatar.egg-info/PKG-INFO` & `pyavatar-0.1.6/pyavatar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyavatar
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate simple user avatars from an input string.
 Home-page: https://github.com/smallwat3r/pyavatar
 Author: Matthieu Petiteau
 Author-email: mpetiteau.pro@gmail.com
 License: MIT
 Keywords: avatar
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Pillow==10.3.0
 
 <h3 align="center">pyavatar</h3>
 <p align="center">Create default user avatars from a given string</p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/1.png" />
   <img src="https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/2.png" />
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: pyavatar Version: 0.1.5 Summary: Generate simple
+Metadata-Version: 2.1 Name: pyavatar Version: 0.1.6 Summary: Generate simple
 user avatars from an input string. Home-page: https://github.com/smallwat3r/
 pyavatar Author: Matthieu Petiteau Author-email: mpetiteau.pro@gmail.com
 License: MIT Keywords: avatar Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Pillow==10.3.0
                               ******** ppyyaavvaattaarr ********
                 Create default user avatars from a given string
 [https://raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/1.png][https:
   //raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/2.png][https://
         raw.githubusercontent.com/smallwat3r/pyavatar/master/ext/3.png]
    _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_s_m_a_l_l_w_a_t_3_r_/_p_y_a_v_a_t_a_r_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_w_h_e_e_l_/_p_y_a_v_a_t_a_r_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
```

### Comparing `pyavatar-0.1.5/pyproject.toml` & `pyavatar-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyavatar-0.1.5/setup.py` & `pyavatar-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyavatar-0.1.5/tests/test_pyavatar.py` & `pyavatar-0.1.6/tests/test_pyavatar.py`

 * *Files identical despite different names*

