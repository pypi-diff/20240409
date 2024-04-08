# Comparing `tmp/ludwig-0.9.2.tar.gz` & `tmp/ludwig-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ludwig-0.9.2.tar", last modified: Wed Jan 17 04:24:59 2024, max compression
+gzip compressed data, was "ludwig-0.9.3.tar", last modified: Tue Jan 23 04:11:03 2024, max compression
```

## Comparing `ludwig-0.9.2.tar` & `ludwig-0.9.3.tar`

### file list

```diff
@@ -1,765 +1,765 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.145802 ludwig-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-01-17 04:24:57.000000 ludwig-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 04:24:57.000000 ludwig-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-01-17 04:24:57.000000 ludwig-0.9.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-01-17 04:24:59.145802 ludwig-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-01-17 04:24:57.000000 ludwig-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.037801 ludwig-0.9.2/ludwig/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.037801 ludwig-0.9.2/ludwig/accounting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/accounting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/accounting/used_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)   110530 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/api_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/automl/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/auto_tune_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15934 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/automl/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/base_automl_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/automl/defaults/combiner/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/combiner/concat_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/combiner/tabnet_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/combiner/transformer_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   101826 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/reference_configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/automl/defaults/text/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/automl/defaults/text/bert_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/_ray210_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    45025 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.041801 ludwig-0.9.2/ludwig/backend/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/backend/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/profiler_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/profiler_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/summary_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/benchmarking/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/combiners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/combiners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42333 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/combiners/combiners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/config_sampling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_sampling/explore_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_sampling/parameter_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/config_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31409 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_validation/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_validation/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/config_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/contribs/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/aim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/comet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.045801 ludwig-0.9.2/ludwig/contribs/mlflow/
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/mlflow/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/contribs/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.049801 ludwig-0.9.2/ludwig/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.049801 ludwig-0.9.2/ludwig/data/batcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/bucketed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/random_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/batcher/test_batcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.049801 ludwig-0.9.2/ludwig/data/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/cache/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/cache/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/cache/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/concatenate_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.049801 ludwig-0.9.2/ludwig/data/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataframe/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataframe/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataframe/modin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataframe/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.049801 ludwig-0.9.2/ludwig/data/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataset/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19286 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataset/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/dataset_synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    92272 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/split_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.053801 ludwig-0.9.2/ludwig/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.065801 ludwig-0.9.2/ludwig/datasets/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/adult_census_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ae_price_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/agnews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/allstate_claims_severity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/alpaca.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/amazon_employee_access_challenge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/amazon_review_polarity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/amazon_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ames_housing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/bbcnews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/bnp_claims_management.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/bookprice_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/california_house_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/code_alpaca.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/connect4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/consumer_complaints.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/consumer_complaints_generation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/creditcard_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/customer_churn_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/data_scientist_salary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/dbpedia.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/electricity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ethos_binary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/fake_job_postings2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/fever.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/flickr8k.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/forest_cover.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/goemotions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/goodbooks_books.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/google_quest_qa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/higgs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/hugging_face.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ieee_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/imbalanced_insurance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/imdb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/imdb_genre_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/insurance_lite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/iris.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/irony.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/jc_penney_products.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/jigsaw_unintended_bias.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/kdd_appetency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/kdd_churn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/kdd_upselling.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/kick_starter_funding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/melbourne_airbnb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/mercari_price_suggestion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/mercari_price_suggestion100K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/mercedes_benz_greener.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/mnist.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/mushroom_edibility.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/naval.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/news_channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/news_popularity2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/noshow_appointments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/numerai28pt6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ohsumed_7400.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/ohsumed_cmu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/otto_group_product.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/poker_hand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/porto_seguro_safe_driver.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/product_sentiment_machine_hack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/protein.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/reuters_cmu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/reuters_r8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/rossman_store_sales.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/santander_customer_satisfaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/santander_customer_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/santander_value_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/sarcastic_headlines.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/sarcos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/sst2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/sst3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/sst5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/synthetic_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/telco_customer_churn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/temperature.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/titanic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/twitter_bots.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/walmart_recruiting.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/wine_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/wmt15.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/women_clothing_review.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/yahoo_answers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/yelp_review_polarity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/yelp_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/configs/yosemite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/kaggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.069801 ludwig-0.9.2/ludwig/datasets/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/adult_census_income.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/agnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/allstate_claims_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/code_alpaca_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/consumer_complaints_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/creditcard_fraud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/dataset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/ethos_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/flickr8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/forest_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/goemotions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/higgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/ieee_fraud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/insurance_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/kdd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/naval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/rossman_store_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/santander_value_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/sarcastic_headlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/sarcos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/split_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/loaders/sst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.073801 ludwig-0.9.2/ludwig/datasets/model_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/adult_census_income_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/ames_housing_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/bnp_claims_management_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/forest_cover_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/higgs_best.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/higgs_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/ieee_fraud_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/mnist_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/mushroom_edibility_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/otto_group_product_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/poker_hand_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/synthetic_fraud_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/model_configs/titanic_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.073801 ludwig-0.9.2/ludwig/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/generic_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/llm_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/sequence_decoder_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/sequence_tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/decoders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.073801 ludwig-0.9.2/ludwig/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/_ray_210_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/distributed/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.077801 ludwig-0.9.2/ludwig/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/generic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/h3_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.077801 ludwig-0.9.2/ludwig/encoders/image/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/image/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24110 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/image/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    95825 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/set_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    99872 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/text_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/encoders/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    21882 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.077801 ludwig-0.9.2/ludwig/explain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24758 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/captum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/captum_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/explanation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/explain/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.081801 ludwig-0.9.2/ludwig/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    23087 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/category_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/date_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/feature_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    41888 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/image_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/number_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    22040 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/sequence_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/set_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/text_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/features/vector_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.081801 ludwig-0.9.2/ludwig/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46845 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/syncer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/hyperopt_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.085801 ludwig-0.9.2/ludwig/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/ecd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    34573 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)    23579 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/models/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.085801 ludwig-0.9.2/ludwig/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/attention_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    48867 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/convolutional_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17081 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/embedding_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/fully_connected_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/initializer_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.089801 ludwig-0.9.2/ludwig/modules/loss_implementations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/loss_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/loss_implementations/corn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/loss_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/metric_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/metric_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/mlp_mixer_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/normalization_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/optimization_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/recurrent_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/reduction_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/tabnet_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/modules/training_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.089801 ludwig-0.9.2/ludwig/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.089801 ludwig-0.9.2/ludwig/schema/combiners/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/common_transformer_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/project_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/sequence_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/combiners/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/common_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.093801 ludwig-0.9.2/ludwig/schema/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/decoders/llm_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/decoders/sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/decoders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.093801 ludwig-0.9.2/ludwig/schema/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/ecd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/defaults/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.093801 ludwig-0.9.2/ludwig/schema/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/h3_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.093801 ludwig-0.9.2/ludwig/schema/encoders/image/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30726 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/image/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/image/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/set_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.097801 ludwig-0.9.2/ludwig/schema/encoders/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/text/hf_model_params.py
--rw-r--r--   0 runner    (1001) docker     (127)   124372 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/text_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/encoders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.097801 ludwig-0.9.2/ludwig/schema/features/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/audio_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.097801 ludwig-0.9.2/ludwig/schema/features/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/augmentation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/augmentation/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/augmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/category_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/date_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/image_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.097801 ludwig-0.9.2/ludwig/schema/features/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/loss/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/number_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.101801 ludwig-0.9.2/ludwig/schema/features/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/bag.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/set.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/preprocessing/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/sequence_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/set_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/text_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/features/vector_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.101801 ludwig-0.9.2/ludwig/schema/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    22089 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/search_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/hyperopt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.105801 ludwig-0.9.2/ludwig/schema/llms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21763 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/llms/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.105801 ludwig-0.9.2/ludwig/schema/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.105801 ludwig-0.9.2/ludwig/schema/metadata/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    89482 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/combiners.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/decoders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   464459 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/encoders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    47655 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/features.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/llm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/loss.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/optimizers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/preprocessing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    45952 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/configs/trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/metadata/parameter_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.109801 ludwig-0.9.2/ludwig/schema/model_types/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/ecd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/model_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    41549 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    48422 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.109801 ludwig-0.9.2/ludwig/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    81844 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    48515 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/trainer_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/trainers/trainer_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.117802 ludwig-0.9.2/ludwig/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/algorithms_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/audio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/augmentation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.117802 ludwig-0.9.2/ludwig/utils/automl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/field_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/ray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/type_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35777 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/batch_size_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/carton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38086 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.121801 ludwig-0.9.2/ludwig/utils/entmax/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/entmax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/entmax/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/entmax/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/entmax/root_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/error_handling_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/gbm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/h3_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/horovod_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/inference_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/llm_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/loss_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/metrics_printed_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/neuropod_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/nlp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/numerical_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/output_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/state_dict_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/strings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/structural_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/system_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50046 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24162 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29019 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/triton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17890 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/upload_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/version_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    45601 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/utils/visualization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.121801 ludwig-0.9.2/ludwig/vector_index/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/vector_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/vector_index/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/vector_index/faiss.py
--rw-r--r--   0 runner    (1001) docker     (127)   169425 2024-01-17 04:24:57.000000 ludwig-0.9.2/ludwig/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.037801 ludwig-0.9.2/ludwig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25859 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-17 04:24:58.000000 ludwig-0.9.2/ludwig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-17 04:24:57.000000 ludwig-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_benchmarking.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_distributed.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_hyperopt.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_llm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_serve.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_tree.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-17 04:24:57.000000 ludwig-0.9.2/requirements_viz.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-17 04:24:59.145802 ludwig-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-01-17 04:24:57.000000 ludwig-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.029801 ludwig-0.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.129802 ludwig-0.9.2/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/parameter_update_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/synthetic_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    30727 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_automl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_cached_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_carton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_class_imbalance_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_config_global_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_contrib_aim.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_contrib_comet.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_contrib_wandb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_custom_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_date_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    45975 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_graph_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)    23442 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_hyperopt_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_hyperopt_ray_horovod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_input_feature_tied.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_kfold_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    45735 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_missing_value_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_model_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18376 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_model_training_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_neuropod.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_number_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41854 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    39944 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_sequence_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_simple_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)    16673 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_triton.py
--rw-r--r--   0 runner    (1001) docker     (127)    60772 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    38601 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/test_visualization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    40405 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/integration_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.129802 ludwig-0.9.2/tests/ludwig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.129802 ludwig-0.9.2/tests/ludwig/automl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/automl/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/automl/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/automl/test_tune_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/automl/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.133802 ludwig-0.9.2/tests/ludwig/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/check_dead_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/download_all_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/test_dataset_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/datasets/test_model_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.133802 ludwig-0.9.2/tests/ludwig/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_generic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_h3_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_image_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_llm_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_set_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/encoders/test_text_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.137802 ludwig-0.9.2/tests/ludwig/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_category_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_date_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_image_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_number_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_sequence_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_set_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_text_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/features/test_timeseries_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.137802 ludwig-0.9.2/tests/ludwig/models/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/models/test_trainable_image_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/models/test_training_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/models/test_training_success.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.137802 ludwig-0.9.2/tests/ludwig/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_convolutional_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_embedding_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_fully_connected_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_initializer_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_loss_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_metric_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_mlp_mixer_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_normalization_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_recurrent_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_reduction_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_tabnet_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/modules/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.145802 ludwig-0.9.2/tests/ludwig/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_algorithm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_audio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30352 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_class_balancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_error_handling_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_hyperopt_ray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_numerical_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_output_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_state_dict_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_strings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_upload_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/ludwig/utils/test_version_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:59.145802 ludwig-0.9.2/tests/training_success/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/training_success/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/training_success/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-01-17 04:24:57.000000 ludwig-0.9.2/tests/training_success/test_training_success.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.739816 ludwig-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-01-23 04:11:01.000000 ludwig-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-23 04:11:01.000000 ludwig-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-01-23 04:11:01.000000 ludwig-0.9.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-01-23 04:11:03.739816 ludwig-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-01-23 04:11:01.000000 ludwig-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.639817 ludwig-0.9.3/ludwig/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/accounting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/accounting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/accounting/used_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110530 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/api_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/automl/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/auto_tune_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15934 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/automl/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/base_automl_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/automl/defaults/combiner/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/combiner/concat_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/combiner/tabnet_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/combiner/transformer_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   101826 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/reference_configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/automl/defaults/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/automl/defaults/text/bert_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/_ray210_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45025 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.647817 ludwig-0.9.3/ludwig/backend/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/backend/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.647817 ludwig-0.9.3/ludwig/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/profiler_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/profiler_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17773 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/summary_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/benchmarking/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.647817 ludwig-0.9.3/ludwig/combiners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/combiners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42333 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/combiners/combiners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.647817 ludwig-0.9.3/ludwig/config_sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_sampling/explore_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_sampling/parameter_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.647817 ludwig-0.9.3/ludwig/config_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31409 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_validation/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_validation/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/config_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.651817 ludwig-0.9.3/ludwig/contribs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/comet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.651817 ludwig-0.9.3/ludwig/contribs/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/mlflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/contribs/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.651817 ludwig-0.9.3/ludwig/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.651817 ludwig-0.9.3/ludwig/data/batcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/bucketed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/random_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/batcher/test_batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.651817 ludwig-0.9.3/ludwig/data/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/cache/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/cache/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/cache/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/concatenate_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.655817 ludwig-0.9.3/ludwig/data/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataframe/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataframe/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataframe/modin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataframe/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.655817 ludwig-0.9.3/ludwig/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataset/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19286 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataset/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/dataset_synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92272 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/split_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.655817 ludwig-0.9.3/ludwig/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.667817 ludwig-0.9.3/ludwig/datasets/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/adult_census_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ae_price_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/agnews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/allstate_claims_severity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/alpaca.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/amazon_employee_access_challenge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/amazon_review_polarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/amazon_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ames_housing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/bbcnews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/bnp_claims_management.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/bookprice_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/california_house_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/code_alpaca.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/connect4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/consumer_complaints.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/consumer_complaints_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/creditcard_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/customer_churn_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/data_scientist_salary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/dbpedia.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/electricity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ethos_binary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/fake_job_postings2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/fever.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/flickr8k.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/forest_cover.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/goemotions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/goodbooks_books.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/google_quest_qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/higgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/hugging_face.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ieee_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/imbalanced_insurance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/imdb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/imdb_genre_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/insurance_lite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/iris.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/irony.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/jc_penney_products.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/jigsaw_unintended_bias.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/kdd_appetency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/kdd_churn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/kdd_upselling.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/kick_starter_funding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/melbourne_airbnb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/mercari_price_suggestion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/mercari_price_suggestion100K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/mercedes_benz_greener.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/mnist.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/mushroom_edibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/naval.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/news_channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/news_popularity2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/noshow_appointments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/numerai28pt6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ohsumed_7400.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/ohsumed_cmu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/otto_group_product.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/poker_hand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/porto_seguro_safe_driver.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/product_sentiment_machine_hack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/protein.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/reuters_cmu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/reuters_r8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/rossman_store_sales.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/santander_customer_satisfaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/santander_customer_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/santander_value_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/sarcastic_headlines.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/sarcos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/sst2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/sst3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/sst5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/synthetic_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/telco_customer_churn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/temperature.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/titanic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/twitter_bots.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/walmart_recruiting.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/wine_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/wmt15.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/women_clothing_review.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/yahoo_answers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/yelp_review_polarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/yelp_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/configs/yosemite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/kaggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.671817 ludwig-0.9.3/ludwig/datasets/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/adult_census_income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/agnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/allstate_claims_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/code_alpaca_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/consumer_complaints_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/creditcard_fraud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/dataset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/ethos_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/flickr8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/forest_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/goemotions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/higgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/ieee_fraud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/insurance_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/kdd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/naval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/rossman_store_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/santander_value_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/sarcastic_headlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/sarcos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/split_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/loaders/sst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.675817 ludwig-0.9.3/ludwig/datasets/model_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/adult_census_income_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/ames_housing_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/bnp_claims_management_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/forest_cover_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/higgs_best.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/higgs_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/ieee_fraud_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/mnist_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/mushroom_edibility_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/otto_group_product_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/poker_hand_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/synthetic_fraud_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/model_configs/titanic_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.675817 ludwig-0.9.3/ludwig/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/generic_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/llm_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/sequence_decoder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/sequence_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/decoders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.675817 ludwig-0.9.3/ludwig/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/_ray_210_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/distributed/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.679817 ludwig-0.9.3/ludwig/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/generic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/h3_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.679817 ludwig-0.9.3/ludwig/encoders/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/image/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24110 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/image/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95825 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/set_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100102 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/text_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/encoders/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21882 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.679817 ludwig-0.9.3/ludwig/explain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24758 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/captum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/captum_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/explain/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.683817 ludwig-0.9.3/ludwig/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23087 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/feature_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41888 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/image_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22040 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/sequence_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/features/vector_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.683817 ludwig-0.9.3/ludwig/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46845 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/syncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/hyperopt_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.687816 ludwig-0.9.3/ludwig/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34573 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23579 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/models/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.687816 ludwig-0.9.3/ludwig/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/attention_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48867 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/convolutional_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17081 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/embedding_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/fully_connected_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/initializer_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.687816 ludwig-0.9.3/ludwig/modules/loss_implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/loss_implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/loss_implementations/corn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/loss_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/metric_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/metric_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/mlp_mixer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/normalization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/optimization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/recurrent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/reduction_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/tabnet_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/modules/training_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.691817 ludwig-0.9.3/ludwig/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.691817 ludwig-0.9.3/ludwig/schema/combiners/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/common_transformer_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/project_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/sequence_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/combiners/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/common_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.691817 ludwig-0.9.3/ludwig/schema/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/decoders/llm_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/decoders/sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/decoders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.695817 ludwig-0.9.3/ludwig/schema/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/defaults/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.695817 ludwig-0.9.3/ludwig/schema/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/h3_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.695817 ludwig-0.9.3/ludwig/schema/encoders/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30726 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/image/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/image/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/set_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.695817 ludwig-0.9.3/ludwig/schema/encoders/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/text/hf_model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124372 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/text_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/encoders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.699817 ludwig-0.9.3/ludwig/schema/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/audio_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.699817 ludwig-0.9.3/ludwig/schema/features/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/augmentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/augmentation/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/augmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/image_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.699817 ludwig-0.9.3/ludwig/schema/features/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/loss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/number_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.703817 ludwig-0.9.3/ludwig/schema/features/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/bag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/preprocessing/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/sequence_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/features/vector_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.703817 ludwig-0.9.3/ludwig/schema/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22089 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/search_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/hyperopt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.703817 ludwig-0.9.3/ludwig/schema/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21763 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/llms/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.703817 ludwig-0.9.3/ludwig/schema/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.707816 ludwig-0.9.3/ludwig/schema/metadata/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    89482 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/combiners.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26192 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/decoders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   464459 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/encoders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    47655 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/features.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/llm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/loss.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/optimizers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/preprocessing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    45952 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/configs/trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/metadata/parameter_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.707816 ludwig-0.9.3/ludwig/schema/model_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/model_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41549 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48422 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.707816 ludwig-0.9.3/ludwig/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48515 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/trainer_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23805 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/trainers/trainer_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.715816 ludwig-0.9.3/ludwig/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/algorithms_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/audio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/augmentation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.719817 ludwig-0.9.3/ludwig/utils/automl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/field_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/ray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/type_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35777 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/batch_size_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/carton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38086 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.719817 ludwig-0.9.3/ludwig/utils/entmax/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/entmax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/entmax/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/entmax/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/entmax/root_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/error_handling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/gbm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/h3_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/horovod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/inference_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/llm_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27792 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/loss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/metrics_printed_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/neuropod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/nlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/numerical_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/output_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/state_dict_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21574 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/strings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/structural_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50266 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24162 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29019 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/triton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17890 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/version_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45601 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/utils/visualization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.719817 ludwig-0.9.3/ludwig/vector_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/vector_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/vector_index/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/vector_index/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169425 2024-01-23 04:11:01.000000 ludwig-0.9.3/ludwig/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.643817 ludwig-0.9.3/ludwig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25859 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-23 04:11:03.000000 ludwig-0.9.3/ludwig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-23 04:11:01.000000 ludwig-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_benchmarking.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_distributed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_hyperopt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_llm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_serve.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_tree.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-23 04:11:01.000000 ludwig-0.9.3/requirements_viz.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-23 04:11:03.739816 ludwig-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-01-23 04:11:01.000000 ludwig-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.635817 ludwig-0.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.727816 ludwig-0.9.3/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/parameter_update_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/synthetic_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30727 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_automl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_cached_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_carton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_class_imbalance_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_config_global_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_contrib_aim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_contrib_comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_contrib_wandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_custom_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45975 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_graph_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23442 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_hyperopt_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_hyperopt_ray_horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_input_feature_tied.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_kfold_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46761 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_missing_value_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_model_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18376 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_model_training_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_neuropod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41854 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39944 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_sequence_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_simple_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16673 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60772 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38601 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/test_visualization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40405 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/integration_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.727816 ludwig-0.9.3/tests/ludwig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.727816 ludwig-0.9.3/tests/ludwig/automl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/automl/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/automl/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/automl/test_tune_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/automl/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.731816 ludwig-0.9.3/tests/ludwig/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/check_dead_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/download_all_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/test_dataset_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/datasets/test_model_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.731816 ludwig-0.9.3/tests/ludwig/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_generic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_h3_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_image_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_llm_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_set_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/encoders/test_text_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.731816 ludwig-0.9.3/tests/ludwig/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_image_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_sequence_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/features/test_timeseries_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.735816 ludwig-0.9.3/tests/ludwig/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/models/test_trainable_image_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/models/test_training_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/models/test_training_success.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.735816 ludwig-0.9.3/tests/ludwig/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_convolutional_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_embedding_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_fully_connected_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_initializer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_loss_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_metric_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_mlp_mixer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_normalization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_recurrent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_reduction_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_tabnet_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/modules/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.739816 ludwig-0.9.3/tests/ludwig/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_algorithm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_audio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30352 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_class_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_error_handling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_hyperopt_ray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_numerical_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_output_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_state_dict_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_strings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/ludwig/utils/test_version_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:03.739816 ludwig-0.9.3/tests/training_success/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/training_success/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/training_success/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-01-23 04:11:01.000000 ludwig-0.9.3/tests/training_success/test_training_success.py
```

### Comparing `ludwig-0.9.2/LICENSE` & `ludwig-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/NOTICE` & `ludwig-0.9.3/NOTICE`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/PKG-INFO` & `ludwig-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ludwig
-Version: 0.9.2
+Version: 0.9.3
 Summary: Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.
 Home-page: https://github.com/ludwig-ai/ludwig
 Author: Piero Molino
 Author-email: piero.molino@gmail.com
 License: Apache 2.0
 Download-URL: https://pypi.org/project/ludwig/
 Description: <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ludwig Version: 0.9.2 Summary: Declarative machine
+Metadata-Version: 2.1 Name: ludwig Version: 0.9.3 Summary: Declarative machine
 learning: End-to-end machine learning pipelines using data-driven
 configurations. Home-page: https://github.com/ludwig-ai/ludwig Author: Piero
 Molino Author-email: piero.molino@gmail.com License: Apache 2.0 Download-URL:
 https://pypi.org/project/ludwig/ Description:
        _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_u_d_w_i_g_-_a_i_/_l_u_d_w_i_g_-_d_o_c_s_/_r_a_w_/_m_a_s_t_e_r_/_d_o_c_s_/_i_m_a_g_e_s_/
                            _l_u_d_w_i_g___h_e_r_o___s_m_a_l_l_e_r_._j_p_g_]
  _Declarative deep learning framework built for scale and efficiency._ [![PyPI
```

