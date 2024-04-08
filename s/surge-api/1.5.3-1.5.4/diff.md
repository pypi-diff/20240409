# Comparing `tmp/surge_api-1.5.3-py3-none-any.whl.zip` & `tmp/surge_api-1.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 18679 bytes, number of entries: 16
+Zip file size: 18758 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      260 b- defN 24-Mar-13 18:58 surge/__init__.py
--rw-r--r--  2.0 unx     3363 b- defN 24-Apr-04 21:46 surge/api_resource.py
+-rw-r--r--  2.0 unx     3363 b- defN 24-Apr-04 21:58 surge/api_resource.py
 -rw-r--r--  2.0 unx      949 b- defN 24-Mar-13 18:58 surge/carousel.py
 -rw-r--r--  2.0 unx     1606 b- defN 24-Mar-13 18:58 surge/errors.py
--rw-r--r--  2.0 unx    14523 b- defN 24-Apr-04 21:46 surge/projects.py
--rw-r--r--  2.0 unx    32290 b- defN 24-Apr-04 21:46 surge/questions.py
--rw-r--r--  2.0 unx     5551 b- defN 24-Apr-04 21:46 surge/reports.py
+-rw-r--r--  2.0 unx    14523 b- defN 24-Apr-04 21:58 surge/projects.py
+-rw-r--r--  2.0 unx    36342 b- defN 24-Apr-08 22:55 surge/questions.py
+-rw-r--r--  2.0 unx     5551 b- defN 24-Apr-04 21:58 surge/reports.py
 -rw-r--r--  2.0 unx      939 b- defN 24-Mar-13 18:58 surge/responses.py
--rw-r--r--  2.0 unx     6185 b- defN 24-Apr-04 21:46 surge/tasks.py
--rw-r--r--  2.0 unx     4433 b- defN 24-Apr-04 21:46 surge/teams.py
+-rw-r--r--  2.0 unx     6185 b- defN 24-Apr-04 21:58 surge/tasks.py
+-rw-r--r--  2.0 unx     4433 b- defN 24-Apr-04 21:58 surge/teams.py
 -rw-r--r--  2.0 unx      442 b- defN 24-Mar-13 18:58 surge/utils.py
--rw-r--r--  2.0 unx     1062 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4402 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-04 21:48 surge_api-1.5.3.dist-info/RECORD
-16 files, 77304 bytes uncompressed, 16741 bytes compressed:  78.3%
+-rw-r--r--  2.0 unx     1062 b- defN 24-Apr-08 22:59 surge_api-1.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4452 b- defN 24-Apr-08 22:59 surge_api-1.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 22:59 surge_api-1.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-08 22:59 surge_api-1.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-08 22:59 surge_api-1.5.4.dist-info/RECORD
+16 files, 81406 bytes uncompressed, 16820 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: surge/teams.py
 Comment: 
 
 Filename: surge/utils.py
 Comment: 
 
-Filename: surge_api-1.5.3.dist-info/LICENSE
+Filename: surge_api-1.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: surge_api-1.5.3.dist-info/METADATA
+Filename: surge_api-1.5.4.dist-info/METADATA
 Comment: 
 
-Filename: surge_api-1.5.3.dist-info/WHEEL
+Filename: surge_api-1.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: surge_api-1.5.3.dist-info/top_level.txt
+Filename: surge_api-1.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: surge_api-1.5.3.dist-info/RECORD
+Filename: surge_api-1.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## surge/questions.py

