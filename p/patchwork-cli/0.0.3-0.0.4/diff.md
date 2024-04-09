# Comparing `tmp/patchwork_cli-0.0.3.tar.gz` & `tmp/patchwork_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.3.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.4.tar", max compression
```

## Comparing `patchwork_cli-0.0.3.tar` & `patchwork_cli-0.0.4.tar`

### file list

```diff
@@ -1,88 +1,92 @@
--rw-r--r--   0        0        0    34522 2024-04-02 03:23:14.301159 patchwork_cli-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     5115 2024-04-04 04:10:24.325019 patchwork_cli-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.325070 patchwork_cli-0.0.3/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.325169 patchwork_cli-0.0.3/patchwork/__main__.py
--rw-r--r--   0        0        0     2849 2024-04-04 04:10:24.326540 patchwork_cli-0.0.3/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.326608 patchwork_cli-0.0.3/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    12408 2024-04-04 04:10:24.326830 patchwork_cli-0.0.3/patchwork/common/client/scm.py
--rw-r--r--   0        0        0      816 2024-04-04 04:10:24.326964 patchwork_cli-0.0.3/patchwork/common/utils.py
--rw-r--r--   0        0        0     1546 2024-04-04 04:10:24.327093 patchwork_cli-0.0.3/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-04-04 04:10:24.327205 patchwork_cli-0.0.3/patchwork/managed_files.py
--rw-r--r--   0        0        0     2775 2024-04-04 04:10:24.327337 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     2182 2024-04-04 04:10:24.327457 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      809 2024-04-04 04:10:24.327567 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5434 2024-04-04 04:10:24.327717 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0      704 2024-04-04 04:10:24.327912 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2409 2024-04-04 04:10:24.328054 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2210 2024-04-04 04:10:24.328186 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0      612 2024-04-04 04:10:24.328301 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-04-04 04:10:24.328415 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3551 2024-04-04 04:10:24.328546 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.328578 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      608 2024-04-04 04:10:24.328738 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-04-04 04:10:24.328850 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-04-04 04:10:24.328995 patchwork_cli-0.0.3/patchwork/patchflows/README.md
--rw-r--r--   0        0        0      276 2024-04-04 04:10:24.329097 patchwork_cli-0.0.3/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-04-04 04:10:24.329202 patchwork_cli-0.0.3/patchwork/step.py
--rw-r--r--   0        0        0     5970 2024-04-04 04:10:24.329355 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-04-04 04:10:24.329481 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.329529 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0     2437 2024-04-04 04:10:24.329709 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-04-04 04:10:24.329832 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-04-04 04:10:24.329947 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.329981 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-04 04:10:24.330160 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/CallOpenAI.py
--rw-r--r--   0        0        0      503 2024-04-04 04:10:24.330285 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330316 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-04 04:10:24.330494 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-04-04 04:10:24.330605 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330636 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-04 04:10:24.330809 patchwork_cli-0.0.3/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-04-04 04:10:24.330922 patchwork_cli-0.0.3/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330952 patchwork_cli-0.0.3/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0     1358 2024-04-04 04:10:24.331210 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-04-04 04:10:24.331316 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.331443 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0     8850 2024-04-04 04:10:24.331758 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-04-04 04:10:24.331913 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.331952 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.332032 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-04-04 04:10:24.332199 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-04-04 04:10:24.332325 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-04-04 04:10:24.332433 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-04-04 04:10:24.332544 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-04-04 04:10:24.332732 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-04-04 04:10:24.332877 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0     8880 2024-04-04 04:10:24.333049 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-04-04 04:10:24.333176 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.333207 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0     1647 2024-04-04 04:10:24.333385 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-04-04 04:10:24.333529 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.333560 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0    12367 2024-04-04 04:10:24.333765 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-04-04 04:10:24.333884 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-04-04 04:10:24.334021 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334052 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0     3255 2024-04-04 04:10:24.334221 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-04-04 04:10:24.334344 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334374 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-04 04:10:24.334523 patchwork_cli-0.0.3/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-04-04 04:10:24.334875 patchwork_cli-0.0.3/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334943 patchwork_cli-0.0.3/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0     3182 2024-04-04 04:10:24.335255 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-04-04 04:10:24.335372 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.335405 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0     1652 2024-04-04 04:10:24.335557 patchwork_cli-0.0.3/patchwork/steps/README.md
--rw-r--r--   0        0        0      903 2024-04-04 04:10:24.335681 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 04:10:24.335793 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.335826 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-04 04:10:24.335982 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4744 2024-04-04 04:10:24.336123 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0     2026 2024-04-04 04:10:24.336229 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/TestScanDepscan.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.336258 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      677 2024-04-04 04:10:24.336398 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1055 2024-04-04 04:10:24.336499 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-04-04 04:10:24.336528 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0     1481 2024-04-04 04:10:24.336660 patchwork_cli-0.0.3/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     1555 2024-04-04 04:10:24.337840 patchwork_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6258 1970-01-01 00:00:00.000000 patchwork_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5239 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/__main__.py
+-rw-r--r--   0        0        0     2849 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    12408 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0      816 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1546 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/managed_files.py
+-rw-r--r--   0        0        0     2775 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     4783 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      809 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5434 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5418 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      704 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2210 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3832 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      612 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3551 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3631 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0      276 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/step.py
+-rw-r--r--   0        0        0     5970 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0     2437 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0     2822 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/CallOpenAI.py
+-rw-r--r--   0        0        0      503 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0     8811 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0     8880 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0     1648 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0    12392 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0     3344 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0     3182 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0     1652 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/README.md
+-rw-r--r--   0        0        0      903 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1387 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4744 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0     2026 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/TestScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1055 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2101 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 patchwork_cli-0.0.4/PKG-INFO
```

### Comparing `patchwork_cli-0.0.3/LICENSE.txt` & `patchwork_cli-0.0.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -629,16 +629,16 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Affero General Public License for more details.
 
