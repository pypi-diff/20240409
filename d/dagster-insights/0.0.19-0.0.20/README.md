# Comparing `tmp/dagster-insights-0.0.19.tar.gz` & `tmp/dagster-insights-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-insights-0.0.19.tar", last modified: Tue Mar  5 23:22:39 2024, max compression
+gzip compressed data, was "dagster-insights-0.0.20.tar", last modified: Tue Apr  9 20:43:00 2024, max compression
```

## Comparing `dagster-insights-0.0.19.tar` & `dagster-insights-0.0.20.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.591319 dagster-insights-0.0.19/
--rw-r--r--   0 prha       (501) staff       (20)       90 2024-01-10 23:26:38.000000 dagster-insights-0.0.19/LICENSE.md
--rw-r--r--   0 prha       (501) staff       (20)     1287 2024-03-05 23:22:39.590846 dagster-insights-0.0.19/PKG-INFO
--rw-r--r--   0 prha       (501) staff       (20)      929 2024-01-10 23:26:38.000000 dagster-insights-0.0.19/README.md
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.590209 dagster-insights-0.0.19/dagster_insights.egg-info/
--rw-r--r--   0 prha       (501) staff       (20)     1287 2024-03-05 23:22:39.000000 dagster-insights-0.0.19/dagster_insights.egg-info/PKG-INFO
--rw-r--r--   0 prha       (501) staff       (20)     1428 2024-03-05 23:22:39.000000 dagster-insights-0.0.19/dagster_insights.egg-info/SOURCES.txt
--rw-r--r--   0 prha       (501) staff       (20)        1 2024-03-05 23:22:39.000000 dagster-insights-0.0.19/dagster_insights.egg-info/dependency_links.txt
--rw-r--r--   0 prha       (501) staff       (20)       14 2024-03-05 23:22:39.000000 dagster-insights-0.0.19/dagster_insights.egg-info/requires.txt
--rw-r--r--   0 prha       (501) staff       (20)       28 2024-03-05 23:22:39.000000 dagster-insights-0.0.19/dagster_insights.egg-info/top_level.txt
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.584583 dagster-insights-0.0.19/dagster_insights_prerelease/
--rw-r--r--   0 prha       (501) staff       (20)      290 2024-01-10 23:26:38.000000 dagster-insights-0.0.19/dagster_insights_prerelease/__init__.py
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.586673 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/
--rw-r--r--   0 prha       (501) staff       (20)     1873 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/__init__.py
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.587863 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/
--rw-r--r--   0 prha       (501) staff       (20)        0 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/__init__.py
--rw-r--r--   0 prha       (501) staff       (20)      816 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/bigquery_utils.py
--rw-r--r--   0 prha       (501) staff       (20)     6941 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/dbt_wrapper.py
--rw-r--r--   0 prha       (501) staff       (20)     3234 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 prha       (501) staff       (20)      138 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/errors.py
--rw-r--r--   0 prha       (501) staff       (20)     2375 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/insights_utils.py
--rw-r--r--   0 prha       (501) staff       (20)    10824 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/metrics_utils.py
--rw-r--r--   0 prha       (501) staff       (20)     1403 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/query.py
-drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-03-05 23:22:39.589665 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/
--rw-r--r--   0 prha       (501) staff       (20)        0 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/__init__.py
--rw-r--r--   0 prha       (501) staff       (20)     5611 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 prha       (501) staff       (20)     5145 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/dbt_wrapper.py
--rw-r--r--   0 prha       (501) staff       (20)     7064 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/definitions.py
--rw-r--r--   0 prha       (501) staff       (20)     9358 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 prha       (501) staff       (20)     3808 2024-03-05 23:22:36.000000 dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/snowflake_utils.py
--rw-r--r--   0 prha       (501) staff       (20)      358 2024-03-05 23:05:02.000000 dagster-insights-0.0.19/pyproject.toml
--rw-r--r--   0 prha       (501) staff       (20)       38 2024-03-05 23:22:39.591434 dagster-insights-0.0.19/setup.cfg
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.413414 dagster-insights-0.0.20/
+-rw-r--r--   0 prha       (501) staff       (20)       90 2024-03-20 04:14:20.000000 dagster-insights-0.0.20/LICENSE.md
+-rw-r--r--   0 prha       (501) staff       (20)     1287 2024-04-09 20:43:00.413205 dagster-insights-0.0.20/PKG-INFO
+-rw-r--r--   0 prha       (501) staff       (20)      929 2024-03-20 04:14:20.000000 dagster-insights-0.0.20/README.md
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.412969 dagster-insights-0.0.20/dagster_insights.egg-info/
+-rw-r--r--   0 prha       (501) staff       (20)     1287 2024-04-09 20:43:00.000000 dagster-insights-0.0.20/dagster_insights.egg-info/PKG-INFO
+-rw-r--r--   0 prha       (501) staff       (20)     1428 2024-04-09 20:43:00.000000 dagster-insights-0.0.20/dagster_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 prha       (501) staff       (20)        1 2024-04-09 20:43:00.000000 dagster-insights-0.0.20/dagster_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 prha       (501) staff       (20)       14 2024-04-09 20:43:00.000000 dagster-insights-0.0.20/dagster_insights.egg-info/requires.txt
+-rw-r--r--   0 prha       (501) staff       (20)       28 2024-04-09 20:43:00.000000 dagster-insights-0.0.20/dagster_insights.egg-info/top_level.txt
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.410255 dagster-insights-0.0.20/dagster_insights_prerelease/
+-rw-r--r--   0 prha       (501) staff       (20)      290 2024-03-20 04:14:20.000000 dagster-insights-0.0.20/dagster_insights_prerelease/__init__.py
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.411146 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/
+-rw-r--r--   0 prha       (501) staff       (20)     1873 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/__init__.py
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.411730 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/
+-rw-r--r--   0 prha       (501) staff       (20)        0 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/__init__.py
+-rw-r--r--   0 prha       (501) staff       (20)      816 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/bigquery_utils.py
+-rw-r--r--   0 prha       (501) staff       (20)     7964 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/dbt_wrapper.py
+-rw-r--r--   0 prha       (501) staff       (20)     3234 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 prha       (501) staff       (20)      138 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/errors.py
+-rw-r--r--   0 prha       (501) staff       (20)     2524 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/insights_utils.py
+-rw-r--r--   0 prha       (501) staff       (20)    10835 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/metrics_utils.py
+-rw-r--r--   0 prha       (501) staff       (20)     1403 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/query.py
+drwxr-xr-x   0 prha       (501) staff       (20)        0 2024-04-09 20:43:00.412771 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/
+-rw-r--r--   0 prha       (501) staff       (20)        0 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/__init__.py
+-rw-r--r--   0 prha       (501) staff       (20)     5611 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 prha       (501) staff       (20)     5185 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/dbt_wrapper.py
+-rw-r--r--   0 prha       (501) staff       (20)     7064 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/definitions.py
+-rw-r--r--   0 prha       (501) staff       (20)     9358 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 prha       (501) staff       (20)     3808 2024-04-09 20:42:59.000000 dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/snowflake_utils.py
+-rw-r--r--   0 prha       (501) staff       (20)      358 2024-04-09 20:22:30.000000 dagster-insights-0.0.20/pyproject.toml
+-rw-r--r--   0 prha       (501) staff       (20)       38 2024-04-09 20:43:00.413464 dagster-insights-0.0.20/setup.cfg
```

### Comparing `dagster-insights-0.0.19/PKG-INFO` & `dagster-insights-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-insights
-Version: 0.0.19
+Version: 0.0.20
 Summary: Latest pre-release patches for dagster_cloud.dagster_insights.
 Author: Dagster Labs
 License: Released under the same license as dagster-cloud: https://pypi.org/project/dagster-cloud/
         
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dagster-cloud
```

### Comparing `dagster-insights-0.0.19/README.md` & `dagster-insights-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights.egg-info/PKG-INFO` & `dagster-insights-0.0.20/dagster_insights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-insights
-Version: 0.0.19
+Version: 0.0.20
 Summary: Latest pre-release patches for dagster_cloud.dagster_insights.
 Author: Dagster Labs
 License: Released under the same license as dagster-cloud: https://pypi.org/project/dagster-cloud/
         
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dagster-cloud
```

### Comparing `dagster-insights-0.0.19/dagster_insights.egg-info/SOURCES.txt` & `dagster-insights-0.0.20/dagster_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/__init__.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/bigquery_utils.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/dbt_wrapper.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/dbt_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
-    Any,
     Iterable,
     Iterator,
     Optional,
     Union,
 )
 
