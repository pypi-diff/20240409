# Comparing `tmp/cosl-0.0.8.tar.gz` & `tmp/cosl-0.0.9.tar.gz`

## Comparing `cosl-0.0.8.tar` & `cosl-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 cosl-0.0.8/CODEOWNERS
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 cosl-0.0.8/tox.ini
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 cosl-0.0.8/.github/workflows/pull-request.yaml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 cosl-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/__init__.py
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/cos_tool.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/grafana_dashboard.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/juju_topology.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/py.typed
--rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/rules.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 cosl-0.0.8/src/cosl/types.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_cos_tool.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_cos_tool_logql.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_cos_tool_promql.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_grafana_dashboard.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_import_all.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_juju_topology.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_juju_topology_from_charm.py
--rw-r--r--   0        0        0    16356 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/test_rules_promql.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/alert_rules_with_unit_topology/nothing_is_up.rule
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/bad_alert_expressions/missing_expr.rule
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/bad_alert_rules/bad_yaml.rule
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/non_standard_prometheus_alert_rules/odd.rule
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/cpu_overuse.rule
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/cpu_overuse_no_labels.rule
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/target_missing.rule
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/with_template_string.rule
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/with_template_string_and_unit.rule
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cosl-0.0.8/tests/promql_rules/prometheus_alert_rules/nested/target_missing.rule
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cosl-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 cosl-0.0.8/LICENSE
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 cosl-0.0.8/README.md
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 cosl-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 cosl-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 cosl-0.0.9/CODEOWNERS
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 cosl-0.0.9/tox.ini
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cosl-0.0.9/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 cosl-0.0.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 cosl-0.0.9/.github/workflows/pull-request.yaml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 cosl-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/__init__.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/cos_tool.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/grafana_dashboard.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/juju_topology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/py.typed
+-rw-r--r--   0        0        0    17259 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/rules.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 cosl-0.0.9/src/cosl/types.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_cos_tool.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_cos_tool_logql.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_cos_tool_promql.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_grafana_dashboard.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_import_all.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_juju_topology.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_juju_topology_from_charm.py
+-rw-r--r--   0        0        0    16356 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/test_rules_promql.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/alert_rules_with_unit_topology/nothing_is_up.rule
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/bad_alert_expressions/missing_expr.rule
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/bad_alert_rules/bad_yaml.rule
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/non_standard_prometheus_alert_rules/odd.rule
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/cpu_overuse.rule
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/cpu_overuse_no_labels.rule
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/target_missing.rule
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/with_template_string.rule
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/with_template_string_and_unit.rule
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cosl-0.0.9/tests/promql_rules/prometheus_alert_rules/nested/target_missing.rule
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cosl-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 cosl-0.0.9/LICENSE
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 cosl-0.0.9/README.md
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 cosl-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 cosl-0.0.9/PKG-INFO
```

### Comparing `cosl-0.0.8/tox.ini` & `cosl-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/.github/workflows/pull-request.yaml` & `cosl-0.0.9/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/.github/workflows/release.yaml` & `cosl-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/src/cosl/cos_tool.py` & `cosl-0.0.9/src/cosl/cos_tool.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/src/cosl/grafana_dashboard.py` & `cosl-0.0.9/src/cosl/grafana_dashboard.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/src/cosl/juju_topology.py` & `cosl-0.0.9/src/cosl/juju_topology.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/src/cosl/rules.py` & `cosl-0.0.9/src/cosl/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,18 @@
                             if label not in rule["labels"]:
                                 rule["labels"][label] = val
 
                         # insert juju topology filters into a prometheus rule
                         repl = r'job=~".+"' if self.query_type == "logql" else ""
                         rule["expr"] = self.tool.inject_label_matchers(  # type: ignore
                             expression=re.sub(r"%%juju_topology%%,?", repl, rule["expr"]),
-                            topology=self.topology.alert_expression_dict,
+                            topology={
+                                k: rule["labels"][k]
+                                for k in ("juju_model", "juju_model_uuid", "juju_application")
+                            },
                             query_type=self.query_type,
                         )
 
             return groups
 
     def _group_name(self, root_path: str, file_path: str, group_name: str) -> str:
         """Generate group name from path and topology.
```

### Comparing `cosl-0.0.8/src/cosl/types.py` & `cosl-0.0.9/src/cosl/types.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_cos_tool.py` & `cosl-0.0.9/tests/test_cos_tool.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_cos_tool_logql.py` & `cosl-0.0.9/tests/test_cos_tool_logql.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_cos_tool_promql.py` & `cosl-0.0.9/tests/test_cos_tool_promql.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_juju_topology.py` & `cosl-0.0.9/tests/test_juju_topology.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_juju_topology_from_charm.py` & `cosl-0.0.9/tests/test_juju_topology_from_charm.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/tests/test_rules_promql.py` & `cosl-0.0.9/tests/test_rules_promql.py`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/.gitignore` & `cosl-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/LICENSE` & `cosl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cosl-0.0.8/pyproject.toml` & `cosl-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "PyYAML", "typing-extensions"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cosl"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="sed-i", email="82407168+sed-i@users.noreply.github.com" },
 ]
 description = "Utils for COS Lite charms"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `cosl-0.0.8/PKG-INFO` & `cosl-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utils for COS Lite charms
 Project-URL: Homepage, https://github.com/canonical/cos-lib
 Project-URL: Bug Tracker, https://github.com/canonical/cos-lib/issues
 Author-email: sed-i <82407168+sed-i@users.noreply.github.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

