# Comparing `tmp/phc-ingestion-0.8.0.tar.gz` & `tmp/phc-ingestion-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.8.0.tar", last modified: Sun Apr  7 13:29:20 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.1.tar", last modified: Tue Apr  9 10:46:09 2024, max compression
```

## Comparing `phc-ingestion-0.8.0.tar` & `phc-ingestion-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       16 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      507 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      747 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0    12312 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/ihc.py
--rw-r--r--   0        0        0      555 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4706 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/json.py
--rw-r--r--   0        0        0     9497 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     2051 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/specimen_details.py
--rw-r--r--   0        0        0     4363 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1027 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tmb.py
--rw-r--r--   0        0        0     1595 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3298 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5451 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0       68 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1010 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      770 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9497 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4363 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1027 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3298 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5451 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0       68 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1010 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.1/PKG-INFO
```

### Comparing `phc-ingestion-0.8.0/ingestion/caris/process.py` & `phc-ingestion-0.8.1/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.1/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.1/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.1/ingestion/caris/util/hla.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import TypedDict, Literal
 
 
 class HlaResult(TypedDict):
     gene: Literal["HLA-A", "HLA-B", "HLA-C"]
     interpretation: str
-    mhClass: Literal["I"]
+    mhClass: Literal["I", "gDNA"]
     genotype: str
 
 
 def extract_hla_result_from_test_result(test_result) -> HlaResult:
     gene = test_result.get("gene", "")
     if gene not in ["HLA-A", "HLA-B", "HLA-C"]:
         raise RuntimeError(f"Unknown HLA gene detected: {gene}")
     interpretation = test_result.get("result_group", "")
     mh_class = test_result.get("mhClass", "")
-    if mh_class != "I":
+    if mh_class not in ["I", "gDNA"]:
         raise RuntimeError(f"Unknown MHC class detected: {mh_class}")
+
     genotype = test_result.get("genotype", "")
 
     return HlaResult(gene=gene, interpretation=interpretation, mhClass=mh_class, genotype=genotype)
```

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/ihc.py` & `phc-ingestion-0.8.1/ingestion/caris/util/ihc.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.1/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/json.py` & `phc-ingestion-0.8.1/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/metadata.py` & `phc-ingestion-0.8.1/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/specimen_details.py` & `phc-ingestion-0.8.1/ingestion/caris/util/specimen_details.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.1/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/tmb.py` & `phc-ingestion-0.8.1/ingestion/caris/util/tmb.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.1/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.1/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/foundation/process.py` & `phc-ingestion-0.8.1/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.1/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.1/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.1/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.1/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/generic/process.py` & `phc-ingestion-0.8.1/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/generic/utils.py` & `phc-ingestion-0.8.1/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/process.py` & `phc-ingestion-0.8.1/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.1/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.1/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.1/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.1/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.8.1/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.1/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.1/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.1/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.1/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.1/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.1/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.0/pyproject.toml` & `phc-ingestion-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.8.0"
+version = "0.8.1"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

