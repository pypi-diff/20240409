# Comparing `tmp/wordview-1.3.0.tar.gz` & `tmp/wordview-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-1.3.0.tar", max compression
+gzip compressed data, was "wordview-1.4.0.tar", max compression
```

## Comparing `wordview-1.3.0.tar` & `wordview-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3617 2024-04-04 11:52:47.999539 wordview-1.3.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2024-04-04 11:52:47.999539 wordview-1.3.0/LICENSE
--rw-r--r--   0        0        0     1061 2024-04-04 11:52:48.167539 wordview-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      163 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4789 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       53 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/__init__.py
--rw-r--r--   0        0        0    11136 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/bias.py
--rw-r--r--   0        0        0     4131 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/bias_analysis/bias_terms.py
--rw-r--r--   0        0        0       48 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0     1416 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/io/dataframe_reader.py
--rw-r--r--   0        0        0       34 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     1764 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/association_measures.py
--rw-r--r--   0        0        0    10974 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     1967 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/mwes/patterns.py
--rw-r--r--   0        0        0      111 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3155 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0     3794 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/preprocessing/count.py
--rw-r--r--   0        0        0       75 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0     5809 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/chat/chat.html
--rw-r--r--   0        0        0    14234 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0    16189 2024-04-04 11:52:48.191539 wordview-1.3.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 wordview-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3728 2024-04-09 14:47:32.052822 wordview-1.4.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2024-04-09 14:47:32.052822 wordview-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1061 2024-04-09 14:47:32.208824 wordview-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       53 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/bias_analysis/__init__.py
+-rw-r--r--   0        0        0    11136 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/bias_analysis/bias.py
+-rw-r--r--   0        0        0     4131 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/bias_analysis/bias_terms.py
+-rw-r--r--   0        0        0     9145 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/chat_ui/chat.html
+-rw-r--r--   0        0        0       48 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0     1416 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/io/dataframe_reader.py
+-rw-r--r--   0        0        0       34 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     1229 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/mwes/association_measures.py
+-rw-r--r--   0        0        0    15108 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3295 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/mwes/patterns.py
+-rw-r--r--   0        0        0      111 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3155 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0     3794 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/preprocessing/count.py
+-rw-r--r--   0        0        0       75 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    14411 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0    16151 2024-04-09 14:47:32.232824 wordview-1.4.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 wordview-1.4.0/PKG-INFO
```

### Comparing `wordview-1.3.0/CHANGES.rst` & `wordview-1.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Version 1.4.0
+-------------
+- Chat feature for MWE.
+- Improve chat UI.
+- MWE and text analysis improvements.
+
+
 Version 1.3.0
 -------------
 - Chat feature for text analysis.
 
 
 Version 1.2.0
 -------------