-import dagster._check as check
+import yaml
 from dagster import (
     AssetCheckResult,
     AssetExecutionContext,
     AssetKey,
     AssetMaterialization,
     AssetObservation,
-    MetadataValue,
     OpExecutionContext,
     Output,
 )
-from dagster._core.definitions.metadata import MetadataMapping
-from google.cloud import bigquery
+from dagster_dbt import DbtCliInvocation
+from dagster_dbt.version import __version__ as dagster_dbt_version
+from packaging import version
 
 from ..insights_utils import extract_asset_info_from_event
 from .bigquery_utils import build_bigquery_cost_metadata, marker_asset_key_for_job
 
 if TYPE_CHECKING:
-    from dagster_dbt import DbtCliInvocation
+    from dbt.adapters.base.impl import BaseAdapter
+    from google.cloud import bigquery
+
+OPAQUE_ID_SQL_SIGIL = "bigquery_dagster_dbt_v1_opaque_id"
+DEFAULT_BQ_REGION = "region-us"
+MIN_DAGSTER_DBT_VERSION = "1.7.0"
 
 
 @dataclass
 class BigQueryCostInfo:
     asset_key: AssetKey
     partition: Optional[str]
     job_id: Optional[str]
@@ -43,39 +47,22 @@
         return (
             f"{self.asset_key.to_string()}:{self.partition}"
             if self.partition
             else self.asset_key.to_string()
         )
 
 
