# Comparing `tmp/jcci-0.1.2.tar.gz` & `tmp/jcci-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.1.2.tar", last modified: Mon Apr  8 04:32:48 2024, max compression
+gzip compressed data, was "jcci-0.1.3.tar", last modified: Mon Apr  8 06:41:54 2024, max compression
```

## Comparing `jcci-0.1.2.tar` & `jcci-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.967731 jcci-0.1.2/
--rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    15384 2024-04-08 04:32:48.965735 jcci-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4471 2024-04-08 04:32:29.000000 jcci-0.1.2/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-08 04:32:29.000000 jcci-0.1.2/README.pypi.md
--rw-rw-rw-   0        0        0      763 2024-04-08 04:32:29.000000 jcci-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 04:32:48.968731 jcci-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.921731 jcci-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.950732 jcci-0.1.2/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.2/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    45109 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.2/src/jcci/config.py
--rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.2/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.2/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.2/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     7935 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/graph.py
--rw-rw-rw-   0        0        0    38345 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4371 2024-04-08 04:24:10.000000 jcci-0.1.2/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.2/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.962733 jcci-0.1.2/src/jcci.egg-info/
--rw-rw-rw-   0        0        0    15384 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 04:32:48.000000 jcci-0.1.2/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 04:32:48.960731 jcci-0.1.2/test/
--rw-rw-rw-   0        0        0     2525 2024-01-18 02:12:50.000000 jcci-0.1.2/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:41:54.420808 jcci-0.1.3/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    15384 2024-04-08 06:41:54.414806 jcci-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4471 2024-04-08 04:32:29.000000 jcci-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-08 04:32:29.000000 jcci-0.1.3/README.pypi.md
+-rw-rw-rw-   0        0        0      763 2024-04-08 06:41:17.000000 jcci-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 06:41:54.420808 jcci-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 06:41:54.363803 jcci-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 06:41:54.398810 jcci-0.1.3/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:41:00.000000 jcci-0.1.3/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    43468 2024-04-08 05:45:58.000000 jcci-0.1.3/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.3/src/jcci/config.py
+-rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.3/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5352 2024-03-25 09:59:06.000000 jcci-0.1.3/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.3/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7935 2024-04-08 04:24:10.000000 jcci-0.1.3/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    38314 2024-04-08 06:38:12.000000 jcci-0.1.3/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4371 2024-04-08 04:24:10.000000 jcci-0.1.3/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.3/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-08 06:41:54.412803 jcci-0.1.3/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15384 2024-04-08 06:41:53.000000 jcci-0.1.3/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-08 06:41:54.000000 jcci-0.1.3/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 06:41:53.000000 jcci-0.1.3/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-08 06:41:53.000000 jcci-0.1.3/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 06:41:53.000000 jcci-0.1.3/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 06:41:54.410806 jcci-0.1.3/test/
+-rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.1.3/test/test_case.py
```

### Comparing `jcci-0.1.2/LICENSE` & `jcci-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/PKG-INFO` & `jcci-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.2
+Version: 0.1.3
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `jcci-0.1.2/README.md` & `jcci-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/README.pypi.md` & `jcci-0.1.3/README.pypi.md`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/pyproject.toml` & `jcci-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `jcci-0.1.2/src/jcci/analyze.py` & `jcci-0.1.3/src/jcci/analyze.py`

 * *Files 12% similar despite different names*