```

### Comparing `wordview-1.3.0/LICENSE` & `wordview-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/pyproject.toml` & `wordview-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "1.3.0"
+version = "1.4.0"
 description = """Wordview is a Python package for Exploratory Data Analysis of text and provides many statistics about your data in the form of plots, tables, and descriptions allowing you to have both a high-level and detailed overview of your data."""
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 include = ["CHANGES.rst"]
 exclude = ["notebooks/", "tests/", "data/"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-1.3.0/wordview/anomaly/gaussianize.py` & `wordview-1.4.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/anomaly/normaldist.py` & `wordview-1.4.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/bias_analysis/bias.py` & `wordview-1.4.0/wordview/bias_analysis/bias.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/bias_analysis/bias_terms.py` & `wordview-1.4.0/wordview/bias_analysis/bias_terms.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/clustering/cluster.py` & `wordview-1.4.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/io/dataframe_reader.py` & `wordview-1.4.0/wordview/io/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/mwes/association_measures.py` & `wordview-1.4.0/wordview/mwes/association_measures.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 import json
 import math
 
 
 class PMICalculator:
     """Calculates the Pointwise Mutual Information (PMI) of an n-gram candidate."""
 
-    def __init__(self, ngram_count_source=None, ngram_count_file_path=None):
+    def __init__(self, ngram_count_source: dict):
         """Initializes a new instance of PMICalculator class.
 
         Args:
             ngram_count_source: A dictionary containing ngram counts.
-            ngram_count_file_path: A path to a json file containing ngram counts.
 
         Returns:
             None
         """
-        if ngram_count_source:
-            self.counts = ngram_count_source
-        elif ngram_count_file_path:
-            self.counts = self._load_ngram_counts(ngram_count_file_path)
-        else:
-            raise ValueError("Either count_source or count_file_path must be provided.")
-
+        self.counts = ngram_count_source
         self.total_count = sum(self.counts.values())
 
-    def _load_ngram_counts(self, count_file_path) -> dict[str, int]:
-        with open(count_file_path, "r") as file:
-            counts = json.load(file)
-        return counts
-
     def _prob(self, ngram) -> float:
         return self.counts.get(ngram, 0) / self.total_count
 
     def compute_association(self, ngram: str) -> float:
         """Computes the association measure (AM)  --currently only in terms of
         PMI, of an n-gram candidate.
```

### Comparing `wordview-1.3.0/wordview/mwes/mwe.py` & `wordview-1.4.0/wordview/mwes/mwe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import json
 import re
 import string
+import threading
 from re import Match
 from typing import Optional
 
 import nltk
 import pandas
+from flask import Flask, jsonify, request, send_from_directory
 from nltk import RegexpParser, word_tokenize
+from openai import OpenAI
 from tabulate import tabulate  # type: ignore
 from tqdm import tqdm
 
 from bin.nltk_resources import check_nltk_resources
 from wordview import logger
 from wordview.io.dataframe_reader import DataFrameReader
 from wordview.mwes.association_measures import PMICalculator
@@ -22,25 +26,29 @@
     return match
 
 
 check_nltk_resources()
 
 
 class MWE:
-    """Extract MWEs of type LVC, VPC, Noun Compounds, Adjective Compounds, and custom patterns from a text corpus."""
+    """Extract MWEs of typeS:
+    LVC, VPC, Noun Compounds, Adjective Compounds, and custom patterns from a text corpus.
+    """
 
     def __init__(
         self,
         df: pandas.DataFrame,
         text_column: str,
         ngram_count_source=None,
         ngram_count_file_path=None,
         language: str = "EN",
         custom_patterns: Optional[str] = None,
         only_custom_patterns: bool = False,
+        mwe_frequency_threshold: int = 10,
+        association_threshold: float = 1.0,
     ) -> None:
         """Initializes a new instance of MWE class.
 
         Args:
             df: A pandas DataFrame containing the text corpus.
             text_column: The name of the column containing the text.
             ngram_count_source: A dictionary containing ngram counts.
@@ -52,22 +60,39 @@
                 You can use multiple and/or nested patterns, separated by a newline character e.g.:
                 custom_pattern = '''
                 VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
                 PROPN: {<NNP>+} # Proper noun
                 ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
                 ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase'''
             only_custom_pattern: If True, only the custom pattern will be used to extract MWEs, otherwise, the default patterns will be used as well.
+            mwe_frequency_threshold: The minimum frequency of an MWE to be considered for extraction. Defaults to 10.
+            association_threshold: A threshold value for the association measure. Only MWEs with an association measure above this threshold will be returned.
 
             Returns:
                 None
         """
         self.language = language.upper()
         self.mwes: dict[str, dict[str, float]] = {}
         self.reader = DataFrameReader(df, text_column)
         self.mwe_extractor = None
+        self.counts = {}
+        self.association_threshold = association_threshold
+        self.mwe_frequency_threshold = mwe_frequency_threshold
+
+        if ngram_count_source:
+            self.counts = ngram_count_source
+        elif ngram_count_file_path:
+            try:
+                self.counts = self._load_ngram_counts(ngram_count_file_path)
+            except ValueError as e:
+                raise ValueError(
+                    "Failed to load n-gram counts. Ensure the file path is correct."
+                ) from e
+            except Exception as e:
+                raise Exception(f"An unexpected error occurred: {str(e)}") from e
 
         mwe_patterns: str = ""
         if language == "EN":
             for _, value in EnMWEPatterns().patterns.items():
                 for v in value:
                     mwe_patterns += v + "\n"
         elif language == "DE":
@@ -87,35 +112,99 @@
                         with a value of: {custom_patterns}."
                     )
                 mwe_patterns = custom_patterns
             else:
                 mwe_patterns += "\n" + custom_patterns
 
         # Create an MWEPatternAssociation extractor object
-        self.mwe_extractor = MWEPatternAssociation(
+        self.mwe_extractor = MWEPatternCountAssociation(
             association_measure=PMICalculator(
-                ngram_count_source=ngram_count_source,
-                ngram_count_file_path=ngram_count_file_path,
+                ngram_count_source=self.counts,
             ),
             custom_pattern=mwe_patterns,
+            count_source=self.counts,
+            mwe_frequency_threshold=self.mwe_frequency_threshold,
+            association_threshold=self.association_threshold,
         )
 
+    def chat(self, api_key: str = ""):
+        """Chat with OpenAI's latest model about MWEs .
+        Access the chat UI in your localhost under http://127.0.0.1:5001/
+
+        Args:
+            api_key: OpenAI API key.
+
+        Returns:
+            None
+        """
+        self.api_key = api_key
+        self.chat_client = OpenAI(api_key=api_key)
+        base_content = f"""Answer any questions about the Multiword Expressions (MWEs) that extracted from the uploaded text corpus by Wordview and are presented in the following MWEs dictionary.
+        \n\n
+        ------------------------------
+        MWEs dictionary:
+        ------------------------------
+        {self.mwes}
+        \n\n
+        Important Points:\n
+        - Answer the questions without including "According/based on to MWEs dictionary".\n
+        - The format of the above dictionary is as follows:\n
+            "MWE Type": "MWE instance 1": "Association measure", "MWE instance 2": "Association measure", ...\n
+        - There could be other custom types in which case you should just mention the dictionary key.\n
+        - Depending on a parameter N set by the user, each MWE type contains at most N instances. But it can contain less or even 0.
+        - Return the association measures that you read from the dictionary with only two decimal places.
+        """
+        chat_history = [
+            {"role": "system", "content": base_content},
+        ]
+        app = Flask(__name__, static_folder="path_to_your_ui_folder")
+
+        @app.route("/")
+        def index():
+            return send_from_directory("../chat_ui", "chat.html")
+
+        @app.route("/chat", methods=["POST"])
+        def chat():
+            user_input = request.json["message"]
+            chat_history.append({"role": "user", "content": user_input})
+            response = (
+                self.chat_client.chat.completions.create(
+                    model="gpt-3.5-turbo",
+                    messages=chat_history,
+                )
+                .choices[0]
+                .message.content
+            )
+            chat_history.append({"role": "assistant", "content": response})
+            return jsonify({"reply": response})
+
+        def run():
+            app.run(port=5001)
+
+        flask_thread = threading.Thread(target=run)
+        flask_thread.start()
+
+    def _load_ngram_counts(self, count_file_path) -> dict[str, int]:
+        with open(count_file_path, "r") as file:
+            counts = json.load(file)
+        return counts
+
     def extract_mwes(
         self,
         sort: bool = True,
         top_n: Optional[int] = None,
     ) -> dict[str, dict[str, float]]:
-        """Extract MWEs from the text corpus.
+        """Extract MWEs from the text corpus and add them to self.mwes.
 
         Args:
             sort: If True, the MWEs will be sorted in descending order of association measure.
             top_n: If provided, only the top n MWEs will be returned.
 
         Returns:
-            A dictionary containing the MWEs and their association measures.
+            None.
         """
         for sentence in tqdm(self.reader.get_sentences()):
             try:
                 tokens = [
                     word
                     for word in word_tokenize(sentence)
                     if word not in string.punctuation
@@ -164,24 +253,34 @@
                     table_data, headers=headers, tablefmt="double_outline"
                 )
                 sub_tables.append(table_str)
         final_table = "\n\n".join(sub_tables)
         print(final_table)
 
 
-class MWEPatternAssociation:
+class MWEPatternCountAssociation:
     """Extract MWE candidates from a list of tokens based on a given pattern."""
 
-    def __init__(self, association_measure: PMICalculator, custom_pattern: str) -> None:
+    def __init__(
+        self,
+        association_measure: PMICalculator,
+        custom_pattern: str,
+        count_source: dict,
+        mwe_frequency_threshold: int,
+        association_threshold: float,
+    ) -> None:
         """Initializes a new instance of MWEExtractor class.
 
         Args:
             association_measure: An instance of an association measure class.
             custom_pattern: A string pattern to match against the tokens.
                      See the examples of the user-defined patterns below.
+            count_source: A dictionary containing ngram counts.
+            mwe_frequency_threshold: The minimum frequency of an MWE to be considered for extraction.
+            association_threshold: A threshold value for the association measure. Only MWEs with an association measure above this threshold will be returned.
 
             Examples of user-defined patterns:
             - NP: {<DT>?<JJ>*<NN>} # Noun phrase
             - VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
             - PP: {<IN><NP>} # Prepositional phrase
 
             You can use multiple and/or nested patterns, separated by a newline character:
@@ -192,25 +291,27 @@
             ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase
             '''
             In this case, patterns of a clause are executed in order.  An earlier
             pattern may introduce a chunk boundary that prevents a later pattern from executing.
         """
         self.pattern = custom_pattern
         self.association_measure = association_measure
+        self.counts = count_source
+        self.mwe_frequency_threshold = mwe_frequency_threshold
+        self.association_threshold = association_threshold
 
     def _extract_mwe_candidates(self, tokens: list[str]) -> dict:
         """
         Extract variable-length MWE from tokenized input, using a user-defined POS regex pattern.
 
         Args:
             tokens (list[str]): A list of tokens from which mwe candidates are to be extracted.
 
         Returns:
-            match_counter (dict[str, dict[str, int]]): A counter dictionary with count of matched strings, grouped by pattern label.
-                                                    An empty list if none were found.
+            matches
         """
 
         def get_pos_tags(tokens: list[str]) -> list[tuple[str, str]]:
             pos_tags = nltk.pos_tag(tokens)
             return pos_tags
 
         def validate_input() -> None:
@@ -252,25 +353,25 @@
         return matches
 
     def _measure_candidate_association(self, tokens: list[str], threshold: float = 1.0):
         """Measure the association of MWE candidates.
 
         Args:
             tokens: A list of tokens from which mwe candidates are to be extracted.
-            threshold: A threshold value for the association measure. Only MWEs with an association measure above this threshold will be returned.
 
         Returns:
             A dictionary containing the MWEs and their association measures.
         """
         mwes: dict[str, dict[str, float]] = {}
         for mwe_type, candidate_set in self._extract_mwe_candidates(
             tokens=tokens
         ).items():
             if mwe_type not in mwes:
                 mwes[mwe_type] = {}
             for mwe_candidate in candidate_set:
-                association = self.association_measure.compute_association(
-                    mwe_candidate
-                )
-                if association > threshold:
-                    mwes[mwe_type][mwe_candidate] = association
+                if self.counts.get(mwe_candidate, 0) >= self.mwe_frequency_threshold:  # type: ignore
+                    association = self.association_measure.compute_association(
+                        mwe_candidate
+                    )
+                    if association > self.association_threshold:
+                        mwes[mwe_type][mwe_candidate] = association
         return mwes
```

### Comparing `wordview-1.3.0/wordview/preprocessing/cleaning.py` & `wordview-1.4.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/preprocessing/count.py` & `wordview-1.4.0/wordview/preprocessing/count.py`

 * *Files identical despite different names*

### Comparing `wordview-1.3.0/wordview/text_analysis/chat/chat.html` & `wordview-1.4.0/wordview/chat_ui/chat.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,211 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap" rel="stylesheet">
+    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@400;500;700&display=swap" rel="stylesheet">
     <title>Chat Interface</title>
     <style>
         body { 
-            font-family: 'Roboto', sans-serif;
+            font-family: 'Roboto Mono', monospace;
             margin: 0;
             padding: 0;
             display: flex;
             justify-content: center;
             align-items: center;
             height: 100vh;
-            background-color: #f7f7f7;
+            background-color: #b6b6b6;
         }
         .chat-container {
             width: 66%;
             max-width: 800px;
-            background: #fff;
+            background: #374852;
             border-radius: 8px;
             box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
             overflow: hidden;
             display: flex;
             flex-direction: column;
         }
-        .message-container {
+        /* .message-container {
             padding: 20px;
             overflow-y: auto;
             flex-grow: 1;
-            margin-bottom: 10px; /* Adjusted to add space at the bottom */
-        }
+            margin-bottom: 10px;
+        } */
+        .message-container {
+            overflow-y: auto; /* Enables vertical scrolling */
+            max-height: 850px; /* Set a max-height that fits your design */
+            padding: 10px;
+            margin-bottom: 10px;
+            width: 100%; /* Ensure it fills the container */
+            box-sizing: border-box; /* Include padding and border in the width and height */
+            position: relative;
+        }
+        /* Styling the scrollbar itself */
+        .message-container::-webkit-scrollbar {
+            width: 10px; /* Adjust the width of the scrollbar */
+        }
+        /* Styling the track (part the thumb slides within) */
+        .message-container::-webkit-scrollbar-track {
+            background: #f1f1f1; /* Light grey background on the track */
+            border-radius: 10px; /* Rounded corners on the track */
+        }
+
+        /* Styling the thumb (the part that you drag) */
+        .message-container::-webkit-scrollbar-thumb {
+            background: #888; /* Dark grey thumb */
+            border-radius: 10px; /* Rounded corners on the thumb */
+        }
+
+        /* Handle on hover */
+        .message-container::-webkit-scrollbar-thumb:hover {
+            background: #555; /* Darker grey on hover */
+        }
+
+
+
+
+        /* Standard Oval Style of Message Bubbles */
+        /*
         .message {
             margin-bottom: 12px;
             padding: 10px;
             border-radius: 20px;
             color: #333;
             font-size: 14px;
             line-height: 1.4;
-            width: fit-content; /* Makes messages not stretch full width */
+            width: fit-content;
         }