-def _extract_metadata_value(value: Optional[MetadataValue], default_value: Any = None) -> Any:
-    return value.value if value else default_value
-
-
-def _extract_bigquery_info_from_metadata(metadata: MetadataMapping):
-    job_id = _extract_metadata_value(metadata.get("job_id"))
-    bytes_billed = _extract_metadata_value(metadata.get("bytes_billed"), 0)
-    slots_ms = _extract_metadata_value(metadata.get("slots_ms"), 0)
-    return job_id, bytes_billed, slots_ms
-
-
-def _asset_partition_key(asset_key: AssetKey, partition_key: Optional[str]) -> str:
-    return f"{asset_key.to_string()}:{partition_key}" if partition_key else asset_key.to_string()
-
-
 def dbt_with_bigquery_insights(
     context: Union[OpExecutionContext, AssetExecutionContext],
-    dbt_cli_invocation: "DbtCliInvocation",
+    dbt_cli_invocation: DbtCliInvocation,
     dagster_events: Optional[
         Iterable[Union[Output, AssetMaterialization, AssetObservation, AssetCheckResult]]
     ] = None,
+    skip_config_check=False,
     record_observation_usage: bool = True,
-    explicitly_query_information_schema: bool = False,
-    bigquery_client: Optional[bigquery.Client] = None,
-    bigquery_location: Optional[str] = None,
 ) -> Iterator[Union[Output, AssetMaterialization, AssetObservation, AssetCheckResult]]:
     """Wraps a dagster-dbt invocation to associate each BigQuery query with the produced
     asset materializations. This allows the cost of each query to be associated with the asset
     materialization that it produced.
 
     If called in the context of an op (rather than an asset), filters out any Output events
     which do not correspond with any output of the op.
@@ -98,68 +85,105 @@
         def jaffle_shop_dbt_assets(
             context: AssetExecutionContext,
             dbt: DbtCliResource,
         ):
             dbt_cli_invocation = dbt.cli(["build"], context=context)
             yield from dbt_with_bigquery_insights(context, dbt_cli_invocation)
     """
-    if explicitly_query_information_schema:
-        check.inst_param(bigquery_client, "bigquery_client", bigquery.Client)
-        check.str_param(bigquery_location, "bigquery_location")
+    if not skip_config_check:
+        adapter_type = dbt_cli_invocation.manifest["metadata"]["adapter_type"]
+        if adapter_type != "bigquery":
+            raise RuntimeError(
+                f"The 'bigquery' adapter must be used but instead found '{adapter_type}'"
+            )
+        dbt_project_config = yaml.safe_load(
+            (dbt_cli_invocation.project_dir / "dbt_project.yml").open("r")
+        )
+        # sanity check that the sigil is present somewhere in the query comment
+        query_comment = dbt_project_config.get("query-comment")
+        if query_comment is None:
+            raise RuntimeError("query-comment is required in dbt_project.yml but it was missing")
+        comment = query_comment.get("comment")
+        if comment is None:
+            raise RuntimeError(
+                "query-comment.comment is required in dbt_project.yml but it was missing"
+            )
+        if OPAQUE_ID_SQL_SIGIL not in comment:
+            raise RuntimeError(
+                "query-comment.comment in dbt_project.yml must contain the string"
+                f" '{OPAQUE_ID_SQL_SIGIL}'. Read the Dagster Insights docs for more info."
+            )
 
     if dagster_events is None:
         dagster_events = dbt_cli_invocation.stream()
 
