# Comparing `tmp/rst2dep-1.2.0.1.tar.gz` & `tmp/rst2dep-1.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rst2dep-1.2.0.1.tar", last modified: Thu Feb 29 19:27:51 2024, max compression
+gzip compressed data, was "rst2dep-1.2.1.0.tar", last modified: Tue Apr  9 19:17:23 2024, max compression
```

## Comparing `rst2dep-1.2.0.1.tar` & `rst2dep-1.2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 19:27:51.983967 rst2dep-1.2.0.1/
--rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.2.0.1/LICENSE
--rw-rw-rw-   0        0        0      780 2024-02-29 19:27:51.983967 rst2dep-1.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7271 2024-02-29 19:25:34.000000 rst2dep-1.2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 19:27:51.971788 rst2dep-1.2.0.1/rst2dep/
--rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.2.0.1/rst2dep/GUM_academic_census.rs4
--rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.2.0.1/rst2dep/__init__.py
--rw-rw-rw-   0        0        0     3019 2024-02-29 19:21:04.000000 rst2dep-1.2.0.1/rst2dep/__main__.py
--rw-rw-rw-   0        0        0    24689 2023-10-26 19:38:49.000000 rst2dep-1.2.0.1/rst2dep/classes.py
--rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.2.0.1/rst2dep/dep2rst.py
--rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.2.0.1/rst2dep/example.conllu
--rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.2.0.1/rst2dep/example.rs3
--rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.2.0.1/rst2dep/example.rsd
--rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.2.0.1/rst2dep/feature_extraction.py
--rw-rw-rw-   0        0        0     3840 2024-02-26 15:24:31.000000 rst2dep-1.2.0.1/rst2dep/four_units.rs4
--rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.2.0.1/rst2dep/four_units.rsd
--rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.2.0.1/rst2dep/four_units.txt
--rw-rw-rw-   0        0        0    16500 2024-02-29 19:12:01.000000 rst2dep-1.2.0.1/rst2dep/rst2dep.py
--rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.2.0.1/rst2dep/run_tests.py
--rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.2.0.1/rst2dep/salinity_chain.rsd
--rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.2.0.1/rst2dep/salinity_li.rsd
-drwxrwxrwx   0        0        0        0 2024-02-29 19:27:51.983967 rst2dep-1.2.0.1/rst2dep.egg-info/
--rw-rw-rw-   0        0        0      780 2024-02-29 19:27:51.000000 rst2dep-1.2.0.1/rst2dep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-02-29 19:27:51.000000 rst2dep-1.2.0.1/rst2dep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 19:27:51.000000 rst2dep-1.2.0.1/rst2dep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-29 19:27:51.000000 rst2dep-1.2.0.1/rst2dep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 19:27:51.983967 rst2dep-1.2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-02-29 19:21:25.000000 rst2dep-1.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.998139 rst2dep-1.2.1.0/
+-rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      762 2024-04-09 19:17:22.997138 rst2dep-1.2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7680 2024-04-09 15:29:13.000000 rst2dep-1.2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.990139 rst2dep-1.2.1.0/rst2dep/
+-rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.2.1.0/rst2dep/GUM_academic_census.rs4
+-rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.2.1.0/rst2dep/__init__.py
+-rw-rw-rw-   0        0        0     3091 2024-04-09 19:13:59.000000 rst2dep-1.2.1.0/rst2dep/__main__.py
+-rw-rw-rw-   0        0        0    24689 2023-10-26 19:38:49.000000 rst2dep-1.2.1.0/rst2dep/classes.py
+-rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.2.1.0/rst2dep/dep2rst.py
+-rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.2.1.0/rst2dep/example.conllu
+-rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.2.1.0/rst2dep/example.rs3
+-rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.2.1.0/rst2dep/example.rsd
+-rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.2.1.0/rst2dep/feature_extraction.py
+-rw-rw-rw-   0        0        0     3897 2024-04-09 14:58:00.000000 rst2dep-1.2.1.0/rst2dep/four_units.rs4
+-rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.2.1.0/rst2dep/four_units.rsd
+-rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.2.1.0/rst2dep/four_units.txt
+-rw-rw-rw-   0        0        0    16922 2024-04-09 15:25:37.000000 rst2dep-1.2.1.0/rst2dep/rst2dep.py
+-rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.2.1.0/rst2dep/run_tests.py
+-rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.2.1.0/rst2dep/salinity_chain.rsd
+-rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.2.1.0/rst2dep/salinity_li.rsd
+drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.996148 rst2dep-1.2.1.0/rst2dep.egg-info/
+-rw-rw-rw-   0        0        0      762 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:17:22.999138 rst2dep-1.2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-04-09 19:13:45.000000 rst2dep-1.2.1.0/setup.py
```

### Comparing `rst2dep-1.2.0.1/LICENSE` & `rst2dep-1.2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/PKG-INFO` & `rst2dep-1.2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rst2dep
-Version: 1.2.0.1
+Version: 1.2.1.0
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.1.0
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.0.1
-Description: UNKNOWN
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
```

### Comparing `rst2dep-1.2.0.1/README.md` & `rst2dep-1.2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 2. Run `> python setup.py install`
 
 You can also download the scripts and manually run scripts (rst2dep.py, dep2rst.py, etc.), but you won't be able to run it as a module or import easily as shown below.
 
 ## Usage
 
 ```
-usage: python -m rst2dep [-h] [-c ROOT] [-p] [-f {rsd,conllu,rs3,rs4}] [-d {ltr,rtl,dist}] [-r] infiles
+usage: python -m rst2dep [-h] [-c ROOT] [-p] [-s] [-a {li,chain,hirao}] [-f {rsd,conllu,rs3,rs4}] [-d {ltr,rtl,dist}] [-r] infiles
 
 positional arguments:
   infiles               file name or glob pattern, e.g. *.rs3
 
 optional arguments:
   -h, --help            show this help message and exit
   -c ROOT, --corpus_root ROOT
@@ -34,15 +34,15 @@
   -f {rsd,conllu,rs3,rs4}, --format {rsd,conllu,rs3,rs4}
                         input format
   -d {ltr,rtl,dist}, --depth {ltr,rtl,dist}
                         how to order depth
   -r, --rels            use DEFAULT_RELATIONS for the .rs3 header instead of rels in input data
   -a {li,chain,hirao}, --algorithm {li,chain,hirao}
                         dependency head algorithm (default: li)
-  -s, --same_unit       retain same-unit multinucs in hirao algorithm
+  -s, --same_unit       retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain
 ```
 
 If you have installed the library you can run the converter directly on the commandline with the options you want like this:
 
 ```
 python -m rst2dep -p -f rs3 example.rs3
 ```