### Comparing `ludwig-0.9.2/README.md` & `ludwig-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/__init__.py` & `ludwig-0.9.3/ludwig/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/accounting/used_tokens.py` & `ludwig-0.9.3/ludwig/accounting/used_tokens.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/api.py` & `ludwig-0.9.3/ludwig/api.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/api_annotations.py` & `ludwig-0.9.3/ludwig/api_annotations.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/auto_tune_config.py` & `ludwig-0.9.3/ludwig/automl/auto_tune_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/automl.py` & `ludwig-0.9.3/ludwig/automl/automl.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/base_config.py` & `ludwig-0.9.3/ludwig/automl/base_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/defaults/combiner/concat_config.yaml` & `ludwig-0.9.3/ludwig/automl/defaults/combiner/concat_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/defaults/combiner/tabnet_config.yaml` & `ludwig-0.9.3/ludwig/automl/defaults/combiner/tabnet_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/defaults/combiner/transformer_config.yaml` & `ludwig-0.9.3/ludwig/automl/defaults/combiner/transformer_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/defaults/reference_configs.yaml` & `ludwig-0.9.3/ludwig/automl/defaults/reference_configs.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/automl/defaults/text/bert_config.yaml` & `ludwig-0.9.3/ludwig/automl/defaults/text/bert_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/__init__.py` & `ludwig-0.9.3/ludwig/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/_ray210_compat.py` & `ludwig-0.9.3/ludwig/backend/_ray210_compat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/base.py` & `ludwig-0.9.3/ludwig/backend/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/datasource.py` & `ludwig-0.9.3/ludwig/backend/datasource.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/deepspeed.py` & `ludwig-0.9.3/ludwig/backend/deepspeed.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/horovod.py` & `ludwig-0.9.3/ludwig/backend/horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/ray.py` & `ludwig-0.9.3/ludwig/backend/ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/backend/utils/storage.py` & `ludwig-0.9.3/ludwig/backend/utils/storage.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/artifacts.py` & `ludwig-0.9.3/ludwig/benchmarking/artifacts.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/benchmark.py` & `ludwig-0.9.3/ludwig/benchmarking/benchmark.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/profiler.py` & `ludwig-0.9.3/ludwig/benchmarking/profiler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/profiler_callbacks.py` & `ludwig-0.9.3/ludwig/benchmarking/profiler_callbacks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/profiler_dataclasses.py` & `ludwig-0.9.3/ludwig/benchmarking/profiler_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/reporting.py` & `ludwig-0.9.3/ludwig/benchmarking/reporting.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/summarize.py` & `ludwig-0.9.3/ludwig/benchmarking/summarize.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/summary_dataclasses.py` & `ludwig-0.9.3/ludwig/benchmarking/summary_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/benchmarking/utils.py` & `ludwig-0.9.3/ludwig/benchmarking/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/callbacks.py` & `ludwig-0.9.3/ludwig/callbacks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/check.py` & `ludwig-0.9.3/ludwig/check.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/cli.py` & `ludwig-0.9.3/ludwig/cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/collect.py` & `ludwig-0.9.3/ludwig/collect.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/combiners/combiners.py` & `ludwig-0.9.3/ludwig/combiners/combiners.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/config_sampling/explore_schema.py` & `ludwig-0.9.3/ludwig/config_sampling/explore_schema.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/config_sampling/parameter_sampling.py` & `ludwig-0.9.3/ludwig/config_sampling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/config_validation/checks.py` & `ludwig-0.9.3/ludwig/config_validation/checks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/config_validation/preprocessing.py` & `ludwig-0.9.3/ludwig/config_validation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/config_validation/validation.py` & `ludwig-0.9.3/ludwig/config_validation/validation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/constants.py` & `ludwig-0.9.3/ludwig/constants.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contrib.py` & `ludwig-0.9.3/ludwig/contrib.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/__init__.py` & `ludwig-0.9.3/ludwig/contribs/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/aim.py` & `ludwig-0.9.3/ludwig/contribs/aim.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/comet.py` & `ludwig-0.9.3/ludwig/contribs/comet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/mlflow/__init__.py` & `ludwig-0.9.3/ludwig/contribs/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/mlflow/model.py` & `ludwig-0.9.3/ludwig/contribs/mlflow/model.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/contribs/wandb.py` & `ludwig-0.9.3/ludwig/contribs/wandb.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/batcher/base.py` & `ludwig-0.9.3/ludwig/data/batcher/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/batcher/bucketed.py` & `ludwig-0.9.3/ludwig/data/batcher/bucketed.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/batcher/iterable.py` & `ludwig-0.9.3/ludwig/data/batcher/iterable.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/batcher/random_access.py` & `ludwig-0.9.3/ludwig/data/batcher/random_access.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/batcher/test_batcher.py` & `ludwig-0.9.3/ludwig/data/batcher/test_batcher.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/cache/manager.py` & `ludwig-0.9.3/ludwig/data/cache/manager.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/cache/types.py` & `ludwig-0.9.3/ludwig/data/cache/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/cache/util.py` & `ludwig-0.9.3/ludwig/data/cache/util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/concatenate_datasets.py` & `ludwig-0.9.3/ludwig/data/concatenate_datasets.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataframe/__init__.py` & `ludwig-0.9.3/ludwig/data/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataframe/base.py` & `ludwig-0.9.3/ludwig/data/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataframe/dask.py` & `ludwig-0.9.3/ludwig/data/dataframe/dask.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataframe/modin.py` & `ludwig-0.9.3/ludwig/data/dataframe/modin.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataframe/pandas.py` & `ludwig-0.9.3/ludwig/data/dataframe/pandas.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataset/__init__.py` & `ludwig-0.9.3/ludwig/data/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataset/base.py` & `ludwig-0.9.3/ludwig/data/dataset/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataset/pandas.py` & `ludwig-0.9.3/ludwig/data/dataset/pandas.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataset/ray.py` & `ludwig-0.9.3/ludwig/data/dataset/ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/dataset_synthesizer.py` & `ludwig-0.9.3/ludwig/data/dataset_synthesizer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/negative_sampling.py` & `ludwig-0.9.3/ludwig/data/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/postprocessing.py` & `ludwig-0.9.3/ludwig/data/postprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/preprocessing.py` & `ludwig-0.9.3/ludwig/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/prompt.py` & `ludwig-0.9.3/ludwig/data/prompt.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/sampler.py` & `ludwig-0.9.3/ludwig/data/sampler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/split.py` & `ludwig-0.9.3/ludwig/data/split.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/split_dataset.py` & `ludwig-0.9.3/ludwig/data/split_dataset.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/data/utils.py` & `ludwig-0.9.3/ludwig/data/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/__init__.py` & `ludwig-0.9.3/ludwig/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/archives.py` & `ludwig-0.9.3/ludwig/datasets/archives.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/adult_census_income.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/adult_census_income.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ae_price_prediction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ae_price_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/agnews.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/agnews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/amazon_employee_access_challenge.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/amazon_employee_access_challenge.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/amazon_review_polarity.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/amazon_review_polarity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/amazon_reviews.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/amazon_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ames_housing.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ames_housing.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/bnp_claims_management.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/bnp_claims_management.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/bookprice_prediction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/bookprice_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/california_house_price.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/california_house_price.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/code_alpaca.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/code_alpaca.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/connect4.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/connect4.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/consumer_complaints.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/consumer_complaints.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/consumer_complaints_generation.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/consumer_complaints_generation.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/creditcard_fraud.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/creditcard_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/customer_churn_prediction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/customer_churn_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/data_scientist_salary.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/data_scientist_salary.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/dbpedia.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/dbpedia.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/electricity.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/electricity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ethos_binary.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ethos_binary.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/fake_job_postings2.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/fake_job_postings2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/fever.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/fever.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/flickr8k.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/flickr8k.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/forest_cover.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/forest_cover.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/goemotions.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/goemotions.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/goodbooks_books.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/goodbooks_books.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/google_quest_qa.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/google_quest_qa.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/higgs.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/higgs.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ieee_fraud.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ieee_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/imbalanced_insurance.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/imbalanced_insurance.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/imdb.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/imdb.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/imdb_genre_prediction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/imdb_genre_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/insurance_lite.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/insurance_lite.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/iris.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/iris.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/irony.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/irony.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/jc_penney_products.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/jc_penney_products.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/jigsaw_unintended_bias.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/jigsaw_unintended_bias.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/kdd_appetency.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/kdd_appetency.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/kdd_churn.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/kdd_churn.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/kdd_upselling.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/kdd_upselling.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/kick_starter_funding.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/kick_starter_funding.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/melbourne_airbnb.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/melbourne_airbnb.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/mercari_price_suggestion.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/mercari_price_suggestion.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/mercari_price_suggestion100K.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/mercari_price_suggestion100K.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/mercedes_benz_greener.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/mercedes_benz_greener.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/mnist.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/mnist.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/mushroom_edibility.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/mushroom_edibility.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/naval.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/naval.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/news_channel.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/news_channel.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/news_popularity2.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/news_popularity2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/noshow_appointments.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/noshow_appointments.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/numerai28pt6.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/numerai28pt6.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ohsumed_7400.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ohsumed_7400.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/ohsumed_cmu.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/ohsumed_cmu.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/otto_group_product.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/otto_group_product.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/poker_hand.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/poker_hand.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/porto_seguro_safe_driver.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/porto_seguro_safe_driver.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/product_sentiment_machine_hack.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/product_sentiment_machine_hack.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/protein.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/protein.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/reuters_cmu.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/reuters_cmu.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/reuters_r8.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/reuters_r8.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/rossman_store_sales.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/rossman_store_sales.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/santander_customer_transaction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/santander_customer_transaction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/santander_value_prediction.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/santander_value_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/sarcastic_headlines.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/sarcastic_headlines.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/sarcos.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/sarcos.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/sst2.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/sst2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/sst3.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/sst3.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/sst5.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/sst5.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/synthetic_fraud.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/synthetic_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/telco_customer_churn.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/telco_customer_churn.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/temperature.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/temperature.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/twitter_bots.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/twitter_bots.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/wine_reviews.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/wine_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/women_clothing_review.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/women_clothing_review.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/yahoo_answers.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/yahoo_answers.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/yelp_review_polarity.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/yelp_review_polarity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/configs/yelp_reviews.yaml` & `ludwig-0.9.3/ludwig/datasets/configs/yelp_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/dataset_config.py` & `ludwig-0.9.3/ludwig/datasets/dataset_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/kaggle.py` & `ludwig-0.9.3/ludwig/datasets/kaggle.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/adult_census_income.py` & `ludwig-0.9.3/ludwig/datasets/loaders/adult_census_income.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/agnews.py` & `ludwig-0.9.3/ludwig/datasets/loaders/agnews.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/allstate_claims_severity.py` & `ludwig-0.9.3/ludwig/datasets/loaders/allstate_claims_severity.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/code_alpaca_loader.py` & `ludwig-0.9.3/ludwig/datasets/loaders/code_alpaca_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/consumer_complaints_loader.py` & `ludwig-0.9.3/ludwig/datasets/loaders/consumer_complaints_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/creditcard_fraud.py` & `ludwig-0.9.3/ludwig/datasets/loaders/creditcard_fraud.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/dataset_loader.py` & `ludwig-0.9.3/ludwig/datasets/loaders/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/ethos_binary.py` & `ludwig-0.9.3/ludwig/datasets/loaders/ethos_binary.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/flickr8k.py` & `ludwig-0.9.3/ludwig/datasets/loaders/flickr8k.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/forest_cover.py` & `ludwig-0.9.3/ludwig/datasets/loaders/forest_cover.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/goemotions.py` & `ludwig-0.9.3/ludwig/datasets/loaders/goemotions.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/higgs.py` & `ludwig-0.9.3/ludwig/datasets/loaders/higgs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/hugging_face.py` & `ludwig-0.9.3/ludwig/datasets/loaders/hugging_face.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/ieee_fraud.py` & `ludwig-0.9.3/ludwig/datasets/loaders/ieee_fraud.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/insurance_lite.py` & `ludwig-0.9.3/ludwig/datasets/loaders/insurance_lite.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/kdd_loader.py` & `ludwig-0.9.3/ludwig/datasets/loaders/kdd_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/mnist.py` & `ludwig-0.9.3/ludwig/datasets/loaders/mnist.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/naval.py` & `ludwig-0.9.3/ludwig/datasets/loaders/naval.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/rossman_store_sales.py` & `ludwig-0.9.3/ludwig/datasets/loaders/rossman_store_sales.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/santander_value_prediction.py` & `ludwig-0.9.3/ludwig/datasets/loaders/santander_value_prediction.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/sarcastic_headlines.py` & `ludwig-0.9.3/ludwig/datasets/loaders/sarcastic_headlines.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/sarcos.py` & `ludwig-0.9.3/ludwig/datasets/loaders/sarcos.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/split_loaders.py` & `ludwig-0.9.3/ludwig/datasets/loaders/split_loaders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/loaders/sst.py` & `ludwig-0.9.3/ludwig/datasets/loaders/sst.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/adult_census_income_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/adult_census_income_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/ames_housing_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/ames_housing_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/bnp_claims_management_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/bnp_claims_management_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/forest_cover_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/forest_cover_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/higgs_best.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/higgs_best.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/higgs_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/higgs_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/ieee_fraud_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/ieee_fraud_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/mushroom_edibility_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/mushroom_edibility_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/otto_group_product_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/otto_group_product_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/poker_hand_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/poker_hand_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml` & `ludwig-0.9.3/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/datasets/utils.py` & `ludwig-0.9.3/ludwig/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/base.py` & `ludwig-0.9.3/ludwig/decoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/generic_decoders.py` & `ludwig-0.9.3/ludwig/decoders/generic_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/llm_decoders.py` & `ludwig-0.9.3/ludwig/decoders/llm_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/registry.py` & `ludwig-0.9.3/ludwig/decoders/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/sequence_decoder_utils.py` & `ludwig-0.9.3/ludwig/decoders/sequence_decoder_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/sequence_decoders.py` & `ludwig-0.9.3/ludwig/decoders/sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/sequence_tagger.py` & `ludwig-0.9.3/ludwig/decoders/sequence_tagger.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/decoders/utils.py` & `ludwig-0.9.3/ludwig/decoders/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/__init__.py` & `ludwig-0.9.3/ludwig/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/_ray_210_compat.py` & `ludwig-0.9.3/ludwig/distributed/_ray_210_compat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/base.py` & `ludwig-0.9.3/ludwig/distributed/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/ddp.py` & `ludwig-0.9.3/ludwig/distributed/ddp.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/deepspeed.py` & `ludwig-0.9.3/ludwig/distributed/deepspeed.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/fsdp.py` & `ludwig-0.9.3/ludwig/distributed/fsdp.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/distributed/horovod.py` & `ludwig-0.9.3/ludwig/distributed/horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/bag_encoders.py` & `ludwig-0.9.3/ludwig/encoders/bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/base.py` & `ludwig-0.9.3/ludwig/encoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/category_encoders.py` & `ludwig-0.9.3/ludwig/encoders/category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/date_encoders.py` & `ludwig-0.9.3/ludwig/encoders/date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/generic_encoders.py` & `ludwig-0.9.3/ludwig/encoders/generic_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/h3_encoders.py` & `ludwig-0.9.3/ludwig/encoders/h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/image/base.py` & `ludwig-0.9.3/ludwig/encoders/image/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/image/torchvision.py` & `ludwig-0.9.3/ludwig/encoders/image/torchvision.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/registry.py` & `ludwig-0.9.3/ludwig/encoders/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/sequence_encoders.py` & `ludwig-0.9.3/ludwig/encoders/sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/set_encoders.py` & `ludwig-0.9.3/ludwig/encoders/set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/encoders/text_encoders.py` & `ludwig-0.9.3/ludwig/encoders/text_encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -2383,15 +2383,19 @@
 
 
 @DeveloperAPI
 @register_encoder("llm", [TEXT])
 class LLMEncoder(Encoder):
     # Per-adapter type prefixes for parameter names in the state dict, taken from
     # https://github.com/huggingface/peft/blob/0f1e9091cc975eb5458cc163bf1843a34fb42b76/src/peft/utils/save_and_load.py#L173C9-L180