```diff
@@ -64,15 +64,28 @@
                 required=q["required"],
                 preexisting_annotations=q["preexisting_annotations"],
                 require_tiebreaker=q["require_tie_breaker"],
                 shown_by_option_id=q["shown_by_item_option_id"],
                 hidden_by_option_id=q["hidden_by_item_option_id"],
                 holistic=q["holistic"],
                 question_category=q.get("question_category"))
-
+        elif q["type"] == "likert":
+            return LikertQuestion(
+                q["text"],
+                q["label"],
+                id=q["id"],
+                options=q["options"],
+                options_info=options_info,
+                required=q["required"],
+                preexisting_annotations=q["preexisting_annotations"],
+                require_tiebreaker=q["require_tie_breaker"],
+                shown_by_option_id=q["shown_by_item_option_id"],
+                hidden_by_option_id=q["hidden_by_item_option_id"],
+                holistic=q["holistic"],
+                question_category=q.get("question_category"))
         elif q["type"] == "checkbox":
             return CheckboxQuestion(
                 q["text"],
                 q["label"],
                 id=q["id"],
                 options=q["options"],
                 options_info=options_info,
@@ -271,14 +284,69 @@
                          required=required,
                          column_header=column_header,
                          question_category=question_category)
         self.options = options
         self.options_info = options_info
         self.descriptions = descriptions
         self.preexisting_annotations = preexisting_annotations
+        self.require_tiebreaker = require_tiebreaker
+        self.hidden_by_option_id = hidden_by_option_id
+        self.shown_by_option_id = shown_by_option_id
+        self.holistic = holistic
+
+
+class LikertQuestion(Question):
+
+    def __init__(self,
+                 text,
+                 label,
+                 id=None,
+                 options=[],
+                 options_info=None,
+                 descriptions=[],
+                 required=True,
+                 preexisting_annotations=None,
+                 require_tiebreaker=False,
+                 column_header=None,
+                 hidden_by_option_id=None,
+                 shown_by_option_id=None,
+                 holistic=False,
+                 question_category=None):
+        '''
+        Create a likert radio question.
+
+        Args:
+            text (string): Required. The text of the question being asked, e.g. "Is the sentiment of this text positive or negative?"
+            label (string): Required. The label of the question being asked, e.g. "Overall Quality: Model A"
+            id (string): The UUID of this question, if it has been created. Otherwise, it will be None.
+            options (list of strings): Required. A list of the options for the radios, e.g. ["Yes", "No"].
+            options_info (list of objects): Additional information about the options if the question has already been created. Otherwise, it will be None.
+            descriptions(list of strings): Tooltip text for the options. This should have the same length as the options.
+                You can substitute in empty strings if one option doesn't have a tooltip.
+            required (boolean): Defaults to true. Whether or not workers must fill out this question before moving on to the next task.
+            preexisting_annotations (string): You can use preexisting annotations to prepopulate the radio selection with an option specified in the task data.
+                The preexisting_annotations param should contain the task data key you are loading the default values from.
+            require_tiebreaker (boolean): If set to true, more workers will be assigned to this task if fewer than 50% agree on an answer.
+                For example, imagine you are using two workers per task. If one selects Option A and the second one selections Option B a third will be assigned to the task to break the tie.
+            column_header (string): This value will be used as the column header for the results table on the Surge AI site and in results CSV and JSON files.
+            hidden_by_option_id (string): If set, this question will be visible by default but hidden when the option with the provided id is selected.
+            shown_by_option_id (string). If set, this question will be hidden by default but shown when the option with the provided id is selected.
+            question_category (string): The question category for the relevant workstream.
+        '''
+        super().__init__(id,
+                         text,
+                         label,
+                         type_="likert",
+                         required=required,
+                         column_header=column_header,
+                         question_category=question_category)
+        self.options = options
+        self.options_info = options_info
+        self.descriptions = descriptions
+        self.preexisting_annotations = preexisting_annotations
         self.require_tiebreaker = require_tiebreaker
         self.hidden_by_option_id = hidden_by_option_id
         self.shown_by_option_id = shown_by_option_id
         self.holistic = holistic
 
 
 class CheckboxQuestion(Question):
```

