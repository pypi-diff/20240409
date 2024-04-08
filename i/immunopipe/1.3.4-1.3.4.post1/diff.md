# Comparing `tmp/immunopipe-1.3.4.tar.gz` & `tmp/immunopipe-1.3.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunopipe-1.3.4.tar", max compression
+gzip compressed data, was "immunopipe-1.3.4.post1.tar", max compression
```

## Comparing `immunopipe-1.3.4.tar` & `immunopipe-1.3.4.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35128 2024-04-05 03:27:08.824260 immunopipe-1.3.4/LICENSE
--rw-r--r--   0        0        0     1448 2024-04-05 03:27:08.824260 immunopipe-1.3.4/README.md
--rw-r--r--   0        0        0      143 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/__init__.py
--rw-r--r--   0        0        0      109 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/__main__.py
--rw-r--r--   0        0        0     7461 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/inhouse.py
--rw-r--r--   0        0        0      503 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/pipeline.py
--rw-r--r--   0        0        0    32543 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/processes.py
--rw-r--r--   0        0        0     1581 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/reports/CloneHeterogeneity.svelte
--rw-r--r--   0        0        0      683 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/reports/MarkersOverlapping.svelte
--rw-r--r--   0        0        0      101 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/reports/TCellSelection.svelte
--rw-r--r--   0        0        0     4769 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/scripts/CloneHeterogeneity.R
--rw-r--r--   0        0        0     2029 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/scripts/MarkersOverlapping.R
--rw-r--r--   0        0        0    15647 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/scripts/TCellSelection.R
--rw-r--r--   0        0        0     3281 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/validate_config.py
--rw-r--r--   0        0        0       22 2024-04-05 03:27:08.880260 immunopipe-1.3.4/immunopipe/version.py
--rw-r--r--   0        0        0     1107 2024-04-05 03:27:08.880260 immunopipe-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 immunopipe-1.3.4/setup.py
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 immunopipe-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-08 23:53:51.638916 immunopipe-1.3.4.post1/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-08 23:53:51.638916 immunopipe-1.3.4.post1/README.md
+-rw-r--r--   0        0        0      143 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/__main__.py
+-rw-r--r--   0        0        0     7461 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/inhouse.py
+-rw-r--r--   0        0        0      503 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/pipeline.py
+-rw-r--r--   0        0        0    33594 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/processes.py
+-rw-r--r--   0        0        0     1581 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/CloneHeterogeneity.svelte
+-rw-r--r--   0        0        0      683 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/MarkersOverlapping.svelte
+-rw-r--r--   0        0        0      101 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/TCellSelection.svelte
+-rw-r--r--   0        0        0     4769 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/CloneHeterogeneity.R
+-rw-r--r--   0        0        0     2029 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/MarkersOverlapping.R
+-rw-r--r--   0        0        0    15647 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/TCellSelection.R
+-rw-r--r--   0        0        0     3281 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/validate_config.py
+-rw-r--r--   0        0        0       28 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/version.py
+-rw-r--r--   0        0        0     1127 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/pyproject.toml
+-rw-r--r--   0        0        0     2470 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post1/setup.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post1/PKG-INFO
```

### Comparing `immunopipe-1.3.4/LICENSE` & `immunopipe-1.3.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/README.md` & `immunopipe-1.3.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/inhouse.py` & `immunopipe-1.3.4.post1/immunopipe/inhouse.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/processes.py` & `immunopipe-1.3.4.post1/immunopipe/processes.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,17 +38,21 @@
 from .validate_config import validate_config
 
 toml_dumps = FILTERS["toml_dumps"]
 just_loading = is_loading_pipeline()
 config = validate_config()
 
 DOC_BASEURL = "https://pwwang.github.io/immunopipe"