-    ADAPTER_PARAM_NAME_PREFIX = {"lora": "lora_", "adalora": "lora_"}
+    ADAPTER_PARAM_NAME_PREFIX = {
+        "adalora": "lora_",
+        "ia3": "ia3_",
+        "lora": "lora_",
+    }
 
     def __init__(self, encoder_config: LLMEncoderConfig = None, **kwargs):
         super().__init__()
         self.register_load_state_dict_post_hook(self.remove_missing_non_adapter_keys)
 
         self.config = encoder_config
 
@@ -2421,14 +2425,22 @@
         # Initialize tokenizer
         self.tokenizer = HFTokenizer(self.config.base_model).tokenizer
 
         self.attention_masks = None
 
         clear_data_cache()
 
+        # Because we use the last hidden state as encoder output rather than the logits, the final module of the model
+        # has input pass through but no gradient update in the backward pass. This can lead to a DDP error. Freezing
+        # the module prevents this from happening. This is done at initialization to prevent "unused parameters" errors
+        # from happening when the encoder is used before `prepare_for_training` is called, for example during batch
+        # size tuning.
+        out_module = list(self.model.modules())[-1]
+        out_module.requires_grad_(requires_grad=False)
+
     @staticmethod
     def get_schema_cls() -> Type[BaseEncoderConfig]:
         return LLMEncoderConfig
 
     @property
     def input_shape(self) -> torch.Size:
         return torch.Size([self.max_sequence_length])