## Comparing `surge_api-1.5.3.dist-info/LICENSE` & `surge_api-1.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `surge_api-1.5.3.dist-info/METADATA` & `surge_api-1.5.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surge-api
-Version: 1.5.3
+Version: 1.5.4
 Summary: Surge Python SDK
 Home-page: https://github.com/surge-ai/surge-python
 Author: Surge
 Author-email: team@surgehq.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -89,22 +89,25 @@
 Or you can create a new project from scratch by creating your own template and list of Question:
 
 ```python
 from surge.questions import FreeResponseQuestion, MultipleChoiceQuestion, CheckboxQuestion
 
 # Create a new Project
 free_response_q = FreeResponseQuestion(
-    text="What is this company's website?")
+    text="What is this company's website?",
+    label="")
 
 multiple_choice_q = MultipleChoiceQuestion(
     text="What category does this company belong to?",
+    label="Category",
     options=["Tech", "Sports", "Gaming"])
 
 checkbox_q = CheckboxQuestion(
     text="Check all the social media accounts this company has",
+    label="",
     options=["Facebook", "Twitter", "Pinterest", "Google+"])
 
 fields_template_text = '''
     <p>Company: {{company}}</p>
 '''
 
 project = surge.Project.create(
```

## Comparing `surge_api-1.5.3.dist-info/RECORD` & `surge_api-1.5.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 surge/__init__.py,sha256=EbBXghvhL6SxEURWh2-92f0oM9vsw0sG3C82fHCI_ko,260
 surge/api_resource.py,sha256=m89DCbbEo4zdLtoa5tUo1cg2RFGRCnuK5YTAC-KfEVI,3363
 surge/carousel.py,sha256=ZCYGVsgd8G2u-goTB49RuzbknV-s3v7hYgr9jQVYtv8,949
 surge/errors.py,sha256=N83WpLlqrRi_Y03-q8JUXlutgCUpUrMeL47TvbOv11c,1606
 surge/projects.py,sha256=y7uK5pLsf4EnJD9BCIhb9N-aZPcKXmIMGw5iMLmEuVI,14523
-surge/questions.py,sha256=gqs1C2gy3JXSUqzqknbDHH4QISS7-3f-XBVGwKp-Tio,32290
+surge/questions.py,sha256=RdJD0efM-Ep5OKPzDzUffY9PZsFOQl6sIiPKRzfzqmQ,36342
 surge/reports.py,sha256=pbBtaV3-MBvmZ8-FFpl2s9WY_LOakYhUtAdr43Nx1WE,5551
 surge/responses.py,sha256=uQIQj55KS2H334OBXIe59FFEerOnDuqk0MhTTUye-D4,939
 surge/tasks.py,sha256=sy8OU1Qh2Q504eEw7zC9PSmIs8sQARAysb4cURhNyp4,6185
 surge/teams.py,sha256=GbmonLJ_44UeG4Fr4KBGu9-pBgZPI_I1ovwyFnTC1po,4433
 surge/utils.py,sha256=4SO3vQVwOOgn-mrDFmUH0HipfRJwcU8v5eTXp4uoZag,442
-surge_api-1.5.3.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
-surge_api-1.5.3.dist-info/METADATA,sha256=PnkIMq1KPmmtZ-187v7p4fiEsz-g3WIZIZ5lIxQHvxw,4402
-surge_api-1.5.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-surge_api-1.5.3.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
-surge_api-1.5.3.dist-info/RECORD,,
+surge_api-1.5.4.dist-info/LICENSE,sha256=n298NNjFKoaxocxZ1_4E-TJURJV1-MLq78cFp6bo2I0,1062
+surge_api-1.5.4.dist-info/METADATA,sha256=bYwlW-N6TcRS-OGi695V_PI9zQz448fAhYTZoFSuBk0,4452
+surge_api-1.5.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+surge_api-1.5.4.dist-info/top_level.txt,sha256=jnubIyC0boBGzxSTRKNAKSVrVru3VgSHWf_q_qFRm_A,6
+surge_api-1.5.4.dist-info/RECORD,,
```

