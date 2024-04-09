# Comparing `tmp/keras-nightly-3.2.0.dev2024040803.tar.gz` & `tmp/keras-nightly-3.2.0.dev2024040818.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nightly-3.2.0.dev2024040803.tar", last modified: Mon Apr  8 03:20:22 2024, max compression
+gzip compressed data, was "keras-nightly-3.2.0.dev2024040818.tar", last modified: Mon Apr  8 18:13:27 2024, max compression
```

## Comparing `keras-nightly-3.2.0.dev2024040803.tar` & `keras-nightly-3.2.0.dev2024040818.tar`

### file list

```diff
@@ -1,691 +1,691 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.715318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.719318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.723318 keras-nightly-3.2.0.dev2024040803/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.727318 keras-nightly-3.2.0.dev2024040803/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.731318 keras-nightly-3.2.0.dev2024040803/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.735318 keras-nightly-3.2.0.dev2024040803/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.735318 keras-nightly-3.2.0.dev2024040803/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.735318 keras-nightly-3.2.0.dev2024040803/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.735318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.739318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.739318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.743318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.747318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    35373 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.747318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.747318 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.751318 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.751318 keras-nightly-3.2.0.dev2024040803/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31619 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.755318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.759318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.759318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.759318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    62696 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.763318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.763318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.767318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.771318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.771318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.775318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.775318 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.775318 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.779318 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.779318 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.779318 keras-nightly-3.2.0.dev2024040803/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.783318 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.783318 keras-nightly-3.2.0.dev2024040803/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32036 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.783318 keras-nightly-3.2.0.dev2024040803/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   189853 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.787318 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    36189 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.787318 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.787318 keras-nightly-3.2.0.dev2024040803/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.787318 keras-nightly-3.2.0.dev2024040803/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.791318 keras-nightly-3.2.0.dev2024040803/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.791318 keras-nightly-3.2.0.dev2024040803/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.791318 keras-nightly-3.2.0.dev2024040803/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.791318 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.791318 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45199 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26523 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 03:20:17.000000 keras-nightly-3.2.0.dev2024040803/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-08 03:20:22.000000 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-08 03:20:22.000000 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:20:22.000000 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 03:20:22.000000 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 03:20:22.000000 keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:20:22.799318 keras-nightly-3.2.0.dev2024040803/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 03:20:20.000000 keras-nightly-3.2.0.dev2024040803/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.908118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.912118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.916118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.920118 keras-nightly-3.2.0.dev2024040818/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.924118 keras-nightly-3.2.0.dev2024040818/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.928118 keras-nightly-3.2.0.dev2024040818/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.932118 keras-nightly-3.2.0.dev2024040818/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.932118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.932118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.936118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.936118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.940118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.944118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.944118 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.948118 keras-nightly-3.2.0.dev2024040818/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.952118 keras-nightly-3.2.0.dev2024040818/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.952118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.952118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.952118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.956118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.956118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62696 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.960118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.960118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.960118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.964118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.968118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.968118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.972118 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.972118 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.972118 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.972118 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.972118 keras-nightly-3.2.0.dev2024040818/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.976118 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.976118 keras-nightly-3.2.0.dev2024040818/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32036 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.980118 keras-nightly-3.2.0.dev2024040818/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189853 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.980118 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36189 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.980118 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.980118 keras-nightly-3.2.0.dev2024040818/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.984118 keras-nightly-3.2.0.dev2024040818/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.984118 keras-nightly-3.2.0.dev2024040818/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.984118 keras-nightly-3.2.0.dev2024040818/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.984118 keras-nightly-3.2.0.dev2024040818/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.984118 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.988118 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45199 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26523 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 18:13:22.000000 keras-nightly-3.2.0.dev2024040818/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-08 18:13:27.000000 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-08 18:13:27.000000 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:13:27.000000 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 18:13:27.000000 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 18:13:27.000000 keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:13:27.992118 keras-nightly-3.2.0.dev2024040818/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 18:13:26.000000 keras-nightly-3.2.0.dev2024040818/setup.py
```

### Comparing `keras-nightly-3.2.0.dev2024040803/PKG-INFO` & `keras-nightly-3.2.0.dev2024040818/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024040803
+Version: 3.2.0.dev2024040818
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024040803/README.md` & `keras-nightly-3.2.0.dev2024040818/README.md`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.2.0.dev2024040803"
+__version__ = "3.2.0.dev2024040818"
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/config/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/distribution/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/random/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/tree/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/_tf_keras/keras/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/applications/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/config/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/distribution/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/ops/nn/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/random/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/activations/activations.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/api_export.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/convnext.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/densenet.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/efficientnet.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/efficientnet_v2.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/imagenet_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/inception_resnet_v2.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/inception_v3.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet_v2.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/mobilenet_v3.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/nasnet.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/resnet.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/resnet_v2.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/vgg16.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/vgg19.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/applications/xception.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/backend_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/dtypes.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/global_state.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/keras_tensor.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/name_scope.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/stateless_scope.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/common/variables.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/config.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/exports.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/core.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/linalg.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/math.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/nn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/numpy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/random.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/sparse.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/jax/trainer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/core.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/linalg.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/math.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/nn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/numpy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/random.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         random_numbers = np.append(random_numbers, valid)
 
     # Truncate the result array to the desired size and reshape it
     return random_numbers[:flat_shape].astype(dtype).reshape(shape)
 
 
 def dropout(inputs, rate, noise_shape=None, seed=None):
+    dtype = inputs.dtype
     seed = draw_seed(seed)
 
     keep_prob = 1.0 - rate
 
     # If noise_shape is not provided, use the shape of inputs
     if noise_shape is None:
         noise_shape = inputs.shape
@@ -81,15 +82,17 @@
             n if n is not None else inputs.shape[i]
             for i, n in enumerate(noise_shape)
         ]
 
     rng = np.random.default_rng(seed)
     mask = rng.uniform(size=noise_shape) < keep_prob
     mask = np.broadcast_to(mask, inputs.shape)
-    return np.where(mask, inputs / keep_prob, np.zeros_like(inputs))
+    return np.where(
+        mask, (inputs / keep_prob).astype(dtype), np.zeros_like(inputs)
+    )
 
 
 def shuffle(x, axis=0, seed=None):
     seed = draw_seed(seed)
     rng = np.random.default_rng(seed)
     return rng.permuted(x, axis=axis)
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/numpy/trainer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/core.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/linalg.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/math.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/nn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/numpy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/random.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/random.py`

 * *Files 25% similar despite different names*