-    asset_info_by_job_id = {}
-    cost_by_asset = defaultdict(list)
+    asset_info_by_unique_id = {}
     for dagster_event in dagster_events:
-        if isinstance(dagster_event, (AssetMaterialization, AssetObservation, Output)):
+        if isinstance(
+            dagster_event, (AssetMaterialization, AssetObservation, Output, AssetCheckResult)
+        ):
+            unique_id = dagster_event.metadata["unique_id"].value
             asset_key, partition = extract_asset_info_from_event(
                 context, dagster_event, record_observation_usage
             )
             if not asset_key:
                 asset_key = marker_asset_key_for_job(context.job_def)
-            job_id, bytes_billed, slots_ms = _extract_bigquery_info_from_metadata(
-                dagster_event.metadata
-            )
-            if bytes_billed or slots_ms:
-                asset_info_by_job_id[job_id] = (asset_key, partition)
-                cost_info = BigQueryCostInfo(asset_key, partition, job_id, slots_ms, bytes_billed)
-                cost_by_asset[cost_info.asset_partition_key].append(cost_info)
+            asset_info_by_unique_id[unique_id] = (asset_key, partition)
 
         yield dagster_event
 
-    if explicitly_query_information_schema and bigquery_client:
-        marker_asset_key = marker_asset_key_for_job(context.job_def)
-        run_results_json = dbt_cli_invocation.get_artifact("run_results.json")
-        invocation_id = run_results_json["metadata"]["invocation_id"]
-        assert bigquery_client
-        try:
-            cost_query = f"""
-                SELECT job_id, SUM(total_bytes_billed) AS bytes_billed, SUM(total_slot_ms) AS slots_ms
-                FROM `{bigquery_location}`.INFORMATION_SCHEMA.JOBS
-                WHERE query like '%{invocation_id}%'
-                GROUP BY job_id
-            """
-            context.log.info(f"Querying INFORMATION_SCHEMA.JOBS for bytes billed: {cost_query}")
-            query_result = bigquery_client.query(cost_query)
+    marker_asset_key = marker_asset_key_for_job(context.job_def)
+    run_results_json = dbt_cli_invocation.get_artifact("run_results.json")
+    invocation_id = run_results_json["metadata"]["invocation_id"]
+
+    # backcompat-proof in case the invocation does not have an instantiated adapter on it
+    adapter: Optional["BaseAdapter"] = getattr(dbt_cli_invocation, "adapter", None)
+    if not adapter:
+        if version.parse(dagster_dbt_version) < version.parse(MIN_DAGSTER_DBT_VERSION):
+            upgrade_message = f" Extracting cost information requires dagster_dbt>={MIN_DAGSTER_DBT_VERSION} (found {dagster_dbt_version}). "
+        else:
+            upgrade_message = ""
+
+        context.log.error(
+            "Could not find a BigQuery adapter on the dbt CLI invocation. Skipping cost analysis."
+            + upgrade_message
+        )
+        return
 
-            # overwrite cost_by_asset that is computed from the metadata
-            cost_by_asset = defaultdict(list)
+    cost_by_asset = defaultdict(list)
+    try:
+        with adapter.connection_named("dagster_insights:bigquery_cost"):
+            client: "bigquery.Client" = adapter.connections.get_thread_connection().handle
+            dataset = client.get_dataset(adapter.config.credentials.schema)
+            region = f"region-{dataset.location.lower()}" if dataset.location else DEFAULT_BQ_REGION
+            query_result = client.query(
+                rf"""
+                    SELECT
+                    job_id,
+                    regexp_extract(query, r"{OPAQUE_ID_SQL_SIGIL}\[\[\[(.*?):{invocation_id}\]\]\]") as unique_id,
+                    total_bytes_billed AS bytes_billed,
+                    total_slot_ms AS slots_ms
+                    FROM `{dataset.project}`.`{region}`.INFORMATION_SCHEMA.JOBS
+                    WHERE query like '%{invocation_id}%'
+                """
+            )
             for row in query_result:
-                asset_key, partition = asset_info_by_job_id.get(
-                    row.job_id, (marker_asset_key, None)
+                if not row.unique_id:
+                    continue
+                asset_key, partition = asset_info_by_unique_id.get(
+                    row.unique_id, (marker_asset_key, None)
                 )
                 if row.bytes_billed or row.slots_ms:
                     cost_info = BigQueryCostInfo(
                         asset_key, partition, row.job_id, row.bytes_billed, row.slots_ms
                     )
                     cost_by_asset[cost_info.asset_partition_key].append(cost_info)
-        except:
-            context.log.exception("Could not query information_schema.jobs for bytes billed")
+    except:
+        context.log.exception("Could not query information_schema for BigQuery cost information")
+        return
 
     for cost_info_list in cost_by_asset.values():
         bytes_billed = sum(item.bytes_billed for item in cost_info_list)
         slots_ms = sum(item.slots_ms for item in cost_info_list)
         job_ids = [item.job_id for item in cost_info_list]
         asset_key = cost_info_list[0].asset_key
         partition = cost_info_list[0].partition
```

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/bigquery/insights_bigquery_resource.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/insights_utils.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/insights_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Tuple, Union
 
 import dagster._check as check
 from dagster import (
+    AssetCheckResult,
     AssetExecutionContext,
     AssetKey,
     AssetMaterialization,
     AssetObservation,
     DagsterInvariantViolationError,
     OpExecutionContext,
     Output,
@@ -38,18 +39,19 @@
     return asset_info.key
 
 
 def extract_asset_info_from_event(context, dagster_event, record_observation_usage):
     if isinstance(dagster_event, AssetMaterialization):
         return dagster_event.asset_key, dagster_event.partition
 
-    if isinstance(dagster_event, AssetObservation) and record_observation_usage:
-        return dagster_event.asset_key, dagster_event.partition
+    if isinstance(dagster_event, (AssetCheckResult, AssetObservation)) and record_observation_usage:
+        partition = dagster_event.partition if isinstance(dagster_event, AssetObservation) else None
+        return dagster_event.asset_key, partition
 
-    if isinstance(dagster_event, AssetObservation):
+    if isinstance(dagster_event, (AssetCheckResult, AssetObservation)):
         return None, None
 
     if isinstance(dagster_event, Output):
         asset_key = get_asset_key_for_output(context, dagster_event.output_name)
         partition_key = None
         if asset_key and context._step_execution_context.has_asset_partitions_for_output(  # noqa: SLF001
             dagster_event.output_name
```

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/metrics_utils.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/metrics_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 def get_post_request_params(
     instance: DagsterInstance,
 ) -> Tuple[requests.Session, str, Dict[str, str], int, Optional[Dict[str, str]]]:
     if not isinstance(instance, DagsterCloudAgentInstance):
         raise RuntimeError("This asset only functions in a running Dagster Cloud instance")
 
     return (
-        instance.rest_requests_session,
+        instance.requests_managed_retries_session,
         instance.dagster_cloud_gen_insights_url_url,
         instance.dagster_cloud_api_headers(DagsterCloudInstanceScope.DEPLOYMENT),
         instance.dagster_cloud_api_timeout,
         instance.dagster_cloud_api_proxies,
     )
```

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/query.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/query.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/dagster_snowflake_insights.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/dbt_wrapper.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/dbt_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
                 )
 
     if dagster_events is None:
         dagster_events = dbt_cli_invocation.stream()
 
     asset_and_partition_key_to_unique_id: List[Tuple[AssetKey, Optional[str], Any]] = []
     for dagster_event in dagster_events:
-        if isinstance(dagster_event, (AssetMaterialization, AssetObservation, Output)):
+        if isinstance(
+            dagster_event, (AssetMaterialization, AssetObservation, Output, AssetCheckResult)
+        ):
             unique_id = dagster_event.metadata["unique_id"].value
             asset_key, partition = extract_asset_info_from_event(
                 context, dagster_event, record_observation_usage
             )
             if not asset_key:
                 asset_key = marker_asset_key_for_job(context.job_def)
```

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/definitions.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/insights_snowflake_resource.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-insights-0.0.19/dagster_insights_prerelease/dagster_insights_patched/snowflake/snowflake_utils.py` & `dagster-insights-0.0.20/dagster_insights_prerelease/dagster_insights_patched/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