@@ -65,15 +65,15 @@
 
 ## Details
 
 ### rst2dep
 
 The default conversion follows Li et al.'s (2013) convention of taking the left-most child of multinuclear relations as the head child governed by the relation applied to the whole multinuc, and attaching each subsequent multinuclear child to the first child using the multinuclear relation; thus if a contrast multinuc with units [2-3] is an elaboration on unit [1], the child [2] will become an elaboration dependent of [1], and [3] will become a contrast dependent of child [2]. An alternative algorithm implementing a chain conversion where multinuc children become dependents of their most recent sibling, instead of the leftmost sibling, is also available (use `--algorithm=chain`), as is the Hirao et al. (2014) algorithm (`--algorithm=hirao`), which attaches all multinuc children to the parent of the multinuc, using the relation of the multinuc as a whole. 
 
-For the Hirao et al. algorithm note that no multinuclear relations will be retained in the output, since they will be recursively replaced with whatever satellite relation governs their parent; also note that this means that there could be multiple ROOT nodes (all multinuc children of the document root), and  "same-unit" relations will be destroyed in the same manner. To exceptionally keep same-unit multinucs in the Hirao et al. conversion, use the option `--same_unit`.
+For the Hirao et al. algorithm note that no multinuclear relations will be retained in the output, since they will be recursively replaced with whatever satellite relation governs their parent; also note that this means that there could be multiple ROOT nodes (all multinuc children of the document root), and  "same-unit" relations will be destroyed in the same manner. To exceptionally keep same-unit multinucs in the Hirao et al. conversion, use the option `--same_unit`. The same option can be used in the Chain algorithm to exceptionally convert "same-unit" relations according to the Li et al. algorithm (i.e. same-unit children all attach to the leftmost child of the same-unit multinuclear node, but satellites of all other multinuclear node types attach in a chain to the most recent multinuclear child).
 
 By convention, multinuclear relations are converted with relation names ending in `_m`, while satellite RST relations are converted with names ending in `_r`. The original nesting depth is ignored in the conversion, but attachment point height for each dependent is retained in the third column of the output file, allowing deterministic reconstruction of the constituent tree using dep2rst, assuming a projective, hierarchically ordered tree with the Li et al. algorithm (other algorithms are not guaranteed to be reversible). Conversion of non-projective .rs3 constituent trees to dependencies is also supported, but cannot be reversed currently.
 
 Optionally, users can also specify an additional folder containing subfolders `dep/` and `xml/` with .conllu parses and [GUM](https://gucorpling.org/gum/) style XML to add features to the output file. 
 
 
 ### dep2rst
```

### Comparing `rst2dep-1.2.0.1/rst2dep/GUM_academic_census.rs4` & `rst2dep-1.2.1.0/rst2dep/GUM_academic_census.rs4`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/__main__.py` & `rst2dep-1.2.1.0/rst2dep/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from .rst2dep import make_rsd
 from .dep2rst import rsd2rs3, conllu2rsd
 from argparse import ArgumentParser
 import sys, os, io
 
 def run_conversion():
-    parser = ArgumentParser(usage="python -m rst2dep [-h] [-c ROOT] [-p] [-f {rsd,conllu,rs3,rs4}] [-d {ltr,rtl,dist}] [-r] infiles")
+    parser = ArgumentParser(usage="python -m rst2dep [-h] [-c ROOT] [-p] [-s] [-a {li,hirao,chain}] [-f {rsd,conllu,rs3,rs4}] [-d {ltr,rtl,dist}] [-r] infiles")
     parser.add_argument("infiles", action="store", help="file name or glob pattern, e.g. *.rs3")
     parser.add_argument("-c", "--corpus_root", action="store", dest="root", default="",
                         help="optional: path to corpus root folder containing a directory dep/ and \n" +
                              "a directory xml/ containing additional corpus formats")
     parser.add_argument("-p", "--print", dest="prnt", action="store_true", help="print output instead of serializing to a file")
     parser.add_argument("-f", "--format", choices=["rsd", "conllu", "rs3", "rs4"], default="rs3", help="input format")
     parser.add_argument("-d", "--depth", choices=["ltr", "rtl", "dist"], default="dist", help="how to order depth")
     parser.add_argument("-r", "--rels", action="store_true", help="use DEFAULT_RELATIONS for the .rs3 header instead of rels in input data")
     parser.add_argument("-a","--algorithm",choices=["li","chain","hirao"],help="dependency head algorithm (default: li)",default="li")
-    parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm")
+    parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain")
 
     options = parser.parse_args()
 
     inpath = options.infiles
 
     if "*" in inpath:
         from glob import glob
@@ -55,9 +55,10 @@
 
             if options.prnt:
                 print(output)
             else:
                 with open("output" + os.sep + os.path.basename(file_).replace(".rsd",".rs3").replace(".conllu",".rs3"),'w',encoding="utf8",newline="\n") as f:
                     f.write(output)
 
+
 if __name__ == "__main__":
-    run_conversion()
+    run_conversion()
```

### Comparing `rst2dep-1.2.0.1/rst2dep/classes.py` & `rst2dep-1.2.1.0/rst2dep/classes.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/dep2rst.py` & `rst2dep-1.2.1.0/rst2dep/dep2rst.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/example.conllu` & `rst2dep-1.2.1.0/rst2dep/example.conllu`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/example.rs3` & `rst2dep-1.2.1.0/rst2dep/example.rs3`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/example.rsd` & `rst2dep-1.2.1.0/rst2dep/example.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/feature_extraction.py` & `rst2dep-1.2.1.0/rst2dep/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/four_units.rs4` & `rst2dep-1.2.1.0/rst2dep/four_units.rs4`

 * *Files 2% similar despite different names*

```diff
@@ -32,34 +32,35 @@
 			<rel name="restatement-repetition" type="multinuc"/>
 			<rel name="same-unit" type="multinuc"/>
 			<rel name="topic-question" type="rst"/>
 			<rel name="topic-solutionhood" type="rst"/>
 		</relations>
 		<sigtypes>
 			<sig type="dm" subtypes="dm"/>
-			<sig type="reference" subtypes="comparative_reference;demonstrative_reference;personal_reference;propositional_reference"/>
+			<sig type="genre" subtypes="inverted_pyramid_scheme;layout;newspaper_style_attribution;newspaper_style_definition"/>
+			<sig type="graphical" subtypes="colon;dash;items_in_sequence;parentheses;question_mark;semicolon"/>
+			<sig type="graphical+syntactic" subtypes="comma+past_participial_clause;comma+present_participial_clause"/>
 			<sig type="lexical" subtypes="alternate_expression;indicative_phrase;indicative_word"/>
-			<sig type="semantic" subtypes="antonymy;general_word;indicative_word_pair;lexical_chain;meronymy;repetition;synonymy"/>
+			<sig type="lexical+syntactic" subtypes="indicative_word+present_participial_clause"/>
 			<sig type="morphological" subtypes="tense"/>
-			<sig type="syntactic" subtypes="adjectival_modifier;imperative_clause;infinitival_clause;interrupted_matrix_clause;nominal_modifier;parallel_syntactic_construction;past_participial_clause;present_participial_clause;relative_clause;reported_speech;subject_auxiliary_inversion"/>
-			<sig type="graphical" subtypes="colon;dash;items_in_sequence;parentheses;question_mark;semicolon"/>
-			<sig type="genre" subtypes="inverted_pyramid_scheme;layout;newspaper_style_attribution;newspaper_style_definition"/>
 			<sig type="numerical" subtypes="same_count"/>
+			<sig type="orphan" subtypes="orphan"/>
+			<sig type="reference" subtypes="comparative_reference;demonstrative_reference;personal_reference;propositional_reference"/>
 			<sig type="reference+syntactic" subtypes="comparative_reference+subject np;demonstrative_reference+subject np;personal_reference+subject np;propositional_reference+subject np"/>
+			<sig type="semantic" subtypes="antonymy;general_word;indicative_word_pair;lexical_chain;meronymy;repetition;synonymy"/>
 			<sig type="semantic+syntactic" subtypes="general_word+subject np;lexical_chain+subject np;meronymy+subject np;repetition+subject np;synonymy+subject np"/>
-			<sig type="lexical+syntactic" subtypes="indicative_word+present_participial_clause"/>
+			<sig type="syntactic" subtypes="adjectival_modifier;imperative_clause;infinitival_clause;interrupted_matrix_clause;nominal_modifier;parallel_syntactic_construction;past_participial_clause;present_participial_clause;relative_clause;reported_speech;subject_auxiliary_inversion"/>
 			<sig type="syntactic+positional" subtypes="past_participial_clause+beginning;present_participial_clause+beginning"/>
 			<sig type="syntactic+semantic" subtypes="parallel_syntactic_construction+lexical_chain"/>
-			<sig type="graphical+syntactic" subtypes="comma+past_participial_clause;comma+present_participial_clause"/>
 			<sig type="unsure" subtypes="unsure"/>
-			<sig type="orphan" subtypes="orphan"/>
 		</sigtypes>
 	</header>
 	<body>
 		<segment id="1" parent="6" relname="span">This is a unit.</segment>
-		<segment id="2" parent="5" relname="joint-list">Specifically we must X,</segment>
-		<segment id="3" parent="5" relname="joint-list">and Y</segment>
-		<segment id="4" parent="5" relname="joint-list">and also Z.</segment>
-		<group id="5" type="multinuc" parent="1" relname="elaboration-additional"/>
+		<segment id="2" parent="5" relname="same-unit">Specifically we must X,</segment>
+		<segment id="3" parent="5" relname="same-unit">and Y</segment>
+		<segment id="4" parent="5" relname="causal-result">and also Z.</segment>
+		<group id="5" type="multinuc" parent="7" relname="span"/>
 		<group id="6" type="span" />
+		<group id="7" type="span" parent="1" relname="elaboration-additional"/>
 	</body>
 </rst>
```

### Comparing `rst2dep-1.2.0.1/rst2dep/rst2dep.py` & `rst2dep-1.2.1.0/rst2dep/rst2dep.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,52 +16,54 @@
 
 # Add hardwired genre identifiers which appear as substring in filenames here
 GENRES = {"_news_":"news","_whow_":"whow","_voyage_":"voyage","_interview_":"interview",
           "_bio_":"bio","_fiction_":"fiction","_academic_":"academic","_reddit_":"reddit",
           "_speech_":"speech","_textbook_":"textbook","_vlog_":"vlog","_conversation_":"conversation",}
 
 
-def find_dep_head(nodes, source, exclude, block, initial_deprel, algorithm="li"):
+def find_dep_head(nodes, source, exclude, block, initial_deprel, algorithm="li", keep_same_unit=False):
     parent = nodes[source].parent
     if parent != "0":
         if nodes[parent].kind == "multinuc":
             for child in nodes[parent].children:
                 # Check whether exclude and child are under the same multinuc and exclude is further to the left
                 if nodes[child].left > int(exclude) and nodes[child].left >= nodes[parent].left and int(exclude) >= nodes[parent].left:
                     block.append(child)
     else:
         # Prevent EDU children of root from being dep head - only multinuc children possible at this point
         for child in nodes[source].children:
             if nodes[child].kind == "edu":
                 block.append(child)
-    candidate = seek_other_edu_child(nodes, nodes[source].parent, exclude, block, initial_deprel, algorithm=algorithm)
+    candidate = seek_other_edu_child(nodes, nodes[source].parent, exclude, block, initial_deprel, algorithm=algorithm, keep_same_unit=keep_same_unit)
     if candidate is not None:
         return candidate
     else:
         if parent == "0":
             return None
         else:
             if parent not in nodes:
                 raise IOError("Node with id " + source + " has parent id " + parent + " which is not listed\n")
-            return find_dep_head(nodes, parent, exclude, block, initial_deprel, algorithm=algorithm)
+            return find_dep_head(nodes, parent, exclude, block, initial_deprel, algorithm=algorithm, keep_same_unit=keep_same_unit)
 
 
-def seek_other_edu_child(nodes, source, exclude, block, initial_deprel, algorithm="li"):
+def seek_other_edu_child(nodes, source, exclude, block, initial_deprel, algorithm="li", keep_same_unit=False):
     """
     Recursive function to find some child of a node which is an EDU and does not have the excluded ID
 
     :param nodes: dictionary of IDs to NODE objects
     :param source: the source node from which to traverse
     :param exclude: node ID to exclude as target child
     :param block: list of IDs for which children should not be traversed (multinuc right children)
     :param initial_deprel: the original dependency relation of the node triggering the search (needed for algo != li)
     :param algorithm: the algorithm to use for dependency head selection, one of {li,chain,hirao}
     :return: the found child ID or None if none match
     """
 
+    #if nodes[source].left == 43:
+    #    a=4
     if source == "0":
         return None
     else:
         # Check if this is already an EDU
         if nodes[source].kind == "edu" and source != exclude and source not in block:
             return source
         # Loop through children of this node
@@ -85,31 +87,31 @@
                     #not (nodes[child_id].parent == nodes[exclude].parent and nodes[source].kind == "multinuc" and int(child_id) > int(exclude)):  # preclude right pointing rel between multinuc siblings
                 return child_id
             # Found a non-terminal child
             elif child_id != exclude:
                 # If it's a span, check below it, following only span relation paths
                 if nodes[source].kind == "span":
                     if nodes[child_id].relname == "span":
-                        candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm)
+                        candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm, keep_same_unit=keep_same_unit)
                         if candidate is not None:
                             return candidate
                 # If it's a multinuc...
                 elif nodes[source].kind == "multinuc":