-        /* Bot messages */
         .bot {
-            background-color: #E7F3FF; /* Soft blue for AI responses */
+            background-color: #E7F3FF;
             align-self: flex-start;
-            margin: 0 0 12px 20px; /* Adjust if needed to fine-tune the spacing */
+            margin: 0 0 12px 20px;
             border-radius: 20px;
             padding: 10px;
             max-width: 80%;
-            border: 1px solid #BDDFFF; /* Slightly darker blue for border */
+            border: 1px solid #BDDFFF;
         }
-        /* User messages */
         .user {
-            background-color: #DCF8C6; /* Keep the light green for user messages */
+            background-color: #DCF8C6;
             align-self: flex-end;
-            margin: 0 20px 12px 0; /* Adjust if needed for spacing */
+            margin: 0 20px 12px 0;
             border-radius: 20px;
             padding: 10px;
             max-width: 80%;
-            border: 1px solid #C4E6B0; /* Slightly darker green for border */
+            border: 1px solid #C4E6B0;
         }
         .input-container {
             display: flex;
             padding: 10px;
             border-top: 1px solid #eee;
-            align-items: center; /* Ensures vertical alignment */
+            align-items: center;
         }
         input[type="text"] {
             flex-grow: 1;
             border: 1px solid #ddd;
             border-radius: 20px;
             padding: 10px;
             margin-right: 8px;
             outline: none;
             font-size: 14px;
         }
