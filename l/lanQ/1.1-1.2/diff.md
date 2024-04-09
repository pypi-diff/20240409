# Comparing `tmp/lanQ-1.1.tar.gz` & `tmp/lanQ-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.1.tar", last modified: Wed Apr  3 05:59:27 2024, max compression
+gzip compressed data, was "lanQ-1.2.tar", last modified: Tue Apr  9 06:12:22 2024, max compression
```

## Comparing `lanQ-1.1.tar` & `lanQ-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.862362 lanQ-1.1/
--rw-rw-rw-   0        0        0      192 2024-04-03 05:59:27.860368 lanQ-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7924 2024-04-03 05:56:27.000000 lanQ-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.859397 lanQ-1.1/lanQ.egg-info/
--rw-rw-rw-   0        0        0      192 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 05:59:27.000000 lanQ-1.1/lanQ.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 05:59:27.857376 lanQ-1.1/lanQ_rule/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.1/lanQ_rule/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-04-03 05:46:02.000000 lanQ-1.1/lanQ_rule/base.py
--rw-rw-rw-   0        0        0     7941 2024-04-03 05:50:12.000000 lanQ-1.1/lanQ_rule/common_rule.py
--rw-rw-rw-   0        0        0      868 2024-03-25 03:11:10.000000 lanQ-1.1/lanQ_rule/const.py
--rw-rw-rw-   0        0        0      975 2024-04-03 05:52:18.000000 lanQ-1.1/lanQ_rule/model_rule.py
--rw-rw-rw-   0        0        0     1126 2024-04-03 05:46:02.000000 lanQ-1.1/lanQ_rule/prompt_rule.py
--rw-rw-rw-   0        0        0       42 2024-04-03 05:59:27.863363 lanQ-1.1/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-04-03 05:58:48.000000 lanQ-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.206966 lanQ-1.2/
+-rw-rw-rw-   0        0        0      192 2024-04-09 06:12:22.203970 lanQ-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5672 2024-04-08 09:38:17.000000 lanQ-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.202973 lanQ-1.2/lanQ.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 06:12:22.000000 lanQ-1.2/lanQ.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 06:12:22.200978 lanQ-1.2/lanQ_rule/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:32:28.000000 lanQ-1.2/lanQ_rule/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-04-03 05:46:02.000000 lanQ-1.2/lanQ_rule/base.py
+-rw-rw-rw-   0        0        0    10522 2024-04-08 09:12:55.000000 lanQ-1.2/lanQ_rule/common_rule.py
+-rw-rw-rw-   0        0        0     1040 2024-04-08 09:12:55.000000 lanQ-1.2/lanQ_rule/const.py
+-rw-rw-rw-   0        0        0      975 2024-04-03 05:52:18.000000 lanQ-1.2/lanQ_rule/model_rule.py
+-rw-rw-rw-   0        0        0     1126 2024-04-03 05:46:02.000000 lanQ-1.2/lanQ_rule/prompt_rule.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 06:12:22.206966 lanQ-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-08 09:29:55.000000 lanQ-1.2/setup.py
```

### Comparing `lanQ-1.1/lanQ_rule/base.py` & `lanQ-1.2/lanQ_rule/base.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.1/lanQ_rule/common_rule.py` & `lanQ-1.2/lanQ_rule/common_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,14 +86,25 @@
         return res
     if str_len / seg_len <= 1.1:
         res["error_status"] = True
         res["error_type"] = ERROR_CHAOS_ZH
         res['error_reason'] = '中文乱码'
     return res
 
+def common_check_photo(content: str) -> dict:
+    """content是否包含图片"""
+    res = {'error_status': False}
+    pattern = '!\[\]\(http[s]?://.*?jpeg "\n"\)'
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_CHECK_PHOTO
+        res['error_reason'] = matches
+    return res
+
 def common_colon_end(content: str) -> dict:
     """content最后一个字符是冒号."""
     res = {'error_status': False}
     if len(content) <= 0:
         return res
     if content[-1] == ':':
         res['error_status'] = True
