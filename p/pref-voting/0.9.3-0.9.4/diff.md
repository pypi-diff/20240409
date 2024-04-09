# Comparing `tmp/pref_voting-0.9.3.tar.gz` & `tmp/pref_voting-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.9.3.tar", max compression
+gzip compressed data, was "pref_voting-0.9.4.tar", max compression
```

## Comparing `pref_voting-0.9.3.tar` & `pref_voting-0.9.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.3/LICENSE
--rw-r--r--   0        0        0     3940 2024-03-19 19:30:31.741533 pref_voting-0.9.3/README.md
--rw-r--r--   0        0        0       22 2024-03-24 12:47:05.771993 pref_voting-0.9.3/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.3/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.3/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.3/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.3/pref_voting/axioms.py
--rw-r--r--   0        0        0    31422 2024-03-19 01:31:26.659805 pref_voting-0.9.3/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.3/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.3/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    22821 2024-02-18 15:20:46.307786 pref_voting-0.9.3/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.3/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.3/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.3/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.3/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.3/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     7381 2024-03-02 21:50:31.230170 pref_voting-0.9.3/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.3/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.3/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    16728 2024-03-19 21:10:58.370606 pref_voting-0.9.3/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9046 2024-03-19 18:47:57.579346 pref_voting-0.9.3/pref_voting/io/writers.py
--rw-r--r--   0        0        0    89656 2024-03-15 21:02:37.621434 pref_voting-0.9.3/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.3/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22546 2024-02-19 22:05:43.231361 pref_voting-0.9.3/pref_voting/mappings.py
--rw-r--r--   0        0        0    69328 2024-03-24 12:46:34.602418 pref_voting-0.9.3/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    32539 2024-02-11 14:13:54.257214 pref_voting-0.9.3/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.3/pref_voting/other_methods.py
--rw-r--r--   0        0        0     4208 2024-03-19 01:40:26.748429 pref_voting-0.9.3/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.3/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.3/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.3/pref_voting/rankings.py
--rw-r--r--   0        0        0    19338 2024-03-17 10:25:26.075343 pref_voting-0.9.3/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1432 2024-02-18 15:58:01.798373 pref_voting-0.9.3/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.3/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.3/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.3/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.3/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.3/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.3/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     7778 2024-03-21 10:44:35.625747 pref_voting-0.9.3/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.3/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-03-21 10:30:56.840551 pref_voting-0.9.3/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     5459 2024-03-21 21:04:51.742423 pref_voting-0.9.3/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-03-21 21:05:45.274545 pref_voting-0.9.3/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.3/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-03-21 00:53:24.052619 pref_voting-0.9.3/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3924 2024-03-19 18:13:23.959157 pref_voting-0.9.3/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.3/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.3/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.3/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    52062 2023-12-13 22:47:24.616165 pref_voting-0.9.3/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.3/pref_voting/voting_method.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.3/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-03-21 10:24:43.130670 pref_voting-0.9.3/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      759 2024-03-24 12:47:05.770446 pref_voting-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 pref_voting-0.9.3/setup.py
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 pref_voting-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3940 2024-03-19 19:30:31.741533 pref_voting-0.9.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 01:52:38.732190 pref_voting-0.9.4/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.4/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.4/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.4/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.4/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33153 2024-04-09 01:46:10.634579 pref_voting-0.9.4/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.4/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.4/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    22821 2024-02-18 15:20:46.307786 pref_voting-0.9.4/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.4/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.4/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.4/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.4/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.4/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     7381 2024-03-02 21:50:31.230170 pref_voting-0.9.4/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.4/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.4/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    16728 2024-03-19 21:10:58.370606 pref_voting-0.9.4/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9046 2024-03-19 18:47:57.579346 pref_voting-0.9.4/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    89656 2024-03-15 21:02:37.621434 pref_voting-0.9.4/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.4/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22546 2024-02-19 22:05:43.231361 pref_voting-0.9.4/pref_voting/mappings.py
+-rw-r--r--   0        0        0    69328 2024-04-08 19:41:37.247038 pref_voting-0.9.4/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    32539 2024-02-11 14:13:54.257214 pref_voting-0.9.4/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.4/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     4208 2024-03-19 01:40:26.748429 pref_voting-0.9.4/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.4/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.4/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.4/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21026 2024-04-09 01:46:10.635021 pref_voting-0.9.4/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1432 2024-02-18 15:58:01.798373 pref_voting-0.9.4/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.4/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.4/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.4/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.4/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.4/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.4/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-0.9.4/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.4/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-0.9.4/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-0.9.4/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-0.9.4/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.4/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-0.9.4/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-0.9.4/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.4/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.4/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.4/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    52062 2023-12-13 22:47:24.616165 pref_voting-0.9.4/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.4/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.4/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-0.9.4/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      759 2024-04-09 01:52:38.731193 pref_voting-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 pref_voting-0.9.4/setup.py
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 pref_voting-0.9.4/PKG-INFO
```

### Comparing `pref_voting-0.9.3/LICENSE` & `pref_voting-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/README.md` & `pref_voting-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/analysis.py` & `pref_voting-0.9.4/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/axiom.py` & `pref_voting-0.9.4/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/c1_methods.py` & `pref_voting-0.9.4/pref_voting/c1_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Implementations of voting methods that work on both profiles and majority graphs.
 '''
 
 from pref_voting.voting_method import  *
 from pref_voting.helper import get_mg, get_weak_mg
 from pref_voting.margin_based_methods import distance_to_margin_graph
 from pref_voting.probabilistic_methods import c1_maximal_lottery
+from pref_voting.rankings import Ranking, break_ties_alphabetically
 import copy
 import math
 from itertools import product, permutations, combinations, chain
 import networkx as nx
 import matplotlib.pyplot as plt
 
 @vm(name = "Condorcet")
@@ -106,14 +107,47 @@
 
 
     """    
     c_scores = edata.copeland_scores(curr_cands = curr_cands)
     max_score = max(c_scores.values())
     return sorted([c for c in c_scores.keys() if c_scores[c] == max_score])
 
+@swf(name = "Copeland ranking")
+def copeland_ranking(edata, curr_cands=None, local=True, tie_breaking=None):
+    """The SWF that ranks candidates by their Copeland scores. If local is True, then the Copeland scores are computed with respect to the profile restricted to curr_cands. Otherwise, the Copeland scores are computed with respect to the entire profile.
+
+    Args:
+        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): The candidates to rank. If None, then all candidates in profile are ranked
+        local (bool, optional): If True, then the Copeland scores are computed with respect to the profile restricted to curr_cands. Otherwise, the Copeland scores are computed with respect to the entire profile.
+        tie_breaking (str, optional): The tie-breaking method to use. If None, then no tie-breaking is used. If "alphabetic", then the tie-breaking is done alphabetically.
+
+    Returns:
+        A Ranking object
+    """
+
+    cands = edata.candidates if curr_cands is None else curr_cands
+
+    if local:
+        copeland_scores_dict = edata.copeland_scores(curr_cands=cands)
+
+    else:
+        c_scores = edata.copeland_scores(curr_cands=edata.candidates)
+        copeland_scores_dict = {c: c_scores[c] for c in cands}
+
+    for cand in cands:
+        copeland_scores_dict[cand] = -copeland_scores_dict[cand]
+
+    copeland_ranking = Ranking(copeland_scores_dict)
+    copeland_ranking.normalize_ranks()
+
+    if tie_breaking == "alphabetic":
+        copeland_ranking = break_ties_alphabetically(copeland_ranking)
+
+    return copeland_ranking
 
 @vm(name = "Llull")
 def llull(edata, curr_cands = None):
     """The Llull score for a candidate :math:`c` is the number of candidates that :math:`c` is weakly majority preferred to.  This is equivalent to calculating the Copeland scores for a candidate :math:`c` with 1 point for each candidate that :math:`c` is majority preferred to, 1/2 point for each candidate that :math:`c` is tied with, and 0 points for each candidate that is majority preferred to :math:`c`.  The Llull winners are the candidates with the maximum Llull score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
@@ -887,12 +921,16 @@
     uc_fish,
     uc_bordes,
     uc_mckelvey,
     top_cycle,
     gocha,
 ]
 
+c1_swf = [
+    copeland_ranking
+]
+
 defeat_methods = [
     top_cycle_defeat,
     uc_gill_defeat,
     uc_fish_defeat
 ]
```

### Comparing `pref_voting-0.9.3/pref_voting/combined_methods.py` & `pref_voting-0.9.4/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/dominance_axioms.py` & `pref_voting-0.9.4/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/generate_profiles.py` & `pref_voting-0.9.4/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/generate_spatial_profiles.py` & `pref_voting-0.9.4/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/generate_utility_profiles.py` & `pref_voting-0.9.4/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.9.4/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/grade_methods.py` & `pref_voting-0.9.4/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/grade_profiles.py` & `pref_voting-0.9.4/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/helper.py` & `pref_voting-0.9.4/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/invariance_axioms.py` & `pref_voting-0.9.4/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/io/readers.py` & `pref_voting-0.9.4/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/io/writers.py` & `pref_voting-0.9.4/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/iterative_methods.py` & `pref_voting-0.9.4/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/maj_graph_ex1.png` & `pref_voting-0.9.4/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/mappings.py` & `pref_voting-0.9.4/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/margin_based_methods.py` & `pref_voting-0.9.4/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/monotonicity_axioms.py` & `pref_voting-0.9.4/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/other_methods.py` & `pref_voting-0.9.4/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/probabilistic_methods.py` & `pref_voting-0.9.4/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/profiles.py` & `pref_voting-0.9.4/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/profiles_with_ties.py` & `pref_voting-0.9.4/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/rankings.py` & `pref_voting-0.9.4/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/scoring_methods.py` & `pref_voting-0.9.4/pref_voting/scoring_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     Returns:
         A Ranking object
     """
 
     cands = profile.candidates if curr_cands is None else curr_cands
 
     if local:
-        plurality_scores_dict = profile.plurality_scores(curr_cands = curr_cands)
+        plurality_scores_dict = profile.plurality_scores(curr_cands = cands)
 
     else:
         plurality_scores_dict = profile.plurality_scores()
         plurality_scores_dict = {k: v for k, v in plurality_scores_dict.items() if k in cands}
 
     assert plurality_scores_dict != {}, "Cannot calculate plurality scores."
 
@@ -150,15 +150,15 @@
     Returns:
         A Ranking object
     """
 
     cands = profile.candidates if curr_cands is None else curr_cands
 
     if local:
-        borda_scores_dict = profile.borda_scores(curr_cands = curr_cands)
+        borda_scores_dict = profile.borda_scores(curr_cands = cands)
 
     else:
         borda_scores_dict = profile.borda_scores()
         borda_scores_dict = {k: v for k, v in borda_scores_dict.items() if k in cands}
 
     for cand in cands:
         borda_scores_dict[cand] = -borda_scores_dict[cand]
@@ -208,14 +208,48 @@
     cands_to_ignore = np.array([c for c in profile.candidates if c not in curr_cands])
     
     last_place_scores = {c: _num_rank_last(rankings, rcounts, cands_to_ignore, c) for c in curr_cands}
     min_last_place_score = min(list(last_place_scores.values()))
     
     return sorted([c for c in curr_cands if last_place_scores[c] == min_last_place_score])
 
+@swf(name="Anti-Plurality ranking")
+def anti_plurality_ranking(profile, curr_cands=None, local=True, tie_breaking=None):
+    """The SWF that ranks the candidates in curr_cands according to their Anti-Plurality scores. If local is True, then the Anti-Plurality scores are computed with respect to the profile restricted to curr_cands. Otherwise, the Anti-Plurality scores are computed with respect to the entire profile.
+
+    Args:
+        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): The candidates to rank. If None, then all candidates in profile are ranked
+        local (bool, optional): If True, then the Anti-Plurality scores are computed with respect to the profile restricted to curr_cands. Otherwise, the Anti-Plurality scores are computed with respect to the entire profile.
+        tie_breaking (str, optional): The tie-breaking method to use. If None, then no tie-breaking is used. If "alphabetic", then the tie-breaking is done alphabetically.
+
+    Returns:
+        A Ranking object
+    """
+
+    cands = profile.candidates if curr_cands is None else curr_cands
+
+    rankings, rcounts = profile.rankings_counts
+
+    if local:
+        cands_to_ignore = np.array([c for c in profile.candidates if c not in cands])
+
+    else:
+        cands_to_ignore = np.array([])
+    
+    anti_plurality_scores_dict = {c: _num_rank_last(rankings, rcounts, cands_to_ignore, c) for c in cands}
+
+    ap_ranking = Ranking(anti_plurality_scores_dict)
+    ap_ranking.normalize_ranks()
+
+    if tie_breaking == "alphabetic":
+        ap_ranking = break_ties_alphabetically(ap_ranking)
+
+    return ap_ranking
+
 
 @vm(name = "Scoring Rule")
 def scoring_rule(profile, curr_cands = None, score = lambda num_cands, rank : 1 if rank == 1 else 0):
     """A general scoring rule.  Each voter assign a score to each candidate using the ``score`` function based on their submitted ranking (restricted to candidates in ``curr_cands``).   Returns that candidates with the greatest overall score in the profile restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -417,14 +451,15 @@
     
     return sorted([c for c in restricted_prof.candidates if b_scores[c] == max_borda_score])
 
 
 scoring_swfs = [
     plurality_ranking,
     borda_ranking,
+    anti_plurality_ranking,
     score_ranking   
 ]
 
 scoring_vms = [
     anti_plurality,
     plurality, 
     borda,
```

### Comparing `pref_voting-0.9.3/pref_voting/social_welfare_function.py` & `pref_voting-0.9.4/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/spatial_profiles.py` & `pref_voting-0.9.4/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/conftest.py` & `pref_voting-0.9.4/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_c1_methods.py` & `pref_voting-0.9.4/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_majority_graph.py` & `pref_voting-0.9.4/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_margin_graph.py` & `pref_voting-0.9.4/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_profile.py` & `pref_voting-0.9.4/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-0.9.4/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_spatial_profile.py` & `pref_voting-0.9.4/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_support_graph.py` & `pref_voting-0.9.4/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_utility_functions.py` & `pref_voting-0.9.4/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/tests/test_voting_method.py` & `pref_voting-0.9.4/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/utility_functions.py` & `pref_voting-0.9.4/pref_voting/utility_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,40 +31,40 @@
         float: The utility of the candidate to the voter.
     """
 
     return np.dot(v_pos, c_pos)
 
 def linear_utility(v_pos: float32[:], c_pos: float32[:]):
     """
-    The utility of the voter for the candidate is negative of the difference in positions. 
+    The utility of the candidate for the voter is negative of the Euclidean distance between the positions. 
 
     Args:   
         v_pos (numpy array): The position(s) of the voter.
         c_pos (numpy array): The position(s) of the candidate.  
     Returns:
         float: The utility of the candidate to the voter.
     """
     return -np.linalg.norm(v_pos - c_pos)
 
 def quadratic_utility(v_pos: float32[:], c_pos: float32[:]):
     """ 
-    The utility of the voter for the candidate is negative of the squared difference in positions.
+    The utility of the candidate for the voter is negative of the squared Euclidean distance between the positions. 
 
     Args:
         v_pos (numpy array): The position(s) of the voter.
         c_pos (numpy array): The position(s) of the candidate.
     Returns:
         float: The utility of the candidate to the voter.
     """
     return -np.linalg.norm(v_pos - c_pos)**2
 
 
 def city_block_utility(v_pos: float32[:], c_pos: float32[:]):
     """
-    The utility of the voter for the candidate is negative of the city-block distance between the positions (also known as the Manhattan distance). 
+    The utility of the candidate for the voter is the negative of the city-block distance between the positions (also known as the Manhattan distance). 
 
     Args:
         v_pos (numpy array): The position(s) of the voter.
         c_pos (numpy array): The position(s) of the candidate.
     Returns:
         float: The utility of the candidate to the voter.
     """
```

### Comparing `pref_voting-0.9.3/pref_voting/utility_methods.py` & `pref_voting-0.9.4/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/utility_profiles.py` & `pref_voting-0.9.4/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/variable_candidate_axioms.py` & `pref_voting-0.9.4/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/variable_voter_axioms.py` & `pref_voting-0.9.4/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/voting_method.py` & `pref_voting-0.9.4/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.9.4/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.3/pyproject.toml` & `pref_voting-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.9.3"
+version = "0.9.4"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.9.3/setup.py` & `pref_voting-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.0,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.\n- v0.4 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.\n- v0.4.8 (2023-5-31): Add bottom two IRV and Tideman\'s alternative voting methods.\n- v0.4.12 (2023-6-3): Add probabilistic methods.\n- v0.5.0 (2023-9-24): Add _Mapping class with Utility and Grade as subclasses of _Mapping, add GradeProfile class, add Score Vote, Approval Vote, and STAR Vote.\n- v0.5.4 (2023-10-01): Add median grading voting methods.\n- v0.7.0 (2024-02-18): Use prefsampling for generating preference profiles.\n- v0.9.0 (2024-03-19): Add save/load functions for saving election data.\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-0.9.3/PKG-INFO` & `pref_voting-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.9.3
+Version: 0.9.4
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