```diff
@@ -471,56 +471,19 @@
     def _gen_all_possible_method_param_list(self, method_param):
         method_param_list = []
         method_name = method_param.split('(')[0]
         param_type_str = method_param.split('(')[1].split(')')[0]
         param_type_list = param_type_str.split(',')
         if not param_type_list:
             return method_param_list
-        all_possible_method_param_list = []
-        self._replace_with_unknown(param_type_list, all_possible_method_param_list, 0)
-        lst = list(set(tuple(sub_list) for sub_list in all_possible_method_param_list))
-        for param_type_list in lst:
+        all_possible_method_param_list = self._replace_with_null_unknown(param_type_list)
+        for param_type_list in all_possible_method_param_list:
             method_param_list.append(f'{method_name}({",".join(param_type_list)})')
         return method_param_list
 
-    def _replace_with_null(self, lst):
-        # lst = [item.split('<')[0].replace('<', '').replace('>', '') for item in lst]
-        results = []
-        lowercase_indices = [i for i, s in enumerate(lst) if s and s[0].islower()]  # 首字母小写的元素索引
-
-        for num_replacements in range(len(lst) + 1):  # 遍历替换0到所有元素的情况
-            replaceable_indices = [i for i in range(len(lst)) if i not in lowercase_indices]  # 可替换的元素索引
-            for replace_indices in combinations(replaceable_indices, num_replacements):  # 所有可能的替换索引组合
-                new_lst = lst[:]  # 创建原始列表的副本
-                for idx in replace_indices:
-                    if new_lst[idx].lower() not in constant.JAVA_BASIC_TYPE:
-                        if new_lst[idx].startswith('List'):
-                            new_lst2 = new_lst[:]
-                            new_lst2[idx] = 'ArrayList'
-                            results.append(new_lst2)
-                        elif new_lst[idx].startswith('Map'):
-                            new_lst2 = new_lst[:]
-                            new_lst2[idx] = 'HashMap'
-                            results.append(new_lst2)
-                        elif new_lst[idx].startswith('Set'):
-                            new_lst2 = new_lst[:]
-                            new_lst2[idx] = 'HashSet'
-                            results.append(new_lst2)
-                        new_lst[idx] = constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
-                    else:
-                        new_lst2 = new_lst[:]
-                        new_lst2[idx] = constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
-                        results.append(new_lst2)
-                        new_lst[idx] = 'null'
-                        self._replace_extends_class(new_lst2, results)
-                results.append(new_lst)
-                self._replace_extends_class(new_lst, results)
-        results.append([constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN for _ in lst])
-        return results
-
     def _replace_extends_class(self, new_lst, results):
         for i in range(0, len(new_lst)):
             if new_lst[i].lower() in constant.JAVA_BASIC_TYPE \
                     or new_lst[i] == constant.PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN \
                     or new_lst[i] == 'null':
                 continue
             extends_package_class_list = self._get_extends_package_class(new_lst[i])
@@ -534,15 +497,26 @@
         for item in lst:
             if item == new_lst:
                 is_duplicate = True
                 break
         return is_duplicate
 
     # Step 5.4.1.1
-    def _replace_with_unknown(self, lst: list, results: list, idx: int):
+    def _replace_with_null_unknown(self, lst: list):
+        need_replace_list = []
+        replaced_list = []
+        results = []
+        self._replace_params_with_unknown(lst, results, 0, need_replace_list)
+        for item in need_replace_list:
+            if item not in replaced_list:
+                replaced_list.append(item)
+                self._replace_params_with_unknown(item['list'], results, item['index'], need_replace_list)
+        return list(set(tuple(sub_list) for sub_list in results))
+
+    def _replace_params_with_unknown(self, lst: list, results: list, idx: int, need_replace_list: list):
         # data = [item.split('<')[0].replace('<', '').replace('>', '') for item in data]
         for i in range(idx, len(lst)):
             new_lst = lst[:]
             if not self._is_duplicate_item(new_lst, results):
                 results.append(new_lst)
             if new_lst[i].lower() not in constant.JAVA_BASIC_TYPE:
                 new_lst2 = new_lst[:]
@@ -550,28 +524,28 @@
                     new_lst2[i] = 'ArrayList'
                 elif new_lst[i].startswith('Map'):
                     new_lst2[i] = 'HashMap'
                 elif new_lst[i].startswith('Set'):
                     new_lst2[i] = 'HashSet'
                 if not self._is_duplicate_item(new_lst2, results):
                     results.append(new_lst2)
-                    self._replace_with_unknown(new_lst2, results, idx)
+                    need_replace_list.append({'list': new_lst2, 'index': idx})
             else:
                 if new_lst[i][0].isupper() and new_lst[i] != 'String':
                     new_lst2 = new_lst[:]
                     new_lst2[i] = new_lst[i][0].lower() + new_lst[i][1:]
                     if not self._is_duplicate_item(new_lst2, results):
                         results.append(new_lst2)
-                        self._replace_with_unknown(new_lst2, results, idx)
+                        need_replace_list.append({'list': new_lst2, 'index': idx})
             for el in ['null', 'unknown']:
                 new_lst_tmp = new_lst[:]
                 new_lst_tmp[i] = el
                 if not self._is_duplicate_item(new_lst_tmp, results):
                     results.append(new_lst_tmp)
-                    self._replace_with_unknown(new_lst_tmp, results, min(idx, len(new_lst) - 1))
+                    need_replace_list.append({'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)})
 
     # Step 5.5
     def _get_method_param_string(self, method_db: dict):
         method_name: str = method_db['method_name']
         params: list = json.loads(method_db['parameters'])
         params_type_list = [param['parameter_type'] for param in params]
         return f'{method_name}({",".join(params_type_list)})'
```

### Comparing `jcci-0.1.2/src/jcci/constant.py` & `jcci-0.1.3/src/jcci/constant.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci/database.py` & `jcci-0.1.3/src/jcci/database.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci/diff_parse.py` & `jcci-0.1.3/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci/graph.py` & `jcci-0.1.3/src/jcci/graph.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci/java_parse.py` & `jcci-0.1.3/src/jcci/java_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         imports = [dict(import_obj, class_id=class_id, project_id=self.project_id) for import_obj in import_list]
         self.sqlite.update_data(f'DELETE FROM import WHERE class_id={class_id}')
         self.sqlite.insert_data('import', imports)
 
         # 处理 field 信息
         field_list = self._parse_fields(tree.types[0].fields, package_name, class_id, import_map)
         field_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': package_class, 'start_line': field_obj['start_line']} for field_obj in field_list}
-        import_map = dict((k, v) for k, v in import_map.items() if v.startswith('com.patsnap'))
+        import_map = dict((k, v) for k, v in import_map.items())
 
         # 将extend class的field导进来
         extends_class_fields_map = self._get_extends_class_fields_map(class_id)
         extends_class_fields_map.update(field_map)
         # 处理 methods 信息
         self._parse_method(tree.types[0].methods, lines, class_id, import_map, extends_class_fields_map)
```

### Comparing `jcci-0.1.2/src/jcci/mapper_parse.py` & `jcci-0.1.3/src/jcci/mapper_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci/sql.py` & `jcci-0.1.3/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.2/src/jcci.egg-info/PKG-INFO` & `jcci-0.1.3/src/jcci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.2
+Version: 0.1.3
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

