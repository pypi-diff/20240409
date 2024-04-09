# Comparing `tmp/best-ec2-1.1.2.tar.gz` & `tmp/best-ec2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best-ec2-1.1.2.tar", last modified: Mon Apr  8 16:10:22 2024, max compression
+gzip compressed data, was "best-ec2-1.1.3.tar", last modified: Tue Apr  9 19:52:03 2024, max compression
```

## Comparing `best-ec2-1.1.2.tar` & `best-ec2-1.1.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.073442 best-ec2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)    16771 2024-04-08 16:10:22.073442 best-ec2-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16216 2024-04-08 16:09:55.000000 best-ec2-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:09:55.000000 best-ec2-1.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-08 16:10:22.073442 best-ec2-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-08 16:09:55.000000 best-ec2-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.065442 best-ec2-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.069442 best-ec2-1.1.2/src/best_ec2/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/aws_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/best_ec2.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/best_ec2_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6423 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/spot_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/src/best_ec2/strategies/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3653 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/abstract_sort_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_on_demand_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_spot_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/strategies/sort_strategy_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4763 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/types.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-08 16:09:55.000000 best-ec2-1.1.2/src/best_ec2/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/src/best_ec2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16771 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      775 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-08 16:10:22.000000 best-ec2-1.1.2/src/best_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:10:22.072442 best-ec2-1.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12201 2024-04-08 16:09:55.000000 best-ec2-1.1.2/tests/test_int.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:52:03.904629 best-ec2-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)    16771 2024-04-09 19:52:03.904629 best-ec2-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16216 2024-04-09 19:51:33.000000 best-ec2-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 19:51:33.000000 best-ec2-1.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-09 19:52:03.904629 best-ec2-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-09 19:51:33.000000 best-ec2-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:52:03.897629 best-ec2-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:52:03.901629 best-ec2-1.1.3/src/best_ec2/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/aws_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/best_ec2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8710 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/best_ec2_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/enrichers.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4332 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/spot_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:52:03.903629 best-ec2-1.1.3/src/best_ec2/strategies/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/strategies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3249 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/strategies/abstract_sort_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/strategies/sort_on_demand_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3973 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/strategies/sort_spot_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/strategies/sort_strategy_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-09 19:51:33.000000 best-ec2-1.1.3/src/best_ec2/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:52:03.904629 best-ec2-1.1.3/src/best_ec2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16771 2024-04-09 19:52:03.000000 best-ec2-1.1.3/src/best_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      783 2024-04-09 19:52:03.000000 best-ec2-1.1.3/src/best_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 19:52:03.000000 best-ec2-1.1.3/src/best_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-09 19:52:03.000000 best-ec2-1.1.3/src/best_ec2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-09 19:52:03.000000 best-ec2-1.1.3/src/best_ec2.egg-info/top_level.txt
```

### Comparing `best-ec2-1.1.2/PKG-INFO` & `best-ec2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best-ec2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
 Home-page: https://gitlab.com/aliaksei-kankou/best-ec2/python-package
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: boto3>=1.29.2
```

### Comparing `best-ec2-1.1.2/README.md` & `best-ec2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.2/setup.cfg` & `best-ec2-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = best-ec2
-version = 1.1.2
+version = 1.1.3
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/aliaksei-kankou/best-ec2/python-package
```

### Comparing `best-ec2-1.1.2/src/best_ec2/aws_utils.py` & `best-ec2-1.1.3/src/best_ec2/aws_utils.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.2/src/best_ec2/best_ec2.py` & `best-ec2-1.1.3/src/best_ec2/best_ec2.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.2/src/best_ec2/best_ec2_impl.py` & `best-ec2-1.1.3/src/best_ec2/best_ec2_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     UsageClass,
     Architecture,
     InstanceTypeInfo,
     FilterEntry,
     PriceDetails,
     SpotPriceCacheKey,
     RequestConfig,