```diff
@@ -95,33 +95,46 @@
     x = tfnp.swapaxes(x, axis1=0, axis2=axis)
     return x
 
 
 def gamma(shape, alpha, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
-    return tf.random.stateless_gamma(
-        shape,
-        alpha=alpha,
-        dtype=dtype,
-        seed=seed,
+    # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    return tf.cast(
+        tf.random.stateless_gamma(
+            shape,
+            alpha=alpha,
+            dtype=intemediate_dtype,
+            seed=seed,
+        ),
+        dtype,
     )
 
 
 def binomial(shape, counts, probabilities, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
-    sample = tf.random.stateless_binomial(
-        shape=shape,
-        seed=seed,
-        counts=counts,
-        probs=probabilities,
-        output_dtype=dtype,
+    # TODO: `tf.random.stateless_binomial` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    return tf.cast(
+        tf.random.stateless_binomial(
+            shape=shape,
+            seed=seed,
+            counts=counts,
+            probs=probabilities,
+            output_dtype=intemediate_dtype,
+        ),
+        dtype,
     )
-    return sample
 
 
 def beta(shape, alpha, beta, dtype=None, seed=None):
     dtype = dtype or floatx()
     # since tensorflow doesn't offer a beta distribution function
     # so we'll use the formula U(a,b) = (X(a) / (X(a) + Y(b)),
     # where U(a,b) is a beta-distributed random variable with
@@ -134,32 +147,42 @@
     # due to the usage of same seed.
     seed_1 = tf_draw_seed(seed)
     # The choice of 12 is totally arbitrary, as we're
     # incrementing the first drawn seed by a CONSTANT to
     # ensure deterministic results.
     seed_2 = seed_1 + 12
 
-    alpha = tf.convert_to_tensor(alpha, dtype=dtype)
-    beta = tf.convert_to_tensor(beta, dtype=dtype)
+    # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    alpha = tf.convert_to_tensor(alpha, dtype=intemediate_dtype)
+    beta = tf.convert_to_tensor(beta, dtype=intemediate_dtype)
 
     # tensorflow's tf.random.stateless_gamma has a bit of unconventional
     # implementation of the stateless_gamma function where it checks the
     # broadcastability of alpha's shape with ONLY the RIGHTMOST dimension of
     # the specified output shape instead of considering the whole.
     # Consequently, it then results in errors for perfectly broadcastable shapes
     # such as for output shape of (2, 3) and alpha shape of (1, 3)
     # So to resolve this, we explicitly broadcast alpha and beta to shape before
     # passing them to the stateless_gamma function.
     if tf.rank(alpha) > 1:
         alpha = tf.broadcast_to(alpha, shape)
     if tf.rank(beta) > 1:
         beta = tf.broadcast_to(beta, shape)
 
-    gamma_a = tf.random.stateless_gamma(
-        shape=shape, seed=seed_1, alpha=alpha, dtype=dtype
+    gamma_a = tf.cast(
+        tf.random.stateless_gamma(
+            shape=shape, seed=seed_1, alpha=alpha, dtype=intemediate_dtype
+        ),
+        dtype,
     )
-    gamma_b = tf.random.stateless_gamma(
-        shape=shape, seed=seed_2, alpha=beta, dtype=dtype
+    gamma_b = tf.cast(
+        tf.random.stateless_gamma(
+            shape=shape, seed=seed_2, alpha=beta, dtype=intemediate_dtype
+        ),
+        dtype,
     )
     sample = gamma_a / (gamma_a + gamma_b)
     return sample
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -678,21 +678,28 @@
     return_sequences,
 ):
     """GRU with cuDNN implementation which is only available for GPU."""
     if mask is not None:
         _assert_valid_mask(mask)
         sequence_lengths = _compute_sequence_length_from_mask(mask, time_major)
     else:
-        sequence_lengths = None
+        if time_major:
+            batch_dim = tf.shape(inputs)[1]
+            max_sequence_length = tf.shape(inputs)[0]
+        else:
+            batch_dim = tf.shape(inputs)[0]
+            max_sequence_length = tf.shape(inputs)[1]
+        sequence_lengths = tf.fill([batch_dim], max_sequence_length)
 
     if not time_major and sequence_lengths is None:
         inputs = tf.transpose(inputs, perm=(1, 0, 2))
         seq_axis, batch_axis = (0, 1)
     else:
         seq_axis, batch_axis = (0, 1) if time_major else (1, 0)
+
     # For init_h, cuDNN expects one more dim of num_layers before or after batch
     # dim for time major or batch major inputs respectively
     init_h = tf.expand_dims(initial_state, axis=seq_axis)
 
     weights = tf.split(kernel, 3, axis=1)
     weights += tf.split(recurrent_kernel, 3, axis=1)
     # Note that the bias was initialized as shape (2, 3 * units), flatten it to
@@ -715,57 +722,44 @@
     params = _standardize_cudnn_weights(
         weights=weights,
         biases=bias,
         shape=tf.constant([-1]),
         transpose_weights=True,
     )
 
-    if sequence_lengths is not None:
-        if go_backwards:
-            # Three reversals are required. E.g.,
-            # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
-            # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
-            # output_from_cudnn = [6, 5, 4, 0, 0]
-            # expected_output = [0, 0, 6, 5 ,4]
-            inputs = tf.reverse_sequence(
-                inputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-        outputs, h, _, _, _ = tf.raw_ops.CudnnRNNV3(
-            input=inputs,
-            input_h=init_h,
-            input_c=0,
-            params=params,
-            is_training=True,
-            rnn_mode="gru",
-            sequence_lengths=sequence_lengths,
-            time_major=time_major,
+    if go_backwards:
+        # Three reversals are required. E.g.,
+        # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
+        # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
+        # output_from_cudnn = [6, 5, 4, 0, 0]
+        # expected_output = [0, 0, 6, 5 ,4]
+        inputs = tf.reverse_sequence(
+            inputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
-        if go_backwards:
-            outputs = tf.reverse_sequence(
-                outputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-            outputs = tf.reverse(outputs, axis=[seq_axis])
-    else:
-        if go_backwards:
-            # Reverse axis 0 since the input is already convert to time major.
-            inputs = tf.reverse(inputs, axis=[0])
-        outputs, h, _, _ = tf.raw_ops.CudnnRNN(
-            input=inputs,
-            input_h=init_h,
-            input_c=0,
-            params=params,
-            is_training=True,
-            rnn_mode="gru",
+    outputs, h, _, _, _ = tf.raw_ops.CudnnRNNV3(
+        input=inputs,
+        input_h=init_h,
+        input_c=0,
+        params=params,
+        is_training=True,
+        rnn_mode="gru",
+        sequence_lengths=sequence_lengths,
+        time_major=time_major,
+    )
+    if go_backwards:
+        outputs = tf.reverse_sequence(
+            outputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
+        outputs = tf.reverse(outputs, axis=[seq_axis])
 
     last_output = outputs[-1]
     if not time_major and sequence_lengths is None and return_sequences:
         outputs = tf.transpose(outputs, perm=[1, 0, 2])
     state = tf.squeeze(h, axis=seq_axis)
 
     # In the case of variable length input, the cudnn kernel will fill zeros for
@@ -876,15 +870,21 @@
     go_backwards,
     return_sequences,
 ):
     if mask is not None:
         _assert_valid_mask(mask)
         sequence_lengths = _compute_sequence_length_from_mask(mask, time_major)
     else:
-        sequence_lengths = None
+        if time_major:
+            batch_dim = tf.shape(inputs)[1]
+            max_sequence_length = tf.shape(inputs)[0]
+        else:
+            batch_dim = tf.shape(inputs)[0]
+            max_sequence_length = tf.shape(inputs)[1]
+        sequence_lengths = tf.fill([batch_dim], max_sequence_length)
 
     if not time_major and sequence_lengths is None:
         inputs = tf.transpose(inputs, perm=(1, 0, 2))
         seq_axis, batch_axis = (0, 1)
     else:
         seq_axis, batch_axis = (0, 1) if time_major else (1, 0)
     # For init_h and init_c, cuDNN expects one more dim of num_layers before or
@@ -914,60 +914,44 @@
     params = _standardize_cudnn_weights(
         weights=weights,
         biases=tf.split(full_bias, 8),
         shape=tf.constant([-1]),
         transpose_weights=True,
     )
 
-    if sequence_lengths is not None:
-        if go_backwards:
-            # Three reversals are required. E.g.,
-            # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
-            # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
-            # output_from_cudnn = [6, 5, 4, 0, 0]
-            # expected_output = [0, 0, 6, 5 ,4]
-            inputs = tf.reverse_sequence(
-                inputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-        outputs, h, c, _, _ = tf.raw_ops.CudnnRNNV3(
-            input=inputs,
-            input_h=init_h,
-            input_c=init_c,
-            params=params,
-            is_training=True,
-            rnn_mode="lstm",
-            sequence_lengths=sequence_lengths,
-            time_major=time_major,
+    if go_backwards:
+        # Three reversals are required. E.g.,
+        # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
+        # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
+        # output_from_cudnn = [6, 5, 4, 0, 0]
+        # expected_output = [0, 0, 6, 5 ,4]
+        inputs = tf.reverse_sequence(
+            inputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
-        if go_backwards:
-            outputs = tf.reverse_sequence(
-                outputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-            outputs = tf.reverse(outputs, axis=[seq_axis])
-    else:
-        # # Fill the array with shape [batch] with value of max timesteps.
-        # sequence_length = array_ops.fill([array_ops.shape(inputs)[1]],
-        #                                  array_ops.shape(inputs)[0])
-        if go_backwards:
-            # Reverse axis 0 since the input is already convert to time major.
-            inputs = tf.reverse(inputs, axis=[0])
-        outputs, h, c, _ = tf.raw_ops.CudnnRNN(
-            input=inputs,
-            input_h=init_h,
-            input_c=init_c,
-            params=params,
-            is_training=True,
-            rnn_mode="lstm",
+    outputs, h, c, _, _ = tf.raw_ops.CudnnRNNV3(
+        input=inputs,
+        input_h=init_h,
+        input_c=init_c,
+        params=params,
+        is_training=True,
+        rnn_mode="lstm",
+        sequence_lengths=sequence_lengths,
+        time_major=time_major,
+    )
+    if go_backwards:
+        outputs = tf.reverse_sequence(
+            outputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
+        outputs = tf.reverse(outputs, axis=[seq_axis])
 
     last_output = outputs[-1]
     if not time_major and sequence_lengths is None and return_sequences:
         outputs = tf.transpose(outputs, perm=[1, 0, 2])
     h = tf.squeeze(h, axis=seq_axis)
     c = tf.squeeze(c, axis=seq_axis)
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/sparse.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/trackable.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/tensorflow/trainer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/core.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/linalg.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/math.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/nn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/numpy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/random.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,21 @@
         generator=generator,
         dtype=dtype,
         device=get_device(),
     )
 
 
 def truncated_normal(shape, mean=0.0, stddev=1.0, dtype=None, seed=None):
+    dtype = to_torch_dtype(dtype)
     # Take a larger standard normal dist, discard values outside 2 * stddev
     # Offset by mean and stddev
     x = normal(tuple(shape) + (4,), mean=0, stddev=1, dtype=dtype, seed=seed)
     valid = (x > -2) & (x < 2)
     indexes = valid.max(-1, keepdim=True)[1]
-    trunc_x = torch.empty(shape, device=get_device())
+    trunc_x = torch.empty(shape, dtype=dtype, device=get_device())
     trunc_x.data.copy_(x.gather(-1, indexes).squeeze(-1))
     trunc_x.data.mul_(stddev).add_(mean)
     return trunc_x
 
 
 def _get_concrete_noise_shape(inputs, noise_shape):
     if noise_shape is None:
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/backend/torch/trainer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/backup_and_restore.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/callback.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/callback_list.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/csv_logger.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/early_stopping.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/history.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/lambda_callback.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/learning_rate_scheduler.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/model_checkpoint.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/progbar_logger.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/remote_monitor.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/swap_ema_weights.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/tensorboard.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/callbacks/terminate_on_nan.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/constraints/constraints.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/boston_housing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/california_housing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar10.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/cifar100.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/fashion_mnist.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/imdb.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/mnist.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/datasets/reuters.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/distribution/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/distribution/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/dtype_policies/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/dtype_policies/dtype_policy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/export/export_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/export/export_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Library for exporting inference-only Keras models/layers."""
 
 import inspect
+import itertools
+import string
 
 from absl import logging
 
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.layers import Layer
@@ -211,18 +213,20 @@
                 2) provide an `input_signature` argument that specifies the
                 shape and dtype of the inputs (see below).
             input_signature: Used to specify the shape and dtype of the
                 inputs to `fn`. List of `tf.TensorSpec` objects (one
                 per positional input argument of `fn`). Nested arguments are
                 allowed (see below for an example showing a Functional model
                 with 2 input arguments).
-            jax2tf_kwargs: Dict for additional arguments to pass to `jax2tf`.
+            jax2tf_kwargs: Optional. A dict for arguments to pass to `jax2tf`.
                 Supported only when the backend is JAX. See documentation for
                 [`jax2tf.convert`](
                     https://github.com/google/jax/blob/main/jax/experimental/jax2tf/README.md).
+                The values for `native_serialization` and `polymorphic_shapes`,
+                if not provided, are automatically computed.
 
         Returns:
             The `tf.function` wrapping `fn` that was added to the archive.
 
         Example:
 
         Adding an endpoint using the `input_signature` argument when the
@@ -331,21 +335,17 @@
                 #    original function
                 # 5. Wrap in a `tf.function`
                 def stateless_fn(variables, *args, **kwargs):
                     state_mapping = zip(self._backend_variables, variables)
                     with StatelessScope(state_mapping=state_mapping):
                         return fn(*args, **kwargs)
 
-                variables_spec = [
-                    _make_tensor_spec(v) for v in self._backend_variables
-                ]
-
                 jax2tf_stateless_fn = self._convert_jax2tf_function(
                     stateless_fn,
-                    [variables_spec] + input_signature,
+                    input_signature,
                     jax2tf_kwargs=jax2tf_kwargs,
                 )
 
                 def stateful_fn(*args, **kwargs):
                     return jax2tf_stateless_fn(
                         # Change the trackable `ListWrapper` to a plain `list`
                         list(self._tf_trackable.variables),
@@ -539,35 +539,59 @@
                         self._tf_trackable._misc_assets.append(trackable)
 
     def _convert_jax2tf_function(self, fn, input_signature, jax2tf_kwargs=None):
         from jax.experimental import jax2tf
 
         if jax2tf_kwargs is None:
             jax2tf_kwargs = {}
+
         if "native_serialization" not in jax2tf_kwargs:
             jax2tf_kwargs["native_serialization"] = (
                 self._check_device_compatible()
             )
 
-        shapes = []
-        for spec in input_signature:
-            shapes.append(self._spec_to_poly_shape(spec))
-
-        return jax2tf.convert(
-            fn,
-            polymorphic_shapes=shapes,
-            **jax2tf_kwargs,
+        variables_shapes = self._to_polymorphic_shape(
+            self._backend_variables, allow_none=False
         )
+        if "polymorphic_shapes" in jax2tf_kwargs:
+            input_shapes = jax2tf_kwargs["polymorphic_shapes"]
+        else:
+            input_shapes = self._to_polymorphic_shape(input_signature)
+        jax2tf_kwargs["polymorphic_shapes"] = [variables_shapes] + input_shapes
+
+        return jax2tf.convert(fn, **jax2tf_kwargs)
 
-    def _spec_to_poly_shape(self, spec):
-        if isinstance(spec, (dict, list)):
-            return tree.map_structure(self._spec_to_poly_shape, spec)
-        spec_shape = spec.shape
-        spec_shape = str(spec_shape).replace("None", "b")
-        return spec_shape
+    def _to_polymorphic_shape(self, struct, allow_none=True):
+        if allow_none:
+            # Generates unique names: a, b, ... z, aa, ab, ... az, ba, ... zz
+            # for unknown non-batch dims. Defined here to be scope per endpoint.
+            dim_names = itertools.chain(
+                string.ascii_lowercase,
+                itertools.starmap(
+                    lambda a, b: a + b,
+                    itertools.product(string.ascii_lowercase, repeat=2),
+                ),
+            )
+
+        def convert_shape(x):
+            poly_shape = []
+            for index, dim in enumerate(list(x.shape)):
+                if dim is not None:
+                    poly_shape.append(str(dim))
+                elif not allow_none:
+                    raise ValueError(
+                        f"Illegal None dimension in {x} with shape {x.shape}"
+                    )
+                elif index == 0:
+                    poly_shape.append("batch")
+                else:
+                    poly_shape.append(next(dim_names))
+            return "(" + ", ".join(poly_shape) + ")"
+
+        return tree.map_structure(convert_shape, struct)
 
     def _check_device_compatible(self):
         from jax import default_backend as jax_device
 
         if (
             jax_device() == "gpu"
             and len(tf.config.list_physical_devices("GPU")) == 0
@@ -608,22 +632,24 @@
 
 def _get_save_spec(model):
     shapes_dict = getattr(model, "_build_shapes_dict", None)
     if not shapes_dict:
         return None
 
     if len(shapes_dict) == 1:
-        return tf.TensorSpec(
-            shape=list(shapes_dict.values())[0], dtype=model.input_dtype
-        )
+        shape = list(shapes_dict.values())[0]
+        shape = (None,) + shape[1:]
+        return tf.TensorSpec(shape=shape, dtype=model.input_dtype)
 
     specs = {}
-    for key, value in shapes_dict.items():
+    for key, shape in shapes_dict.items():
         key = key.rstrip("_shape")
-        specs[key] = tf.TensorSpec(shape=value, dtype=model.input_dtype)
+        shape = (None,) + shape[1:]
+        specs[key] = tf.TensorSpec(shape=shape, dtype=model.input_dtype)
+
     return specs
 
 
 @keras_export("keras.layers.TFSMLayer")
 class TFSMLayer(Layer):
     """Reload a Keras model/layer that was saved via SavedModel / ExportArchive.
 
@@ -754,15 +780,16 @@
             "call_endpoint": self.call_endpoint,
             "call_training_endpoint": self.call_training_endpoint,
         }
         return {**base_config, **config}
 
 
 def _make_tensor_spec(x):
-    return tf.TensorSpec(x.shape, dtype=x.dtype, name=x.name)
+    shape = (None,) + x.shape[1:]
+    return tf.TensorSpec(shape, dtype=x.dtype, name=x.name)
 
 
 def _print_signature(fn, name):
     concrete_fn = fn._list_all_concrete_functions()[0]
     pprinted_signature = concrete_fn.pretty_printed_signature(verbose=True)
     lines = pprinted_signature.split("\n")
     lines = [f"* Endpoint '{name}'"] + lines[1:]
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/initializers/constant_initializers.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/initializers/initializer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/initializers/random_initializers.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/activation.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/elu.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/leaky_relu.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/prelu.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/relu.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/activations/softmax.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/additive_attention.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/attention.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/grouped_query_attention.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/attention/multi_head_attention.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_conv.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/base_separable_conv.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/separable_conv1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/convolutional/separable_conv2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/dense.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/einsum_dense.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/embedding.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/identity.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/input_layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/lambda_layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/masking.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/core/wrapper.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/input_spec.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/add.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/average.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/base_merge.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/concatenate.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/dot.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/maximum.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/minimum.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/multiply.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/merging/subtract.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/batch_normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/group_normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/layer_normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/spectral_normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/normalization/unit_normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/average_pooling3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/base_global_pooling.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/base_pooling.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/pooling/max_pooling3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/category_encoding.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/center_crop.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/discretization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/feature_space.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/hashing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/index_lookup.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/integer_lookup.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/normalization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_brightness.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_contrast.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_crop.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_flip.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_rotation.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_translation.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/random_zoom.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/rescaling.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/resizing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/string_lookup.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/text_vectorization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/activity_regularization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/alpha_dropout.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/dropout.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/gaussian_dropout.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     def call(self, inputs, training=False):
         if training and self.rate > 0:
             stddev = math.sqrt(self.rate / (1.0 - self.rate))
             return inputs * backend.random.normal(
                 shape=ops.shape(inputs),
                 mean=1.0,
                 stddev=stddev,
+                dtype=self.compute_dtype,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/gaussian_noise.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/gaussian_noise.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     def call(self, inputs, training=False):
         if training and self.stddev > 0:
             return inputs + backend.random.normal(
                 shape=ops.shape(inputs),
                 mean=0.0,
                 stddev=self.stddev,
+                dtype=self.compute_dtype,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/regularization/spatial_dropout.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/cropping3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/flatten.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/permute.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/repeat_vector.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/reshape.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/up_sampling3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/reshaping/zero_padding3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/bidirectional.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm1d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm2d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/conv_lstm3d.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/gru.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/lstm.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/simple_rnn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/layers/rnn/time_distributed.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/backend.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/layers.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/losses.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/sequence.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/preprocessing/text.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/json_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/legacy_h5_format.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/saving_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/legacy/saving/serialization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/losses/loss.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/losses/losses.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/accuracy_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/confusion_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/f_score_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/hinge_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/iou_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/metric.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/metrics_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/probabilistic_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/reduction_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/metrics/regression_metrics.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/models/cloning.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/models/functional.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/models/model.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/models/sequential.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/models/variable_mapping.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/core.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/function.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/image.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/linalg.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/math.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/nn.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/node.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/numpy.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/operation.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/operation_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/ops/symbolic_arguments.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adadelta.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adafactor.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adagrad.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adam.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adamax.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/adamw.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/base_optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/ftrl.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/lion.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/loss_scale_optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/nadam.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/optimizer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/rmsprop.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/optimizers/sgd.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/quantizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/quantizers/quantizers.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/random/random.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/random/seed_generator.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/regularizers/regularizers.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/saving/object_registration.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/saving/saving_api.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/saving/saving_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             model, filepath, overwrite, include_optimizer
         )
     else:
         raise ValueError(
             "Invalid filepath extension for saving. "
             "Please add either a `.keras` extension for the native Keras "
             f"format (recommended) or a `.h5` extension. "
-            "Use `tf.saved_model.save()` if you want to export a SavedModel "
+            "Use `model.export(filepath)` if you want to export a SavedModel "
             "for use with TFLite/TFServing/etc. "
             f"Received: filepath={filepath}."
         )
 
 
 @keras_export(["keras.saving.load_model", "keras.models.load_model"])
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/saving/saving_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/saving/serialization_lib.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/testing/test_case.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/testing/test_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/compile_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/array_slicing.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/data_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/epoch_iterator.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/trainers/trainer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/argument_validation.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/audio_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/backend_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/code_stats.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/dataset_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/dtype_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/file_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/image_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/image_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/io_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/jax_layer.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/model_visualization.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/module_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/naming.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/numerical_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/progbar.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/python_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/rng_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/sequence_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/summary_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/text_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/tf_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/timeseries_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/torch_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/traceback_utils.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/tracking.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/src/utils/tree.py` & `keras-nightly-3.2.0.dev2024040818/keras/src/utils/tree.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/tree/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040818/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/PKG-INFO` & `keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024040803
+Version: 3.2.0.dev2024040818
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024040803/keras_nightly.egg-info/SOURCES.txt` & `keras-nightly-3.2.0.dev2024040818/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040803/setup.py` & `keras-nightly-3.2.0.dev2024040818/setup.py`

 * *Files identical despite different names*