+TEST_OUTPUT_BASEURL = "https://raw.githubusercontent.com/pwwang/immunopipe/dev/tests/output"  # noqa: E501
 
 
-@annotate.format_doc(indent=1, vars={"baseurl": DOC_BASEURL})
+@annotate.format_doc(
+    indent=1,
+    vars={"baseurl": DOC_BASEURL, "output_baseurl": TEST_OUTPUT_BASEURL},
+)
 class SampleInfo(SampleInfo_):
     """{{Summary}}
 
     This process is the entrance of the pipeline. It just pass by input file and list
     the sample information in the report.
 
     To specify the input file in the configuration file, use the following
@@ -97,67 +101,95 @@
     cache = false
     ```
     ///
 
     Examples:
         ### Example data
 
-        | Subject | Sample | Source | Score |
-        | ------- | ------ | ------ | ----- |
-        | A       | A1     | Tumor  | 1     |
-        | A       | A2     | Numor  | 8     |
-        | A       | A3     | Tumor  |3      |
-        | A       | A4     | Normal |8      |
-        | B       | B1     | Tumor  |2      |
-        | B       | B2     | Normal |8      |
-        | B       | B3     | Tumor  |4      |
-        | B       | B4     | Normal |8      |
-        | C       | C1     | Tumor  |9      |
-        | C       | C2     | Normal |3      |
-        | C       | C3     | Tumor  |7      |
-        | C       | C4     | Normal |3      |
-        | D       | D1     | Tumor  |10     |
-        | D       | D2     | Normal |5      |
-        | D       | D3     | Tumor  |10     |
-        | D       | D4     | Normal |5      |
-        | E       | E1     | Tumor  |6      |
-        | E       | E2     | Normal |5      |
-        | E       | E3     | Tumor  |6      |
-        | E       | E4     | Normal |5      |
-        | F       | F1     | Tumor  |8      |
-        | F       | F2     | Normal |10     |
-        | F       | F3     | Tumor  |8      |
-        | F       | F4     | Normal |10     |
+        | Sample | Age | Sex | Diagnosis |
+        |--------|-----|-----|-----------|
+        | C1     | 62  | F   | Colitis   |
+        | C2     | 71.2| F   | Colitis   |
+        | C3     | 56.2| M   | Colitis   |
+        | C4     | 61.5| M   | Colitis   |
+        | C5     | 72.8| M   | Colitis   |
+        | C6     | 78.4| M   | Colitis   |
+        | C7     | 61.6| F   | Colitis   |
+        | C8     | 49.5| F   | Colitis   |
+        | NC1    | 43.6| M   | NoColitis |
+        | NC2    | 68.1| M   | NoColitis |
+        | NC3    | 70.5| F   | NoColitis |
+        | NC4    | 63.7| M   | NoColitis |
+        | NC5    | 58.5| M   | NoColitis |
+        | NC6    | 49.3| F   | NoColitis |
+        | CT1    | 21.4| F   | Control   |
+        | CT2    | 61.7| M   | Control   |
+        | CT3    | 50.5| M   | Control   |
+        | CT4    | 43.4| M   | Control   |
+        | CT5    | 70.6| F   | Control   |
+        | CT6    | 44.3| M   | Control   |
+        | CT7    | 50.2| M   | Control   |
+        | CT8    | 61.5| F   | Control   |
 
-        ### Count the number of samples per Source
+        ### Count the number of samples per Diagnosis
 
         ```toml
-        [SampleInfo.envs.stats]
-        Samples_Source = { "group": "Source" }
-        Samples_Source_each_Subject = { "group": "Source", "each": "Subject" }
+        [SampleInfo.envs.stats."N_Samples_per_Diagnosis (pie)"]
+        on = "sample"
+        group = "Diagnosis"
         ```
 
-        ![Samples_Source]({{baseurl}}/processes/images/SampleInfo_Samples_Source.png)
+        ![Samples_Diagnosis]({{output_baseurl}}/sampleinfo/SampleInfo/N_Samples_per_Diagnosis (pie).png)
 
-        ### Explore the distribution of the Score
+        What if we want a bar plot instead of a pie chart?
 
         ```toml
-        [SampleInfo.envs.stats.Score_Source_vlnbox]
-        on = "Score"
-        group = "Source"
-        plot = "violin+box"
-
-        [SampleInfo.envs.stats.Score_Source_each_Subject_vlnbox]
-        on = "Score"
-        group = "Source"
-        plot = "violin+box"
-        each = "Subject"
+        [SampleInfo.envs.stats."N_Samples_per_Diagnosis (bar)"]
+        on = "sample"
+        group = "Diagnosis"
+        plot = "barplot"
         ```
 
-        ![Score_Source]({{baseurl}}/processes/images/SampleInfo_Score_Source.png)
+        ![Samples_Diagnosis_bar]({{output_baseurl}}/sampleinfo/SampleInfo/N_Samples_per_Diagnosis (bar).png)
+
+        ### Explore Age distribution
+
+        The distribution of Age of all samples
+
+        ```toml
+        [SampleInfo.envs.stats."Age_distribution (boxplot)"]
+        on = "Age"
+        ```
+
+        ![Age_distribution]({{output_baseurl}}/sampleinfo/SampleInfo/Age_distribution (boxplot).png)
+
+        How about the distribution of Age in each Diagnosis, and make it violin + boxplot?
+
+        ```toml
+        [SampleInfo.envs.stats."Age_distribution_per_Diagnosis (violin + boxplot)"]
+        on = "Age"
+        group = "Diagnosis"
+        plot = "violin+boxplot"
+        ```
+
+        ![Age_distribution_per_Diagnosis]({{output_baseurl}}/sampleinfo/SampleInfo/Age_distribution_per_Diagnosis (violin + boxplot).png)
+
+        How about Age distribution per Sex in each Diagnosis?
+
+        ```toml
+        [SampleInfo.envs.stats."Age_distribution_per_Sex_in_each_Diagnosis (boxplot)"]
+        on = "Age"
+        group = "Sex"
+        each = "Diagnosis"
+        plot = "boxplot"
+        ncol = 3
+        devpars = {height = 450}
+        ```
+
+        ![Age_distribution_per_Sex_in_each_Diagnosis]({{output_baseurl}}/sampleinfo/SampleInfo/Age_distribution_per_Sex_in_each_Diagnosis (boxplot).png)
 
     Input:
         infile (required): {{Input.infile.help | indent: 12}}.
             The input file should have the following columns.
             * Sample: A unique id for each sample.
             * TCRData: The directory for single-cell TCR data for this sample.
                 Specifically, it should contain filtered_contig_annotations.csv
```

### Comparing `immunopipe-1.3.4/immunopipe/reports/CloneHeterogeneity.svelte` & `immunopipe-1.3.4.post1/immunopipe/reports/CloneHeterogeneity.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/reports/MarkersOverlapping.svelte` & `immunopipe-1.3.4.post1/immunopipe/reports/MarkersOverlapping.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/scripts/CloneHeterogeneity.R` & `immunopipe-1.3.4.post1/immunopipe/scripts/CloneHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/scripts/MarkersOverlapping.R` & `immunopipe-1.3.4.post1/immunopipe/scripts/MarkersOverlapping.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/scripts/TCellSelection.R` & `immunopipe-1.3.4.post1/immunopipe/scripts/TCellSelection.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/immunopipe/validate_config.py` & `immunopipe-1.3.4.post1/immunopipe/validate_config.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4/pyproject.toml` & `immunopipe-1.3.4.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "immunopipe"
 description = "A pipeline for integrative analysis for scTCR- and scRNA-seq data"
 authors = [ "pwwang <pwwang@pwwang.com>",]
-version = "1.3.4"
+version = "1.3.4-post1"
 license = "GNU General Public License v3.0"
 readme = "README.md"
 homepage = "https://github.com/pwwang/immunopipe"
 repository = "https://github.com/pwwang/immunopipe"
 
 [tool.poetry.build]
 generate-setup-file = true
@@ -26,14 +26,15 @@
 diagram = ["pipen-diagram"]
 runinfo = ["pipen-runinfo"]
 
 [tool.poetry.group.docs.dependencies]
 pipen-cli-ref = "^0.3"
 
 [tool.poetry.dev-dependencies]
+pytest = "^8"
 
 [tool.poetry.scripts]
 immunopipe = "immunopipe.pipeline:main"
 
 [tool.poetry.group.dev.dependencies]
 # pipen-dry = "^0.1.0"
```

### Comparing `immunopipe-1.3.4/setup.py` & `immunopipe-1.3.4.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'runinfo': ['pipen-runinfo>=0.6,<0.7']}
 
 entry_points = \
 {'console_scripts': ['immunopipe = immunopipe.pipeline:main']}
 
 setup_kwargs = {
     'name': 'immunopipe',
-    'version': '1.3.4',
+    'version': '1.3.4.post1',
     'description': 'A pipeline for integrative analysis for scTCR- and scRNA-seq data',
     'long_description': '<p align="center">\n  <img height="120" style="height: 120px" src="https://github.com/pwwang/immunopipe/blob/dev/docs/logo.png?raw=true" />\n</p>\n<p align="center">Integrative analysis for single-cell RNA sequencing and single-cell TCR sequencing data</p>\n<hr />\n\n`immunopipe` is a pipeline based on [`pipen`](https://github.com/pwwang/pipen) framework. It includes a set of processes for scTCR- and scRNA-seq data analysis in `R`, `python` and `bash`. The pipeline is designed to be flexible and configurable.\n\n<p align="center">\n  <img src="https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.ms.png?raw=true" />\n</p>\n\nSee a more detailed flowchart [here](https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.flowchart.png?raw=true).\n\n## Documentaion\n\n[https://pwwang.github.io/immunopipe](https://pwwang.github.io/immunopipe)\n\n## Proposing more analyses\n\nIf you have any suggestions for more analyses, please feel free to open an issue [here](https://github.com/pwwang/immunopipe/issues/new)\n\n## Example\n\n[https://github.com/pwwang/immunopipe-example](https://github.com/pwwang/immunopipe-example)\n\n## Gallery\n\nThere are some datasets with both scRNA-seq and scTCR-seq data available in the publications. The data were reanalyzed using `immunopipe` with the configurations provided in each repository, where the results are also available.\n\nCheck out the [gallery](https://pwwang.github.io/immunopipe/gallery) for more details.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/immunopipe',
```

### Comparing `immunopipe-1.3.4/PKG-INFO` & `immunopipe-1.3.4.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immunopipe
-Version: 1.3.4
+Version: 1.3.4.post1
 Summary: A pipeline for integrative analysis for scTCR- and scRNA-seq data
 Home-page: https://github.com/pwwang/immunopipe
 License: GNU General Public License v3.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

