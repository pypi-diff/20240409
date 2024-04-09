# Comparing `tmp/seesus-1.2.0.tar.gz` & `tmp/seesus-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mengcai/Documents/Dissertation/classifier/seesus/dist/.tmp-1pgvbkmx/seesus-1.2.0.tar", last modified: Wed Nov  8 12:43:30 2023, max compression
+gzip compressed data, was "/Users/mengcai/Documents/Dissertation/classifier/seesus/dist/.tmp-p9uwexgm/seesus-1.2.1.tar", last modified: Tue Apr  9 20:42:49 2024, max compression
```

## Comparing `seesus-1.2.0.tar` & `seesus-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.227461 seesus-1.2.0/
--rw-r--r--   0 mengcai    (501) staff       (20)     1799 2023-09-21 16:19:24.000000 seesus-1.2.0/.gitignore
--rw-r--r--   0 mengcai    (501) staff       (20)    35149 2023-04-05 18:30:04.000000 seesus-1.2.0/LICENSE
--rw-r--r--   0 mengcai    (501) staff       (20)     2515 2023-11-08 12:43:30.227132 seesus-1.2.0/PKG-INFO
--rw-r--r--   0 mengcai    (501) staff       (20)     1810 2023-11-06 15:06:26.000000 seesus-1.2.0/README.md
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.217533 seesus-1.2.0/docs/
--rw-r--r--   0 mengcai    (501) staff       (20)   166686 2023-09-22 13:16:00.000000 seesus-1.2.0/docs/logo.jpg
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.222033 seesus-1.2.0/docs/seesus/
--rw-r--r--   0 mengcai    (501) staff       (20)    51867 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/SDG_desc.html
--rw-r--r--   0 mengcai    (501) staff       (20)   435653 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/SDG_keys.html
--rw-r--r--   0 mengcai    (501) staff       (20)     8862 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/index.html
--rw-r--r--   0 mengcai    (501) staff       (20)    20085 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/see_keys.html
--rw-r--r--   0 mengcai    (501) staff       (20)    33664 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/seesus.html
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.222484 seesus-1.2.0/docs/seesus/tests/
--rw-r--r--   0 mengcai    (501) staff       (20)     6503 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/tests/index.html
--rw-r--r--   0 mengcai    (501) staff       (20)    13216 2023-09-22 13:53:04.000000 seesus-1.2.0/docs/seesus/tests/test_seesus.html
--rw-r--r--   0 mengcai    (501) staff       (20)    16121 2023-11-07 14:34:41.000000 seesus-1.2.0/example.ipynb
--rw-r--r--   0 mengcai    (501) staff       (20)      916 2023-11-08 12:42:23.000000 seesus-1.2.0/pyproject.toml
--rw-r--r--   0 mengcai    (501) staff       (20)       38 2023-11-08 12:43:30.227513 seesus-1.2.0/setup.cfg
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.215937 seesus-1.2.0/src/
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.225268 seesus-1.2.0/src/seesus/
--rw-r--r--   0 mengcai    (501) staff       (20)    42007 2023-09-22 10:33:09.000000 seesus-1.2.0/src/seesus/SDG_desc.py
--rw-r--r--   0 mengcai    (501) staff       (20)   402478 2023-09-22 10:32:57.000000 seesus-1.2.0/src/seesus/SDG_keys.py
--rw-r--r--   0 mengcai    (501) staff       (20)      319 2023-09-22 10:33:30.000000 seesus-1.2.0/src/seesus/__init__.py
--rw-r--r--   0 mengcai    (501) staff       (20)     7744 2023-09-22 10:32:45.000000 seesus-1.2.0/src/seesus/see_keys.py
--rw-r--r--   0 mengcai    (501) staff       (20)     8223 2023-11-06 16:25:55.000000 seesus-1.2.0/src/seesus/seesus.py
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.226165 seesus-1.2.0/src/seesus.egg-info/
--rw-r--r--   0 mengcai    (501) staff       (20)     2515 2023-11-08 12:43:30.000000 seesus-1.2.0/src/seesus.egg-info/PKG-INFO
--rw-r--r--   0 mengcai    (501) staff       (20)      581 2023-11-08 12:43:30.000000 seesus-1.2.0/src/seesus.egg-info/SOURCES.txt
--rw-r--r--   0 mengcai    (501) staff       (20)        1 2023-11-08 12:43:30.000000 seesus-1.2.0/src/seesus.egg-info/dependency_links.txt
--rw-r--r--   0 mengcai    (501) staff       (20)       34 2023-11-08 12:43:30.000000 seesus-1.2.0/src/seesus.egg-info/requires.txt
--rw-r--r--   0 mengcai    (501) staff       (20)        7 2023-11-08 12:43:30.000000 seesus-1.2.0/src/seesus.egg-info/top_level.txt
-drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2023-11-08 12:43:30.226435 seesus-1.2.0/tests/
--rw-r--r--   0 mengcai    (501) staff       (20)        0 2023-09-21 16:25:18.000000 seesus-1.2.0/tests/__init__.py
--rw-r--r--   0 mengcai    (501) staff       (20)     1541 2023-09-22 10:33:58.000000 seesus-1.2.0/tests/test_seesus.py
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.526090 seesus-1.2.1/
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.514869 seesus-1.2.1/.github/
+-rw-r--r--   0 mengcai    (501) staff       (20)        7 2023-04-05 09:40:14.000000 seesus-1.2.1/.github/.gitignore
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.515242 seesus-1.2.1/.github/workflows/
+-rw-r--r--   0 mengcai    (501) staff       (20)      911 2024-01-03 10:28:00.000000 seesus-1.2.1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 mengcai    (501) staff       (20)     1799 2023-09-21 16:19:24.000000 seesus-1.2.1/.gitignore
+-rw-r--r--   0 mengcai    (501) staff       (20)     1704 2024-04-09 19:04:27.000000 seesus-1.2.1/CITATION.cff
+-rw-r--r--   0 mengcai    (501) staff       (20)    35149 2023-04-05 18:30:04.000000 seesus-1.2.1/LICENSE
+-rw-r--r--   0 mengcai    (501) staff       (20)     6479 2024-04-09 20:42:49.525748 seesus-1.2.1/PKG-INFO
+-rw-r--r--   0 mengcai    (501) staff       (20)     5774 2024-04-09 19:44:15.000000 seesus-1.2.1/README.md
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.515617 seesus-1.2.1/docs/
+-rw-r--r--   0 mengcai    (501) staff       (20)   166686 2023-09-22 13:16:00.000000 seesus-1.2.1/docs/logo.jpg
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.517935 seesus-1.2.1/docs/seesus/
+-rw-r--r--   0 mengcai    (501) staff       (20)    51867 2024-04-09 20:33:42.000000 seesus-1.2.1/docs/seesus/SDG_desc.html
+-rw-r--r--   0 mengcai    (501) staff       (20)   435653 2024-04-09 20:33:42.000000 seesus-1.2.1/docs/seesus/SDG_keys.html
+-rw-r--r--   0 mengcai    (501) staff       (20)     8604 2024-04-09 20:36:23.000000 seesus-1.2.1/docs/seesus/index.html
+-rw-r--r--   0 mengcai    (501) staff       (20)    20085 2024-04-09 20:33:42.000000 seesus-1.2.1/docs/seesus/see_keys.html
+-rw-r--r--   0 mengcai    (501) staff       (20)    34502 2024-04-09 20:33:42.000000 seesus-1.2.1/docs/seesus/seesus.html
+-rw-r--r--   0 mengcai    (501) staff       (20)    29117 2024-02-22 11:44:14.000000 seesus-1.2.1/example.ipynb
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.520067 seesus-1.2.1/paper/
+-rw-r--r--   0 mengcai    (501) staff       (20)    56425 2023-11-08 14:02:44.000000 seesus-1.2.1/paper/LOGO_ERC-FLAG_FP.png
+-rw-r--r--   0 mengcai    (501) staff       (20)    13612 2024-02-21 21:05:25.000000 seesus-1.2.1/paper/paper.bib
+-rw-r--r--   0 mengcai    (501) staff       (20)     8553 2024-03-27 10:33:12.000000 seesus-1.2.1/paper/paper.md
+-rw-r--r--   0 mengcai    (501) staff       (20)   270392 2024-04-09 19:16:37.000000 seesus-1.2.1/paper/paper.pdf
+-rw-r--r--   0 mengcai    (501) staff       (20)      916 2024-04-09 20:14:24.000000 seesus-1.2.1/pyproject.toml
+-rw-r--r--   0 mengcai    (501) staff       (20)       38 2024-04-09 20:42:49.526141 seesus-1.2.1/setup.cfg
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.512471 seesus-1.2.1/src/
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.523488 seesus-1.2.1/src/seesus/
+-rw-r--r--   0 mengcai    (501) staff       (20)    42007 2023-09-22 10:33:09.000000 seesus-1.2.1/src/seesus/SDG_desc.py
+-rw-r--r--   0 mengcai    (501) staff       (20)   402478 2023-09-22 10:32:57.000000 seesus-1.2.1/src/seesus/SDG_keys.py
+-rw-r--r--   0 mengcai    (501) staff       (20)      213 2024-04-09 20:33:25.000000 seesus-1.2.1/src/seesus/__init__.py
+-rw-r--r--   0 mengcai    (501) staff       (20)     7744 2023-09-22 10:32:45.000000 seesus-1.2.1/src/seesus/see_keys.py
+-rw-r--r--   0 mengcai    (501) staff       (20)     8223 2023-11-06 16:25:55.000000 seesus-1.2.1/src/seesus/seesus.py
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.525038 seesus-1.2.1/src/seesus.egg-info/
+-rw-r--r--   0 mengcai    (501) staff       (20)     6479 2024-04-09 20:42:49.000000 seesus-1.2.1/src/seesus.egg-info/PKG-INFO
+-rw-r--r--   0 mengcai    (501) staff       (20)      655 2024-04-09 20:42:49.000000 seesus-1.2.1/src/seesus.egg-info/SOURCES.txt
+-rw-r--r--   0 mengcai    (501) staff       (20)        1 2024-04-09 20:42:49.000000 seesus-1.2.1/src/seesus.egg-info/dependency_links.txt
+-rw-r--r--   0 mengcai    (501) staff       (20)       34 2024-04-09 20:42:49.000000 seesus-1.2.1/src/seesus.egg-info/requires.txt
+-rw-r--r--   0 mengcai    (501) staff       (20)        7 2024-04-09 20:42:49.000000 seesus-1.2.1/src/seesus.egg-info/top_level.txt
+drwxr-xr-x   0 mengcai    (501) staff       (20)        0 2024-04-09 20:42:49.524689 seesus-1.2.1/tests/
+-rw-r--r--   0 mengcai    (501) staff       (20)        0 2023-09-21 16:25:18.000000 seesus-1.2.1/tests/__init__.py
+-rw-r--r--   0 mengcai    (501) staff       (20)     1774 2024-02-21 14:13:53.000000 seesus-1.2.1/tests/test_seesus.py
```

### Comparing `seesus-1.2.0/.gitignore` & `seesus-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/LICENSE` & `seesus-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/docs/logo.jpg` & `seesus-1.2.1/docs/logo.jpg`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/docs/seesus/SDG_desc.html` & `seesus-1.2.1/docs/seesus/SDG_desc.html`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/docs/seesus/SDG_keys.html` & `seesus-1.2.1/docs/seesus/SDG_keys.html`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/docs/seesus/index.html` & `seesus-1.2.1/docs/seesus/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 <article id="content">
 <header>
 <h1 class="title">Package <code>seesus</code></h1>
 </header>
 <section id="section-intro">
 <h2 id="seesus">Seesus</h2>
 <p>A Python tool for checking whether a textual expression aligns with sustainability as defined by the United Nations Sustainable Development Goals.</p>
-<p><strong>version</strong> = "1.0.0"
-<strong>title</strong> = "seesus"
+<p><strong>title</strong> = "seesus"
 <strong>url</strong> = "https://github.com/caimeng2/seesus"
-<strong>license</strong> = "LGPL-3.0"</p>
+<strong>license</strong> = "GPL-3.0"</p>
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">&#34;&#34;&#34;
 seesus
 ------
@@ -64,18 +63,14 @@
 <div class="desc"><p>Classification of SDG targets into social, environmental, and economic sustainability.</p></div>
 </dd>
 <dt><code class="name"><a title="seesus.seesus" href="seesus.html">seesus.seesus</a></code></dt>
 <dd>
 <div class="desc"><p>Identify 17 Sustainable Development Goals (SDGs) and their 169 targets in text,
 and classify into social, environmental, and economic sustainability.</p></div>
 </dd>
-<dt><code class="name"><a title="seesus.tests" href="tests/index.html">seesus.tests</a></code></dt>
-<dd>
-<div class="desc"></div>
-</dd>
 </dl>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
@@ -91,18 +86,17 @@
 <ul id="index">
 <li><h3><a href="#header-submodules">Sub-modules</a></h3>
 <ul>
 <li><code><a title="seesus.SDG_desc" href="SDG_desc.html">seesus.SDG_desc</a></code></li>
 <li><code><a title="seesus.SDG_keys" href="SDG_keys.html">seesus.SDG_keys</a></code></li>
 <li><code><a title="seesus.see_keys" href="see_keys.html">seesus.see_keys</a></code></li>
 <li><code><a title="seesus.seesus" href="seesus.html">seesus.seesus</a></code></li>
-<li><code><a title="seesus.tests" href="tests/index.html">seesus.tests</a></code></li>
 </ul>
 </li>
 </ul>
 </nav>
 </main>
 <footer id="footer">
 <p>Generated by <a href="https://pdoc3.github.io/pdoc"><cite>pdoc</cite> 0.9.2</a>.</p>
 </footer>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 ************ PPaacckkaaggee sseeeessuuss ************
 ********** SSeeeessuuss **********
 A Python tool for checking whether a textual expression aligns with
 sustainability as defined by the United Nations Sustainable Development Goals.
-vveerrssiioonn = "1.0.0" ttiittllee = "seesus" uurrll = "https://github.com/caimeng2/seesus"
-lliicceennssee = "LGPL-3.0"
+ttiittllee = "seesus" uurrll = "https://github.com/caimeng2/seesus" lliicceennssee = "GPL-3.0"
 Expand source code
 """
 seesus
 ------
 A Python tool for checking whether a textual expression aligns with
 sustainability as defined by the United Nations Sustainable Development Goals.
 
@@ -29,17 +28,15 @@
   _s_e_e_s_u_s_._s_e_e___k_e_y_s
       Classification of SDG targets into social, environmental, and economic
       sustainability.
   _s_e_e_s_u_s_._s_e_e_s_u_s
       Identify 17 Sustainable Development Goals (SDGs) and their 169 targets in
       text, and classify into social, environmental, and economic
       sustainability.
-  _s_e_e_s_u_s_._t_e_s_t_s
 ************ IInnddeexx ************
     * _s_e_e_s_u_s
     * ******** _SS_uu_bb_--_mm_oo_dd_uu_ll_ee_ss ********
           o _s_e_e_s_u_s_._S_D_G___d_e_s_c
           o _s_e_e_s_u_s_._S_D_G___k_e_y_s
           o _s_e_e_s_u_s_._s_e_e___k_e_y_s
           o _s_e_e_s_u_s_._s_e_e_s_u_s
-          o _s_e_e_s_u_s_._t_e_s_t_s
 Generated by_p_d_o_c_0_._9_._2.
```