-        button {
+        */
+
+        .message {
+            font-size: 16px; /* Adjusted to match your style preference */
+            line-height: 1.4;
+            border-radius: 8px; /* Rounded corners for the chat bubbles */
+            padding: 10px 15px;
+            margin: 8px 20px;
+            max-width: 80%;
+            width: fit-content;
+            background-color: transparent; /* Making bubble background transparent */
+            border: 1px solid rgba(0, 0, 0, 0.1); /* Optional: subtle border for definition */
+        }
+
+        .user {
+            color: #25d4c8; /* Teal color for user messages */
+            border: 1px solid #25d4c8;
+            align-self: flex-end;
+        }
+
+        .bot {
+            color: #05c729; /* Soft Coral color for bot messages */
+            border: 1px solid #05c729;
+            align-self: flex-start;
+        }
+
+        input[type="text"] {
+            flex-grow: 1;
+            border: 1px solid #b9b8b8; /* Subtle border for definition */
+            border-radius: 8px; /* Matches the message bubbles */
+            padding: 10px; /* Adequate padding for text */
+            margin-right: 8px; /* Space between the input field and the send button */
+            outline: none; /* Removes the default focus outline */
+            font-size: 14px; /* Matching the text size of messages */
+            background-color: #f1eeee; /* Ensures the input background is white or matches the chat UI */
+        }
+
+        .input-container {
+            display: flex;
+            padding: 10px; /* Padding inside the container holding the input */
+            border-top: 1px solid #eee; /* A subtle border at the top separating messages from input */
+            background-color: #f1eeee; /* A slight off-white background for the input area */
+            align-items: center; /* Centers the input and button vertically */
+        }
+
+        /* Oval Button */
+        /* button {
             background-color: #007bff;
             color: white;
             border: none;
             border-radius: 20px;
             padding: 10px 20px;
             font-size: 14px;
             cursor: pointer;
             outline: none;
+        } */
+        /* Arrow Button */
+        button {
+            background-color: transparent; /* Remove background color for a cleaner look */
+            color: #007bff; /* Color of the arrow */
+            border: none;
+            border-radius: 50%; /* Make it round */
+            padding: 10px 12px;
+            font-size: 24px;
+            cursor: pointer;
+            outline: none;
+            transition: background-color 0.3s; /* Smooth transition for hover effect */
         }
         button:hover {
-            background-color: #0056b3;
+            background-color: #f0f0f0;
         }
-        ::-webkit-scrollbar {
+        /* ::-webkit-scrollbar {
             width: 5px;
         }
         ::-webkit-scrollbar-track {
             background: #f1f1f1;
         }
         ::-webkit-scrollbar-thumb {
             background: #888;
-        }
-        ::-webkit-scrollbar-thumb:hover {
+        } */
+        /* ::-webkit-scrollbar-thumb:hover {
             background: #555;
-        }
+        } */
     </style>    
 </head>
 <body>
     <div class="chat-container">
         <div class="message-container" id="chatContainer">
             <!-- Messages will be dynamically added here -->
         </div>
         <div class="input-container">
             <input type="text" id="userInput" placeholder="Type your message here...">
-            <button onclick="sendMessage()">Send</button>
+            <button onclick="sendMessage()">➜</button>
         </div>
     </div>
     
     <script>
         document.getElementById('userInput').addEventListener('keypress', function(e) {
             if (e.key === 'Enter') {
                 e.preventDefault(); // Prevent the default action to stop it from submitting a form if any
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1 +1 @@
-[                    ]Send
+[                    ]➜
```

### Comparing `wordview-1.3.0/wordview/text_analysis/core.py` & `wordview-1.4.0/wordview/text_analysis/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import nltk
 import numpy as np
 import pandas as pd
 import plotly
 import plotly.graph_objs as go
 from langdetect import detect
 from nltk.corpus import stopwords
-from nltk.tokenize import sent_tokenize
+from nltk.tokenize import sent_tokenize, word_tokenize
 from plotly.subplots import make_subplots
 from tqdm import tqdm
 from wordcloud import WordCloud, get_single_color_func
 
 from bin.nltk_resources import check_nltk_resources
 from wordview import logger
 
@@ -333,33 +333,38 @@
     languages = set()
 
     logger.info("Processing text in %s column of the input DataFrame..." % text_col)
     for text in tqdm(df[text_col]):
         ls = detect(text).upper()
         languages.update([ls])
         try:
-            tokens = text.lower().split(" ")
-            doc_lengths.append(len(tokens))
+            doc_len = 0
+            doc_tokens = []
             sentences = sent_tokenize(text.lower())
             for sentence in sentences:
-                sentence_tokens = sentence.split(" ")
+                sentence_tokens = word_tokenize(sentence)
                 sentence_lengths.append(len(sentence_tokens))
+                doc_len += len(sentence_tokens)
+                doc_tokens.extend(sentence_tokens)
+            doc_lengths.append(doc_len)
             if skip_stopwords_punc:
-                tokens = [
-                    t for t in tokens if t not in stop_words and t not in punctuations
+                doc_tokens = [
+                    t
+                    for t in doc_tokens
+                    if t not in stop_words and t not in punctuations
                 ]
-                update_count(token_to_count_dict, tokens)
+                update_count(token_to_count_dict, doc_tokens)
 
         except Exception as e:
             logger.warning(
                 "Processing entry --- %s --- lead to exception: %s" % (text, e.args[0])
             )
             continue
 
-        postag_tokens = nltk.pos_tag(tokens)
+        postag_tokens = nltk.pos_tag(doc_tokens)
 
         for pos in pos_tags:
             pos_items = get_pos(postag_tokens, pos)
             update_count(word_count_by_pos[pos], pos_items)
 
     freq_df = pd.DataFrame(
         {"tokens": token_to_count_dict.keys(), "count": token_to_count_dict.values()}
```

### Comparing `wordview-1.3.0/wordview/text_analysis/wrapper.py` & `wordview-1.4.0/wordview/text_analysis/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,24 +114,24 @@
         base_content = f"""Answer any questions about text and corpus analysis based on the following dictionary of Wordview Analysis.
         \n\n
         ------------------------------
         Wordview Analysis:
         ------------------------------
         {self.return_stats()}
         \n\n
-        Answer the questions without adding According to or Based on to the Wordview Analysis dictionary.
+        Do NOT say according to Wordview Analysis dictionary.
         """
         chat_history = [
             {"role": "system", "content": base_content},
         ]
         app = Flask(__name__, static_folder="path_to_your_ui_folder")
 
         @app.route("/")
         def index():
-            return send_from_directory("chat", "chat.html")
+            return send_from_directory("../chat_ui", "chat.html")
 
         @app.route("/chat", methods=["POST"])
         def chat():
             user_input = request.json["message"]
             chat_history.append({"role": "user", "content": user_input})
             response = (
                 self.chat_client.chat.completions.create(
```

### Comparing `wordview-1.3.0/PKG-INFO` & `wordview-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 1.3.0
+Version: 1.4.0
 Summary: Wordview is a Python package for Exploratory Data Analysis of text and provides many statistics about your data in the form of plots, tables, and descriptions allowing you to have both a high-level and detailed overview of your data.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

