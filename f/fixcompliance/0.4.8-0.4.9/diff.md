# Comparing `tmp/fixcompliance-0.4.8.tar.gz` & `tmp/fixcompliance-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixcompliance-0.4.8.tar", last modified: Wed Mar 13 19:29:29 2024, max compression
+gzip compressed data, was "fixcompliance-0.4.9.tar", last modified: Wed Mar 13 19:55:20 2024, max compression
```

## Comparing `fixcompliance-0.4.8.tar` & `fixcompliance-0.4.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.315545 fixcompliance-0.4.8/fixcompliance/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.315545 fixcompliance-0.4.8/fixcompliance/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.315545 fixcompliance-0.4.8/fixcompliance/data/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.319545 fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (127)    43571 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)    43418 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_cis_2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)    71662 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_well_architected_framework_security_pillar.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/waf_notes.md
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.315545 fixcompliance-0.4.8/fixcompliance/data/checks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/fixcompliance/data/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_acm.json
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_autoscaling.json
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudformation.json
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudfront.json
--rw-r--r--   0 runner    (1001) docker     (127)    54532 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudwatch.json
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_dms.json
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_dynamodb.json
--rw-r--r--   0 runner    (1001) docker     (127)   105818 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ecr.json
--rw-r--r--   0 runner    (1001) docker     (127)    15152 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ecs.json
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_eks.json
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_elb.json
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_glacier.json
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_opensearch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_organizations.json
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_redshift.json
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_route53.json
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sagemaker.json
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_secretsmanager.json
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sns.json
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sqs.json
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ssm.json
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_wafv2.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/fixcompliance/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/fixcompliance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-13 19:29:29.000000 fixcompliance-0.4.8/fixcompliance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-13 19:29:29.000000 fixcompliance-0.4.8/fixcompliance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:29:29.000000 fixcompliance-0.4.8/fixcompliance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:28:33.000000 fixcompliance-0.4.8/fixcompliance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-13 19:29:29.000000 fixcompliance-0.4.8/fixcompliance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:29:29.323545 fixcompliance-0.4.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-13 19:28:12.000000 fixcompliance-0.4.8/test/test_from_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.434894 fixcompliance-0.4.9/fixcompliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.438894 fixcompliance-0.4.9/fixcompliance/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.434894 fixcompliance-0.4.9/fixcompliance/data/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.438894 fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)    43571 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43418 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_cis_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    71662 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_well_architected_framework_security_pillar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/waf_notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.434894 fixcompliance-0.4.9/fixcompliance/data/checks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/fixcompliance/data/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_acm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_autoscaling.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudformation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudfront.json
+-rw-r--r--   0 runner    (1001) docker     (127)    54532 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudwatch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_dms.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_dynamodb.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105818 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ecr.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15152 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ecs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_eks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_elb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_glacier.json
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_organizations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_redshift.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_route53.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sagemaker.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_secretsmanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sns.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sqs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ssm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_wafv2.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/fixcompliance/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/fixcompliance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-13 19:55:20.000000 fixcompliance-0.4.9/fixcompliance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-13 19:55:20.000000 fixcompliance-0.4.9/fixcompliance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:55:20.000000 fixcompliance-0.4.9/fixcompliance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:54:23.000000 fixcompliance-0.4.9/fixcompliance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-13 19:55:20.000000 fixcompliance-0.4.9/fixcompliance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:55:20.442894 fixcompliance-0.4.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-13 19:54:03.000000 fixcompliance-0.4.9/test/test_from_files.py
```

### Comparing `fixcompliance-0.4.8/PKG-INFO` & `fixcompliance-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixcompliance
-Version: 0.4.8
+Version: 0.4.9
 Summary: Fix Inventory Compliance Benchmarks and Checks
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixmetrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `fixcompliance-0.4.8/fixcompliance/__init__.py` & `fixcompliance-0.4.9/fixcompliance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import time
 import threading
 from typing import Any
 from importlib.resources import files as resource_filename
 from pathlib import Path
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 Json = dict[str, Any]
 CACHE_TIMEOUT = 3600
 _cache: dict[str, Any] = {}
 _cache_lock = threading.Lock()
```

### Comparing `fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_cis_1_5.json` & `fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_cis_2_0.json` & `fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_cis_2_0.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/benchmark/aws/aws_well_architected_framework_security_pillar.json` & `fixcompliance-0.4.9/fixcompliance/data/benchmark/aws/aws_well_architected_framework_security_pillar.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/check_template.json` & `fixcompliance-0.4.9/fixcompliance/data/check_template.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_acm.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_acm.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_apigateway.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_autoscaling.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_autoscaling.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudformation.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudformation.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudfront.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudfront.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudtrail.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_cloudwatch.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_cloudwatch.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_config.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_dms.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_dms.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_dynamodb.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_dynamodb.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ec2.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ecr.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ecr.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ecs.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ecs.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_efs.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_eks.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_eks.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_elb.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_elb.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_glacier.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_glacier.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_iam.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_kms.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_lambda.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_opensearch.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_opensearch.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_organizations.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_organizations.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_rds.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_redshift.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_redshift.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_route53.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_route53.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_s3.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sagemaker.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sagemaker.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_secretsmanager.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_secretsmanager.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sns.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sns.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_sqs.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_sqs.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_ssm.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_ssm.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance/data/checks/aws/aws_wafv2.json` & `fixcompliance-0.4.9/fixcompliance/data/checks/aws/aws_wafv2.json`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/fixcompliance.egg-info/PKG-INFO` & `fixcompliance-0.4.9/fixcompliance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixcompliance
-Version: 0.4.8
+Version: 0.4.9
 Summary: Fix Inventory Compliance Benchmarks and Checks
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixmetrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `fixcompliance-0.4.8/fixcompliance.egg-info/SOURCES.txt` & `fixcompliance-0.4.9/fixcompliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixcompliance-0.4.8/pyproject.toml` & `fixcompliance-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixcompliance"
-version = "0.4.8"
+version = "0.4.9"
 authors = [
     { name = "Some Engineering Inc." },
 ]
 description = "Fix Inventory Compliance Benchmarks and Checks"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