@@ -654,8 +654,8 @@
 of the code.  There are many ways you could offer source, and different
 solutions will be better for different programs; see section 13 for the
 specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+<https://www.gnu.org/licenses/>.
```

### Comparing `patchwork_cli-0.0.3/README.md` & `patchwork_cli-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://github.com/patched-codes/patchwork/assets/126385808/e25f2994-20ac-404e-9089-cf070fb209fb" width="160" alt="PatchWork Logo">
+  <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
 </p>
 
 # PatchWork
 
 An open-source framework for patching and managing code repositories using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
@@ -11,14 +11,22 @@
 - **Steps**: A set of reusable atomic actions that define various operations.
 - **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
 Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
 
 ## Installation
 
+### Using Pip
+
+PatchWork is available on PyPI and can be installed using pip:
+
+```bash
+pip install patchwork-cli --upgrade
+```
+
 ### Using Poetry
 
 PatchWork is built using Poetry, a dependency management and packaging tool for Python. To install PatchWork using Poetry, follow these steps:
 
 1. Make sure you have Poetry installed. If you don't have it installed, you can install it by running:
    ```
    curl -sSL https://install.python-poetry.org | python3 -
@@ -27,15 +35,15 @@
 2. Clone the PatchWork repository:
    ```
    git clone https://github.com/patched-codes/patchwork.git
    ```
 
 3. Navigate to the project directory:
    ```
-   cd patchwork_cli
+   cd patchwork
    ```
 
 4. Activate a shell using virtual environment:
    ```
    poetry shell
    ```
```

### Comparing `patchwork_cli-0.0.3/patchwork/app.py` & `patchwork_cli-0.0.4/patchwork/app.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/common/client/scm.py` & `patchwork_cli-0.0.4/patchwork/common/client/scm.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/common/utils.py` & `patchwork_cli-0.0.4/patchwork/common/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/logger.py` & `patchwork_cli-0.0.4/patchwork/logger.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {'1': "{'prompts': {0: {'content': 'You are an expert software engineer, best in the world at "*

 * *      'migrating code from old version of a library to a new version. Based on the given diff '*

 * *      'generated between old and new versions of a library, please create a list of impacted '*

 * *      'methods along with each method also capture a single line describing what needs to be '*

 * *      'changed in a calling method in order to migrate from old to new version of the library. '*

 * *      'Only include the methods t […]*

