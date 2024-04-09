# Comparing `tmp/mteb-1.5.3.tar.gz` & `tmp/mteb-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.5.3.tar", last modified: Mon Apr  8 07:41:30 2024, max compression
+gzip compressed data, was "mteb-1.5.4.tar", last modified: Mon Apr  8 19:31:23 2024, max compression
```

## Comparing `mteb-1.5.3.tar` & `mteb-1.5.4.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.589388 mteb-1.5.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-08 07:41:26.000000 mteb-1.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 07:41:30.589388 mteb-1.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-08 07:41:26.000000 mteb-1.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.529388 mteb-1.5.3/mteb/
--rw-r--r--   0 root         (0) root         (0)     2135 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     6458 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13124 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2505 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2937 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6075 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4892 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)     1037 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6535 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1619 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2499 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3590 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3615 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3553 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1189 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1206 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2813 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.561388 mteb-1.5.3/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2577 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.561388 mteb-1.5.3/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     1997 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1223 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2896 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      977 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3699 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1108 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2182 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2469 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3248 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3250 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2921 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2702 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2613 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)    10336 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1364 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1480 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1466 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2256 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     7080 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1298 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2120 2024-04-08 07:41:27.000000 mteb-1.5.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      890 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 07:41:30.589388 mteb-1.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-08 19:31:19.000000 mteb-1.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 19:31:23.629630 mteb-1.5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-08 19:31:19.000000 mteb-1.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.569630 mteb-1.5.4/mteb/
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.573630 mteb-1.5.4/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.573630 mteb-1.5.4/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13124 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.577630 mteb-1.5.4/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.577630 mteb-1.5.4/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.577630 mteb-1.5.4/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.577630 mteb-1.5.4/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.577630 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.581630 mteb-1.5.4/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.581630 mteb-1.5.4/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.581630 mteb-1.5.4/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.581630 mteb-1.5.4/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.585630 mteb-1.5.4/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.585630 mteb-1.5.4/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.585630 mteb-1.5.4/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.585630 mteb-1.5.4/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.585630 mteb-1.5.4/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.589630 mteb-1.5.4/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.589630 mteb-1.5.4/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.593630 mteb-1.5.4/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.593630 mteb-1.5.4/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.593630 mteb-1.5.4/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.593630 mteb-1.5.4/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.593630 mteb-1.5.4/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.597630 mteb-1.5.4/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2814 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.601630 mteb-1.5.4/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.605630 mteb-1.5.4/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.609630 mteb-1.5.4/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.609630 mteb-1.5.4/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.613630 mteb-1.5.4/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2139 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.613630 mteb-1.5.4/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.613630 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.613630 mteb-1.5.4/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.617631 mteb-1.5.4/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.617631 mteb-1.5.4/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.617631 mteb-1.5.4/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)    10336 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.617631 mteb-1.5.4/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.617631 mteb-1.5.4/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     7080 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.621631 mteb-1.5.4/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-08 19:31:19.000000 mteb-1.5.4/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-08 19:31:23.000000 mteb-1.5.4/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-08 19:31:20.000000 mteb-1.5.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.625630 mteb-1.5.4/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-08 19:31:19.000000 mteb-1.5.4/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 19:31:23.629630 mteb-1.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 19:31:23.629630 mteb-1.5.4/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-08 19:31:19.000000 mteb-1.5.4/tests/test_all_abstasks.py
```

### Comparing `mteb-1.5.3/LICENSE` & `mteb-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/PKG-INFO` & `mteb-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.3
+Version: 1.5.4
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.3/README.md` & `mteb-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/__init__.py` & `mteb-1.5.4/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTask.py` & `mteb-1.5.4/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.5.4/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/CrosslingualTask.py` & `mteb-1.5.4/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/LangMapping.py` & `mteb-1.5.4/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/abstasks/MultilingualTask.py` & `mteb-1.5.4/mteb/abstasks/MultilingualTask.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,9 @@
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang,
                 **self.metadata_dict.get("dataset", None),
             )
+        self.dataset_transform()
         self.data_loaded = True