@@ -2455,35 +2467,28 @@
 
     def prepare_for_training(self):
         # TODO: this implementation will not work if resuming from a previous checkpoint. Need to fix this.
         if self.config.quantization:
             self.prepare_for_quantized_training()
         self.initialize_adapter()
 
-        # Because we use the last hidden state as encoder output rather than the logits, the final module of the model
-        # has input pass through but no gradient update in the backward pass. This can lead to a DDP error. Freezing
-        # the module prevents this from happening.
-        if not self.config.adapter:
-            out_module = list(self.model.modules())[-1]
-            out_module.requires_grad_(requires_grad=False)
-
     def prepare_for_quantized_training(self):
         from peft import prepare_model_for_kbit_training
 
         self.model = prepare_model_for_kbit_training(self.model, use_gradient_checkpointing=False)
 
     def forward(self, inputs: torch.Tensor, mask: Optional[torch.Tensor] = None):
         # Wrap with flash attention backend for faster generation
         with torch.backends.cuda.sdp_kernel(enable_flash=True, enable_math=False, enable_mem_efficient=False) if (
             torch.cuda.is_available() and self.curr_device.type == "cuda"
         ) else contextlib.nullcontext():
             # Get the hidden state of the last layer and return it as the text encoding
             model_outputs = self.model(input_ids=inputs, output_hidden_states=True).hidden_states[-1]
 
-        return {ENCODER_OUTPUT: model_outputs}
+        return {ENCODER_OUTPUT: model_outputs.type(torch.float32)}
 
     def _save_to_state_dict(self, destination: Dict, prefix: str, keep_vars: bool):
         # This is called by `torch.nn.Module.state_dict()` under the hood. `state_dict()` does additional work to
         # prep the dictionary, get submodule state, and run hooks. Overriding this method only impacts the
         # contents of the state_dict.
         # The three args to this method are supplied by Module.state_dict
         # https://github.com/pytorch/pytorch/blob/8739d1e3f9b08f4282fe79fc8dacd781d16913ff/torch/nn/modules/module.py#L1824
```

### Comparing `ludwig-0.9.2/ludwig/error.py` & `ludwig-0.9.3/ludwig/error.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/evaluate.py` & `ludwig-0.9.3/ludwig/evaluate.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/experiment.py` & `ludwig-0.9.3/ludwig/experiment.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/captum.py` & `ludwig-0.9.3/ludwig/explain/captum.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/captum_ray.py` & `ludwig-0.9.3/ludwig/explain/captum_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/explainer.py` & `ludwig-0.9.3/ludwig/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/explanation.py` & `ludwig-0.9.3/ludwig/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/gbm.py` & `ludwig-0.9.3/ludwig/explain/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/explain/util.py` & `ludwig-0.9.3/ludwig/explain/util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/export.py` & `ludwig-0.9.3/ludwig/export.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/audio_feature.py` & `ludwig-0.9.3/ludwig/features/audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/bag_feature.py` & `ludwig-0.9.3/ludwig/features/bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/base_feature.py` & `ludwig-0.9.3/ludwig/features/base_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/binary_feature.py` & `ludwig-0.9.3/ludwig/features/binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/category_feature.py` & `ludwig-0.9.3/ludwig/features/category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/date_feature.py` & `ludwig-0.9.3/ludwig/features/date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/feature_registries.py` & `ludwig-0.9.3/ludwig/features/feature_registries.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/feature_utils.py` & `ludwig-0.9.3/ludwig/features/feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/h3_feature.py` & `ludwig-0.9.3/ludwig/features/h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/image_feature.py` & `ludwig-0.9.3/ludwig/features/image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/number_feature.py` & `ludwig-0.9.3/ludwig/features/number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/sequence_feature.py` & `ludwig-0.9.3/ludwig/features/sequence_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/set_feature.py` & `ludwig-0.9.3/ludwig/features/set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/text_feature.py` & `ludwig-0.9.3/ludwig/features/text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/timeseries_feature.py` & `ludwig-0.9.3/ludwig/features/timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/features/vector_feature.py` & `ludwig-0.9.3/ludwig/features/vector_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/forecast.py` & `ludwig-0.9.3/ludwig/forecast.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/globals.py` & `ludwig-0.9.3/ludwig/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-LUDWIG_VERSION = "0.9.2"
+LUDWIG_VERSION = "0.9.3"
 
 MODEL_WEIGHTS_FILE_NAME = "model_weights"
 MODEL_HYPERPARAMETERS_FILE_NAME = "model_hyperparameters.json"
 TRAIN_SET_METADATA_FILE_NAME = "training_set_metadata.json"
 TRAINING_PROGRESS_TRACKER_FILE_NAME = "training_progress.json"
 TRAINING_CHECKPOINTS_DIR_PATH = "training_checkpoints"
```

### Comparing `ludwig-0.9.2/ludwig/hyperopt/execution.py` & `ludwig-0.9.3/ludwig/hyperopt/execution.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/hyperopt/run.py` & `ludwig-0.9.3/ludwig/hyperopt/run.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/hyperopt/syncer.py` & `ludwig-0.9.3/ludwig/hyperopt/syncer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/hyperopt/utils.py` & `ludwig-0.9.3/ludwig/hyperopt/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/hyperopt_cli.py` & `ludwig-0.9.3/ludwig/hyperopt_cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/base.py` & `ludwig-0.9.3/ludwig/models/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/calibrator.py` & `ludwig-0.9.3/ludwig/models/calibrator.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/ecd.py` & `ludwig-0.9.3/ludwig/models/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/embedder.py` & `ludwig-0.9.3/ludwig/models/embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Optional
 
 import numpy as np
 import pandas as pd
 import torch
 
 from ludwig.api_annotations import DeveloperAPI
 from ludwig.constants import ENCODER_OUTPUT, MODEL_ECD, NAME, PROC_COLUMN, TYPE
@@ -69,15 +69,15 @@
     class _EmbedBatchSizeEvaluator(BatchSizeEvaluator):
         def __init__(self):
             embedder = Embedder(features_to_encode, metadata)
             self.device = get_torch_device()
             self.embedder = embedder.to(self.device)
             self.embedder.eval()
 
-        def step(self, batch_size: int):
+        def step(self, batch_size: int, global_max_sequence_length: Optional[int] = None):
             inputs = {
                 input_feature_name: input_feature.create_sample_input(batch_size=batch_size).to(self.device)
                 for input_feature_name, input_feature in self.embedder.input_features.items()
             }
             with torch.no_grad():
                 self.embedder(inputs)
```

### Comparing `ludwig-0.9.2/ludwig/models/gbm.py` & `ludwig-0.9.3/ludwig/models/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/inference.py` & `ludwig-0.9.3/ludwig/models/inference.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/llm.py` & `ludwig-0.9.3/ludwig/models/llm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/predictor.py` & `ludwig-0.9.3/ludwig/models/predictor.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/registry.py` & `ludwig-0.9.3/ludwig/models/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/models/retrieval.py` & `ludwig-0.9.3/ludwig/models/retrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     model: "SentenceTransformer", samples: List[str]
 ) -> Type[BatchSizeEvaluator]:
     class _RetrievalModelEvaluator(BatchSizeEvaluator):
         def __init__(self):
             self.model = model.to(get_torch_device())
             self.samples = samples
 