-                    if algorithm in ["li","hirao"] or initial_deprel.endswith("_r"):
+                    if algorithm in ["li","hirao"] or initial_deprel.endswith("_r") or (keep_same_unit and "sameunit" in nodes[child_id].relname.lower().replace("_","").replace("-","")):
                         # In Li et al. conversion, only consider the left most child as representing the multinuc topologically
                         if child_id == nodes[source].leftmost_child:
-                            candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm)
+                            candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm, keep_same_unit=keep_same_unit)
                             if candidate is not None:
                                 return candidate
                     elif algorithm == "chain":  # In chain conversion, consider next multinuc child, which should already be sorted
                         if nodes[child_id].dep_rel.endswith("_r") and nodes[child_id].parent == source and not nodes[nodes[child_id].parent].leftmost_child == child_id:
                             # Do not allow traversing against the direction of a satellite relation
                             continue
                         if child_id == left_sibling_id or source != nodes[exclude].parent:
-                            candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm)
+                            candidate = seek_other_edu_child(nodes, child_id, exclude, block, initial_deprel, algorithm=algorithm, keep_same_unit=keep_same_unit)
                             if candidate is not None:
                                 return candidate
     return None
 
 
 def get_distance(node, parent, nodes):
     head = node.parent
@@ -249,15 +251,15 @@
                 new_rel = new_rel.relname
         node.dep_rel = new_rel
         if len(sigs) > 0:
             node.signals = sigs
 
     for nid in nodes:
         node = nodes[nid]