```

### Comparing `mteb-1.5.3/mteb/abstasks/TaskMetadata.py` & `mteb-1.5.4/mteb/abstasks/TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/cmd.py` & `mteb-1.5.4/mteb/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
        --output_folder mteb_output \
        --verbosity 3
 """
 
 from __future__ import annotations
 
 import argparse
-import datetime
 import json
 import logging
 from pathlib import Path
 
 from sentence_transformers import SentenceTransformer
 
 from mteb import MTEB
@@ -31,15 +30,14 @@
 def _save_model_metadata(
     model: SentenceTransformer, model_name: str, output_folder: Path
 ) -> None:
     save_path = output_folder / "model_meta.json"
 
     model_meta = {
         "model_name": model_name,
-        "time_of_run": str(datetime.datetime.today()),
         "versions": model._model_config.get("__version__", None),
     }
 
     with save_path.open("w") as f:
         json.dump(model_meta, f)
```

### Comparing `mteb-1.5.3/mteb/evaluation/MTEB.py` & `mteb-1.5.4/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.5.4/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/evaluation/evaluators/utils.py` & `mteb-1.5.4/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/logging.py` & `mteb-1.5.4/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.5.4/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/__init__.py` & `mteb-1.5.4/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/NewsClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.5.4/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/__init__.py` & `mteb-1.5.4/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class FloresClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="FloresClusteringS2S",
         description="Clustering of sentences from various web articles, 32 topics in total.",
         reference="https://huggingface.co/datasets/facebook/flores",
         dataset={
-            "path": "facebook/flores",
-            "revision": "2db78afdeaccaedc3b33a95442a4e55766887e17",
+            "path": "jinaai/flores_clustering",
+            "revision": "97faaf98d7ef21869d176115e669e2a4286513bf",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["es"],
         main_score="v_measure",
         date=None,
```

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         name="MLSUMClusteringP2P",
         description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
         reference="https://huggingface.co/datasets/mlsum",
         dataset={
             "path": "mlsum",
             "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
             "name": "fr",
-            "split": "test",
+            "trust_remote_code": True,
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
         date=None,
```

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         name="MLSUMClusteringS2S",
         description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
         reference="https://huggingface.co/datasets/mlsum",
         dataset={
             "path": "mlsum",
             "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
             "name": "fr",
-            "split": "test",
+            "trust_remote_code": True,
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
         date=None,
```

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.5.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.5.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.5.4/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.5.4/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.5.4/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.5.4/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.5.4/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.5.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import MultilingualTask
-from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class PawsX(MultilingualTask, AbsTaskPairClassification):
+class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="PawsX",
+        name="SpanishPassageRetrievalS2S",
+        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
+        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
         dataset={
-            "path": "paws-x",
-            "revision": "8a04d940a42cd40658986fdd8e3da561533a3646",
+            "path": "jinaai/spanish_passage_retrieval",
+            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+            "trust_remote_code": True,
         },
-        description="",
-        reference="https://arxiv.org/abs/1908.11828",
+        type="Retrieval",
         category="s2s",
-        type="PairClassification",
-        eval_splits=["test", "validation"],
-        eval_langs=["de", "en", "es", "fr", "ja", "ko", "zh"],
-        main_score="ap",
+        eval_splits=["test"],
+        eval_langs=["es"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -36,34 +36,32 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
-        self.dataset = dict()
-        for lang in self.langs:
-            hf_dataset = datasets.load_dataset(
-                name=lang,
-                **self.metadata_dict["dataset"],
-            )
-
-            sent1 = []
-            sent2 = []
-            labels = []
-
-            for line in hf_dataset["test"]:
-                sent1.append(line["sentence1"])
-                sent2.append(line["sentence2"])
-                labels.append(line["label"])
-
-            self.dataset[lang] = {
-                "test": [
-                    {
-                        "sent1": sent1,
-                        "sent2": sent2,
-                        "labels": labels,
-                    }
-                ]
+        query_rows = datasets.load_dataset(
+            name="queries",
+            split="test",
+            **self.metadata_dict["dataset"],
+        )
+        corpus_rows = datasets.load_dataset(
+            name="corpus.sentences",
+            split="test",
+            **self.metadata_dict["dataset"],
+        )
+        qrels_rows = datasets.load_dataset(
+            name="qrels.s2s",
+            split="test",
+            **self.metadata_dict["dataset"],
+        )
+
+        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
+        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
+        self.relevant_docs = {
+            "test": {
+                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
             }
+        }
 
         self.data_loaded = True
```

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.5.4/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.5.4/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.5.4/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/en/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.5.4/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.5.4/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/__init__.py` & `mteb-1.5.4/mteb/tasks/Retrieval/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from .da.dan_fever import *
 from .da.t2nord_retrieval import *
 from .da.twitterhjerne import *
 from .de.GerDaLIRRetrieval import *
+from .de.GerDaLIRSmallRetrieval import *
 from .de.GermanDPRRetrieval import *
 from .de.GermanQuADRetrieval import *
-from .de.GerDaLIRSmallRetrieval import *
 from .de.LegalQuADRetrieval import *
+from .en.AILACasedocsRetrieval import *
+from .en.AILAStatutesRetrieval import *
 from .en.ArguAnaRetrieval import *
 from .en.ClimateFEVERRetrieval import *
 from .en.CQADupstackAndroidRetrieval import *
 from .en.CQADupstackEnglishRetrieval import *
 from .en.CQADupstackGamingRetrieval import *
 from .en.CQADupstackGisRetrieval import *
 from .en.CQADupstackMathematicaRetrieval import *
@@ -23,29 +25,27 @@
 from .en.CQADupstackWebmastersRetrieval import *
 from .en.CQADupstackWordpressRetrieval import *
 from .en.DBPediaRetrieval import *
 from .en.FEVERRetrieval import *
 from .en.FiQA2018Retrieval import *
 from .en.HagridRetrieval import *
 from .en.HotpotQARetrieval import *
+from .en.LegalBenchConsumerContractsQARetrieval import *
+from .en.LegalBenchCorporateLobbyingRetrieval import *
+from .en.LegalSummarizationRetrieval import *
 from .en.MSMARCORetrieval import *
 from .en.MSMARCOv2Retrieval import *
 from .en.NarrativeQARetrieval import *
 from .en.NFCorpusRetrieval import *
 from .en.NQRetrieval import *
 from .en.QuoraRetrieval import *
 from .en.SCIDOCSRetrieval import *
 from .en.SciFactRetrieval import *
 from .en.Touche2020Retrieval import *
 from .en.TRECCOVIDRetrieval import *
-from .en.AILACasedocsRetrieval import *
-from .en.AILAStatutesRetrieval import *
-from .en.LegalBenchConsumerContractsQARetrieval import *
-from .en.LegalBenchCorporateLobbyingRetrieval import *
-from .en.LegalSummarizationRetrieval import *
 from .es.SpanishPassageRetrievalS2P import *
 from .es.SpanishPassageRetrievalS2S import *
 from .fr.AlloprofRetrieval import *
 from .fr.BSARDRetrieval import *
 from .fr.SyntecRetrieval import *
 from .ko.KoMiracl import *
 from .ko.KoMrtydi import *
@@ -67,8 +67,8 @@
 from .pl.QuoraPLRetrieval import *
 from .pl.SCIDOCSPLRetrieval import *
 from .pl.SciFactPLRetrieval import *
 from .pl.TRECCOVIDPLRetrieval import *
 from .sv.swedn_retrieval import *
 from .sv.swefaq_retrieval import *
 from .zh.CMTEBRetrieval import *
-from .zh.LeCaRDv2Retrieval import *
+from .zh.LeCaRDv2Retrieval import *
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.5.4/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.5.4/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         query_rows = datasets.load_dataset(
             name="queries",
             split=self._EVAL_SPLIT,
+            **self.metadata_dict["dataset"],
         )
         corpus_rows = datasets.load_dataset(
             name="corpus",
             split=self._EVAL_SPLIT,
             **self.metadata_dict["dataset"],
         )
         qrels_rows = datasets.load_dataset(
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="MIT license",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/de/LegalQuADRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/de/LegalQuADRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Question answering"],
         license="CC BY 4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="CC BY 4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="CC BY 4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Question answering"],
         license="CC BY-NC 4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="CC BY 4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="Apache License 2.0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,16 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         data = datasets.load_dataset(
-            split=self._EVAL_SPLIT
-            # BUGFIX: the revision is now used
-            ** self.metadata_dict["dataset"],
+            split=self._EVAL_SPLIT,
+            **self.metadata_dict["dataset"],
         )
         self.queries = {
             self._EVAL_SPLIT: {
                 str(i): row["question"]["text"] for i, row in enumerate(data)
             }
         }
         self.corpus = {
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.5.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,19 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
-        # BUGFIX: the revision is now used
         query_rows = datasets.load_dataset(
             name="queries",
             split="test",
             trust_remote_code=True,
+            **self.metadata_dict["dataset"],
         )
         corpus_rows = datasets.load_dataset(
             name="corpus.documents",
             split="test",
             trust_remote_code=True,
             **self.metadata_dict["dataset"],
         )
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.5.4/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,78 @@
 from __future__ import annotations
 
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks import MultilingualTask
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
+_EVAL_SPLIT = "test"
+_EVAL_LANGS = ["es", "de", "en"]
 
-class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
+
+def _load_xmarket_data(
+    path: str, langs: list, split: str, cache_dir: str = None, revision: str = None
+):
+    corpus = {lang: {split: None} for lang in langs}
+    queries = {lang: {split: None} for lang in langs}
+    relevant_docs = {lang: {split: None} for lang in langs}
+
+    for lang in langs:
+        corpus_rows = datasets.load_dataset(
+            path,
+            f"corpus-{lang}",
+            languages=[lang],
+            split=split,
+            cache_dir=cache_dir,
+        )
+        query_rows = datasets.load_dataset(
+            path,
+            f"queries-{lang}",
+            languages=[lang],
+            revision=revision,
+            split=split,
+            cache_dir=cache_dir,
+        )
+        qrels_rows = datasets.load_dataset(
+            path,
+            f"qrels-{lang}",
+            languages=[lang],
+            revision=revision,
+            split=split,
+            cache_dir=cache_dir,
+        )
+
+        corpus[lang][split] = {row["_id"]: row for row in corpus_rows}
+        queries[lang][split] = {row["_id"]: row["text"] for row in query_rows}
+        relevant_docs[lang][split] = {
+            row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
+        }
+
+    corpus = datasets.DatasetDict(corpus)
+    queries = datasets.DatasetDict(queries)
+    relevant_docs = datasets.DatasetDict(relevant_docs)
+
+    return corpus, queries, relevant_docs
+
+
+class XMarket(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SpanishPassageRetrievalS2S",
-        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
-        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
+        name="XMarket",
+        description="XMarket",
+        reference=None,
         dataset={
-            "path": "jinaai/spanish_passage_retrieval",
-            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+            "path": "jinaai/xmarket_ml",
+            "revision": "dfe57acff5b62c23732a7b7d3e3fb84ff501708b",
         },
         type="Retrieval",
-        category="s2s",
-        eval_splits=["test"],
-        eval_langs=["es"],
+        category="s2p",
+        eval_splits=[_EVAL_SPLIT],
+        eval_langs=_EVAL_LANGS,
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
@@ -35,35 +84,16 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
-        query_rows = datasets.load_dataset(
-            name="queries",
-            split="test",
-            trust_remote_code=True,
-            **self.metadata_dict["dataset"],
-        )
-        corpus_rows = datasets.load_dataset(
-            name="corpus.sentences",
-            split="test",
-            trust_remote_code=True,
-            **self.metadata_dict["dataset"],
-        )
-        qrels_rows = datasets.load_dataset(
-            name="qrels.s2s",
-            split="test",
-            trust_remote_code=True,
-            **self.metadata_dict["dataset"],
+        self.corpus, self.queries, self.relevant_docs = _load_xmarket_data(
+            path=self.metadata_dict["dataset"]["path"],
+            langs=self.metadata.eval_langs,
+            split=self.metadata_dict["eval_splits"][0],
+            cache_dir=kwargs.get("cache_dir", None),
+            revision=self.metadata_dict["dataset"]["revision"],
         )
 
-        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
-        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
-        self.relevant_docs = {
-            "test": {
-                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
-            }
-        }
-
         self.data_loaded = True
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         # fetch both subsets of the dataset
-        # BUGFIX: the revision is now used
         corpus_raw = datasets.load_dataset(
             name="documents",
             **self.metadata_dict["dataset"],
         )
         queries_raw = datasets.load_dataset(
             name="queries",
             **self.metadata_dict["dataset"],
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/fr/BSARDRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         # fetch both subsets of the dataset
-        # BUGFIX: the revision is now used
         corpus_raw = datasets.load_dataset(
             name="documents",
             **self.metadata_dict["dataset"],
         )
         queries_raw = datasets.load_dataset(
             name="queries",
             **self.metadata_dict["dataset"],
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.5.4/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.5.4/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.5.4/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,75 +4,68 @@
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks import MultilingualTask
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 _EVAL_SPLIT = "test"
-_EVAL_LANGS = ["es", "de", "en"]
+_LANGS = ["ar", "de", "es", "fr", "hi", "it", "ja", "ko", "pl", "pt", "ta", "zh"]
 
 
-def _load_xmarket_data(
+def _load_xpqa_data(
     path: str, langs: list, split: str, cache_dir: str = None, revision: str = None
 ):
-    corpus = {lang: {split: None} for lang in langs}
-    queries = {lang: {split: None} for lang in langs}
-    relevant_docs = {lang: {split: None} for lang in langs}
+    queries = {lang: {split: {}} for lang in langs}
+    corpus = {lang: {split: {}} for lang in langs}
+    relevant_docs = {lang: {split: {}} for lang in langs}
 
     for lang in langs:
-        corpus_rows = datasets.load_dataset(
+        data = datasets.load_dataset(
             path,
-            f"corpus-{lang}",
-            languages=[lang],
+            lang,
             split=split,
             cache_dir=cache_dir,
-        )
-        query_rows = datasets.load_dataset(
-            path,
-            f"queries-{lang}",
-            languages=[lang],
             revision=revision,
-            split=split,
-            cache_dir=cache_dir,
         )
-        qrels_rows = datasets.load_dataset(
-            path,
-            f"qrels-{lang}",
-            languages=[lang],
-            revision=revision,
-            split=split,
-            cache_dir=cache_dir,
-        )
-
-        corpus[lang][split] = {row["_id"]: row for row in corpus_rows}
-        queries[lang][split] = {row["_id"]: row["text"] for row in query_rows}
-        relevant_docs[lang][split] = {
-            row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
+        question_ids = {
+            question: _id for _id, question in enumerate(set(data["question"]))
         }
+        answer_ids = {answer: _id for _id, answer in enumerate(set(data["answer"]))}
+
+        for row in data:
+            question = row["question"]
+            answer = row["answer"]
+            query_id = f"Q{question_ids[question]}"
+            queries[lang][split][query_id] = question
+            doc_id = f"D{answer_ids[answer]}"
+            corpus[lang][split][doc_id] = {"text": answer}
+            if query_id not in relevant_docs[lang][split]:
+                relevant_docs[lang][split][query_id] = {}
+            relevant_docs[lang][split][query_id][doc_id] = 1
 
     corpus = datasets.DatasetDict(corpus)
     queries = datasets.DatasetDict(queries)
     relevant_docs = datasets.DatasetDict(relevant_docs)
 
     return corpus, queries, relevant_docs
 
 
-class XMarket(MultilingualTask, AbsTaskRetrieval):
+class XPQARetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="XMarket",
-        description="XMarket",
-        reference=None,
+        name="XPQARetrieval",
+        description="XPQARetrieval",
+        reference="https://arxiv.org/abs/2305.09249",
         dataset={
-            "path": "jinaai/xmarket_ml",
-            "revision": "dfe57acff5b62c23732a7b7d3e3fb84ff501708b",
+            "path": "jinaai/xpqa",
+            "revision": "c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
-        eval_langs=_EVAL_LANGS,
+        eval_langs=_LANGS,
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
@@ -84,16 +77,16 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
-        self.corpus, self.queries, self.relevant_docs = _load_xmarket_data(
+        self.corpus, self.queries, self.relevant_docs = _load_xpqa_data(
             path=self.metadata_dict["dataset"]["path"],
-            langs=self.metadata.eval_langs,
+            langs=self.langs,
             split=self.metadata_dict["eval_splits"][0],
             cache_dir=kwargs.get("cache_dir", None),
             revision=self.metadata_dict["dataset"]["revision"],
         )
 
         self.data_loaded = True
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.5.4/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,76 @@
 from __future__ import annotations
 
-import datasets
-
+from mteb.abstasks.AbsTaskSTS import AbsTaskSTS
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import MultilingualTask
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
-
-_EVAL_SPLIT = "test"
-_LANGS = ["ar", "de", "es", "fr", "hi", "it", "ja", "ko", "pl", "pt", "ta", "zh"]
-
 
-def _load_xpqa_data(
-    path: str, langs: list, split: str, cache_dir: str = None, revision: str = None
-):
-    queries = {lang: {split: {}} for lang in langs}
-    corpus = {lang: {split: {}} for lang in langs}
-    relevant_docs = {lang: {split: {}} for lang in langs}
-
-    for lang in langs:
-        data = datasets.load_dataset(
-            path,
-            lang,
-            split=split,
-            cache_dir=cache_dir,
-            revision=revision,
-        )
-        question_ids = {
-            question: _id for _id, question in enumerate(set(data["question"]))
-        }
-        answer_ids = {answer: _id for _id, answer in enumerate(set(data["answer"]))}
-
-        for row in data:
-            question = row["question"]
-            answer = row["answer"]
-            query_id = f"Q{question_ids[question]}"
-            queries[lang][split][query_id] = question
-            doc_id = f"D{answer_ids[answer]}"
-            corpus[lang][split][doc_id] = {"text": answer}
-            if query_id not in relevant_docs[lang][split]:
-                relevant_docs[lang][split][query_id] = {}
-            relevant_docs[lang][split][query_id][doc_id] = 1
-
-    corpus = datasets.DatasetDict(corpus)
-    queries = datasets.DatasetDict(queries)
-    relevant_docs = datasets.DatasetDict(relevant_docs)
+class SickrPLSTS(AbsTaskSTS):
+    metadata = TaskMetadata(
+        name="SICK-R-PL",
+        dataset={
+            "path": "PL-MTEB/sickr-pl-sts",
+            "revision": "fd5c2441b7eeff8676768036142af4cfa42c1339",
+        },
+        description="Polish version of SICK dataset for textual relatedness.",
+        reference="https://aclanthology.org/2020.lrec-1.207",
+        type="STS",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["pl"],
+        main_score="cosine_spearman",
+        date=None,
+        form=None,
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
+        dialect=None,
+        text_creation=None,
+        bibtex_citation=None,
+        n_samples={"test": 9812},
+        avg_character_length={"test": 42.8},
+    )
 
-    return corpus, queries, relevant_docs
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 5
+        return metadata_dict
 
 
-class XPQARetrieval(MultilingualTask, AbsTaskRetrieval):
+class CdscrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="XPQARetrieval",
-        description="XPQARetrieval",
-        reference="https://arxiv.org/abs/2305.09249",
+        name="CDSC-R",
         dataset={
-            "path": "jinaai/xpqa",
-            "revision": "c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
+            "path": "PL-MTEB/cdscr-sts",
+            "revision": "1cd6abbb00df7d14be3dbd76a7dcc64b3a79a7cd",
         },
-        type="Retrieval",
-        category="s2p",
-        eval_splits=[_EVAL_SPLIT],
-        eval_langs=_LANGS,
-        main_score="ndcg_at_10",
+        description="Compositional Distributional Semantics Corpus for textual relatedness.",
+        reference="https://aclanthology.org/P17-1073.pdf",
+        type="STS",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["pl"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-
-        self.corpus, self.queries, self.relevant_docs = _load_xpqa_data(
-            path=self.metadata_dict["dataset"]["path"],
-            langs=self.langs,
-            split=self.metadata_dict["eval_splits"][0],
-            cache_dir=kwargs.get("cache_dir", None),
-            revision=self.metadata_dict["dataset"]["revision"],
-        )
-
-        self.data_loaded = True
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.5.4/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
         dataset={
             "path": "clarin-knext/quora-pl",
             "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
         },
         type="Retrieval",
         category="s2s",
-        eval_splits=["validation", "test"],  # validation for new DataLoader
+        eval_splits=["validation", "test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
```

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py` & `mteb-1.5.4/mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
         license="MIT license",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
-        bibtex_citation= None,
+        bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
```

### Comparing `mteb-1.5.3/mteb/tasks/STS/__init__.py` & `mteb-1.5.4/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.5.4/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.5.4/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.5.4/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.5.4/mteb/tasks/STS/en/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/es/STSES.py` & `mteb-1.5.4/mteb/tasks/STS/es/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/fr/SickFrSTS.py` & `mteb-1.5.4/mteb/tasks/STS/fr/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.5.4/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.5.4/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.5.4/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.5.4/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.5.4/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py` & `mteb-1.5.4/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/mteb.egg-info/PKG-INFO` & `mteb-1.5.4/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.3
+Version: 1.5.4
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.3/mteb.egg-info/SOURCES.txt` & `mteb-1.5.4/mteb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/pyproject.toml` & `mteb-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.5.3"
+version = "1.5.4"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.5.3/scripts/data/amazon_polarity/create_data.py` & `mteb-1.5.4/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.5.4/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/arxiv/script_clustering.py` & `mteb-1.5.4/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/arxiv/script_raw.py` & `mteb-1.5.4/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/biorxiv/script_clustering.py` & `mteb-1.5.4/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/biorxiv/script_raw.py` & `mteb-1.5.4/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/bucc/create_data.py` & `mteb-1.5.4/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/create_task_table.py` & `mteb-1.5.4/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/germanquad/process_data.py` & `mteb-1.5.4/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/hal/create_data.py` & `mteb-1.5.4/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/imdb/create_data.py` & `mteb-1.5.4/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/medrxiv/script_clustering.py` & `mteb-1.5.4/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/medrxiv/script_raw.py` & `mteb-1.5.4/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/mind/prepare_data.py` & `mteb-1.5.4/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/redditp2p/script_clustering.py` & `mteb-1.5.4/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.5.4/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.5.4/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/summeval_fr/create_data.py` & `mteb-1.5.4/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.5.4/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/merge_cqadupstack.py` & `mteb-1.5.4/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/mteb_meta.py` & `mteb-1.5.4/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_chinese.py` & `mteb-1.5.4/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_english.py` & `mteb-1.5.4/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_french.py` & `mteb-1.5.4/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_german.py` & `mteb-1.5.4/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_korean.py` & `mteb-1.5.4/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/scripts/run_mteb_law.py` & `mteb-1.5.4/scripts/run_mteb_law.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,13 +25,11 @@
 
 model_name = "average_word_embeddings_komninos"
 model = SentenceTransformer(model_name)
 
 for task in TASK_LIST_RETRIEVAL_LAW:
     logger.info(f"Running task: {task}")
     eval_splits = ["test"]
-    evaluation = MTEB(
-        tasks=[task]
-    )
+    evaluation = MTEB(tasks=[task])
     evaluation.run(
         model, output_folder=f"results/{model_name}", eval_splits=eval_splits
     )
```

### Comparing `mteb-1.5.3/scripts/run_mteb_polish.py` & `mteb-1.5.4/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_ClusteringEvaluator.py` & `mteb-1.5.4/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_PairClassificationEvaluator.py` & `mteb-1.5.4/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_RerankingEvaluator.py` & `mteb-1.5.4/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_RetrievalEvaluator.py` & `mteb-1.5.4/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_TaskMetadata.py` & `mteb-1.5.4/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.3/tests/test_all_abstasks.py` & `mteb-1.5.4/tests/test_all_abstasks.py`

 * *Files identical despite different names*