```diff
@@ -12,28 +12,28 @@
             }
         ]
     },
     {
         "id": "getimpact",
         "prompts": [
             {
-                "content": "You are an expert software engineer, best in the world at migrating code from old version of a library to a new version. Based on the given diff generated between old and new versions of a library, please create a list of impacted methods along with each method also capture a single line describing what change has been made in the diff. Only include the methods that are modified or removed. Please provide a response only in the following format: \nA. Impacted methods:\n  1. <Method name>:\n    <Impact of the change>\n  2. <Method name>:\n    <Impact of the change>\n  3. <Method name>:\n    <Impact of the change>\n  n. <Method name>:\n    <Impact of the change>\n",
+                "content": "You are an expert software engineer, best in the world at migrating code from old version of a library to a new version. Based on the given diff generated between old and new versions of a library, please create a list of impacted methods along with each method also capture a single line describing what needs to be changed in a calling method in order to migrate from old to new version of the library. Only include the methods that are modified or removed. Please provide a response only in the following format: \nA. Impacted methods:\n  1. <Method name>:\n    <Impact of the change>\n  2. <Method name>:\n    <Impact of the change>\n  3. <Method name>:\n    <Impact of the change>\n  n. <Method name>:\n    <Impact of the change>\n",
                 "role": "system"
             },
             {
                 "content": "{{diffSection}}",
                 "role": "user"
             }
         ]
     },
     {
         "id": "migratecode",
         "prompts": [
             {
-                "content": "You are an expert software engineer, best in the world at migrating code from old version of a library to a new version. You are given a list of methods and the change summary of what was changed in each the method from old to new version. Analyze all the places where you are calling the methods and see if you need to make any changes to migrate them to the new version. Minimize the amount of changes needed for migration. If no changes are necessary return the original code as is. Only respond with the new code, do not add any comments or change the indentation. Make sure you respond with the full code and not only the parts that are changed.\n{{methodInfoList}}",
+                "content": "You are an expert software engineer, best in the world at migrating code from old version of a library to a new version. You are given a list of methods and the change summary of what needs to be changed in a calling method to migrate from old to new version. Analyze all the places where you are calling the methods and see if you need to make any changes to migrate them to the new version. Minimize the amount of changes needed for migration. If no changes are necessary return the original code as is. Only respond with the new code, do not add any comments or change the indentation. Make sure you respond with the full code and not only the parts that are changed.\n{{methodInfoList}}",
                 "role": "system"
             },
             {
                 "content": "{{previousCode}}",
                 "role": "user"
             }
         ]
```

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/PRReview.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/patchflows/README.md` & `patchwork_cli-0.0.4/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/CallOpenAI.py` & `patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/CallOpenAI.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.4/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.4/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.4/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.4/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,28 +192,27 @@
 
                     vulnerability_count = vulnerability_count + 1
                     if 0 < self.vulnerability_limit <= vulnerability_count:
                         break
 
         self.extracted_code_contexts = [
             {
-                "uri": file_path,
+                "uri": str(file_path),
                 "startLine": start,
                 "endLine": end,
                 "affectedCode": context,
                 "messageText": "\n".join(msgs),
             }
             for (file_path, start, end, context), msgs in grouped_messages.items()
         ]
 
         # Save extracted data to JSON
         output_file = Path(tempfile.mktemp(".json"))
         with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(self.extracted_data, f, indent=2)
+            json.dump(self.extracted_code_contexts, f, indent=2)
 
         logger.info(f"Run completed {self.__class__.__name__}")
 
         return dict(
-            prompt_value_file=output_file,
             code_file=output_file,
-            extracted_code_contexts=self.extracted_code_contexts,
+            prompt_values=self.extracted_code_contexts,
         )