-        def step(self, batch_size: int):
+        def step(self, batch_size: int, global_max_sequence_length: Optional[int] = None):
             self.model.encode(self.samples[:batch_size], batch_size=batch_size, show_progress_bar=False)
 
     return _RetrievalModelEvaluator
 
 
 def create_semantic_retrieval_model_fn(
     model: "SentenceTransformer", batch_size: int
```

### Comparing `ludwig-0.9.2/ludwig/modules/attention_modules.py` & `ludwig-0.9.3/ludwig/modules/attention_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/convolutional_modules.py` & `ludwig-0.9.3/ludwig/modules/convolutional_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/embedding_modules.py` & `ludwig-0.9.3/ludwig/modules/embedding_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/fully_connected_modules.py` & `ludwig-0.9.3/ludwig/modules/fully_connected_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/initializer_modules.py` & `ludwig-0.9.3/ludwig/modules/initializer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/loss_implementations/corn.py` & `ludwig-0.9.3/ludwig/modules/loss_implementations/corn.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/loss_modules.py` & `ludwig-0.9.3/ludwig/modules/loss_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/lr_scheduler.py` & `ludwig-0.9.3/ludwig/modules/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/metric_modules.py` & `ludwig-0.9.3/ludwig/modules/metric_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/metric_registry.py` & `ludwig-0.9.3/ludwig/modules/metric_registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/mlp_mixer_modules.py` & `ludwig-0.9.3/ludwig/modules/mlp_mixer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/normalization_modules.py` & `ludwig-0.9.3/ludwig/modules/normalization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/optimization_modules.py` & `ludwig-0.9.3/ludwig/modules/optimization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/recurrent_modules.py` & `ludwig-0.9.3/ludwig/modules/recurrent_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/reduction_modules.py` & `ludwig-0.9.3/ludwig/modules/reduction_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/tabnet_modules.py` & `ludwig-0.9.3/ludwig/modules/tabnet_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/modules/training_hooks.py` & `ludwig-0.9.3/ludwig/modules/training_hooks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/predict.py` & `ludwig-0.9.3/ludwig/predict.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/preprocess.py` & `ludwig-0.9.3/ludwig/preprocess.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/progress_bar.py` & `ludwig-0.9.3/ludwig/progress_bar.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/common_transformer_options.py` & `ludwig-0.9.3/ludwig/schema/combiners/common_transformer_options.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/comparator.py` & `ludwig-0.9.3/ludwig/schema/combiners/comparator.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/concat.py` & `ludwig-0.9.3/ludwig/schema/combiners/concat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/project_aggregate.py` & `ludwig-0.9.3/ludwig/schema/combiners/project_aggregate.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/sequence.py` & `ludwig-0.9.3/ludwig/schema/combiners/sequence.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/sequence_concat.py` & `ludwig-0.9.3/ludwig/schema/combiners/sequence_concat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/tab_transformer.py` & `ludwig-0.9.3/ludwig/schema/combiners/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/tabnet.py` & `ludwig-0.9.3/ludwig/schema/combiners/tabnet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/transformer.py` & `ludwig-0.9.3/ludwig/schema/combiners/transformer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/combiners/utils.py` & `ludwig-0.9.3/ludwig/schema/combiners/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/common_fields.py` & `ludwig-0.9.3/ludwig/schema/common_fields.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/decoders/base.py` & `ludwig-0.9.3/ludwig/schema/decoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/decoders/llm_decoders.py` & `ludwig-0.9.3/ludwig/schema/decoders/llm_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/decoders/sequence_decoders.py` & `ludwig-0.9.3/ludwig/schema/decoders/sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/decoders/utils.py` & `ludwig-0.9.3/ludwig/schema/decoders/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/defaults/ecd.py` & `ludwig-0.9.3/ludwig/schema/defaults/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/defaults/gbm.py` & `ludwig-0.9.3/ludwig/schema/defaults/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/defaults/llm.py` & `ludwig-0.9.3/ludwig/schema/defaults/llm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/defaults/utils.py` & `ludwig-0.9.3/ludwig/schema/defaults/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/bag_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/base.py` & `ludwig-0.9.3/ludwig/schema/encoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/category_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/date_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/h3_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/image/base.py` & `ludwig-0.9.3/ludwig/schema/encoders/image/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/image/torchvision.py` & `ludwig-0.9.3/ludwig/schema/encoders/image/torchvision.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/sequence_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/set_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/text/hf_model_params.py` & `ludwig-0.9.3/ludwig/schema/encoders/text/hf_model_params.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/text_encoders.py` & `ludwig-0.9.3/ludwig/schema/encoders/text_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/encoders/utils.py` & `ludwig-0.9.3/ludwig/schema/encoders/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/__init__.py` & `ludwig-0.9.3/ludwig/schema/features/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/audio_feature.py` & `ludwig-0.9.3/ludwig/schema/features/audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/augmentation/image.py` & `ludwig-0.9.3/ludwig/schema/features/augmentation/image.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/augmentation/utils.py` & `ludwig-0.9.3/ludwig/schema/features/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/bag_feature.py` & `ludwig-0.9.3/ludwig/schema/features/bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/base.py` & `ludwig-0.9.3/ludwig/schema/features/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/binary_feature.py` & `ludwig-0.9.3/ludwig/schema/features/binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/category_feature.py` & `ludwig-0.9.3/ludwig/schema/features/category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/date_feature.py` & `ludwig-0.9.3/ludwig/schema/features/date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/h3_feature.py` & `ludwig-0.9.3/ludwig/schema/features/h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/image_feature.py` & `ludwig-0.9.3/ludwig/schema/features/image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/loss/loss.py` & `ludwig-0.9.3/ludwig/schema/features/loss/loss.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/loss/utils.py` & `ludwig-0.9.3/ludwig/schema/features/loss/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/number_feature.py` & `ludwig-0.9.3/ludwig/schema/features/number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/audio.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/audio.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/bag.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/bag.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/base.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/binary.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/binary.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/category.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/category.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/date.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/date.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/h3.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/h3.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/image.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/number.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/number.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/sequence.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/set.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/set.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/text.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/timeseries.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/timeseries.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/utils.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/preprocessing/vector.py` & `ludwig-0.9.3/ludwig/schema/features/preprocessing/vector.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/sequence_feature.py` & `ludwig-0.9.3/ludwig/schema/features/sequence_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/set_feature.py` & `ludwig-0.9.3/ludwig/schema/features/set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/text_feature.py` & `ludwig-0.9.3/ludwig/schema/features/text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/timeseries_feature.py` & `ludwig-0.9.3/ludwig/schema/features/timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/utils.py` & `ludwig-0.9.3/ludwig/schema/features/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/features/vector_feature.py` & `ludwig-0.9.3/ludwig/schema/features/vector_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/__init__.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/executor.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/executor.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/parameter.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/parameter.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/scheduler.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/search_algorithm.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/hyperopt/utils.py` & `ludwig-0.9.3/ludwig/schema/hyperopt/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/llms/base_model.py` & `ludwig-0.9.3/ludwig/schema/llms/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from transformers import AutoConfig
 
 from ludwig.api_annotations import DeveloperAPI
 from ludwig.constants import BASE_MODEL
 from ludwig.error import ConfigValidationError
 from ludwig.schema.metadata import LLM_METADATA
 from ludwig.schema.metadata.parameter_metadata import convert_metadata_to_json
-from ludwig.utils.llm_utils import _PHI_BASE_MODEL_MAPPING
 
 logger = logging.getLogger(__name__)
 
 # Maps a preset LLM name to the full slash-delimited HF path. If the user chooses a preset LLM, the preset LLM name is
 # replaced with the full slash-delimited HF path using this map, after JSON validation but before config object
 # initialization.
 MODEL_PRESETS = {
@@ -75,21 +74,14 @@
         given name (which should be a full path) exists locally or in the transformers library.
         """
         if isinstance(model_name, str):
             if model_name in MODEL_PRESETS:
                 return MODEL_PRESETS[model_name]
             if os.path.isdir(model_name):
                 return model_name
-            if model_name in _PHI_BASE_MODEL_MAPPING:
-                logger.warning(
-                    f"{model_name} does not work correctly out of the box since it requires running remote code. "
-                    f"Replacing {model_name} with {_PHI_BASE_MODEL_MAPPING[model_name]} as the base LLM model since "
-                    "this is the official version of the model supported by HuggingFace."
-                )
-                return _PHI_BASE_MODEL_MAPPING[model_name]
             try:
                 AutoConfig.from_pretrained(model_name)
                 return model_name
             except OSError:
                 raise ConfigValidationError(
                     f"Specified base model `{model_name}` could not be loaded. If this is a private repository, make "
                     f"sure to set HUGGING_FACE_HUB_TOKEN in your environment. Check that {model_name} is a valid "
```

### Comparing `ludwig-0.9.2/ludwig/schema/llms/generation.py` & `ludwig-0.9.3/ludwig/schema/llms/generation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/llms/model_parameters.py` & `ludwig-0.9.3/ludwig/schema/llms/model_parameters.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/llms/peft.py` & `ludwig-0.9.3/ludwig/schema/llms/peft.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/llms/prompt.py` & `ludwig-0.9.3/ludwig/schema/llms/prompt.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/llms/quantization.py` & `ludwig-0.9.3/ludwig/schema/llms/quantization.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/lr_scheduler.py` & `ludwig-0.9.3/ludwig/schema/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/__init__.py` & `ludwig-0.9.3/ludwig/schema/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/combiners.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/combiners.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/common.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/common.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/decoders.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/decoders.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/encoders.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/encoders.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/features.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/features.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/llm.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/llm.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/loss.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/loss.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/optimizers.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/optimizers.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/preprocessing.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/preprocessing.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/configs/trainer.yaml` & `ludwig-0.9.3/ludwig/schema/metadata/configs/trainer.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/metadata/parameter_metadata.py` & `ludwig-0.9.3/ludwig/schema/metadata/parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/model_types/base.py` & `ludwig-0.9.3/ludwig/schema/model_types/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/model_types/ecd.py` & `ludwig-0.9.3/ludwig/schema/model_types/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/model_types/gbm.py` & `ludwig-0.9.3/ludwig/schema/model_types/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/model_types/llm.py` & `ludwig-0.9.3/ludwig/schema/model_types/llm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/model_types/utils.py` & `ludwig-0.9.3/ludwig/schema/model_types/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/optimizers.py` & `ludwig-0.9.3/ludwig/schema/optimizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/preprocessing.py` & `ludwig-0.9.3/ludwig/schema/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/profiler.py` & `ludwig-0.9.3/ludwig/schema/profiler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/split.py` & `ludwig-0.9.3/ludwig/schema/split.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/trainer.py` & `ludwig-0.9.3/ludwig/schema/trainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/schema/utils.py` & `ludwig-0.9.3/ludwig/schema/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/serve.py` & `ludwig-0.9.3/ludwig/serve.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/train.py` & `ludwig-0.9.3/ludwig/train.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/trainers/base.py` & `ludwig-0.9.3/ludwig/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/trainers/registry.py` & `ludwig-0.9.3/ludwig/trainers/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/trainers/trainer.py` & `ludwig-0.9.3/ludwig/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,14 +548,15 @@
         training_set: Dataset,
         random_seed: int = default_random_seed,
         max_trials: int = 20,
         halving_limit: int = 3,
         snapshot_weights: bool = True,
         on_best_batch_size_updated: Optional[Callable[[int, float, int], None]] = None,
         tune_for_training: bool = True,
+        global_max_sequence_length: Optional[int] = None,
     ) -> int:
         logger.info("Tuning batch size...")
         skip_save_model = self.skip_save_model
         skip_save_progress = self.skip_save_progress
         skip_save_log = self.skip_save_log
         # Set temporary values
         self.skip_save_model = True
@@ -588,15 +589,15 @@
                 # pretrained models.
                 checkpoint = self.distributed.create_checkpoint_handle(
                     dist_model=self.dist_model, model=self.model, optimizer=self.optimizer, scheduler=self.scheduler
                 )
                 checkpoint.save(os.path.join(tmpdir, "latest.ckpt"), global_step=0)
             try:
                 best_batch_size = evaluator.select_best_batch_size(
-                    len(training_set), max_batch_size, max_trials, self.is_coordinator()
+                    len(training_set), max_batch_size, max_trials, self.is_coordinator(), global_max_sequence_length
                 )
                 best_batch_size = self.distributed.broadcast_object(best_batch_size)
 
                 if tune_for_training:
                     # Update batch size / gradient accumulation before preparing the trainer. This is needed primarily
                     # for DeepSpeed, which needs to know the batch size and gradient accumulation steps before init
                     self.config.batch_size = best_batch_size
@@ -622,15 +623,15 @@
         trainer = self
 
         class _TrainerBatchSizeEvaluator(BatchSizeEvaluator):
             def reset(self):
                 trainer.model.reset_metrics()
                 trainer.optimizer.zero_grad()
 
-            def step(self, batch_size: int):
+            def step(self, batch_size: int, global_max_sequence_length: Optional[int] = None):
                 trainer.distributed.set_batch_size(trainer.dist_model, batch_size)
                 inputs = {
                     input_feature_name: input_feature.create_sample_input(batch_size=batch_size).to(trainer.device)
                     for input_feature_name, input_feature in trainer.model.input_features.items()
                 }
                 targets = {
                     output_feature_name: output_feature.create_sample_output(batch_size=batch_size).to(trainer.device)
@@ -644,15 +645,15 @@
         trainer = self
 
         class _PredictBatchSizeEvaluator(BatchSizeEvaluator):
             def reset(self):
                 trainer.model.reset_metrics()
                 trainer.optimizer.zero_grad()
 
-            def step(self, batch_size: int):
+            def step(self, batch_size: int, global_max_sequence_length: Optional[int] = None):
                 trainer.distributed.set_batch_size(trainer.dist_model, batch_size)
                 inputs = {
                     input_feature_name: input_feature.create_sample_input(batch_size=batch_size).to(trainer.device)
                     for input_feature_name, input_feature in trainer.model.input_features.items()
                 }
                 targets = {
                     output_feature_name: output_feature.create_sample_output(batch_size=batch_size).to(trainer.device)
```

### Comparing `ludwig-0.9.2/ludwig/trainers/trainer_lightgbm.py` & `ludwig-0.9.3/ludwig/trainers/trainer_lightgbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/trainers/trainer_llm.py` & `ludwig-0.9.3/ludwig/trainers/trainer_llm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import os
 import time
 from typing import Callable, Dict, List, Optional, Union
 
+import torch
 from torch.utils.tensorboard import SummaryWriter
 
 from ludwig.constants import MINIMUM_BATCH_SIZE, TEST, TRAINING, VALIDATION
 from ludwig.data.dataset.base import Dataset
 from ludwig.distributed.base import DistributedStrategy, LocalStrategy
 from ludwig.features.feature_utils import LudwigFeatureDict
 from ludwig.models.llm import LLM
@@ -14,14 +15,15 @@
 from ludwig.modules.metric_modules import get_initial_validation_value
 from ludwig.schema.trainer import BaseTrainerConfig, FineTuneTrainerConfig, NoneTrainerConfig
 from ludwig.trainers.base import BaseTrainer
 from ludwig.trainers.registry import register_llm_ray_trainer, register_llm_trainer
 from ludwig.trainers.trainer import Trainer
 from ludwig.types import ModelConfigDict
 from ludwig.utils import time_utils
+from ludwig.utils.batch_size_tuner import BatchSizeEvaluator
 from ludwig.utils.defaults import default_random_seed
 from ludwig.utils.metric_utils import TrainerMetric
 from ludwig.utils.metrics_printed_table import print_metrics_table
 from ludwig.utils.misc_utils import set_random_seed
 from ludwig.utils.torch_utils import get_torch_device
 from ludwig.utils.trainer_utils import append_metrics, get_new_progress_tracker, ProgressTracker
 
@@ -467,14 +469,90 @@
             logger.info(f"Input: {llm_eval_examples['inputs'][i].strip()}")
             logger.info(f"Output: {llm_eval_examples['outputs'][i].strip()}")
             logger.info("--------------------")
 
         progress_tracker.llm_eval_examples = llm_eval_examples
         return append_metrics(self.model, dataset_name, metrics, metrics_log, progress_tracker)
 
+    def tune_batch_size(
+        self,
+        config: ModelConfigDict,
+        training_set: Dataset,
+        random_seed: int = default_random_seed,
+        max_trials: int = 20,
+        halving_limit: int = 3,
+        snapshot_weights: bool = True,
+        on_best_batch_size_updated: Optional[Callable[[int, float, int], None]] = None,
+        tune_for_training: bool = True,
+        global_max_sequence_length: Optional[int] = None,
+    ) -> int:
+        if global_max_sequence_length is None:
+            global_max_sequence_length = self.model.global_max_sequence_length
+        return super().tune_batch_size(
+            config,
+            training_set,
+            random_seed,
+            max_trials,
+            halving_limit,
+            snapshot_weights,
+            on_best_batch_size_updated,
+            tune_for_training,
+            global_max_sequence_length,
+        )
+
+    def _create_batch_size_evaluator(self) -> BatchSizeEvaluator:
+        trainer = self
+
+        class _TrainerBatchSizeEvaluator(BatchSizeEvaluator):
+            def __init__(self):
+                self.input_feature_name, self.input_feature = trainer.model.input_features.items()[0]
+                self.output_feature_name, self.output_feature = trainer.model.output_features.items()[0]
+
+                # Get the length of the longest input sequence from the training data
+                self.input_msl = self.input_feature.input_shape[0]
+                # Get the length of the longest output sequence from the training data
+                self.output_msl = self.output_feature.output_shape[0]
+                # max_sequence_length here is the smaller value between the global max sequence length of the model
+                # and the model's context length
+                if trainer.model.config_obj.output_features[0].preprocessing.max_sequence_length:
+                    self.output_msl = trainer.model.config_obj.output_features[0].preprocessing.max_sequence_length
+
+                # This is useful to create the synthetic input and target data which will be a
+                # random sequence of integers between 0 and vocab_size
+                self.vocab_size = len(trainer.model.config_obj.input_features[0].encoder.vocab)
+
+            def reset(self):
+                trainer.model.reset_metrics()
+                trainer.optimizer.zero_grad()
+
+            def step(self, batch_size: int, global_max_sequence_length: int):
+                trainer.distributed.set_batch_size(trainer.dist_model, batch_size)
+
+                input_msl = self.input_msl
+                output_msl = self.output_msl
+                if self.input_msl + self.output_msl > global_max_sequence_length:
+                    # In this case, we just need to make sure that the length of the synthetic data exceeds
+                    # max_sequence_length by at most a small amount
+                    input_msl = global_max_sequence_length // 2 + 1
+                    output_msl = global_max_sequence_length // 2 + 1
+
+                inputs = {
+                    self.input_feature_name: torch.randint(0, self.vocab_size, size=(batch_size, input_msl))
+                    .to(self.input_feature.input_dtype)
+                    .to(trainer.device)
+                }
+                targets = {
+                    self.output_feature_name: torch.randint(0, self.vocab_size, size=(batch_size, output_msl))
+                    .to(self.output_feature.get_output_dtype())
+                    .to(trainer.device)
+                }
+                trainer.train_step(inputs, targets)
+
+        return _TrainerBatchSizeEvaluator()
+
 
 class RemoteLLMTrainer(NoneTrainer):
     def __init__(self, gpus=None, gpu_memory_limit=None, allow_parallel_threads=True, **kwargs):
         super().__init__(**kwargs)
 
         # Only return results from rank 0 to reduce network overhead
         self.train = self.distributed.return_first(self.train)
```

### Comparing `ludwig-0.9.2/ludwig/types.py` & `ludwig-0.9.3/ludwig/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/upload.py` & `ludwig-0.9.3/ludwig/upload.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/algorithms_utils.py` & `ludwig-0.9.3/ludwig/utils/algorithms_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/audio_utils.py` & `ludwig-0.9.3/ludwig/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/augmentation_utils.py` & `ludwig-0.9.3/ludwig/utils/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/automl/data_source.py` & `ludwig-0.9.3/ludwig/utils/automl/data_source.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/automl/field_info.py` & `ludwig-0.9.3/ludwig/utils/automl/field_info.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/automl/type_inference.py` & `ludwig-0.9.3/ludwig/utils/automl/type_inference.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/automl/utils.py` & `ludwig-0.9.3/ludwig/utils/automl/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/backward_compatibility.py` & `ludwig-0.9.3/ludwig/utils/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/batch_size_tuner.py` & `ludwig-0.9.3/ludwig/utils/batch_size_tuner.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 import torch
 
 from ludwig.api_annotations import DeveloperAPI
 from ludwig.constants import MAX_BATCH_SIZE_DATASET_FRACTION, MIN_POSSIBLE_BATCH_SIZE
 
 logger = logging.getLogger(__name__)
 
+TOTAL_STEPS = 5
+
 
 @DeveloperAPI
 class BatchSizeEvaluator(ABC):
     def select_best_batch_size(
         self,
         dataset_len: int,
         max_batch_size: Optional[int] = None,
         max_trials: int = 20,
         is_coordinator: Optional[bool] = True,
+        global_max_sequence_length: Optional[int] = None,
     ) -> int:
         """Returns optimal batch size as measured by throughput (samples / sec)."""
         logger.info("Tuning batch size...")
 
         max_batch_size = max_batch_size or dataset_len
 
         def _is_valid_batch_size(batch_size):
@@ -47,15 +50,17 @@
         count = 0
         while count < max_trials and _is_valid_batch_size(batch_size):
             if is_coordinator:
                 logger.info(f"Exploring batch_size={batch_size}")
             gc.collect()
 
             try:
-                samples_per_sec = self.evaluate(batch_size, total_steps=5)
+                samples_per_sec = self.evaluate(
+                    batch_size, total_steps=TOTAL_STEPS, global_max_sequence_length=global_max_sequence_length
+                )
                 if is_coordinator:
                     logger.info(f"Throughput at batch_size={batch_size}: {samples_per_sec:.5f} samples/s")
                 if samples_per_sec < best_samples_per_sec:
                     # We assume that once the throughput starts degrading, it won't go up again
                     if is_coordinator:
                         logger.info(f"Throughput decrease at batch_size={batch_size}")
                     break
@@ -84,33 +89,35 @@
                 logger.info(f"Could not tune batch size, using minimum batch size of {MIN_POSSIBLE_BATCH_SIZE}")
             best_batch_size = MIN_POSSIBLE_BATCH_SIZE
 
         if is_coordinator:
             logger.info(f"Selected batch_size={best_batch_size}")
         return best_batch_size
 
-    def evaluate(self, batch_size: int, total_steps: int = 5) -> float:
+    def evaluate(
+        self, batch_size: int, total_steps: int = 5, global_max_sequence_length: Optional[int] = None
+    ) -> float:
         """Evaluates throughput of the given batch size.
 
         Return:
             Median throughput in samples / sec.
         """
         durations = []
         for _ in range(total_steps):
             self.reset()
             start_ts = time.time()
-            self.step(batch_size)
+            self.step(batch_size, global_max_sequence_length=global_max_sequence_length)
             durations.append(time.time() - start_ts)
 
         med_duration_s = statistics.median(durations)
         if med_duration_s == 0.0:
             return float("inf")
 
         return batch_size / med_duration_s
 
     def reset(self):
         """Called at the beginning of each evaluation step."""
         pass
 
-    def step(self, batch_size: int):
+    def step(self, batch_size: int, global_max_sequence_length: Optional[int] = None):
         """Called each step to evaluate the given batch size."""
         raise NotImplementedError("`step` must be implemented by concrete evaluator.")
```

### Comparing `ludwig-0.9.2/ludwig/utils/calibration.py` & `ludwig-0.9.3/ludwig/utils/calibration.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/carton_utils.py` & `ludwig-0.9.3/ludwig/utils/carton_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/checkpoint_utils.py` & `ludwig-0.9.3/ludwig/utils/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/config_utils.py` & `ludwig-0.9.3/ludwig/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/data_utils.py` & `ludwig-0.9.3/ludwig/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/dataframe_utils.py` & `ludwig-0.9.3/ludwig/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/dataset_utils.py` & `ludwig-0.9.3/ludwig/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/date_utils.py` & `ludwig-0.9.3/ludwig/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/defaults.py` & `ludwig-0.9.3/ludwig/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/entmax/__init__.py` & `ludwig-0.9.3/ludwig/utils/entmax/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/entmax/activations.py` & `ludwig-0.9.3/ludwig/utils/entmax/activations.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/entmax/losses.py` & `ludwig-0.9.3/ludwig/utils/entmax/losses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/entmax/root_finding.py` & `ludwig-0.9.3/ludwig/utils/entmax/root_finding.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/eval_utils.py` & `ludwig-0.9.3/ludwig/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/fs_utils.py` & `ludwig-0.9.3/ludwig/utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/gbm_utils.py` & `ludwig-0.9.3/ludwig/utils/gbm_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/h3_util.py` & `ludwig-0.9.3/ludwig/utils/h3_util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/heuristics.py` & `ludwig-0.9.3/ludwig/utils/heuristics.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/hf_utils.py` & `ludwig-0.9.3/ludwig/utils/hf_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/horovod_utils.py` & `ludwig-0.9.3/ludwig/utils/horovod_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/html_utils.py` & `ludwig-0.9.3/ludwig/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/image_utils.py` & `ludwig-0.9.3/ludwig/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/inference_utils.py` & `ludwig-0.9.3/ludwig/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/llm_quantization_utils.py` & `ludwig-0.9.3/ludwig/utils/llm_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/llm_utils.py` & `ludwig-0.9.3/ludwig/utils/llm_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 logger = logging.getLogger(__name__)
 
 
 FALLBACK_CONTEXT_LEN = 2048
 
 transformers_436 = version.parse(transformers.__version__) >= version.parse("4.36.0")
 
-# The official microsoft phi models don't work out of the box because the weights aren't compatiable with HF
-# See https://github.com/huggingface/transformers/issues/28049 for more context.
-_PHI_BASE_MODEL_MAPPING = {
-    "microsoft/phi-1": "susnato/phi-1_dev",
-    "microsoft/phi-1.5": "susnato/phi-1_5_dev",
-    "microsoft/phi-2": "susnato/phi-2",
+# Phi models don't support "device_map='auto'" at model load time as of transformers 4.37.0.
+_MODELS_WITH_DEVICE_MAP_AUTO_EXCLUSION = {
+    "susnato/phi-1_dev",
+    "susnato/phi-1_5_dev",
+    "susnato/phi-2",
+    "microsoft/phi-1",
+    "microsoft/phi-1_5",
+    "microsoft/phi-2",
 }
 
-# The susnato Phi models as of Transformers 4.36.1 don't support "device_map='auto'" at model load time.
-_MODELS_WITH_DEVICE_MAP_AUTO_EXCLUSION = {"susnato/phi-1_dev", "susnato/phi-1_5_dev", "susnato/phi-2"}
-
 
 @default_retry(tries=8)
 def load_pretrained_from_config(
     config_obj: Union["LLMModelConfig", "LLMEncoderConfig"],
     model_config: Optional[AutoConfig] = None,
     weights_save_path: Optional[str] = None,
 ) -> PreTrainedModel:
```

### Comparing `ludwig-0.9.2/ludwig/utils/loss_utils.py` & `ludwig-0.9.3/ludwig/utils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/math_utils.py` & `ludwig-0.9.3/ludwig/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/metric_utils.py` & `ludwig-0.9.3/ludwig/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/metrics_printed_table.py` & `ludwig-0.9.3/ludwig/utils/metrics_printed_table.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/misc_utils.py` & `ludwig-0.9.3/ludwig/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/model_utils.py` & `ludwig-0.9.3/ludwig/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/neuropod_utils.py` & `ludwig-0.9.3/ludwig/utils/neuropod_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/nlp_utils.py` & `ludwig-0.9.3/ludwig/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/numerical_test_utils.py` & `ludwig-0.9.3/ludwig/utils/numerical_test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/output_feature_utils.py` & `ludwig-0.9.3/ludwig/utils/output_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/package_utils.py` & `ludwig-0.9.3/ludwig/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/print_utils.py` & `ludwig-0.9.3/ludwig/utils/print_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/registry.py` & `ludwig-0.9.3/ludwig/utils/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/server_utils.py` & `ludwig-0.9.3/ludwig/utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/state_dict_backward_compatibility.py` & `ludwig-0.9.3/ludwig/utils/state_dict_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/strings_utils.py` & `ludwig-0.9.3/ludwig/utils/strings_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/structural_warning.py` & `ludwig-0.9.3/ludwig/utils/structural_warning.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/system_utils.py` & `ludwig-0.9.3/ludwig/utils/system_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/time_utils.py` & `ludwig-0.9.3/ludwig/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/tokenizers.py` & `ludwig-0.9.3/ludwig/utils/tokenizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -839,38 +839,59 @@
     def get_pad_token(self) -> str:
         return self.tokenizer.pad_token
 
     def get_unk_token(self) -> str:
         return self.tokenizer.unk_token
 
     def _set_pad_token(self) -> None:
-        """Sets the pad token and pad token ID for the tokenizer.
+        """Sets the pad token and pad token ID for the tokenizer."""
 
-        If there is no pad token, then set one by default.
-        If there is no pad token index, then set it to 0.
+        # CodeGenTokenizer Used by Phi-2
+        # GPTNeoXTokenizerFast Used by Pythia
+        from transformers import (
+            CodeGenTokenizer,
+            CodeGenTokenizerFast,
+            CodeLlamaTokenizer,
+            CodeLlamaTokenizerFast,
+            GPT2Tokenizer,
+            GPT2TokenizerFast,
+            GPTNeoXTokenizerFast,
+            LlamaTokenizer,
+            LlamaTokenizerFast,
+        )
+
+        # Tokenizers might have the pad token id attribute since they tend to use the same base class, but
+        # it can be set to None so we check for this explicitly.
+        if hasattr(self.tokenizer, "pad_token_id") and self.tokenizer.pad_token_id is not None:
+            return
+
+        # HACK(geoffrey): gpt2 has no pad token. Recommendation is to use eos token instead.
+        # https://github.com/huggingface/transformers/issues/2630#issuecomment-1290809338
+        # https://github.com/huggingface/transformers/issues/2648#issuecomment-616177044
+        if any(
+            isinstance(self.tokenizer, t)
+            for t in [
+                CodeGenTokenizer,
+                CodeGenTokenizerFast,
+                CodeLlamaTokenizer,
+                CodeLlamaTokenizerFast,
+                GPT2Tokenizer,
+                GPT2TokenizerFast,
+                GPTNeoXTokenizerFast,
+                LlamaTokenizer,
+                LlamaTokenizerFast,
+            ]
+        ):
+            if hasattr(self.tokenizer, "eos_token") and self.tokenizer.eos_token is not None:
+                logger.warning("No padding token id found. Using eos_token as pad_token.")
+                self.tokenizer.pad_token = self.tokenizer.eos_token
+                self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
 
-        Notes:
-        - (geoffrey): gpt2 has no pad token. Recommendation is to use eos token instead.
-            - https://github.com/huggingface/transformers/issues/2630#issuecomment-1290809338
-            - https://github.com/huggingface/transformers/issues/2648#issuecomment-616177044
-        - (Justin): Using the EOS token in place of the pad token causes an issue with HF model.generate() when
-            there are multiple examples in the batch.
-            - https://github.com/facebookresearch/llama/issues/380#issuecomment-1716832417
-            - Recommendation is to set a separate '[PAD]' or '<pad>' token.
-        """
-        if self.tokenizer.pad_token is None:
-            logger.warning("No padding token found. Using '[PAD]' as the pad token.")
-            self.tokenizer.pad_token = "[PAD]"
-
-        # NOTE(geoffrey): you can check this condition separately because these are actually @property methods,
-        # which means one's logic is tightly coupled with the other. If one changes, the other will change as well.
-        # On a related note, that means that this below condition should never be called, but leaving it here in case
-        # it was put here for a reason.
-        # https://github.com/huggingface/transformers/blob/4ab5fb8941a38d172b3883c152c34ae2a0b83a68/src/transformers/tokenization_utils_base.py#L1204-L1210
-        # https://github.com/huggingface/transformers/blob/4ab5fb8941a38d172b3883c152c34ae2a0b83a68/src/transformers/tokenization_utils_base.py#L1266-L1267
+        # Incase any HF tokenizer does not have pad token ID, just default to using 0
+        # as the pad_token_id.
         if self.tokenizer.pad_token_id is None:
             logger.warning("No padding token id found. Using 0 as pad token id.")
             self.tokenizer.pad_token_id = 0
 
     def convert_token_to_id(self, token: str) -> int:
         return self.tokenizer.convert_tokens_to_ids(token)
```

### Comparing `ludwig-0.9.2/ludwig/utils/torch_utils.py` & `ludwig-0.9.3/ludwig/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/trainer_utils.py` & `ludwig-0.9.3/ludwig/utils/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/triton_utils.py` & `ludwig-0.9.3/ludwig/utils/triton_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/types.py` & `ludwig-0.9.3/ludwig/utils/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/upload_utils.py` & `ludwig-0.9.3/ludwig/utils/upload_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/version_transformation.py` & `ludwig-0.9.3/ludwig/utils/version_transformation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/utils/visualization_utils.py` & `ludwig-0.9.3/ludwig/utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/vector_index/__init__.py` & `ludwig-0.9.3/ludwig/vector_index/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/vector_index/faiss.py` & `ludwig-0.9.3/ludwig/vector_index/faiss.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig/visualize.py` & `ludwig-0.9.3/ludwig/visualize.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig.egg-info/PKG-INFO` & `ludwig-0.9.3/ludwig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ludwig
-Version: 0.9.2
+Version: 0.9.3
 Summary: Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.
 Home-page: https://github.com/ludwig-ai/ludwig
 Author: Piero Molino
 Author-email: piero.molino@gmail.com
 License: Apache 2.0
 Download-URL: https://pypi.org/project/ludwig/
 Description: <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ludwig Version: 0.9.2 Summary: Declarative machine
+Metadata-Version: 2.1 Name: ludwig Version: 0.9.3 Summary: Declarative machine
 learning: End-to-end machine learning pipelines using data-driven
 configurations. Home-page: https://github.com/ludwig-ai/ludwig Author: Piero
 Molino Author-email: piero.molino@gmail.com License: Apache 2.0 Download-URL:
 https://pypi.org/project/ludwig/ Description:
        _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_u_d_w_i_g_-_a_i_/_l_u_d_w_i_g_-_d_o_c_s_/_r_a_w_/_m_a_s_t_e_r_/_d_o_c_s_/_i_m_a_g_e_s_/
                            _l_u_d_w_i_g___h_e_r_o___s_m_a_l_l_e_r_._j_p_g_]
  _Declarative deep learning framework built for scale and efficiency._ [![PyPI
```

### Comparing `ludwig-0.9.2/ludwig.egg-info/SOURCES.txt` & `ludwig-0.9.3/ludwig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/ludwig.egg-info/requires.txt` & `ludwig-0.9.3/ludwig.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Cython>=0.25
 h5py!=3.0.0,>=2.6
 numpy>=1.15
-pandas!=1.1.5,>=1.0
+pandas!=1.1.5,<2.2.0,>=1.0
 scipy>=0.18
 tabulate>=0.7
 scikit-learn
 tqdm
 torch>=2.0.0
 torchaudio
 torchtext
 torchvision
 pydantic<2.0
-transformers>=4.36.2
+transformers>=4.37.0
 tifffile
 imagecodecs
 tokenizers>=0.15
 spacy>=2.3
 PyYAML!=5.4.*,<6.0.1,>=3.12
 absl-py
 kaggle
@@ -60,15 +60,15 @@
 dask[dataframe]<2023.4.0
 pyarrow
 ray[data,default,serve,tune]==2.3.1
 tensorboardX<2.3
 GPUtil
 tblib
 awscli
-deepspeed!=0.11.0
+deepspeed!=0.11.0,<0.13.0
 getdaft[ray]==0.1.20
 
 [explain]
 captum
 
 [extra]
 horovod[pytorch]!=0.26.0,>=0.24.0
@@ -87,15 +87,15 @@
 dask[dataframe]<2023.4.0
 pyarrow
 ray[data,default,serve,tune]==2.3.1
 tensorboardX<2.3
 GPUtil
 tblib
 awscli
-deepspeed!=0.11.0
+deepspeed!=0.11.0,<0.13.0
 getdaft[ray]==0.1.20
 ray[default,tune]>=2.0.0
 hyperopt
 hummingbird-ml>=0.4.8
 lightgbm
 lightgbm-ray
 sentence-transformers
@@ -148,15 +148,15 @@
 dask[dataframe]<2023.4.0
 pyarrow
 ray[data,default,serve,tune]==2.3.1
 tensorboardX<2.3
 GPUtil
 tblib
 awscli
-deepspeed!=0.11.0
+deepspeed!=0.11.0,<0.13.0
 getdaft[ray]==0.1.20
 ray[default,tune]>=2.0.0
 hyperopt
 hummingbird-ml>=0.4.8
 lightgbm
 lightgbm-ray
 sentence-transformers
```

### Comparing `ludwig-0.9.2/requirements.txt` & `ludwig-0.9.3/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Cython>=0.25
 h5py>=2.6,!=3.0.0
 numpy>=1.15
-pandas>=1.0,!=1.1.5
+# GitHub Issue for Pinning Pandas < 2.2.0: https://github.com/ludwig-ai/ludwig/issues/3907
+pandas>=1.0,!=1.1.5,<2.2.0
 scipy>=0.18
 tabulate>=0.7
 scikit-learn
 tqdm
 torch>=2.0.0
 torchaudio
 torchtext
 torchvision
 pydantic<2.0
-transformers>=4.36.2
+transformers>=4.37.0
 tifffile
 imagecodecs
 tokenizers>=0.15
 spacy>=2.3
 PyYAML>=3.12,<6.0.1,!=5.4.* #Exlude PyYAML 5.4.* due to incompatibility with awscli
 absl-py
 kaggle
```

### Comparing `ludwig-0.9.2/requirements_test.txt` & `ludwig-0.9.3/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/setup.py` & `ludwig-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     extra_requirements["test"] = extra_requirements["full"] + [line.strip() for line in f if line]
 
 with open(path.join(here, "requirements_extra.txt"), encoding="utf-8") as f:
     extra_requirements["extra"] = [line.strip() for line in f if line]
 
 setup(
     name="ludwig",
-    version="0.9.2",
+    version="0.9.3",
     description="Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ludwig-ai/ludwig",
     download_url="https://pypi.org/project/ludwig/",
     author="Piero Molino",
     author_email="piero.molino@gmail.com",
```

### Comparing `ludwig-0.9.2/tests/integration_tests/parameter_update_utils.py` & `ludwig-0.9.3/tests/integration_tests/parameter_update_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/synthetic_test_data.py` & `ludwig-0.9.3/tests/integration_tests/synthetic_test_data.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_api.py` & `ludwig-0.9.3/tests/integration_tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_audio_feature.py` & `ludwig-0.9.3/tests/integration_tests/test_audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_automl.py` & `ludwig-0.9.3/tests/integration_tests/test_automl.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_cache_manager.py` & `ludwig-0.9.3/tests/integration_tests/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_cached_preprocessing.py` & `ludwig-0.9.3/tests/integration_tests/test_cached_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_carton.py` & `ludwig-0.9.3/tests/integration_tests/test_carton.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_class_imbalance_feature.py` & `ludwig-0.9.3/tests/integration_tests/test_class_imbalance_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_cli.py` & `ludwig-0.9.3/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_collect.py` & `ludwig-0.9.3/tests/integration_tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_config_global_defaults.py` & `ludwig-0.9.3/tests/integration_tests/test_config_global_defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_contrib_aim.py` & `ludwig-0.9.3/tests/integration_tests/test_contrib_aim.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_contrib_comet.py` & `ludwig-0.9.3/tests/integration_tests/test_contrib_comet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_contrib_wandb.py` & `ludwig-0.9.3/tests/integration_tests/test_contrib_wandb.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_custom_components.py` & `ludwig-0.9.3/tests/integration_tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_date_feature.py` & `ludwig-0.9.3/tests/integration_tests/test_date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_dependencies.py` & `ludwig-0.9.3/tests/integration_tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_experiment.py` & `ludwig-0.9.3/tests/integration_tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_explain.py` & `ludwig-0.9.3/tests/integration_tests/test_explain.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_gbm.py` & `ludwig-0.9.3/tests/integration_tests/test_gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_graph_execution.py` & `ludwig-0.9.3/tests/integration_tests/test_graph_execution.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_horovod.py` & `ludwig-0.9.3/tests/integration_tests/test_horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_hyperopt.py` & `ludwig-0.9.3/tests/integration_tests/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_hyperopt_ray.py` & `ludwig-0.9.3/tests/integration_tests/test_hyperopt_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_hyperopt_ray_horovod.py` & `ludwig-0.9.3/tests/integration_tests/test_hyperopt_ray_horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_input_feature_tied.py` & `ludwig-0.9.3/tests/integration_tests/test_input_feature_tied.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_kfold_cv.py` & `ludwig-0.9.3/tests/integration_tests/test_kfold_cv.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_llm.py` & `ludwig-0.9.3/tests/integration_tests/test_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pathlib
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import pytest
 import torch
+import yaml
 
 import ludwig.error as ludwig_error
 from ludwig.api import LudwigModel
 from ludwig.constants import (
     ADAPTER,
     BACKEND,
     BASE_MODEL,
@@ -1205,20 +1206,30 @@
     }
 
     return encoder_config
 
 
 @pytest.mark.parametrize(
     "adapter,quantization",
-    [(None, None), ("lora", None), ("lora", {"bits": 4}), ("lora", {"bits": 8})],
-    ids=["FFT", "LoRA", "LoRA 4-bit", "LoRA 8-bit"],
+    [
+        (None, None),
+        ("lora", None),
+        ("lora", {"bits": 4}),
+        ("lora", {"bits": 8}),
+        ("adalora", None),
+        ("adalora", {"bits": 4}),
+        ("adalora", {"bits": 8}),
+    ],
+    ids=["FFT", "LoRA", "LoRA 4-bit", "LoRA 8-bit", "AdaLoRA", "AdaLoRA 4-bit", "AdaLoRA 8-bit"],
 )
 def test_llm_encoding(llm_encoder_config, adapter, quantization, tmpdir):
     if (
-        _finetune_strategy_requires_cuda(finetune_strategy_name=adapter, quantization_args=quantization)
+        _finetune_strategy_requires_cuda(
+            finetune_strategy_name="lora" if adapter else None, quantization_args=quantization
+        )
         and not (torch.cuda.is_available() and torch.cuda.device_count()) > 0
     ):
         pytest.skip("Skip: quantization requires GPU and none are available.")
 
     dataset_path = os.path.join(tmpdir, "llm_classification_data.csv")
 
     config = {
@@ -1240,14 +1251,47 @@
 
     generate_data(input_features=config[INPUT_FEATURES], output_features=config[OUTPUT_FEATURES], filename=dataset_path)
 
     model = LudwigModel(config)
     model.train(dataset=dataset_path, output_directory=str(tmpdir))
 
 
+def test_llm_batch_size_tuning():
+    dataset = pd.DataFrame({"instruction": ["a"] * 100, "output": ["a"] * 100})
+    config = yaml.safe_load(
+        """
+    model_type: llm
+    input_features:
+        - name: instruction
+          type: text
+    output_features:
+        - name: output
+          type: text
+    prompt:
+        template: >-
+            {instruction}
+    adapter:
+        type: lora
+    trainer:
+        type: finetune
+        optimizer:
+            type: adam
+        train_steps: 1
+        learning_rate: 0.0002
+        eval_batch_size: 2
+    backend:
+        type: local
+    base_model: HuggingFaceH4/tiny-random-LlamaForCausalLM
+        """
+    )
+    model = LudwigModel(config=config)
+    model.train(dataset=dataset)
+    assert model.config_obj.trainer.batch_size > 1
+
+
 @pytest.mark.llm
 def test_llm_used_tokens(tmpdir):
     input_features = [text_feature(name="input", encoder={"type": "passthrough"})]
     output_features = [text_feature(name="output")]
 
     df = pd.read_json("https://raw.githubusercontent.com/sahil280114/codealpaca/master/data/code_alpaca_20k.json").head(
         10
```

### Comparing `ludwig-0.9.2/tests/integration_tests/test_missing_value_strategy.py` & `ludwig-0.9.3/tests/integration_tests/test_missing_value_strategy.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_mlflow.py` & `ludwig-0.9.3/tests/integration_tests/test_mlflow.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_model_save_and_load.py` & `ludwig-0.9.3/tests/integration_tests/test_model_save_and_load.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_model_training_options.py` & `ludwig-0.9.3/tests/integration_tests/test_model_training_options.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_neuropod.py` & `ludwig-0.9.3/tests/integration_tests/test_neuropod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_number_feature.py` & `ludwig-0.9.3/tests/integration_tests/test_number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_peft.py` & `ludwig-0.9.3/tests/integration_tests/test_peft.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_postprocessing.py` & `ludwig-0.9.3/tests/integration_tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_preprocessing.py` & `ludwig-0.9.3/tests/integration_tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_ray.py` & `ludwig-0.9.3/tests/integration_tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_reducers.py` & `ludwig-0.9.3/tests/integration_tests/test_reducers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_regularizers.py` & `ludwig-0.9.3/tests/integration_tests/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_remote.py` & `ludwig-0.9.3/tests/integration_tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_reproducibility.py` & `ludwig-0.9.3/tests/integration_tests/test_reproducibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_sequence_decoders.py` & `ludwig-0.9.3/tests/integration_tests/test_sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_sequence_encoders.py` & `ludwig-0.9.3/tests/integration_tests/test_sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_sequence_features.py` & `ludwig-0.9.3/tests/integration_tests/test_sequence_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_server.py` & `ludwig-0.9.3/tests/integration_tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_simple_features.py` & `ludwig-0.9.3/tests/integration_tests/test_simple_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_timeseries_feature.py` & `ludwig-0.9.3/tests/integration_tests/test_timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_torchscript.py` & `ludwig-0.9.3/tests/integration_tests/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_trainer.py` & `ludwig-0.9.3/tests/integration_tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_triton.py` & `ludwig-0.9.3/tests/integration_tests/test_triton.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_visualization.py` & `ludwig-0.9.3/tests/integration_tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/test_visualization_api.py` & `ludwig-0.9.3/tests/integration_tests/test_visualization_api.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/integration_tests/utils.py` & `ludwig-0.9.3/tests/integration_tests/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/automl/test_base_config.py` & `ludwig-0.9.3/tests/ludwig/automl/test_base_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/automl/test_data_source.py` & `ludwig-0.9.3/tests/ludwig/automl/test_data_source.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/automl/test_tune_config.py` & `ludwig-0.9.3/tests/ludwig/automl/test_tune_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/automl/test_utils.py` & `ludwig-0.9.3/tests/ludwig/automl/test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/__init__.py` & `ludwig-0.9.3/tests/ludwig/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/check_dead_links.py` & `ludwig-0.9.3/tests/ludwig/datasets/check_dead_links.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/download_all_datasets.py` & `ludwig-0.9.3/tests/ludwig/datasets/download_all_datasets.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/test_dataset_configs.py` & `ludwig-0.9.3/tests/ludwig/datasets/test_dataset_configs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/test_datasets.py` & `ludwig-0.9.3/tests/ludwig/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/datasets/test_model_configs.py` & `ludwig-0.9.3/tests/ludwig/datasets/test_model_configs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_bag_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_category_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_date_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_generic_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_generic_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_h3_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_image_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_image_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_llm_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_llm_encoders.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 import pytest
 import torch
 import torch.nn as nn
 from transformers import AutoConfig, PreTrainedModel
 
 from ludwig.encoders.text_encoders import LLMEncoder
 from ludwig.schema.encoders.text_encoders import LLMEncoderConfig
-from ludwig.schema.llms.peft import BaseAdapterConfig, LoraConfig
+from ludwig.schema.llms.peft import AdaloraConfig, BaseAdapterConfig, IA3Config, LoraConfig
 from ludwig.utils.llm_utils import get_context_len
 
 # Mapping of adapter types to test against and their respective config objects.
-ADAPTER_CONFIG_MAP = {"lora": LoraConfig}
+ADAPTER_CONFIG_MAP = {
+    "adalora": AdaloraConfig,
+    "ia3": IA3Config,
+    "lora": LoraConfig,
+}
 
 
 @pytest.fixture()
 def encoder_config() -> LLMEncoderConfig:
     """Create a baseline LLMEncoderConfig.
 
     Returns:
@@ -54,83 +58,121 @@
             A config object for the requested adapter. If any keyword args are passed, they will be used to initialize
             the config.
         """
         new_config = copy.deepcopy(encoder_config)
         new_config.adapter = ADAPTER_CONFIG_MAP[adapter](**kwargs)
         return new_config
 
+    def adapter_param_name_prefix(self, adapter: str) -> str:
+        """Get the PEFT paramter name prefix for a given adapter type.
+
+        Args:
+            adapter: A valid config value for `adapter.type`
+
+        Returns:
+            The PEFT-applied prefix for the adapter's parameter names.
+
+        Raises:
+            KeyError: raised when the provided adapter name is not valid for LLMEncoder.
+        """
+        return LLMEncoder.ADAPTER_PARAM_NAME_PREFIX[adapter]
+
     def test_init(self, encoder_config: LLMEncoderConfig, model_config):
         # Test initializing without an adapter
         encoder = LLMEncoder(encoder_config=encoder_config)
 
         assert encoder.model_name == encoder_config.base_model
         assert isinstance(encoder.model, PreTrainedModel)
-        assert all(map(lambda k: "lora_" not in k, encoder.state_dict().keys()))  # Check adapter was not initialized
+        # Check adapter was not initialized
+        for k in ADAPTER_CONFIG_MAP.keys():
+            prefix = self.adapter_param_name_prefix(k)
+            assert all(map(lambda k: prefix not in k, encoder.state_dict().keys()))
         assert encoder.input_shape == torch.Size([encoder_config.max_sequence_length])
         assert encoder.output_shape == torch.Size([encoder_config.max_sequence_length, model_config.hidden_size])
 
+        # The final layer must not be trainable because it is not used
+        last_module = list(encoder.model.modules())[-1]
+        assert all(not p.requires_grad for p in last_module.parameters())
+
         # Test that max sequence length falls back to the context length when too large
         context_len = get_context_len(model_config)
         cl_config = copy.deepcopy(encoder_config)
         cl_config.max_sequence_length = context_len + 1
 
         encoder = LLMEncoder(encoder_config=cl_config)
 
         assert encoder.model_name == encoder_config.base_model
         assert isinstance(encoder.model, PreTrainedModel)
-        assert all(map(lambda k: "lora_" not in k, encoder.state_dict().keys()))  # Check adapter was not initialized
+        # Check adapter was not initialized
+        for k in ADAPTER_CONFIG_MAP.keys():
+            prefix = self.adapter_param_name_prefix(k)
+            assert all(map(lambda k: prefix not in k, encoder.state_dict().keys()))
         assert encoder.input_shape == torch.Size([context_len])
         assert encoder.output_shape == torch.Size([context_len, model_config.hidden_size])
 
+        # The final layer must not be trainable because it is not used
+        last_module = list(encoder.model.modules())[-1]
+        assert all(not p.requires_grad for p in last_module.parameters())
+
     @pytest.mark.parametrize("adapter", list(ADAPTER_CONFIG_MAP.keys()))
     def test_init_with_adapter(self, encoder_config: LLMEncoderConfig, adapter: str, model_config):
         from peft import PeftModel
 
         encoder_config_with_adapter = self.create_encoder_config_with_adapter(encoder_config, adapter)
         encoder = LLMEncoder(encoder_config=encoder_config_with_adapter)
+        prefix = self.adapter_param_name_prefix(adapter)
 
         # The adapter should not be initialized until `prepare_for_training` is called
         assert not isinstance(encoder.model, PeftModel)
-        assert not any(map(lambda k: "lora_" in k, encoder.state_dict().keys()))
+        assert not any(map(lambda k: prefix in k, encoder.state_dict().keys()))
 
         assert encoder.model_name == encoder_config.base_model
         assert encoder.input_shape == torch.Size([encoder_config.max_sequence_length])
         assert encoder.output_shape == torch.Size([encoder_config.max_sequence_length, model_config.hidden_size])
 
+        # The final layer must not be trainable because it is not used
+        last_module = list(encoder.model.modules())[-1]
+        assert all(not p.requires_grad for p in last_module.parameters())
+
     @pytest.mark.parametrize("adapter", list(ADAPTER_CONFIG_MAP.keys()))
     def test_prepare_for_training(self, encoder_config: LLMEncoderConfig, adapter: str):
         from peft import PeftModel
 
         encoder_config_with_adapter = self.create_encoder_config_with_adapter(encoder_config, adapter)
         encoder = LLMEncoder(encoder_config=encoder_config_with_adapter)
+        prefix = self.adapter_param_name_prefix(adapter)
 
         # The adapter should not be initialized until `prepare_for_training` is called
         assert not isinstance(encoder.model, PeftModel)
-        assert not any(map(lambda k: "lora_" in k, encoder.state_dict().keys()))
+        assert not any(map(lambda k: prefix in k, encoder.state_dict().keys()))
 
         # Initialize the adapter
         encoder.prepare_for_training()
 
         # At this point, the adapter should be initialized and the state dict should contain adapter parameters
         assert isinstance(encoder.model, PeftModel)
-        assert any(map(lambda k: "lora_" in k, encoder.state_dict().keys()))
+        assert any(map(lambda k: prefix in k, encoder.state_dict().keys()))
 
     def test_save_to_state_dict(self, encoder_config: LLMEncoderConfig, tmpdir):
         # With no adapter, the state dict should only contain the model parameters
         encoder = LLMEncoder(encoder_config=encoder_config)
-        assert all(map(lambda k: "lora_" not in k, encoder.state_dict().keys()))
+        # Check adapter was not initialized
+        for k in ADAPTER_CONFIG_MAP.keys():
+            prefix = self.adapter_param_name_prefix(k)
+            assert all(map(lambda k: prefix not in k, encoder.state_dict().keys()))
 
     @pytest.mark.parametrize("adapter", list(ADAPTER_CONFIG_MAP.keys()))
     def test_save_to_state_dict_adapter(self, encoder_config: LLMEncoderConfig, adapter: str, tmpdir):
         # With an adapter, the state dict should only contain adapter parameters
         encoder_config_with_adapter = self.create_encoder_config_with_adapter(encoder_config, adapter)
         encoder = LLMEncoder(encoder_config=encoder_config_with_adapter)
+        prefix = self.adapter_param_name_prefix(adapter)
         # Initialize the adapters
         encoder.prepare_for_training()
-        assert all(map(lambda k: "lora_" in k, encoder.state_dict().keys()))
+        assert all(map(lambda k: prefix in k, encoder.state_dict().keys()))
 
     @pytest.mark.parametrize("wrap", [False, True], ids=["no_wrapper", "with_wrapper"])
     def test_load_from_state_dict(self, encoder_config: LLMEncoderConfig, wrap: bool):
         def weights_init(m):
             """Reinitialize the weights of a torch module."""
             if hasattr(m, "weight") and m.weight.ndim > 1:
                 torch.nn.init.xavier_uniform_(m.weight.data)
@@ -160,14 +202,16 @@
     @pytest.mark.parametrize("adapter", list(ADAPTER_CONFIG_MAP.keys()))
     def test_load_from_state_dict_adapter(self, encoder_config: LLMEncoderConfig, adapter: str, wrap: bool):
         def weights_init(m):
             """Reinitialize the weights of a torch module."""
             if hasattr(m, "weight") and m.weight.ndim > 1:
                 torch.nn.init.xavier_uniform_(m.weight.data)
 
+        prefix = self.adapter_param_name_prefix(adapter)
+
         # Update the config with an adapter
         encoder_config_with_adapter = self.create_encoder_config_with_adapter(encoder_config, adapter)
 
         # Create two encoders from the same config
         encoder1 = LLMEncoder(encoder_config=encoder_config_with_adapter)
         encoder2 = LLMEncoder(encoder_config=encoder_config_with_adapter)
 
@@ -179,16 +223,16 @@
             encoder1 = WrapperModule(encoder1)
             encoder2 = WrapperModule(encoder2)
 
         encoder2.apply(weights_init)
 
         encoder1_sd = encoder1.state_dict()
         encoder2_sd = encoder2.state_dict()
-        adapter_keys = [k for k in encoder1_sd.keys() if "lora_" in k and "weight" in k]
-        model_keys = [k for k in encoder1_sd.keys() if "lora_" not in k]
+        adapter_keys = [k for k in encoder1_sd.keys() if prefix in k and "weight" in k]
+        model_keys = [k for k in encoder1_sd.keys() if prefix not in k]
 
         # The LoRA weights should no longer be equal
         assert all(map(lambda k: not torch.equal(encoder1_sd[k], encoder2_sd[k]), adapter_keys))
 
         # The remaining weights should also no longer be equal
         assert all(map(lambda k: not torch.equal(encoder1_sd[k], encoder2_sd[k]), model_keys))
```

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_sequence_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_set_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/encoders/test_text_encoders.py` & `ludwig-0.9.3/tests/ludwig/encoders/test_text_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_audio_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_bag_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_binary_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_category_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_date_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_feature_utils.py` & `ludwig-0.9.3/tests/ludwig/features/test_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_h3_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_image_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_number_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_sequence_features.py` & `ludwig-0.9.3/tests/ludwig/features/test_sequence_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_set_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_text_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/features/test_timeseries_feature.py` & `ludwig-0.9.3/tests/ludwig/features/test_timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/models/__init__.py` & `ludwig-0.9.3/tests/ludwig/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/models/test_trainable_image_layers.py` & `ludwig-0.9.3/tests/ludwig/models/test_trainable_image_layers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/models/test_training_determinism.py` & `ludwig-0.9.3/tests/ludwig/models/test_training_determinism.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/models/test_training_success.py` & `ludwig-0.9.3/tests/ludwig/models/test_training_success.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/__init__.py` & `ludwig-0.9.3/tests/ludwig/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_attention.py` & `ludwig-0.9.3/tests/ludwig/modules/test_attention.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_convolutional_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_convolutional_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_embedding_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_embedding_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_encoder.py` & `ludwig-0.9.3/tests/ludwig/modules/test_encoder.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_fully_connected_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_fully_connected_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_initializer_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_initializer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_loss_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_loss_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_lr_scheduler.py` & `ludwig-0.9.3/tests/ludwig/modules/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_metric_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_metric_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_mlp_mixer_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_mlp_mixer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_normalization_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_normalization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_recurrent_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_recurrent_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_reduction_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_reduction_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_tabnet_modules.py` & `ludwig-0.9.3/tests/ludwig/modules/test_tabnet_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/modules/test_utils.py` & `ludwig-0.9.3/tests/ludwig/modules/test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/__init__.py` & `ludwig-0.9.3/tests/ludwig/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_algorithm_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_audio_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_backward_compatibility.py` & `ludwig-0.9.3/tests/ludwig/utils/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_calibration.py` & `ludwig-0.9.3/tests/ludwig/utils/test_calibration.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_class_balancing.py` & `ludwig-0.9.3/tests/ludwig/utils/test_class_balancing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_config_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_data_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_dataframe_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_dataset_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_date_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_date_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_defaults.py` & `ludwig-0.9.3/tests/ludwig/utils/test_defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_error_handling_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_error_handling_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_errors.py` & `ludwig-0.9.3/tests/ludwig/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_fs_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_fs_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_heuristics.py` & `ludwig-0.9.3/tests/ludwig/utils/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_hf_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_hf_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_hyperopt_ray_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_hyperopt_ray_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_image_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_llm_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_metric_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_metric_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_model_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_normalization.py` & `ludwig-0.9.3/tests/ludwig/utils/test_normalization.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_numerical_test_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_numerical_test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_output_feature_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_output_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_server_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_server_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_state_dict_backward_compatibility.py` & `ludwig-0.9.3/tests/ludwig/utils/test_state_dict_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_strings_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_strings_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_tokenizers.py` & `ludwig-0.9.3/tests/ludwig/utils/test_tokenizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_torch_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_trainer_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_trainer_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_upload_utils.py` & `ludwig-0.9.3/tests/ludwig/utils/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/ludwig/utils/test_version_transformation.py` & `ludwig-0.9.3/tests/ludwig/utils/test_version_transformation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/training_success/configs.py` & `ludwig-0.9.3/tests/training_success/configs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.9.2/tests/training_success/test_training_success.py` & `ludwig-0.9.3/tests/training_success/test_training_success.py`

 * *Files identical despite different names*