### Comparing `seesus-1.2.0/docs/seesus/see_keys.html` & `seesus-1.2.1/docs/seesus/see_keys.html`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/docs/seesus/seesus.html` & `seesus-1.2.1/docs/seesus/seesus.html`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 import regex as re
 
 from seesus.SDG_keys import SDG_keys
 from seesus.see_keys import see_keys
 from seesus.SDG_desc import goal_desc, tar_desc
 
+
 def id_sus(text):
     &#34;&#34;&#34;
     Identify the UN Sustainable Development Goals (SDGs) and their associated targets in text.
 
     Parameters
     ----------
     text: str
@@ -62,15 +63,15 @@
         Match types, either &#34;direct&#34; (e.g., &#34;no poverty&#34; matches SDG1: No Poverty)
         or &#34;indirect&#34; (e.g., &#34;no more starving&#34; matches SDG2: Zero Hunger).
 
     Raises
     ------
     TypeError: if text is not a string.
     &#34;&#34;&#34;
-    if not isinstance(text, str): # check input data type
+    if not isinstance(text, str):  # check input data type
         raise TypeError(&#34;Input must be a string.&#34;)
 
     sdgs = []
     targets = []
     matches = []
 
     for item in SDG_keys:
@@ -78,21 +79,22 @@
         sdg_keywords = item[&#34;SDG_keywords&#34;]
         match_type = item[&#34;match_type&#34;]
         if re.search(sdg_keywords, text, re.IGNORECASE):
             sdgs.append(sdg_id.split(&#34;_&#34;)[0])
             targets.append(sdg_id)
             matches.append(match_type)
 
-    sdgs = list(set(sdgs)) # keep unique sdgs
+    sdgs = list(set(sdgs))  # keep unique sdgs
     targets = list(set(targets))
     matches = list(set(matches))
     sus = bool(sdgs)
 
     return sus, sdgs, targets, matches
 
+
 def cat_sus(target):
     &#34;&#34;&#34;
     Categorize SDG targets into social, environmental, and economic sustainability.
 
     Parameters
     ----------
     target: list
@@ -100,28 +102,31 @@
 
     Returns
     -------
     see: dict
         A dictionary of boolean values with social, environmental, and economic sustainability
         as keys.
     &#34;&#34;&#34;
-    see = {&#34;social_sustainability&#34;:0, &#34;environmental_sustainability&#34;:0, &#34;economic_sustainability&#34;:0}
+    see = {&#34;social_sustainability&#34;: 0,
+           &#34;environmental_sustainability&#34;: 0, &#34;economic_sustainability&#34;: 0}
 
     for item in see_keys:
         sdg_id, soc, env, econ = item[:4]
         for i in range(len(target)):
             if target[i] == sdg_id:
                 see[&#34;social_sustainability&#34;] += int(soc)
                 see[&#34;environmental_sustainability&#34;] += int(env)
                 see[&#34;economic_sustainability&#34;] += int(econ)
 
-    see = {key: True if see[key] &gt; 0 else False for key in see} # convert to boolean values
+    # convert to boolean values
+    see = {key: True if see[key] &gt; 0 else False for key in see}
 
     return see
 
+
 def label_sdg(sdg_id):
     &#34;&#34;&#34;
     Label SDG id with SDG description.
 
     Parameters
     ----------
     sdg_id: list
@@ -139,14 +144,15 @@
         goal_id, desc = item[:2]
         for i in range(len(sdg_id)):
             if sdg_id[i] == goal_id:
                 sdg_desc.append(desc)
 
     return sdg_desc
 
+
 def label_target(target_id):
     &#34;&#34;&#34;
     Label target id with target description.
 
     Parameters
     ----------
     target_id: list
@@ -164,14 +170,15 @@
         tar_id, desc = item[:2]
         for i in range(len(target_id)):
             if target_id[i] == tar_id:
                 target_desc.append(desc)
 
     return target_desc
 
+
 class SeeSus():
     &#34;&#34;&#34;
     A social, environmental, and economic sustainability classifier.
 
     Attributes
     ----------
     sus: bool
@@ -205,14 +212,23 @@
             a lengthy paragraph.
         &#34;&#34;&#34;
         self.sus, self.sdg, self.target, self.match = id_sus(text)
         self.sdg_desc = label_sdg(self.sdg)
         self.target_desc = label_target(self.target)
         self.see = cat_sus(self.target)
 
+    def __str__(self):
+        &#34;&#34;&#34;
+        Print out a summary of the results from the classifier
+        &#34;&#34;&#34;
+        str = f&#34;The text matched the following SDGs at the target level:\n&#34;
+        for target, target_desc in zip(self.target, self.target_desc):
+            str += f&#34;    {target} - {target_desc}\n&#34;
+        return str
+
     @staticmethod
     def show_syntax(sdg_id):
         &#34;&#34;&#34;
         Print the regular expression match syntax of target-level SDGs.
 
         Parameters
         ----------
@@ -224,15 +240,15 @@
         None
 
         Raises
         ------
         ValueError: if sdg_id is invalid.
         &#34;&#34;&#34;
         ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
-        if sdg_id not in ids: # check if sdg id is valid
+        if sdg_id not in ids:  # check if sdg id is valid
             raise ValueError(f&#34;Invalid input. Choose one in the list: {ids}&#34;)
 
         syntax = [d for d in SDG_keys if d[&#34;SDG_id&#34;] == sdg_id]
         print(syntax)
 
     @staticmethod
     def edit_syntax(sdg_id, new_syntax, match_type=&#34;indirect&#34;):
@@ -257,25 +273,26 @@
         Raises
         ------
         ValueError: if sdg_id is invalid.
         ValueError: if match_type is invalid.
         &#34;&#34;&#34;
         ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
         if sdg_id not in ids:  # check if sdg id is valid
-            raise ValueError(f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
+            raise ValueError(
+                f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
         if match_type not in [&#34;direct&#34;, &#34;indirect&#34;]:  # check if match type is valid
             raise ValueError(
                 f&#34;Invalid input &#39;{match_type}&#39;. Use &#39;direct&#39; or &#39;indirect&#39;. Default is &#39;indirect&#39;.&#34;)
 
         match = 0
         for item in SDG_keys:
             if item[&#34;SDG_id&#34;] == sdg_id and item[&#34;match_type&#34;] == match_type:
                 match += 1
                 item.update({&#34;SDG_keywords&#34;: new_syntax})
-        if match == 0: # when the direct/indirect match type does not exist
+        if match == 0:  # when the direct/indirect match type does not exist
             SDG_keys.append({&#34;SDG_id&#34;: sdg_id,
                              &#34;SDG_keywords&#34;: new_syntax,
                              &#34;match_type&#34;: match_type})
 
         print(f&#34;The {match_type} match syntax of {sdg_id} has been updated.&#34;)</code></pre>
 </details>
 </section>
@@ -317,25 +334,27 @@
 
     Returns
     -------
     see: dict
         A dictionary of boolean values with social, environmental, and economic sustainability
         as keys.
     &#34;&#34;&#34;
-    see = {&#34;social_sustainability&#34;:0, &#34;environmental_sustainability&#34;:0, &#34;economic_sustainability&#34;:0}
+    see = {&#34;social_sustainability&#34;: 0,
+           &#34;environmental_sustainability&#34;: 0, &#34;economic_sustainability&#34;: 0}
 
     for item in see_keys:
         sdg_id, soc, env, econ = item[:4]
         for i in range(len(target)):
             if target[i] == sdg_id:
                 see[&#34;social_sustainability&#34;] += int(soc)
                 see[&#34;environmental_sustainability&#34;] += int(env)
                 see[&#34;economic_sustainability&#34;] += int(econ)
 
-    see = {key: True if see[key] &gt; 0 else False for key in see} # convert to boolean values
+    # convert to boolean values
+    see = {key: True if see[key] &gt; 0 else False for key in see}
 
     return see</code></pre>
 </details>
 </dd>
 <dt id="seesus.seesus.id_sus"><code class="name flex">
 <span>def <span class="ident">id_sus</span></span>(<span>text)</span>
 </code></dt>
@@ -391,15 +410,15 @@
         Match types, either &#34;direct&#34; (e.g., &#34;no poverty&#34; matches SDG1: No Poverty)
         or &#34;indirect&#34; (e.g., &#34;no more starving&#34; matches SDG2: Zero Hunger).
 
     Raises
     ------
     TypeError: if text is not a string.
     &#34;&#34;&#34;
-    if not isinstance(text, str): # check input data type
+    if not isinstance(text, str):  # check input data type
         raise TypeError(&#34;Input must be a string.&#34;)
 
     sdgs = []
     targets = []
     matches = []
 
     for item in SDG_keys:
@@ -407,15 +426,15 @@
         sdg_keywords = item[&#34;SDG_keywords&#34;]
         match_type = item[&#34;match_type&#34;]
         if re.search(sdg_keywords, text, re.IGNORECASE):
             sdgs.append(sdg_id.split(&#34;_&#34;)[0])
             targets.append(sdg_id)
             matches.append(match_type)
 
-    sdgs = list(set(sdgs)) # keep unique sdgs
+    sdgs = list(set(sdgs))  # keep unique sdgs
     targets = list(set(targets))
     matches = list(set(matches))
     sus = bool(sdgs)
 
     return sus, sdgs, targets, matches</code></pre>
 </details>
 </dd>
@@ -592,14 +611,23 @@
             a lengthy paragraph.
         &#34;&#34;&#34;
         self.sus, self.sdg, self.target, self.match = id_sus(text)
         self.sdg_desc = label_sdg(self.sdg)
         self.target_desc = label_target(self.target)
         self.see = cat_sus(self.target)
 
+    def __str__(self):
+        &#34;&#34;&#34;
+        Print out a summary of the results from the classifier
+        &#34;&#34;&#34;
+        str = f&#34;The text matched the following SDGs at the target level:\n&#34;
+        for target, target_desc in zip(self.target, self.target_desc):
+            str += f&#34;    {target} - {target_desc}\n&#34;
+        return str
+
     @staticmethod
     def show_syntax(sdg_id):
         &#34;&#34;&#34;
         Print the regular expression match syntax of target-level SDGs.
 
         Parameters
         ----------
@@ -611,15 +639,15 @@
         None
 
         Raises
         ------
         ValueError: if sdg_id is invalid.
         &#34;&#34;&#34;
         ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
-        if sdg_id not in ids: # check if sdg id is valid
+        if sdg_id not in ids:  # check if sdg id is valid
             raise ValueError(f&#34;Invalid input. Choose one in the list: {ids}&#34;)
 
         syntax = [d for d in SDG_keys if d[&#34;SDG_id&#34;] == sdg_id]
         print(syntax)
 
     @staticmethod
     def edit_syntax(sdg_id, new_syntax, match_type=&#34;indirect&#34;):
@@ -644,25 +672,26 @@
         Raises
         ------
         ValueError: if sdg_id is invalid.
         ValueError: if match_type is invalid.
         &#34;&#34;&#34;
         ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
         if sdg_id not in ids:  # check if sdg id is valid
-            raise ValueError(f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
+            raise ValueError(
+                f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
         if match_type not in [&#34;direct&#34;, &#34;indirect&#34;]:  # check if match type is valid
             raise ValueError(
                 f&#34;Invalid input &#39;{match_type}&#39;. Use &#39;direct&#39; or &#39;indirect&#39;. Default is &#39;indirect&#39;.&#34;)
 
         match = 0
         for item in SDG_keys:
             if item[&#34;SDG_id&#34;] == sdg_id and item[&#34;match_type&#34;] == match_type:
                 match += 1
                 item.update({&#34;SDG_keywords&#34;: new_syntax})
-        if match == 0: # when the direct/indirect match type does not exist
+        if match == 0:  # when the direct/indirect match type does not exist
             SDG_keys.append({&#34;SDG_id&#34;: sdg_id,
                              &#34;SDG_keywords&#34;: new_syntax,
                              &#34;match_type&#34;: match_type})
 
         print(f&#34;The {match_type} match syntax of {sdg_id} has been updated.&#34;)</code></pre>
 </details>
 <h3>Static methods</h3>
@@ -718,25 +747,26 @@
     Raises
     ------
     ValueError: if sdg_id is invalid.
     ValueError: if match_type is invalid.
     &#34;&#34;&#34;
     ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
     if sdg_id not in ids:  # check if sdg id is valid
-        raise ValueError(f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
+        raise ValueError(
+            f&#34;Invalid input &#39;{sdg_id}&#39;. Use one in the list: {ids}.&#34;)
     if match_type not in [&#34;direct&#34;, &#34;indirect&#34;]:  # check if match type is valid
         raise ValueError(
             f&#34;Invalid input &#39;{match_type}&#39;. Use &#39;direct&#39; or &#39;indirect&#39;. Default is &#39;indirect&#39;.&#34;)
 
     match = 0
     for item in SDG_keys:
         if item[&#34;SDG_id&#34;] == sdg_id and item[&#34;match_type&#34;] == match_type:
             match += 1
             item.update({&#34;SDG_keywords&#34;: new_syntax})
-    if match == 0: # when the direct/indirect match type does not exist
+    if match == 0:  # when the direct/indirect match type does not exist
         SDG_keys.append({&#34;SDG_id&#34;: sdg_id,
                          &#34;SDG_keywords&#34;: new_syntax,
                          &#34;match_type&#34;: match_type})
 
     print(f&#34;The {match_type} match syntax of {sdg_id} has been updated.&#34;)</code></pre>
 </details>
 </dd>
@@ -776,15 +806,15 @@
     None
 
     Raises
     ------
     ValueError: if sdg_id is invalid.
     &#34;&#34;&#34;
     ids = list({item[&#34;SDG_id&#34;] for item in SDG_keys})
-    if sdg_id not in ids: # check if sdg id is valid
+    if sdg_id not in ids:  # check if sdg id is valid
         raise ValueError(f&#34;Invalid input. Choose one in the list: {ids}&#34;)
 
     syntax = [d for d in SDG_keys if d[&#34;SDG_id&#34;] == sdg_id]
     print(syntax)</code></pre>
 </details>
 </dd>
 </dl>
```

#### html2text {}

```diff
@@ -8,14 +8,15 @@
 
 import regex as re
 
 from seesus.SDG_keys import SDG_keys
 from seesus.see_keys import see_keys
 from seesus.SDG_desc import goal_desc, tar_desc
 
+
 def id_sus(text):
     """
     Identify the UN Sustainable Development Goals (SDGs) and their associated
 targets in text.
 
     Parameters
     ----------
@@ -39,15 +40,15 @@
 Poverty)
         or "indirect" (e.g., "no more starving" matches SDG2: Zero Hunger).
 
     Raises
     ------
     TypeError: if text is not a string.
     """
-    if not isinstance(text, str): # check input data type
+    if not isinstance(text, str):  # check input data type
         raise TypeError("Input must be a string.")
 
     sdgs = []
     targets = []
     matches = []
 
     for item in SDG_keys:
@@ -55,21 +56,22 @@
         sdg_keywords = item["SDG_keywords"]
         match_type = item["match_type"]
         if re.search(sdg_keywords, text, re.IGNORECASE):
             sdgs.append(sdg_id.split("_")[0])
             targets.append(sdg_id)
             matches.append(match_type)
 
-    sdgs = list(set(sdgs)) # keep unique sdgs
+    sdgs = list(set(sdgs))  # keep unique sdgs
     targets = list(set(targets))
     matches = list(set(matches))
     sus = bool(sdgs)
 
     return sus, sdgs, targets, matches
 
+
 def cat_sus(target):
     """
     Categorize SDG targets into social, environmental, and economic
 sustainability.
 
     Parameters
     ----------
@@ -79,30 +81,31 @@
     Returns
     -------
     see: dict
         A dictionary of boolean values with social, environmental, and economic
 sustainability
         as keys.
     """
-    see = {"social_sustainability":0, "environmental_sustainability":0,
-"economic_sustainability":0}
+    see = {"social_sustainability": 0,
+           "environmental_sustainability": 0, "economic_sustainability": 0}
 
     for item in see_keys:
         sdg_id, soc, env, econ = item[:4]
         for i in range(len(target)):
             if target[i] == sdg_id:
                 see["social_sustainability"] += int(soc)
                 see["environmental_sustainability"] += int(env)
                 see["economic_sustainability"] += int(econ)
 
-    see = {key: True if see[key] > 0 else False for key in see} # convert to
-boolean values
+    # convert to boolean values
+    see = {key: True if see[key] > 0 else False for key in see}
 
     return see
 
+
 def label_sdg(sdg_id):
     """
     Label SDG id with SDG description.
 
     Parameters
     ----------
     sdg_id: list
@@ -120,14 +123,15 @@
         goal_id, desc = item[:2]
         for i in range(len(sdg_id)):
             if sdg_id[i] == goal_id:
                 sdg_desc.append(desc)
 
     return sdg_desc
 
+
 def label_target(target_id):
     """
     Label target id with target description.
 
     Parameters
     ----------
     target_id: list
@@ -145,14 +149,15 @@
         tar_id, desc = item[:2]
         for i in range(len(target_id)):
             if target_id[i] == tar_id:
                 target_desc.append(desc)
 
     return target_desc
 
+
 class SeeSus():
     """
     A social, environmental, and economic sustainability classifier.
 
     Attributes
     ----------
     sus: bool
@@ -189,14 +194,23 @@
             a lengthy paragraph.
         """
         self.sus, self.sdg, self.target, self.match = id_sus(text)
         self.sdg_desc = label_sdg(self.sdg)
         self.target_desc = label_target(self.target)
         self.see = cat_sus(self.target)
 
+    def __str__(self):
+        """
+        Print out a summary of the results from the classifier
+        """
+        str = f"The text matched the following SDGs at the target level:\n"
+        for target, target_desc in zip(self.target, self.target_desc):
+            str += f"    {target} - {target_desc}\n"
+        return str
+
     @staticmethod
     def show_syntax(sdg_id):
         """
         Print the regular expression match syntax of target-level SDGs.
 
         Parameters
         ----------
@@ -208,15 +222,15 @@
         None
 
         Raises
         ------
         ValueError: if sdg_id is invalid.
         """
         ids = list({item["SDG_id"] for item in SDG_keys})
-        if sdg_id not in ids: # check if sdg id is valid
+        if sdg_id not in ids:  # check if sdg id is valid
             raise ValueError(f"Invalid input. Choose one in the list: {ids}")
 
         syntax = [d for d in SDG_keys if d["SDG_id"] == sdg_id]
         print(syntax)
 
     @staticmethod
     def edit_syntax(sdg_id, new_syntax, match_type="indirect"):
@@ -242,28 +256,28 @@
         Raises
         ------
         ValueError: if sdg_id is invalid.
         ValueError: if match_type is invalid.
         """
         ids = list({item["SDG_id"] for item in SDG_keys})
         if sdg_id not in ids:  # check if sdg id is valid
-            raise ValueError(f"Invalid input '{sdg_id}'. Use one in the list:
-{ids}.")
+            raise ValueError(
+                f"Invalid input '{sdg_id}'. Use one in the list: {ids}.")
         if match_type not in ["direct", "indirect"]:  # check if match type is
 valid
             raise ValueError(
                 f"Invalid input '{match_type}'. Use 'direct' or 'indirect'.
 Default is 'indirect'.")
 
         match = 0
         for item in SDG_keys:
             if item["SDG_id"] == sdg_id and item["match_type"] == match_type:
                 match += 1
                 item.update({"SDG_keywords": new_syntax})
-        if match == 0: # when the direct/indirect match type does not exist
+        if match == 0:  # when the direct/indirect match type does not exist
             SDG_keys.append({"SDG_id": sdg_id,
                              "SDG_keywords": new_syntax,
                              "match_type": match_type})
 
         print(f"The {match_type} match syntax of {sdg_id} has been updated.")
 ********** FFuunnccttiioonnss **********
   def cat_sus(target)
@@ -290,27 +304,28 @@
           Returns
           -------
           see: dict
               A dictionary of boolean values with social, environmental, and
       economic sustainability
               as keys.
           """
-          see = {"social_sustainability":0, "environmental_sustainability":0,
-      "economic_sustainability":0}
+          see = {"social_sustainability": 0,
+                 "environmental_sustainability": 0, "economic_sustainability":
+      0}
 
           for item in see_keys:
               sdg_id, soc, env, econ = item[:4]
               for i in range(len(target)):
                   if target[i] == sdg_id:
                       see["social_sustainability"] += int(soc)
                       see["environmental_sustainability"] += int(env)
                       see["economic_sustainability"] += int(econ)
 
-          see = {key: True if see[key] > 0 else False for key in see} # convert
-      to boolean values
+          # convert to boolean values
+          see = {key: True if see[key] > 0 else False for key in see}
 
           return see
   def id_sus(text)
       Identify the UN Sustainable Development Goals (SDGs) and their associated
       targets in text.
       ********** PPaarraammeetteerrss **********
         tteexxtt : str
@@ -360,15 +375,15 @@
               or "indirect" (e.g., "no more starving" matches SDG2: Zero
       Hunger).
 
           Raises
           ------
           TypeError: if text is not a string.
           """
-          if not isinstance(text, str): # check input data type
+          if not isinstance(text, str):  # check input data type
               raise TypeError("Input must be a string.")
 
           sdgs = []
           targets = []
           matches = []
 
           for item in SDG_keys:
@@ -376,15 +391,15 @@
               sdg_keywords = item["SDG_keywords"]
               match_type = item["match_type"]
               if re.search(sdg_keywords, text, re.IGNORECASE):
                   sdgs.append(sdg_id.split("_")[0])
                   targets.append(sdg_id)
                   matches.append(match_type)
 
-          sdgs = list(set(sdgs)) # keep unique sdgs
+          sdgs = list(set(sdgs))  # keep unique sdgs
           targets = list(set(targets))
           matches = list(set(matches))
           sus = bool(sdgs)
 
           return sus, sdgs, targets, matches
   def label_sdg(sdg_id)
       Label SDG id with SDG description.
@@ -525,14 +540,24 @@
                   a lengthy paragraph.
               """
               self.sus, self.sdg, self.target, self.match = id_sus(text)
               self.sdg_desc = label_sdg(self.sdg)
               self.target_desc = label_target(self.target)
               self.see = cat_sus(self.target)
 
+          def __str__(self):
+              """
+              Print out a summary of the results from the classifier
+              """
+              str = f"The text matched the following SDGs at the target level:
+      \n"
+              for target, target_desc in zip(self.target, self.target_desc):
+                  str += f"    {target} - {target_desc}\n"
+              return str
+
           @staticmethod
           def show_syntax(sdg_id):
               """
               Print the regular expression match syntax of target-level SDGs.
 
               Parameters
               ----------
@@ -544,15 +569,15 @@
               None
 
               Raises
               ------
               ValueError: if sdg_id is invalid.
               """
               ids = list({item["SDG_id"] for item in SDG_keys})
-              if sdg_id not in ids: # check if sdg id is valid
+              if sdg_id not in ids:  # check if sdg id is valid
                   raise ValueError(f"Invalid input. Choose one in the list:
       {ids}")
 
               syntax = [d for d in SDG_keys if d["SDG_id"] == sdg_id]
               print(syntax)
 
           @staticmethod
@@ -579,29 +604,29 @@
               Raises
               ------
               ValueError: if sdg_id is invalid.
               ValueError: if match_type is invalid.
               """
               ids = list({item["SDG_id"] for item in SDG_keys})
               if sdg_id not in ids:  # check if sdg id is valid
-                  raise ValueError(f"Invalid input '{sdg_id}'. Use one in the
-      list: {ids}.")
+                  raise ValueError(
+                      f"Invalid input '{sdg_id}'. Use one in the list: {ids}.")
               if match_type not in ["direct", "indirect"]:  # check if match
       type is valid
                   raise ValueError(
                       f"Invalid input '{match_type}'. Use 'direct' or
       'indirect'. Default is 'indirect'.")
 
               match = 0
               for item in SDG_keys:
                   if item["SDG_id"] == sdg_id and item["match_type"] ==
       match_type:
                       match += 1
                       item.update({"SDG_keywords": new_syntax})
-              if match == 0: # when the direct/indirect match type does not
+              if match == 0:  # when the direct/indirect match type does not
       exist
                   SDG_keys.append({"SDG_id": sdg_id,
                                    "SDG_keywords": new_syntax,
                                    "match_type": match_type})
 
               print(f"The {match_type} match syntax of {sdg_id} has been
       updated.")
@@ -649,29 +674,30 @@
                 Raises
                 ------
                 ValueError: if sdg_id is invalid.
                 ValueError: if match_type is invalid.
                 """
                 ids = list({item["SDG_id"] for item in SDG_keys})
                 if sdg_id not in ids:  # check if sdg id is valid
-                    raise ValueError(f"Invalid input '{sdg_id}'. Use one in the
-            list: {ids}.")
+                    raise ValueError(
+                        f"Invalid input '{sdg_id}'. Use one in the list:
+            {ids}.")
                 if match_type not in ["direct", "indirect"]:  # check if match
             type is valid
                     raise ValueError(
                         f"Invalid input '{match_type}'. Use 'direct' or
             'indirect'. Default is 'indirect'.")
 
                 match = 0
                 for item in SDG_keys:
                     if item["SDG_id"] == sdg_id and item["match_type"] ==
             match_type:
                         match += 1
                         item.update({"SDG_keywords": new_syntax})
-                if match == 0: # when the direct/indirect match type does not
+                if match == 0:  # when the direct/indirect match type does not
             exist
                     SDG_keys.append({"SDG_id": sdg_id,
                                      "SDG_keywords": new_syntax,
                                      "match_type": match_type})
 
                 print(f"The {match_type} match syntax of {sdg_id} has been
             updated.")
@@ -701,15 +727,15 @@
                 None
 
                 Raises
                 ------
                 ValueError: if sdg_id is invalid.
                 """
                 ids = list({item["SDG_id"] for item in SDG_keys})
-                if sdg_id not in ids: # check if sdg id is valid
+                if sdg_id not in ids:  # check if sdg id is valid
                     raise ValueError(f"Invalid input. Choose one in the list:
             {ids}")
 
                 syntax = [d for d in SDG_keys if d["SDG_id"] == sdg_id]
                 print(syntax)
 ************ IInnddeexx ************
     * ******** SSuuppeerr--mmoodduullee ********
```

### Comparing `seesus-1.2.0/pyproject.toml` & `seesus-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm[toml] >= 4, <6",
     "wheel >= 0.29.0",
     ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seesus"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
     {name="Meng Cai", email="mengcai24601@gmail.com"},
     {name="Yingjie Li", email="yingjieli.edu@gmail.com"},
     {name="Dirk Colbry", email="colbrydi@msu.edu"},
     {name="Veronica Frans", email="verofrans@gmail.com"},
     {name="Yuqian Zhang", email="zhan1364@msu.edu"}
     ]
```

### Comparing `seesus-1.2.0/src/seesus/SDG_desc.py` & `seesus-1.2.1/src/seesus/SDG_desc.py`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/src/seesus/SDG_keys.py` & `seesus-1.2.1/src/seesus/SDG_keys.py`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/src/seesus/see_keys.py` & `seesus-1.2.1/src/seesus/see_keys.py`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/src/seesus/seesus.py` & `seesus-1.2.1/src/seesus/seesus.py`

 * *Files identical despite different names*

### Comparing `seesus-1.2.0/tests/test_seesus.py` & `seesus-1.2.1/tests/test_seesus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Test seesus module."""
 
 import pytest
 from seesus import seesus
 
 def test_id_sus():
     """Test identifying the UN Sustainable Development Goals (SDGs) and their associated targets in text."""
-    text = "our goal is end poverty"
-    sus, sdgs, targets, matches = seesus.id_sus(text)
-    assert sus == True
-    assert sdgs == ['SDG1']
-    assert targets == ['SDG1_2']
-    assert matches == ['indirect']
+    text1 = "our goal is to end poverty"
+    text2 = "we care about SDG 2"
+    sus1, sdgs1, targets1, matches1 = seesus.id_sus(text1)
+    sus2, sdgs2, targets2, matches2 = seesus.id_sus(text2)
+    assert sus1 == True
+    assert sdgs1 == ['SDG1']
+    assert targets1 == ['SDG1_2']
+    assert matches1 == ['indirect']
+    assert sus2 == True
+    assert sdgs2 == ['SDG2']
+    assert targets2 == ['SDG2_general']
+    assert matches2 == ['direct']
 
 def test_cat_sus():
     """Test categorizing SDG targets into social, environmental, and economic sustainability."""
     assert seesus.cat_sus(["SDG1_2"]) == {'social_sustainability': True, 
                                              'environmental_sustainability': False, 
                                              'economic_sustainability': False}
```

