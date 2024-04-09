# Comparing `tmp/pgscatalog_core-0.1.0.tar.gz` & `tmp/pgscatalog_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_core-0.1.0.tar", max compression
+gzip compressed data, was "pgscatalog_core-0.1.1.tar", max compression
```

## Comparing `pgscatalog_core-0.1.0.tar` & `pgscatalog_core-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1907 2024-03-22 14:29:51.608626 pgscatalog_core-0.1.0/README.md
--rw-r--r--   0        0        0     1199 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1553 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/cli/__init__.py
--rw-r--r--   0        0        0     2308 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/cli/_combine.py
--rwxr-xr-x   0        0        0     6162 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/cli/combine_cli.py
--rwxr-xr-x   0        0        0     4907 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/cli/download_cli.py
--rw-r--r--   0        0        0     3054 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/cli/relabel_cli.py
--rw-r--r--   0        0        0     1485 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/__init__.py
--rw-r--r--   0        0        0      910 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_config.py
--rw-r--r--   0        0        0     5499 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_download.py
--rw-r--r--   0        0        0    13833 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_normalise.py
--rw-r--r--   0        0        0     2876 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_read.py
--rw-r--r--   0        0        0     5581 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_relabel.py
--rw-r--r--   0        0        0    13836 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/catalogapi.py
--rw-r--r--   0        0        0     1473 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/genomebuild.py
--rw-r--r--   0        0        0     4620 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/pgsexceptions.py
--rw-r--r--   0        0        0    33063 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/scorefiles.py
--rw-r--r--   0        0        0     7546 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/scorevariant.py
--rw-r--r--   0        0        0     6939 2024-03-22 14:29:51.612626 pgscatalog_core-0.1.0/src/pgscatalog/core/lib/targetvariants.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pgscatalog_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1907 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/README.md
+-rw-r--r--   0        0        0     1199 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1553 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/__init__.py
+-rw-r--r--   0        0        0     1946 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/_combine.py
+-rwxr-xr-x   0        0        0     5858 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/combine_cli.py
+-rwxr-xr-x   0        0        0     4907 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/download_cli.py
+-rw-r--r--   0        0        0     3054 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/relabel_cli.py
+-rw-r--r--   0        0        0     1485 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_config.py
+-rw-r--r--   0        0        0     5499 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_download.py
+-rw-r--r--   0        0        0    14151 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_normalise.py
+-rw-r--r--   0        0        0     2876 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_read.py
+-rw-r--r--   0        0        0     5581 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_relabel.py
+-rw-r--r--   0        0        0    13836 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/catalogapi.py
+-rw-r--r--   0        0        0     1585 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/genomebuild.py
+-rw-r--r--   0        0        0     4620 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/pgsexceptions.py
+-rw-r--r--   0        0        0    33063 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorefiles.py
+-rw-r--r--   0        0        0     7546 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorevariant.py
+-rw-r--r--   0        0        0     7538 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/targetvariants.py
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pgscatalog_core-0.1.1/PKG-INFO
```

### Comparing `pgscatalog_core-0.1.0/README.md` & `pgscatalog_core-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/pyproject.toml` & `pgscatalog_core-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgscatalog.core"
-version = "0.1.0"
+version = "0.1.1"
 description = "Core tools for working with polygenic scores (PGS) and the PGS Catalog"
 license = "Apache-2.0"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 readme = "README.md"
 packages = [
     { include = "pgscatalog", from = "src" },
 ]