-        dep_parent = find_dep_head(nodes, nid, nid, [], node.dep_rel, algorithm=algorithm)
+        dep_parent = find_dep_head(nodes, nid, nid, [], node.dep_rel, algorithm=algorithm, keep_same_unit=keep_same_unit)
         if dep_parent is None:
             # This is the root
             dep_parent = "0"
         if node.kind == "edu":
             if dep_parent == "0":
                 node.dep_rel = "ROOT"
             node.dep_parent = dep_parent
@@ -348,15 +350,15 @@
             "python rst2dep.py <INFILES>"
     parser = ArgumentParser(description=desc)
     parser.add_argument("infiles",action="store",help="file name or glob pattern, e.g. *.rs3")
     parser.add_argument("-c","--corpus_root",action="store",dest="root",default="",help="optional: path to corpus root folder containing a directory dep/ and \n"+
                                                            "a directory xml/ containing additional corpus formats")
     parser.add_argument("-p","--print",dest="prnt",action="store_true",help="print output instead of serializing to a file")
     parser.add_argument("-a","--algorithm",choices=["li","chain","hirao"],help="dependency head algorithm (default: li)",default="li")
-    parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm")
+    parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain")
 
     options = parser.parse_args()
 
     inpath = options.infiles
 
     if "*" in inpath:
         from glob import glob
```

### Comparing `rst2dep-1.2.0.1/rst2dep/salinity_chain.rsd` & `rst2dep-1.2.1.0/rst2dep/salinity_chain.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep/salinity_li.rsd` & `rst2dep-1.2.1.0/rst2dep/salinity_li.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/rst2dep.egg-info/PKG-INFO` & `rst2dep-1.2.1.0/rst2dep.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: rst2dep
-Version: 1.2.0.1
+Version: 1.2.1.0
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.1.0
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.0.1
-Description: UNKNOWN
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
```

### Comparing `rst2dep-1.2.0.1/rst2dep.egg-info/SOURCES.txt` & `rst2dep-1.2.1.0/rst2dep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.0.1/setup.py` & `rst2dep-1.2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rst2dep',
   packages = find_packages(),
-  version = '1.2.0.1',
+  version = '1.2.1.0',
   description = 'RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   package_data = {'':['README.md','LICENSE','requirements.txt'],'rst2dep':['*']},
   install_requires=[],
   url = 'https://github.com/amir-zeldes/rst2dep',
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.0.1',
+  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.1.0',
   keywords = ['NLP', 'RST', 'discourse', 'dependencies', 'converter', 'conversion','Rhetorical Structure Theory','parsing'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