+    StrategyConfig,
 )
 from .constants import (
     DEFAULT_RESULT_CACHE_TTL_IN_MINUTES,
     DEFAULT_INSTANCE_TYPE_CACHE_TTL_IN_MINUTES,
     DEFAULT_ON_DEMAND_PRICE_CACHE_TTL_IN_MINUTES,
     DEFAULT_SPOT_PRICE_CACHE_TTL_IN_MINUTES,
     DEFAULT_SPOT_CONCURRENCY,
@@ -31,14 +32,15 @@
     DEFAULT_VCPU,
     DEFAULT_MEMORY_GB,
 )
 from .strategies.sort_strategy_factory import SortStrategyFactory
 from .cache import Cache
 from .validators import Validator
 from .filters import FilterChain
+from .enrichers import EnricherChain
 from .utils import remove_none_values
 
 
 class BestEc2Impl:
     def __init__(
         self, options: Optional[BestEc2Options] = None, logger: Optional[Logger] = None
     ):
@@ -94,16 +96,15 @@
         config: Optional[RequestConfig] = None,
     ) -> InstanceTypeResponse:
         request = self._prepare_request_with_defaults(remove_none_values(request))
         ec2_client = self._create_ec2_client(request, config)
 
         Validator.instance_type_request(request)
 
-        cached_result = self._check_cache(request)
-        if cached_result:
+        if cached_result := self._check_cache(request):
             return cached_result
 
         with self._log_runtime("get types"):
             instances = self._describe_and_cache_instance_types(
                 ec2_client, request["region"]
             )
         filtered_instances = self._apply_filters_to_instances(instances, request)
@@ -165,42 +166,49 @@
 
     def _apply_filters_to_instances(
         self, instances: List[InstanceTypeInfo], request: InstanceTypeRequest
     ) -> List[InstanceTypeInfo]:
         self._logger.debug(
             f"Number of instance types before filtering: {len(instances)}"
         )
-        filtered_instances = FilterChain(request.get("region")).execute(
-            instances, request
-        )
+
+        instances = EnricherChain(request.get("region")).apply(instances, request)
+
+        filtered_instances = [
+            instance for instance in instances if FilterChain().apply(instance, request)
+        ]
+
         self._logger.debug(
             f"Number of instance types after filtering: {len(filtered_instances)}"
         )
         return filtered_instances
 
     def _sort_instances_by_strategy(
         self,
         instances: List[InstanceTypeInfo],
         request: InstanceTypeRequest,
         ec2_client: BaseClient,
     ) -> InstanceTypeResponse:
         config = Config(max_pool_connections=self._spot_price_history_concurrency)
         # Use the us-east-1 region for the AWS Pricing API as it is the only supported region for this service
         pricing_client = boto3.client("pricing", region_name="us-east-1", config=config)
-        strategy = SortStrategyFactory.create(
-            request["usage_class"],
-            request.get("region"),
-            pricing_client,
-            ec2_client,
-            self._logger,
-            self._spot_price_history_concurrency,
+        cache = (
             self._on_demand_price_cache
             if request["usage_class"] == UsageClass.ON_DEMAND.value
-            else self._spot_price_cache,
+            else self._spot_price_cache
+        )
+        strategy_config = StrategyConfig(
+            region=request.get("region"),
+            pricing_client=pricing_client,
+            ec2_client=ec2_client,
+            logger=self._logger,
+            concurrency_level=self._spot_price_history_concurrency,
+            cache=cache,
         )
+        strategy = SortStrategyFactory.create(request["usage_class"], strategy_config)
         return strategy.sort(
             instances,
             request["product_description"],
             request.get("availability_zones"),
             request.get("final_spot_price_strategy", "min"),
         )
```

### Comparing `best-ec2-1.1.2/src/best_ec2/cache.py` & `best-ec2-1.1.3/src/best_ec2/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,12 +30,12 @@
     def set(self, key: K, value: V) -> None:
         hash_digest = self._get_unique_string(key)
         self._cache[hash_digest] = CacheEntry(result=value, datetime=datetime.now())
 
     def _get_unique_string(self, key: K) -> str:
         if isinstance(key, str):
             return key
-        hash_object = hashlib.md5(json.dumps(key, sort_keys=True).encode())
+        hash_object = hashlib.sha256(json.dumps(key, sort_keys=True).encode())
         return hash_object.hexdigest()
 
     def _is_valid(self, cache_datetime: datetime) -> bool:
         return (datetime.now() - cache_datetime) < timedelta(minutes=self._ttl_minutes)
```

### Comparing `best-ec2-1.1.2/src/best_ec2/constants.py` & `best-ec2-1.1.3/src/best_ec2/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,9 @@
     "SUSE Linux": "SUSE",
     "Windows": "Windows",
     "Linux/UNIX (Amazon VPC)": "Linux",
     "Red Hat Enterprise Linux (Amazon VPC)": "RHEL",
     "SUSE Linux (Amazon VPC)": "SUSE",
     "Windows (Amazon VPC)": "Windows",
 }