@@ -142,14 +153,75 @@
     ratio = enter_count / count * 100
     if ratio >= 25:
         res["error_status"] = True
         res["error_type"] = ERROR_ENTER_MORE
         res['error_reason'] = '回车超过正文25%'
     return res
 
+def common_html_entity(content: str) -> dict:
+    """检测content是否包含实体标记"""
+    res = {'error_status': False}
+    entities = [
+        "nbsp",
+        "lt",
+        "gt",
+        "amp",
+        "quot",
+        "apos",
+        "hellip",
+        "ndash",
+        "mdash",
+        "lsquo",
+        "rsquo",
+        "ldquo",
+        "rdquo",
+    ]
+    full_entities_1 = [f"&{entity}；" for entity in entities]
+    full_entities_2 = [f"&{entity};" for entity in entities]
+    full_entities_3 = [f"＆{entity};" for entity in entities]
+    full_entities_4 = [f"＆{entity}；" for entity in entities]
+    full_entities = (
+        full_entities_1 + full_entities_2 + full_entities_3 + full_entities_4
+    )
+    # half_entity_1 = [f"{entity}；" for entity in entities]
+    half_entity_2 = [f"＆{entity}" for entity in entities]
+    half_entity_3 = [f"&{entity}" for entity in entities]
+    # half_entity_4 = [f"{entity};" for entity in entities]
+    half_entities = half_entity_2 + half_entity_3
+    # maked_entities = [f"{entity}" for entity in entities]
+    all_entities = full_entities + half_entities
+    for entity in all_entities:
+        if entity in content:
+            res["error_status"] = True
+            res["error_type"] = ERROR_HTML_ENTITY
+            res['error_reason'] = 'html实体标记'
+    return res
+
+def common_img_html_tag(content: str) -> dict:
+    """content是否包含图片或html标签"""
+    res = {'error_status': False}
+    pattern = r"(<img[^>]*>)|<p[^>]*>(.*?)<\/p>|<o:p[^>]*>(.*?)<\/o:p>"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_IMG_HTML_TAG
+        res['error_reason'] = matches
+    return res
+
+def common_invisible_char(content: str) -> dict:
+    """content是否包含不可见字符"""
+    res = {'error_status': False}
+    pattern = r"[\u2000-\u200F\u202F\u205F\u3000\uFEFF\u00A0\u2060-\u206F\uFEFF\xa0]"
+    matches = re.findall(pattern, content)
+    if matches:
+        res["error_status"] = True
+        res["error_type"] = ERROR_INVISIBLE_CHAR
+        res['error_reason'] = matches
+    return res
+
 def common_language_mixed(content: str) -> dict:
     """检查content内是否有中英文混杂."""
     res = {'error_status': False}
     s = normalize(content)
     en_len = len(re.findall(r'[a-zA-Z]', s))
     zh_len = len(re.findall(r'[\u4e00-\u9fa5]', s))
     count_len = len(s)
@@ -191,20 +263,20 @@
         res["error_status"] = True
         res["error_type"] = ERROR_SPACE_MORE
         res['error_reason'] = '存在连续500个空格'
     return res
 
 def common_special_character(content: str) -> dict:
     res = {'error_status': False}
-    pattern = r'[�]'
+    pattern = r"[�□\^]|\{\/U\}"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
         res["error_type"] = ERROR_SPECIAL_CHARACTER
-        res['error_reason'] = '特殊符号�'
+        res['error_reason'] = matches
     return res
 
 def common_url_only(content: str) -> dict:
     """检查content内是否只有url."""
     res = {'error_status': False}
     pattern = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'  # noqa
     s = re.sub(pattern, '', content)
```

### Comparing `lanQ-1.1/lanQ_rule/model_rule.py` & `lanQ-1.2/lanQ_rule/model_rule.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.1/lanQ_rule/prompt_rule.py` & `lanQ-1.2/lanQ_rule/prompt_rule.py`

 * *Files identical despite different names*

