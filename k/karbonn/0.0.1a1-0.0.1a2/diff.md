# Comparing `tmp/karbonn-0.0.1a1.tar.gz` & `tmp/karbonn-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karbonn-0.0.1a1.tar", max compression
+gzip compressed data, was "karbonn-0.0.1a2.tar", max compression
```

## Comparing `karbonn-0.0.1a1.tar` & `karbonn-0.0.1a2.tar`

### file list

```diff
@@ -1,50 +1,69 @@
--rw-r--r--   0        0        0     1501 2024-03-30 15:29:10.227228 karbonn-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     5043 2024-03-30 15:29:10.227228 karbonn-0.0.1a1/README.md
--rw-r--r--   0        0        0     6280 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      805 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/__init__.py
--rw-r--r--   0        0        0      849 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/__init__.py
--rw-r--r--   0        0        0      208 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/activations/__init__.py
--rw-r--r--   0        0        0     1769 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/activations/math.py
--rw-r--r--   0        0        0     3019 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/error.py
--rw-r--r--   0        0        0      469 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/loss/__init__.py
--rw-r--r--   0        0        0     3338 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/loss/asinh.py
--rw-r--r--   0        0        0     2518 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/loss/general_robust.py
--rw-r--r--   0        0        0     2932 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/loss/log.py
--rw-r--r--   0        0        0     2298 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/functional/reduction.py
--rw-r--r--   0        0        0      951 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/__init__.py
--rw-r--r--   0        0        0      771 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/activations/__init__.py
--rw-r--r--   0        0        0     9196 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/activations/alpha.py
--rw-r--r--   0        0        0     7492 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/activations/math.py
--rw-r--r--   0        0        0     2103 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/activations/relu.py
--rw-r--r--   0        0        0     1400 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/activations/snake.py
--rw-r--r--   0        0        0     1294 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/clamp.py
--rw-r--r--   0        0        0     2861 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/exu.py
--rw-r--r--   0        0        0      301 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/loss/__init__.py
--rw-r--r--   0        0        0     5158 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/loss/focal.py
--rw-r--r--   0        0        0     3250 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/loss/general_robust.py
--rw-r--r--   0        0        0     1451 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/modules/residual.py
--rw-r--r--   0        0        0      344 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/testing/__init__.py
--rw-r--r--   0        0        0      727 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/testing/fixtures.py
--rw-r--r--   0        0        0     1080 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/__init__.py
--rw-r--r--   0        0        0     2164 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/device.py
--rw-r--r--   0        0        0     3182 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/factory.py
--rw-r--r--   0        0        0     2088 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/imports.py
--rw-r--r--   0        0        0     5910 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/loss.py
--rw-r--r--   0        0        0     2366 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/mode.py
--rw-r--r--   0        0        0     4059 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/params.py
--rw-r--r--   0        0        0     1745 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/__init__.py
--rw-r--r--   0        0        0     1882 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/attention.py
--rw-r--r--   0        0        0     5143 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/auto.py
--rw-r--r--   0        0        0     2619 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/base.py
--rw-r--r--   0        0        0     1893 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/conv.py
--rw-r--r--   0        0        0     1623 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/embedding.py
--rw-r--r--   0        0        0     1805 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/functional.py
--rw-r--r--   0        0        0     3430 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/linear.py
--rw-r--r--   0        0        0     2645 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/list.py
--rw-r--r--   0        0        0     3577 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/norm.py
--rw-r--r--   0        0        0     1862 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/recurrent.py
--rw-r--r--   0        0        0     2050 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/sequential.py
--rw-r--r--   0        0        0     3684 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/transformer.py
--rw-r--r--   0        0        0     1409 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/unknown.py
--rw-r--r--   0        0        0     3465 2024-03-30 15:29:10.231228 karbonn-0.0.1a1/src/karbonn/utils/size/utils.py
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 karbonn-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     5118 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/README.md
+-rw-r--r--   0        0        0     6348 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1529 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/activations/__init__.py
+-rw-r--r--   0        0        0     1769 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/activations/math.py
+-rw-r--r--   0        0        0     3018 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/error.py
+-rw-r--r--   0        0        0      998 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/loss/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/loss/asinh.py
+-rw-r--r--   0        0        0     2518 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/loss/general_robust.py
+-rw-r--r--   0        0        0     2932 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/loss/log.py
+-rw-r--r--   0        0        0     7699 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/loss/relative.py
+-rw-r--r--   0        0        0     2297 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/functional/reduction.py
+-rw-r--r--   0        0        0     1803 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/activations/__init__.py
+-rw-r--r--   0        0        0     9160 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/activations/alpha.py
+-rw-r--r--   0        0        0     7438 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/activations/math.py
+-rw-r--r--   0        0        0     2091 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/activations/relu.py
+-rw-r--r--   0        0        0     1394 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/activations/snake.py
+-rw-r--r--   0        0        0     1312 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/clamp.py
+-rw-r--r--   0        0        0     1428 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/dtype.py
+-rw-r--r--   0        0        0     2879 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/exu.py
+-rw-r--r--   0        0        0      335 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/fusion/__init__.py
+-rw-r--r--   0        0        0     3092 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/fusion/aggregation.py
+-rw-r--r--   0        0        0     1269 2024-04-09 07:10:58.421725 karbonn-0.0.1a2/src/karbonn/modules/fusion/concat.py
+-rw-r--r--   0        0        0     1212 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/__init__.py
+-rw-r--r--   0        0        0     3669 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/asinh.py
+-rw-r--r--   0        0        0     5369 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/focal.py
+-rw-r--r--   0        0        0     3108 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/general_robust.py
+-rw-r--r--   0        0        0     8216 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/indicators.py
+-rw-r--r--   0        0        0     6401 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/relative.py
+-rw-r--r--   0        0        0     1915 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/loss/transform.py
+-rw-r--r--   0        0        0     1469 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/residual.py
+-rw-r--r--   0        0        0      328 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/scalar/__init__.py
+-rw-r--r--   0        0        0     6856 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/scalar/asinh.py
+-rw-r--r--   0        0        0    14426 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/scalar/cos_sin.py
+-rw-r--r--   0        0        0     2199 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/modules/shape.py
+-rw-r--r--   0        0        0      394 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/testing/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/testing/fixtures.py
+-rw-r--r--   0        0        0     1230 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/device.py
+-rw-r--r--   0        0        0     3182 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/factory.py
+-rw-r--r--   0        0        0     3828 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/imports.py
+-rw-r--r--   0        0        0     1979 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/iterator.py
+-rw-r--r--   0        0        0     5910 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/loss.py
+-rw-r--r--   0        0        0     2366 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/mode.py
+-rw-r--r--   0        0        0     4059 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/params.py
+-rw-r--r--   0        0        0     1745 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/attention.py
+-rw-r--r--   0        0        0     5143 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/auto.py
+-rw-r--r--   0        0        0     2619 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/base.py
+-rw-r--r--   0        0        0     1893 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/conv.py
+-rw-r--r--   0        0        0     1623 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/embedding.py
+-rw-r--r--   0        0        0     1805 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/functional.py
+-rw-r--r--   0        0        0     3430 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/linear.py
+-rw-r--r--   0        0        0     2645 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/list.py
+-rw-r--r--   0        0        0     3577 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/norm.py
+-rw-r--r--   0        0        0     1862 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/recurrent.py
+-rw-r--r--   0        0        0     2050 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/sequential.py
+-rw-r--r--   0        0        0     3684 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/transformer.py
+-rw-r--r--   0        0        0     1409 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/unknown.py
+-rw-r--r--   0        0        0     3465 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/size/utils.py
+-rw-r--r--   0        0        0     4263 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/state_dict.py
+-rw-r--r--   0        0        0      637 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/summary/__init__.py
+-rw-r--r--   0        0        0    22226 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/summary/module.py
+-rw-r--r--   0        0        0     6390 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/summary/parameter.py
+-rw-r--r--   0        0        0     1318 2024-04-09 07:10:58.425725 karbonn-0.0.1a2/src/karbonn/utils/tensor.py
+-rw-r--r--   0        0        0     6439 1970-01-01 00:00:00.000000 karbonn-0.0.1a2/PKG-INFO
```

### Comparing `karbonn-0.0.1a1/LICENSE` & `karbonn-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/README.md` & `karbonn-0.0.1a2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -80,17 +80,17 @@
 pip install karbonn[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/karbonn/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `karbonn` versions and tested dependencies.
 
-| `karbonn` | `coola`      | `numpy`<sup>*</sup> | `objectory`<sup>*</sup> | `torch`       | `python`      |
-|-----------|--------------|---------------------|-------------------------|---------------|---------------|
-| `main`    | `>=0.5,<1.0` | `>=1.21,<2.0`       | `>=0.1,<1.0`            | `>=1.10,<3.0` | `>=3.9,<3.13` |
+| `karbonn` | `coola`      | `numpy`<sup>*</sup> | `objectory`<sup>*</sup> | `tabulate`<sup>*</sup> | `torch`       | `python`      |
+|-----------|--------------|---------------------|-------------------------|------------------------|---------------|---------------|
+| `main`    | `>=0.5,<1.0` | `>=1.22,<2.0`       | `>=0.1,<1.0`            | `>=0.9,<0.10`          | `>=1.10,<3.0` | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -13,23 +13,23 @@
 following command: ```shell pip install karbonn ``` To make the package as slim
 as possible, only the minimal packages required to use `karbonn` are installed.
 To include all the dependencies, you can use the following command: ```shell
 pip install karbonn[all] ``` Please check the [get started page](https://
 durandtibo.github.io/karbonn/get_started) to see how to install only some
 specific dependencies or other alternatives to install the library. The
 following is the corresponding `karbonn` versions and tested dependencies. |
-`karbonn` | `coola` | `numpy`* | `objectory`* | `torch` | `python` | |---------
---|--------------|---------------------|-------------------------|-------------
---|---------------| | `main` | `>=0.5,<1.0` | `>=1.21,<2.0` | `>=0.1,<1.0` |
-`>=1.10,<3.0` | `>=3.9,<3.13` | * indicates an optional dependency ##
-Contributing Please check the instructions in [CONTRIBUTING.md](.github/
-CONTRIBUTING.md). ## Suggestions and Communication Everyone is welcome to
-contribute to the community. If you have any questions or suggestions, you can
-submit [Github Issues](https://github.com/durandtibo/karbonn/issues). We will
-reply to you as soon as possible. Thank you very much. ## API stability :
-warning: While `karbonn` is in development stage, no API is guaranteed to be
-stable from one release to the next. In fact, it is very likely that the API
-will change multiple times before a stable 1.0.0 release. In practice, this
-means that upgrading `karbonn` to a new version will possibly break any code
-that was using the old version of `karbonn`. ## License `karbonn` is licensed
-under BSD 3-Clause "New" or "Revised" license available in [LICENSE](LICENSE)
-file.
+`karbonn` | `coola` | `numpy`* | `objectory`* | `tabulate`* | `torch` |
+`python` | |-----------|--------------|---------------------|------------------
+-------|------------------------|---------------|---------------| | `main` |
+`>=0.5,<1.0` | `>=1.22,<2.0` | `>=0.1,<1.0` | `>=0.9,<0.10` | `>=1.10,<3.0` |
+`>=3.9,<3.13` | * indicates an optional dependency ## Contributing Please check
+the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions
+and Communication Everyone is welcome to contribute to the community. If you
+have any questions or suggestions, you can submit [Github Issues](https://
+github.com/durandtibo/karbonn/issues). We will reply to you as soon as
+possible. Thank you very much. ## API stability :warning: While `karbonn` is in
+development stage, no API is guaranteed to be stable from one release to the
+next. In fact, it is very likely that the API will change multiple times before
+a stable 1.0.0 release. In practice, this means that upgrading `karbonn` to a
+new version will possibly break any code that was using the old version of
+`karbonn`. ## License `karbonn` is licensed under BSD 3-Clause "New" or
+"Revised" license available in [LICENSE](LICENSE) file.
```

### Comparing `karbonn-0.0.1a1/pyproject.toml` & `karbonn-0.0.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "karbonn"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "A library of PyTorch modules"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/karbonn"
 repository = "https://github.com/durandtibo/karbonn"
 keywords = []
 license = "BSD-3-Clause"
@@ -27,24 +27,25 @@
 
 packages = [
     { include = "karbonn", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = ">=0.5,<1.0"
+coola = ">=0.6,<1.0"
 python = ">=3.9,<3.13"
 torch = ">=1.12,<3.0"
 
 # Optional dependencies
 numpy = { version = ">=1.22,<2.0", optional = true }
 objectory = { version = ">=0.1,<1.0", optional = true }
+tabulate = { version = ">=0.9,<0.10", optional = true }
 
 [tool.poetry.extras]
-all = ["numpy", "objectory"]
+all = ["numpy", "objectory", "tabulate"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^2.0"
 mkdocs-material = "^9.5"
```

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/__init__.py` & `karbonn-0.0.1a2/src/karbonn/functional/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "asinh_mse_loss",
     "asinh_smooth_l1_loss",
     "check_loss_reduction_strategy",
     "general_robust_regression_loss",
     "log_cosh_loss",
     "msle_loss",
     "reduce_loss",
+    "relative_loss",
     "safe_exp",
     "safe_log",
     "symmetric_absolute_relative_error",
 ]
 
 from karbonn.functional.activations import safe_exp, safe_log
 from karbonn.functional.error import (
@@ -25,9 +26,10 @@
 )
 from karbonn.functional.loss import (
     asinh_mse_loss,
     asinh_smooth_l1_loss,
     general_robust_regression_loss,
     log_cosh_loss,
     msle_loss,
+    relative_loss,
 )
 from karbonn.functional.reduction import check_loss_reduction_strategy, reduce_loss
```

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/activations/math.py` & `karbonn-0.0.1a2/src/karbonn/functional/activations/math.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/error.py` & `karbonn-0.0.1a2/src/karbonn/functional/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Args:
         prediction: The tensor of predictions.
         target: The target tensor, which must have the same shape and
             data type as ``prediction``.
 
     Returns:
-         The absolute error tensor, which has the same shape and data
+        The absolute error tensor, which has the same shape and data
             type as the inputs.
 
     Example usage:
 
     ```pycon
 
     >>> import torch
```

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/loss/asinh.py` & `karbonn-0.0.1a2/src/karbonn/functional/loss/asinh.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/loss/general_robust.py` & `karbonn-0.0.1a2/src/karbonn/functional/loss/general_robust.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/loss/log.py` & `karbonn-0.0.1a2/src/karbonn/functional/loss/log.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/functional/reduction.py` & `karbonn-0.0.1a2/src/karbonn/functional/reduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,9 +77,9 @@
     """
     if reduction == "mean":
         return tensor.mean()
     if reduction == "sum":
         return tensor.sum()
     if reduction == "none":
         return tensor
-    msg = f"Incorrect reduction: {reduction}. The valid reductions are {VALID_REDUCTIONS}."
+    msg = f"Incorrect reduction: {reduction}. The valid reductions are {VALID_REDUCTIONS}"
     raise ValueError(msg)
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/__init__.py` & `karbonn-0.0.1a2/src/karbonn/modules/activations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-r"""Contains some modules."""
+r"""Contain activation modules."""
 
 from __future__ import annotations
 
 __all__ = [
     "Asinh",
-    "BinaryFocalLoss",
-    "Clamp",
-    "ExU",
+    "BaseAlphaActivation",
     "Exp",
     "ExpSin",
     "Expm1",
     "Gaussian",
-    "GeneralRobustRegressionLoss",
     "Laplacian",
     "Log",
     "Log1p",
     "MultiQuadratic",
     "Quadratic",
     "ReLUn",
-    "ResidualBlock",
     "SafeExp",
     "SafeLog",
     "Sin",
     "Sinh",
     "Snake",
     "SquaredReLU",
-    "binary_focal_loss",
 ]
 
-from karbonn.modules.activations import (
-    Asinh,
-    Exp,
-    Expm1,
+from karbonn.modules.activations.alpha import (
+    BaseAlphaActivation,
     ExpSin,
     Gaussian,
     Laplacian,
-    Log,
-    Log1p,
     MultiQuadratic,
     Quadratic,
-    ReLUn,
+)
+from karbonn.modules.activations.math import (
+    Asinh,
+    Exp,
+    Expm1,
+    Log,
+    Log1p,
     SafeExp,
     SafeLog,
     Sin,
     Sinh,
-    Snake,
-    SquaredReLU,
-)
-from karbonn.modules.clamp import Clamp
-from karbonn.modules.exu import ExU
-from karbonn.modules.loss import (
-    BinaryFocalLoss,
-    GeneralRobustRegressionLoss,
-    binary_focal_loss,
 )
-from karbonn.modules.residual import ResidualBlock
+from karbonn.modules.activations.relu import ReLUn, SquaredReLU
+from karbonn.modules.activations.snake import Snake
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/activations/alpha.py` & `karbonn-0.0.1a2/src/karbonn/modules/activations/alpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import MultiQuadratic
     >>> m = MultiQuadratic()
     >>> m
     MultiQuadratic(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000, 0.7071, 0.4472, 0.3162],
             [0.2425, 0.1961, 0.1644, 0.1414]], grad_fn=<MulBackward0>)
 
     ```
     """
 
     def __init__(self, num_parameters: int = 1, init: float = 1.0, learnable: bool = True) -> None:
@@ -91,16 +91,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import ExpSin
     >>> m = ExpSin()
     >>> m
     ExpSin(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000, 2.3198, 2.4826, 1.1516],
             [0.4692, 0.3833, 0.7562, 1.9290]], grad_fn=<ExpBackward0>)
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -135,16 +135,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Gaussian
     >>> m = Gaussian()
     >>> m
     Gaussian(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000e+00, 6.0653e-01, 1.3534e-01, 1.1109e-02],
             [3.3546e-04, 3.7267e-06, 1.5230e-08, 2.2897e-11]], grad_fn=<ExpBackward0>)
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -179,16 +179,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Laplacian
     >>> m = Laplacian()
     >>> m
     Laplacian(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000e+00, 3.6788e-01, 1.3534e-01, 4.9787e-02],
             [1.8316e-02, 6.7379e-03, 2.4788e-03, 9.1188e-04]], grad_fn=<ExpBackward0>)
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -223,16 +223,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import MultiQuadratic
     >>> m = MultiQuadratic()
     >>> m
     MultiQuadratic(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000, 0.7071, 0.4472, 0.3162],
             [0.2425, 0.1961, 0.1644, 0.1414]], grad_fn=<MulBackward0>)
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -267,16 +267,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Quadratic
     >>> m = Quadratic()
     >>> m
     Quadratic(num_parameters=1, learnable=True)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[1.0000, 0.5000, 0.2000, 0.1000],
             [0.0588, 0.0385, 0.0270, 0.0200]], grad_fn=<MulBackward0>)
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/activations/math.py` & `karbonn-0.0.1a2/src/karbonn/modules/activations/math.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Asinh
     >>> m = Asinh()
     >>> m
     Asinh()