+
+MEBIBYTES_IN_GIBIBYTE = 1024
```

### Comparing `best-ec2-1.1.2/src/best_ec2/exceptions.py` & `best-ec2-1.1.3/src/best_ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.2/src/best_ec2/strategies/abstract_sort_strategy.py` & `best-ec2-1.1.3/src/best_ec2/strategies/abstract_sort_strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,36 @@
 from abc import ABC, abstractmethod
 import operator
-from logging import Logger
 from typing import Dict, List, Optional, Union
 
-from botocore.client import BaseClient
-
 from ..types import (
     FinalSpotPriceStrategy,
     InstanceTypeInfo,
     InstanceTypeResponse,
     ProductDescription,
     InstanceType,
     PriceDetails,
+    StrategyConfig,
 )
-from ..cache import Cache
 
 
 class AbstractSortStrategy(ABC):
-    def __init__(
-        self,
-        region: str,
-        pricing_client: BaseClient,
-        ec2_client: BaseClient,
-        logger: Logger,
-        concurrency_level: int,
-        cache: Cache,
-    ):
-        self._logger = logger
-        self._region = region
-        self._pricing_client = pricing_client
-        self._ec2_client = ec2_client
-        self._concurrency_level = concurrency_level
-        self._cache = cache
+    def __init__(self, config: StrategyConfig):
+        self._config = config
 
     def sort(
         self,
         instance_types_info: List[InstanceTypeInfo],
-        product_desc: ProductDescription,
+        product_description: ProductDescription,
         availability_zones: List[str],
         pricing_strategy: Optional[FinalSpotPriceStrategy],
     ) -> InstanceTypeResponse:
         price_details_by_instance = self._get_price(
             instance_types_info,
-            product_desc,
+            product_description,
             availability_zones,
             pricing_strategy,
         )
 
         sorted_instances = []
         for instance_info in instance_types_info:
             instance_entry = self._build_instance_entry(
@@ -74,15 +58,15 @@
         instance_info: InstanceTypeInfo,
         prices: Dict[str, PriceDetails],
     ) -> Union[InstanceType, None]:
         instance_type_name = instance_info["InstanceType"]
         price_info = prices.get(instance_type_name)
 
         if price_info is None:
-            self._logger.debug(
+            self._config.logger.debug(
                 f"The price for the {instance_type_name} instance type not found"
             )
             return None
 
         entry: InstanceType = {
             "instance_type": instance_type_name,
             "vcpu": instance_info["VCpuInfo"]["DefaultVCpus"],
```

### Comparing `best-ec2-1.1.2/src/best_ec2/strategies/sort_on_demand_strategy.py` & `best-ec2-1.1.3/src/best_ec2/strategies/sort_on_demand_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 import json
 from typing import Dict, List, Optional, Tuple
-from logging import Logger
 
-from botocore.client import BaseClient
-
-from ..cache import Cache
 from ..constants import OS_PRODUCT_DESCRIPTION_MAP, REGIONS
 from ..types import (
     FinalSpotPriceStrategy,
     InstanceTypeInfo,
     ProductDescription,
     PriceDetails,
     FilterEntry,
 )
 from .abstract_sort_strategy import AbstractSortStrategy
 
 
 class SortOnDemandStrategy(AbstractSortStrategy):
     """Sort strategy for On-Demand EC2 instances."""
 
-    def __init__(
-        self,
-        region: str,
-        pricing_client: BaseClient,
-        ec2_client: BaseClient,
-        logger: Logger,
-        concurrency_level: int,
-        cache: Optional[Cache] = None,
-    ):
-        super().__init__(
-            region,
-            pricing_client,
-            ec2_client,
-            logger,
-            concurrency_level,
-            cache,
-        )
-
     def _get_price(
         self,
         filtered_instances: List[InstanceTypeInfo],
         product_description: ProductDescription,
         availability_zones: Optional[List[str]],
         final_spot_price_strategy: FinalSpotPriceStrategy,
     ) -> Dict[str, PriceDetails]:
@@ -51,15 +29,15 @@
     @staticmethod
     def _map_product_description_to_os(product_description: ProductDescription) -> str:
         return OS_PRODUCT_DESCRIPTION_MAP[product_description]
 
     def _get_on_demand_instance_price(
         self, filters: List[FilterEntry]
     ) -> Dict[str, PriceDetails]:
-        paginator = self._pricing_client.get_paginator("get_products")
+        paginator = self._config.pricing_client.get_paginator("get_products")
         records = {}
 
         for page in paginator.paginate(Filters=filters, ServiceCode="AmazonEC2"):
             price_list = page.get("PriceList", [])
 
             for price in price_list:
                 instance_type, instance_price = self._parse_price_details(price)
@@ -73,15 +51,19 @@
             {"Type": "TERM_MATCH", "Field": "preInstalledSw", "Value": "NA"},
             {
                 "Type": "TERM_MATCH",
                 "Field": "productFamily",
                 "Value": "Compute Instance",
             },
             {"Type": "TERM_MATCH", "Field": "termType", "Value": "OnDemand"},
-            {"Type": "TERM_MATCH", "Field": "location", "Value": REGIONS[self._region]},
+            {
+                "Type": "TERM_MATCH",
+                "Field": "location",
+                "Value": REGIONS[self._config.region],
+            },
             {
                 "Type": "TERM_MATCH",
                 "Field": "licenseModel",
                 "Value": "No License required",
             },
             {"Type": "TERM_MATCH", "Field": "tenancy", "Value": "Shared"},
             {"Type": "TERM_MATCH", "Field": "capacitystatus", "Value": "Used"},
@@ -93,21 +75,21 @@
         ]
 
     def _get_and_cache_on_demand_instance_price(
         self, filters: List[FilterEntry]
     ) -> Dict[str, PriceDetails]:
         cache_key = filters
 
-        if cached_price_details := self._cache.get(cache_key):
-            self._logger.info("On-demand price cache hit")
+        if cached_price_details := self._config.cache.get(cache_key):
+            self._config.logger.info("On-demand price cache hit")
             return cached_price_details
 
-        self._logger.info("On-demand price cache miss")
+        self._config.logger.info("On-demand price cache miss")
         price_details = self._get_on_demand_instance_price(filters)
-        self._cache.set(cache_key, price_details)
+        self._config.cache.set(cache_key, price_details)
         return price_details
 
     @staticmethod
     def _parse_price_details(price: str) -> Tuple[str, float]:
         details = json.loads(price)
         price_dimensions = next(iter(details["terms"]["OnDemand"].values()))[
             "priceDimensions"
```

### Comparing `best-ec2-1.1.2/src/best_ec2/strategies/sort_spot_strategy.py` & `best-ec2-1.1.3/src/best_ec2/strategies/sort_spot_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-from logging import Logger
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Dict, List, Optional
 
-from botocore.client import BaseClient
-
 from ..types import (
     FinalSpotPriceStrategy,
     InstanceTypeInfo,
     ProductDescription,
     PriceDetails,
     TypePriceDetails,
+    StrategyConfig,
 )
 from ..aws_utils import AwsUtils
 from ..exceptions import InvalidStrategyError
-from ..cache import Cache
 from .abstract_sort_strategy import AbstractSortStrategy
 
 
 class SortSpotStrategy(AbstractSortStrategy):
-    def __init__(
-        self,
-        region: str,
-        pricing_client: BaseClient,
-        ec2_client: BaseClient,
-        logger: Logger,
-        spot_price_history_concurrency: int,
-        cache: Cache,
-    ):
-        super().__init__(
-            region,
-            pricing_client,
-            ec2_client,
-            logger,
-            spot_price_history_concurrency,
-            cache,
-        )
-        self._aws_utils = AwsUtils(ec2_client)
+    def __init__(self, config: StrategyConfig):
+        super().__init__(config)
+        self._aws_utils = AwsUtils(config.ec2_client)
 
     def _get_price(
         self,
         filtered_instances: List[InstanceTypeInfo],
         product_description: ProductDescription,
         availability_zones: Optional[List[str]],
         final_spot_price_strategy: FinalSpotPriceStrategy,
@@ -52,20 +34,20 @@
         cache_key = {
             "filtered_instances": filtered_instances,
             "product_description": product_description,
             "availability_zones": availability_zones,
             "final_spot_price_strategy": final_spot_price_strategy,
         }
 
-        if cached_price_details := self._cache.get(cache_key):
-            self._logger.info("Spot price cache hit")
+        if cached_price_details := self._config.cache.get(cache_key):
+            self._config.logger.info("Spot price cache hit")
             return cached_price_details
-        self._logger.info("Spot price cache miss")
+        self._config.logger.info("Spot price cache miss")
 
-        with ThreadPoolExecutor(max_workers=self._concurrency_level) as executor:
+        with ThreadPoolExecutor(max_workers=self._config.concurrency_level) as executor:
             futures = [
                 executor.submit(
                     self._get_spot_instance_price,
                     ec2_instance,
                     product_description,
                     availability_zones,
                     final_spot_price_strategy,
@@ -75,15 +57,15 @@
 
             ec2_prices = {
                 future.result()["instance_type"]: future.result()["price_details"]
                 for future in as_completed(futures)
                 if future.result()
             }
 
-        self._cache.set(cache_key, ec2_prices)
+        self._config.cache.set(cache_key, ec2_prices)
         return ec2_prices
 
     def _get_spot_instance_price(
         self,
         ec2_instance: InstanceTypeInfo,
         product_description: ProductDescription,
         availability_zones: List[str],
@@ -91,29 +73,31 @@
     ) -> Optional[TypePriceDetails]:
         instance_type = ec2_instance["InstanceType"]
         filters = [{"Name": "product-description", "Values": [product_description]}]
 
         if availability_zones:
             filters.append({"Name": "availability-zone", "Values": availability_zones})
 
-        response = self._ec2_client.describe_spot_price_history(
+        response = self._config.ec2_client.describe_spot_price_history(
             InstanceTypes=[instance_type], Filters=filters
         )
 
         history_events = response["SpotPriceHistory"]
         az_price: Dict[str, float] = {
             event["AvailabilityZone"]: float(event["SpotPrice"])
             for event in history_events
             if event["AvailabilityZone"] in availability_zones
         }
 
         prices = list(az_price.values())
 
         if len(prices) == 0:
-            self._logger.info(f"Spot price for the {instance_type} is not available")
+            self._config.logger.info(
+                f"Spot price for the {instance_type} is not available"
+            )
             return None
 
         spot_price = self._calculate_spot_price(prices, strategy)
 
         return {
             "instance_type": instance_type,
             "price_details": {"price": spot_price, "az_price": az_price},
@@ -121,13 +105,13 @@
 
     @staticmethod
     def _calculate_spot_price(
         prices: List[float], strategy: FinalSpotPriceStrategy
     ) -> float:
         if strategy == "average":
             return sum(prices) / len(prices)
-        elif strategy == "max":
+        if strategy == "max":
             return max(prices)
-        elif strategy == "min":
+        if strategy == "min":
             return min(prices)
-        else:
-            raise InvalidStrategyError(strategy)
+
+        raise InvalidStrategyError(strategy)
```

### Comparing `best-ec2-1.1.2/src/best_ec2/types.py` & `best-ec2-1.1.3/src/best_ec2/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from typing import Optional, Dict, TypeVar, TypedDict, List, Union
+from logging import Logger
 
 from botocore.client import BaseClient
 from botocore.config import Config
 
+from .cache import Cache
+
 
 class UsageClass(Enum):
     SPOT = "spot"
     ON_DEMAND = "on-demand"
 
 
 class Architecture(Enum):
@@ -47,16 +51,21 @@
     Type: str
 
 
 class InstanceStorageInfo(TypedDict):
     Disks: List[DiskInfo]
 
 
+class Gpu(TypedDict):
+    Count: int
+
+
 class GpuInfo(TypedDict):
-    total_gpu_memory: int
+    Gpus: list[Gpu]
+    TotalGpuMemoryInMiB: int
 
 
 class _InstanceTypeRequired(TypedDict):
     price: float
     instance_type: str
     vcpu: int
     memory_gb: int
@@ -185,7 +194,17 @@
 
 
 class SpotPriceCacheKey(TypedDict):
     filtered_instances: List[InstanceTypeInfo]
     product_description: ProductDescription
     availability_zones: Optional[List[str]]
     final_spot_price_strategy: FinalSpotPriceStrategy
+
+
+@dataclass
+class StrategyConfig:
+    region: str
+    pricing_client: BaseClient
+    ec2_client: BaseClient
+    logger: Logger
+    concurrency_level: int
+    cache: Optional[Cache] = field(default=None)
```

### Comparing `best-ec2-1.1.2/src/best_ec2/validators.py` & `best-ec2-1.1.3/src/best_ec2/validators.py`

 * *Files identical despite different names*

### Comparing `best-ec2-1.1.2/src/best_ec2.egg-info/PKG-INFO` & `best-ec2-1.1.3/src/best_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best-ec2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Best EC2, the smart solution designed to optimize your Amazon EC2 instance type selection process. The app simplifies the challenge of choosing the optimal EC2 instance type that matches your specific requirements, balancing performance, cost, and computing needs.
 Home-page: https://gitlab.com/aliaksei-kankou/best-ec2/python-package
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: boto3>=1.29.2
```

### Comparing `best-ec2-1.1.2/src/best_ec2.egg-info/SOURCES.txt` & `best-ec2-1.1.3/src/best_ec2.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 src/best_ec2/__init__.py
 src/best_ec2/aws_utils.py
 src/best_ec2/best_ec2.py
 src/best_ec2/best_ec2_impl.py
 src/best_ec2/cache.py
 src/best_ec2/constants.py
+src/best_ec2/enrichers.py
 src/best_ec2/exceptions.py
 src/best_ec2/filters.py
 src/best_ec2/spot_utils.py
 src/best_ec2/types.py
 src/best_ec2/utils.py
 src/best_ec2/validators.py
 src/best_ec2.egg-info/PKG-INFO
@@ -19,9 +20,8 @@
 src/best_ec2.egg-info/dependency_links.txt
 src/best_ec2.egg-info/requires.txt
 src/best_ec2.egg-info/top_level.txt
 src/best_ec2/strategies/__init__.py
 src/best_ec2/strategies/abstract_sort_strategy.py
 src/best_ec2/strategies/sort_on_demand_strategy.py
 src/best_ec2/strategies/sort_spot_strategy.py
-src/best_ec2/strategies/sort_strategy_factory.py
-tests/test_int.py
+src/best_ec2/strategies/sort_strategy_factory.py
```