```

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     continue
 
                 extracted_response = openai_response
                 for partition in partitions[:-1]:
                     _, _, extracted_response = extracted_response.partition(partition)
 
                 if partitions[-1] != "":
-                    extracted_response, _, _ = extracted_response.partition(partitions[-1])
+                    extracted_response, _, _ = extracted_response.rpartition(partitions[-1])
 
                 if extracted_response == "":
                     continue
 
                 output[key] = extracted_response
             outputs.append(output)
```

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,14 +244,15 @@
         for src_file, data in result.items():
             # Attempt to read the src_file's content
             try:
                 with open(src_file, "r") as file:
                     file_content = file.read()
             except FileNotFoundError:
                 logger.info(f"File not found in the current working directory: {src_file}")
+                continue
 
             lines = file_content.splitlines(keepends=True)
             # Update the structure with the PackageManagerFile content
             update_msg = ""
             for update_info in data["Updates"]:
                 update_msg = (
                     update_msg
```

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.4/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         self.code_snippets_path = inputs[CODE_SNIPPETS_KEY]
         self.extracted_responses = inputs[UPDATED_SNIPPETS_KEY]
 
     def run(self) -> dict:
         code_snippets = load_json_file(self.code_snippets_path)
 
         modified_code_files = []
-        for code_snippet, extracted_response in zip(code_snippets, self.extracted_responses):
+        sorted_list = sorted(zip(code_snippets, self.extracted_responses), key=lambda x: x[0]["startLine"], reverse=True)
+        for code_snippet, extracted_response in sorted_list:
             uri = code_snippet["uri"]
             start_line = code_snippet["startLine"]
             end_line = code_snippet["endLine"]
             new_code = extracted_response.get("patch")
             if new_code is None:
                 continue
```

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.4/patchwork/steps/PreparePR/PreparePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.4/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/README.md` & `patchwork_cli-0.0.4/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/TestScanDepscan.py` & `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/TestScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/patchwork/steps/__init__.py` & `patchwork_cli-0.0.4/patchwork/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.3/pyproject.toml` & `patchwork_cli-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["patched.code"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Quality Assurance",
+    "Topic :: Software Development :: Testing",
+    "Topic :: Utilities"
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "~8.1.0"
 pygithub = "~2.1.1"
 gitpython = "~3.1.40"
 semgrep = "^1.51.0"
```

### Comparing `patchwork_cli-0.0.3/PKG-INFO` & `patchwork_cli-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: AGPL
 Author: patched.code
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: gitpython (>=3.1.40,<3.2.0)
 Requires-Dist: libcst (>=1.2.0,<1.3.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: orjson (>=3.9.15,<3.10.0)
 Requires-Dist: owasp-depscan (>=5.2.12,<6.0.0)
@@ -26,15 +36,15 @@
 Requires-Dist: semgrep (>=1.51.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<3.1.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="https://github.com/patched-codes/patchwork/assets/126385808/e25f2994-20ac-404e-9089-cf070fb209fb" width="160" alt="PatchWork Logo">
+  <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
 </p>
 
 # PatchWork
 
 An open-source framework for patching and managing code repositories using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
@@ -42,14 +52,22 @@
 - **Steps**: A set of reusable atomic actions that define various operations.
 - **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
 Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
 
 ## Installation
 
+### Using Pip
+
+PatchWork is available on PyPI and can be installed using pip:
+
+```bash
+pip install patchwork-cli --upgrade
+```
+
 ### Using Poetry
 
 PatchWork is built using Poetry, a dependency management and packaging tool for Python. To install PatchWork using Poetry, follow these steps:
 
 1. Make sure you have Poetry installed. If you don't have it installed, you can install it by running:
    ```
    curl -sSL https://install.python-poetry.org | python3 -
@@ -58,15 +76,15 @@
 2. Clone the PatchWork repository:
    ```
    git clone https://github.com/patched-codes/patchwork.git
    ```
 
 3. Navigate to the project directory:
    ```
-   cd patchwork_cli
+   cd patchwork
    ```
 
 4. Activate a shell using virtual environment:
    ```
    poetry shell
    ```
```