-    >>> output = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
+    >>> out
     tensor([[-0.8814,  0.0000,  0.8814],
             [-1.4436,  1.4436,  2.0947]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -54,16 +54,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Exp
     >>> m = Exp()
     >>> m
     Exp()
-    >>> output = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
+    >>> out
     tensor([[ 0.3679,  1.0000,  2.7183],
             [ 0.1353,  7.3891, 54.5981]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -85,16 +85,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Expm1
     >>> m = Expm1()
     >>> m
     Expm1()
-    >>> output = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
+    >>> out
     tensor([[-0.6321,  0.0000,  1.7183],
             [-0.8647,  6.3891, 53.5981]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -116,16 +116,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Log
     >>> m = Log()
     >>> m
     Log()
-    >>> output = m(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
+    >>> out
     tensor([[0.0000, 0.6931, 1.0986],
             [1.3863, 1.6094, 1.7918]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -147,16 +147,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Log1p
     >>> m = Log1p()
     >>> m
     Log1p()
-    >>> output = m(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[0.0, 1.0, 2.0], [3.0, 4.0, 5.0]]))
+    >>> out
     tensor([[0.0000, 0.6931, 1.0986],
             [1.3863, 1.6094, 1.7918]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -183,16 +183,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import SafeExp
     >>> m = SafeExp()
     >>> m
     SafeExp(max=20.0)
-    >>> output = m(torch.tensor([[0.01, 0.1, 1.0], [10.0, 100.0, 1000.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[0.01, 0.1, 1.0], [10.0, 100.0, 1000.0]]))
+    >>> out
     tensor([[1.0101e+00, 1.1052e+00, 2.7183e+00],
             [2.2026e+04, 4.8517e+08, 4.8517e+08]])
 
     ```
     """
 
     def __init__(self, max: float = 20.0) -> None:  # noqa: A002
@@ -226,16 +226,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import SafeLog
     >>> m = SafeLog()
     >>> m
     SafeLog(min=1e-08)
-    >>> output = m(torch.tensor([[1e-4, 1e-5, 1e-6], [1e-8, 1e-9, 1e-10]]))
-    >>> output
+    >>> out = m(torch.tensor([[1e-4, 1e-5, 1e-6], [1e-8, 1e-9, 1e-10]]))
+    >>> out
     tensor([[ -9.2103, -11.5129, -13.8155],
             [-18.4207, -18.4207, -18.4207]])
 
     ```
     """
 
     def __init__(self, min: float = 1e-8) -> None:  # noqa: A002
@@ -261,16 +261,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Sin
     >>> m = Sin()
     >>> m
     Sin()
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[ 0.0000,  0.8415,  0.9093,  0.1411],
             [-0.7568, -0.9589, -0.2794,  0.6570]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
@@ -290,16 +290,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Sinh
     >>> m = Sinh()
     >>> m
     Sinh()
-    >>> output = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
-    >>> output
+    >>> out = m(torch.tensor([[-1.0, 0.0, 1.0], [-2.0, 2.0, 4.0]]))
+    >>> out
     tensor([[-1.1752,  0.0000,  1.1752],
             [-3.6269,  3.6269, 27.2899]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/activations/relu.py` & `karbonn-0.0.1a2/src/karbonn/modules/activations/relu.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import ReLUn
     >>> m = ReLUn(max=5)
     >>> m
     ReLUn(max=5.0)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[0., 1., 2., 3.],
             [4., 5., 5., 5.]])
 
     ```
     """
 
     def __init__(self, max: float = 1.0) -> None:  # noqa: A002
@@ -71,16 +71,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import SquaredReLU
     >>> m = SquaredReLU()
     >>> m
     SquaredReLU()
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[ 0.,  1.,  4.,  9.],
             [16., 25., 36., 49.]])
 
     ```
     """
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:  # noqa: A002
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/activations/snake.py` & `karbonn-0.0.1a2/src/karbonn/modules/activations/snake.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     ```pycon
 
     >>> import torch
     >>> from karbonn import Snake
     >>> m = Snake()
     >>> m
     Snake(frequency=1.0)
-    >>> output = m(torch.arange(8, dtype=torch.float).view(2, 4))
-    >>> output
+    >>> out = m(torch.arange(8, dtype=torch.float).view(2, 4))
+    >>> out
     tensor([[0.0000, 1.7081, 2.8268, 3.0199],
             [4.5728, 5.9195, 6.0781, 7.4316]])
 
     ```
     """
 
     def __init__(self, frequency: float = 1.0) -> None:
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/clamp.py` & `karbonn-0.0.1a2/src/karbonn/modules/clamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
     ```pycon
     >>> import torch
     >>> from karbonn import Clamp
     >>> m = Clamp(min=-1, max=2)
     >>> m
     Clamp(min=-1, max=2)
-    >>> m(torch.tensor([[-2.0, -1.0, 0.0], [1.0, 2.0, 3.0]]))
+    >>> out = m(torch.tensor([[-2.0, -1.0, 0.0], [1.0, 2.0, 3.0]]))
+    >>> out
     tensor([[-1., -1.,  0.], [ 1.,  2.,  2.]])
 
     ```
     """
 
     def __init__(self, min: float | None = -1.0, max: float | None = 1.0) -> None:  # noqa: A002
         super().__init__()
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/exu.py` & `karbonn-0.0.1a2/src/karbonn/modules/exu.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     ```pycon
     >>> import torch
     >>> from karbonn import ExU
     >>> m = ExU(4, 6)
     >>> m
     ExU(in_features=4, out_features=6, bias=True)
-    >>> m(torch.rand(6, 4))
+    >>> out = m(torch.rand(6, 4))
+    >>> out
     tensor([[...]], grad_fn=<MmBackward0>)
 
     ```
     """
 
     def __init__(
         self,
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/loss/focal.py` & `karbonn-0.0.1a2/src/karbonn/modules/loss/focal.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,18 +42,25 @@
     Example usage:
 
     ```pycon
 
     >>> import torch
     >>> from karbonn import BinaryFocalLoss
     >>> criterion = BinaryFocalLoss(nn.BCEWithLogitsLoss(reduction="none"))
+    >>> criterion
+    BinaryFocalLoss(
+      alpha=0.5, gamma=2.0, reduction=mean
+      (loss): BCEWithLogitsLoss()
+    )
     >>> input = torch.randn(3, 2, requires_grad=True)
-    >>> target = torch.rand(3, 2, requires_grad=False)
-    >>> output = criterion(input, target)
-    >>> output.backward()
+    >>> target = torch.rand(3, 2)
+    >>> loss = criterion(input, target)
+    >>> loss
+    tensor(..., grad_fn=<MeanBackward0>)
+    >>> loss.backward()
 
     ```
     """
 
     def __init__(
         self,
         loss: nn.Module | dict,
@@ -76,15 +83,15 @@
             msg = f"Incorrect parameter gamma ({gamma}). Gamma has to be positive (>=0)."
             raise ValueError(msg)
 
         check_loss_reduction_strategy(reduction)
         self.reduction = reduction
 
     def extra_repr(self) -> str:
-        return f"alpha={self._alpha}, gamma={self._gamma}"
+        return f"alpha={self._alpha}, gamma={self._gamma}, reduction={self.reduction}"
 
     def forward(self, prediction: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         r"""Compute the binary Focal Loss.
 
         Args:
             prediction: The predicted probabilities or the
                 un-normalized scores.
@@ -133,21 +140,21 @@
 
     ```pycon
 
     >>> from karbonn import binary_focal_loss
     >>> criterion = binary_focal_loss()
     >>> criterion
     BinaryFocalLoss(
-      alpha=0.5, gamma=2.0
+      alpha=0.5, gamma=2.0, reduction=mean
       (loss): BCELoss()
     )
     >>> criterion = binary_focal_loss(logits=True)
     >>> criterion
     BinaryFocalLoss(
-      alpha=0.5, gamma=2.0
+      alpha=0.5, gamma=2.0, reduction=mean
       (loss): BCEWithLogitsLoss()
     )
 
     ```
     """
     loss = nn.BCEWithLogitsLoss(reduction="none") if logits else nn.BCELoss(reduction="none")
     return BinaryFocalLoss(loss=loss, alpha=alpha, gamma=gamma, reduction=reduction)
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/loss/general_robust.py` & `karbonn-0.0.1a2/src/karbonn/modules/loss/general_robust.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,19 +52,21 @@
 
     ```pycon
 
     >>> import torch
     >>> from karbonn import GeneralRobustRegressionLoss
     >>> criterion = GeneralRobustRegressionLoss()
     >>> criterion
-    GeneralRobustRegressionLoss(alpha=2.0, scale=1.0, max=None)
+    GeneralRobustRegressionLoss(alpha=2.0, scale=1.0, max=None, reduction=mean)
     >>> input = torch.randn(3, 2, requires_grad=True)
     >>> target = torch.rand(3, 2, requires_grad=False)
-    >>> output = criterion(input, target)
-    >>> output.backward()
+    >>> loss = criterion(input, target)
+    >>> loss
+    tensor(..., grad_fn=<MeanBackward0>)
+    >>> loss.backward()
 
     ```
     """
 
     def __init__(
         self,
         alpha: float = 2.0,
@@ -80,27 +82,20 @@
         self._scale = float(scale)
         self._max = max
 
         check_loss_reduction_strategy(reduction)
         self.reduction = reduction
 
     def extra_repr(self) -> str:
-        return f"alpha={self._alpha}, scale={self._scale}, max={self._max}"
+        return (
+            f"alpha={self._alpha}, scale={self._scale}, max={self._max}, "
+            f"reduction={self.reduction}"
+        )
 
     def forward(self, prediction: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        r"""Compute the loss values and reduces them.
-
-        Args:
-            prediction: The predictions.
-            target: The target values.
-
-        Returns:
-            The loss. The shape of the tensor depends on the reduction
-                strategy.
-        """
         return general_robust_regression_loss(
             prediction=prediction,
             target=target,
             alpha=self._alpha,
             scale=self._scale,
             max=self._max,
             reduction=self.reduction,
```

### Comparing `karbonn-0.0.1a1/src/karbonn/modules/residual.py` & `karbonn-0.0.1a2/src/karbonn/modules/residual.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
       (residual): Sequential(
         (0): Linear(in_features=4, out_features=6, bias=True)
         (1): ReLU()
         (2): Linear(in_features=6, out_features=4, bias=True)
       )
       (skip): Identity()
     )
-    >>> m(torch.rand(6, 4))
+    >>> out = m(torch.rand(6, 4))
+    >>> out
     tensor([[...]], grad_fn=<AddBackward0>)
 
     ```
     """
 
     def __init__(
         self,
```

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/__init__.py` & `karbonn-0.0.1a2/src/karbonn/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 r"""Contain utility functions."""
 
 from __future__ import annotations
 
 __all__ = [
     "create_sequential",
+    "find_module_state_dict",
     "freeze_module",
     "get_module_device",
     "get_module_devices",
     "has_learnable_parameters",
     "has_parameters",
     "is_loss_decreasing",
     "is_loss_decreasing_with_adam",
     "is_loss_decreasing_with_sgd",
     "is_module_config",
     "is_module_on_device",
+    "load_state_dict_to_module",
     "module_mode",
     "num_learnable_parameters",
     "num_parameters",
     "setup_module",
     "top_module_mode",
     "unfreeze_module",
 ]
@@ -38,7 +40,8 @@
     freeze_module,
     has_learnable_parameters,
     has_parameters,
     num_learnable_parameters,
     num_parameters,
     unfreeze_module,
 )
+from karbonn.utils.state_dict import find_module_state_dict, load_state_dict_to_module
```

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/device.py` & `karbonn-0.0.1a2/src/karbonn/utils/device.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/factory.py` & `karbonn-0.0.1a2/src/karbonn/utils/factory.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/imports.py` & `karbonn-0.0.1a2/src/karbonn/utils/imports.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 r"""Implement some utility functions to manage optional dependencies."""
 
 from __future__ import annotations
 
 __all__ = [
     "check_objectory",
+    "check_tabulate",
     "is_objectory_available",
+    "is_tabulate_available",
     "objectory_available",
+    "tabulate_available",
 ]
 
 from importlib.util import find_spec
 from typing import TYPE_CHECKING, Any
 
 from coola.utils.imports import decorator_package_available
 
@@ -82,7 +85,78 @@
     ...     return 42 + n
     ...
     >>> my_function()
 
     ```
     """
     return decorator_package_available(fn, is_objectory_available)
+
+
+####################
+#     tabulate     #
+####################
+
+
+def is_tabulate_available() -> bool:
+    r"""Indicate if the ``tabulate`` package is installed or not.
+
+    Returns:
+        ``True`` if ``tabulate`` is available otherwise ``False``.
+
+    Example usage:
+
+    ```pycon
+    >>> from karbonn.utils.imports import is_tabulate_available
+    >>> is_tabulate_available()
+
+    ```
+    """
+    return find_spec("tabulate") is not None
+
+
+def check_tabulate() -> None:
+    r"""Check if the ``tabulate`` package is installed.
+
+    Raises:
+        RuntimeError: if the ``tabulate`` package is not installed.
+
+    Example usage:
+
+    ```pycon
+    >>> from karbonn.utils.imports import check_tabulate
+    >>> check_tabulate()
+
+    ```
+    """
+    if not is_tabulate_available():
+        msg = (
+            "`tabulate` package is required but not installed. "
+            "You can install `tabulate` package with the command:\n\n"
+            "pip install tabulate\n"
+        )
+        raise RuntimeError(msg)
+
+
+def tabulate_available(fn: Callable[..., Any]) -> Callable[..., Any]:
+    r"""Implement a decorator to execute a function only if ``tabulate``
+    package is installed.
+
+    Args:
+        fn: Specifies the function to execute.
+
+    Returns:
+        A wrapper around ``fn`` if ``tabulate`` package is installed,
+            otherwise ``None``.
+
+    Example usage:
+
+    ```pycon
+    >>> from karbonn.utils.imports import tabulate_available
+    >>> @tabulate_available
+    ... def my_function(n: int = 0) -> int:
+    ...     return 42 + n
+    ...
+    >>> my_function()
+
+    ```
+    """
+    return decorator_package_available(fn, is_tabulate_available)
```

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/loss.py` & `karbonn-0.0.1a2/src/karbonn/utils/loss.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/mode.py` & `karbonn-0.0.1a2/src/karbonn/utils/mode.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/params.py` & `karbonn-0.0.1a2/src/karbonn/utils/params.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/__init__.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/__init__.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/attention.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/attention.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/auto.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/auto.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/base.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/base.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/conv.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/conv.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/embedding.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/embedding.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/functional.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/functional.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/linear.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/linear.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/list.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/list.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/norm.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/norm.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/recurrent.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/recurrent.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/sequential.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/sequential.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/transformer.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/transformer.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/unknown.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/unknown.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/src/karbonn/utils/size/utils.py` & `karbonn-0.0.1a2/src/karbonn/utils/size/utils.py`

 * *Files identical despite different names*

### Comparing `karbonn-0.0.1a1/PKG-INFO` & `karbonn-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karbonn
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A library of PyTorch modules
 Home-page: https://github.com/durandtibo/karbonn
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -18,17 +18,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
-Requires-Dist: coola (>=0.5,<1.0)
+Requires-Dist: coola (>=0.6,<1.0)
 Requires-Dist: numpy (>=1.22,<2.0) ; extra == "all"
 Requires-Dist: objectory (>=0.1,<1.0) ; extra == "all"
+Requires-Dist: tabulate (>=0.9,<0.10) ; extra == "all"
 Requires-Dist: torch (>=1.12,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/karbonn
 Description-Content-Type: text/markdown
 
 # karbonn
 
 <p align="center">
@@ -111,17 +112,17 @@
 pip install karbonn[all]
 ```
 
 Please check the [get started page](https://durandtibo.github.io/karbonn/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `karbonn` versions and tested dependencies.
 
-| `karbonn` | `coola`      | `numpy`<sup>*</sup> | `objectory`<sup>*</sup> | `torch`       | `python`      |
-|-----------|--------------|---------------------|-------------------------|---------------|---------------|
-| `main`    | `>=0.5,<1.0` | `>=1.21,<2.0`       | `>=0.1,<1.0`            | `>=1.10,<3.0` | `>=3.9,<3.13` |
+| `karbonn` | `coola`      | `numpy`<sup>*</sup> | `objectory`<sup>*</sup> | `tabulate`<sup>*</sup> | `torch`       | `python`      |
+|-----------|--------------|---------------------|-------------------------|------------------------|---------------|---------------|
+| `main`    | `>=0.5,<1.0` | `>=1.22,<2.0`       | `>=0.1,<1.0`            | `>=0.9,<0.10`          | `>=1.10,<3.0` | `>=3.9,<3.13` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
 
 Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: karbonn Version: 0.0.1a1 Summary: A library of
+Metadata-Version: 2.1 Name: karbonn Version: 0.0.1a2 Summary: A library of
 PyTorch modules Home-page: https://github.com/durandtibo/karbonn License: BSD-
 3-Clause Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Software Development :: Libraries Provides-
-Extra: all Requires-Dist: coola (>=0.5,<1.0) Requires-Dist: numpy (>=1.22,<2.0)
+Extra: all Requires-Dist: coola (>=0.6,<1.0) Requires-Dist: numpy (>=1.22,<2.0)
 ; extra == "all" Requires-Dist: objectory (>=0.1,<1.0) ; extra == "all"
-Requires-Dist: torch (>=1.12,<3.0) Project-URL: Repository, https://github.com/
-durandtibo/karbonn Description-Content-Type: text/markdown # karbonn
+Requires-Dist: tabulate (>=0.9,<0.10) ; extra == "all" Requires-Dist: torch
+(>=1.12,<3.0) Project-URL: Repository, https://github.com/durandtibo/karbonn
+Description-Content-Type: text/markdown # karbonn
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_1_d_6_6_f_4_2_1_8_d_5_d_a_8_1_c_2_e_d_0_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_1_d_6_6_f_4_2_1_8_d_5_d_a_8_1_c_2_e_d_0_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
@@ -29,23 +30,23 @@
 following command: ```shell pip install karbonn ``` To make the package as slim
 as possible, only the minimal packages required to use `karbonn` are installed.
 To include all the dependencies, you can use the following command: ```shell
 pip install karbonn[all] ``` Please check the [get started page](https://
 durandtibo.github.io/karbonn/get_started) to see how to install only some
 specific dependencies or other alternatives to install the library. The
 following is the corresponding `karbonn` versions and tested dependencies. |
-`karbonn` | `coola` | `numpy`* | `objectory`* | `torch` | `python` | |---------
---|--------------|---------------------|-------------------------|-------------
---|---------------| | `main` | `>=0.5,<1.0` | `>=1.21,<2.0` | `>=0.1,<1.0` |
-`>=1.10,<3.0` | `>=3.9,<3.13` | * indicates an optional dependency ##
-Contributing Please check the instructions in [CONTRIBUTING.md](.github/
-CONTRIBUTING.md). ## Suggestions and Communication Everyone is welcome to
-contribute to the community. If you have any questions or suggestions, you can
-submit [Github Issues](https://github.com/durandtibo/karbonn/issues). We will
-reply to you as soon as possible. Thank you very much. ## API stability :
-warning: While `karbonn` is in development stage, no API is guaranteed to be
-stable from one release to the next. In fact, it is very likely that the API
-will change multiple times before a stable 1.0.0 release. In practice, this
-means that upgrading `karbonn` to a new version will possibly break any code
-that was using the old version of `karbonn`. ## License `karbonn` is licensed
-under BSD 3-Clause "New" or "Revised" license available in [LICENSE](LICENSE)
-file.
+`karbonn` | `coola` | `numpy`* | `objectory`* | `tabulate`* | `torch` |
+`python` | |-----------|--------------|---------------------|------------------
+-------|------------------------|---------------|---------------| | `main` |
+`>=0.5,<1.0` | `>=1.22,<2.0` | `>=0.1,<1.0` | `>=0.9,<0.10` | `>=1.10,<3.0` |
+`>=3.9,<3.13` | * indicates an optional dependency ## Contributing Please check
+the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions
+and Communication Everyone is welcome to contribute to the community. If you
+have any questions or suggestions, you can submit [Github Issues](https://
+github.com/durandtibo/karbonn/issues). We will reply to you as soon as
+possible. Thank you very much. ## API stability :warning: While `karbonn` is in
+development stage, no API is guaranteed to be stable from one release to the
+next. In fact, it is very likely that the API will change multiple times before
+a stable 1.0.0 release. In practice, this means that upgrading `karbonn` to a
+new version will possibly break any code that was using the old version of
+`karbonn`. ## License `karbonn` is licensed under BSD 3-Clause "New" or
+"Revised" license available in [LICENSE](LICENSE) file.
```