```

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/__init__.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/cli/_combine.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/_combine.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,14 @@
 import os
 
 from ..lib.scorevariant import ScoreVariant
 
 logger = logging.getLogger(__name__)
 
 
-def normalise(
-    scoring_file, liftover=False, drop_missing=False, chain_dir=None, target_build=None
-):
-    """Normalise all rows in a scoring file"""
-    return list(
-        scoring_file.normalise(
-            liftover=liftover,
-            drop_missing=drop_missing,
-            chain_dir=chain_dir,
-            target_build=target_build,
-        )
-    )
-
-
 def get_variant_log(batch):
     # these statistics can only be generated while iterating through variants
     n_variants = collections.Counter("n_variants" for item in batch)
     hm_source = collections.Counter(getattr(item, "hm_source") for item in batch)
     return n_variants + hm_source
```

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/cli/combine_cli.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/combine_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import argparse
-import concurrent.futures
 import json
 import logging
 import pathlib
 import sys
 import textwrap
 
 from tqdm import tqdm
-from ..lib import GenomeBuild, ScoringFile
+from pgscatalog.core import GenomeBuild, ScoringFile
 
-from ._combine import normalise, get_variant_log, TextFileWriter
+from pgscatalog.core.cli._combine import get_variant_log, TextFileWriter
 
 logger = logging.getLogger(__name__)
 
 
 def run():
     args = parse_args()
 
@@ -33,15 +32,15 @@
             logger.debug("Compressing output with gzip")
             compress_output = True
         case _:
             logger.debug("Not compressing output")
             compress_output = False
 
     paths = list(set(args.scorefiles))  # unique paths only
-    scoring_files = [ScoringFile(x) for x in paths]
+    scoring_files = sorted([ScoringFile(x) for x in paths], key=lambda x: x.pgs_id)
     target_build = GenomeBuild.from_string(args.target_build)
 
     for x in scoring_files:
         if x.genome_build != target_build and not args.liftover:
             raise ValueError(
                 f"Can't combine scoring file with genome build {x.genome_build!r} when {target_build=} without --liftover"
             )
@@ -58,34 +57,23 @@
             "liftover": True,
             "chain_dir": chain_dir,
             "target_build": target_build,
         }
     else:
         liftover_kwargs = {"liftover": False}
 
-    with concurrent.futures.ThreadPoolExecutor() as executor:
-        futures = []
-        for scorefile in scoring_files:
-            logger.info(f"Submitting {scorefile!r} for execution")
-            futures.append(
-                executor.submit(
-                    normalise,
-                    scorefile,
-                    drop_missing=args.drop_missing,
-                    **liftover_kwargs,
-                )
-            )
-        # TODO: do this I/O asynchronously
-        for future in tqdm(
-            concurrent.futures.as_completed(futures), total=len(futures)
-        ):
-            writer = TextFileWriter(compress=compress_output, filename=out_path)
-            normalised_score = future.result()
-            writer.write(normalised_score)
-            variant_log.append(get_variant_log(normalised_score))
+    for scorefile in tqdm(scoring_files, total=len(scoring_files)):
+        logger.info(f"Processing {scorefile.pgs_id}")
+        normalised_score = list(
+            scorefile.normalise(drop_missing=args.drop_missing, **liftover_kwargs)
+        )
+        # TODO: go back to concurrent execution + write to multiple files
+        writer = TextFileWriter(compress=compress_output, filename=out_path)
+        writer.write(normalised_score)
+        variant_log.append(get_variant_log(normalised_score))
 
     score_log = []
     for sf, log in zip(scoring_files, variant_log, strict=True):
         score_log.append(sf.get_log(variant_log=log))
 
     log_out_path = pathlib.Path(args.outfile).parent / args.logfile
     with open(log_out_path, "w") as f:
```

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/cli/download_cli.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/cli/relabel_cli.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/relabel_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/__init__.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_config.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_config.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_download.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_download.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_normalise.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_normalise.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,19 +183,23 @@
     >>> list(assign_effect_type([variant])) # doctest: +ELLIPSIS
     [ScoreVariant(...,effect_type=EffectType.DOMINANT,...)]
 
     is_recessive and is_dominant fields are parsed from strings to bools during __init__.
     """
     for variant in variants:
         match (variant.is_recessive, variant.is_dominant):
-            case (None, None) | (False, False):
-                pass  # default value is additive, pass to break match and yield
-            case (False, True):
+            case (None, None) | (False, False) | (None, False) | (False, None):
+                # none is OK because is_recessive or is_dominant column may be missing
+                # default value is already set to additive, so just yield the variant
+                pass
+            case (False, True) | (None, True):
+                # none is OK because is_recessive column may be missing
                 variant.effect_type = EffectType.DOMINANT
-            case (True, False):
+            case (True, False) | (True, None):
+                # none is OK because is_dominant column may be missing
                 variant.effect_type = EffectType.RECESSIVE
             case _:
                 logger.critical(f"Bad effect type setting: {variant}")
                 raise Exception
         yield variant
```

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_read.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_read.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/_relabel.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_relabel.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/catalogapi.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/catalogapi.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/genomebuild.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/genomebuild.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     GenomeBuild.GRCh38
     """
 
     GRCh37 = "GRCh37"
     GRCh38 = "GRCh38"
     # just included to handle older files, incompatible unless harmonised:
     NCBI36 = "NCBI36"  # ew
+    NCBI35 = "NCBI35"  # huh
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return f"{type(self).__name__}.{self.name}"
 
@@ -43,9 +44,11 @@
                 return cls(GenomeBuild.GRCh37)
             case "GRCh38" | "hg38":
                 return cls(GenomeBuild.GRCh38)
             case "NR" | "" | None:
                 return None
             case "NCBI36" | "hg18":
                 return cls(GenomeBuild.NCBI36)
+            case "NCBI35" | "hg17":
+                return cls(GenomeBuild.NCBI35)
             case _:
                 raise ValueError(f"Can't match {build=}")
```

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/pgsexceptions.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/pgsexceptions.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/scorefiles.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorefiles.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/scorevariant.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorevariant.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.0/src/pgscatalog/core/lib/targetvariants.py` & `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/targetvariants.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,14 +105,22 @@
     ...    variant
     ...    break
     TargetVariant(chrom='1', pos=10180, ref='C', alt='T', id='1:10180:T:C')
 
     Note, A1/A2 isn't guaranteed to be ref/alt because of PLINK1 file format
     limitations. PGS Catalog libraries handle this internally, but you should be
     aware REF/ALT can be swapped by plink during VCF to bim conversion.
+
+    Some pvar files can contain a lot of comments in the header, which are ignored:
+
+    >>> pvar = TargetVariants(Config.ROOT_DIR / "tests" / "data" / "1000G.pvar")
+    >>> for variant in pvar:
+    ...     variant
+    ...     break
+    TargetVariant(chrom='1', pos=10390, ref='CCCCTAACCCCTAACCCTAACCCTAACCCTAACCCTAACCCTAA', alt='C', id='1:10390:CCCCTAACCCCTAACCCTAACCCTAACCCTAACCCTAACCCTAA:C')
     """
 
     def __init__(self, path, chrom=None):
         match n := pathlib.Path(path).name:
             case _ if "pvar" in n:
                 self.ftype = TargetType.PVAR
             case _ if "bim" in n:
@@ -189,15 +197,21 @@
                 [chroms, positions, ids, refs, alts], schema=self.pa_schema()
             )
 
 
 def read_pvar(path):
     with xopen(path, "rt") as f:
         # pvars do have a header column and support arbitrary columns
-        reader = csv.DictReader(f, delimiter="\t")
+        for line in f:
+            if line.startswith("##"):
+                continue
+            else:
+                fieldnames = line.strip().split("\t")
+                break
+        reader = csv.DictReader(f, fieldnames=fieldnames, delimiter="\t")
         fields = {
             "#CHROM": "chrom",
             "POS": "pos",
             "REF": "ref",
             "ALT": "alt",
             "ID": "id",
         }
```

### Comparing `pgscatalog_core-0.1.0/PKG-INFO` & `pgscatalog_core-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgscatalog.core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Core tools for working with polygenic scores (PGS) and the PGS Catalog
 License: Apache-2.0
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

