# Comparing `tmp/deepdoctection-0.30.tar.gz` & `tmp/deepdoctection-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdoctection-0.30.tar", last modified: Tue Feb 20 08:57:02 2024, max compression
+gzip compressed data, was "deepdoctection-0.31.tar", last modified: Tue Apr  9 11:12:19 2024, max compression
```

## Comparing `deepdoctection-0.30.tar` & `deepdoctection-0.31.tar`

### file list

```diff
@@ -1,271 +1,272 @@
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.270275 deepdoctection-0.30/
--rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2023-10-02 16:42:43.000000 deepdoctection-0.30/LICENSE
--rw-r--r--   0 janis     (1000) janis     (1000)    18784 2024-02-20 08:57:02.270275 deepdoctection-0.30/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)    12628 2023-11-13 15:10:05.000000 deepdoctection-0.30/README.md
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/
--rw-rw-r--   0 janis     (1000) janis     (1000)    12894 2024-02-20 08:53:59.000000 deepdoctection-0.30/deepdoctection/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19017 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/analyzer/dd.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/configs/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/configs/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2227 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/configs/conf_dd_one.yaml
--rw-rw-r--   0 janis     (1000) janis     (1000)       35 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/configs/conf_tesseract.yaml
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6806 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/dataflow/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10018 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/dataflow/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6769 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/dataflow/custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20542 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/dataflow/custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15756 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/dataflow/parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4526 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/dataflow/serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9626 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/dataflow/stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20021 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/datapoint/annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23538 2024-02-06 15:06:03.000000 deepdoctection-0.30/deepdoctection/datapoint/box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6651 2023-11-23 20:59:32.000000 deepdoctection-0.30/deepdoctection/datapoint/convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    27148 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/datapoint/image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    37349 2024-02-09 16:45:53.000000 deepdoctection-0.30/deepdoctection/datapoint/view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.242275 deepdoctection-0.30/deepdoctection/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7404 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/datasets/adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18947 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/datasets/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4099 2023-11-02 17:09:26.000000 deepdoctection-0.30/deepdoctection/datasets/dataflow_builder.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    20603 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/info.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12013 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/datasets/instances/fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6622 2023-11-02 17:09:26.000000 deepdoctection-0.30/deepdoctection/datasets/instances/iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4675 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12225 2023-11-02 17:09:26.000000 deepdoctection-0.30/deepdoctection/datasets/instances/pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8554 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/datasets/instances/pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/xfund.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/datasets/instances/xsl/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/xsl/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
--rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/datasets/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3364 2023-11-13 14:54:48.000000 deepdoctection-0.30/deepdoctection/datasets/save.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19638 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/eval/accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4803 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/eval/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/eval/cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19182 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/eval/eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/eval/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9212 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/eval/tedsmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5756 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/eval/tp_eval_callback.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1194 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11989 2023-12-15 15:09:06.000000 deepdoctection-0.30/deepdoctection/extern/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18703 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/d2detect.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1866 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15015 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/extern/doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2999 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9319 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    39398 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    51436 2024-02-09 16:47:05.000000 deepdoctection-0.30/deepdoctection/extern/model.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3692 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/pdftext.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/extern/pt/
--rw-rw-r--   0 janis     (1000) janis     (1000)      771 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/pt/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1458 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/pt/nms.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1372 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/pt/ptutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12292 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5700 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/extern/texocr.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/extern/tp/
--rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tfutils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5054 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpcompat.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3711 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/common.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.246275 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/config/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/config/config.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.250275 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9512 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13620 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11108 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17832 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4644 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4216 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/predict.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11947 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/preproc.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.250275 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7525 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/extern/tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.250275 deepdoctection-0.30/deepdoctection/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1294 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15922 2023-11-24 15:56:27.000000 deepdoctection-0.30/deepdoctection/mapper/cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5840 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8422 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5428 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35348 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7896 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/mapper/maputils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7780 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/match.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/mapper/misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/mapper/pascalstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6822 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/mapper/prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23567 2023-11-01 17:14:31.000000 deepdoctection-0.30/deepdoctection/mapper/pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4504 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/mapper/tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8807 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/mapper/xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.250275 deepdoctection-0.30/deepdoctection/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14111 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/pipe/anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    13182 2023-12-17 18:38:12.000000 deepdoctection-0.30/deepdoctection/pipe/base.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    11062 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    14378 2023-12-17 18:38:12.000000 deepdoctection-0.30/deepdoctection/pipe/common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9531 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9007 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/pipe/doctectionpipe.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5579 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5262 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    18031 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    35266 2024-02-16 09:43:48.000000 deepdoctection-0.30/deepdoctection/pipe/order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    22439 2023-11-13 09:03:06.000000 deepdoctection-0.30/deepdoctection/pipe/refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      902 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    50474 2024-02-06 15:21:33.000000 deepdoctection-0.30/deepdoctection/pipe/segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10985 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/pipe/text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3193 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/pipe/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/py.typed
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.250275 deepdoctection-0.30/deepdoctection/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15740 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/train/d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10610 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/train/hf_detr_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    21335 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/train/hf_layoutlm_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12952 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/train/tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/deepdoctection/utils/
--rw-rw-r--   0 janis     (1000) janis     (1000)     2299 2023-11-02 17:09:26.000000 deepdoctection-0.30/deepdoctection/utils/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4583 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/utils/concurrency.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4060 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/utils/context.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2024-01-03 11:33:54.000000 deepdoctection-0.30/deepdoctection/utils/detection_types.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3470 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/utils/develop.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17620 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/utils/env_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19248 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/utils/file_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9094 2023-12-30 11:21:01.000000 deepdoctection-0.30/deepdoctection/utils/fs.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/utils/identifier.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9931 2024-01-20 15:59:58.000000 deepdoctection-0.30/deepdoctection/utils/logger.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/utils/metacfg.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7693 2023-12-31 14:32:27.000000 deepdoctection-0.30/deepdoctection/utils/pdf_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12188 2023-11-01 17:14:31.000000 deepdoctection-0.30/deepdoctection/utils/settings.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1830 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/utils/tqdm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8379 2023-10-02 16:42:43.000000 deepdoctection-0.30/deepdoctection/utils/transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5323 2023-12-14 12:05:31.000000 deepdoctection-0.30/deepdoctection/utils/utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    23693 2024-02-20 08:48:22.000000 deepdoctection-0.30/deepdoctection/utils/viz.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/deepdoctection.egg-info/
--rw-r--r--   0 janis     (1000) janis     (1000)    18784 2024-02-20 08:57:02.000000 deepdoctection-0.30/deepdoctection.egg-info/PKG-INFO
--rw-rw-r--   0 janis     (1000) janis     (1000)     7990 2024-02-20 08:57:02.000000 deepdoctection-0.30/deepdoctection.egg-info/SOURCES.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)        1 2024-02-20 08:57:02.000000 deepdoctection-0.30/deepdoctection.egg-info/dependency_links.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     1814 2024-02-20 08:57:02.000000 deepdoctection-0.30/deepdoctection.egg-info/requires.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)       15 2024-02-20 08:57:02.000000 deepdoctection-0.30/deepdoctection.egg-info/top_level.txt
--rw-rw-r--   0 janis     (1000) janis     (1000)     2270 2024-02-20 08:57:02.270275 deepdoctection-0.30/setup.cfg
--rw-rw-r--   0 janis     (1000) janis     (1000)     6972 2024-02-20 08:55:35.000000 deepdoctection-0.30/setup.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/
--rw-rw-r--   0 janis     (1000) janis     (1000)      725 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/analyzer/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/analyzer/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    28969 2024-01-25 17:25:48.000000 deepdoctection-0.30/tests/analyzer/test_dd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    17385 2023-11-13 09:03:06.000000 deepdoctection-0.30/tests/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    64799 2023-12-17 18:38:12.000000 deepdoctection-0.30/tests/data.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/dataflow/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/test_custom.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/test_custom_serialize.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/test_parallel_map.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/dataflow/test_stats.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/datapoint/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datapoint/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datapoint/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5857 2023-11-13 09:03:06.000000 deepdoctection-0.30/tests/datapoint/test_annotation.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datapoint/test_box.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datapoint/test_convert.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12138 2023-11-13 09:03:06.000000 deepdoctection-0.30/tests/datapoint/test_image.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4782 2023-12-17 18:38:12.000000 deepdoctection-0.30/tests/datapoint/test_view.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/datasets/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/__init__.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/datasets/instances/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)      974 2024-01-20 15:59:58.000000 deepdoctection-0.30/tests/datasets/instances/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_doclaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_fintabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2090 2023-12-17 18:38:12.000000 deepdoctection-0.30/tests/datasets/instances/test_funsd.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1268 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_layouttest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_publaynet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_pubtables1m.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_pubtabnet.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/instances/test_rvlcdip.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2782 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/test_adapter.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     8598 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/test_info.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/datasets/test_registry.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.254275 deepdoctection-0.30/tests/eval/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/test_accmetric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3818 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/test_cocometric.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2933 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/test_eval.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1258 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/eval/test_tedsmetric.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/tests/extern/
--rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2393 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5426 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1645 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_deskew.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4956 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_doctrocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2135 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_fastlang.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3777 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_hfdetr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    19412 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_hflayoutlm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2052 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_pdftext.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3438 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_tessocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1621 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_texocr.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4360 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/extern/test_tpdetect.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/tests/mapper/
--rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    81517 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/data.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_cats.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_cocostruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1903 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_d2struct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2046 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_hfstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2381 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_iiitar13k.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     5552 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_laylmstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_misc.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2894 2024-01-20 15:59:58.000000 deepdoctection-0.30/tests/mapper/test_prodigystruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_pubstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_tpstruct.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_utils.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/mapper/test_xfundstruct.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/tests/pipe/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     6252 2023-11-13 09:03:06.000000 deepdoctection-0.30/tests/pipe/test_anngen.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4480 2023-11-13 09:03:06.000000 deepdoctection-0.30/tests/pipe/test_cell.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3445 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_common.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_language.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1955 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_layout.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     4596 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_lm.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_order.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     9646 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_refine.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_registry.py
--rw-rw-r--   0 janis     (1000) janis     (1000)    15618 2023-12-30 11:21:01.000000 deepdoctection-0.30/tests/pipe/test_segment.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     7729 2023-11-13 14:54:48.000000 deepdoctection-0.30/tests/pipe/test_text.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1892 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/pipe/test_transform.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     2244 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/test_utils.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/tests/train/
--rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/train/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/train/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/train/test_d2_frcnn_train.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3532 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests/train/test_tp_frcnn_train.py
-drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-02-20 08:57:02.258275 deepdoctection-0.30/tests_d2/
--rw-rw-r--   0 janis     (1000) janis     (1000)      761 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests_d2/__init__.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     1554 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests_d2/conftest.py
--rw-rw-r--   0 janis     (1000) janis     (1000)     3220 2023-10-02 16:42:43.000000 deepdoctection-0.30/tests_d2/test_d2detect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.681617 deepdoctection-0.31/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11351 2023-10-02 16:42:43.000000 deepdoctection-0.31/LICENSE
+-rw-r--r--   0 janis     (1000) janis     (1000)    17927 2024-04-09 11:12:19.681617 deepdoctection-0.31/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12780 2024-04-09 11:09:39.000000 deepdoctection-0.31/README.md
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12960 2024-04-09 11:10:50.000000 deepdoctection-0.31/deepdoctection/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19057 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/analyzer/dd.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/configs/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/configs/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2227 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/configs/conf_dd_one.yaml
+-rw-rw-r--   0 janis     (1000) janis     (1000)       35 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/configs/conf_tesseract.yaml
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      845 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6221 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10018 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/dataflow/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6809 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20851 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15843 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4568 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/dataflow/serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9626 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/dataflow/stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.657617 deepdoctection-0.31/deepdoctection/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1643 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21017 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23489 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datapoint/box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6716 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datapoint/convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    28754 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    39112 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datapoint/view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1154 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7406 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22274 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/datasets/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4101 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/dataflow_builder.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    20601 2024-03-25 16:11:04.000000 deepdoctection-0.31/deepdoctection/datasets/info.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1388 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12014 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12013 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/datasets/instances/fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6938 2024-02-29 11:20:47.000000 deepdoctection-0.31/deepdoctection/datasets/instances/funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6622 2023-11-02 17:09:26.000000 deepdoctection-0.31/deepdoctection/datasets/instances/iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4367 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/datasets/instances/layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5193 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12225 2023-11-02 17:09:26.000000 deepdoctection-0.31/deepdoctection/datasets/instances/pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8554 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/datasets/instances/pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6608 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7715 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xfund.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1952 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/instances/xsl/pascal_voc.xsl
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2543 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/datasets/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3364 2023-11-13 14:54:48.000000 deepdoctection-0.31/deepdoctection/datasets/save.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1006 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19639 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4855 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8755 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19186 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1051 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/eval/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9212 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/eval/tedsmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5795 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/eval/tp_eval_callback.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1194 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12786 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23071 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/d2detect.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2932 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    24606 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4350 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11582 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    42706 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    51436 2024-02-09 16:47:05.000000 deepdoctection-0.31/deepdoctection/extern/model.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3736 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/pdftext.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/pt/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      771 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/pt/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1458 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/pt/nms.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1407 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/extern/pt/ptutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17143 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/extern/tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5745 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/texocr.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      706 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1479 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tfutils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5068 2024-03-15 09:27:28.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpcompat.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3711 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/common.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.661617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11284 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/config.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9512 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13620 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7061 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5685 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11108 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17832 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4644 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4216 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/predict.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11898 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/preproc.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2203 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3539 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8780 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/extern/tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1294 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15922 2023-11-24 15:56:27.000000 deepdoctection-0.31/deepdoctection/mapper/cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5840 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/mapper/cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8473 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5479 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    35347 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8149 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/maputils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7780 2023-11-13 09:03:06.000000 deepdoctection-0.31/deepdoctection/mapper/match.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6520 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3844 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/mapper/pascalstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6804 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    23588 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4506 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/mapper/tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8807 2024-02-20 15:30:45.000000 deepdoctection-0.31/deepdoctection/mapper/xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1121 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15198 2024-04-08 14:21:56.000000 deepdoctection-0.31/deepdoctection/pipe/anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14618 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/base.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12149 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    14782 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9531 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8986 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/doctectionpipe.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5612 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5298 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18029 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    35266 2024-03-15 09:27:06.000000 deepdoctection-0.31/deepdoctection/pipe/order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    22921 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/pipe/refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      902 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/pipe/registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    50631 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    11168 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/pipe/text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3736 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/pipe/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/py.typed
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.665617 deepdoctection-0.31/deepdoctection/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1196 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15856 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10717 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/hf_detr_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    21695 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/train/hf_layoutlm_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12952 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/train/tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/deepdoctection/utils/
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2371 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4608 2024-03-15 09:27:28.000000 deepdoctection-0.31/deepdoctection/utils/concurrency.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4076 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/context.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2024-02-28 10:19:33.000000 deepdoctection-0.31/deepdoctection/utils/detection_types.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3470 2023-12-30 11:21:01.000000 deepdoctection-0.31/deepdoctection/utils/develop.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    18629 2024-04-08 13:16:57.000000 deepdoctection-0.31/deepdoctection/utils/env_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2367 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/error.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19089 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/file_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9142 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/fs.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2159 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/identifier.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9931 2024-01-20 15:59:58.000000 deepdoctection-0.31/deepdoctection/utils/logger.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5203 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/metacfg.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7711 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/pdf_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12290 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/settings.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1830 2023-10-02 16:42:43.000000 deepdoctection-0.31/deepdoctection/utils/tqdm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8381 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5185 2024-03-03 12:42:06.000000 deepdoctection-0.31/deepdoctection/utils/utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    25468 2024-04-08 10:00:25.000000 deepdoctection-0.31/deepdoctection/utils/viz.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.677617 deepdoctection-0.31/deepdoctection.egg-info/
+-rw-r--r--   0 janis     (1000) janis     (1000)    17927 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/PKG-INFO
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8020 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/SOURCES.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)        1 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/dependency_links.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1598 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/requires.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)       15 2024-04-09 11:12:19.000000 deepdoctection-0.31/deepdoctection.egg-info/top_level.txt
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2270 2024-04-09 11:12:19.685617 deepdoctection-0.31/setup.cfg
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7076 2024-04-09 11:12:14.000000 deepdoctection-0.31/setup.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      725 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/analyzer/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/analyzer/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    28969 2024-01-25 17:25:48.000000 deepdoctection-0.31/tests/analyzer/test_dd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    17384 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    67349 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/data.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/dataflow/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2342 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5389 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1632 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_custom.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4274 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_custom_serialize.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_parallel_map.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2836 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/dataflow/test_stats.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datapoint/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7468 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5857 2023-11-13 09:03:06.000000 deepdoctection-0.31/tests/datapoint/test_annotation.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12861 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/test_box.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1534 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datapoint/test_convert.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    13809 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/datapoint/test_image.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4782 2023-12-17 18:38:12.000000 deepdoctection-0.31/tests/datapoint/test_view.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datasets/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/__init__.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.669617 deepdoctection-0.31/tests/datasets/instances/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)      974 2024-01-20 15:59:58.000000 deepdoctection-0.31/tests/datasets/instances/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1285 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_doclaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2514 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_fintabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2146 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/datasets/instances/test_funsd.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1268 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1911 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_layouttest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1922 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_publaynet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1931 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_pubtables1m.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1924 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_pubtabnet.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1464 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/instances/test_rvlcdip.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2782 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/test_adapter.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     8597 2024-03-03 12:42:06.000000 deepdoctection-0.31/tests/datasets/test_info.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2153 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/datasets/test_registry.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/eval/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3244 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    12696 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_accmetric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3818 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_cocometric.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2933 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_eval.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2418 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1258 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/eval/test_tedsmetric.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/extern/
+-rw-rw-r--   0 janis     (1000) janis     (1000)        0 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2672 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5482 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1977 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/extern/test_deskew.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6244 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/test_doctrocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2135 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_fastlang.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3777 2024-03-15 09:27:28.000000 deepdoctection-0.31/tests/extern/test_hfdetr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    19412 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_hflayoutlm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2052 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_pdftext.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4993 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/extern/test_tessocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1621 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_texocr.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4360 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/extern/test_tpdetect.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/mapper/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7056 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    81526 2024-04-09 11:09:39.000000 deepdoctection-0.31/tests/mapper/data.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    10518 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_cats.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3621 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_cocostruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1903 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_d2struct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2046 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_hfstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2381 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_iiitar13k.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5552 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_laylmstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_misc.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2894 2024-01-20 15:59:58.000000 deepdoctection-0.31/tests/mapper/test_prodigystruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6679 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_pubstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1827 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_tpstruct.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2611 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_utils.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2555 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/mapper/test_xfundstruct.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/pipe/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     6536 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_anngen.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     5313 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_cell.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3445 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_common.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2676 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_language.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2009 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_layout.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     4596 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_lm.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7862 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_order.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     9646 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_refine.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1784 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/pipe/test_registry.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)    15618 2023-12-30 11:21:01.000000 deepdoctection-0.31/tests/pipe/test_segment.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     7959 2024-04-08 13:16:57.000000 deepdoctection-0.31/tests/pipe/test_text.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2036 2024-04-08 10:00:25.000000 deepdoctection-0.31/tests/pipe/test_transform.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     2244 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/test_utils.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.673617 deepdoctection-0.31/tests/train/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      641 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3239 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1854 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/test_d2_frcnn_train.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3532 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests/train/test_tp_frcnn_train.py
+drwxrwxr-x   0 janis     (1000) janis     (1000)        0 2024-04-09 11:12:19.677617 deepdoctection-0.31/tests_d2/
+-rw-rw-r--   0 janis     (1000) janis     (1000)      761 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests_d2/__init__.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     1554 2023-10-02 16:42:43.000000 deepdoctection-0.31/tests_d2/conftest.py
+-rw-rw-r--   0 janis     (1000) janis     (1000)     3221 2024-03-15 09:27:28.000000 deepdoctection-0.31/tests_d2/test_d2detect.py
```

### Comparing `deepdoctection-0.30/LICENSE` & `deepdoctection-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/PKG-INFO` & `deepdoctection-0.31/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.30
+Version: 0.31
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -13,143 +13,116 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: catalogue==2.0.7
+Requires-Dist: catalogue==2.0.10
 Requires-Dist: huggingface_hub>=0.12.0
-Requires-Dist: importlib-metadata>=4.11.2
+Requires-Dist: importlib-metadata>=5.0.0
 Requires-Dist: jsonlines==3.1.0
 Requires-Dist: mock==4.0.3
 Requires-Dist: networkx>=2.7.1
 Requires-Dist: numpy>=1.21
 Requires-Dist: packaging>=20.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pypdf>=3.16.0
-Requires-Dist: pyyaml==6.0
+Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: pyzmq>=16
 Requires-Dist: termcolor>=1.1
 Requires-Dist: tabulate>=0.7.7
 Requires-Dist: tqdm==4.64.0
 Provides-Extra: tf
-Requires-Dist: catalogue==2.0.7; extra == "tf"
+Requires-Dist: catalogue==2.0.10; extra == "tf"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "tf"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "tf"
+Requires-Dist: importlib-metadata>=5.0.0; extra == "tf"
 Requires-Dist: jsonlines==3.1.0; extra == "tf"
 Requires-Dist: mock==4.0.3; extra == "tf"
 Requires-Dist: networkx>=2.7.1; extra == "tf"
 Requires-Dist: numpy>=1.21; extra == "tf"
 Requires-Dist: packaging>=20.0; extra == "tf"
 Requires-Dist: Pillow>=10.0.0; extra == "tf"
 Requires-Dist: pypdf>=3.16.0; extra == "tf"
-Requires-Dist: pyyaml==6.0; extra == "tf"
+Requires-Dist: pyyaml>=6.0.1; extra == "tf"
 Requires-Dist: pyzmq>=16; extra == "tf"
 Requires-Dist: termcolor>=1.1; extra == "tf"
 Requires-Dist: tabulate>=0.7.7; extra == "tf"
 Requires-Dist: tqdm==4.64.0; extra == "tf"
-Requires-Dist: tensorpack; extra == "tf"
+Requires-Dist: tensorpack==0.11; extra == "tf"
 Requires-Dist: protobuf==3.20.1; extra == "tf"
 Requires-Dist: tensorflow-addons>=0.17.1; extra == "tf"
 Requires-Dist: tf2onnx>=1.9.2; extra == "tf"
 Requires-Dist: python-doctr==0.7.0; extra == "tf"
 Requires-Dist: pycocotools>=2.0.2; extra == "tf"
 Requires-Dist: boto3; extra == "tf"
 Requires-Dist: pdfplumber>=0.7.1; extra == "tf"
-Requires-Dist: fasttext; extra == "tf"
-Requires-Dist: jdeskew; extra == "tf"
+Requires-Dist: fasttext==0.9.2; extra == "tf"
+Requires-Dist: jdeskew>=0.2.2; extra == "tf"
 Requires-Dist: apted==1.0.3; extra == "tf"
 Requires-Dist: distance==0.1.3; extra == "tf"
 Requires-Dist: lxml>=4.9.1; extra == "tf"
 Provides-Extra: pt
-Requires-Dist: catalogue==2.0.7; extra == "pt"
+Requires-Dist: catalogue==2.0.10; extra == "pt"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "pt"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "pt"
+Requires-Dist: importlib-metadata>=5.0.0; extra == "pt"
 Requires-Dist: jsonlines==3.1.0; extra == "pt"
 Requires-Dist: mock==4.0.3; extra == "pt"
 Requires-Dist: networkx>=2.7.1; extra == "pt"
 Requires-Dist: numpy>=1.21; extra == "pt"
 Requires-Dist: packaging>=20.0; extra == "pt"
 Requires-Dist: Pillow>=10.0.0; extra == "pt"
 Requires-Dist: pypdf>=3.16.0; extra == "pt"
-Requires-Dist: pyyaml==6.0; extra == "pt"
+Requires-Dist: pyyaml>=6.0.1; extra == "pt"
 Requires-Dist: pyzmq>=16; extra == "pt"
 Requires-Dist: termcolor>=1.1; extra == "pt"
 Requires-Dist: tabulate>=0.7.7; extra == "pt"
 Requires-Dist: tqdm==4.64.0; extra == "pt"
-Requires-Dist: timm; extra == "pt"
+Requires-Dist: timm>=0.9.16; extra == "pt"
 Requires-Dist: transformers>=4.36.0; extra == "pt"
-Requires-Dist: accelerate; extra == "pt"
+Requires-Dist: accelerate>=0.29.1; extra == "pt"
 Requires-Dist: python-doctr==0.7.0; extra == "pt"
 Requires-Dist: boto3; extra == "pt"
 Requires-Dist: pdfplumber>=0.7.1; extra == "pt"
-Requires-Dist: fasttext; extra == "pt"
-Requires-Dist: jdeskew; extra == "pt"
+Requires-Dist: fasttext==0.9.2; extra == "pt"
+Requires-Dist: jdeskew>=0.2.2; extra == "pt"
 Requires-Dist: apted==1.0.3; extra == "pt"
 Requires-Dist: distance==0.1.3; extra == "pt"
 Requires-Dist: lxml>=4.9.1; extra == "pt"
 Provides-Extra: docs
-Requires-Dist: tensorpack; extra == "docs"
+Requires-Dist: tensorpack==0.11; extra == "docs"
 Requires-Dist: boto3; extra == "docs"
 Requires-Dist: transformers>=4.36.0; extra == "docs"
-Requires-Dist: accelerate; extra == "docs"
+Requires-Dist: accelerate>=0.29.1; extra == "docs"
 Requires-Dist: pdfplumber>=0.7.1; extra == "docs"
 Requires-Dist: lxml>=4.9.1; extra == "docs"
-Requires-Dist: lxml-stubs; extra == "docs"
-Requires-Dist: jdeskew; extra == "docs"
+Requires-Dist: lxml-stubs>=0.5.1; extra == "docs"
+Requires-Dist: jdeskew>=0.2.2; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: griffe==0.25.0; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: python-dotenv==1.0.0; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: black==23.7.0; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pylint==2.17.4; extra == "dev"
 Requires-Dist: mypy==1.4.1; extra == "dev"
 Requires-Dist: wandb; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
-Requires-Dist: types-termcolor==1.1.3; extra == "dev"
-Requires-Dist: types-tabulate; extra == "dev"
-Requires-Dist: types-tqdm; extra == "dev"
-Requires-Dist: lxml-stubs; extra == "dev"
-Requires-Dist: types-Pillow; extra == "dev"
-Requires-Dist: types-urllib3; extra == "dev"
+Requires-Dist: types-PyYAML>=6.0.12.12; extra == "dev"
+Requires-Dist: types-termcolor>=1.1.3; extra == "dev"
+Requires-Dist: types-tabulate>=0.9.0.3; extra == "dev"
+Requires-Dist: types-tqdm>=4.66.0.5; extra == "dev"
+Requires-Dist: lxml-stubs>=0.5.1; extra == "dev"
+Requires-Dist: types-Pillow>=10.2.0.20240406; extra == "dev"
+Requires-Dist: types-urllib3>=1.26.25.14; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest==8.0.2; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: hf
-Requires-Dist: catalogue==2.0.7; extra == "hf"
-Requires-Dist: huggingface_hub>=0.12.0; extra == "hf"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "hf"
-Requires-Dist: jsonlines==3.1.0; extra == "hf"
-Requires-Dist: mock==4.0.3; extra == "hf"
-Requires-Dist: networkx>=2.7.1; extra == "hf"
-Requires-Dist: numpy>=1.21; extra == "hf"
-Requires-Dist: packaging>=20.0; extra == "hf"
-Requires-Dist: Pillow>=10.0.0; extra == "hf"
-Requires-Dist: pypdf>=3.16.0; extra == "hf"
-Requires-Dist: pyyaml==6.0; extra == "hf"
-Requires-Dist: pyzmq>=16; extra == "hf"
-Requires-Dist: termcolor>=1.1; extra == "hf"
-Requires-Dist: tabulate>=0.7.7; extra == "hf"
-Requires-Dist: tqdm==4.64.0; extra == "hf"
-Requires-Dist: timm; extra == "hf"
-Requires-Dist: transformers>=4.36.0; extra == "hf"
-Requires-Dist: accelerate; extra == "hf"
-Requires-Dist: python-doctr==0.7.0; extra == "hf"
-Requires-Dist: boto3; extra == "hf"
-Requires-Dist: pdfplumber>=0.7.1; extra == "hf"
-Requires-Dist: fasttext; extra == "hf"
-Requires-Dist: jdeskew; extra == "hf"
-Requires-Dist: apted==1.0.3; extra == "hf"
-Requires-Dist: distance==0.1.3; extra == "hf"
-Requires-Dist: lxml>=4.9.1; extra == "hf"
 
 
 <p align="center">
   <img src="https://github.com/deepdoctection/deepdoctection/raw/master/docs/tutorials/_imgs/dd_logo.png" alt="Deep Doctection Logo" width="60%">
   <h3 align="center">
   A Document AI Package
   </h3>
@@ -187,15 +160,17 @@
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
  - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference. 
+   not required anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+   (not contained in the built-in Analyzer).
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.30/README.md` & `deepdoctection-0.31/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,17 @@
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
  - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference. 
+   not required anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+   (not contained in the built-in Analyzer).
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.30/deepdoctection/__init__.py` & `deepdoctection-0.31/deepdoctection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from .utils.env_info import auto_select_lib_and_device
 from .utils.file_utils import _LazyModule, get_tf_version, pytorch_available, tf_available
 from .utils.logger import logger
 
 # pylint: enable=wrong-import-position
 
-__version__ = 0.30
+__version__ = 0.31
 
 _IMPORT_STRUCTURE = {
     "analyzer": [
         "maybe_copy_config_to_cache",
         "config_sanity_checks",
         "build_detector",
         "build_padder",
@@ -175,14 +175,15 @@
         "ImageTransformer",
         "InferenceResize",
         "D2FrcnnDetector",
         "D2FrcnnTracingDetector",
         "Jdeskewer",
         "DoctrTextlineDetector",
         "DoctrTextRecognizer",
+        "DocTrRotationTransformer",
         "FasttextLangDetector",
         "HFDetrDerivedDetector",
         "HFLayoutLmTokenClassifierBase",
         "HFLayoutLmTokenClassifier",
         "HFLayoutLmv2TokenClassifier",
         "HFLayoutLmv3TokenClassifier",
         "HFLayoutLmSequenceClassifier",
@@ -190,14 +191,15 @@
         "HFLayoutLmv3SequenceClassifier",
         "ModelProfile",
         "ModelCatalog",
         "print_model_infos",
         "ModelDownloadManager",
         "PdfPlumberTextDetector",
         "TesseractOcrDetector",
+        "TesseractRotationTransformer",
         "TextractOcrDetector",
         "TPFrcnnDetector",
     ],
     "extern.pt": ["set_torch_auto_device", "get_num_gpu", "batched_nms"],
     "extern.tp": ["disable_tfv2", "ModelDescWithConfig", "TensorpackPredictor"],
     "extern.tp.tpfrcnn": ["CustomResize", "anchors_and_labels", "augment"],
     "extern.tp.tpfrcnn.utils": ["area", "pairwise_intersection", "pairwise_iou"],
@@ -275,15 +277,15 @@
         "TableSegmentationRefinementService",
         "generate_html_string",
         "pipeline_component_registry",
         "TableSegmentationService",
         "PubtablesSegmentationService",
         "SegmentationResult",
         "TextExtractionService",
-        "SimpleTransformPipelineComponent",
+        "SimpleTransformService",
     ],
     "train": [
         "D2Trainer",
         "train_d2_faster_rcnn",
         "LayoutLMTrainer",
         "train_hf_layoutlm",
         "train_faster_rcnn",
```

### Comparing `deepdoctection-0.30/deepdoctection/analyzer/__init__.py` & `deepdoctection-0.31/deepdoctection/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/analyzer/dd.py` & `deepdoctection-0.31/deepdoctection/analyzer/dd.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,20 @@
     return absolute_path
 
 
 def config_sanity_checks(cfg: AttrDict) -> None:
     """Some config sanity checks"""
     if cfg.USE_PDF_MINER and cfg.USE_OCR and cfg.OCR.USE_DOCTR:
         raise ValueError("Configuration USE_PDF_MINER= True and USE_OCR=True and USE_DOCTR=True is not allowed")
-    if cfg.OCR.USE_TESSERACT + cfg.OCR.USE_DOCTR + cfg.OCR.USE_TEXTRACT != 1:
-        raise ValueError(
-            "Choose either OCR.USE_TESSERACT=True or OCR.USE_DOCTR=True or OCR.USE_TEXTRACT=True and set the other two "
-            "to False. Only one OCR system can be activated."
-        )
+    if cfg.USE_OCR:
+        if cfg.OCR.USE_TESSERACT + cfg.OCR.USE_DOCTR + cfg.OCR.USE_TEXTRACT != 1:
+            raise ValueError(
+                "Choose either OCR.USE_TESSERACT=True or OCR.USE_DOCTR=True or OCR.USE_TEXTRACT=True "
+                "and set the other two to False. Only one OCR system can be activated."
+            )
 
 
 def build_detector(
     cfg: AttrDict, mode: str
 ) -> Union["D2FrcnnDetector", "TPFrcnnDetector", "HFDetrDerivedDetector", "D2FrcnnTracingDetector"]:
     """Building a D2-Detector, a TP-Detector as Detr-Detector or a D2-Torch Tracing Detector according to
     the config
```

### Comparing `deepdoctection-0.30/deepdoctection/configs/__init__.py` & `deepdoctection-0.31/deepdoctection/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/configs/conf_dd_one.yaml` & `deepdoctection-0.31/deepdoctection/configs/conf_dd_one.yaml`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/__init__.py` & `deepdoctection-0.31/deepdoctection/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/base.py` & `deepdoctection-0.31/deepdoctection/dataflow/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,14 @@
 import threading
 from abc import ABC, abstractmethod
 from typing import Any, Iterator, no_type_check
 
 from ..utils.utils import get_rng
 
 
-class DataFlowTerminated(BaseException):
-    """
-    An exception indicating that the DataFlow is unable to produce any more
-    data, i.e. something wrong happened so that calling `__iter__`
-    cannot give a valid iterator anymore.
-    In most DataFlow this will never be raised.
-    """
-
-
-class DataFlowResetStateNotCalled(BaseException):
-    """
-    An exception indicating that `reset_state()` has not been called before starting
-    iteration.
-    """
-
-    def __init__(self) -> None:
-        super().__init__("Iterating a dataflow requires .reset_state() to be called first")
-
-
 class DataFlowReentrantGuard:
     """
     A tool to enforce non-reentrancy.
     Mostly used on DataFlow whose `get_data` is stateful,
     so that multiple instances of the iterator cannot co-exist.
     """
```

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/common.py` & `deepdoctection-0.31/deepdoctection/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/custom.py` & `deepdoctection-0.31/deepdoctection/dataflow/custom.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
 <https://github.com/tensorpack/dataflow/blob/master/dataflow/dataflow/common.py>
 """
 from typing import Any, Callable, Iterable, Iterator, List, Optional
 
 import numpy as np
 
+from ..utils.error import DataFlowResetStateNotCalledError
 from ..utils.logger import LoggingRecord, logger
 from ..utils.tqdm import get_tqdm
 from ..utils.utils import get_rng
-from .base import DataFlow, DataFlowReentrantGuard, DataFlowResetStateNotCalled, ProxyDataFlow
+from .base import DataFlow, DataFlowReentrantGuard, ProxyDataFlow
 from .serialize import DataFromIterable, DataFromList
 
 __all__ = ["CacheData", "CustomDataFromList", "CustomDataFromIterable"]
 
 
 class CacheData(ProxyDataFlow):
     """
@@ -61,15 +62,15 @@
     def reset_state(self) -> None:
         super().reset_state()
         self._guard = DataFlowReentrantGuard()
         self.buffer = []
 
     def __iter__(self) -> Iterator[Any]:
         if self._guard is None:
-            raise DataFlowResetStateNotCalled()
+            raise DataFlowResetStateNotCalledError()
 
         with self._guard:
             if self.buffer:
                 if self.shuffle:
                     self.rng.shuffle(self.buffer)
                 yield from self.buffer
             else:
@@ -135,15 +136,15 @@
     def __len__(self) -> int:
         if self.max_datapoints is not None:
             return min(self.max_datapoints, len(self.lst))
         return len(self.lst)
 
     def __iter__(self) -> Iterator[Any]:
         if self.rng is None:
-            raise DataFlowResetStateNotCalled()
+            raise DataFlowResetStateNotCalledError()
         if self.rebalance_func is not None:
             lst_tmp = self.rebalance_func(self.lst)
             logger.info(LoggingRecord(f"CustomDataFromList: subset size after re-balancing: {len(lst_tmp)}"))
         else:
             lst_tmp = self.lst
 
         if self.shuffle:
```

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/custom_serialize.py` & `deepdoctection-0.31/deepdoctection/dataflow/custom_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 import json
 import os
 from collections import defaultdict
 from pathlib import Path
 from typing import DefaultDict, Dict, List, Optional, Sequence, Union
 
 from jsonlines import Reader, Writer
+from tabulate import tabulate
+from termcolor import colored
 
 from ..utils.context import timed_operation
 from ..utils.detection_types import JsonDict, Pathlike
+from ..utils.error import FileExtensionError
 from ..utils.identifier import get_uuid_from_str
 from ..utils.pdf_utils import PDFStreamer
 from ..utils.tqdm import get_tqdm
-from ..utils.utils import FileExtensionError, is_file_extension
+from ..utils.utils import is_file_extension
 from .base import DataFlow
 from .common import FlattenData, JoinData, MapData
 from .custom import CacheData, CustomDataFromIterable, CustomDataFromList
 
 __all__ = ["SerializerJsonlines", "SerializerFiles", "SerializerCoco", "SerializerPdfDoc", "SerializerTabsepFiles"]
 
 
@@ -219,15 +222,15 @@
         return df
 
     @staticmethod
     def save() -> None:
         """
         Not implemented
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class CocoParser:
     """
     A simplified version of the Microsoft COCO helper class for reading  annotations. It currently supports only
     bounding box annotations
 
@@ -279,16 +282,22 @@
             self.imgs = imgs
             self.cats = cats
 
     def info(self) -> None:
         """
         Print information about the annotation file.
         """
+        rows = []
         for key, value in self.dataset["info"].items():
-            print(f"{key}: {value}")
+            row = [key, value]
+            rows.append(row)
+
+        header = ["key", "value"]
+        table = tabulate(rows, headers=header, tablefmt="fancy_grid", stralign="left", numalign="left")
+        print(colored(table, "cyan"))
 
     def get_ann_ids(
         self,
         img_ids: Optional[Union[int, Sequence[int]]] = None,
         cat_ids: Optional[Union[int, Sequence[int]]] = None,
         area_range: Optional[Sequence[int]] = None,
         is_crowd: Optional[bool] = None,
@@ -495,15 +504,15 @@
         return df
 
     @staticmethod
     def save() -> None:
         """
         Not implemented
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class SerializerPdfDoc:
     """
     Serialize a pdf document with an arbitrary number of pages.
 
     **Example:**
@@ -543,15 +552,15 @@
         return df
 
     @staticmethod
     def save(path: Pathlike) -> None:
         """
         Not implemented
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @staticmethod
     def split(path: Pathlike, path_target: Optional[Pathlike] = None, max_datapoint: Optional[int] = None) -> None:
         """
         Split a document into single pages.
         """
         if path_target is None:
```

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/parallel_map.py` & `deepdoctection-0.31/deepdoctection/dataflow/parallel_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import Any, Callable, Iterator, List, no_type_check
 
 import zmq
 
 from ..utils.concurrency import StoppableThread, enable_death_signal, start_proc_mask_signal
+from ..utils.error import DataFlowTerminatedError
 from ..utils.logger import LoggingRecord, logger
-from .base import DataFlow, DataFlowReentrantGuard, DataFlowTerminated, ProxyDataFlow
+from .base import DataFlow, DataFlowReentrantGuard, ProxyDataFlow
 from .common import RepeatedData
 from .serialize import PickleSerializer
 
 
 @no_type_check
 def del_weakref(x):
     """delete weakref"""
@@ -45,22 +46,22 @@
 @no_type_check
 @contextmanager
 def _zmq_catch_error(name):
     try:
         yield
     except zmq.ContextTerminated as exc:
         logger.info(LoggingRecord(f"_zmq_catch_error: [{name}] Context terminated."))
-        raise DataFlowTerminated() from exc
+        raise DataFlowTerminatedError() from exc
     except zmq.ZMQError as exc:
         if exc.errno == errno.ENOTSOCK:  # socket closed
             logger.info(LoggingRecord(f"_zmq_catch_error: [{name}]  Socket closed."))
-            raise DataFlowTerminated() from exc
-        raise ValueError from exc
+            raise DataFlowTerminatedError() from exc
+        raise ValueError() from exc
     except Exception as exc:
-        raise ValueError from exc
+        raise ValueError() from exc
 
 
 @no_type_check
 def _get_pipe_name(name):
     if sys.platform.startswith("linux"):
         # linux supports abstract sockets: http://api.zeromq.org/4-1:zmq-ipc
         pipename = f"ipc://@{name}-pipe-{str(uuid.uuid1())[:8]}"
@@ -74,16 +75,16 @@
         pipename = f"ipc://{filename}"
     return pipename
 
 
 class _ParallelMapData(ProxyDataFlow, ABC):
     def __init__(self, df: DataFlow, buffer_size: int, strict: bool = False) -> None:
         super().__init__(df)
-        if not buffer_size:
-            raise ValueError("buffer_size must be a positive number")
+        if buffer_size <= 0:
+            raise ValueError(f"buffer_size must be a positive number, got {buffer_size}")
         self._buffer_size = buffer_size
         self._buffer_occupancy = 0  # actual #elements in buffer, only useful in strict mode
         self._strict = strict
 
     def reset_state(self) -> None:
         super().reset_state()
         if not self._strict:
@@ -91,20 +92,20 @@
         else:
             df = self.df  # type: ignore
         self._iter = iter(df)
 
     @no_type_check
     @abstractmethod
     def _recv(self):
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @no_type_check
     @abstractmethod
     def _send(self, dp: Any):
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @no_type_check
     def _recv_filter_none(self):
         ret = self._recv()
         assert ret is not None, f"[{type(self).__name__}] map function cannot return None when strict mode is used."
         return ret
 
@@ -394,16 +395,16 @@
             try:
                 buffer_size = min(buffer_size, len(df))
             except Exception:  # pylint: disable=W0703  # ds may not have a length
                 pass
 
         _ParallelMapData.__init__(self, df, buffer_size, strict)
         _MultiProcessZMQDataFlow.__init__(self)
-        if not num_proc:
-            raise ValueError("num_proc must be a positive number")
+        if num_proc <= 0:
+            raise ValueError(f"num_proc must be a positive number, got {num_proc}")
         self.num_proc = num_proc
         self.map_func = map_func
         self._strict = strict
         self._procs = []
 
     @no_type_check
     def _create_worker(self, idx, pipename, hwm):
```

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/serialize.py` & `deepdoctection-0.31/deepdoctection/dataflow/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 import pickle
 from copy import copy
 from typing import Any, Iterable, Iterator, List, Optional, Tuple, Union
 
 import numpy as np
 
-from .base import DataFlow, DataFlowResetStateNotCalled, RNGDataFlow
+from ..utils.error import DataFlowResetStateNotCalledError
+from .base import DataFlow, RNGDataFlow
 
 
 class DataFromList(RNGDataFlow):
     """Wrap a list of datapoints to a DataFlow"""
 
     def __init__(self, lst: List[Any], shuffle: bool = True) -> None:
         """
@@ -40,15 +41,15 @@
         else:
             idxs = np.arange(len(self.lst))
             if self.rng is not None:
                 self.rng.shuffle(idxs)
                 for k in idxs:
                     yield self.lst[k]
             else:
-                raise DataFlowResetStateNotCalled()
+                raise DataFlowResetStateNotCalledError()
 
 
 class DataFromIterable(DataFlow):
     """Wrap an iterable of datapoints to a DataFlow"""
 
     def __init__(self, iterable: Iterable[Any]) -> None:
         """
@@ -59,15 +60,15 @@
         try:
             self._len = len(iterable)  # type: ignore
         except (NotImplementedError, TypeError):
             pass
 
     def __len__(self) -> int:
         if self._len is None:
-            raise NotImplementedError
+            raise NotImplementedError()
         return self._len
 
     def __iter__(self) -> Iterator[Any]:
         yield from self._itr
 
     def reset_state(self) -> None:
         pass
@@ -103,15 +104,15 @@
             raise ValueError(f"self.dtype={self.dtype} and self.shapes={self.shapes} must have same length")
 
     def __len__(self) -> int:
         return self._size
 
     def __iter__(self) -> Iterator[Any]:
         if self.rng is None:
-            raise DataFlowResetStateNotCalled()
+            raise DataFlowResetStateNotCalledError()
         if self.random:
             for _ in range(self._size):
                 val = []
                 for idx, _ in enumerate(self.shapes):
                     var = (
                         self.rng.rand(*self.shapes[idx]) * (self.domain[idx][1] - self.domain[idx][0])
                         + self.domain[idx][0]
```

### Comparing `deepdoctection-0.30/deepdoctection/dataflow/stats.py` & `deepdoctection-0.31/deepdoctection/dataflow/stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/__init__.py` & `deepdoctection-0.31/deepdoctection/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/annotation.py` & `deepdoctection-0.31/deepdoctection/datapoint/annotation.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,27 +20,37 @@
 """
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union, no_type_check
 
 from ..utils.detection_types import JsonDict
+from ..utils.error import AnnotationError, UUIDError
 from ..utils.identifier import get_uuid, is_uuid_like
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import DefaultType, ObjectTypes, SummaryType, TypeOrStr, get_type
 from .box import BoundingBox
 from .convert import as_dict
 
 
 @no_type_check
 def ann_from_dict(cls, **kwargs):
     """
     A factory function to create subclasses of annotations from a given dict
     """
-    ann = cls(kwargs.get("external_id"), kwargs.get("category_name"), kwargs.get("category_id"), kwargs.get("score"))
+    _init_kwargs = {
+        "external_id": kwargs.get("external_id"),
+        "category_name": kwargs.get("category_name"),
+        "category_id": kwargs.get("category_id"),
+        "score": kwargs.get("score"),
+        "service_id": kwargs.get("service_id"),
+        "model_id": kwargs.get("model_id"),
+        "session_id": kwargs.get("session_id"),
+    }
+    ann = cls(**_init_kwargs)
     ann.active = kwargs.get("active")
     ann._annotation_id = kwargs.get("_annotation_id")  # pylint: disable=W0212
     if isinstance(kwargs.get("sub_categories"), dict):
         for key, value in kwargs["sub_categories"].items():
             if "value" in value:
                 ann.dump_sub_category(key, ContainerAnnotation.from_dict(**value))
             else:
@@ -70,19 +80,25 @@
 
     `active`: Always set to `True`. You can change the value using `deactivate` .
 
     `external_id`: A string or integer value for generating an annotation id. Note, that the resulting annotation
     id will not depend on the defining attributes.
 
     `_annotation_id`: Unique id for annotations. Will always be given as string representation of a md5-hash.
+    `service_id`: Service that generated the annotation. This will be the name of a pipeline component
+    `model_id`: Model that generated the annotation. This will be the name of particular model
+    `session_id`: Session id for the annotation. This will be the id of the session in which the annotation was created.
     """
 
     active: bool = field(default=True, init=False, repr=True)
     external_id: Optional[Union[str, int]] = field(default=None, init=True, repr=False)
     _annotation_id: Optional[str] = field(default=None, init=False, repr=True)
+    service_id: Optional[str] = field(default=None)
+    model_id: Optional[str] = field(default=None)
+    session_id: Optional[str] = field(default=None)
 
     def __post_init__(self) -> None:
         """
         Will check, if the external id provided is an uuid. If not will use the external id as seed for defining an
         uuid.
         """
 
@@ -97,46 +113,46 @@
     @property
     def annotation_id(self) -> str:
         """
         annotation_id
         """
         if self._annotation_id:
             return self._annotation_id
-        raise ValueError("Dump annotation first or pass external_id to create an annotation id")
+        raise AnnotationError("Dump annotation first or pass external_id to create an annotation id")
 
     @annotation_id.setter
     def annotation_id(self, input_id: str) -> None:
         """
         annotation_id setter
         """
         if self._annotation_id is not None:
-            raise AssertionError("Annotation_id already defined and cannot be reset")
+            raise AnnotationError("Annotation_id already defined and cannot be reset")
         if is_uuid_like(input_id):
             self._annotation_id = input_id
         elif isinstance(input_id, property):
             pass
         else:
-            raise ValueError("Annotation_id must be uuid3 string")
+            raise AnnotationError("Annotation_id must be uuid3 string")
 
     @abstractmethod
     def get_defining_attributes(self) -> List[str]:
         """
         Defining attributes of an annotation instance are attributes, of which you think that they uniquely
         describe the annotation object. If you do not provide an external id, only the defining attributes will be used
         for generating the annotation id.
 
         :return: A list of attributes.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def _assert_attributes_have_str(self, state_id: bool = False) -> None:
         defining_attributes = self.get_state_attributes() if state_id else self.get_defining_attributes()
         for attr in defining_attributes:
             if not hasattr(eval("self." + attr), "__str__"):  # pylint: disable=W0123
-                raise AttributeError(f"Attribute {attr} must have __str__ method")
+                raise AnnotationError(f"Attribute {attr} must have __str__ method")
 
     @staticmethod
     def set_annotation_id(annotation: "CategoryAnnotation", *container_id_context: Optional[str]) -> str:
         """
         Defines the `annotation_id` by attributes of the annotation class as well as by external parameters given by a
         tuple or list of container id contexts.
 
@@ -175,25 +191,25 @@
         """
         Method to initialize a derived class from dict.
 
         :param kwargs: dict with `Annotation` attributes
 
         :return: Annotation instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
     def get_state_attributes() -> List[str]:
         """
         Similar to `get_defining_attributes` but for `state_id`
 
         :return: A list of attributes.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @property
     def state_id(self) -> str:
         """
         Different to `annotation_id` this id does depend on every defined state attributes and might therefore change
         over time.
 
@@ -286,15 +302,20 @@
 
         :param sub_category_name: key for defining the sub category.
         :param annotation: Annotation instance to dump
         :param container_id_context: Tuple/list of context ids.
         """
 
         if sub_category_name in self.sub_categories:
-            raise KeyError(f"{sub_category_name} as sub category already defined for " f"{self.annotation_id}")
+            raise AnnotationError(
+                f"sub category {sub_category_name} already defined: "
+                f"annotation_id: {self.annotation_id}, "
+                f"category_name: {self.category_name}, "
+                f"category_id: {self.category_id}"
+            )
 
         if self._annotation_id is not None:
             if annotation._annotation_id is None:  # pylint: disable=W0212
                 annotation.annotation_id = self.set_annotation_id(annotation, self.annotation_id, *container_id_context)
         else:
             tmp_annotation_id = self.set_annotation_id(self)
             if annotation._annotation_id is None:  # pylint: disable=W0212
@@ -329,15 +350,15 @@
         Dumps an `annotation_id` to a given key, in order to store relations between annotations. Note, that the
         referenced annotation must be stored elsewhere.
 
         :param key: The key, where to place the annotation id.
         :param annotation_id: An annotation id
         """
         if not is_uuid_like(annotation_id):
-            raise ValueError("Annotation_id must be uuid")
+            raise UUIDError("Annotation_id must be uuid")
 
         key_type = get_type(key)
         if key not in self.relationships:
             self.relationships[key_type] = []
         if annotation_id not in self.relationships[key_type]:
             self.relationships[key_type].append(annotation_id)
 
@@ -432,22 +453,22 @@
         from `bounding_box`. Raises `ValueError` if no bounding box is available."""
         if self.image and image_id:
             box = self.image.get_embedding(image_id)
         else:
             box = self.bounding_box
         if box:
             return box
-        raise ValueError(f"bounding_box has not been initialized for {self.annotation_id}")
+        raise AnnotationError(f"bounding_box has not been initialized for {self.annotation_id}")
 
     def get_summary(self, key: ObjectTypes) -> CategoryAnnotation:
         """Get summary sub categories from `image`. Raises `ValueError` if `key` is not available"""
         if self.image:
             if self.image.summary:
                 return self.image.summary.get_sub_category(key)
-        raise ValueError(f"Summary does not exist for {self.annotation_id} and key: {key}")
+        raise AnnotationError(f"Summary does not exist for {self.annotation_id} and key: {key}")
 
 
 @dataclass
 class SummaryAnnotation(CategoryAnnotation):
     """
     A dataclass for adding summaries. The various summaries can be stored as sub categories.
```

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/box.py` & `deepdoctection-0.31/deepdoctection/datapoint/box.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from typing import List, Optional, Sequence, no_type_check
 
 import numpy as np
 import numpy.typing as npt
 from numpy import float32
 
 from ..utils.detection_types import ImageType
+from ..utils.error import BoundingBoxError
 from ..utils.file_utils import cocotools_available
 from ..utils.logger import LoggingRecord, logger
 
 if cocotools_available():
     import pycocotools.mask as coco_mask
 
 
@@ -136,18 +137,14 @@
     """
 
     if cocotools_available():
         return coco_iou(boxes1, boxes2)
     return np_iou(boxes1, boxes2)
 
 
-class BoundingBoxError(BaseException):
-    """Special exception only for `BoundingBox`"""
-
-
 @dataclass
 class BoundingBox:
     """
     Rectangular bounding box dataclass for object detection. Store coordinates and allows several
     representations. You can define an instance by passing the upper left point along with either height
     and width or along with the lower right point. Pass absolute_coords = 'True' if you work with image
     pixel coordinates. If you work with coordinates in the range between (0,1) then pass absolute_coords
```

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/convert.py` & `deepdoctection-0.31/deepdoctection/datapoint/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import numpy as np
 from numpy import uint8
 from numpy.typing import NDArray
 from pypdf import PdfReader
 
 from ..utils.detection_types import ImageType
 from ..utils.develop import deprecated
+from ..utils.error import DependencyError
 from ..utils.pdf_utils import pdf_to_np_array
 from ..utils.viz import viz_handler
 
 __all__ = [
     "convert_b64_to_np_array",
     "convert_np_array_to_b64",
     "convert_np_array_to_b64_b",
@@ -117,15 +118,16 @@
     :param pdf_bytes: A pdf as bytes object. A byte representation can from a pdf file can be generated e.g. with
                       `utils.fs.load_bytes_from_pdf_file`
     :param dpi: The dpi value of the resulting output image. For high resolution set dpi=300.
     :return: Image as numpy array.
     """
     from pdf2image import convert_from_bytes  # type: ignore # pylint: disable=C0415, E0401
 
-    assert which("pdftoppm") is not None, "convert_pdf_bytes_to_np_array requires poppler to be installed"
+    if which("pdftoppm") is None:
+        raise DependencyError("convert_pdf_bytes_to_np_array requires poppler to be installed")
 
     with BytesIO(pdf_bytes) as pdf_file:
         pdf = PdfReader(pdf_file).pages[0]
     shape = pdf.mediabox  # pylint: disable=E1101
     height = shape[3] - shape[1]
     width = shape[2] - shape[0]
     buffered = BytesIO()
```

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/image.py` & `deepdoctection-0.31/deepdoctection/datapoint/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union, no_type_check
 
 import numpy as np
 from numpy import uint8
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
+from ..utils.error import AnnotationError, BoundingBoxError, ImageError, UUIDError
 from ..utils.identifier import get_uuid, is_uuid_like
 from ..utils.settings import ObjectTypes, get_type
 from .annotation import Annotation, BoundingBox, ImageAnnotation, SummaryAnnotation
 from .box import crop_box_from_image, global_to_local_coords, intersection_box
 from .convert import as_dict, convert_b64_to_np_array, convert_np_array_to_b64, convert_pdf_bytes_to_np_array_v2
 
 
@@ -104,29 +105,29 @@
     @property
     def image_id(self) -> str:
         """
         image_id
         """
         if self._image_id is not None:
             return self._image_id
-        raise ValueError("image_id not set")
+        raise ImageError("image_id not set")
 
     @image_id.setter
     def image_id(self, input_id: str) -> None:
         """
         image_id setter
         """
         if self._image_id is not None:
-            raise ValueError("image_id already defined and cannot be reset")
+            raise ImageError("image_id already defined and cannot be reset")
         if is_uuid_like(input_id):
             self._image_id = input_id
         elif isinstance(input_id, property):
             pass
         else:
-            raise ValueError("image_id must be uuid3 string")
+            raise UUIDError("image_id must be uuid3 string")
 
     @property
     def image(self) -> Optional[ImageType]:
         """
         image
         """
         return self._image
@@ -149,15 +150,15 @@
             self._self_embedding()
         elif isinstance(image, bytes):
             self._image = convert_pdf_bytes_to_np_array_v2(image, dpi=environ.get("DPI", 300))  # type: ignore
             self.set_width_height(self._image.shape[1], self._image.shape[0])
             self._self_embedding()
         else:
             if not isinstance(image, np.ndarray):
-                raise TypeError(f"Cannot load image is of type: {type(image)}")
+                raise ImageError(f"Cannot load image is of type: {type(image)}")
             self._image = image.astype(uint8)
             self.set_width_height(self._image.shape[1], self._image.shape[0])
             self._self_embedding()
 
     @property
     def summary(self) -> Optional[SummaryAnnotation]:
         """summary"""
@@ -244,24 +245,24 @@
 
     @property
     def width(self) -> float:
         """
         width
         """
         if self._bbox is None:
-            raise ValueError("Width not available. Call set_width_height first")
+            raise ImageError("Width not available. Call set_width_height first")
         return self._bbox.width
 
     @property
     def height(self) -> float:
         """
         height
         """
         if self._bbox is None:
-            raise ValueError("Height not available. Call set_width_height first")
+            raise ImageError("Height not available. Call set_width_height first")
         return self._bbox.height
 
     def set_width_height(self, width: float, height: float) -> None:
         """
         Defines bounding box of the image if not already set. Use this, if you do not want to keep the image separated
         for memory reasons.
 
@@ -277,15 +278,15 @@
         Set embedding pair. Pass an image_id and a bounding box defining the spacial position of this image with
         respect to the embedding image.
 
         :param image_id: A uuid of the embedding image.
         :param bounding_box: bounding box of this image in terms of the embedding image.
         """
         if not isinstance(bounding_box, BoundingBox):
-            raise TypeError(f"Bounding box must be of type BoundingBox, is of type {type(bounding_box)}")
+            raise BoundingBoxError(f"Bounding box must be of type BoundingBox, is of type {type(bounding_box)}")
         self.embeddings[image_id] = bounding_box
 
     def get_embedding(self, image_id: str) -> BoundingBox:
         """
         Returns the bounding box according to the `image_id`.
 
         :param image_id: uuid string of the embedding image
@@ -303,81 +304,117 @@
         Dump an annotation to the Image dataclass. This is the central method for associating an annotation with
         an image. It gives the annotation an `annotation_id` in relation to the `image_id` in order to ensure uniqueness
         across all images.
 
         :param annotation: image annotation to store
         """
         if not isinstance(annotation, ImageAnnotation):
-            raise TypeError(
+            raise AnnotationError(
                 f"Annotation must be of type ImageAnnotation: "
                 f"{annotation.annotation_id} but is of type {str(type(annotation))}"
             )
         if annotation._annotation_id is None:  # pylint: disable=W0212
             annotation.annotation_id = self.define_annotation_id(annotation)
         if annotation.annotation_id in self._annotation_ids:
-            raise ValueError(f"Cannot dump annotation with already taken " f"id {annotation.annotation_id}")
+            raise ImageError(f"Cannot dump annotation with already taken " f"id {annotation.annotation_id}")
         self._annotation_ids.append(annotation.annotation_id)
         self.annotations.append(annotation)
 
     def get_annotation(
         self,
         category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
         annotation_ids: Optional[Union[str, Sequence[str]]] = None,
-        annotation_types: Optional[Union[str, Sequence[str]]] = None,
+        service_id: Optional[Union[str, Sequence[str]]] = None,
+        model_id: Optional[Union[str, Sequence[str]]] = None,
+        session_ids: Optional[Union[str, Sequence[str]]] = None,
+        ignore_inactive: bool = True,
     ) -> List[ImageAnnotation]:
         """
         Selection of annotations from the annotation container. Filter conditions can be defined by specifying
         the annotation_id or the category name. (Since only image annotations are currently allowed in the container,
         annotation_type is a redundant filter condition.) Only annotations that have  active = 'True' are
         returned. If more than one condition is provided, only annotations will be returned that satisfy all conditions.
         If no condition is provided, it will return all active annotations.
 
         :param category_names: A single name or list of names
         :param annotation_ids: A single id or list of ids
-        :param annotation_types: A type name or list of type names.
+        :param service_id: A single service name or list of service names
+        :param model_id: A single model name or list of model names
+        :param session_ids: A single session id or list of session ids
+        :param ignore_inactive: If set to `True` only active annotations are returned.
+
         :return: A (possibly empty) list of Annotations
         """
 
-        cat_names = [category_names] if isinstance(category_names, (ObjectTypes, str)) else category_names
-        if cat_names is not None:
-            cat_names = [get_type(cat_name) for cat_name in cat_names]
-        ann_ids = [annotation_ids] if isinstance(annotation_ids, str) else annotation_ids
-        ann_types = [annotation_types] if isinstance(annotation_types, str) else annotation_types
+        if category_names is not None:
+            category_names = (
+                [get_type(cat_name) for cat_name in category_names]
+                if isinstance(category_names, (list, set))
+                else [get_type(category_names)]  # type:ignore
+            )
 
-        anns = filter(lambda x: x.active, self.annotations)
+        ann_ids = [annotation_ids] if isinstance(annotation_ids, str) else annotation_ids
+        service_id = [service_id] if isinstance(service_id, str) else service_id
+        model_id = [model_id] if isinstance(model_id, str) else model_id
+        session_id = [session_ids] if isinstance(session_ids, str) else session_ids
 
-        if ann_types is not None:
-            for type_name in ann_types:
-                anns = filter(lambda x: isinstance(x, eval(type_name)), anns)  # pylint: disable=W0123, W0640
+        if ignore_inactive:
+            anns = filter(lambda x: x.active, self.annotations)
+        else:
+            anns = self.annotations  # type:ignore
 
-        if cat_names is not None:
-            anns = filter(lambda x: x.category_name in cat_names, anns)  # type:ignore
+        if category_names is not None:
+            anns = filter(lambda x: x.category_name in category_names, anns)  # type:ignore
 
         if ann_ids is not None:
             anns = filter(lambda x: x.annotation_id in ann_ids, anns)  # type:ignore
 
+        if service_id is not None:
+            anns = filter(lambda x: x.service_id in service_id, anns)  # type:ignore
+
+        if model_id is not None:
+            anns = filter(lambda x: x.model_id in model_id, anns)  # type:ignore
+
+        if session_id is not None:
+            anns = filter(lambda x: x.session_id in session_id, anns)  # type:ignore
+
         return list(anns)
 
     def get_annotation_iter(
         self,
         category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
         annotation_ids: Optional[Union[str, Sequence[str]]] = None,
-        annotation_types: Optional[Union[str, Sequence[str]]] = None,
+        service_id: Optional[Union[str, Sequence[str]]] = None,
+        model_id: Optional[Union[str, Sequence[str]]] = None,
+        session_ids: Optional[Union[str, Sequence[str]]] = None,
+        ignore_inactive: bool = True,
     ) -> Iterable[ImageAnnotation]:
         """
         Get annotation as an iterator. Same as `get_annotation` but returns an iterator instead of a list.
 
         :param category_names: A single name or list of names
         :param annotation_ids: A single id or list of ids
-        :param annotation_types: A type name or list of type names.
+        :param service_id: A single service name or list of service names
+        :param model_id: A single model name or list of model names
+        :param session_ids: A single session id or list of session ids
+        :param ignore_inactive: If set to `True` only active annotations are returned.
 
         :return: A (possibly empty) list of annotations
         """
 
-        return iter(self.get_annotation(category_names, annotation_ids, annotation_types))
+        return iter(
+            self.get_annotation(
+                category_names=category_names,
+                annotation_ids=annotation_ids,
+                service_id=service_id,
+                model_id=model_id,
+                session_ids=session_ids,
+                ignore_inactive=ignore_inactive,
+            )
+        )
 
     def as_dict(self) -> Dict[str, Any]:
         """
         Returns the full image dataclass as dict. Uses the custom `convert.as_dict` to disregard attributes
         defined by `remove_keys`.
 
         :return:  A custom dict.
@@ -435,30 +472,30 @@
         """
 
         ann = self.get_annotation(annotation_ids=annotation_id)[0]
 
         new_image = Image(file_name=self.file_name, location=self.location, external_id=annotation_id)
 
         if self._bbox is None or ann.bounding_box is None:
-            raise ValueError(f"Bounding box for image and ImageAnnotation ({annotation_id}) must be set")
+            raise ImageError(f"Bounding box for image and ImageAnnotation ({annotation_id}) must be set")
 
         new_bounding_box = intersection_box(self._bbox, ann.bounding_box, self.width, self.height)
         if new_bounding_box.absolute_coords:
             width = new_bounding_box.width
             height = new_bounding_box.height
         else:
             width = new_bounding_box.width * self.width
             height = new_bounding_box.height * self.height
         new_image.set_width_height(width, height)
         new_image.set_embedding(self.image_id, bounding_box=new_bounding_box)
 
         if crop_image and self.image is not None:
             new_image.image = crop_box_from_image(self.image, ann.bounding_box, self.width, self.height)
         elif crop_image and self.image is None:
-            raise ValueError("crop_image = True requires self.image to be not None")
+            raise ImageError("crop_image = True requires self.image to be not None")
 
         ann.image = new_image
 
     def maybe_ann_to_sub_image(self, annotation_id: str, category_names: Union[str, List[str]]) -> None:
         """
         Provides a supplement to `image_ann_to_image` and mainly operates on the `ImageAnnotation.image` of
         the image annotation. The aim is to assign image annotations from this image one hierarchy level lower to the
@@ -468,28 +505,28 @@
         :param annotation_id: image annotation you want to assign image annotation from this image. Note, that the
                               annotation must have a not None `image`.
         :param category_names: Filter the proposals of all image categories of this image by some given category names.
         """
 
         ann = self.get_annotation(annotation_ids=annotation_id)[0]
         if ann.image is None:
-            raise ValueError("When adding sub images to ImageAnnotation then ImageAnnotation.image must not be None")
+            raise ImageError("When adding sub images to ImageAnnotation then ImageAnnotation.image must not be None")
         assert ann.bounding_box is not None
         box = ann.bounding_box.to_list("xyxy")
         proposals = self.get_annotation(category_names)
         points = np.array([prop.get_bounding_box(self.image_id).center for prop in proposals])
         ann_ids = np.array([prop.annotation_id for prop in proposals])
         indices = np.where(
             (box[0] < points[:, 0]) & (box[1] < points[:, 1]) & (box[2] > points[:, 0]) & (box[3] > points[:, 1])
         )[0]
         selected_ids = ann_ids[indices]
         sub_images = self.get_annotation(annotation_ids=selected_ids.tolist())
         for sub_image in sub_images:
             if sub_image.image is None:
-                raise ValueError(
+                raise ImageError(
                     "When setting an embedding to ImageAnnotation then ImageAnnotation.image must not be None"
                 )
             sub_image.image.set_embedding(
                 annotation_id,
                 global_to_local_coords(sub_image.get_bounding_box(self.image_id), ann.get_bounding_box(self.image_id)),
             )
             ann.image.dump(sub_image)
```

### Comparing `deepdoctection-0.30/deepdoctection/datapoint/view.py` & `deepdoctection-0.31/deepdoctection/datapoint/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from copy import copy
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple, Type, Union, no_type_check
 
 import numpy as np
 
 from ..utils.detection_types import ImageType, JsonDict, Pathlike
+from ..utils.error import AnnotationError, ImageError
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import (
     CellType,
     LayoutType,
     ObjectTypes,
     PageType,
     Relationships,
@@ -92,15 +93,15 @@
                 self.base_page.image, bounding_box, self.base_page.width, self.base_page.height
             )
 
             if interactive:
                 interactive_imshow(np_image)
                 return None
             return np_image
-        raise ValueError(f"base_page.image is None for {self.annotation_id}")
+        raise AnnotationError(f"base_page.image is None for {self.annotation_id}")
 
     def __getattr__(self, item: str) -> Optional[Union[str, int, List[str]]]:
         """
         Get attributes defined by registered `self.get_attribute_names()` in a multi step process:
 
         - Unregistered attributes will raise an `AttributeError`.
         - Registered attribute will look for a corresponding sub category. If the sub category does not exist `Null`
@@ -111,15 +112,15 @@
           `category_id` will be returned.
         - If nothing works, look at `self.image.summary` if the item exist. Follow the same logic as for ordinary sub
           categories.
         :param item: attribute name
         :return: value according to the logic described above
         """
         if item not in self.get_attribute_names():
-            raise AttributeError(f"Attribute {item} is not supported for {type(self)}")
+            raise AnnotationError(f"Attribute {item} is not supported for {type(self)}")
         if item in self.sub_categories:
             sub_cat = self.get_sub_category(get_type(item))
             if item != sub_cat.category_name:
                 return sub_cat.category_name
             if isinstance(sub_cat, ContainerAnnotation):
                 return sub_cat.value
             return int(sub_cat.category_id)
@@ -322,15 +323,15 @@
         out = " ".join([" ".join(row + ["\n"]) for row in self.csv])
         return out
 
     @property
     def text(self) -> str:
         try:
             return str(self)
-        except TypeError:
+        except (TypeError, AnnotationError):
             return super().text
 
     @property
     def text_(self) -> Dict[str, Union[str, List[str]]]:
         cells = self.cells
         if not cells:
             return super().text_
@@ -364,15 +365,15 @@
         try:
             cells = self.cells
             all_words = []
             cells.sort(key=lambda x: (x.row_number, x.column_number))
             for cell in cells:
                 all_words.extend(cell.get_ordered_words())  # type: ignore
             return all_words
-        except TypeError:
+        except (TypeError, AnnotationError):
             return super().get_ordered_words()
 
 
 IMAGE_ANNOTATION_TO_LAYOUTS: Dict[ObjectTypes, Type[Union[Layout, Table, Word]]] = {
     **{i: Layout for i in LayoutType if (i not in {LayoutType.table, LayoutType.word, LayoutType.cell})},
     LayoutType.table: Table,
     LayoutType.table_rotated: Table,
@@ -448,48 +449,79 @@
         "words",
         "file_name",
         "location",
         "document_id",
         "page_number",
     }
 
-    @no_type_check
-    def get_annotation(
+    def get_annotation(  # type: ignore
         self,
         category_names: Optional[Union[str, ObjectTypes, Sequence[Union[str, ObjectTypes]]]] = None,
         annotation_ids: Optional[Union[str, Sequence[str]]] = None,
-        annotation_types: Optional[Union[str, Sequence[str]]] = None,
+        service_id: Optional[Union[str, Sequence[str]]] = None,
+        model_id: Optional[Union[str, Sequence[str]]] = None,
+        session_ids: Optional[Union[str, Sequence[str]]] = None,
+        ignore_inactive: bool = True,
     ) -> List[ImageAnnotationBaseView]:
         """
+        Selection of annotations from the annotation container. Filter conditions can be defined by specifying
+        the annotation_id or the category name. (Since only image annotations are currently allowed in the container,
+        annotation_type is a redundant filter condition.) Only annotations that have  active = 'True' are
+        returned. If more than one condition is provided, only annotations will be returned that satisfy all conditions.
+        If no condition is provided, it will return all active annotations.
+
         Identical to its base class method for having correct return types. If the base class changes, please
         change this method as well.
+
+        :param category_names: A single name or list of names
+        :param annotation_ids: A single id or list of ids
+        :param service_id: A single service name or list of service names
+        :param model_id: A single model name or list of model names
+        :param session_ids: A single session id or list of session ids
+        :param ignore_inactive: If set to `True` only active annotations are returned.
+
+        :return: A (possibly empty) list of Annotations
         """
-        cat_names = [category_names] if isinstance(category_names, (ObjectTypes, str)) else category_names
-        if cat_names is not None:
-            cat_names = [get_type(cat_name) for cat_name in cat_names]
+
+        if category_names is not None:
+            category_names = (
+                [get_type(cat_name) for cat_name in category_names]
+                if isinstance(category_names, list)
+                else [get_type(category_names)]  # type:ignore
+            )
         ann_ids = [annotation_ids] if isinstance(annotation_ids, str) else annotation_ids
-        ann_types = [annotation_types] if isinstance(annotation_types, str) else annotation_types
+        service_id = [service_id] if isinstance(service_id, str) else service_id
+        model_id = [model_id] if isinstance(model_id, str) else model_id
+        session_id = [session_ids] if isinstance(session_ids, str) else session_ids
+
+        if ignore_inactive:
+            anns = filter(lambda x: x.active, self.annotations)
+        else:
+            anns = self.annotations  # type:ignore
 
-        anns = filter(lambda x: x.active, self.annotations)
+        if category_names is not None:
+            anns = filter(lambda x: x.category_name in category_names, anns)  # type:ignore
 
-        if ann_types is not None:
-            for type_name in ann_types:
-                anns = filter(lambda x: isinstance(x, eval(type_name)), anns)  # pylint: disable=W0123, W0640
+        if ann_ids is not None:
+            anns = filter(lambda x: x.annotation_id in ann_ids, anns)  # type:ignore
 
-        if cat_names is not None:
-            anns = filter(lambda x: x.category_name in cat_names, anns)
+        if service_id is not None:
+            anns = filter(lambda x: x.generating_service in service_id, anns)  # type:ignore
 
-        if ann_ids is not None:
-            anns = filter(lambda x: x.annotation_id in ann_ids, anns)
+        if model_id is not None:
+            anns = filter(lambda x: x.generating_model in model_id, anns)  # type:ignore
+
+        if session_id is not None:
+            anns = filter(lambda x: x.session_id in session_id, anns)  # type:ignore
 
-        return list(anns)
+        return list(anns)  # type:ignore
 
     def __getattr__(self, item: str) -> Any:
         if item not in self.get_attribute_names():
-            raise AttributeError(f"Attribute {item} is not supported for {type(self)}")
+            raise ImageError(f"Attribute {item} is not supported for {type(self)}")
         if self.summary is not None:
             if item in self.summary.sub_categories:
                 sub_cat = self.summary.get_sub_category(get_type(item))
                 if item != sub_cat.category_name:
                     return sub_cat.category_name
                 if isinstance(sub_cat, ContainerAnnotation):
                     return sub_cat.value
@@ -625,18 +657,18 @@
 
         :param annotation_id: id of central layout element
         :param context_size: number of elements to the left and right of the central element
         :return: list of `ImageAnnotationBaseView` objects
         """
         ann = self.get_annotation(annotation_ids=annotation_id)[0]
         if ann.category_name not in self.floating_text_block_categories:
-            raise ValueError(
-                f"Annotation {annotation_id} with category_name {ann.category_name} is not a floating text "
-                f"block category. Cannot get context. Make sure to make this category a floating text "
-                f"block"
+            raise ImageError(
+                f"Cannot get context. Make sure to parametrize this category to a floating text: "
+                f"annotation_id: {annotation_id},"
+                f"category_name: {ann.category_name}"
             )
         block_with_order = self._order("layouts")
         position = block_with_order.index(ann)
         return block_with_order[
             max(0, position - context_size) : min(position + context_size + 1, len(block_with_order))
         ]
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/__init__.py` & `deepdoctection-0.31/deepdoctection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/adapter.py` & `deepdoctection-0.31/deepdoctection/datasets/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,8 +161,8 @@
 
     def __len__(self) -> int:
         if self.number_datapoints:
             return self.number_datapoints
         return len(self.df)
 
     def __getitem__(self, item: Any) -> None:
-        raise NotImplementedError
+        raise NotImplementedError()
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/base.py` & `deepdoctection-0.31/deepdoctection/datasets/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for the base class of datasets.
 """
-
+import json
 import os
 import pprint
 from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
+from inspect import signature
+from pathlib import Path
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
 
 import numpy as np
 
 from ..dataflow import CacheData, ConcatData, CustomDataFromList, DataFlow
-from ..datapoint import Image
+from ..datapoint.image import Image
 from ..utils.detection_types import Pathlike
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from .dataflow_builder import DataFlowBaseBuilder
 from .info import DatasetCategories, DatasetInfo, get_merged_categories
 
 
@@ -47,17 +49,19 @@
         assert self._info() is not None, "Dataset requires at least a name defined in DatasetInfo"
         self._dataset_info = self._info()
         self._dataflow_builder = self._builder()
         self._dataflow_builder.categories = self._categories()
         self._dataflow_builder.splits = self._dataset_info.splits
 
         if not self.dataset_available() and self.is_built_in():
-            print(
-                f"Dataset {self._dataset_info.name} not locally found. Please download at {self._dataset_info.url}"
-                f" and place under {self._dataflow_builder.get_workdir()}"
+            logger.warning(
+                LoggingRecord(
+                    f"Dataset {self._dataset_info.name} not locally found. Please download at {self._dataset_info.url}"
+                    f" and place under {self._dataflow_builder.get_workdir()}"
+                )
             )
 
     @property
     def dataset_info(self) -> DatasetInfo:
         """
         dataset_info
         """
@@ -72,32 +76,32 @@
 
     @abstractmethod
     def _categories(self) -> DatasetCategories:
         """
         Construct the DatasetCategory object.
         """
 
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @classmethod
     @abstractmethod
     def _info(cls) -> DatasetInfo:
         """
         Construct the DatasetInfo object.
         """
 
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def _builder(self) -> DataFlowBaseBuilder:
         """
         Construct the DataFlowBaseBuilder object. It needs to be implemented in the derived class.
         """
 
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def dataset_available(self) -> bool:
         """
         Datasets must be downloaded and maybe unzipped manually. Checks, if the folder exists, where the dataset is
         expected.
         """
         if os.path.isdir(self._dataflow_builder.get_workdir()):
@@ -110,15 +114,15 @@
         Returns flag to indicate if dataset is custom or built int.
         """
         return False
 
 
 class _BuiltInDataset(DatasetBase, ABC):
     """
-    Dataclass for built-in dataset. Do not use this it
+    Dataclass for built-in dataset. Do not use this
     """
 
     _name: Optional[str] = None
 
     @staticmethod
     def is_built_in() -> bool:
         """
@@ -423,18 +427,87 @@
         self.location = location
         self.init_categories = init_categories
         if init_sub_categories is None:
             self.init_sub_categories: Mapping[ObjectTypes, Mapping[ObjectTypes, Sequence[ObjectTypes]]] = {}
         else:
             self.init_sub_categories = init_sub_categories
         self.annotation_files = annotation_files
+        if signature(dataflow_builder.__init__).parameters.keys() != {"self", "location", "annotation_files"}:
+            raise TypeError(
+                "Dataflow builder must have the signature `def __init__(self, location: Pathlike, "
+                "annotation_files: Optional[Mapping[str, Union[str, Sequence[str]]]] = None):`"
+            )
         self.dataflow_builder = dataflow_builder(self.location, self.annotation_files)
         super().__init__()
 
     def _info(self) -> DatasetInfo:  # type: ignore  # pylint: disable=W0221
         return DatasetInfo(name=self.name, type=self.type, description="", license="", url="", splits={})
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=self.init_categories, init_sub_categories=self.init_sub_categories)
 
     def _builder(self) -> DataFlowBaseBuilder:
         return self.dataflow_builder
+
+    @staticmethod
+    def from_dataset_card(file_path: str, dataflow_builder: Type[DataFlowBaseBuilder]) -> "CustomDataset":
+        """
+        This static method creates a CustomDataset instance from a dataset card.
+
+        A dataset card is a JSON file that contains metadata about the dataset such as its name, type, location,
+        initial categories, initial sub categories, and annotation files. The dataflow_builder parameter is a class
+        that inherits from DataFlowBaseBuilder and is used to build the dataflow for the dataset.
+
+        :param file_path: The path to the dataset card (JSON file).
+        :param dataflow_builder: The class used to build the dataflow for the dataset.
+        :return: A CustomDataset instance created from the dataset card.
+        """
+
+        with open(file_path, "r", encoding="UTF-8") as file:
+            meta_data = json.load(file)
+        meta_data["dataset_type"] = get_type(meta_data["dataset_type"])
+        meta_data["location"] = Path(meta_data["location"])
+        meta_data["init_categories"] = [get_type(cat) for cat in meta_data["init_categories"]]
+        meta_data["init_sub_categories"] = (
+            {
+                get_type(cat): {
+                    get_type(sub_cat_key): [get_type(sub_cat_value) for sub_cat_value in sub_cat_values]
+                    for sub_cat_key, sub_cat_values in sub_cats.items()
+                }
+                for cat, sub_cats in meta_data["init_sub_categories"].items()
+            }
+            if meta_data["init_sub_categories"] is not None
+            else None
+        )
+        return CustomDataset(**meta_data, dataflow_builder=dataflow_builder)
+
+    def as_dict(self) -> Mapping[str, Any]:
+        """
+        Return the meta-data of the dataset as a dictionary.
+
+        :return: A dictionary containing the meta-data of the dataset.
+        """
+        return {
+            "name": self.name,
+            "dataset_type": self.type,
+            "location": str(self.location),
+            "annotation_files": self.annotation_files,
+            "init_categories": [cat.value for cat in self.init_categories],
+            "init_sub_categories": {
+                cat.value: {
+                    sub_cat_key.value: [sub_cat_value.value for sub_cat_value in sub_cat_values]
+                    for sub_cat_key, sub_cat_values in sub_cats.items()
+                }
+                for cat, sub_cats in self.init_sub_categories.items()
+            }
+            if self.init_sub_categories is not None
+            else None,
+        }
+
+    def save_dataset_card(self, file_path: str) -> None:
+        """
+        Save the dataset card to a JSON file.
+
+        :param file_path: file_path
+        """
+        with open(file_path, "w", encoding="UTF-8") as file:
+            json.dump(self.as_dict(), file, indent=4)
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/dataflow_builder.py` & `deepdoctection-0.31/deepdoctection/datasets/dataflow_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     def build(self, **kwargs: Union[str, int]) -> DataFlow:
         """
         Consult the docstring w.r.t `DataFlowBaseBuilder`.
 
         :param kwargs: A custom set of arguments/values
         :return: dataflow
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def get_annotation_file(self, split: str) -> str:
         """Get single annotation file."""
         split_file = self.annotation_files[split]
         if isinstance(split_file, str):
             return split_file
         raise TypeError("Unsupported get method for sequence type splits")
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/info.py` & `deepdoctection-0.31/deepdoctection/datasets/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
         :param cat_to_sub_cat: A dict of pairs of category/sub-category. Note that the combination must be available
                                according to the initial settings.
         """
 
         _cat_to_sub_cat = {get_type(key): get_type(value) for key, value in cat_to_sub_cat.items()}
         if not self._allow_update:
-            raise PermissionError("Replacing categories with sub categories is not allowed")
+            raise RuntimeWarning("Replacing categories with sub categories is not allowed")
         self._categories_update = self.init_categories
         categories = self.get_categories(name_as_key=True)
         cats_or_sub_cats = [
             self.init_sub_categories.get(cat, {cat: [cat]}).get(_cat_to_sub_cat.get(cat, cat), [cat])
             for cat in categories  # pylint: disable=E1133
         ]
         self._cat_to_sub_cat = _cat_to_sub_cat
@@ -328,15 +328,15 @@
         Filter categories of a dataset. This will keep all the categories chosen and remove all others.
         This method can only be called once per object.
 
         :param categories: A single category name or a list of category names.
         """
 
         if not self._allow_update:
-            raise PermissionError("Filtering categories is not allowed")
+            raise RuntimeWarning("Filtering categories is not allowed")
         if isinstance(categories, (ObjectTypes, str)):
             categories = [get_type(categories)]
         else:
             categories = [get_type(category) for category in categories]
 
         self._categories_filter_update: Sequence[ObjectTypes] = [
             cat for cat in self._categories_update if cat in categories
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/__init__.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/doclaynet.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/fintabnet.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/funsd.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/funsd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/iiitar13k.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/layouttest.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/layouttest.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,20 +45,15 @@
 
 _LICENSE = (
     "The annotations in this dataset belong to Dr. Janis Meyer and are licensed \n"
     " under a Community Data License Agreement \n"
     " – Permissive – Version 1.0 License. Dr. Janis Meyer does not own the copyright of the images. \n"
     " Use of the images must abide by the PMC Open Access Subset Terms of Use."
 )
-_URL = [
-    "https://www.googleapis.com/drive/v3/files/1ZD4Ef4gd2FIfp7vR8jbnrZeXD3gSWNqE?alt"
-    "=media&key=AIzaSyDuoPG6naK-kRJikScR7cP_1sQBF1r3fWU",
-    "https://www.googleapis.com/drive/v3/files/18HD62LFLa1iAmqffo4SyjuEQ32MzyNQ0?alt"
-    "=media&key=AIzaSyDuoPG6naK-kRJikScR7cP_1sQBF1r3fWU",
-]
+
 _SPLITS: Mapping[str, str] = {"test": "test", "predict": "predict"}
 _TYPE = DatasetType.object_detection
 _LOCATION = "testlayout"
 
 _ANNOTATION_FILES: Mapping[str, str] = {
     "test": "xrf_layout_test.jsonl",
     "predict": "xrf_layout_test_predict.jsonl",
@@ -73,15 +68,15 @@
     LayoutTest
     """
 
     _name = _NAME
 
     @classmethod
     def _info(cls) -> DatasetInfo:
-        return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, url=_URL, splits=_SPLITS, type=_TYPE)
+        return DatasetInfo(name=_NAME, description=_DESCRIPTION, license=_LICENSE, splits=_SPLITS, type=_TYPE)
 
     def _categories(self) -> DatasetCategories:
         return DatasetCategories(init_categories=_INIT_CATEGORIES)
 
     def _builder(self) -> "LayoutTestBuilder":
         return LayoutTestBuilder(location=_LOCATION, annotation_files=_ANNOTATION_FILES)
```

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/publaynet.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/pubtables1m.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/pubtabnet.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/rvlcdip.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/xfund.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/xfund.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/xsl/__init__.py` & `deepdoctection-0.31/deepdoctection/datasets/instances/xsl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/instances/xsl/pascal_voc.xsl` & `deepdoctection-0.31/deepdoctection/datasets/instances/xsl/pascal_voc.xsl`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/registry.py` & `deepdoctection-0.31/deepdoctection/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/datasets/save.py` & `deepdoctection-0.31/deepdoctection/datasets/save.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/eval/__init__.py` & `deepdoctection-0.31/deepdoctection/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/eval/accmetric.py` & `deepdoctection-0.31/deepdoctection/eval/accmetric.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     :return: Accuracy score with only unmasked values to be considered
     """
 
     np_label_gt, np_label_pr = np.asarray(label_gt), np.asarray(label_predictions)
     if len(np_label_gt) != len(np_label_pr):
         raise ValueError(
-            f"length of label_gt ({len(np_label_gt)}) and label_predictions" f" ({len(np_label_pr)}) must be equal"
+            f"length label_gt: {len(np_label_gt)}, length label_predictions: ({len(np_label_pr)}) but must be equal"
         )
     if masks is not None:
         np_label_gt, np_label_pr = _mask_some_gt_and_pr_labels(np_label_gt, np_label_pr, masks)
 
     number_samples = np_label_gt.shape[0]
     return float((np_label_gt == np_label_pr).sum() / number_samples)
```

### Comparing `deepdoctection-0.30/deepdoctection/eval/base.py` & `deepdoctection-0.31/deepdoctection/eval/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, Optional, Tuple
 
 from ..dataflow import DataFlow
 from ..datasets.info import DatasetCategories
 from ..utils.detection_types import JsonDict
+from ..utils.error import DependencyError
 from ..utils.file_utils import Requirement
 
 
 class MetricBase(ABC):
     """
     Base class for metrics. Metrics only exist as classes and are not instantiated. They consist of two class variables:
 
@@ -48,58 +49,58 @@
     mapper: Callable[[Any, Any], Optional[Any]]
     _results: List[JsonDict]
 
     def __new__(cls, *args, **kwargs):  # type: ignore # pylint: disable=W0613
         requirements = cls.get_requirements()
         name = cls.__name__ if hasattr(cls, "__name__") else cls.__class__.__name__
         if not all(requirement[1] for requirement in requirements):
-            raise ImportError(
+            raise DependencyError(
                 "\n".join(
                     [f"{name} has the following dependencies:"]
                     + [requirement[2] for requirement in requirements if not requirement[1]]
                 )
             )
         return super().__new__(cls)
 
     @classmethod
     @abstractmethod
     def get_requirements(cls) -> List[Requirement]:
         """
         Get a list of requirements for running the detector
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @classmethod
     @abstractmethod
     def get_distance(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> List[JsonDict]:
         """
         Takes of the ground truth processing strand as well as the prediction strand and generates the metric results.
 
         :param dataflow_gt: Dataflow with ground truth annotations.
         :param dataflow_predictions: Dataflow with predictions.
         :param categories:  DatasetCategories with respect to the underlying dataset.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @classmethod
     @abstractmethod
     def dump(
         cls, dataflow_gt: DataFlow, dataflow_predictions: DataFlow, categories: DatasetCategories
     ) -> Tuple[Any, Any]:
         """
         Dump the dataflow with ground truth annotations and predictions. Use it as auxiliary method and call it from
         `get_distance`.
 
         :param dataflow_gt: Dataflow with ground truth annotations.
         :param dataflow_predictions: Dataflow with predictions.
         :param categories: DatasetCategories with respect to the underlying dataset.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @classmethod
     def result_list_to_dict(cls, results: List[JsonDict]) -> JsonDict:
         """
         Converts the result from `get_distance` to a dict. It concatenates all keys of the inner dict and uses
         the metric result 'val' as value.
```

### Comparing `deepdoctection-0.30/deepdoctection/eval/cocometric.py` & `deepdoctection-0.31/deepdoctection/eval/cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/eval/eval.py` & `deepdoctection-0.31/deepdoctection/eval/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                         sub_cats,
                     )
                 else:
                     raise AttributeError(
                         "metric has no attribute sub_cats and cannot be used for token classification datasets"
                     )
             else:
-                raise NotImplementedError
+                raise NotImplementedError()
 
         else:
             self.wandb_table_agent = None
 
     @overload
     def run(
         self, output_as_dict: Literal[False] = False, **dataflow_build_kwargs: Union[str, int]
@@ -267,15 +267,15 @@
             summary_sub_cats_to_remove = meta_anns["summaries"]
             df_pr = MapData(df_pr, remove_cats(summary_sub_categories=summary_sub_cats_to_remove))
 
         elif self.dataset.dataset_info.type == DatasetType.token_classification:
             sub_cats_to_remove = meta_anns["sub_categories"]
             df_pr = MapData(df_pr, remove_cats(sub_categories=sub_cats_to_remove))
         else:
-            raise NotImplementedError
+            raise NotImplementedError()
 
         return df_pr
 
     def compare(self, interactive: bool = False, **kwargs: Union[str, int]) -> Optional[ImageType]:
         """
         Visualize ground truth and prediction datapoint. Given a dataflow config it will run predictions per sample
         and concat the prediction image (with predicted bounding boxes) with ground truth image.
```

### Comparing `deepdoctection-0.30/deepdoctection/eval/registry.py` & `deepdoctection-0.31/deepdoctection/eval/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/eval/tedsmetric.py` & `deepdoctection-0.31/deepdoctection/eval/tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/eval/tp_eval_callback.py` & `deepdoctection-0.31/deepdoctection/eval/tp_eval_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,18 +79,19 @@
         """
         self.dataset_name = dataset.dataset_info.name
         self.build_eval_kwargs = build_eval_kwargs
         self.in_names, self.out_names = in_names, out_names
         self.num_gpu = get_num_gpu()
         self.category_names = category_names
         self.sub_categories = sub_categories
-        assert isinstance(pipeline_component.predictor, TPFrcnnDetector), (
-            f"pipeline_component.predictor must be of "
-            f"type TPFrcnnDetector but is type {type(pipeline_component.predictor)}"
-        )
+        if not isinstance(pipeline_component.predictor, TPFrcnnDetector):
+            raise TypeError(
+                f"pipeline_component.predictor must be of type TPFrcnnDetector but is "
+                f"type {type(pipeline_component.predictor)}"
+            )
         self.cfg = pipeline_component.predictor.model.cfg
         if _use_replicated(self.cfg):
             self.evaluator = Evaluator(dataset, pipeline_component, metric, num_threads=self.num_gpu * 2)
         else:
             raise NotImplementedError("Can only evaluate in replicated training mode.")
 
     def _setup_graph(self) -> None:
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/__init__.py` & `deepdoctection-0.31/deepdoctection/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/base.py` & `deepdoctection-0.31/deepdoctection/extern/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 """
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 
 from ..utils.detection_types import ImageType, JsonDict, Requirement
+from ..utils.identifier import get_uuid_from_str
 from ..utils.settings import DefaultType, ObjectTypes, TypeOrStr, get_type
 
 
 class PredictorBase(ABC):
     """
     Abstract base class for all types of predictors (e.g. object detectors language models, ...)
     """
 
     name: str
+    model_id: str
 
     def __new__(cls, *args, **kwargs):  # type: ignore # pylint: disable=W0613
         requirements = cls.get_requirements()
         name = cls.__name__ if hasattr(cls, "__name__") else cls.__class__.__name__
         if not all(requirement[1] for requirement in requirements):
             raise ImportError(
                 "\n".join(
@@ -49,22 +51,30 @@
 
     @classmethod
     @abstractmethod
     def get_requirements(cls) -> List[Requirement]:
         """
         Get a list of requirements for running the detector
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def clone(self) -> "PredictorBase":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
+
+    def get_model_id(self) -> str:
+        """
+        Get the generating model
+        """
+        if self.name is not None:
+            return get_uuid_from_str(self.name)[:8]
+        raise ValueError("name must be set before calling get_model_id")
 
 
 @dataclass
 class DetectionResult:
     """
     Simple mutable storage for detection results.
 
@@ -98,14 +108,15 @@
     absolute_coords: bool = True
     class_name: ObjectTypes = DefaultType.default_type
     text: Optional[Union[str, ObjectTypes]] = None
     block: Optional[str] = None
     line: Optional[str] = None
     uuid: Optional[str] = None
     relationships: Optional[Dict[str, Any]] = None
+    angle: Optional[float] = None
 
 
 class ObjectDetector(PredictorBase):
     """
     Abstract base class for object detection. This can be anything ranging from layout detection to OCR.
     Use this to connect external detectors with Deep-Doctection predictors on images.
 
@@ -129,15 +140,15 @@
         self._categories = {key: get_type(value) for key, value in categories.items()}
 
     @abstractmethod
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @property
     def accepts_batch(self) -> bool:
         """
         whether to accept batches in `predict`
         """
         return False
@@ -170,22 +181,22 @@
         self._categories = {key: get_type(value) for key, value in categories.items()}
 
     @abstractmethod
     def predict(self, pdf_bytes: bytes) -> List[DetectionResult]:
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def get_width_height(self, pdf_bytes: bytes) -> Tuple[float, float]:
         """
         Abstract method get_width_height
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def clone(self) -> PredictorBase:
         return self.__class__()
 
     @property
     def accepts_batch(self) -> bool:
         """
@@ -208,15 +219,15 @@
     """
 
     @abstractmethod
     def predict(self, images: List[Tuple[str, ImageType]]) -> List[DetectionResult]:
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @property
     def accepts_batch(self) -> bool:
         """
         whether to accept batches in `predict`
         """
         return True
@@ -290,28 +301,28 @@
         self._categories = {key: get_type(value) for key, value in categories.items()}
 
     @abstractmethod
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:  # type: ignore
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def possible_tokens(self) -> List[ObjectTypes]:
         """
         Returns a list of possible detectable tokens
         """
         return list(self.categories.values())
 
     @abstractmethod
     def clone(self) -> "LMTokenClassifier":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @staticmethod
     def default_kwargs_for_input_mapping() -> JsonDict:
         """
         Add some default arguments that might be necessary when preparing a sample. Overwrite this method
         for some custom setting. `default_arguments_for_input_mapping` in `LMTokenClassifierService`.
         """
@@ -337,28 +348,28 @@
         self._categories = {key: get_type(value) for key, value in categories.items()}
 
     @abstractmethod
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:  # type: ignore
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def possible_categories(self) -> List[ObjectTypes]:
         """
         Returns a list of possible detectable categories for a sequence
         """
         return list(self.categories.values())
 
     @abstractmethod
     def clone(self) -> "LMSequenceClassifier":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @staticmethod
     def default_kwargs_for_input_mapping() -> JsonDict:
         """
         Add some default arguments that might be necessary when preparing a sample. Overwrite this method
         for some custom setting. `default_arguments_for_input_mapping` in `LMTokenClassifierService`.
         """
@@ -384,30 +395,45 @@
         self._categories = {key: get_type(value) for key, value in categories.items()}
 
     @abstractmethod
     def predict(self, text_string: str) -> DetectionResult:
         """
         Abstract method predict
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def possible_languages(self) -> List[ObjectTypes]:
         """
         Returns a list of possible detectable languages
         """
         return list(self.categories.values())
 
 
 class ImageTransformer(PredictorBase):
     """
     Abstract base class for transforming an image. The `transform` accepts and returns a numpy array
     """
 
     @abstractmethod
-    def transform(self, np_img: ImageType) -> ImageType:
+    def transform(self, np_img: ImageType, specification: DetectionResult) -> ImageType:
         """
         Abstract method transform
         """
-        raise NotImplementedError
+        raise NotImplementedError()
+
+    @abstractmethod
+    def predict(self, np_img: ImageType) -> DetectionResult:
+        """
+        Abstract method predict
+        """
+        raise NotImplementedError()
 
     def clone(self) -> PredictorBase:
         return self.__class__()
+
+    @staticmethod
+    @abstractmethod
+    def possible_category() -> ObjectTypes:
+        """
+        Returns a (single) category the `ImageTransformer` can predict
+        """
+        raise NotImplementedError()
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/d2detect.py` & `deepdoctection-0.31/deepdoctection/extern/d2detect.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 D2 GeneralizedRCNN model as predictor for deepdoctection pipeline
 """
 import io
+from abc import ABC
 from copy import copy
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Mapping, Optional, Sequence
 
 import numpy as np
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import (
     detectron2_available,
     get_detectron2_requirement,
     get_pytorch_requirement,
     pytorch_available,
 )
-from ..utils.metacfg import set_config_by_yaml
+from ..utils.metacfg import AttrDict, set_config_by_yaml
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from ..utils.transform import InferenceResize, ResizeTransform
 from .base import DetectionResult, ObjectDetector, PredictorBase
 from .pt.nms import batched_nms
 from .pt.ptutils import set_torch_auto_device
 
 if pytorch_available():
@@ -140,32 +141,99 @@
             np_boxes = np.expand_dims(np_boxes, axis=0)
     detect_result_list = []
     for box, label, score in zip(np_boxes, classes, scores):
         detect_result_list.append(DetectionResult(box=box.tolist(), class_id=label.item(), score=score.item()))
     return detect_result_list
 
 
-class D2FrcnnDetector(ObjectDetector):
+class D2FrcnnDetectorMixin(ObjectDetector, ABC):
+    """
+    Base class for D2 Faster-RCNN implementation. This class only implements the basic wrapper functions
+    """
+
+    def __init__(
+        self,
+        categories: Mapping[str, TypeOrStr],
+        filter_categories: Optional[Sequence[TypeOrStr]] = None,
+    ):
+        """
+        :param categories: A dict with key (indices) and values (category names). Index 0 must be reserved for a
+                           dummy 'BG' category. Note, that this convention is different from the builtin D2 framework,
+                           where models in the model zoo are trained with 'BG' class having the highest index.
+        :param filter_categories: The model might return objects that are not supposed to be predicted and that should
+                                  be filtered. Pass a list of category names that must not be returned
+        """
+
+        if filter_categories:
+            filter_categories = [get_type(cat) for cat in filter_categories]
+        self.filter_categories = filter_categories
+        self._categories_d2 = self._map_to_d2_categories(copy(categories))
+        self.categories = {idx: get_type(cat) for idx, cat in categories.items()}
+
+    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
+        """
+        Populating category names to detection results
+
+        :param detection_results: list of detection results. Will also filter categories
+        :return: List of detection results with attribute class_name populated
+        """
+        filtered_detection_result: List[DetectionResult] = []
+        for result in detection_results:
+            result.class_name = self._categories_d2[str(result.class_id)]
+            if isinstance(result.class_id, int):
+                result.class_id += 1
+            if self.filter_categories:
+                if result.class_name not in self.filter_categories:
+                    filtered_detection_result.append(result)
+            else:
+                filtered_detection_result.append(result)
+        return filtered_detection_result
+
+    @classmethod
+    def _map_to_d2_categories(cls, categories: Mapping[str, TypeOrStr]) -> Dict[str, ObjectTypes]:
+        return {str(int(k) - 1): get_type(v) for k, v in categories.items()}
+
+    def possible_categories(self) -> List[ObjectTypes]:
+        return list(self.categories.values())
+
+    @staticmethod
+    def get_inference_resizer(min_size_test: int, max_size_test: int) -> InferenceResize:
+        """Returns the resizer for the inference
+
+        :param min_size_test: minimum size of the resized image
+        :param max_size_test: maximum size of the resized image
+        """
+        return InferenceResize(min_size_test, max_size_test)
+
+    @staticmethod
+    def get_name(path_weights: str, architecture: str) -> str:
+        """Returns the name of the model"""
+        return f"detectron2_{architecture}" + "_".join(Path(path_weights).parts[-2:])
+
+
+class D2FrcnnDetector(D2FrcnnDetectorMixin):
     """
     D2 Faster-RCNN implementation with all the available backbones, normalizations throughout the model
     as well as FPN, optional Cascade-RCNN and many more.
 
     Currently, masks are not included in the data model.
 
     There are no adjustment to the original implementation of Detectron2. Only one post-processing step is followed by
     the standard D2 output that takes into account of the situation that detected objects are disjoint. For more infos
     on this topic, see <https://github.com/facebookresearch/detectron2/issues/978> .
 
+    ```python
         config_path = ModelCatalog.get_full_path_configs("dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml")
         weights_path = ModelDownloadManager.maybe_download_weights_and_configs("item/d2_model-800000-layout.pkl")
         categories = ModelCatalog.get_profile("item/d2_model-800000-layout.pkl").categories
 
         d2_predictor = D2FrcnnDetector(config_path,weights_path,categories,device="cpu")
 
         detection_results = d2_predictor.predict(bgr_image_np_array)
+    ```
     """
 
     def __init__(
         self,
         path_yaml: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
@@ -187,38 +255,35 @@
                            where models in the model zoo are trained with 'BG' class having the highest index.
         :param config_overwrite:  Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
         :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
         :param filter_categories: The model might return objects that are not supposed to be predicted and that should
                                   be filtered. Pass a list of category names that must not be returned
         """
+        super().__init__(categories, filter_categories)
 
-        self.name = "_".join(Path(path_weights).parts[-3:])
-        self._categories_d2 = self._map_to_d2_categories(copy(categories))
         self.path_weights = path_weights
-        d2_conf_list = ["MODEL.WEIGHTS", path_weights]
-        config_overwrite = config_overwrite if config_overwrite else []
-        for conf in config_overwrite:
-            key, val = conf.split("=", maxsplit=1)
-            d2_conf_list.extend([key, val])
-
         self.path_yaml = path_yaml
-        self.categories = copy(categories)  # type: ignore
+
+        config_overwrite = config_overwrite if config_overwrite else []
         self.config_overwrite = config_overwrite
         if device is not None:
             self.device = device
         else:
             self.device = set_torch_auto_device()
-        if filter_categories:
-            filter_categories = [get_type(cat) for cat in filter_categories]
-        self.filter_categories = filter_categories
+
+        d2_conf_list = self._get_d2_config_list(path_weights, config_overwrite)
         self.cfg = self._set_config(path_yaml, d2_conf_list, device)
-        self.d2_predictor = D2FrcnnDetector.set_model(self.cfg)
-        self.resizer = InferenceResize(self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
-        self._instantiate_d2_predictor()
+
+        self.name = self.get_name(path_weights, self.cfg.MODEL.META_ARCHITECTURE)
+        self.model_id = self.get_model_id()
+
+        self.d2_predictor = self._set_model(self.cfg)
+        self._instantiate_d2_predictor(self.d2_predictor, path_weights)
+        self.resizer = self.get_inference_resizer(self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
 
     @staticmethod
     def _set_config(
         path_yaml: str, d2_conf_list: List[str], device: Optional[Literal["cpu", "cuda"]] = None
     ) -> "CfgNode":
         cfg = get_cfg()
         # additional attribute with default value, so that the true value can be loaded from the configs
@@ -227,26 +292,27 @@
         cfg.merge_from_list(d2_conf_list)
         if not torch.cuda.is_available() or device == "cpu":
             cfg.MODEL.DEVICE = "cpu"
         cfg.freeze()
         return cfg
 
     @staticmethod
-    def set_model(config: "CfgNode") -> "GeneralizedRCNN":
+    def _set_model(config: "CfgNode") -> "GeneralizedRCNN":
         """
         Build the D2 model. It uses the available builtin tools of D2
 
         :param config: Model config
         :return: The GeneralizedRCNN model
         """
         return build_model(config.clone()).eval()
 
-    def _instantiate_d2_predictor(self) -> None:
-        checkpointer = DetectionCheckpointer(self.d2_predictor)
-        checkpointer.load(self.cfg.MODEL.WEIGHTS)
+    @staticmethod
+    def _instantiate_d2_predictor(wrapped_model: "GeneralizedRCNN", path_weights: str) -> None:
+        checkpointer = DetectionCheckpointer(wrapped_model)
+        checkpointer.load(path_weights)
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Prediction per image.
 
         :param np_img: image as numpy array
         :return: A list of DetectionResult
@@ -255,74 +321,94 @@
             np_img,
             self.d2_predictor,
             self.resizer,
             self.cfg.NMS_THRESH_CLASS_AGNOSTIC,
         )
         return self._map_category_names(detection_results)
 
-    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
-        """
-        Populating category names to detection results
-
-        :param detection_results: list of detection results. Will also filter categories
-        :return: List of detection results with attribute class_name populated
-        """
-        filtered_detection_result: List[DetectionResult] = []
-        for result in detection_results:
-            result.class_name = self._categories_d2[str(result.class_id)]
-            if isinstance(result.class_id, int):
-                result.class_id += 1
-            if self.filter_categories:
-                if result.class_name not in self.filter_categories:
-                    filtered_detection_result.append(result)
-            else:
-                filtered_detection_result.append(result)
-        return filtered_detection_result
-
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_detectron2_requirement()]
 
-    @classmethod
-    def _map_to_d2_categories(cls, categories: Mapping[str, TypeOrStr]) -> Dict[str, ObjectTypes]:
-        return {str(int(k) - 1): get_type(v) for k, v in categories.items()}
-
     def clone(self) -> PredictorBase:
         return self.__class__(
             self.path_yaml,
             self.path_weights,
             self.categories,
             self.config_overwrite,
             self.device,
             self.filter_categories,
         )
 
-    def possible_categories(self) -> List[ObjectTypes]:
-        return list(self.categories.values())
+    @staticmethod
+    def get_wrapped_model(
+        path_yaml: str, path_weights: str, config_overwrite: List[str], device: Literal["cpu", "cuda"]
+    ) -> "GeneralizedRCNN":
+        """
+        Get the wrapped model. Useful if one do not want to build the wrapper but only needs the instantiated model.
+
+        Example:
+        ```python
+
+            path_yaml = ModelCatalog.get_full_path_configs("dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml")
+            weights_path = ModelDownloadManager.maybe_download_weights_and_configs("item/d2_model-800000-layout.pkl")
+            model = D2FrcnnDetector.get_wrapped_model(path_yaml,weights_path,["OUTPUT.FRCNN_NMS_THRESH=0.3",
+                                                                              "OUTPUT.RESULT_SCORE_THRESH=0.6"],
+                                                                              "cpu")
+            detect_result_list = d2_predict_image(np_img,model,InferenceResize(800,1333),0.3)
+        ```
+        :param path_yaml: The path to the yaml config. If the model is built using several config files, always use
+                          the highest level .yaml file.
+        :param path_weights: The path to the model checkpoint.
+        :param config_overwrite: Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
+                                 ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
+        :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
+        :return: Detectron2 GeneralizedRCNN model
+        """
 
+        if device is None:
+            device = set_torch_auto_device()
+        d2_conf_list = D2FrcnnDetector._get_d2_config_list(path_weights, config_overwrite)
+        cfg = D2FrcnnDetector._set_config(path_yaml, d2_conf_list, device)
+        model = D2FrcnnDetector._set_model(cfg)
+        D2FrcnnDetector._instantiate_d2_predictor(model, path_weights)
+        return model
 
-class D2FrcnnTracingDetector(ObjectDetector):
+    @staticmethod
+    def _get_d2_config_list(path_weights: str, config_overwrite: List[str]) -> List[str]:
+        d2_conf_list = ["MODEL.WEIGHTS", path_weights]
+        config_overwrite = config_overwrite if config_overwrite else []
+        for conf in config_overwrite:
+            key, val = conf.split("=", maxsplit=1)
+            d2_conf_list.extend([key, val])
+        return d2_conf_list
+
+
+class D2FrcnnTracingDetector(D2FrcnnDetectorMixin):
     """
     D2 Faster-RCNN exported torchscript model. Using this predictor has the advantage that Detectron2 does not have to
     be installed. The associated config setting only contains parameters that are involved in pre-and post-processing.
     Depending on running the model with CUDA or on a CPU, it will need the appropriate exported model.
 
     Currently, masks are not included in the data model.
 
     There are no adjustment to the original implementation of Detectron2. Only one post-processing step is followed by
     the standard D2 output that takes into account of the situation that detected objects are disjoint. For more infos
     on this topic, see <https://github.com/facebookresearch/detectron2/issues/978> .
 
+    Example:
+    ```python
         config_path = ModelCatalog.get_full_path_configs("dd/d2/item/CASCADE_RCNN_R_50_FPN_GN.yaml")
         weights_path = ModelDownloadManager.maybe_download_weights_and_configs("item/d2_model-800000-layout.pkl")
         categories = ModelCatalog.get_profile("item/d2_model-800000-layout.pkl").categories
 
         d2_predictor = D2FrcnnDetector(config_path,weights_path,categories)
 
         detection_results = d2_predictor.predict(bgr_image_np_array)
+    ```
     """
 
     def __init__(
         self,
         path_yaml: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
@@ -339,35 +425,36 @@
                            dummy 'BG' category. Note, that this convention is different from the builtin D2 framework,
                            where models in the model zoo are trained with 'BG' class having the highest index.
         :param config_overwrite:  Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"].
         :param filter_categories: The model might return objects that are not supposed to be predicted and that should
                                   be filtered. Pass a list of category names that must not be returned
         """
-        self.name = "_".join(Path(path_weights).parts[-2:])
-        self._categories_d2 = self._map_to_d2_categories(copy(categories))
+
+        super().__init__(categories, filter_categories)
+
         self.path_weights = path_weights
         self.path_yaml = path_yaml
-        self.categories = copy(categories)  # type: ignore
-        self.config_overwrite = config_overwrite
-        if filter_categories:
-            filter_categories = [get_type(cat) for cat in filter_categories]
-        self.filter_categories = filter_categories
-        self.cfg = set_config_by_yaml(self.path_yaml)
+
+        self.config_overwrite = copy(config_overwrite)
+        self.cfg = self._set_config(self.path_yaml, self.path_weights, self.config_overwrite)
+
+        self.name = self.get_name(path_weights, self.cfg.MODEL.META_ARCHITECTURE)
+        self.model_id = self.get_model_id()
+
+        self.resizer = self.get_inference_resizer(self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
+        self.d2_predictor = self.get_wrapped_model(self.path_weights)
+
+    @staticmethod
+    def _set_config(path_yaml: str, path_weights: str, config_overwrite: Optional[List[str]]) -> AttrDict:
+        cfg = set_config_by_yaml(path_yaml)
         config_overwrite = config_overwrite if config_overwrite else []
         config_overwrite.extend([f"MODEL.WEIGHTS={path_weights}"])
-        self.cfg.update_args(config_overwrite)
-        self.resizer = InferenceResize(self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
-        self.d2_predictor = self._instantiate_d2_predictor()
-
-    def _instantiate_d2_predictor(self) -> Any:
-        with open(self.path_weights, "rb") as file:
-            buffer = io.BytesIO(file.read())
-        # Load all tensors to the original device
-        return torch.jit.load(buffer)
+        cfg.update_args(config_overwrite)
+        return cfg
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Prediction per image.
 
         :param np_img: image as numpy array
         :return: A list of DetectionResult
@@ -414,7 +501,20 @@
                     filtered_detection_result.append(result)
             else:
                 filtered_detection_result.append(result)
         return filtered_detection_result
 
     def possible_categories(self) -> List[ObjectTypes]:
         return list(self.categories.values())
+
+    @staticmethod
+    def get_wrapped_model(path_weights: str) -> Any:
+        """
+        Get the wrapped model. Useful if one do not want to build the wrapper but only needs the instantiated model.
+
+        :param path_weights:
+        :return:
+        """
+        with open(path_weights, "rb") as file:
+            buffer = io.BytesIO(file.read())
+        # Load all tensors to the original device
+        return torch.jit.load(buffer)
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/doctrocr.py` & `deepdoctection-0.31/deepdoctection/train/d2_frcnn_train.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# File: doctrocr.py
+# File: d2_frcnn_train.py
 
 # Copyright 2021 Dr. Janis Meyer. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,333 +12,385 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Deepdoctection wrappers for DocTr OCR text line detection and text recognition models
+Module for training Detectron2 `GeneralizedRCNN`
 """
 
-from pathlib import Path
-from typing import Any, List, Literal, Mapping, Optional, Tuple
-from zipfile import ZipFile
-
-from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import (
-    doctr_available,
-    get_doctr_requirement,
-    get_pytorch_requirement,
-    get_tensorflow_requirement,
-    get_tf_addons_requirements,
-    pytorch_available,
-    tf_addons_available,
-    tf_available,
-)
-from ..utils.fs import load_json
-from ..utils.settings import LayoutType, ObjectTypes, TypeOrStr
-from .base import DetectionResult, ObjectDetector, PredictorBase, TextRecognizer
-from .pt.ptutils import set_torch_auto_device
-
-if doctr_available() and ((tf_addons_available() and tf_available()) or pytorch_available()):
-    from doctr.models.detection.predictor import DetectionPredictor  # pylint: disable=W0611
-    from doctr.models.detection.zoo import detection_predictor
-    from doctr.models.preprocessor import PreProcessor
-    from doctr.models.recognition.predictor import RecognitionPredictor  # pylint: disable=W0611
-    from doctr.models.recognition.zoo import ARCHS, recognition
-
-if pytorch_available():
-    import torch
-
-if tf_available():
-    import tensorflow as tf  # type: ignore  # pylint: disable=E0401
-
-
-def _set_device_str(device: Optional[str] = None) -> str:
-    if device is not None:
-        if tf_available():
-            device = "/" + device.replace("cuda", "gpu") + ":0"
-    elif pytorch_available():
-        device = set_torch_auto_device()
-    else:
-        device = "/gpu:0"  # we impose to install tensorflow-gpu because of Tensorpack models
-    return device
-
-
-def _load_model(path_weights: str, doctr_predictor: Any, device: str, lib: str) -> None:
-    if lib == "PT" and pytorch_available():
-        state_dict = torch.load(path_weights, map_location=device)
-        for key in list(state_dict.keys()):
-            state_dict["model." + key] = state_dict.pop(key)
-        doctr_predictor.load_state_dict(state_dict)
-        doctr_predictor.to(device)
-    elif lib == "TF" and tf_available():
-        # Unzip the archive
-        params_path = Path(path_weights).parent
-        is_zip_path = path_weights.endswith(".zip")
-        if is_zip_path:
-            with ZipFile(path_weights, "r") as file:
-                file.extractall(path=params_path)
-                doctr_predictor.model.load_weights(params_path / "weights")
-        else:
-            doctr_predictor.model.load_weights(path_weights)
-
 
-def doctr_predict_text_lines(np_img: ImageType, predictor: "DetectionPredictor", device: str) -> List[DetectionResult]:
-    """
-    Generating text line DetectionResult based on Doctr DetectionPredictor.
+import copy
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Type, Union
 
-    :param np_img: Image in np.array.
-    :param predictor: `doctr.models.detection.predictor.DetectionPredictor`
-    :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
-    :return: A list of text line detection results (without text).
-    """
-    if tf_available() and device is not None:
-        with tf.device(device):
-            raw_output = predictor([np_img])
-    else:
-        raw_output = predictor([np_img])
-    detection_results = [
-        DetectionResult(
-            box=box[:4].tolist(), class_id=1, score=box[4], absolute_coords=False, class_name=LayoutType.word
-        )
-        for box in raw_output[0]["words"]
-    ]
-    return detection_results
+from detectron2.config import CfgNode, get_cfg
+from detectron2.data import DatasetMapper, build_detection_train_loader
+from detectron2.data.transforms import RandomFlip, ResizeShortestEdge
+from detectron2.engine import DefaultTrainer, HookBase, default_writers, hooks
+from detectron2.utils import comm
+from detectron2.utils.events import EventWriter, get_event_storage
+from fvcore.nn.precise_bn import get_bn_modules  # type: ignore
+from torch.utils.data import DataLoader, IterableDataset
+
+from ..datasets.adapter import DatasetAdapter
+from ..datasets.base import DatasetBase
+from ..datasets.registry import get_dataset
+from ..eval.base import MetricBase
+from ..eval.eval import Evaluator
+from ..eval.registry import metric_registry
+from ..extern.d2detect import D2FrcnnDetector
+from ..extern.pt.ptutils import get_num_gpu
+from ..mapper.d2struct import image_to_d2_frcnn_training
+from ..pipe.base import PredictorPipelineComponent
+from ..pipe.registry import pipeline_component_registry
+from ..utils.error import DependencyError
+from ..utils.file_utils import get_wandb_requirement, wandb_available
+from ..utils.logger import LoggingRecord, logger
+from ..utils.utils import string_to_dict
+
+if wandb_available():
+    import wandb
+
+
+def _set_config(
+    path_config_yaml: str,
+    conf_list: List[str],
+    dataset_train: DatasetBase,
+    dataset_val: Optional[DatasetBase],
+    metric_name: Optional[str],
+    metric: Optional[Union[Type[MetricBase], MetricBase]],
+    pipeline_component_name: Optional[str],
+) -> CfgNode:
+    cfg = get_cfg()
+    cfg.defrost()
+    cfg.NMS_THRESH_CLASS_AGNOSTIC = 0.01
+    cfg.DATASETS.TRAIN = (dataset_train.dataset_info.name,)
+    cfg.WANDB = CfgNode()
+    cfg.WANDB.USE_WANDB = False
+    cfg.WANDB.PROJECT = None
+    cfg.WANDB.REPO = "deepdoctection"
+    cfg.merge_from_file(path_config_yaml)
+    cfg.merge_from_list(conf_list)
+
+    cfg.TEST.DO_EVAL = (
+        cfg.TEST.EVAL_PERIOD > 0
+        and dataset_val is not None
+        and (metric_name is not None or metric is not None)
+        and pipeline_component_name is not None
+    )
+    if cfg.TEST.DO_EVAL:
+        cfg.DATASETS.TEST = (dataset_val.dataset_info.name,)  # type: ignore
+    cfg.freeze()
+    return cfg
+
+
+def _update_for_eval(config_overwrite: List[str]) -> List[str]:
+    ret = [item for item in config_overwrite if not "WANDB" in item]
+    return ret
 
 
-def doctr_predict_text(
-    inputs: List[Tuple[str, ImageType]], predictor: "RecognitionPredictor", device: str
-) -> List[DetectionResult]:
+class WandbWriter(EventWriter):
     """
-    Calls Doctr text recognition model on a batch of numpy arrays (text lines predicted from a text line detector) and
-    returns the recognized text as DetectionResult
-
-    :param inputs: list of tuples containing the annotation_id of the input image and the numpy array of the cropped
-                   text line
-    :param predictor: `doctr.models.detection.predictor.RecognitionPredictor`
-    :param device: Will only be used in tensorflow settings. Either /gpu:0 or /cpu:0
-    :return: A list of DetectionResult containing recognized text.
+    Write all scalars to a wandb tool.
     """
 
-    uuids, images = list(zip(*inputs))
-    if tf_available() and device is not None:
-        with tf.device(device):
-            raw_output = predictor(list(images))
-    else:
-        raw_output = predictor(list(images))
-    detection_results = [
-        DetectionResult(score=output[1], text=output[0], uuid=uuid) for uuid, output in zip(uuids, raw_output)
-    ]
-    return detection_results
-
+    def __init__(
+        self,
+        project: str,
+        repo: str,
+        config: Optional[Union[Dict[str, Any], CfgNode]] = None,
+        window_size: int = 20,
+        **kwargs: Any,
+    ):
+        """
+        :param project: W&B Project name
+        :param config: the project level configuration object
+        :param window_size: the scalars will be median-smoothed by this window size
+        :param kwargs: other arguments passed to `wandb.init(...)`
+        """
+        if config is None:
+            config = {}
+        self._window_size = window_size
+        self._run = wandb.init(project=project, config=config, **kwargs) if not wandb.run else wandb.run
+        self._run._label(repo=repo)  # type:ignore
 
-class DoctrTextlineDetector(ObjectDetector):
-    """
-    A deepdoctection wrapper of DocTr text line detector. We model text line detection as ObjectDetector
-    and assume to use this detector in a ImageLayoutService.
-    DocTr supports several text line detection implementations but provides only a subset of pre-trained models.
-    The most usable one for document OCR for which a pre-trained model exists is DBNet as described in “Real-time Scene
-    Text Detection with Differentiable Binarization”, with a ResNet-50 backbone. This model can be used in either
-    Tensorflow or PyTorch.
-    Some other pre-trained models exist that have not been registered in `ModelCatalog`. Please check the DocTr library
-    and organize the download of the pre-trained model by yourself.
-
-    **Example:**
-
-                 path_weights_tl = ModelDownloadManager.maybe_download_weights_and_configs("doctr/db_resnet50/pt
-                 /db_resnet50-ac60cadc.pt")
-                 # Use "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip" for Tensorflow
-
-                 categories = ModelCatalog.get_profile("doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt").categories
-                 det = DoctrTextlineDetector("db_resnet50",path_weights_tl,categories,"cpu")
-                 layout = ImageLayoutService(det,to_image=True, crop_image=True)
-
-                 path_weights_tr = dd.ModelDownloadManager.maybe_download_weights_and_configs("doctr/crnn_vgg16_bn
-                 /pt/crnn_vgg16_bn-9762b0b0.pt")
-                 rec = DoctrTextRecognizer("crnn_vgg16_bn", path_weights_tr, "cpu")
-                 text = TextExtractionService(rec, extract_from_roi="word")
+    def write(self) -> None:
+        storage = get_event_storage()
 
-                 analyzer = DoctectionPipe(pipeline_component_list=[layout,text])
+        log_dict = {}
+        for key, (val, _) in storage.latest_with_smoothing_hint(self._window_size).items():
+            log_dict[key] = val
 
-                 path = "/path/to/image_dir"
-                 df = analyzer.analyze(path = path)
+        self._run.log(log_dict)  # type:ignore
 
-                 for dp in df:
-                     ...
+    def close(self) -> None:
+        self._run.finish()  # type:ignore
 
 
+class D2Trainer(DefaultTrainer):
+    """
+    Detectron2 `DefaultTrainer` with some custom method for handling datasets and running evaluation. The setting is
+    made to train standard models in detectron2.
     """
 
-    def __init__(
-        self,
-        architecture: str,
-        path_weights: str,
-        categories: Mapping[str, TypeOrStr],
-        device: Optional[Literal["cpu", "cuda"]] = None,
-        lib: str = "TF",
-    ) -> None:
-        self.lib = lib
-        self.name = "doctr_text_detector"
-        self.architecture = architecture
-        self.path_weights = path_weights
-        self.doctr_predictor = detection_predictor(
-            arch=self.architecture, pretrained=False, pretrained_backbone=False
-        )  # we will be loading the model
-        # later because there is no easy way in doctr to load a model by giving only a path to its weights
-        self.categories = categories  # type: ignore
-        self.device_input = device
-        self.device = _set_device_str(device)
-        self.load_model()
-
-    def predict(self, np_img: ImageType) -> List[DetectionResult]:
-        """
-        Prediction per image.
+    def __init__(self, cfg: CfgNode, torch_dataset: IterableDataset[Any], mapper: DatasetMapper) -> None:
+        self.dataset = torch_dataset
+        self.mapper = mapper
+        self.evaluator: Optional[Evaluator] = None
+        self.build_val_dict: Mapping[str, str] = {}
+        super().__init__(cfg)
 
-        :param np_img: image as numpy array
-        :return: A list of DetectionResult
+    def build_hooks(self) -> List[HookBase]:
         """
-        detection_results = doctr_predict_text_lines(np_img, self.doctr_predictor, self.device)
-        return detection_results
+        Overwritten from DefaultTrainer. This ensures that the EvalHook is being called before the writer and
+        all metrics are being written to JSON, Tensorboard etc.
 
-    @classmethod
-    def get_requirements(cls) -> List[Requirement]:
-        if tf_available():
-            return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
-        if pytorch_available():
-            return [get_pytorch_requirement(), get_doctr_requirement()]
-        raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextlineDetector")
+        :return: list[HookBase]
+        """
+        cfg = self.cfg.clone()
+        cfg.defrost()
+        cfg.DATALOADER.NUM_WORKERS = 0  # save some memory and time for PreciseBN
+
+        ret = [
+            hooks.IterationTimer(),
+            hooks.LRScheduler(),
+            (
+                hooks.PreciseBN(
+                    # Run at the same freq as (but before) evaluation.
+                    cfg.TEST.EVAL_PERIOD,
+                    self.model,  # pylint: disable=E1101
+                    # Build a new data loader to not affect training
+                    self.build_train_loader(cfg),
+                    cfg.TEST.PRECISE_BN.NUM_ITER,
+                )
+                if cfg.TEST.PRECISE_BN.ENABLED and get_bn_modules(self.model)  # pylint: disable=E1101
+                else None
+            ),
+        ]
+
+        # Do PreciseBN before checkpointer, because it updates the model and need to
+        # be saved by checkpointer.
+        # This is not always the best: if checkpointing has a different frequency,
+        # some checkpoints may have more precise statistics than others.
+        if comm.is_main_process():
+            ret.append(hooks.PeriodicCheckpointer(self.checkpointer, cfg.SOLVER.CHECKPOINT_PERIOD))
+
+        # Do evaluation after checkpointer, because then if it fails,
+        # we can use the saved checkpoint to debug.
+        if self.cfg.TEST.DO_EVAL:
+            ret.append(
+                hooks.EvalHook(
+                    cfg.TEST.EVAL_PERIOD,
+                    lambda: self.eval_with_dd_evaluator(**self.build_val_dict),  # pylint: disable=W0108
+                )
+            )
+
+        if comm.is_main_process():
+            # Here the default print/log frequency of each writer is used.
+            # run writers in the end, so that evaluation metrics are written
+            ret.append(hooks.PeriodicWriter(self.build_writers(), period=20))
 
-    def clone(self) -> PredictorBase:
-        return self.__class__(self.architecture, self.path_weights, self.categories, self.device_input, self.lib)
+        return ret
 
-    def possible_categories(self) -> List[ObjectTypes]:
-        return [LayoutType.word]
+    def build_writers(self) -> List[EventWriter]:
+        """
+        Build a list of writers to be using `default_writers()`.
+        If you'd like a different list of writers, you can overwrite it in
+        your trainer.
 
-    def load_model(self) -> None:
-        """Loading model weights"""
-        _load_model(self.path_weights, self.doctr_predictor, self.device, self.lib)
+        :return: A list of `EventWriter` objects.
+        """
+        writers_list = default_writers(self.cfg.OUTPUT_DIR, self.max_iter)
+        if self.cfg.WANDB.USE_WANDB:
+            _, _wandb_available, err_msg = get_wandb_requirement()
+            if not _wandb_available:
+                raise DependencyError(err_msg)
+            if self.cfg.WANDB.PROJECT is None:
+                raise ValueError("When using W&B, you must specify a project, i.e. WANDB.PROJECT")
+            writers_list.append(WandbWriter(self.cfg.WANDB.PROJECT, self.cfg.WANDB.REPO, self.cfg))
+        return writers_list
 
+    def build_train_loader(self, cfg: CfgNode) -> DataLoader[Any]:  # pylint: disable=W0221
+        """
+        Overwritten method from `DefaultTrainer`.
 
-class DoctrTextRecognizer(TextRecognizer):
-    """
-    A deepdoctection wrapper of DocTr text recognition predictor. The base class is a TextRecognizer that takes
-    a batch of sub images (e.g. text lines from a text detector) and returns a list with text spotted in the sub images.
-    DocTr supports several text recognition models but provides only a subset of pre-trained models.
+        :param cfg: Configuration
+        :return: The data loader for a given dataset adapter, mapper.
+        """
+        return build_detection_train_loader(
+            dataset=self.dataset, mapper=self.mapper, total_batch_size=cfg.SOLVER.IMS_PER_BATCH
+        )
 
-    This model that is most suitable for document text recognition is the CRNN implementation with a VGG-16 backbone as
-    described in “An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to
-    Scene Text Recognition”. It can be used in either Tensorflow or PyTorch.
+    def eval_with_dd_evaluator(self, **build_eval_kwargs: str) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
+        """
+        Running the Evaluator. This method will be called from the `EvalHook`
 
-    For more details please check the official DocTr documentation by Mindee: https://mindee.github.io/doctr/
+        :param build_eval_kwargs: dataflow eval config kwargs of the underlying dataset
+        :return: A dict of evaluation results
+        """
+        assert self.evaluator is not None
+        assert self.evaluator.pipe_component is not None
+        for comp in self.evaluator.pipe_component.pipe_components:
+            comp.predictor.d2_predictor = copy.deepcopy(self.model).eval()  # type: ignore # pylint: disable=E1101
+        scores = self.evaluator.run(True, **build_eval_kwargs)
+        return scores
 
-    **Example:**
+    def setup_evaluator(
+        self,
+        dataset_val: DatasetBase,
+        pipeline_component: PredictorPipelineComponent,
+        metric: Union[Type[MetricBase], MetricBase],
+        build_val_dict: Optional[Mapping[str, str]] = None,
+    ) -> None:
+        """
+        Setup of evaluator before starting training. During training, predictors will be replaced by current
+        checkpoints.
 
-                 path_weights_tl = ModelDownloadManager.maybe_download_weights_and_configs("doctr/db_resnet50/pt
-                 /db_resnet50-ac60cadc.pt")
-                 # Use "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip" for Tensorflow
+        :param dataset_val: dataset on which to run evaluation
+        :param pipeline_component: pipeline component to plug into the evaluator
+        :param metric: A metric class
+        :param build_val_dict: evaluation dataflow build config
+        """
+        if wandb_available():
+            run = wandb.run if wandb.run is not None else None
+        else:
+            run = None
+        self.evaluator = Evaluator(
+            dataset_val,
+            pipeline_component,
+            metric,
+            num_threads=get_num_gpu() * 2,
+            run=run,
+        )
+        if build_val_dict:
+            self.build_val_dict = build_val_dict
+        assert self.evaluator.pipe_component
+        for comp in self.evaluator.pipe_component.pipe_components:
+            assert isinstance(comp, PredictorPipelineComponent)
+            assert isinstance(comp.predictor, D2FrcnnDetector)
+            comp.predictor.d2_predictor = None
 
-                 categories = ModelCatalog.get_profile("doctr/db_resnet50/pt/db_resnet50-ac60cadc.pt").categories
-                 det = DoctrTextlineDetector("db_resnet50",path_weights_tl,categories,"cpu")
-                 layout = ImageLayoutService(det,to_image=True, crop_image=True)
+    @classmethod
+    def build_evaluator(cls, cfg, dataset_name):  # type: ignore
+        raise NotImplementedError()
 
-                 path_weights_tr = dd.ModelDownloadManager.maybe_download_weights_and_configs("doctr/crnn_vgg16_bn
-                 /pt/crnn_vgg16_bn-9762b0b0.pt")
-                 rec = DoctrTextRecognizer("crnn_vgg16_bn", path_weights_tr, "cpu")
-                 text = TextExtractionService(rec, extract_from_roi="word")
 
-                 analyzer = DoctectionPipe(pipeline_component_list=[layout,text])
+def train_d2_faster_rcnn(
+    path_config_yaml: str,
+    dataset_train: Union[str, DatasetBase],
+    path_weights: str,
+    config_overwrite: Optional[List[str]] = None,
+    log_dir: str = "train_log/frcnn",
+    build_train_config: Optional[Sequence[str]] = None,
+    dataset_val: Optional[DatasetBase] = None,
+    build_val_config: Optional[Sequence[str]] = None,
+    metric_name: Optional[str] = None,
+    metric: Optional[Union[Type[MetricBase], MetricBase]] = None,
+    pipeline_component_name: Optional[str] = None,
+) -> None:
+    """
+    Adaptation of <https://github.com/facebookresearch/detectron2/blob/main/tools/train_net.py> for training Detectron2
+    standard models
 
-                 path = "/path/to/image_dir"
-                 df = analyzer.analyze(path = path)
+    Train Detectron2 from scratch or fine-tune a model using this API. Compared to Tensorpack this framework trains much
+    faster, e.g. <https://detectron2.readthedocs.io/en/latest/notes/benchmarks.html> .
 
-                 for dp in df:
-                     ...
+    This training script is devoted to the case where one cluster with one GPU is available. To run on several machines
+    with more than one GPU use `detectron2.engine.launch` .
 
+        if __name__ == "__main__":
+
+                launch(train_d2_faster_rcnn,
+                       num_gpus,
+                       num_machines,
+                       machine_rank,
+                       dist_url,
+                       args=(path_config_yaml,
+                             path_weights,
+                             config_overwrite,
+                             log_dir,
+                             build_train_config,
+                             dataset_val,
+                             build_val_config,
+                             metric_name,
+                             metric,
+                             pipeline_component_name),)
+
+
+    :param path_config_yaml: path to a D2 config file. Check
+                             https://github.com/facebookresearch/detectron2/blob/main/detectron2/config/defaults.py
+                             for various settings.
+    :param dataset_train: the dataset to use for training.
+    :param path_weights: path to a checkpoint, if you want to continue training or fine-tune. Will train from scratch if
+                         an empty string is passed
+    :param config_overwrite: Pass a list of arguments if some configs from the .yaml file should be replaced. Use the
+                             list convention, e.g. ['TRAIN.STEPS_PER_EPOCH=500', 'OUTPUT.RESULT_SCORE_THRESH=0.4']
+    :param log_dir: Path to log dir. Will default to `train_log/frcnn`
+    :param build_train_config: dataflow build setting. Again, use list convention setting, e.g. ['max_datapoints=1000']
+    :param dataset_val: the dataset to use for validation.
+    :param build_val_config: same as `build_train_config` but for validation
+    :param metric_name: A metric name to choose for validation. Will use the default setting. If you want a custom
+                        metric setting, pass a metric explicitly.
+    :param metric: A metric to choose for validation.
+    :param pipeline_component_name: A pipeline component name to use for validation.
     """
 
-    def __init__(
-        self,
-        architecture: str,
-        path_weights: str,
-        device: Optional[Literal["cpu", "cuda"]] = None,
-        lib: str = "TF",
-        path_config_json: Optional[str] = None,
-    ) -> None:
-        """
-        :param architecture: DocTR supports various text recognition models, e.g. "crnn_vgg16_bn",
-        "crnn_mobilenet_v3_small". The full list can be found here:
-        https://github.com/mindee/doctr/blob/main/doctr/models/recognition/zoo.py#L16.
-        :param path_weights: Path to the weights of the model
-        :param device: "cpu" or "cuda". Will default to "cuda" if the required hardware is available.
-        :param lib: "TF" or "PT". Will default to "TF".
-        :param path_config_json: Path to a json file containing the configuration of the model. Useful, if you have
-        a model trained on custom vocab.
-        """
-        self.lib = lib
-        self.name = "doctr_text_recognizer"
-        self.architecture = architecture
-        self.path_weights = path_weights
-        self.device_input = device
-        self.device = _set_device_str(device)
-        self.path_config_json = path_config_json
-        self.doctr_predictor = self.build_model()
-        self.load_model()
-
-    def predict(self, images: List[Tuple[str, ImageType]]) -> List[DetectionResult]:
-        """
-        Prediction on a batch of text lines
-
-        :param images: list of tuples with the annotation_id of the sub image and a numpy array
-        :return: A list of DetectionResult
-        """
-        if images:
-            return doctr_predict_text(images, self.doctr_predictor, self.device)
-        return []
-
-    @classmethod
-    def get_requirements(cls) -> List[Requirement]:
-        if tf_available():
-            return [get_tensorflow_requirement(), get_doctr_requirement(), get_tf_addons_requirements()]
-        if pytorch_available():
-            return [get_pytorch_requirement(), get_doctr_requirement()]
-        raise ModuleNotFoundError("Neither Tensorflow nor PyTorch has been installed. Cannot use DoctrTextRecognizer")
-
-    def clone(self) -> PredictorBase:
-        return self.__class__(self.architecture, self.path_weights, self.device_input, self.lib)
-
-    def load_model(self) -> None:
-        """Loading model weights"""
-        _load_model(self.path_weights, self.doctr_predictor, self.device, self.lib)
-
-    def build_model(self) -> "RecognitionPredictor":
-        """Building the model"""
-
-        # inspired and adapted from https://github.com/mindee/doctr/blob/main/doctr/models/recognition/zoo.py
-        custom_configs = {}
-        batch_size = 32
-        recognition_configs = {}
-        if self.path_config_json:
-            custom_configs = load_json(self.path_config_json)
-            custom_configs.pop("arch", None)
-            custom_configs.pop("url", None)
-            custom_configs.pop("task", None)
-            recognition_configs["mean"] = custom_configs.pop("mean")
-            recognition_configs["std"] = custom_configs.pop("std")
-            batch_size = custom_configs.pop("batch_size")
-        recognition_configs["batch_size"] = batch_size
-
-        if isinstance(self.architecture, str):
-            if self.architecture not in ARCHS:
-                raise ValueError(f"unknown architecture '{self.architecture}'")
+    assert get_num_gpu() > 0, "Has to train with GPU!"
 
-            model = recognition.__dict__[self.architecture](pretrained=True, pretrained_backbone=True, **custom_configs)
-        else:
-            if not isinstance(
-                self.architecture,
-                (recognition.CRNN, recognition.SAR, recognition.MASTER, recognition.ViTSTR, recognition.PARSeq),
-            ):
-                raise ValueError(f"unknown architecture: {type(self.architecture)}")
-            model = self.architecture
+    build_train_dict: Dict[str, str] = {}
+    if build_train_config is not None:
+        build_train_dict = string_to_dict(",".join(build_train_config))
+    if "split" not in build_train_dict:
+        build_train_dict["split"] = "train"
+
+    build_val_dict: Dict[str, str] = {}
+    if build_val_config is not None:
+        build_val_dict = string_to_dict(",".join(build_val_config))
+    if "split" not in build_val_dict:
+        build_val_dict["split"] = "val"
+
+    if config_overwrite is None:
+        config_overwrite = []
+    conf_list = [
+        "MODEL.WEIGHTS",
+        path_weights,
+        "OUTPUT_DIR",
+        log_dir,
+    ]
+    for conf in config_overwrite:
+        key, val = conf.split("=", maxsplit=1)
+        conf_list.extend([key, val])
+
+    if isinstance(dataset_train, str):
+        dataset_train = get_dataset(dataset_train)
+
+    cfg = _set_config(
+        path_config_yaml, conf_list, dataset_train, dataset_val, metric_name, metric, pipeline_component_name
+    )
+
+    if metric_name is not None:
+        metric = metric_registry.get(metric_name)
+
+    dataset = DatasetAdapter(dataset_train, True, image_to_d2_frcnn_training(False), True, **build_train_dict)
+    augment_list = [ResizeShortestEdge(cfg.INPUT.MIN_SIZE_TRAIN, cfg.INPUT.MAX_SIZE_TRAIN), RandomFlip()]
+    mapper = DatasetMapper(is_train=True, augmentations=augment_list, image_format="BGR")
+
+    logger.info(LoggingRecord(f"Config: \n {str(cfg)}", cfg.to_dict()))
+
+    trainer = D2Trainer(cfg, dataset, mapper)
+    trainer.resume_or_load()
+
+    if cfg.TEST.DO_EVAL:
+        categories = dataset_val.dataflow.categories.get_categories(filtered=True)  # type: ignore
+        config_overwrite = _update_for_eval(config_overwrite)
+        detector = D2FrcnnDetector(path_config_yaml, path_weights, categories, config_overwrite, cfg.MODEL.DEVICE)
+        pipeline_component_cls = pipeline_component_registry.get(pipeline_component_name)
+        pipeline_component = pipeline_component_cls(detector)
+        assert isinstance(pipeline_component, PredictorPipelineComponent)
+
+        if metric_name is not None:
+            metric = metric_registry.get(metric_name)
+        assert metric is not None
 
-        input_shape = model.cfg["input_shape"][:2] if tf_available() else model.cfg["input_shape"][-2:]
-        return RecognitionPredictor(PreProcessor(input_shape, preserve_aspect_ratio=True, **recognition_configs), model)
+        trainer.setup_evaluator(dataset_val, pipeline_component, metric, build_val_dict)  # type: ignore
+    return trainer.train()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/hfdetr.py` & `deepdoctection-0.31/deepdoctection/extern/hfdetr.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 HF Detr model for object detection.
 """
 
+from abc import ABC
+from pathlib import Path
 from typing import List, Literal, Mapping, Optional, Sequence
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import (
     get_pytorch_requirement,
     get_transformers_requirement,
     pytorch_available,
@@ -90,15 +92,56 @@
     keep_labels = results["labels"][keep]
     return [
         DetectionResult(box=box.tolist(), score=score.item(), class_id=class_id.item())
         for box, score, class_id in zip(keep_boxes, keep_scores, keep_labels)
     ]
 
 
-class HFDetrDerivedDetector(ObjectDetector):
+class HFDetrDerivedDetectorMixin(ObjectDetector, ABC):
+    """Base class for Detr object detector. This class only implements the basic wrapper functions"""
+
+    def __init__(self, categories: Mapping[str, TypeOrStr], filter_categories: Optional[Sequence[TypeOrStr]] = None):
+        """
+
+        :param categories: A dict with key (indices) and values (category names).
+        :param filter_categories: The model might return objects that are not supposed to be predicted and that should
+                                  be filtered. Pass a list of category names that must not be returned
+        """
+        self.categories = {idx: get_type(cat) for idx, cat in categories.items()}
+        if filter_categories:
+            filter_categories = [get_type(cat) for cat in filter_categories]
+        self.filter_categories = filter_categories
+
+    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
+        """
+        Populating category names to detection results. Will also filter categories
+
+        :param detection_results: list of detection results
+        :return: List of detection results with attribute class_name populated
+        """
+        filtered_detection_result: List[DetectionResult] = []
+        for result in detection_results:
+            result.class_name = self.categories[str(result.class_id + 1)]  # type: ignore
+            if isinstance(result.class_id, int):
+                result.class_id += 1
+            if self.filter_categories:
+                if result.class_name not in self.filter_categories:
+                    filtered_detection_result.append(result)
+            else:
+                filtered_detection_result.append(result)
+
+        return filtered_detection_result
+
+    @staticmethod
+    def get_name(path_weights: str) -> str:
+        """Returns the name of the model"""
+        return "Transformers_Tatr_" + "_".join(Path(path_weights).parts[-2:])
+
+
+class HFDetrDerivedDetector(HFDetrDerivedDetectorMixin):
     """
     Model wrapper for TableTransformerForObjectDetection that again is based on
 
     https://github.com/microsoft/table-transformer .
 
     The wrapper can be used to load pre-trained models for table detection and table structure recognition. Running Detr
     models trained from scratch on custom datasets is possible as well. Note, that this wrapper will load
@@ -134,86 +177,100 @@
         :param path_weights: The path to the model checkpoint.
         :param path_feature_extractor_config_json: The path to the feature extractor config.
         :param categories: A dict with key (indices) and values (category names).
         :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
         :param filter_categories: The model might return objects that are not supposed to be predicted and that should
                                   be filtered. Pass a list of category names that must not be returned
         """
-        self.name = "Detr"
-        self.categories = {idx: get_type(cat) for idx, cat in categories.items()}
+        super().__init__(categories, filter_categories)
+
         self.path_config = path_config_json
         self.path_weights = path_weights
         self.path_feature_extractor_config = path_feature_extractor_config_json
-        self.config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=self.path_config)
-        self.config.use_timm_backbone = True
-        self.config.threshold = 0.1
-        self.config.nms_threshold = 0.05
-        self.hf_detr_predictor = self.set_model(path_weights)
-        self.feature_extractor = self.set_pre_processor()
+
+        self.name = self.get_name(self.path_weights)
+        self.model_id = self.get_model_id()
+
+        self.config = self.get_config(path_config_json)
+
+        self.hf_detr_predictor = self.get_model(self.path_weights, self.config)
+        self.feature_extractor = self.get_pre_processor(self.path_feature_extractor_config)
 
         if device is not None:
             self.device = device
         else:
             self.device = set_torch_auto_device()
         self.hf_detr_predictor.to(self.device)
-        if filter_categories:
-            filter_categories = [get_type(cat) for cat in filter_categories]
-        self.filter_categories = filter_categories
 
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         results = detr_predict_image(
             np_img,
             self.hf_detr_predictor,
             self.feature_extractor,
             self.device,
             self.config.threshold,
             self.config.nms_threshold,
         )
         return self._map_category_names(results)
 
-    def set_model(self, path_weights: str) -> "TableTransformerForObjectDetection":
+    @staticmethod
+    def get_model(path_weights: str, config: "PretrainedConfig") -> "TableTransformerForObjectDetection":
         """
         Builds the Detr model
 
-        :param path_weights: weights
+        :param path_weights: The path to the model checkpoint.
+        :param config: `PretrainedConfig`
         :return: TableTransformerForObjectDetection instance
         """
         return TableTransformerForObjectDetection.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=self.config
+            pretrained_model_name_or_path=path_weights, config=config
         )
 
-    def set_pre_processor(self) -> "DetrFeatureExtractor":
+    @staticmethod
+    def get_pre_processor(path_feature_extractor_config: str) -> "DetrFeatureExtractor":
         """
         Builds the feature extractor
 
         :return: DetrFeatureExtractor
         """
-        return AutoFeatureExtractor.from_pretrained(pretrained_model_name_or_path=self.path_feature_extractor_config)
+        return AutoFeatureExtractor.from_pretrained(pretrained_model_name_or_path=path_feature_extractor_config)
 
-    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
+    @staticmethod
+    def get_config(path_config: str) -> "PretrainedConfig":
         """
-        Populating category names to detection results. Will also filter categories
+        Builds the config
 
-        :param detection_results: list of detection results
-        :return: List of detection results with attribute class_name populated
+        :param path_config: The path to the json config.
+        :return: PretrainedConfig instance
         """
-        filtered_detection_result: List[DetectionResult] = []
-        for result in detection_results:
-            result.class_name = self.categories[str(result.class_id + 1)]  # type: ignore
-            if isinstance(result.class_id, int):
-                result.class_id += 1
-            if self.filter_categories:
-                if result.class_name not in self.filter_categories:
-                    filtered_detection_result.append(result)
-            else:
-                filtered_detection_result.append(result)
-
-        return filtered_detection_result
+        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config)
+        config.use_timm_backbone = True
+        config.threshold = 0.1
+        config.nms_threshold = 0.05
+        return config
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_pytorch_requirement(), get_transformers_requirement()]
 
     def clone(self) -> "HFDetrDerivedDetector":
         return self.__class__(
             self.path_config, self.path_weights, self.path_feature_extractor_config, self.categories, self.device
         )
+
+    @staticmethod
+    def get_wrapped_model(
+        path_config_json: str, path_weights: str, device: Optional[Literal["cpu", "cuda"]] = None
+    ) -> "TableTransformerForObjectDetection":
+        """
+        Get the wrapped model
+
+        :param path_config_json: The path to the json config.
+        :param path_weights: The path to the model checkpoint.
+        :param device: "cpu" or "cuda". If not specified will auto select depending on what is available
+        :return: TableTransformerForObjectDetection instance
+        """
+        config = HFDetrDerivedDetector.get_config(path_config_json)
+        hf_detr_predictor = HFDetrDerivedDetector.get_model(path_weights, config)
+        if device is None:
+            device = set_torch_auto_device()
+        return hf_detr_predictor.to(device)
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/hflayoutlm.py` & `deepdoctection-0.31/deepdoctection/extern/hflayoutlm.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,15 +196,14 @@
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
         """
 
-        self.name = "_".join(Path(path_weights).parts[-3:])
         if categories is None:
             if categories_semantics is None:
                 raise ValueError("If categories is None then categories_semantics cannot be None")
             if categories_bio is None:
                 raise ValueError("If categories is None then categories_bio cannot be None")
 
         self.path_config = path_config_json
@@ -298,14 +297,19 @@
             self.path_weights,
             self.categories_semantics,
             self.categories_bio,
             self.categories,
             self.device,
         )
 
+    @staticmethod
+    def get_name(path_weights: str, architecture: str) -> str:
+        """Returns the name of the model"""
+        return f"Transformers_{architecture}_" + "_".join(Path(path_weights).parts[-2:])
+
 
 class HFLayoutLmTokenClassifier(HFLayoutLmTokenClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMForTokenClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/model_doc/layoutlm> for documentation of the model itself.
     Note that this model is equipped with a head that is only useful when classifying tokens. For sequence
     classification and other things please use another model of the family.
@@ -353,18 +357,17 @@
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
         """
-        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMForTokenClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
+        self.name = self.get_name(path_weights, "LayoutLM")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
         super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
@@ -384,14 +387,26 @@
 
         results = predict_token_classes(
             ann_ids, input_ids, attention_mask, token_type_ids, boxes, tokens, self.model, None
         )
 
         return self._map_category_names(results)
 
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMForTokenClassification.from_pretrained(pretrained_model_name_or_path=path_weights, config=config)
+
 
 class HFLayoutLmv2TokenClassifier(HFLayoutLmTokenClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMv2ForTokenClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/v4.24.0/en/model_doc/layoutlmv2>  for documentation of the model
     itself. Note that this model is equipped with a head that is only useful when classifying tokens. For sequence
     classification and other things please use another model of the family.
@@ -441,18 +456,17 @@
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
         """
-        config = LayoutLMv2Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMv2ForTokenClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
+        self.name = self.get_name(path_weights, "LayoutLMv2")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
         super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
@@ -485,14 +499,28 @@
     def default_kwargs_for_input_mapping() -> JsonDict:
         """
         Add some default arguments that might be necessary when preparing a sample. Overwrite this method
         for some custom setting.
         """
         return {"image_width": 224, "image_height": 224}
 
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = LayoutLMv2Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMv2ForTokenClassification.from_pretrained(
+            pretrained_model_name_or_path=path_weights, config=config
+        )
+
 
 class HFLayoutLmv3TokenClassifier(HFLayoutLmTokenClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMv3ForTokenClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/v4.24.0/en/model_doc/layoutlmv3>  for documentation of the model
     itself. Note that this model is equipped with a head that is only useful when classifying tokens. For sequence
     classification and other things please use another model of the family.
@@ -542,18 +570,17 @@
                                      entities self. To be consistent with detectors use only values >0. Conversion will
                                      be done internally.
         :param categories_bio: A dict with key (indices) and values (category names) for NER tags (i.e. BIO). To be
                                consistent with detectors use only values>0. Conversion will be done internally.
         :param categories: If you have a pre-trained model you can pass a complete dict of NER categories
         :param device: The device (cpu,"cuda"), where to place the model.
         """
-        config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMv3ForTokenClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
+        self.name = self.get_name(path_weights, "LayoutLMv3")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
         super().__init__(path_config_json, path_weights, categories_semantics, categories_bio, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> List[TokenClassResult]:
         """
         Launch inference on LayoutLm for token classification. Pass the following arguments
 
         `input_ids:` Token converted to ids to be taken from `LayoutLMTokenizer`
@@ -588,14 +615,28 @@
             "image_width": 224,
             "image_height": 224,
             "color_mode": "RGB",
             "pixel_mean": np.array(IMAGENET_DEFAULT_MEAN, dtype=np.float32),
             "pixel_std": np.array(IMAGENET_DEFAULT_STD, dtype=np.float32),
         }
 
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMv3ForTokenClassification.from_pretrained(
+            pretrained_model_name_or_path=path_weights, config=config
+        )
+
 
 class HFLayoutLmSequenceClassifierBase(LMSequenceClassifier, ABC):
     """
     Abstract base class for wrapping LayoutLM models  for sequence classification into the deepdoctection framework.
     """
 
     model: Union["LayoutLMForSequenceClassification", "LayoutLMv2ForSequenceClassification"]
@@ -603,15 +644,14 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-        self.name = "_".join(Path(path_weights).parts[-3:])
         self.path_config = path_config_json
         self.path_weights = path_weights
         self.categories = copy(categories)  # type: ignore
 
         if device is not None:
             self.device = device
         else:
@@ -687,14 +727,19 @@
 
         input_ids = input_ids.to(self.device)
         attention_mask = attention_mask.to(self.device)
         token_type_ids = token_type_ids.to(self.device)
         boxes = boxes.to(self.device)
         return input_ids, attention_mask, token_type_ids, boxes
 
+    @staticmethod
+    def get_name(path_weights: str, architecture: str) -> str:
+        """Returns the name of the model"""
+        return f"Transformers_{architecture}_" + "_".join(Path(path_weights).parts[-2:])
+
 
 class HFLayoutLmSequenceClassifier(HFLayoutLmSequenceClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMForSequenceClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/model_doc/layoutlm> for documentation of the model itself.
     Note that this model is equipped with a head that is only useful for classifying the input sequence. For token
     classification and other things please use another model of the family.
@@ -726,14 +771,16 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
+        self.name = self.get_name(path_weights, "LayoutLM")
+        self.model_id = self.get_model_id()
         config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
         self.model = LayoutLMForSequenceClassification.from_pretrained(
             pretrained_model_name_or_path=path_weights, config=config
         )
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
@@ -747,14 +794,28 @@
             self.model,
         )
 
         result.class_id += 1
         result.class_name = self.categories[str(result.class_id)]
         return result
 
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = PretrainedConfig.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMForSequenceClassification.from_pretrained(
+            pretrained_model_name_or_path=path_weights, config=config
+        )
+
 
 class HFLayoutLmv2SequenceClassifier(HFLayoutLmSequenceClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMv2ForSequenceClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/v4.24.0/en/model_doc/layoutlmv2> for documentation of the model
     itself. Note that this model is equipped with a head that is only useful for classifying the input sequence. For
     token classification and other things please use another model of the family.
@@ -786,18 +847,17 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-        config = LayoutLMv2Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMv2ForSequenceClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
+        self.name = self.get_name(path_weights, "LayoutLMv2")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
         input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
         images = encodings.get("image")
         if isinstance(images, torch.Tensor):
             images = images.to(self.device)
@@ -814,14 +874,28 @@
     def default_kwargs_for_input_mapping() -> JsonDict:
         """
         Add some default arguments that might be necessary when preparing a sample. Overwrite this method
         for some custom setting.
         """
         return {"image_width": 224, "image_height": 224}
 
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = LayoutLMv2Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMv2ForSequenceClassification.from_pretrained(
+            pretrained_model_name_or_path=path_weights, config=config
+        )
+
 
 class HFLayoutLmv3SequenceClassifier(HFLayoutLmSequenceClassifierBase):
     """
     A wrapper class for `transformers.LayoutLMv3ForSequenceClassification` to use within a pipeline component.
     Check <https://huggingface.co/docs/transformers/v4.24.0/en/model_doc/layoutlmv3> for documentation of the model
     itself. Note that this model is equipped with a head that is only useful for classifying the input sequence. For
     token classification and other things please use another model of the family.
@@ -853,18 +927,17 @@
     def __init__(
         self,
         path_config_json: str,
         path_weights: str,
         categories: Mapping[str, TypeOrStr],
         device: Optional[Literal["cpu", "cuda"]] = None,
     ):
-        config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
-        self.model = LayoutLMv3ForSequenceClassification.from_pretrained(
-            pretrained_model_name_or_path=path_weights, config=config
-        )
+        self.name = self.get_name(path_weights, "LayoutLMv3")
+        self.model_id = self.get_model_id()
+        self.model = self.get_wrapped_model(path_config_json, path_weights)
         super().__init__(path_config_json, path_weights, categories, device)
 
     def predict(self, **encodings: Union[List[List[str]], "torch.Tensor"]) -> SequenceClassResult:
         input_ids, attention_mask, token_type_ids, boxes = self._validate_encodings(**encodings)
         images = encodings.get("pixel_values")
         if isinstance(images, torch.Tensor):
             images = images.to(self.device)
@@ -886,7 +959,21 @@
         return {
             "image_width": 224,
             "image_height": 224,
             "color_mode": "RGB",
             "pixel_mean": np.array(IMAGENET_DEFAULT_MEAN, dtype=np.float32),
             "pixel_std": np.array(IMAGENET_DEFAULT_STD, dtype=np.float32),
         }
+
+    @staticmethod
+    def get_wrapped_model(path_config_json: str, path_weights: str) -> Any:
+        """
+        Get the inner (wrapped) model.
+
+        :param path_config_json: path to .json config file
+        :param path_weights: path to model artifact
+        :return: 'nn.Module'
+        """
+        config = LayoutLMv3Config.from_pretrained(pretrained_model_name_or_path=path_config_json)
+        return LayoutLMv3ForSequenceClassification.from_pretrained(
+            pretrained_model_name_or_path=path_weights, config=config
+        )
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/model.py` & `deepdoctection-0.31/deepdoctection/extern/model.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/pdftext.py` & `deepdoctection-0.31/deepdoctection/extern/pdftext.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         df = pipe.analyze(path="path/to/document.pdf")
         for dp in df:
             ...
 
     """
 
     def __init__(self) -> None:
-        self.name = "pdfplumber"
+        self.name = "Pdfplumber"
+        self.model_id = self.get_model_id()
         self.categories = {"1": LayoutType.word}
 
     def predict(self, pdf_bytes: bytes) -> List[DetectionResult]:
         """
         Call pdfminer.six and returns detected text as detection results
 
         :param pdf_bytes: bytes of a single pdf page
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/pt/__init__.py` & `deepdoctection-0.31/deepdoctection/extern/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/pt/nms.py` & `deepdoctection-0.31/deepdoctection/extern/pt/nms.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/pt/ptutils.py` & `deepdoctection-0.31/deepdoctection/extern/pt/ptutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 # limitations under the License.
 
 """
 Torch related utils
 """
 
 
+from ...utils.error import DependencyError
 from ...utils.file_utils import pytorch_available
 
 
 def set_torch_auto_device() -> "torch.device":  # type: ignore
     """
     Returns cuda device if available, otherwise cpu
     """
     if pytorch_available():
         from torch import cuda, device  # pylint: disable=C0415
 
         return device("cuda" if cuda.is_available() else "cpu")
-    raise ModuleNotFoundError("Pytorch must be installed")
+    raise DependencyError("Pytorch must be installed")
 
 
 def get_num_gpu() -> int:
     """
     Returns number of CUDA devices if pytorch is available
 
     :return:
     """
 
     if pytorch_available():
         from torch import cuda  # pylint: disable=C0415
 
         return cuda.device_count()
-    raise ModuleNotFoundError("Pytorch must be installed")
+    raise DependencyError("Pytorch must be installed")
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/tessocr.py` & `deepdoctection-0.31/deepdoctection/extern/tessocr.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Tesseract OCR engine for text extraction
 """
 import shlex
+import string
 import subprocess
 import sys
 from errno import ENOENT
 from itertools import groupby
 from os import environ
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Mapping, Optional, Union
 
-import numpy as np
+from packaging.version import InvalidVersion, Version, parse
 
 from ..utils.context import save_tmp_file, timeout_manager
 from ..utils.detection_types import ImageType, Requirement
-from ..utils.file_utils import _TESS_PATH, TesseractNotFound, get_tesseract_requirement
+from ..utils.error import DependencyError, TesseractError
+from ..utils.file_utils import _TESS_PATH, get_tesseract_requirement
 from ..utils.metacfg import config_to_cli_str, set_config_by_yaml
-from ..utils.settings import LayoutType, ObjectTypes
-from .base import DetectionResult, ObjectDetector, PredictorBase
+from ..utils.settings import LayoutType, ObjectTypes, PageType
+from ..utils.viz import viz_handler
+from .base import DetectionResult, ImageTransformer, ObjectDetector, PredictorBase
 
 # copy and paste with some light modifications from https://github.com/madmaze/pytesseract/tree/master/pytesseract
 
 
 _LANG_CODE_TO_TESS_LANG_CODE = {
     "fre": "fra",
     "dut": "nld",
@@ -53,26 +56,14 @@
     "glg": "gla",
     "slv": "slk",
     "alb": "nor",
     "nn": "eng",
 }
 
 
-class TesseractError(RuntimeError):
-    """
-    Tesseract Error
-    """
-
-    def __init__(self, status: int, message: str) -> None:
-        super().__init__()
-        self.status = status
-        self.message = message
-        self.args = (status, message)
-
-
 def _subprocess_args() -> Dict[str, Any]:
     # See https://github.com/pyinstaller/pyinstaller/wiki/Recipe-subprocess
     # for reference and comments.
 
     kwargs = {
         "stdin": subprocess.PIPE,
         "stderr": subprocess.PIPE,
@@ -105,24 +96,68 @@
 
 def _run_tesseract(tesseract_args: List[str]) -> None:
     try:
         proc = subprocess.Popen(tesseract_args, **_subprocess_args())  # pylint: disable=R1732
     except OSError as error:
         if error.errno != ENOENT:
             raise error from error
-        raise TesseractNotFound("Tesseract not found. Please install or add to your PATH.") from error
+        raise DependencyError("Tesseract not found. Please install or add to your PATH.") from error
 
     with timeout_manager(proc, 0) as error_string:
         if proc.returncode:
             raise TesseractError(
                 proc.returncode,
                 " ".join(line for line in error_string.decode("utf-8").splitlines()).strip(),  # type: ignore
             )
 
 
+def get_tesseract_version() -> Version:
+    """
+    Returns Version object of the Tesseract version
+    """
+    try:
+        output = subprocess.check_output(
+            ["tesseract", "--version"],
+            stderr=subprocess.STDOUT,
+            env=environ,
+            stdin=subprocess.DEVNULL,
+        )
+    except OSError as error:
+        raise DependencyError("Tesseract not found. Please install or add to your PATH.") from error
+
+    raw_version = output.decode("utf-8")
+    str_version, *_ = raw_version.lstrip(string.printable[10:]).partition(" ")
+    str_version, *_ = str_version.partition("-")
+
+    try:
+        version = parse(str_version)
+        assert version >= Version("3.05")
+    except (AssertionError, InvalidVersion) as error:
+        raise SystemExit(f'Invalid tesseract version: "{raw_version}"') from error
+
+    return version
+
+
+def image_to_angle(image: ImageType) -> Mapping[str, str]:
+    """
+    Generating a tmp file and running tesseract to get the orientation of the image.
+
+    :param image: Image in np.array.
+    :return: A dictionary with keys 'Orientation in degrees' and 'Orientation confidence'.
+    """
+    with save_tmp_file(image, "tess_") as (tmp_name, input_file_name):
+        _run_tesseract(_input_to_cli_str("osd", "--psm 0", 0, input_file_name, tmp_name))
+        with open(tmp_name + ".osd", "rb") as output_file:
+            output = output_file.read().decode("utf-8")
+
+    return {
+        key_value[0]: key_value[1] for key_value in (line.split(": ") for line in output.split("\n") if len(line) >= 2)
+    }
+
+
 def image_to_dict(image: ImageType, lang: str, config: str) -> Dict[str, List[Union[str, int, float]]]:
     """
     This is more or less pytesseract.image_to_data with a dict as returned value.
     What happens under the hood is:
 
     - saving an image file
     - defining tesseracts command line
@@ -216,15 +251,14 @@
                                 detected text, if this in known in advance. Combinations are possible, e.g. "deu",
                                 "fr+eng".
     :param text_lines: If True, it will return DetectionResults of Text lines as well.
     :param config: The config parameter passing to Tesseract. Consult also https://guides.nyu.edu/tesseract/usage
     :return: A list of tesseract extractions wrapped in DetectionResult
     """
 
-    np_img = np_img.astype(np.uint8)
     results = image_to_dict(np_img, supported_languages, config)
     all_results = []
 
     for caption in zip(
         results["left"],
         results["top"],
         results["width"],
@@ -245,14 +279,24 @@
             )
             all_results.append(word)
     if text_lines:
         all_results = tesseract_line_to_detectresult(all_results)
     return all_results
 
 
+def predict_rotation(np_img: ImageType) -> Mapping[str, str]:
+    """
+    Predicts the rotation of an image using the Tesseract OCR engine.
+
+    :param np_img: numpy array of the image
+    :return: A dictionary with keys 'Orientation in degrees' and 'Orientation confidence'
+    """
+    return image_to_angle(np_img)
+
+
 class TesseractOcrDetector(ObjectDetector):
     """
     Text object detector based on Tesseracts OCR engine. Note that tesseract has to be installed separately.
 
     The current Tesseract release is 4.1.1. A version 5.xx can be integrated via direct installation at
     https://github.com/tesseract-ocr/tesseract. Building from source is necessary here.
 
@@ -288,15 +332,17 @@
         """
         Set up the configuration which is stored in a yaml-file, that need to be passed through.
 
         :param path_yaml: The path to the yaml config
         :param config_overwrite: Overwrite config parameters defined by the yaml file with new values.
                                  E.g. ["oem=14"]
         """
-        self.name = _TESS_PATH
+        self.name = self.get_name()
+        self.model_id = self.get_model_id()
+
         if config_overwrite is None:
             config_overwrite = []
 
         hyper_param_config = set_config_by_yaml(path_yaml)
         if len(config_overwrite):
             hyper_param_config.update_args(config_overwrite)
 
@@ -312,21 +358,21 @@
     def predict(self, np_img: ImageType) -> List[DetectionResult]:
         """
         Transfer of a numpy array and call of pytesseract. Return of the detection results.
 
         :param np_img: image as numpy array
         :return: A list of DetectionResult
         """
-        detection_results = predict_text(
+
+        return predict_text(
             np_img,
             supported_languages=self.config.LANGUAGES,
             text_lines=self.config.LINES,
             config=config_to_cli_str(self.config, "LANGUAGES", "LINES"),
         )
-        return detection_results
 
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_tesseract_requirement()]
 
     def clone(self) -> PredictorBase:
         return self.__class__(self.path_yaml, self.config_overwrite)
@@ -338,7 +384,73 @@
 
     def set_language(self, language: ObjectTypes) -> None:
         """
         Pass a language to change the model selection. For runtime language selection.
         :param language: `Languages`
         """
         self.config.LANGUAGES = _LANG_CODE_TO_TESS_LANG_CODE.get(language, language.value)
+
+    @staticmethod
+    def get_name() -> str:
+        """Returns the name of the model"""
+        return f"Tesseract_{get_tesseract_version()}"
+
+
+class TesseractRotationTransformer(ImageTransformer):
+    """
+    The `TesseractRotationTransformer` class is a specialized image transformer that is designed to handle image
+    rotation in the context of Optical Character Recognition (OCR) tasks. It inherits from the `ImageTransformer`
+    base class and implements methods for predicting and applying rotation transformations to images.
+
+    The `predict` method determines the angle of the rotated image. It can only handle angles that are multiples of 90
+    degrees.
+    This method uses the Tesseract OCR engine to predict the rotation angle of an image.
+
+    The `transform` method applies the predicted rotation to the image, effectively rotating the image backwards.
+    This method uses either the Pillow library or OpenCV for the rotation operation, depending on the configuration.
+
+    This class can be particularly useful in OCR tasks where the orientation of the text in the image matters.
+    The class also provides methods for cloning itself and for getting the requirements of the Tesseract OCR system.
+
+    **Example:**
+                    transformer = TesseractRotationTransformer()
+                    detection_result = transformer.predict(np_img)
+                    rotated_image = transformer.transform(np_img, detection_result)
+    """
+
+    def __init__(self) -> None:
+        self.name = _TESS_PATH + "-rotation"
+
+    def transform(self, np_img: ImageType, specification: DetectionResult) -> ImageType:
+        """
+        Applies the predicted rotation to the image, effectively rotating the image backwards.
+        This method uses either the Pillow library or OpenCV for the rotation operation, depending on the configuration.
+
+        :param np_img: The input image as a numpy array.
+        :param specification: A `DetectionResult` object containing the predicted rotation angle.
+        :return: The rotated image as a numpy array.
+        """
+        return viz_handler.rotate_image(np_img, specification.angle)  # type: ignore
+
+    def predict(self, np_img: ImageType) -> DetectionResult:
+        """
+        Determines the angle of the rotated image. It can only handle angles that are multiples of 90 degrees.
+        This method uses the Tesseract OCR engine to predict the rotation angle of an image.
+
+        :param np_img: The input image as a numpy array.
+        :return: A `DetectionResult` object containing the predicted rotation angle and confidence.
+        """
+        output_dict = predict_rotation(np_img)
+        return DetectionResult(
+            angle=float(output_dict["Orientation in degrees"]), score=float(output_dict["Orientation confidence"])
+        )
+
+    @classmethod
+    def get_requirements(cls) -> List[Requirement]:
+        return [get_tesseract_requirement()]
+
+    def clone(self) -> PredictorBase:
+        return self.__class__()
+
+    @staticmethod
+    def possible_category() -> PageType:
+        return PageType.angle
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/texocr.py` & `deepdoctection-0.31/deepdoctection/extern/texocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
 
     def __init__(self, text_lines: bool = False, **credentials_kwargs: str) -> None:
         """
         :param text_lines: If True, it will return DetectionResults of Text lines as well.
         :param credentials_kwargs: `aws_access_key_id`, `aws_secret_access_key` or `aws_session_token`
         """
         self.name = "textract"
+        self.model_id = self.get_model_id()
+
         self.text_lines = text_lines
         self.client = boto3.client("textract", **credentials_kwargs)
         if self.text_lines:
             self.categories = {"1": LayoutType.word, "2": LayoutType.line}
         else:
             self.categories = {"1": LayoutType.word}
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/__init__.py` & `deepdoctection-0.31/deepdoctection/extern/tp/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tfutils.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tfutils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpcompat.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpcompat.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def get_inference_tensor_names(self) -> Tuple[List[str], List[str]]:
         """
         Returns lists of tensor names to be used to create an inference callable. "build_graph" must create tensors
         of these names when called under inference context.
 
         :return: Tuple of list input and list output names. The names must coincide with tensor within the model.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class TensorpackPredictor(ABC):
     """
     The base class for wrapping a Tensorpack predictor. It takes a ModelDescWithConfig from Tensorpack and weights and
     builds a Tensorpack offline predictor (e.g. a default session will be generated when initializing).
 
@@ -102,30 +102,30 @@
             output_names=self._model.get_inference_tensor_names()[1],
         )
 
         return predict_config
 
     @staticmethod
     @abstractmethod
-    def set_model(
+    def get_wrapped_model(
         path_yaml: str, categories: Mapping[str, ObjectTypes], config_overwrite: Union[List[str], None]
     ) -> ModelDescWithConfig:
         """
         Implement the config generation, its modification and instantiate a version of the model. See
         `pipe.tpfrcnn.TPFrcnnDetector` for an example
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def predict(self, np_img: Any) -> Any:
         """
         Implement, how `self.tp_predictor` is invoked and raw prediction results are generated. Do use only raw
         objects and nothing, which is related to the DD API.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @property
     def model(self) -> ModelDescWithConfig:
         """
         model
         """
         return self._model
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/common.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/config/config.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/config/config.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/backbone.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/generalized_rcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_cascade.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_fpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_frcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_mrcnn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/modeling/model_rpn.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/predict.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/predict.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/preproc.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/preproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,24 @@
 import numpy as np
 
 # pylint: disable=import-error
 from tensorpack.dataflow.imgaug import AugmentorList, ImageAugmentor
 
 from ....datapoint.convert import box_to_point4, point4_to_box
 from ....utils.detection_types import ImageType, JsonDict
+from ....utils.error import MalformedData
 from ....utils.logger import log_once
 from .common import filter_boxes_inside_shape, np_iou
 from .modeling.model_fpn import get_all_anchors_fpn
 from .utils.np_box_ops import area as np_area
 from .utils.np_box_ops import ioa as np_ioa
 
 # pylint: enable=import-error
 
 
-class MalformedData(BaseException):
-    """
-    Exception class for malformed data
-    """
-
-
 def augment(dp: JsonDict, imgaug_list: List[ImageAugmentor], add_mask: bool) -> JsonDict:
     """
     Augment an image according to a list of augmentors.
 
     :param dp: A dict with "image","gt_boxes","gt_labels"
     :param imgaug_list: List auf augmentors
     :param add_mask: not implemented
@@ -58,15 +53,15 @@
     dp["image"] = image_aug
     dp["gt_boxes"] = gt_boxes
 
     if len(gt_boxes):
         assert np.min(np_area(gt_boxes)) > 0, "some boxes have zero area"
 
     if add_mask:
-        raise NotImplementedError
+        raise NotImplementedError()
 
     return dp
 
 
 def anchors_and_labels(
     dp: JsonDict,
     anchor_strides: Tuple[int],
```

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py` & `deepdoctection-0.31/deepdoctection/extern/tp/tpfrcnn/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/extern/tpdetect.py` & `deepdoctection-0.31/deepdoctection/extern/tpdetect.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,72 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 TP Faster RCNN model as predictor for deepdoctection pipeline
 """
 
+from abc import ABC
 from copy import copy
 from pathlib import Path
-from typing import List, Mapping, Optional, Sequence, Union
+from typing import Dict, List, Mapping, Optional, Sequence, Union
 
 from ..utils.detection_types import ImageType, Requirement
 from ..utils.file_utils import get_tensorflow_requirement, get_tensorpack_requirement, tensorpack_available
 from ..utils.metacfg import set_config_by_yaml
 from ..utils.settings import ObjectTypes, TypeOrStr, get_type
 from .base import DetectionResult, ObjectDetector, PredictorBase
 
 if tensorpack_available():
     from .tp.tpcompat import TensorpackPredictor
     from .tp.tpfrcnn.config.config import model_frcnn_config
     from .tp.tpfrcnn.modeling.generalized_rcnn import ResNetFPNModel
     from .tp.tpfrcnn.predict import tp_predict_image
 
 
-class TPFrcnnDetector(TensorpackPredictor, ObjectDetector):
+class TPFrcnnDetectorMixin(ObjectDetector, ABC):
+    """Base class for TP FRCNN detector. This class only implements the basic wrapper functions"""
+
+    def __init__(self, categories: Mapping[str, TypeOrStr], filter_categories: Optional[Sequence[TypeOrStr]] = None):
+        self.categories = copy(categories)  # type: ignore
+        if filter_categories:
+            filter_categories = [get_type(cat) for cat in filter_categories]
+        self.filter_categories = filter_categories
+        self._tp_categories = self._map_to_tp_categories(categories)
+
+    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
+        """
+        Populating category names to detection results
+
+        :param detection_results: list of detection results
+        :return: List of detection results with attribute class_name populated
+        """
+        filtered_detection_result: List[DetectionResult] = []
+        for result in detection_results:
+            result.class_name = self._tp_categories[str(result.class_id)]
+            if self.filter_categories:
+                if result.class_name not in self.filter_categories:
+                    filtered_detection_result.append(result)
+            else:
+                filtered_detection_result.append(result)
+        return filtered_detection_result
+
+    @staticmethod
+    def _map_to_tp_categories(categories: Mapping[str, TypeOrStr]) -> Dict[str, ObjectTypes]:
+        categories = {str(key): get_type(categories[val]) for key, val in enumerate(categories, 1)}
+        categories["0"] = get_type("background")
+        return categories  # type: ignore
+
+    @staticmethod
+    def get_name(path_weights: str, architecture: str) -> str:
+        """Returns the name of the model"""
+        return f"Tensorpack_{architecture}" + "_".join(Path(path_weights).parts[-2:])
+
+
+class TPFrcnnDetector(TensorpackPredictor, TPFrcnnDetectorMixin):
     """
     Tensorpack Faster-RCNN implementation with FPN and optional Cascade-RCNN. The backbones Resnet-50, Resnet-101 and
     their Resnext counterparts are also available. Normalization options (group normalization, synchronized batch
     normalization) for backbone in FPN can be chosen as well.
 
     Currently, masks are not included in the data model. However, Mask-RCNN is implemented in this version.
 
@@ -83,27 +123,31 @@
         :param config_overwrite: Overwrite some hyperparameters defined by the yaml file with some new values. E.g.
                                  ["OUTPUT.FRCNN_NMS_THRESH=0.3","OUTPUT.RESULT_SCORE_THRESH=0.6"]
         :param ignore_mismatch: When True will ignore mismatches between checkpoint weights and models. This is needed
                                 if a pre-trained model is to be fine-tuned on a custom dataset.
         :param filter_categories: The model might return objects that are not supposed to be predicted and that should
                                   be filtered. Pass a list of category names that must not be returned
         """
-        self.name = "_".join(Path(path_weights).parts[-3:])
         self.path_yaml = path_yaml
+
         self.categories = copy(categories)  # type: ignore
         self.config_overwrite = config_overwrite
         if filter_categories:
             filter_categories = [get_type(cat) for cat in filter_categories]
         self.filter_categories = filter_categories
-        model = TPFrcnnDetector.set_model(path_yaml, self.categories, config_overwrite)
-        super().__init__(model, path_weights, ignore_mismatch)
+        model = TPFrcnnDetector.get_wrapped_model(path_yaml, self.categories, config_overwrite)
+        TensorpackPredictor.__init__(self, model, path_weights, ignore_mismatch)
+        TPFrcnnDetectorMixin.__init__(self, categories, filter_categories)
+
+        self.name = self.get_name(path_weights, self._model.cfg.TAG)
+        self.model_id = self.get_model_id()
         assert self._number_gpus > 0, "Model only support inference with GPU"
 
     @staticmethod
-    def set_model(
+    def get_wrapped_model(
         path_yaml: str, categories: Mapping[str, ObjectTypes], config_overwrite: Union[List[str], None]
     ) -> ResNetFPNModel:
         """
         Calls all necessary methods to build TP ResNetFPNModel
 
         :param path_yaml: path to the model config
         :param categories: A dict of categories with indices as keys
@@ -134,31 +178,14 @@
             self.tp_predictor,
             self._model.cfg.PREPROC.SHORT_EDGE_SIZE,
             self._model.cfg.PREPROC.MAX_SIZE,
             self._model.cfg.MRCNN.ACCURATE_PASTE,
         )
         return self._map_category_names(detection_results)
 
-    def _map_category_names(self, detection_results: List[DetectionResult]) -> List[DetectionResult]:
-        """
-        Populating category names to detection results
-
-        :param detection_results: list of detection results
-        :return: List of detection results with attribute class_name populated
-        """
-        filtered_detection_result: List[DetectionResult] = []
-        for result in detection_results:
-            result.class_name = self._model.cfg.DATA.CLASS_DICT[str(result.class_id)]
-            if self.filter_categories:
-                if result.class_name not in self.filter_categories:
-                    filtered_detection_result.append(result)
-            else:
-                filtered_detection_result.append(result)
-        return filtered_detection_result
-
     @classmethod
     def get_requirements(cls) -> List[Requirement]:
         return [get_tensorflow_requirement(), get_tensorpack_requirement()]
 
     def clone(self) -> PredictorBase:
         return self.__class__(
             self.path_yaml,
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/__init__.py` & `deepdoctection-0.31/deepdoctection/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/cats.py` & `deepdoctection-0.31/deepdoctection/mapper/cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/cocostruct.py` & `deepdoctection-0.31/deepdoctection/mapper/cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/d2struct.py` & `deepdoctection-0.31/deepdoctection/mapper/d2struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             "bbox_mode": BoxMode.XYXY_ABS,
             "bbox": box.to_list(mode="xyxy"),
             "category_id": int(ann.category_id) - 1,
         }
         annotations.append(mapped_ann)
 
         if add_mask:
-            raise NotImplementedError
+            raise NotImplementedError("Segmentation in deepdoctection is not supported")
 
     output["annotations"] = annotations
 
     return output
 
 
 def pt_nms_image_annotations(
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/hfstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/hfstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             "bbox": box.to_list(mode="xywh"),
             "category_id": int(ann.category_id) - 1,
             "area": box.area,
         }
         annotations.append(mapped_ann)
 
     if add_mask:
-        raise NotImplementedError
+        raise NotImplementedError("Segmentation in deepdoctection is not supported")
 
     output["annotations"] = annotations
 
     return output
 
 
 @dataclass
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/laylmstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/laylmstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     for ann in anns:
         all_ann_ids.append(ann.annotation_id)
         char_cat = ann.get_sub_category(WordType.characters)
         if not isinstance(char_cat, ContainerAnnotation):
             raise TypeError(f"char_cat must be of type ContainerAnnotation but is of type {type(char_cat)}")
         word = char_cat.value
         if not isinstance(word, str):
-            raise ValueError(f"word must be of type str but is of type {type(word)}")
+            raise TypeError(f"word must be of type str but is of type {type(word)}")
         all_words.append(word)
 
         box = ann.get_bounding_box(dp.image_id)
         if not box.absolute_coords:
             box = box.transform(dp.width, dp.height, absolute_coords=True)
         all_boxes.append(word_id_to_segment_box.get(ann.annotation_id, box).to_list(mode="xyxy"))
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/maputils.py` & `deepdoctection-0.31/deepdoctection/mapper/maputils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from types import TracebackType
 from typing import Any, Callable, Dict, Mapping, Optional, Sequence, Union
 
 import numpy as np
 from tabulate import tabulate
 from termcolor import colored
 
-from ..datapoint.box import BoundingBoxError
 from ..utils.detection_types import DP, BaseExceptionType, S, T
+from ..utils.error import AnnotationError, BoundingBoxError, ImageError, UUIDError
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import ObjectTypes
 
 __all__ = ["MappingContextManager", "DefaultMapper", "maybe_get_fake_score", "LabelSummarizer", "curry"]
 
 
 class MappingContextManager:
@@ -68,15 +68,26 @@
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         """
         context exit
         """
         if (
             exc_type
-            in (KeyError, ValueError, IndexError, AssertionError, TypeError, BoundingBoxError, FileNotFoundError)
+            in (
+                KeyError,
+                ValueError,
+                IndexError,
+                AssertionError,
+                TypeError,
+                FileNotFoundError,
+                BoundingBoxError,
+                AnnotationError,
+                ImageError,
+                UUIDError,
+            )
             and exc_tb is not None
         ):
             frame_summary = traceback.extract_tb(exc_tb)[0]
             log_dict = {
                 "file_name": self.dp_name,
                 "error_type": type(exc_val).__name__,
                 "error_msg": str(exc_val),
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/match.py` & `deepdoctection-0.31/deepdoctection/mapper/match.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/misc.py` & `deepdoctection-0.31/deepdoctection/mapper/misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/pascalstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/pascalstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/mapper/prodigystruct.py` & `deepdoctection-0.31/deepdoctection/mapper/prodigystruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             if category_name_mapping is not None:
                 label = category_name_mapping.get(span["label"])
                 if not label:
                     label = span["label"]
             else:
                 label = span["label"]
             if not isinstance(label, str):
-                raise ValueError("label could not assigned to be a string")
+                raise TypeError("label must be a string")
 
             annotation = ImageAnnotation(
                 category_name=label,
                 bounding_box=bbox,
                 category_id=categories_name_as_key[label],
                 score=score,
                 external_id=external_id,
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/pubstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/pubstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,22 @@
     index_cells_tmp[-1].append(index_cells[-1])
     return index_cells_tmp
 
 
 def _item_spans(html: Sequence[str], index_cells: Sequence[Sequence[int]], item: str) -> List[List[int]]:
     item_spans = [
         [
-            int(html[index_cell - 1].replace(item + "=", "").replace('"', ""))
-            if (item in html[index_cell - 1] and html[index_cell] == ">")
-            else (
-                int(html[index_cell - 2].replace(item + "=", "").replace('"', ""))
-                if (item in html[index_cell - 2] and html[index_cell] == ">")
-                else 1
+            (
+                int(html[index_cell - 1].replace(item + "=", "").replace('"', ""))
+                if (item in html[index_cell - 1] and html[index_cell] == ">")
+                else (
+                    int(html[index_cell - 2].replace(item + "=", "").replace('"', ""))
+                    if (item in html[index_cell - 2] and html[index_cell] == ">")
+                    else 1
+                )
             )
             for index_cell in index_cell_per_row
         ]
         for index_cell_per_row in index_cells
     ]
     return item_spans
 
@@ -206,17 +208,15 @@
             item_ann.dump_sub_category(TableType.item, item_sub_ann, image.image_id)
             image.dump(item_ann)
 
     if pubtables_like:  # pubtables_like:
         items = image.get_annotation(category_names=TableType.item)
         item_type_anns = [ann for ann in items if ann.get_sub_category(TableType.item).category_name == item_type]
         item_type_anns.sort(
-            key=lambda x: x.bounding_box.cx  # type: ignore
-            if item_type == LayoutType.column
-            else x.bounding_box.cy  # type: ignore
+            key=lambda x: (x.bounding_box.cx if item_type == LayoutType.column else x.bounding_box.cy)  # type: ignore
         )
         if table.bounding_box:
             tmp_item_xy = table.bounding_box.uly + 1.0 if item_type == LayoutType.row else table.bounding_box.ulx + 1.0
         for idx, item in enumerate(item_type_anns):
             with MappingContextManager(
                 dp_name=image.file_name,
                 filter_level="bounding box",
@@ -385,15 +385,15 @@
 
     if transforming_context.context_error:
         return None
 
     with MappingContextManager(str(idx)) as mapping_context:
         max_rs, max_cs = 0, 0
         if idx is None:
-            raise ValueError("No valid datapoint external id")
+            raise TypeError("imgid is None but must be a string")
 
         image = Image(file_name=os.path.split(dp["filename"])[1], location=dp["filename"], external_id=idx)
 
         if is_file_extension(dp["filename"], ".png"):
             np_image = load_image_from_file(dp["filename"])
         if is_file_extension(dp["filename"], ".pdf"):
             pdf_bytes = load_bytes_from_pdf_file(dp["filename"])
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/tpstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/tpstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     for ann in anns:
         box = ann.get_bounding_box(dp.image_id)
         all_boxes.append(box.to_list(mode="xyxy"))
         all_categories.append(ann.category_id)
 
         if add_mask:
-            raise NotImplementedError
+            raise NotImplementedError()
 
     output["gt_boxes"] = np.asarray(all_boxes, dtype="float32")
     output["gt_labels"] = np.asarray(all_categories, dtype="int32")
     if not os.path.isfile(dp.location) and dp.image is None:
         return None
 
     output["file_name"] = dp.location  # full path
```

### Comparing `deepdoctection-0.30/deepdoctection/mapper/xfundstruct.py` & `deepdoctection-0.31/deepdoctection/mapper/xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/pipe/__init__.py` & `deepdoctection-0.31/deepdoctection/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/pipe/anngen.py` & `deepdoctection-0.31/deepdoctection/pipe/anngen.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,28 +38,31 @@
 
     When the image is transferred, the annotations are stored in a cache dictionary so that access via the annotation ID
     can be performed efficiently.
 
     The manager is part of each `PipelineComponent`.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, service_id: str, model_id: Optional[str] = None) -> None:
         self._datapoint: Optional[Image] = None
         self._cache_anns: Dict[str, ImageAnnotation] = {}
         self.datapoint_is_passed: bool = False
         self.category_id_mapping: Optional[Mapping[int, int]] = None
+        self.service_id = service_id
+        self.model_id = model_id
+        self.session_id: Optional[str] = None
 
     @property
     def datapoint(self) -> Image:
         """
         datapoint
         """
         if self._datapoint is not None:
             return self._datapoint
-        raise ValueError("no datapoint passed")
+        raise ValueError("No datapoint passed")
 
     @datapoint.setter
     def datapoint(self, dp: Image) -> None:
         """
         datapoint
         """
         self._datapoint = dp
@@ -150,14 +153,17 @@
                     self.datapoint.height,
                 )
             ann = ImageAnnotation(
                 category_name=detect_result.class_name,
                 bounding_box=box,
                 category_id=str(detect_result.class_id),
                 score=detect_result.score,
+                service_id=self.service_id,
+                model_id=self.model_id,
+                session_id=self.session_id,
             )
             if to_annotation_id is not None:
                 parent_ann = self._cache_anns[to_annotation_id]
                 if parent_ann.image is None:
                     raise ValueError("image cannot be None")
                 parent_ann.image.dump(ann)
                 parent_ann.image.image_ann_to_image(ann.annotation_id)
@@ -204,15 +210,22 @@
             filter_level="annotation",
             category_annotation={
                 "category_name": category_name.value,
                 "sub_cat_key": sub_cat_key.value,
                 "annotation_id": annotation_id,
             },
         ) as annotation_context:
-            cat_ann = CategoryAnnotation(category_name=category_name, category_id=str(category_id), score=score)
+            cat_ann = CategoryAnnotation(
+                category_name=category_name,
+                category_id=str(category_id),
+                score=score,
+                service_id=self.service_id,
+                model_id=self.model_id,
+                session_id=self.session_id,
+            )
             self._cache_anns[annotation_id].dump_sub_category(sub_cat_key, cat_ann)
         if annotation_context.context_error:
             return None
         return cat_ann.annotation_id
 
     def set_container_annotation(
         self,
@@ -242,26 +255,32 @@
                 "category_name": category_name.value,
                 "sub_cat_key": sub_cat_key.value,
                 "annotation_id": annotation_id,
                 "value": str(value),
             },
         ) as annotation_context:
             cont_ann = ContainerAnnotation(
-                category_name=category_name, category_id=str(category_id), value=value, score=score
+                category_name=category_name,
+                category_id=str(category_id),
+                value=value,
+                score=score,
+                service_id=self.service_id,
+                model_id=self.model_id,
+                session_id=self.session_id,
             )
             self._cache_anns[annotation_id].dump_sub_category(sub_cat_key, cont_ann)
         if annotation_context.context_error:
             return None
         return cont_ann.annotation_id
 
     def set_summary_annotation(
         self,
         summary_key: ObjectTypes,
         summary_name: ObjectTypes,
-        summary_number: int,
+        summary_number: Optional[int] = None,
         summary_value: Optional[str] = None,
         summary_score: Optional[float] = None,
         annotation_id: Optional[str] = None,
     ) -> Optional[str]:
         """
         Creates a sub category of a summary annotation. If a summary of the given `annotation_id` does not exist, it
         will create a new one.
@@ -290,24 +309,32 @@
             summary_annotation={
                 "summary_key": summary_key.value,
                 "summary_name": summary_name.value,
                 "summary_value": summary_value,
                 "annotation_id": annotation_id,
             },
         ) as annotation_context:
-            if summary_value:
+            if summary_value is not None:
                 ann = ContainerAnnotation(
                     category_name=summary_name,
-                    category_id=str(summary_number),
+                    category_id=str(summary_number) if summary_number is not None else "",
                     value=summary_value,
                     score=summary_score,
+                    service_id=self.service_id,
+                    model_id=self.model_id,
+                    session_id=self.session_id,
                 )
             else:
                 ann = CategoryAnnotation(
-                    category_name=summary_name, category_id=str(summary_number), score=summary_score
+                    category_name=summary_name,
+                    category_id=str(summary_number) if summary_number is not None else "",
+                    score=summary_score,
+                    service_id=self.service_id,
+                    model_id=self.model_id,
+                    session_id=self.session_id,
                 )
             image.summary.dump_sub_category(summary_key, ann, image.image_id)
 
         if annotation_context.context_error:
             return None
         return ann.annotation_id
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/base.py` & `deepdoctection-0.31/deepdoctection/pipe/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 """
 Module for the base class for building pipelines
 """
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from copy import deepcopy
 from typing import Any, Callable, DefaultDict, Dict, List, Mapping, Optional, Set, Union
+from uuid import uuid1
 
 from ..dataflow import DataFlow, MapData
 from ..datapoint.image import Image
 from ..extern.base import ImageTransformer, ObjectDetector, PdfMiner, TextRecognizer
 from ..utils.context import timed_operation
 from ..utils.detection_types import JsonDict
+from ..utils.identifier import get_uuid_from_str
 from .anngen import DatapointManager
 
 
 class PipelineComponent(ABC):
     """
     Base class for pipeline components. Pipeline components are the parts that make up a pipeline. They contain the
     abstract `serve`, in which the component steps are defined. Within pipelines, pipeline components take an
@@ -54,16 +56,17 @@
 
     def __init__(self, name: str):
         """
         :param name: The name of the pipeline component. The name will be used to identify a pipeline component in a
                      pipeline. Use something that describe the task of the pipeline.
         """
         self.name = name
+        self.service_id = self.get_service_id()
         self._meta_has_all_types()
-        self.dp_manager = DatapointManager()
+        self.dp_manager = DatapointManager(self.service_id)
         self.timer_on = False
 
     @abstractmethod
     def serve(self, dp: Image) -> None:
         """
         Processing an image through the whole pipeline component. Abstract method that contains all processing steps of
         the component. Please note that dp is already available to the dp_manager and operations for this can be carried
@@ -71,15 +74,15 @@
 
         dp was transferred to the dp_manager via an assignment. This means that operations on dp directly or operations
         via dp_manager are equivalent.
 
         As a simplified interface `serve` does not have to return a dp. The data point is passed on within
         pipelines internally (via `pass_datapoint`).
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def pass_datapoint(self, dp: Image) -> Image:
         """
         Acceptance, handover to dp_manager, transformation and forwarding of dp. To measure the time, use
 
             self.timer_on = True
 
@@ -105,38 +108,44 @@
         return MapData(df, self.pass_datapoint)
 
     @abstractmethod
     def clone(self) -> "PipelineComponent":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def get_meta_annotation(self) -> JsonDict:
         """
         Get a dict of list of annotation type. The dict must contain
 
         `image_annotation` with values: a list of category names,
         `sub_categories` with values: a dict with category names as keys and a list of the generated sub categories
         `relationships` with values: a dict with category names as keys and a list of the generated relationships
         `summaries` with values: A list of summary sub categories
         :return: Dict with meta infos as just described
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def _meta_has_all_types(self) -> None:
         if not {"image_annotations", "sub_categories", "relationships", "summaries"}.issubset(
             set(self.get_meta_annotation().keys())
         ):
             raise TypeError(
                 f" 'get_meta_annotation' must return dict with all required keys. "
                 f"Got {self.get_meta_annotation().keys()}"
             )
 
+    def get_service_id(self) -> str:
+        """
+        Get the generating model
+        """
+        return get_uuid_from_str(self.name)[:8]
+
 
 class PredictorPipelineComponent(PipelineComponent, ABC):
     """
     Lightweight abstract pipeline component class with `predictor`. Object detectors that only read in images as
     numpy array and return `DetectResult`s are currently permitted.
     """
 
@@ -147,18 +156,19 @@
     ) -> None:
         """
         :param name: Will be passed to base class
         :param predictor: An Object detector for predicting
         """
         self.predictor = predictor
         super().__init__(name)
+        self.dp_manager = DatapointManager(self.service_id, self.predictor.model_id)
 
     @abstractmethod
     def clone(self) -> "PredictorPipelineComponent":
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class LanguageModelPipelineComponent(PipelineComponent, ABC):
     """
     Abstract pipeline component class with two attributes `tokenizer` and `language_model` .
     """
 
@@ -171,23 +181,23 @@
         """
         :param name: Will be passed to base class
         :param tokenizer: Tokenizer, typing allows currently anything. This will be changed in the future
         :param mapping_to_lm_input_func: Function mapping image to layout language model features
         """
 
         self.tokenizer = tokenizer
-        self.mapping_to_lm_input_func = mapping_to_lm_input_func
         super().__init__(name)
+        self.mapping_to_lm_input_func = mapping_to_lm_input_func
 
     @abstractmethod
     def clone(self) -> "LanguageModelPipelineComponent":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class ImageTransformPipelineComponent(PipelineComponent, ABC):
     """
     Abstract pipeline component class with one model to transform images. This component is meant to be used at the
     beginning of a pipeline
     """
@@ -202,15 +212,15 @@
         super().__init__(name)
 
     @abstractmethod
     def clone(self) -> "ImageTransformPipelineComponent":
         """
         Clone an instance
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class Pipeline(ABC):
     """
     Abstract base class for creating pipelines. Pipelines represent the framework with which documents can be processed
     by reading individual pages, processing the pages through the pipeline infrastructure and returning the extracted
     information.
@@ -224,48 +234,64 @@
 
     This creates a pipeline using the following command arrangement:
 
     **Example:**
 
             layout = LayoutPipeComponent(layout_detector ...)
             text = TextExtractPipeComponent(text_detector ...)
-            simple_pipe = MyPipeline (pipeline_component = [layout, text])
+            simple_pipe = MyPipeline(pipeline_component = [layout, text])
             doc_dataflow = simple_pipe.analyze(input = path / to / dir)
 
             for page in doc_dataflow:
                 print(page)
 
     In doing so, page contains all document structures determined via the pipeline (either directly from the Image core
     model or already processed further).
 
     In addition to `analyze`, the internal `_entry` is used to bundle preprocessing steps.
+
+    It is possible to set a session id for the pipeline. This is useful for logging purposes. The session id can be
+    either passed to the pipeline via the `analyze` method or generated automatically.
+
+    To generate a session_id automatically:
+
+    **Example:**
+
+           pipe = MyPipeline(pipeline_component = [layout, text])
+           pipe.set_session_id = True
+
+           df = pipe.analyze(input = "path/to/dir") # session_id is generated automatically
     """
 
     def __init__(self, pipeline_component_list: List[PipelineComponent]) -> None:
         """
         :param pipeline_component_list: A list of pipeline components.
         """
         self.pipe_component_list = pipeline_component_list
+        self.set_session_id = False
 
     @abstractmethod
     def _entry(self, **kwargs: Any) -> DataFlow:
         """
         Use this method to bundle all preprocessing, such as loading one or more documents, so that a dataflow is
         provided as a return value that can be passed on to the pipeline backbone.
 
         :param kwargs: Arguments, for dynamic customizing of the processing or for the transfer of processing types
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
-    def _build_pipe(self, df: DataFlow) -> DataFlow:
+    def _build_pipe(self, df: DataFlow, session_id: Optional[str] = None) -> DataFlow:
         """
         Composition of the backbone
         """
+        if session_id is None and self.set_session_id:
+            session_id = self.get_session_id()
         for component in self.pipe_component_list:
             component.timer_on = True
+            component.dp_manager.session_id = session_id
             df = component.predict_dataflow(df)
         return df
 
     @abstractmethod
     def analyze(self, **kwargs: Any) -> DataFlow:
         """
         Try to keep this method as the only one necessary for the user. All processing steps, such as preprocessing,
@@ -273,15 +299,15 @@
         generated via
 
             doc = iter(df)
             page = next(doc)
 
         can be triggered.
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def get_meta_annotation(self) -> JsonDict:
         """
         Collects meta annotations from all pipeline components and summarizes the returned results
 
         :return: Meta annotations with information about image annotations (list), sub categories (dict with category
                  names and generated sub categories), relationships (dict with category names and generated
@@ -297,26 +323,34 @@
             meta_anns = deepcopy(component.get_meta_annotation())
             pipeline_populations["image_annotations"].extend(meta_anns["image_annotations"])  # type: ignore
             for key, value in meta_anns["sub_categories"].items():
                 pipeline_populations["sub_categories"][key].update(value)
             for key, value in meta_anns["relationships"].items():
                 pipeline_populations["relationships"][key].update(value)
             pipeline_populations["summaries"].extend(meta_anns["summaries"])  # type: ignore
-
+        pipeline_populations["sub_categories"] = dict(pipeline_populations["sub_categories"])  # type: ignore
+        pipeline_populations["relationships"] = dict(pipeline_populations["relationships"])  # type: ignore
         return pipeline_populations
 
     def get_pipeline_info(
-        self, position: Optional[int] = None, name: Optional[str] = None
-    ) -> Union[Mapping[int, str], str, int]:
+        self, service_id: Optional[str] = None, name: Optional[str] = None
+    ) -> Union[str, Mapping[str, str]]:
         """Get pipeline information: Returns a dictionary with a description of each pipeline component
-        :param position: position of the pipeline component in the pipeline
+        :param service_id: service_id of the pipeline component to search for
         :param name: name of the pipeline component to search for
         :return: Either a full dictionary with position and name of all pipeline components or the name, if the position
                  has been passed or the position if the name has been passed.
         """
-        comp_info = {key: comp.name for key, comp in enumerate(self.pipe_component_list)}
+        comp_info = {comp.service_id: comp.name for comp in self.pipe_component_list}
         comp_info_name_as_key = {value: key for key, value in comp_info.items()}
-        if position is not None:
-            return comp_info[position]
+        if service_id is not None:
+            return comp_info[service_id]
         if name is not None:
             return comp_info_name_as_key[name]
         return comp_info
+
+    @staticmethod
+    def get_session_id() -> str:
+        """
+        Get the generating a session id
+        """
+        return str(uuid1())[:8]
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/cell.py` & `deepdoctection-0.31/deepdoctection/pipe/cell.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 """
 from collections import Counter
 from copy import deepcopy
 from typing import Dict, List, Mapping, Optional, Sequence, Union
 
 import numpy as np
 
+from ..datapoint.annotation import ImageAnnotation
+from ..datapoint.box import crop_box_from_image
 from ..datapoint.image import Image
 from ..extern.base import DetectionResult, ObjectDetector, PdfMiner
-from ..utils.detection_types import JsonDict
+from ..utils.detection_types import ImageType, JsonDict
 from ..utils.settings import ObjectTypes, Relationships
 from ..utils.transform import PadTransform
 from .base import PredictorPipelineComponent
 from .registry import pipeline_component_registry
 
 
 class DetectResultGenerator:
@@ -177,26 +179,22 @@
         - Selection of ImageAnnotation to present to the detector.
         - Invoke the detector
         - Optionally invoke the DetectResultGenerator
         - Generate ImageAnnotations and dump to parent image and sub image.
         """
         sub_image_anns = dp.get_annotation_iter(category_names=self.sub_image_name)
         for sub_image_ann in sub_image_anns:
-            if sub_image_ann.image is None:
-                raise ValueError("sub_image_ann.image is None, but must be an image")
-            np_image = sub_image_ann.image.image
-            if self.padder:
-                np_image = self.padder.apply_image(np_image)
-            detect_result_list = self.predictor.predict(np_image)
+            np_image = self.prepare_np_image(sub_image_ann)
+            detect_result_list = self.predictor.predict(np_image)  # type: ignore
             if self.padder and detect_result_list:
                 boxes = np.array([detect_result.box for detect_result in detect_result_list])
                 boxes_orig = self.padder.inverse_apply_coords(boxes)
                 for idx, detect_result in enumerate(detect_result_list):
                     detect_result.box = boxes_orig[idx, :].tolist()
-            if self.detect_result_generator:
+            if self.detect_result_generator and sub_image_ann.image:
                 self.detect_result_generator.width = sub_image_ann.image.width
                 self.detect_result_generator.height = sub_image_ann.image.height
                 detect_result_list = self.detect_result_generator.create_detection_result(detect_result_list)
 
             for detect_result in detect_result_list:
                 if self.category_id_mapping:
                     if detect_result.class_id:
@@ -231,7 +229,30 @@
         return self.__class__(
             predictor,
             deepcopy(self.sub_image_name),
             deepcopy(self.category_id_mapping),
             deepcopy(self.detect_result_generator),
             padder_clone,
         )
+
+    def prepare_np_image(self, sub_image_ann: ImageAnnotation) -> ImageType:
+        """Maybe crop and pad a np_array before passing it to the predictor.
+
+        Note that we currently assume to a two level hierachy of images, e.g. we can crop a sub-image from the base
+        image, e.g. the original input but we cannot crop a sub-image from an image which is itself a sub-image.
+
+        :param sub_image_ann: ImageAnnotation to be processed
+        :return: processed np_image
+        """
+        if sub_image_ann.image is None:
+            raise ValueError("sub_image_ann.image is None, but must be an datapoint.Image")
+        np_image = sub_image_ann.image.image
+        if np_image is None and self.dp_manager.datapoint.image is not None:
+            np_image = crop_box_from_image(
+                self.dp_manager.datapoint.image,
+                sub_image_ann.get_bounding_box(self.dp_manager.datapoint.image_id),
+                self.dp_manager.datapoint.width,
+                self.dp_manager.datapoint.height,
+            )
+        if self.padder:
+            np_image = self.padder.apply_image(np_image)
+        return np_image
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/common.py` & `deepdoctection-0.31/deepdoctection/pipe/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
             # Assigning means that text and title annotation will receive a relationship called "CHILD" which is a list
               of annotation ids of mapped words.
     """
 
     def __init__(
         self,
-        parent_categories: Union[TypeOrStr, List[TypeOrStr]],
-        child_categories: Union[TypeOrStr, List[TypeOrStr]],
+        parent_categories: Union[TypeOrStr, Sequence[TypeOrStr]],
+        child_categories: Union[TypeOrStr, Sequence[TypeOrStr]],
         matching_rule: Literal["iou", "ioa"],
         threshold: float,
         use_weighted_intersections: bool = False,
         max_parent_only: bool = False,
     ) -> None:
         """
         :param parent_categories: list of categories to be used a for parent class. Will generate a child-relationship
@@ -108,16 +108,24 @@
         :param use_weighted_intersections: This is currently only implemented for matching_rule 'ioa'. Instead of using
                                            the ioa_matrix it will use mat weighted ioa in order to take into account
                                            that intersections with more cells will likely decrease the ioa value. By
                                            multiplying the ioa with the number of all intersection for each child this
                                            value calibrate the ioa.
         :param max_parent_only: Will assign to each child at most one parent with maximum ioa
         """
-        self.parent_categories = parent_categories
-        self.child_categories = child_categories
+        self.parent_categories = (
+            [get_type(parent_categories)]  # type: ignore
+            if not isinstance(parent_categories, (list, set))
+            else [get_type(parent_category) for parent_category in parent_categories]
+        )
+        self.child_categories = (
+            [get_type(child_categories)]  # type: ignore
+            if not isinstance(child_categories, (list, set))
+            else [get_type(child_category) for child_category in child_categories]
+        )
         assert matching_rule in ["iou", "ioa"], "segment rule must be either iou or ioa"
         self.matching_rule = matching_rule
         self.threshold = threshold
         self.use_weighted_intersections = use_weighted_intersections
         self.max_parent_only = max_parent_only
         super().__init__("matching")
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/concurrency.py` & `deepdoctection-0.31/deepdoctection/pipe/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/pipe/doctectionpipe.py` & `deepdoctection-0.31/deepdoctection/pipe/doctectionpipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     else:
         file_name = dp["file_name"]
     if path is None:
         path_tmp = doc_path
     else:
         path_tmp = path
     logger.info(LoggingRecord(f"Processing {file_name}", {"path": path_tmp, "df": path_tmp, "file_name": file_name}))
-    # logger.info("Processing %s", file_name, {"path": path_tmp, "df": path_tmp, "file_name": file_name})
     return dp
 
 
 @curry
 def _to_image(dp: Union[str, Mapping[str, Union[str, bytes]]], dpi: Optional[int] = None) -> Optional[Image]:
     return to_image(dp, dpi)
 
@@ -217,16 +216,17 @@
 
         `kwargs key max_datapoints:` Stops processing as soon as max_datapoints images have been processed
 
         :return: dataflow
         """
 
         output = kwargs.get("output", "page")
+        session_id = kwargs.get("session_id")
         assert output in ("page", "image", "dict"), "output must be either page image or dict"
         df = self._entry(**kwargs)
-        df = self._build_pipe(df)
+        df = self._build_pipe(df, session_id=session_id)  # type: ignore
         if output == "page":
             df = self.dataflow_to_page(df)
         elif output == "dict":
             df = self.dataflow_to_page(df)
             df = MapData(df, lambda dp: dp.as_dict())
         return df
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/language.py` & `deepdoctection-0.31/deepdoctection/pipe/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from copy import copy, deepcopy
 from typing import Optional, Sequence
 
 from ..datapoint.image import Image
 from ..datapoint.view import Page
 from ..extern.base import LanguageDetector, ObjectDetector
 from ..utils.detection_types import JsonDict
+from ..utils.error import ImageError
 from ..utils.settings import PageType, TypeOrStr, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
 
 @pipeline_component_registry.register("LanguageDetectionService")
 class LanguageDetectionService(PipelineComponent):
@@ -82,27 +83,27 @@
 
     def serve(self, dp: Image) -> None:
         if self.text_detector is None:
             page = Page.from_image(dp, self.text_container, self.floating_text_block_categories)  # type: ignore
             text = page.text_no_line_break
         else:
             if dp.image is None:
-                raise ValueError("dp.image cannot be None")
+                raise ImageError("image cannot be None")
             detect_result_list = self.text_detector.predict(dp.image)
             # this is a concatenation of all detection result. No reading order
             text = " ".join([result.text for result in detect_result_list if result.text is not None])
         predict_result = self.predictor.predict(text)
         self.dp_manager.set_summary_annotation(
             PageType.language, PageType.language, 1, predict_result.text, predict_result.score
         )
 
     def clone(self) -> PipelineComponent:
         predictor = self.predictor.clone()
         if not isinstance(predictor, LanguageDetector):
-            raise ValueError(f"Predictor must be of type LanguageDetector, but is of type {type(predictor)}")
+            raise TypeError(f"Predictor must be of type LanguageDetector, but is of type {type(predictor)}")
         return self.__class__(
             predictor,
             copy(self.text_container),
             deepcopy(self.text_detector),
             deepcopy(self.floating_text_block_categories),
         )
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/layout.py` & `deepdoctection-0.31/deepdoctection/pipe/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from typing import Optional
 
 import numpy as np
 
 from ..datapoint.image import Image
 from ..extern.base import ObjectDetector, PdfMiner
 from ..utils.detection_types import JsonDict
+from ..utils.error import ImageError
 from ..utils.transform import PadTransform
 from .base import PredictorPipelineComponent
 from .registry import pipeline_component_registry
 
 
 @pipeline_component_registry.register("ImageLayoutService")
 class ImageLayoutService(PredictorPipelineComponent):
@@ -75,15 +76,15 @@
     def serve(self, dp: Image) -> None:
         if self.skip_if_layout_extracted:
             categories = self.predictor.possible_categories()  # type: ignore
             anns = dp.get_annotation(category_names=categories)
             if anns:
                 return
         if dp.image is None:
-            raise ValueError("image cannot be None")
+            raise ImageError("image cannot be None")
         np_image = dp.image
         if self.padder:
             np_image = self.padder.apply_image(np_image)
         detect_result_list = self.predictor.predict(np_image)  # type: ignore
         if self.padder and detect_result_list:
             boxes = np.array([detect_result.box for detect_result in detect_result_list])
             boxes_orig = self.padder.inverse_apply_coords(boxes)
@@ -110,9 +111,9 @@
 
     def clone(self) -> "PredictorPipelineComponent":
         predictor = self.predictor.clone()
         padder_clone = None
         if self.padder:
             padder_clone = self.padder.clone()
         if not isinstance(predictor, ObjectDetector):
-            raise ValueError(f"predictor must be of type ObjectDetector, but is of type {type(predictor)}")
+            raise TypeError(f"predictor must be of type ObjectDetector, but is of type {type(predictor)}")
         return self.__class__(predictor, self.to_image, self.crop_image, padder_clone, self.skip_if_layout_extracted)
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/lm.py` & `deepdoctection-0.31/deepdoctection/pipe/lm.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         use_xlm_tokenizer = False
         if tokenizer_class is not None:
             use_xlm_tokenizer = True
         tokenizer_reference = get_tokenizer_from_architecture(
             self.language_model.model.__class__.__name__, use_xlm_tokenizer
         )
         if not isinstance(self.tokenizer, type(tokenizer_reference)):
-            raise ValueError(
+            raise TypeError(
                 f"You want to use {type(self.tokenizer)} but you should use {type(tokenizer_reference)} "
                 f"in this framework"
             )
 
 
 @pipeline_component_registry.register("LMSequenceClassifierService")
 class LMSequenceClassifierService(LanguageModelPipelineComponent):
@@ -362,11 +362,11 @@
         use_xlm_tokenizer = False
         if tokenizer_class is not None:
             use_xlm_tokenizer = True
         tokenizer_reference = get_tokenizer_from_architecture(
             self.language_model.model.__class__.__name__, use_xlm_tokenizer
         )
         if not isinstance(self.tokenizer, type(tokenizer_reference)):
-            raise ValueError(
+            raise TypeError(
                 f"You want to use {type(self.tokenizer)} but you should use {type(tokenizer_reference)} "
                 f"in this framework"
             )
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/order.py` & `deepdoctection-0.31/deepdoctection/pipe/order.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/pipe/refine.py` & `deepdoctection-0.31/deepdoctection/pipe/refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.box import merge_boxes
 from ..datapoint.image import Image
 from ..extern.base import DetectionResult
 from ..mapper.maputils import MappingContextManager
 from ..utils.detection_types import JsonDict
+from ..utils.error import AnnotationError, ImageError
 from ..utils.settings import CellType, LayoutType, Relationships, TableType, get_type
 from .base import PipelineComponent
 from .registry import pipeline_component_registry
 
 __all__ = ["TableSegmentationRefinementService", "generate_html_string"]
 
 
@@ -298,15 +299,15 @@
     Takes the table segmentation by using table cells row number, column numbers etc. and generates a html
     representation.
 
     :param table: An annotation that has a not None image and fully segmented cell annotation.
     :return: HTML representation of the table
     """
     if table.image is None:
-        raise ValueError("table.image cannot be None")
+        raise ImageError("table.image cannot be None")
     table_image = table.image
     cells = table_image.get_annotation(
         category_names=[
             LayoutType.cell,
             CellType.header,
             CellType.body,
             CellType.spanning,
@@ -408,15 +409,15 @@
         ]
         super().__init__("table_segment_refine")
 
     def serve(self, dp: Image) -> None:
         tables = dp.get_annotation(category_names=self._table_name)
         for table in tables:
             if table.image is None:
-                raise ValueError("table.image cannot be None")
+                raise ImageError("table.image cannot be None")
             tiles_to_cells_list = tiles_to_cells(dp, table)
             connected_components, tile_to_cell_dict = connected_component_tiles(tiles_to_cells_list)
             rectangle_tiling = generate_rectangle_tiling(connected_components)
             rectangle_cells_list = rectangle_cells(rectangle_tiling, tile_to_cell_dict)
             for tiling, cells_to_merge in zip(rectangle_tiling, rectangle_cells_list):
                 no_context_error = True
                 if len(cells_to_merge) != 1:
@@ -460,22 +461,29 @@
             cells = table.image.get_annotation(category_names=self._cell_names)
             number_of_rows = max(int(cell.get_sub_category(CellType.row_number).category_id) for cell in cells)
             number_of_cols = max(int(cell.get_sub_category(CellType.column_number).category_id) for cell in cells)
             max_row_span = max(int(cell.get_sub_category(CellType.row_span).category_id) for cell in cells)
             max_col_span = max(int(cell.get_sub_category(CellType.column_span).category_id) for cell in cells)
             # TODO: the summaries should be sub categories of the underlying ann
             if table.image.summary is not None:
-                if TableType.number_of_rows in table.image.summary.sub_categories:
-                    table.get_summary(TableType.number_of_rows)
-                if TableType.number_of_columns in table.image.summary.sub_categories:
-                    table.get_summary(TableType.number_of_columns)
-                if TableType.max_row_span in table.image.summary.sub_categories:
-                    table.get_summary(TableType.max_row_span)
-                if TableType.max_col_span in table.image.summary.sub_categories:
-                    table.get_summary(TableType.max_col_span)
+                if (
+                    TableType.number_of_rows in table.image.summary.sub_categories
+                    and TableType.number_of_columns in table.image.summary.sub_categories
+                    and TableType.max_row_span in table.image.summary.sub_categories
+                    and TableType.max_col_span in table.image.summary.sub_categories
+                ):
+                    table.image.summary.remove_sub_category(TableType.number_of_rows)
+                    table.image.summary.remove_sub_category(TableType.number_of_columns)
+                    table.image.summary.remove_sub_category(TableType.max_row_span)
+                    table.image.summary.remove_sub_category(TableType.max_col_span)
+                else:
+                    raise AnnotationError(
+                        "Table summary does not contain sub categories TableType.number_of_rows, "
+                        "TableType.number_of_columns, TableType.max_row_span, TableType.max_col_span"
+                    )
 
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_rows, TableType.number_of_rows, number_of_rows, annotation_id=table.annotation_id
             )
             self.dp_manager.set_summary_annotation(
                 TableType.number_of_columns,
                 TableType.number_of_columns,
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/registry.py` & `deepdoctection-0.31/deepdoctection/pipe/registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/pipe/segment.py` & `deepdoctection-0.31/deepdoctection/pipe/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.box import BoundingBox, global_to_local_coords, intersection_boxes, iou
 from ..datapoint.image import Image
 from ..extern.base import DetectionResult
 from ..mapper.maputils import MappingContextManager
 from ..mapper.match import match_anns_by_intersection
 from ..utils.detection_types import JsonDict
+from ..utils.error import ImageError
 from ..utils.settings import CellType, LayoutType, ObjectTypes, Relationships, TableType
 from .base import PipelineComponent
 from .refine import generate_html_string
 from .registry import pipeline_component_registry
 
 __all__ = ["TableSegmentationService", "SegmentationResult", "PubtablesSegmentationService"]
 
@@ -132,20 +133,20 @@
     :return: Image
     """
 
     item_ann_ids = table.get_relationship(Relationships.child)
 
     rows = dp.get_annotation(category_names=row_name, annotation_ids=item_ann_ids)
     if table.image is None:
-        raise ValueError("table.image cannot be None")
+        raise ImageError("table.image cannot be None")
     table_embedding_box = table.get_bounding_box(dp.image_id)
 
     for row in rows:
         if row.image is None:
-            raise ValueError("row.image cannot be None")
+            raise ImageError("row.image cannot be None")
         row_embedding_box = row.get_bounding_box(dp.image_id)
         row_embedding_box.ulx = table_embedding_box.ulx + 1.0
         row_embedding_box.lrx = table_embedding_box.lrx - 1.0
 
         # updating all bounding boxes for rows
         row.image.set_embedding(
             row.annotation_id,
@@ -162,15 +163,15 @@
 
     choose_items_by_iou(dp, rows, remove_iou_threshold_rows)
 
     cols = dp.get_annotation(category_names=col_name, annotation_ids=item_ann_ids)
 
     for col in cols:
         if col.image is None:
-            raise ValueError("row.image cannot be None")
+            raise ImageError("row.image cannot be None")
         col_embedding_box = col.get_bounding_box(dp.image_id)
         col_embedding_box.uly = table_embedding_box.uly + 1.0
         col_embedding_box.lry = table_embedding_box.lry - 1.0
 
         # updating all bounding boxes for cols
         col.image.set_embedding(
             col.annotation_id,
@@ -190,27 +191,27 @@
     return dp
 
 
 def _tile_by_stretching_rows_left_and_rightwise(
     dp: Image, items: List[ImageAnnotation], table: ImageAnnotation, item_name: str
 ) -> None:
     if table.image is None:
-        raise ValueError("table.image cannot be None")
+        raise ImageError("table.image cannot be None")
     table_embedding_box = table.get_bounding_box(dp.image_id)
 
     tmp_item_xy = table_embedding_box.uly + 1.0 if item_name == LayoutType.row else table_embedding_box.ulx + 1.0
     tmp_item_table_xy = 1.0
     for idx, item in enumerate(items):
         with MappingContextManager(
             dp_name=dp.file_name,
             filter_level="bounding box",
             image_annotation={"category_name": item.category_name, "annotation_id": item.annotation_id},
         ):
             if item.image is None:
-                raise ValueError("item.image cannot be None")
+                raise ImageError("item.image cannot be None")
             item_embedding_box = item.get_bounding_box(dp.image_id)
             if idx != len(items) - 1:
                 next_item_embedding_box = items[idx + 1].get_bounding_box(dp.image_id)
                 tmp_next_item_xy = (
                     (item_embedding_box.lry + next_item_embedding_box.uly) / 2
                     if item_name == LayoutType.row
                     else (item_embedding_box.lrx + next_item_embedding_box.ulx) / 2
@@ -254,27 +255,27 @@
             tmp_item_table_xy = tmp_table_next_item_xy
 
 
 def _tile_by_stretching_rows_leftwise_column_downwise(
     dp: Image, items: List[ImageAnnotation], table: ImageAnnotation, item_name: str
 ) -> None:
     if table.image is None:
-        raise ValueError("table.image cannot be None")
+        raise ImageError("table.image cannot be None")
     table_embedding_box = table.get_bounding_box(dp.image_id)
 
     tmp_item_xy = table_embedding_box.uly + 1.0 if item_name == LayoutType.row else table_embedding_box.ulx + 1.0
     tmp_item_table_xy = 1.0
     for item in items:
         with MappingContextManager(
             dp_name=dp.file_name,
             filter_level="bounding box",
             image_annotation={"category_name": item.category_name, "annotation_id": item.annotation_id},
         ):
             if item.image is None:
-                raise ValueError("item.image cannot be None")
+                raise ImageError("item.image cannot be None")
             item_embedding_box = item.get_bounding_box(dp.image_id)
             new_embedding_box = BoundingBox(
                 ulx=item_embedding_box.ulx if item_name == LayoutType.row else tmp_item_xy,
                 uly=tmp_item_xy if item_name == LayoutType.row else item_embedding_box.uly,
                 lrx=item_embedding_box.lrx,
                 lry=item_embedding_box.lry,
                 absolute_coords=True,
@@ -335,17 +336,17 @@
     :return: Image
     """
 
     item_ann_ids = table.get_relationship(Relationships.child)
     items = dp.get_annotation(category_names=item_name, annotation_ids=item_ann_ids)
 
     items.sort(
-        key=lambda x: x.get_bounding_box(dp.image_id).cx
-        if item_name == LayoutType.column
-        else x.get_bounding_box(dp.image_id).cy
+        key=lambda x: (
+            x.get_bounding_box(dp.image_id).cx if item_name == LayoutType.column else x.get_bounding_box(dp.image_id).cy
+        )
     )
 
     if stretch_rule == "left":
         _tile_by_stretching_rows_leftwise_column_downwise(dp, items, table, item_name)
     else:
         _tile_by_stretching_rows_left_and_rightwise(dp, items, table, item_name)
 
@@ -733,17 +734,19 @@
                 dp = choose_items_by_iou(dp, items_proposals, self.item_iou_threshold, False, reference_items_proposals)
 
                 # new query of items so that we only get active annotations
                 items = dp.get_annotation(category_names=item_name, annotation_ids=item_ann_ids)
 
                 # we will assume that either all or no image attribute has been generated
                 items.sort(
-                    key=lambda x: x.get_bounding_box(dp.image_id).cx  # pylint: disable=W0640
-                    if item_name == LayoutType.column  # pylint: disable=W0640
-                    else x.get_bounding_box(dp.image_id).cy  # pylint: disable=W0640
+                    key=lambda x: (
+                        x.get_bounding_box(dp.image_id).cx  # pylint: disable=W0640
+                        if item_name == LayoutType.column  # pylint: disable=W0640
+                        else x.get_bounding_box(dp.image_id).cy  # pylint: disable=W0640
+                    )
                 )
 
                 for item_number, item in enumerate(items, 1):
                     self.dp_manager.set_category_annotation(
                         sub_item_name, item_number, sub_item_name, item.annotation_id
                     )
             raw_table_segments = segment_table(
@@ -935,17 +938,19 @@
                 item_name, sub_item_name = item_sub_item_name[0], item_sub_item_name[1]
                 if self.tile_table:
                     dp = tile_tables_with_items_per_table(dp, table, item_name, self.stretch_rule)
                 items = dp.get_annotation(category_names=item_name, annotation_ids=item_ann_ids)
 
                 # we will assume that either all or no image attribute has been generated
                 items.sort(
-                    key=lambda x: x.get_bounding_box(dp.image_id).cx
-                    if item_name == LayoutType.column  # pylint: disable=W0640
-                    else x.get_bounding_box(dp.image_id).cy
+                    key=lambda x: (
+                        x.get_bounding_box(dp.image_id).cx
+                        if item_name == LayoutType.column  # pylint: disable=W0640
+                        else x.get_bounding_box(dp.image_id).cy
+                    )
                 )
 
                 for item_number, item in enumerate(items, 1):
                     self.dp_manager.set_category_annotation(
                         sub_item_name, item_number, sub_item_name, item.annotation_id
                     )
             rows = dp.get_annotation(category_names=self.item_names[0], annotation_ids=item_ann_ids)
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/text.py` & `deepdoctection-0.31/deepdoctection/pipe/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import List, Optional, Sequence, Tuple, Union
 
 from ..datapoint.annotation import ImageAnnotation
 from ..datapoint.image import Image
 from ..extern.base import ObjectDetector, PdfMiner, TextRecognizer
 from ..extern.tessocr import TesseractOcrDetector
 from ..utils.detection_types import ImageType, JsonDict
+from ..utils.error import ImageError
 from ..utils.settings import PageType, TypeOrStr, WordType, get_type
 from .base import PredictorPipelineComponent
 from .registry import pipeline_component_registry
 
 __all__ = ["TextExtractionService"]
 
 
@@ -85,15 +86,18 @@
             [get_type(extract_from_roi)]
             if isinstance(extract_from_roi, str)
             else [get_type(roi_category) for roi_category in extract_from_roi]
         )
         super().__init__(self._get_name(text_extract_detector.name), text_extract_detector)
         if self.extract_from_category:
             if not isinstance(self.predictor, (ObjectDetector, TextRecognizer)):
-                raise TypeError("Predicting from a cropped image requires to pass an ObjectDetector or TextRecognizer.")
+                raise TypeError(
+                    f"Predicting from a cropped image requires to pass an ObjectDetector or "
+                    f"TextRecognizer. Got {type(self.predictor)}"
+                )
         if run_time_ocr_language_selection:
             assert isinstance(
                 self.predictor, TesseractOcrDetector
             ), "Only TesseractOcrDetector supports multiple languages"
 
         self.run_time_ocr_language_selection = run_time_ocr_language_selection
         self.skip_if_text_extracted = skip_if_text_extracted
@@ -167,21 +171,21 @@
 
         :param text_roi: `Image` or `ImageAnnotation`
         :return: pdf bytes or numpy array
         """
 
         if isinstance(text_roi, ImageAnnotation):
             if text_roi.image is None:
-                raise ValueError("text_roi.image cannot be None")
+                raise ImageError("text_roi.image cannot be None")
             if text_roi.image.image is None:
-                raise ValueError("text_roi.image.image cannot be None")
+                raise ImageError("text_roi.image.image cannot be None")
             return text_roi.image.image
         if isinstance(self.predictor, ObjectDetector):
             if not isinstance(text_roi, Image):
-                raise ValueError("text_roi must be an image")
+                raise ImageError("text_roi must be an image")
             return text_roi.image
         if isinstance(text_roi, list):
             assert all(roi.image is not None for roi in text_roi)
             assert all(roi.image.image is not None for roi in text_roi)  # type: ignore
             return [(roi.annotation_id, roi.image.image) for roi in text_roi]  # type: ignore
         if isinstance(self.predictor, PdfMiner) and text_roi.pdf_bytes is not None:
             return text_roi.pdf_bytes
@@ -197,26 +201,28 @@
                     f"{type(self.predictor)}"
                 )
             sub_cat_dict = {category: {WordType.characters} for category in self.predictor.possible_categories()}
         return dict(
             [
                 (
                     "image_annotations",
-                    self.predictor.possible_categories()
-                    if isinstance(self.predictor, (ObjectDetector, PdfMiner))
-                    else [],
+                    (
+                        self.predictor.possible_categories()
+                        if isinstance(self.predictor, (ObjectDetector, PdfMiner))
+                        else []
+                    ),
                 ),
                 ("sub_categories", sub_cat_dict),
                 ("relationships", {}),
                 ("summaries", []),
             ]
         )
 
     @staticmethod
     def _get_name(text_detector_name: str) -> str:
         return f"text_extract_{text_detector_name}"
 
     def clone(self) -> "PredictorPipelineComponent":
         predictor = self.predictor.clone()
         if not isinstance(predictor, (ObjectDetector, PdfMiner, TextRecognizer)):
-            raise ValueError(f"predictor must be of type ObjectDetector or PdfMiner, but is of type {type(predictor)}")
+            raise ImageError(f"predictor must be of type ObjectDetector or PdfMiner, but is of type {type(predictor)}")
         return self.__class__(predictor, deepcopy(self.extract_from_category), self.run_time_ocr_language_selection)
```

### Comparing `deepdoctection-0.30/deepdoctection/pipe/transform.py` & `deepdoctection-0.31/deepdoctection/pipe/transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 Module for transform style pipeline components. These pipeline components are used for various transforming operations
 on images (e.g. deskew, de-noising or more general GAN like operations.
 """
 
 from ..datapoint.image import Image
 from ..extern.base import ImageTransformer
 from ..utils.detection_types import JsonDict
-from ..utils.logger import LoggingRecord, logger
 from .base import ImageTransformPipelineComponent
 from .registry import pipeline_component_registry
 
 
 @pipeline_component_registry.register("SimpleTransformService")
 class SimpleTransformService(ImageTransformPipelineComponent):
     """
@@ -45,34 +44,42 @@
 
         :param transform_predictor: image transformer
         """
         super().__init__(self._get_name(transform_predictor.name), transform_predictor)
 
     def serve(self, dp: Image) -> None:
         if dp.annotations:
-            logger.warning(
-                LoggingRecord(
-                    f"{self.name} has already received image with image annotations. These annotations "
-                    f"will not be transformed and might cause unexpected output in your pipeline."
-                )
+            raise RuntimeError(
+                "SimpleTransformService receives datapoints with ÌmageAnnotations. This violates the "
+                "pipeline building API but this can currently be catched only at runtime. "
+                "Please make sure that this component is the first one in the pipeline."
             )
+
         if dp.image is not None:
-            np_image_transform = self.transform_predictor.transform(dp.image)
+            detection_result = self.transform_predictor.predict(dp.image)
+            transformed_image = self.transform_predictor.transform(dp.image, detection_result)
             self.dp_manager.datapoint.clear_image(True)
-            self.dp_manager.datapoint.image = np_image_transform
+            self.dp_manager.datapoint.image = transformed_image
+            self.dp_manager.set_summary_annotation(
+                summary_key=self.transform_predictor.possible_category(),
+                summary_name=self.transform_predictor.possible_category(),
+                summary_number=None,
+                summary_value=getattr(detection_result, self.transform_predictor.possible_category().value, None),
+                summary_score=detection_result.score,
+            )
 
     def clone(self) -> "SimpleTransformService":
         return self.__class__(self.transform_predictor)
 
     def get_meta_annotation(self) -> JsonDict:
         return dict(
             [
                 ("image_annotations", []),
                 ("sub_categories", {}),
                 ("relationships", {}),
-                ("summaries", []),
+                ("summaries", [self.transform_predictor.possible_category()]),
             ]
         )
 
     @staticmethod
     def _get_name(transform_name: str) -> str:
         return f"simple_transform_{transform_name}"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdoctection-0.30/deepdoctection/train/__init__.py` & `deepdoctection-0.31/deepdoctection/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/train/hf_detr_train.py` & `deepdoctection-0.31/deepdoctection/train/hf_detr_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,17 @@
             assert isinstance(comp, PredictorPipelineComponent)
             assert isinstance(comp.predictor, HFDetrDerivedDetector)
             comp.predictor.hf_detr_predictor = None
         self.build_eval_kwargs = build_eval_kwargs
 
     def evaluate(
         self,
-        eval_dataset: Optional[Dataset[Any]] = None,
-        ignore_keys: Optional[List[str]] = None,
-        metric_key_prefix: str = "eval",
+        eval_dataset: Optional[Dataset[Any]] = None,  # pylint: disable=W0613
+        ignore_keys: Optional[List[str]] = None,  # pylint: disable=W0613
+        metric_key_prefix: str = "eval",  # pylint: disable=W0613
     ) -> Dict[str, float]:
         """
         Overwritten method from `Trainer`. Arguments will not be used.
         """
         assert self.evaluator is not None
         assert self.evaluator.pipe_component is not None
 
@@ -189,17 +189,19 @@
 
     number_samples = len(dataset)
     conf_dict = {
         "output_dir": log_dir,
         "remove_unused_columns": False,
         "per_device_train_batch_size": 2,
         "max_steps": number_samples,
-        "evaluation_strategy": "steps"
-        if (dataset_val is not None and metric is not None and pipeline_component_name is not None)
-        else "no",
+        "evaluation_strategy": (
+            "steps"
+            if (dataset_val is not None and metric is not None and pipeline_component_name is not None)
+            else "no"
+        ),
         "eval_steps": 5000,
     }
 
     for conf in config_overwrite:
         key, val = conf.split("=", maxsplit=1)
         try:
             val = int(val)  # type: ignore
```

### Comparing `deepdoctection-0.30/deepdoctection/train/hf_layoutlm_train.py` & `deepdoctection-0.31/deepdoctection/train/hf_layoutlm_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     HFLayoutLmv3TokenClassifier,
 )
 from ..mapper.laylmstruct import LayoutLMDataCollator, image_to_raw_layoutlm_features
 from ..pipe.base import LanguageModelPipelineComponent
 from ..pipe.lm import get_tokenizer_from_architecture
 from ..pipe.registry import pipeline_component_registry
 from ..utils.env_info import get_device
+from ..utils.error import DependencyError
 from ..utils.file_utils import wandb_available
 from ..utils.logger import LoggingRecord, logger
 from ..utils.settings import DatasetType, LayoutType, ObjectTypes, WordType
 from ..utils.utils import string_to_dict
 
 if wandb_available():
     import wandb
@@ -176,23 +177,25 @@
         assert self.evaluator.pipe_component
         for comp in self.evaluator.pipe_component.pipe_components:
             comp.language_model.model = None  # type: ignore
         self.build_eval_kwargs = build_eval_kwargs
 
     def evaluate(
         self,
-        eval_dataset: Optional[Dataset[Any]] = None,
-        ignore_keys: Optional[List[str]] = None,
-        metric_key_prefix: str = "eval",
+        eval_dataset: Optional[Dataset[Any]] = None,  # pylint: disable=W0613
+        ignore_keys: Optional[List[str]] = None,  # pylint: disable=W0613
+        metric_key_prefix: str = "eval",  # pylint: disable=W0613
     ) -> Dict[str, float]:
         """
         Overwritten method from `Trainer`. Arguments will not be used.
         """
-        assert self.evaluator is not None
-        assert self.evaluator.pipe_component is not None
+        if self.evaluator is None:
+            raise ValueError("Evaluator not set up. Please use `setup_evaluator` before running evaluation")
+        if self.evaluator.pipe_component is None:
+            raise ValueError("Pipeline component not set up. Please use `setup_evaluator` before running evaluation")
 
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
         for comp in self.evaluator.pipe_component.pipe_components:
             comp.language_model.model = copy.deepcopy(self.model).eval()  # type: ignore
         if isinstance(self.build_eval_kwargs, dict):
             scores = self.evaluator.run(True, **self.build_eval_kwargs)
@@ -218,15 +221,15 @@
     elif model_type:
         model_cls, model_wrapper_cls, config_cls = _MODEL_TYPE_AND_TASK_TO_MODEL_CLASS[(model_type, dataset_type)]
         tokenizer_fast = _MODEL_TYPE_TO_TOKENIZER[(model_type, use_xlm_tokenizer)]
     else:
         raise KeyError("model_type and architectures not available in configs")
 
     if not model_cls:
-        raise ValueError("model not eligible to run with this framework")
+        raise UserWarning("model not eligible to run with this framework")
 
     return config_cls, model_cls, model_wrapper_cls, tokenizer_fast
 
 
 def train_hf_layoutlm(
     path_config_json: str,
     dataset_train: Union[str, DatasetBase],
@@ -343,15 +346,15 @@
                 categories=LayoutType.word,
                 sub_categories={LayoutType.word: [WordType.token_class]},
                 keys=False,
                 values_as_dict=True,
                 name_as_key=True,
             )[LayoutType.word][WordType.token_class]
     else:
-        raise ValueError("Dataset type not supported for training")
+        raise UserWarning("Dataset type not supported for training")
 
     config_cls, model_cls, model_wrapper_cls, tokenizer_fast = _get_model_class_and_tokenizer(
         path_config_json, dataset_type, use_xlm_tokenizer
     )
     image_to_raw_layoutlm_kwargs = {"dataset_type": dataset_type, "use_token_tag": use_token_tag}
     if segment_positions:
         image_to_raw_layoutlm_kwargs["segment_positions"] = segment_positions  # type: ignore
@@ -370,17 +373,19 @@
     # Need to set remove_unused_columns to False, as the DataCollator for column removal will remove some raw features
     # that are necessary for the tokenizer.
     conf_dict = {
         "output_dir": log_dir,
         "remove_unused_columns": False,
         "per_device_train_batch_size": 8,
         "max_steps": number_samples,
-        "evaluation_strategy": "steps"
-        if (dataset_val is not None and metric is not None and pipeline_component_name is not None)
-        else "no",
+        "evaluation_strategy": (
+            "steps"
+            if (dataset_val is not None and metric is not None and pipeline_component_name is not None)
+            else "no"
+        ),
         "eval_steps": 100,
         "use_wandb": False,
         "wandb_project": None,
         "wandb_repo": "deepdoctection",
         "sliding_window_stride": 0,
         "max_batch_size": 0,
     }
@@ -412,15 +417,15 @@
     wandb_project = conf_dict.pop("wandb_project")
     wandb_repo = conf_dict.pop("wandb_repo")
 
     # Initialize Wandb, if necessary
     run = None
     if use_wandb:
         if not wandb_available():
-            raise ModuleNotFoundError("WandB must be installed separately")
+            raise DependencyError("WandB must be installed separately")
         run = wandb.init(project=wandb_project, config=conf_dict)  # type: ignore
         run._label(repo=wandb_repo)  # type: ignore # pylint: disable=W0212
     else:
         os.environ["WANDB_DISABLED"] = "True"
 
     # Will inform about dataloader warnings if max_steps exceeds length of dataset
     if conf_dict["max_steps"] > number_samples:  # type: ignore
```

### Comparing `deepdoctection-0.30/deepdoctection/train/tp_frcnn_train.py` & `deepdoctection-0.31/deepdoctection/train/tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/__init__.py` & `deepdoctection-0.31/deepdoctection/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # File: __init__.py
 
 """
 Init file for utils package
 """
 from typing import Optional, Tuple, Union, no_type_check
 
+from .concurrency import *
 from .context import *
+from .env_info import *
+from .error import *
 from .file_utils import *
 from .fs import *
 from .identifier import *
 from .logger import *
 from .metacfg import *
 from .pdf_utils import *
 from .settings import *
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/concurrency.py` & `deepdoctection-0.31/deepdoctection/utils/concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 '"import prctl" failed! Install python-prctl so that processes can be cleaned with guarantee.', "warn"
             )
         return
     assert hasattr(
         prctl, "set_pdeathsig"
     ), "prctl.set_pdeathsig does not exist! Note that you need to install 'python-prctl' instead of 'prctl'."
     # is SIGHUP a good choice?
-    prctl.set_pdeathsig(signal.SIGHUP)
+    prctl.set_pdeathsig(signal.SIGHUP)  # pylint: disable=E1101
 
 
 # taken from https://github.com/tensorpack/dataflow/blob/master/dataflow/utils/concurrency.py
 
 
 @no_type_check
 def start_proc_mask_signal(proc):
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/context.py` & `deepdoctection-0.31/deepdoctection/utils/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         try:
             _, error_string = proc.communicate(timeout=seconds)
             yield error_string
         except subprocess.TimeoutExpired:
             proc.terminate()
             proc.kill()
             proc.returncode = -1
-            raise RuntimeError("Tesseract process timeout")  # pylint: disable=W0707
+            raise RuntimeError(f"timeout for process id: {proc.pid}")  # pylint: disable=W0707
     finally:
         if proc.stdin is not None:
             proc.stdin.close()
         if proc.stdout is not None:
             proc.stdout.close()
         if proc.stderr is not None:
             proc.stderr.close()
@@ -84,15 +84,15 @@
     """
     try:
         with NamedTemporaryFile(prefix=prefix, delete=False) as file:
             if isinstance(image, str):
                 yield file.name, path.realpath(path.normpath(path.normcase(image)))
                 return
             if isinstance(image, (np.ndarray, np.generic)):
-                input_file_name = file.name + ".PNG"
+                input_file_name = file.name + "_input.PNG"
                 viz_handler.write_image(input_file_name, image)
                 yield file.name, input_file_name
             if isinstance(image, bytes):
                 input_file_name = file.name
                 file.write(image)
                 file.flush()
                 yield file.name, input_file_name
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/detection_types.py` & `deepdoctection-0.31/deepdoctection/utils/detection_types.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/develop.py` & `deepdoctection-0.31/deepdoctection/utils/develop.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/env_info.py` & `deepdoctection-0.31/deepdoctection/utils/env_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 import ast
 import importlib
 import os
 import re
 import subprocess
 import sys
 from collections import defaultdict
-from typing import List, Optional, Tuple
+from typing import List, Literal, Optional, Tuple
 
 import numpy as np
 from tabulate import tabulate
 
 from .file_utils import (
     apted_available,
     aws_available,
@@ -416,15 +416,15 @@
     except AttributeError:
         data.append(("deepdoctection", "imported a wrong installation"))
 
     has_prctl = True
     try:
         import prctl  # type: ignore
 
-        _ = prctl.set_pdeathsig  # noqa
+        _ = prctl.set_pdeathsig  # pylint: disable=E1101
     except ModuleNotFoundError:
         has_prctl = False
     data.append(("python-prctl", str(has_prctl)))
 
     # print system compilers when extension fails to build
     if sys.platform != "win32":  # don't know what to do for windows
         data.append(("Plattform", sys.platform))
@@ -448,83 +448,116 @@
 
     if pytorch_available():
         env_str += collect_torch_env()
 
     return env_str
 
 
+def set_env(name: str, value: str) -> None:
+    """
+    Set an environment variable if it is not already set.
+
+    :param name: The name of the environment variable
+    :param value: The value of the environment variable
+    """
+
+    if os.environ.get(name):
+        return
+    os.environ[name] = value
+    return
+
+
 def auto_select_lib_and_device() -> None:
     """
     Select the DL library and subsequently the device.
     This will set environment variable `USE_TENSORFLOW`, `USE_PYTORCH` and `USE_CUDA`
 
     If TF is available, use TF unless a GPU is not available, in which case choose PT. If CUDA is not available and PT
     is not installed raise ImportError.
     """
 
+    # USE_TF and USE_TORCH are env variables that steer DL library selection for Doctr.
     if tf_available() and tensorpack_available():
         from tensorpack.utils.gpu import get_num_gpu  # pylint: disable=E0401
 
         if get_num_gpu() >= 1:
-            os.environ["USE_TENSORFLOW"] = "True"
-            os.environ["USE_PYTORCH"] = "False"
-            os.environ["USE_CUDA"] = "True"
-            os.environ["USE_MPS"] = "False"
+            set_env("USE_TENSORFLOW", "True")
+            set_env("USE_PYTORCH", "False")
+            set_env("USE_CUDA", "True")
+            set_env("USE_MPS", "False")
+            set_env("USE_TF", "TRUE")
+            set_env("USE_TORCH", "False")
             return
         if pytorch_available():
-            os.environ["USE_TENSORFLOW"] = "False"
-            os.environ["USE_PYTORCH"] = "True"
-            os.environ["USE_CUDA"] = "False"
+            set_env("USE_TENSORFLOW", "False")
+            set_env("USE_PYTORCH", "True")
+            set_env("USE_CUDA", "False")
+            set_env("USE_TF", "False")
+            set_env("USE_TORCH", "TRUE")
             return
         logger.warning(
             LoggingRecord("You have Tensorflow installed but no GPU is available. All Tensorflow models require a GPU.")
         )
+    if tf_available():
+        set_env("USE_TENSORFLOW", "False")
+        set_env("USE_PYTORCH", "False")
+        set_env("USE_CUDA", "False")
+        set_env("USE_TF", "AUTO")
+        set_env("USE_TORCH", "AUTO")
+        return
+
     if pytorch_available():
         import torch
 
         if torch.cuda.is_available():
-            os.environ["USE_TENSORFLOW"] = "False"
-            os.environ["USE_PYTORCH"] = "True"
-            os.environ["USE_CUDA"] = "True"
+            set_env("USE_TENSORFLOW", "False")
+            set_env("USE_PYTORCH", "True")
+            set_env("USE_CUDA", "True")
+            set_env("USE_TF", "False")
+            set_env("USE_TORCH", "TRUE")
             return
         if torch.backends.mps.is_available():
-            os.environ["USE_TENSORFLOW"] = "False"
-            os.environ["USE_PYTORCH"] = "True"
-            os.environ["USE_CUDA"] = "False"
-            os.environ["USE_MPS"] = "True"
+            set_env("USE_TENSORFLOW", "False")
+            set_env("USE_PYTORCH", "True")
+            set_env("USE_CUDA", "False")
+            set_env("USE_MPS", "True")
+            set_env("USE_TF", "False")
+            set_env("USE_TORCH", "TRUE")
             return
-        os.environ["USE_TENSORFLOW"] = "False"
-        os.environ["USE_PYTORCH"] = "True"
-        os.environ["USE_CUDA"] = "False"
-        os.environ["USE_MPS"] = "False"
+        set_env("USE_TENSORFLOW", "False")
+        set_env("USE_PYTORCH", "True")
+        set_env("USE_CUDA", "False")
+        set_env("USE_MPS", "False")
+        set_env("USE_TF", "AUTO")
+        set_env("USE_TORCH", "AUTO")
         return
     logger.warning(
         LoggingRecord(
             "Neither Tensorflow or Pytorch are available. You will not be able to use any Deep Learning "
             "model from the library."
         )
     )
 
 
-def get_device(ignore_cpu: bool = True) -> str:
+def get_device(ignore_cpu: bool = True) -> Literal["cuda", "mps", "cpu"]:
     """
     Device checks for running PyTorch with CUDA, MPS or optionall CPU.
     If nothing can be found and if `disable_cpu` is deactivated it will raise a `ValueError`
 
     :param ignore_cpu: Will not consider `cpu` as valid return value
     :return: Either cuda or mps
     """
 
     if ast.literal_eval(os.environ.get("USE_CUDA", "True")):
         return "cuda"
     if ast.literal_eval(os.environ.get("USE_MPS", "True")):
         return "mps"
     if not ignore_cpu:
         return "cpu"
-    raise ValueError("Could not find either GPU nor MPS")
+    raise RuntimeWarning("Could not find either GPU nor MPS")
 
 
 def auto_select_viz_library() -> None:
     """Setting PIL as default image library if cv2 is not installed"""
 
     # if env variables are already set, don't change them
     if os.environ.get("USE_DD_PILLOW") or os.environ.get("USE_DD_OPENCV"):
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/file_utils.py` & `deepdoctection-0.31/deepdoctection/utils/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from types import ModuleType
 from typing import Any, Tuple, Union, no_type_check
 
 import importlib_metadata
 from packaging import version
 
 from .detection_types import Requirement
+from .error import DependencyError
 from .logger import LoggingRecord, logger
 from .metacfg import AttrDict
 
 _GENERIC_ERR_MSG = "Please check the required version either in the docs or in the setup file"
 
 # Tensorflow and Tensorpack dependencies
 _TF_AVAILABLE = False
@@ -259,15 +260,15 @@
 def set_tesseract_path(tesseract_path: str) -> None:
     """Set the Tesseract path. If you have tesseract installed in Anaconda,
        you can use this function to set tesseract path.
 
     :param tesseract_path: Tesseract installation path.
     """
     if tesseract_path is None:
-        raise ValueError("tesseract_path is empty.")
+        raise TypeError("tesseract_path cannot be None")
 
     global _TESS_AVAILABLE  # pylint: disable=W0603
     global _TESS_PATH  # pylint: disable=W0603
 
     tesseract_flag = which(tesseract_path)
 
     if tesseract_flag is None:
@@ -284,33 +285,27 @@
     """
     return bool(_TESS_AVAILABLE)
 
 
 # copy paste from https://github.com/madmaze/pytesseract/blob/master/pytesseract/pytesseract.py
 
 
-class TesseractNotFound(BaseException):
-    """
-    Exception class for Tesseract being not found
-    """
-
-
 def get_tesseract_version() -> Union[int, version.Version]:
     """
     Returns Version object of the Tesseract version. We need at least Tesseract 3.05
     """
     try:
         output = subprocess.check_output(
             [_TESS_PATH, "--version"],
             stderr=subprocess.STDOUT,
             env=environ,
             stdin=subprocess.DEVNULL,
         )
     except OSError:
-        raise TesseractNotFound(_TESS_ERR_MSG) from OSError
+        raise DependencyError(_TESS_ERR_MSG) from OSError
 
     raw_version = output.decode("utf-8")
     str_version, *_ = raw_version.lstrip(string.printable[10:]).partition(" ")
     str_version, *_ = str_version.partition("-")
 
     current_version = version.parse(str_version)
 
@@ -344,20 +339,14 @@
 def pdf_to_cairo_available() -> bool:
     """
     Returns True if pdftocairo is installed
     """
     return bool(_PDF_TO_CAIRO_AVAILABLE)
 
 
-class PopplerNotFound(BaseException):
-    """
-    Exception class for Poppler being not found
-    """
-
-
 def get_poppler_version() -> Union[int, version.Version]:
     """
     Returns Version object of the Poppler version. We need at least Tesseract 3.05
     """
 
     if pdf_to_ppm_available():
         command = "pdftoppm"
@@ -367,15 +356,15 @@
         return 0
 
     try:
         output = subprocess.check_output(
             [command, "-v"], stderr=subprocess.STDOUT, env=environ, stdin=subprocess.DEVNULL
         )
     except OSError:
-        raise PopplerNotFound() from OSError
+        raise DependencyError(_POPPLER_ERR_MSG) from OSError
 
     raw_version = output.decode("utf-8")
     list_version = raw_version.split("\n", maxsplit=1)[0].split(" ")[-1].split(".")
 
     current_version = version.parse(".".join(list_version[:2]))
 
     return current_version
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/fs.py` & `deepdoctection-0.31/deepdoctection/utils/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,25 @@
 
 from .detection_types import ImageType, JsonDict, Pathlike
 from .develop import deprecated
 from .logger import LoggingRecord, logger
 from .pdf_utils import get_pdf_file_reader, get_pdf_file_writer
 from .settings import CONFIGS, DATASET_DIR, MODEL_DIR, PATH
 from .tqdm import get_tqdm
-from .utils import FileExtensionError, is_file_extension
+from .utils import is_file_extension
 from .viz import viz_handler
 
 __all__ = [
     "load_image_from_file",
     "load_bytes_from_pdf_file",
     "get_load_image_func",
     "maybe_path_or_pdf",
     "download",
     "mkdir_p",
-    "is_file_extension",
     "load_json",
-    "FileExtensionError",
     "sub_path",
     "get_package_path",
     "get_configs_dir_path",
     "get_weights_dir_path",
     "get_dataset_dir_path",
 ]
 
@@ -121,16 +119,16 @@
         size = stat_info.st_size
     except IOError:
         logger.error(LoggingRecord(f"Failed to download {url}"))
         raise
     assert size > 0, f"Downloaded an empty file from {url}!"
 
     if expect_size is not None and size != expect_size:
-        logger.error(LoggingRecord(f"File downloaded from {url} does not match the expected size!"))
-        logger.error(
+        logger.warning(LoggingRecord(f"File downloaded from {url} does not match the expected size!"))
+        logger.warning(
             LoggingRecord("You may have downloaded a broken file, or the upstream may have modified the file.")
         )
 
     logger.info(LoggingRecord(f"Successfully downloaded {file_name}. {sizeof_fmt(size)}."))
     return f_path
 
 
@@ -206,21 +204,23 @@
     """
     Return the loading function according to its file extension.
 
     :param path: Path to a file
     :return: The function loading the file (and converting to its desired format)
     """
 
-    assert is_file_extension(path, [".png", ".jpeg", ".jpg", ".pdf", ".tif"]), f"image type not allowed: {path}"
+    assert is_file_extension(path, [".png", ".jpeg", ".jpg", ".pdf", ".tif"]), f"image type not allowed: " f"{path}"
 
     if is_file_extension(path, [".png", ".jpeg", ".jpg", ".tif"]):
         return load_image_from_file
     if is_file_extension(path, [".pdf"]):
         return load_bytes_from_pdf_file
-    return NotImplemented
+    raise NotImplementedError(
+        "File extension not supported by any loader. Please specify a file type and raise an issue"
+    )
 
 
 def maybe_path_or_pdf(path: Pathlike) -> int:
     """
     Checks if the path points to a directory or a pdf document. Returns 1 if the path points to a directory, 2
     if the path points to a pdf doc or 0, if none of the previous is true.
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/identifier.py` & `deepdoctection-0.31/deepdoctection/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/logger.py` & `deepdoctection-0.31/deepdoctection/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/metacfg.py` & `deepdoctection-0.31/deepdoctection/utils/metacfg.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/pdf_utils.py` & `deepdoctection-0.31/deepdoctection/utils/pdf_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 from typing import Generator, List, Optional, Tuple
 
 from numpy import uint8
 from pypdf import PdfReader, PdfWriter, errors
 
 from .context import save_tmp_file, timeout_manager
 from .detection_types import ImageType, Pathlike
-from .file_utils import PopplerNotFound, pdf_to_cairo_available, pdf_to_ppm_available, qpdf_available
+from .error import DependencyError, FileExtensionError
+from .file_utils import pdf_to_cairo_available, pdf_to_ppm_available, qpdf_available
 from .logger import LoggingRecord, logger
-from .utils import FileExtensionError, is_file_extension
+from .utils import is_file_extension
 from .viz import viz_handler
 
 __all__ = ["decrypt_pdf_document", "get_pdf_file_reader", "get_pdf_file_writer", "PDFStreamer", "pdf_to_np_array"]
 
 
 def decrypt_pdf_document(path: Pathlike) -> bool:
     """
@@ -161,15 +162,15 @@
     cmd_args: List[str] = []
 
     if pdf_to_ppm_available():
         command = "pdftoppm"
     elif pdf_to_cairo_available():
         command = "pdftocairo"
     else:
-        raise PopplerNotFound("Poppler not found. Please install or add to your PATH.")
+        raise DependencyError("Poppler not found. Please install or add to your PATH.")
 
     if platform.system() == "Windows":
         command = command + ".exe"
     cmd_args.append(command)
     cmd_args.extend(["-r", str(dpi), str(input_file_name)])
     cmd_args.append("-png")
     cmd_args.append(str(output_file_name))
@@ -197,15 +198,15 @@
 
 def _run_poppler(poppler_args: List[str]) -> None:
     try:
         proc = subprocess.Popen(poppler_args)  # pylint: disable=R1732
     except OSError as error:
         if error.errno != ENOENT:
             raise error from error
-        raise PopplerNotFound("Poppler not found. Please install or add to your PATH.") from error
+        raise DependencyError("Poppler not found. Please install or add to your PATH.") from error
 
     with timeout_manager(proc, 0):
         if proc.returncode:
             raise PopplerError(status=proc.returncode, message="Syntax Error: PDF cannot be read with Poppler")
 
 
 def pdf_to_np_array(pdf_bytes: bytes, size: Optional[Tuple[int, int]] = None, dpi: int = 200) -> ImageType:
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/settings.py` & `deepdoctection-0.31/deepdoctection/utils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 @object_types_registry.register("PageType")
 class PageType(ObjectTypes):
     """Type for document page properties"""
 
     document_type = "document_type"
     language = "language"
+    angle = "angle"
 
 
 @object_types_registry.register("SummaryType")
 class SummaryType(ObjectTypes):
     """Summary type member"""
 
     summary = "summary"
@@ -121,14 +122,15 @@
     section_header = "section_header"
     page = "page"
     cell = "cell"
     row = "row"
     column = "column"
     word = "word"
     line = "line"
+    background = "background"
 
 
 @object_types_registry.register("TableType")
 class TableType(ObjectTypes):
     """Types for table properties"""
 
     item = "item"
@@ -320,15 +322,17 @@
 
     :param token: TokenClasses member
     :param tag: BioTag member
     :return: TokenClassWithTag member
     """
     if isinstance(token, TokenClasses) and isinstance(tag, BioTag):
         return _TOKEN_AND_TAG_TO_TOKEN_CLASS_WITH_TAG[(token, tag)]
-    raise TypeError("Token must be of type TokenClasses and tag must be of type BioTag")
+    raise TypeError(
+        f"Token must be of type TokenClasses, is of {type(token)} and tag " f"{type(tag)} must be of type BioTag"
+    )
 
 
 def token_class_with_tag_to_token_class_and_tag(
     token_class_with_tag: ObjectTypes,
 ) -> Optional[Tuple[ObjectTypes, ObjectTypes]]:
     """
     This is the reverse mapping from TokenClassWithTag members to TokenClasses and BioTag
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/tqdm.py` & `deepdoctection-0.31/deepdoctection/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/deepdoctection/utils/transform.py` & `deepdoctection-0.31/deepdoctection/utils/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     It should take and return a numpy array of Nx2, where each row is the (x, y) coordinate.
     The implementation of each method may choose to modify its input data in-place for efficient transformation.
     """
 
     @abstractmethod
     def apply_image(self, img: ImageType) -> ImageType:
         """The transformation that should be applied to the image"""
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class ResizeTransform(BaseTransform):
     """
     Resize the image.
     """
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/utils.py` & `deepdoctection-0.31/deepdoctection/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,20 +140,14 @@
     :param obj: some object to use to generate random seed.
     :return: np.random.RandomState: the RNG.
     """
     seed = (id(obj) + os.getpid() + int(datetime.now().strftime("%Y%m%d%H%M%S%f"))) % 4294967295
     return np.random.RandomState(seed)
 
 
-class FileExtensionError(BaseException):
-    """
-    An exception indicating that a file does not seem to have an expected type
-    """
-
-
 def is_file_extension(file_name: Pathlike, extension: Union[str, Sequence[str]]) -> bool:
     """
     Check if a given file name has a given extension
 
     :param file_name: the file name, either full along with path or as stand alone
     :param extension: the extension of the file. Must add a dot (.)
     :return: True/False
```

### Comparing `deepdoctection-0.30/deepdoctection/utils/viz.py` & `deepdoctection-0.31/deepdoctection/utils/viz.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 import numpy as np
 import numpy.typing as npt
 from numpy import float32, uint8
 
 from .detection_types import ImageType
 from .env_info import auto_select_viz_library
+from .error import DependencyError
 from .file_utils import get_opencv_requirement, get_pillow_requirement, opencv_available, pillow_available
 
 if opencv_available():
     import cv2
 
 if pillow_available():
     from PIL import Image, ImageDraw
@@ -303,26 +304,28 @@
             "convert_b64_to_np": "_cv2_convert_b64_to_np",
             "resize": "_cv2_resize",
             "get_text_size": "_cv2_get_text_size",
             "draw_rectangle": "_cv2_draw_rectangle",
             "draw_text": "_cv2_draw_text",
             "interactive_imshow": "_cv2_interactive_imshow",
             "encode": "_cv2_encode",
+            "rotate_image": "_cv2_rotate_image",
         },
         "pillow": {
             "read_image": "_pillow_read_image",
             "write_image": "_pillow_write_image",
             "convert_np_to_b64": "_pillow_convert_np_to_b64",
             "convert_b64_to_np": "_pillow_convert_b64_to_np",
             "resize": "_pillow_resize",
             "get_text_size": "_pillow_get_text_size",
             "draw_rectangle": "_pillow_draw_rectangle",
             "draw_text": "_pillow_draw_text",
             "interactive_imshow": "_pillow_interactive_imshow",
             "encode": "_pillow_encode",
+            "rotate_image": "_pillow_rotate_image",
         },
     }
 
     def __init__(self) -> None:
         """Selecting the image processing library and fonts"""
         package = self._select_package()
         self.pkg_func_dict: Dict[str, str] = {}
@@ -348,20 +351,20 @@
                 "Both variables USE_DD_OPENCV and USE_DD_PILLOW are set to True. Please set one of them to False."
             )
 
         # USE_DD_OPENCV has priority
         if maybe_cv2:
             requirements = get_opencv_requirement()
             if not requirements[1]:
-                raise ImportError(requirements[2])
+                raise DependencyError(requirements[2])
             return maybe_cv2
 
         requirements = get_pillow_requirement()
         if not requirements[1]:
-            raise ImportError(requirements[2])
+            raise DependencyError(requirements[2])
         return "pillow"
 
     def _set_vars(self, package: str) -> None:
         self.pkg_func_dict = self.PACKAGE_FUNCS[package]
         if package == "pillow":
             image = Image.fromarray(np.uint8(np.ones((1, 1, 3))))
             self.font = ImageDraw.ImageDraw(image).getfont()
@@ -686,10 +689,49 @@
 
     @staticmethod
     def _pillow_interactive_imshow(np_image: ImageType) -> None:
         name = "q, x: quit / s: save"
         pil_image = Image.fromarray(np.uint8(np_image[:, :, ::-1]))
         pil_image.show(name)
 
+    def rotate_image(self, np_image: ImageType, angle: int) -> ImageType:
+        """Rotating an image by some angle"""
+        return getattr(self, self.pkg_func_dict["rotate_image"])(np_image, angle)
+
+    @staticmethod
+    def _cv2_rotate_image(np_image: ImageType, angle: float) -> ImageType:
+        # copy & paste from https://stackoverflow.com/questions/43892506
+        # /opencv-python-rotate-image-without-cropping-sides
+
+        height, width = np_image.shape[:2]
+        image_center = (width / 2, height / 2)
+        rotation_mat = cv2.getRotationMatrix2D(center=image_center, angle=angle, scale=1.0)
+
+        # rotation calculates the cos and sin, taking absolutes of those.
+        abs_cos = abs(rotation_mat[0, 0])
+        abs_sin = abs(rotation_mat[0, 1])
+
+        # find the new width and height bounds
+        bound_w = int(height * abs_sin + width * abs_cos)
+        bound_h = int(height * abs_cos + width * abs_sin)
+
+        # subtract old image center (bringing image back to origo) and adding the new image center coordinates
+        rotation_mat[0, 2] += bound_w / 2 - image_center[0]
+        rotation_mat[1, 2] += bound_h / 2 - image_center[1]
+
+        np_image = cv2.warpAffine(  # type: ignore
+            src=np_image,
+            M=rotation_mat,
+            dsize=(bound_w, bound_h),
+        )
+
+        return np_image
+
+    @staticmethod
+    def _pillow_rotate_image(np_image: ImageType, angle: int) -> ImageType:
+        pil_image = Image.fromarray(np.uint8(np_image[:, :, ::-1]))
+        pil_image_rotated = pil_image.rotate(angle, expand=True)
+        return np.array(pil_image_rotated)[:, :, ::-1]
+
 
 auto_select_viz_library()
 viz_handler = VizPackageHandler()
```

### Comparing `deepdoctection-0.30/deepdoctection.egg-info/PKG-INFO` & `deepdoctection-0.31/deepdoctection.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdoctection
-Version: 0.30
+Version: 0.31
 Summary: Repository for Document AI
 Home-page: https://github.com/deepdoctection/deepdoctection
 Author: Dr. Janis Meyer
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -13,143 +13,116 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: catalogue==2.0.7
+Requires-Dist: catalogue==2.0.10
 Requires-Dist: huggingface_hub>=0.12.0
-Requires-Dist: importlib-metadata>=4.11.2
+Requires-Dist: importlib-metadata>=5.0.0
 Requires-Dist: jsonlines==3.1.0
 Requires-Dist: mock==4.0.3
 Requires-Dist: networkx>=2.7.1
 Requires-Dist: numpy>=1.21
 Requires-Dist: packaging>=20.0
 Requires-Dist: Pillow>=10.0.0
 Requires-Dist: pypdf>=3.16.0
-Requires-Dist: pyyaml==6.0
+Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: pyzmq>=16
 Requires-Dist: termcolor>=1.1
 Requires-Dist: tabulate>=0.7.7
 Requires-Dist: tqdm==4.64.0
 Provides-Extra: tf
-Requires-Dist: catalogue==2.0.7; extra == "tf"
+Requires-Dist: catalogue==2.0.10; extra == "tf"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "tf"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "tf"
+Requires-Dist: importlib-metadata>=5.0.0; extra == "tf"
 Requires-Dist: jsonlines==3.1.0; extra == "tf"
 Requires-Dist: mock==4.0.3; extra == "tf"
 Requires-Dist: networkx>=2.7.1; extra == "tf"
 Requires-Dist: numpy>=1.21; extra == "tf"
 Requires-Dist: packaging>=20.0; extra == "tf"
 Requires-Dist: Pillow>=10.0.0; extra == "tf"
 Requires-Dist: pypdf>=3.16.0; extra == "tf"
-Requires-Dist: pyyaml==6.0; extra == "tf"
+Requires-Dist: pyyaml>=6.0.1; extra == "tf"
 Requires-Dist: pyzmq>=16; extra == "tf"
 Requires-Dist: termcolor>=1.1; extra == "tf"
 Requires-Dist: tabulate>=0.7.7; extra == "tf"
 Requires-Dist: tqdm==4.64.0; extra == "tf"
-Requires-Dist: tensorpack; extra == "tf"
+Requires-Dist: tensorpack==0.11; extra == "tf"
 Requires-Dist: protobuf==3.20.1; extra == "tf"
 Requires-Dist: tensorflow-addons>=0.17.1; extra == "tf"
 Requires-Dist: tf2onnx>=1.9.2; extra == "tf"
 Requires-Dist: python-doctr==0.7.0; extra == "tf"
 Requires-Dist: pycocotools>=2.0.2; extra == "tf"
 Requires-Dist: boto3; extra == "tf"
 Requires-Dist: pdfplumber>=0.7.1; extra == "tf"
-Requires-Dist: fasttext; extra == "tf"
-Requires-Dist: jdeskew; extra == "tf"
+Requires-Dist: fasttext==0.9.2; extra == "tf"
+Requires-Dist: jdeskew>=0.2.2; extra == "tf"
 Requires-Dist: apted==1.0.3; extra == "tf"
 Requires-Dist: distance==0.1.3; extra == "tf"
 Requires-Dist: lxml>=4.9.1; extra == "tf"
 Provides-Extra: pt
-Requires-Dist: catalogue==2.0.7; extra == "pt"
+Requires-Dist: catalogue==2.0.10; extra == "pt"
 Requires-Dist: huggingface_hub>=0.12.0; extra == "pt"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "pt"
+Requires-Dist: importlib-metadata>=5.0.0; extra == "pt"
 Requires-Dist: jsonlines==3.1.0; extra == "pt"
 Requires-Dist: mock==4.0.3; extra == "pt"
 Requires-Dist: networkx>=2.7.1; extra == "pt"
 Requires-Dist: numpy>=1.21; extra == "pt"
 Requires-Dist: packaging>=20.0; extra == "pt"
 Requires-Dist: Pillow>=10.0.0; extra == "pt"
 Requires-Dist: pypdf>=3.16.0; extra == "pt"
-Requires-Dist: pyyaml==6.0; extra == "pt"
+Requires-Dist: pyyaml>=6.0.1; extra == "pt"
 Requires-Dist: pyzmq>=16; extra == "pt"
 Requires-Dist: termcolor>=1.1; extra == "pt"
 Requires-Dist: tabulate>=0.7.7; extra == "pt"
 Requires-Dist: tqdm==4.64.0; extra == "pt"
-Requires-Dist: timm; extra == "pt"
+Requires-Dist: timm>=0.9.16; extra == "pt"
 Requires-Dist: transformers>=4.36.0; extra == "pt"
-Requires-Dist: accelerate; extra == "pt"
+Requires-Dist: accelerate>=0.29.1; extra == "pt"
 Requires-Dist: python-doctr==0.7.0; extra == "pt"
 Requires-Dist: boto3; extra == "pt"
 Requires-Dist: pdfplumber>=0.7.1; extra == "pt"
-Requires-Dist: fasttext; extra == "pt"
-Requires-Dist: jdeskew; extra == "pt"
+Requires-Dist: fasttext==0.9.2; extra == "pt"
+Requires-Dist: jdeskew>=0.2.2; extra == "pt"
 Requires-Dist: apted==1.0.3; extra == "pt"
 Requires-Dist: distance==0.1.3; extra == "pt"
 Requires-Dist: lxml>=4.9.1; extra == "pt"
 Provides-Extra: docs
-Requires-Dist: tensorpack; extra == "docs"
+Requires-Dist: tensorpack==0.11; extra == "docs"
 Requires-Dist: boto3; extra == "docs"
 Requires-Dist: transformers>=4.36.0; extra == "docs"
-Requires-Dist: accelerate; extra == "docs"
+Requires-Dist: accelerate>=0.29.1; extra == "docs"
 Requires-Dist: pdfplumber>=0.7.1; extra == "docs"
 Requires-Dist: lxml>=4.9.1; extra == "docs"
-Requires-Dist: lxml-stubs; extra == "docs"
-Requires-Dist: jdeskew; extra == "docs"
+Requires-Dist: lxml-stubs>=0.5.1; extra == "docs"
+Requires-Dist: jdeskew>=0.2.2; extra == "docs"
 Requires-Dist: jinja2==3.0.3; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: griffe==0.25.0; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: python-dotenv==1.0.0; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: black==23.7.0; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: pylint==2.17.4; extra == "dev"
 Requires-Dist: mypy==1.4.1; extra == "dev"
 Requires-Dist: wandb; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
-Requires-Dist: types-termcolor==1.1.3; extra == "dev"
-Requires-Dist: types-tabulate; extra == "dev"
-Requires-Dist: types-tqdm; extra == "dev"
-Requires-Dist: lxml-stubs; extra == "dev"
-Requires-Dist: types-Pillow; extra == "dev"
-Requires-Dist: types-urllib3; extra == "dev"
+Requires-Dist: types-PyYAML>=6.0.12.12; extra == "dev"
+Requires-Dist: types-termcolor>=1.1.3; extra == "dev"
+Requires-Dist: types-tabulate>=0.9.0.3; extra == "dev"
+Requires-Dist: types-tqdm>=4.66.0.5; extra == "dev"
+Requires-Dist: lxml-stubs>=0.5.1; extra == "dev"
+Requires-Dist: types-Pillow>=10.2.0.20240406; extra == "dev"
+Requires-Dist: types-urllib3>=1.26.25.14; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest==8.0.2; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: hf
-Requires-Dist: catalogue==2.0.7; extra == "hf"
-Requires-Dist: huggingface_hub>=0.12.0; extra == "hf"
-Requires-Dist: importlib-metadata>=4.11.2; extra == "hf"
-Requires-Dist: jsonlines==3.1.0; extra == "hf"
-Requires-Dist: mock==4.0.3; extra == "hf"
-Requires-Dist: networkx>=2.7.1; extra == "hf"
-Requires-Dist: numpy>=1.21; extra == "hf"
-Requires-Dist: packaging>=20.0; extra == "hf"
-Requires-Dist: Pillow>=10.0.0; extra == "hf"
-Requires-Dist: pypdf>=3.16.0; extra == "hf"
-Requires-Dist: pyyaml==6.0; extra == "hf"
-Requires-Dist: pyzmq>=16; extra == "hf"
-Requires-Dist: termcolor>=1.1; extra == "hf"
-Requires-Dist: tabulate>=0.7.7; extra == "hf"
-Requires-Dist: tqdm==4.64.0; extra == "hf"
-Requires-Dist: timm; extra == "hf"
-Requires-Dist: transformers>=4.36.0; extra == "hf"
-Requires-Dist: accelerate; extra == "hf"
-Requires-Dist: python-doctr==0.7.0; extra == "hf"
-Requires-Dist: boto3; extra == "hf"
-Requires-Dist: pdfplumber>=0.7.1; extra == "hf"
-Requires-Dist: fasttext; extra == "hf"
-Requires-Dist: jdeskew; extra == "hf"
-Requires-Dist: apted==1.0.3; extra == "hf"
-Requires-Dist: distance==0.1.3; extra == "hf"
-Requires-Dist: lxml>=4.9.1; extra == "hf"
 
 
 <p align="center">
   <img src="https://github.com/deepdoctection/deepdoctection/raw/master/docs/tutorials/_imgs/dd_logo.png" alt="Deep Doctection Logo" width="60%">
   <h3 align="center">
   A Document AI Package
   </h3>
@@ -187,15 +160,17 @@
  - There is a small dataset for token classification [available](https://huggingface.co/datasets/deepdoctection/FRFPE)
    and a lot of new [tutorials](https://github.com/deepdoctection/notebooks/blob/main/Layoutlm_v2_on_custom_token_classification.ipynb) 
    to show, how to train and evaluate this dataset using LayoutLMv1, LayoutLMv2, LayoutXLM and LayoutLMv3.
  - Comprehensive configuration of **analyzer** like choosing different models, output parsing, OCR selection.
    Check this [notebook](https://github.com/deepdoctection/notebooks/blob/main/Analyzer_Configuration.ipynb) or the 
    [docs](https://deepdoctection.readthedocs.io/en/latest/tutorials/analyzer_configuration_notebook/) for more infos.
  - Document layout analysis and table recognition now runs with Torchscript (CPU) as well and Detectron2 is 
-   not required anymore for basic inference. 
+   not required anymore for basic inference.
+ - [**new**] More angle predictors for determining the rotation of a document based on Tesseract and DocTr 
+   (not contained in the built-in Analyzer).
 
 **deep**doctection provides on top of that methods for pre-processing inputs to models like cropping or resizing and to 
 post-process results, like validating duplicate outputs, relating words to detected layout segments or ordering words 
 into contiguous text. You will get an output in JSON format that you can customize even further by yourself. 
      
 Have a look at the [**introduction notebook**](https://github.com/deepdoctection/notebooks/blob/main/Get_Started.ipynb) in the 
 [notebook repo](https://github.com/deepdoctection/notebooks) for an easy start.
```

### Comparing `deepdoctection-0.30/deepdoctection.egg-info/SOURCES.txt` & `deepdoctection-0.31/deepdoctection.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 deepdoctection/train/tp_frcnn_train.py
 deepdoctection/utils/__init__.py
 deepdoctection/utils/concurrency.py
 deepdoctection/utils/context.py
 deepdoctection/utils/detection_types.py
 deepdoctection/utils/develop.py
 deepdoctection/utils/env_info.py
+deepdoctection/utils/error.py
 deepdoctection/utils/file_utils.py
 deepdoctection/utils/fs.py
 deepdoctection/utils/identifier.py
 deepdoctection/utils/logger.py
 deepdoctection/utils/metacfg.py
 deepdoctection/utils/pdf_utils.py
 deepdoctection/utils/settings.py
```

### Comparing `deepdoctection-0.30/deepdoctection.egg-info/requires.txt` & `deepdoctection-0.31/deepdoctection.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,107 @@
-catalogue==2.0.7
+catalogue==2.0.10
 huggingface_hub>=0.12.0
-importlib-metadata>=4.11.2
+importlib-metadata>=5.0.0
 jsonlines==3.1.0
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
-pyyaml==6.0
+pyyaml>=6.0.1
 pyzmq>=16
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
 
 [dev]
 python-dotenv==1.0.0
 click
 black==23.7.0
-isort
+isort==5.13.2
 pylint==2.17.4
 mypy==1.4.1
 wandb
-types-PyYAML
-types-termcolor==1.1.3
-types-tabulate
-types-tqdm
-lxml-stubs
-types-Pillow
-types-urllib3
+types-PyYAML>=6.0.12.12
+types-termcolor>=1.1.3
+types-tabulate>=0.9.0.3
+types-tqdm>=4.66.0.5
+lxml-stubs>=0.5.1
+types-Pillow>=10.2.0.20240406
+types-urllib3>=1.26.25.14
 
 [docs]
-tensorpack
+tensorpack==0.11
 boto3
 transformers>=4.36.0
-accelerate
+accelerate>=0.29.1
 pdfplumber>=0.7.1
 lxml>=4.9.1
-lxml-stubs
-jdeskew
+lxml-stubs>=0.5.1
+jdeskew>=0.2.2
 jinja2==3.0.3
 mkdocs-material
 mkdocstrings-python
 griffe==0.25.0
 
-[hf]
-catalogue==2.0.7
-huggingface_hub>=0.12.0
-importlib-metadata>=4.11.2
-jsonlines==3.1.0
-mock==4.0.3
-networkx>=2.7.1
-numpy>=1.21
-packaging>=20.0
-Pillow>=10.0.0
-pypdf>=3.16.0
-pyyaml==6.0
-pyzmq>=16
-termcolor>=1.1
-tabulate>=0.7.7
-tqdm==4.64.0
-timm
-transformers>=4.36.0
-accelerate
-python-doctr==0.7.0
-boto3
-pdfplumber>=0.7.1
-fasttext
-jdeskew
-apted==1.0.3
-distance==0.1.3
-lxml>=4.9.1
-
 [pt]
-catalogue==2.0.7
+catalogue==2.0.10
 huggingface_hub>=0.12.0
-importlib-metadata>=4.11.2
+importlib-metadata>=5.0.0
 jsonlines==3.1.0
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
-pyyaml==6.0
+pyyaml>=6.0.1
 pyzmq>=16
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
-timm
+timm>=0.9.16
 transformers>=4.36.0
-accelerate
+accelerate>=0.29.1
 python-doctr==0.7.0
 boto3
 pdfplumber>=0.7.1
-fasttext
-jdeskew
+fasttext==0.9.2
+jdeskew>=0.2.2
 apted==1.0.3
 distance==0.1.3
 lxml>=4.9.1
 
 [test]
-pytest
+pytest==8.0.2
 pytest-cov
 
 [tf]
-catalogue==2.0.7
+catalogue==2.0.10
 huggingface_hub>=0.12.0
-importlib-metadata>=4.11.2
+importlib-metadata>=5.0.0
 jsonlines==3.1.0
 mock==4.0.3
 networkx>=2.7.1
 numpy>=1.21
 packaging>=20.0
 Pillow>=10.0.0
 pypdf>=3.16.0
-pyyaml==6.0
+pyyaml>=6.0.1
 pyzmq>=16
 termcolor>=1.1
 tabulate>=0.7.7
 tqdm==4.64.0
-tensorpack
+tensorpack==0.11
 protobuf==3.20.1
 tensorflow-addons>=0.17.1
 tf2onnx>=1.9.2
 python-doctr==0.7.0
 pycocotools>=2.0.2
 boto3
 pdfplumber>=0.7.1
-fasttext
-jdeskew
+fasttext==0.9.2
+jdeskew>=0.2.2
 apted==1.0.3
 distance==0.1.3
 lxml>=4.9.1
```

### Comparing `deepdoctection-0.30/setup.cfg` & `deepdoctection-0.31/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/setup.py` & `deepdoctection-0.31/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,74 +38,74 @@
 sys.path.insert(0, ROOT)
 
 # Taken from https://github.com/huggingface/transformers/blob/master/setup.py. Will list all dependencies, even those
 # that need to be installed separately
 _DEPS = [
     # the minimum requirements to run pipelines without considering DL models specific dependencies
     "apted==1.0.3",
-    "catalogue==2.0.7",
+    "catalogue==2.0.10",
     "distance==0.1.3",
     "huggingface_hub>=0.12.0",
-    "importlib-metadata>=4.11.2",
+    "importlib-metadata>=5.0.0",
     "jsonlines==3.1.0",
     "lxml>=4.9.1",
     "mock==4.0.3",
     "networkx>=2.7.1",
     "numpy>=1.21",
     "opencv-python==4.8.0.76",  # this is not required anymore, but we keep its version as a reference
     "packaging>=20.0",
     "Pillow>=10.0.0",
     "pycocotools>=2.0.2",
     "pypdf>=3.16.0",
     "python-prctl",
-    "pyyaml==6.0",
+    "pyyaml>=6.0.1",
     "pyzmq>=16",
     "termcolor>=1.1",
     "tabulate>=0.7.7",
     "tqdm==4.64.0",
     # type-stubs
-    "types-PyYAML",
-    "types-termcolor==1.1.3",
-    "types-tabulate",
-    "types-tqdm",
-    "types-Pillow",
-    "types-urllib3",
-    "lxml-stubs",
+    "types-PyYAML>=6.0.12.12",
+    "types-termcolor>=1.1.3",
+    "types-tabulate>=0.9.0.3",
+    "types-tqdm>=4.66.0.5",
+    "types-Pillow>=10.2.0.20240406",
+    "types-urllib3>=1.26.25.14",
+    "lxml-stubs>=0.5.1",
     # Tensorflow related dependencies
     "protobuf==3.20.1",
-    "tensorpack",
+    "tensorpack==0.11",
     # PyTorch related dependencies
-    "timm",
+    "timm>=0.9.16",
     "transformers>=4.36.0",
-    "accelerate",
+    "accelerate>=0.29.1",
     # As maintenance of Detectron2 decreases, we will now use our own Fork the keep updating after rigorous testing.
     # This will hopefully prevent from issues like 233
-    "detectron2 @ git+https://github.com/deepdoctection/detectron2.git",
+    "detectron2 @ git+https://github.com/facebookresearch/detectron2.git",
     # other third party related dependencies (services or DL libraries). Must be installed by users
-    "jdeskew",
+    "jdeskew>=0.2.2",
     "boto3",
     "pdfplumber>=0.7.1",
     "tensorflow-addons>=0.17.1",
     "tf2onnx>=1.9.2",
     "python-doctr==0.7.0",
-    "fasttext",
+    "fasttext==0.9.2",
     # dev dependencies
     "python-dotenv==1.0.0",
     "click",  # version will not break black
     "black==23.7.0",
-    "isort",
+    "isort==5.13.2",
     "pylint==2.17.4",
     "mypy==1.4.1",
     # docs
     "jinja2==3.0.3",
     "mkdocs-material",
     "mkdocstrings-python",
     "griffe==0.25.0",
     # test
-    "pytest",
+    "pytest==8.0.2",
     "pytest-cov",
     "wandb",
 ]
 
 # lookup table with items like:
 # pycocotools: "pycocotools>=2.0.2"
 # tensorpack: "tensorpack"
@@ -149,15 +149,15 @@
 
 # Tensorflow dependencies. We also add pycocotools as they wouldn't have been added otherwise
 tf_deps = deps_list("tensorpack", "protobuf", "tensorflow-addons", "tf2onnx", "python-doctr", "pycocotools")
 
 # PyTorch dependencies
 pt_deps = deps_list("timm", "transformers", "accelerate", "python-doctr")
 
-source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/deepdoctection/detectron2.git")
+source_pt_deps = pt_deps + deps_list("detectron2 @ git+https://github.com/facebookresearch/detectron2.git")
 
 # Putting all together
 tf_deps = dist_deps + tf_deps + additional_deps
 pt_deps = dist_deps + pt_deps + additional_deps
 source_pt_deps = dist_deps + source_pt_deps + additional_deps
 
 
@@ -205,19 +205,18 @@
 # TODO: add function that lists correct not pre-installed third party libs in package, such that requirement errors
 #  can be printed with correct version dependencies.
 # when uploading to pypi first comment all source extra dependencies so that there are no dependencies to dataflow
 
 EXTRA_DEPS = {
     "tf": tf_deps,
     "pt": pt_deps,
-#    "source-pt": source_pt_deps,
+ #   "source-pt": source_pt_deps,
     "docs": docs_deps,
     "dev": dev_deps,
     "test": test_deps,
-    "hf": pt_deps,
 }
 
 setup(
     name="deepdoctection",
     version=get_version(),
     author="Dr. Janis Meyer",
     url="https://github.com/deepdoctection/deepdoctection",
```

### Comparing `deepdoctection-0.30/tests/__init__.py` & `deepdoctection-0.31/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/analyzer/__init__.py` & `deepdoctection-0.31/tests/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/analyzer/test_dd.py` & `deepdoctection-0.31/tests/analyzer/test_dd.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/conftest.py` & `deepdoctection-0.31/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Module for globally accessible fixtures
 """
-
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Mapping, Sequence, Tuple
 
 import numpy as np
 from pytest import fixture
```

### Comparing `deepdoctection-0.30/tests/data.py` & `deepdoctection-0.31/tests/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,47 +55,59 @@
 
     layout_anns = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=100.0, uly=160.0, lrx=200.0, lry=260.0, absolute_coords=True),
             score=0.63,
             category_name=LayoutType.title,
             category_id="2",
+            model_id="test_model",
+            service_id="d0b8e9f3",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=50.0, uly=50.0, lrx=150.0, lry=200.0, absolute_coords=True),
             score=0.97,
             category_name=LayoutType.table,
             category_id="4",
+            model_id="test_model",
+            service_id="d0b8e9f3",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=100.0, uly=320.0, lrx=150.0, lry=350.0, absolute_coords=True),
             score=0.53,
             category_name=LayoutType.text,
             category_id="1",
+            model_id="test_model",
+            service_id="d0b8e9f3",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=200.0, uly=50.0, lrx=250.0, lry=200.0, absolute_coords=True),
             score=0.83,
             category_name=LayoutType.table,
             category_id="4",
+            model_id="test_model",
+            service_id="d0b8e9f3",
         ),
     ]
 
     layout_ann_for_ordering = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=100.0, uly=160.0, lrx=200.0, lry=260.0, absolute_coords=True),
             score=0.9,
             category_name=LayoutType.title,
             category_id="2",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=100.0, uly=300.0, lrx=250.0, lry=350.0, absolute_coords=True),
             score=0.8,
             category_name=LayoutType.text,
             category_id="1",
+            model_id="test_model",
+            service_id="test_service",
         ),
     ]
 
     cell_detect_results = [
         [
             DetectionResult(box=[20.0, 20.0, 25.0, 30.0], score=0.8, class_id=1, class_name=CellType.header),
             DetectionResult(box=[40.0, 40.0, 50.0, 50.0], score=0.53, class_id=2, class_name=CellType.body),
@@ -106,28 +118,34 @@
     cell_layout_anns = [
         [
             ImageAnnotation(
                 bounding_box=BoundingBox(ulx=20.0, uly=20.0, lrx=25.0, lry=30.0, absolute_coords=True),
                 category_id="1",
                 category_name=CellType.header,
                 score=0.8,
+                model_id="test_model",
+                service_id="test_service",
             ),
             ImageAnnotation(
                 bounding_box=BoundingBox(ulx=40.0, uly=40.0, lrx=50.0, lry=50.0, absolute_coords=True),
                 category_id="2",
                 category_name=CellType.body,
                 score=0.53,
+                model_id="test_model",
+                service_id="test_service",
             ),
         ],
         [
             ImageAnnotation(
                 bounding_box=BoundingBox(ulx=15.0, uly=20.0, lrx=20.0, lry=30.0, absolute_coords=True),
                 category_id="1",
                 category_name=CellType.body,
                 score=0.4,
+                model_id="test_model",
+                service_id="test_service",
             )
         ],
     ]
 
     global_cell_boxes = [
         [
             BoundingBox(absolute_coords=True, ulx=70.0, uly=70.0, lrx=75.0, lry=80.0),
@@ -138,171 +156,191 @@
 
     table_layout_ann = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=100.0, uly=100.0, lrx=200.0, lry=400.0, absolute_coords=True),
             score=0.97,
             category_name=LayoutType.table,
             category_id="2",
+            model_id="test_model",
+            service_id="test_service",
         )
     ]
 
     cell_layout_anns_one_table = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=10.0, uly=100.0, lrx=20.0, lry=150.0, absolute_coords=True),
             score=0.8,
             category_name=LayoutType.cell,
             category_id="3",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=10.0, uly=200.0, lrx=20.0, lry=250.0, absolute_coords=True),
             score=0.7,
             category_name=LayoutType.cell,
             category_id="3",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=40.0, uly=100.0, lrx=50.0, lry=150.0, absolute_coords=True),
             score=0.6,
             category_name=LayoutType.cell,
             category_id="3",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=40.0, uly=200.0, lrx=50.0, lry=250.0, absolute_coords=True),
             score=0.5,
             category_name=LayoutType.cell,
             category_id="3",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=80.0, uly=260.0, lrx=90.0, lry=280.0, absolute_coords=True),
             score=0.4,
             category_name=LayoutType.cell,
             category_id="3",
+            model_id="test_model",
+            service_id="test_service",
         ),
     ]
 
     row_layout_anns = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=15.0, uly=100.0, lrx=60.0, lry=150.0, absolute_coords=True),
             score=0.8,
             category_name=LayoutType.row,
             category_id="6",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=15.0, uly=200.0, lrx=70.0, lry=240.0, absolute_coords=True),
             score=0.7,
             category_name=LayoutType.row,
             category_id="6",
+            model_id="test_model",
+            service_id="test_service",
         ),
     ]
 
     row_box_tiling_table = [
         BoundingBox(ulx=101.0, uly=101.0, lrx=199.0, lry=250.0, absolute_coords=True),
         BoundingBox(ulx=101.0, uly=250.0, lrx=199.0, lry=399.0, absolute_coords=True),
     ]
 
     col_layout_anns = [
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=10.0, uly=50.0, lrx=20.0, lry=250.0, absolute_coords=True),
             score=0.3,
             category_name=LayoutType.column,
             category_id="7",
+            model_id="test_model",
+            service_id="test_service",
         ),
         ImageAnnotation(
             bounding_box=BoundingBox(ulx=40.0, uly=20.0, lrx=50.0, lry=240.0, absolute_coords=True),
             score=0.2,
             category_name=LayoutType.column,
             category_id="7",
+            model_id="test_model",
+            service_id="test_service",
         ),
     ]
 
     col_box_tiling_table = [
         BoundingBox(ulx=101.0, uly=101.0, lrx=120.0, lry=399.0, absolute_coords=True),
         BoundingBox(ulx=120.0, uly=101.0, lrx=199.0, lry=399.0, absolute_coords=True),
     ]
 
     row_sub_cats = [
-        CategoryAnnotation(category_name=CellType.row_number, category_id="1"),
-        CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
+        CategoryAnnotation(category_name=CellType.row_number, category_id="1", service_id="dbf4f87c"),
+        CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
     ]
 
     col_sub_cats = [
-        CategoryAnnotation(category_name=CellType.column_number, category_id="1"),
-        CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
+        CategoryAnnotation(category_name=CellType.column_number, category_id="1", service_id="dbf4f87c"),
+        CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
     ]
 
     cell_sub_cats = [
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="0"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="0"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="0"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="0"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="0", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="0", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="0", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="0", service_id="dbf4f87c"),
         ),
     ]
 
     cell_sub_cats_when_table_fully_tiled = [
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
         (
-            CategoryAnnotation(category_name=CellType.row_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.column_number, category_id="2"),
-            CategoryAnnotation(category_name=CellType.row_span, category_id="1"),
-            CategoryAnnotation(category_name=CellType.column_span, category_id="1"),
+            CategoryAnnotation(category_name=CellType.row_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_number, category_id="2", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.row_span, category_id="1", service_id="dbf4f87c"),
+            CategoryAnnotation(category_name=CellType.column_span, category_id="1", service_id="dbf4f87c"),
         ),
     ]
 
     summary_sub_cat_when_table_fully_tiled = (
-        CategoryAnnotation(category_name=TableType.number_of_rows, category_id="2"),
-        CategoryAnnotation(category_name=TableType.number_of_columns, category_id="2"),
-        CategoryAnnotation(category_name=TableType.max_row_span, category_id="1"),
-        CategoryAnnotation(category_name=TableType.max_col_span, category_id="1"),
+        CategoryAnnotation(category_name=TableType.number_of_rows, category_id="2", service_id="dbf4f87c"),
+        CategoryAnnotation(category_name=TableType.number_of_columns, category_id="2", service_id="dbf4f87c"),
+        CategoryAnnotation(category_name=TableType.max_row_span, category_id="1", service_id="dbf4f87c"),
+        CategoryAnnotation(category_name=TableType.max_col_span, category_id="1", service_id="dbf4f87c"),
     )
 
     summary_htab_sub_cat = ContainerAnnotation(
         category_name=TableType.html, value="<table><tr><td></td><td></td></tr><tr><td></td><td></td></tr></table>"
     )
 
     word_results_list = [
@@ -1560,18 +1598,20 @@
     BAK = "BAK"
     BAK_1 = "BAK_1"
     BAK_11 = "BAK_11"
     BAK_12 = "BAK_12"
     BAK_21 = "BAK_21"
     BAK_22 = "BAK_22"
     BLA = "BLA"
+    BLU = "BLU"
     cat = "cat"
     FOO_1 = "FOO_1"
     FOO_2 = "FOO_2"
     FOO_3 = "FOO_3"
+    BLI = "BLI"
     FOOBAK = "FOOBAK"
     Test = "TEST"
     TEST_SUMMARY = "TEST_SUMMARY"
     baz = "baz"
     BAZ = "BAZ"
     b_foo = "B-FOO"
     i_foo = "I-FOO"
```

### Comparing `deepdoctection-0.30/tests/dataflow/__init__.py` & `deepdoctection-0.31/tests/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/conftest.py` & `deepdoctection-0.31/tests/dataflow/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/test_common.py` & `deepdoctection-0.31/tests/dataflow/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/test_custom.py` & `deepdoctection-0.31/tests/dataflow/test_custom.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/test_custom_serialize.py` & `deepdoctection-0.31/tests/dataflow/test_custom_serialize.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/test_parallel_map.py` & `deepdoctection-0.31/tests/dataflow/test_parallel_map.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/dataflow/test_stats.py` & `deepdoctection-0.31/tests/dataflow/test_stats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/__init__.py` & `deepdoctection-0.31/tests/datapoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/conftest.py` & `deepdoctection-0.31/tests/datapoint/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/test_annotation.py` & `deepdoctection-0.31/tests/datapoint/test_annotation.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/test_box.py` & `deepdoctection-0.31/tests/datapoint/test_box.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/test_convert.py` & `deepdoctection-0.31/tests/datapoint/test_convert.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datapoint/test_image.py` & `deepdoctection-0.31/tests/datapoint/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from numpy import float32, ones
 from numpy.testing import assert_array_equal
 from pytest import mark, raises
 
 from deepdoctection.dataflow import DataFlow, MapData, SerializerJsonlines
 from deepdoctection.datapoint import BoundingBox, CategoryAnnotation, Image, ImageAnnotation
 from deepdoctection.utils import get_uuid
+from deepdoctection.utils.error import ImageError
 from deepdoctection.utils.settings import get_type
 
 from ..test_utils import anns_to_ids, collect_datapoint_from_dataflow, get_test_path
 from .conftest import TestPdfPage, WhiteImage
 
 
 class TestImage:
@@ -78,15 +79,15 @@
         Once image_id is assigned, it cannot be reassigned
         :param image: test image
         """
         # Arrange
         test_image = Image(file_name=image.file_name, location=image.loc, external_id=image.external_id)
 
         # Act and assert
-        with raises(ValueError):
+        with raises(ImageError):
             test_image.image_id = "ec2aac06-c261-3669-b8bd-4486a54ce740"
 
     @staticmethod
     @mark.basic
     def test_image_stores_correct_image_and_meta(image: WhiteImage) -> None:
         """
         Image stores image given as np.array correctly. It returns height as width as expected
@@ -196,15 +197,15 @@
             category_id="1",
             bounding_box=BoundingBox(ulx=1.0, uly=1.0, width=1.0, height=2.0, absolute_coords=True),
         )
 
         # Act and Assert
         test_image.dump(cat)
 
-        with raises(ValueError):
+        with raises(ImageError):
             test_image.dump(cat)
 
     @staticmethod
     @mark.basic
     def test_get_annotation(image: WhiteImage) -> None:
         """
         Annotations are returned by conditions.
@@ -223,40 +224,75 @@
             bounding_box=BoundingBox(ulx=2.0, uly=2.0, width=2.0, height=2.0, absolute_coords=True),
         )
         cat_3 = ImageAnnotation(
             category_name="BAK",
             category_id="1",
             bounding_box=BoundingBox(ulx=1.5, uly=2.4, width=3.0, height=9.0, absolute_coords=True),
         )
+        cat_4 = ImageAnnotation(
+            category_name="BLI",
+            category_id="3",
+            bounding_box=BoundingBox(ulx=1.5, uly=2.4, width=3.0, height=9.0, absolute_coords=True),
+            service_id="test_service",
+        )
+        cat_5 = ImageAnnotation(
+            category_name="BLU",
+            category_id="5",
+            bounding_box=BoundingBox(ulx=1.5, uly=2.4, width=3.0, height=9.0, absolute_coords=True),
+            model_id="test_model",
+        )
 
         test_image.dump(cat_1)
         test_image.dump(cat_2)
         test_image.dump(cat_3)
+        test_image.dump(cat_4)
+        test_image.dump(cat_5)
 
         # Act
         filtered_anns_1 = test_image.get_annotation(category_names="FOO")
         filtered_anns_1_ids = anns_to_ids(filtered_anns_1)
+
         filtered_anns_2 = test_image.get_annotation(category_names="BLA")
         filtered_anns_2_ids = anns_to_ids(filtered_anns_2)
-        filtered_anns_3 = test_image.get_annotation(annotation_ids=[cat_1.annotation_id, cat_3.annotation_id])
 
+        filtered_anns_3 = test_image.get_annotation(annotation_ids=[cat_1.annotation_id, cat_3.annotation_id])
         filtered_anns_3_ids = anns_to_ids(filtered_anns_3)
+
         filtered_anns_4 = test_image.get_annotation(
             annotation_ids=[cat_2.annotation_id, cat_3.annotation_id],
         )
         filtered_anns_4_ids = anns_to_ids(filtered_anns_4)
+
         filtered_anns_5 = test_image.get_annotation_iter()
         filtered_anns_5_ids = anns_to_ids(filtered_anns_5)
 
+        filtered_anns_6 = test_image.get_annotation(service_id="test_service")
+        filtered_anns_6_ids = anns_to_ids(filtered_anns_6)
+
+        filtered_anns_7 = test_image.get_annotation(model_id="test_model")
+        filtered_anns_7_ids = anns_to_ids(filtered_anns_7)
+
+        filtered_anns_8 = test_image.get_annotation(service_id="test_model", annotation_ids=[cat_2.annotation_id])
+        filtered_anns_8_ids = anns_to_ids(filtered_anns_8)
+
         # Assert
         assert set(filtered_anns_1_ids) == {cat_1.annotation_id}
         assert set(filtered_anns_2_ids) == set()
         assert set(filtered_anns_3_ids) == {cat_1.annotation_id, cat_3.annotation_id}
         assert set(filtered_anns_4_ids) == {cat_2.annotation_id, cat_3.annotation_id}
-        assert set(filtered_anns_5_ids) == {cat_1.annotation_id, cat_2.annotation_id, cat_3.annotation_id}
+        assert set(filtered_anns_5_ids) == {
+            cat_1.annotation_id,
+            cat_2.annotation_id,
+            cat_3.annotation_id,
+            cat_4.annotation_id,
+            cat_5.annotation_id,
+        }
+        assert set(filtered_anns_6_ids) == {cat_4.annotation_id}
+        assert set(filtered_anns_7_ids) == {cat_5.annotation_id}
+        assert set(filtered_anns_8_ids) == set()
 
     @staticmethod
     @mark.basic
     def test_image_ann_to_image(image: WhiteImage) -> None:
         """
         test  image_ann_to_image add attr: image to ImageAnnotation and generates Image instance correctly
         """
@@ -303,14 +339,24 @@
         """
         test_file_path = get_test_path() / "test_image.json"
         image = Image.from_file(test_file_path.as_posix())
         assert isinstance(image, Image)
 
     @staticmethod
     @mark.basic
+    def test_load_image_from_legacy_test_file() -> None:
+        """
+        test class from_file returns an image
+        """
+        test_file_path = get_test_path() / "legacy_test_image.json"
+        image = Image.from_file(test_file_path.as_posix())
+        assert isinstance(image, Image)
+
+    @staticmethod
+    @mark.basic
     def test_state_id_changes_when_annotations_added(image: WhiteImage) -> None:
         """
         state_id changes when annotations are added
         """
 
         # Arrange
         test_image = Image(location=image.loc, file_name=image.file_name)
```

### Comparing `deepdoctection-0.30/tests/datapoint/test_view.py` & `deepdoctection-0.31/tests/datapoint/test_view.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/__init__.py` & `deepdoctection-0.31/tests/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/__init__.py` & `deepdoctection-0.31/tests/datasets/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/conftest.py` & `deepdoctection-0.31/tests/datasets/instances/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_doclaynet.py` & `deepdoctection-0.31/tests/datasets/instances/test_doclaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_fintabnet.py` & `deepdoctection-0.31/tests/datasets/instances/test_fintabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_funsd.py` & `deepdoctection-0.31/tests/datasets/instances/test_funsd.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     funsd.dataflow.get_workdir = get_test_path  # type: ignore
     funsd.dataflow.splits = {"test": ""}
     funsd.dataflow.annotation_files = {"test": ""}
     df = funsd.dataflow.build()
 
     # Act
     df_list = collect_datapoint_from_dataflow(df)
-    assert len(df_list) == 5  # the first four images coming from files not related to funsd data
-    dp = df_list[3]
+    assert len(df_list) == 6  # the first four images coming from files not related to funsd data
+    dp = [dp for dp in df_list if dp.file_name == "test_file_funsd.png"][0]
     word = dp.get_annotation(category_names=LayoutType.word)[0]
     assert word.get_sub_category(WordType.token_class) is not None
     assert word.get_sub_category(WordType.characters) is not None
     assert word.get_sub_category(WordType.tag) is not None
     assert word.get_sub_category(WordType.token_tag) is not None
 
     text = dp.get_annotation(category_names=LayoutType.text)[0]
```

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_iiitar13k.py` & `deepdoctection-0.31/tests/datasets/instances/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_layouttest.py` & `deepdoctection-0.31/tests/datasets/instances/test_layouttest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_publaynet.py` & `deepdoctection-0.31/tests/datasets/instances/test_publaynet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_pubtables1m.py` & `deepdoctection-0.31/tests/datasets/instances/test_pubtables1m.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_pubtabnet.py` & `deepdoctection-0.31/tests/datasets/instances/test_pubtabnet.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/instances/test_rvlcdip.py` & `deepdoctection-0.31/tests/datasets/instances/test_rvlcdip.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/test_adapter.py` & `deepdoctection-0.31/tests/datasets/test_adapter.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/datasets/test_info.py` & `deepdoctection-0.31/tests/datasets/test_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,10 +264,10 @@
         """
 
         # Arrange
         cat_1, cat_2 = TestMergeDatasetCategories.setup()
         merge = get_merged_categories(cat_1, cat_2)
 
         # Act & Assert
-        with pytest.raises(PermissionError):
+        with pytest.raises(RuntimeWarning):
             merge.filter_categories(categories="BAZ")
             merge.set_cat_to_sub_cat({"FOO": "FOO_1"})
```

### Comparing `deepdoctection-0.30/tests/datasets/test_registry.py` & `deepdoctection-0.31/tests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/__init__.py` & `deepdoctection-0.31/tests/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/conftest.py` & `deepdoctection-0.31/tests/eval/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/test_accmetric.py` & `deepdoctection-0.31/tests/eval/test_accmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/test_cocometric.py` & `deepdoctection-0.31/tests/eval/test_cocometric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/test_eval.py` & `deepdoctection-0.31/tests/eval/test_eval.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/test_registry.py` & `deepdoctection-0.31/tests/eval/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/eval/test_tedsmetric.py` & `deepdoctection-0.31/tests/eval/test_tedsmetric.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/extern/conftest.py` & `deepdoctection-0.31/tests/extern/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 """
 Fixtures for extern package testing
 """
 from typing import List
 
 from pytest import fixture
 
+from deepdoctection.extern.base import DetectionResult
 from deepdoctection.utils.detection_types import JsonDict
 
 from ..data import get_textract_response
 from ..mapper.data import DatapointXfund
-from .data import PDF_BYTES, PDF_BYTES_2, get_detr_categories
+from .data import ANGLE_RESULT, PDF_BYTES, PDF_BYTES_2, get_detr_categories
 
 
 @fixture(name="layoutlm_input_for_predictor")
 def fixture_layoutlm_input_for_predictor() -> JsonDict:
     """
     Layoutlm input
     """
@@ -87,13 +88,21 @@
 def fixture_pdf_bytes_page_2() -> bytes:
     """
     fixture pdf bytes
     """
     return PDF_BYTES_2
 
 
+@fixture(name="angle_detection_result")
+def fixture_angle_detection_result() -> DetectionResult:
+    """
+    fixture detection result for running rotation image transformation
+    """
+    return ANGLE_RESULT
+
+
 @fixture(name="detr_categories")
 def fixture_detr_categories() -> JsonDict:
     """
     fixture object types
     """
     return get_detr_categories()
```

### Comparing `deepdoctection-0.30/tests/extern/data.py` & `deepdoctection-0.31/tests/extern/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         block="1",
         line="2",
         class_id=1,
         class_name=LayoutType.word,
     ),
 ]
 
+ANGLE_RESULT = DetectionResult(angle=90.0, score=8.73)
+
 
 def get_detr_categories() -> JsonDict:
     """detr_categories"""
     return {
         "1": LayoutType.table,
         "2": LayoutType.column,
         "3": LayoutType.row,
```

### Comparing `deepdoctection-0.30/tests/extern/test_deskew.py` & `deepdoctection-0.31/tests/extern/test_deskew.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Testing module extern.deskew
 """
+import os
+from ast import literal_eval
 
 from numpy.testing import assert_array_equal
 from pytest import mark
 
 from deepdoctection.extern.deskew import Jdeskewer
 from deepdoctection.utils.fs import load_image_from_file
 from tests.test_utils import get_test_path
@@ -30,28 +32,36 @@
 class TestJdeskewer:
     """
     Test Jdeskewer
     """
 
     @staticmethod
     @mark.additional
-    def test_deskewer_transforms_image() -> None:
+    def test_deskewer_predicts_angle_and_transforms_image() -> None:
         """
         Detector deskews image and rotates it accordingly
         """
 
         # Arrange
         test_path_input_image = get_test_path() / "skewed_input.png"
-        test_path_gt_image = get_test_path() / "skewed_gt.png"
+
+        if literal_eval(os.environ["USE_DD_OPENCV"]):
+            test_path_gt_image = get_test_path() / "skewed_gt_opencv.png"
+        else:
+            test_path_gt_image = get_test_path() / "skewed_gt_pil.png"
 
         image = load_image_from_file(test_path_input_image)
         image_gt = load_image_from_file(test_path_gt_image)
 
         deskewer = Jdeskewer()
 
         # Act
         assert image is not None
-        output_image = deskewer.transform(image)
+        detect_result = deskewer.predict(image)
 
         # Assert
+        assert detect_result.angle == 4.5326
+
+        # Act
+        output_image = deskewer.transform(image, detect_result)
         assert image_gt is not None
         assert_array_equal(image_gt, output_image)
```

### Comparing `deepdoctection-0.30/tests/extern/test_doctrocr.py` & `deepdoctection-0.31/tests/extern/test_doctrocr.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Testing module extern.doctrocr
 """
 
-
+import os
 from typing import List, Tuple
 from unittest.mock import MagicMock, patch
 
 from pytest import mark
 
 from deepdoctection.extern.base import DetectionResult
-from deepdoctection.extern.doctrocr import DoctrTextlineDetector, DoctrTextRecognizer
+from deepdoctection.extern.doctrocr import DocTrRotationTransformer, DoctrTextlineDetector, DoctrTextRecognizer
 from deepdoctection.extern.model import ModelCatalog, ModelDownloadManager
 from deepdoctection.utils.detection_types import ImageType
 from tests.data import Annotations
 
 
 def get_mock_word_results(np_img: ImageType, predictor, device) -> List[DetectionResult]:  # type: ignore  # pylint: disable=W0613
     """
@@ -86,14 +86,15 @@
         Detector calls doctr_predict_text_lines. Only runs in tf environment
         """
 
         # Arrange
         path_weights = ModelDownloadManager.maybe_download_weights_and_configs(
             "doctr/db_resnet50/tf/db_resnet50-adcafc63.zip"
         )
+        os.environ["USE_TENSORFLOW"] = "True"
         categories = ModelCatalog.get_profile("doctr/db_resnet50/tf/db_resnet50-adcafc63.zip").categories
         doctr = DoctrTextlineDetector("db_resnet50", path_weights, categories, "cpu")  # type: ignore
 
         # Act
         results = doctr.predict(np_image)
 
         # Assert
@@ -133,14 +134,57 @@
         Detector calls doctr_predict_text. Only runs in tf environment
         """
 
         # Arrange
         path_weights = ModelDownloadManager.maybe_download_weights_and_configs(
             "doctr/crnn_vgg16_bn/tf/crnn_vgg16_bn-76b7f2c6.zip"
         )
+        os.environ["USE_TENSORFLOW"] = "True"
         doctr = DoctrTextRecognizer("crnn_vgg16_bn", path_weights, "cpu")
 
         # Act
         results = doctr.predict(text_lines)
 
         # Assert
         assert len(results) == 2
+
+
+class TestDocTrRotationTransformer:
+    """
+    Test DocTrRotationTransformer
+    """
+
+    @staticmethod
+    @mark.pt_deps
+    @patch("deepdoctection.extern.doctrocr.estimate_orientation", MagicMock(return_value=180.0))
+    def test_doctr_rotation_transformer_predicts_image(np_image: ImageType) -> None:
+        """
+        DocTrRotationTransformer calls predict and returns correct DetectionResult
+        """
+
+        # Arrange
+        transformer = DocTrRotationTransformer()
+
+        # Act
+        result = transformer.predict(np_image)
+
+        # Assert
+        assert result.angle == 180.0
+
+    @staticmethod
+    @mark.pt_deps
+    def test_doctr_rotation_transformer_rotates_image(
+        np_image: ImageType, angle_detection_result: DetectionResult
+    ) -> None:
+        """
+        DocTrRotationTransformer calls transform and returns rotated image
+        """
+
+        # Arrange
+        transformer = DocTrRotationTransformer()
+
+        # Act
+        np_output = transformer.transform(np_image, angle_detection_result)
+
+        # Assert
+        assert np_output.shape[0] == np_image.shape[1]
+        assert np_output.shape[1] == np_image.shape[0]
```

### Comparing `deepdoctection-0.30/tests/extern/test_fastlang.py` & `deepdoctection-0.31/tests/extern/test_fastlang.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/extern/test_hfdetr.py` & `deepdoctection-0.31/tests/extern/test_hfdetr.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 class TestHFDetrDerivedDetector:
     """
     Test HFDetrDerivedDetector
     """
 
     @staticmethod
     @mark.pt_deps
-    @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.set_model", MagicMock(return_value=MagicMock()))
-    @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.set_pre_processor", MagicMock())
+    @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.get_model", MagicMock(return_value=MagicMock()))
+    @patch("deepdoctection.extern.hfdetr.HFDetrDerivedDetector.get_pre_processor", MagicMock())
     @patch("deepdoctection.extern.hfdetr.PretrainedConfig.from_pretrained", MagicMock())
     def test_hf_detr_predicts_image(detr_categories: Dict[str, ObjectTypes], np_image: ImageType) -> None:
         """
         D2 FRCNN calls predict_image and post processes DetectionResult correctly, e.g. adding class names
         """
 
         # Arrange
```

### Comparing `deepdoctection-0.30/tests/extern/test_hflayoutlm.py` & `deepdoctection-0.31/tests/extern/test_hflayoutlm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/extern/test_pdftext.py` & `deepdoctection-0.31/tests/extern/test_pdftext.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/extern/test_tessocr.py` & `deepdoctection-0.31/tests/extern/test_tessocr.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 """
 from typing import List
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from deepdoctection.extern.base import DetectionResult
-from deepdoctection.extern.tessocr import TesseractOcrDetector, tesseract_line_to_detectresult
+from deepdoctection.extern.tessocr import (
+    TesseractOcrDetector,
+    TesseractRotationTransformer,
+    tesseract_line_to_detectresult,
+)
 from deepdoctection.utils.detection_types import ImageType
-from deepdoctection.utils.file_utils import TesseractNotFound
+from deepdoctection.utils.error import DependencyError
 from tests.data import Annotations
 
 from .data import WORD_RESULTS
 
 
 @pytest.fixture(name="word_result_list_same_line")
 def fixture_pdf_bytes_page_2() -> List[DetectionResult]:
@@ -62,15 +66,15 @@
     ) -> None:
         """
         This tests shows that the dependency implementation of the base class and is representative for
         the dependency logic of all derived classes.
         """
 
         # Act and Assert
-        with pytest.raises(TesseractNotFound):
+        with pytest.raises(DependencyError):
             TesseractOcrDetector(path_yaml=path_to_tesseract_yaml)
 
     @staticmethod
     @pytest.mark.basic
     @patch("deepdoctection.utils.file_utils.get_tesseract_version", MagicMock(return_value=3.15))
     @patch("deepdoctection.extern.tessocr.predict_text", MagicMock(side_effect=get_mock_word_results))
     def test_tesseract_ocr_predicts_image(path_to_tesseract_yaml: str, np_image: ImageType) -> None:
@@ -99,7 +103,62 @@
 
     # Assert
     assert len(detect_result_list) == 3
     line_detect_result = detect_result_list[2]
     assert line_detect_result.box == [10.0, 10.0, 38.0, 24.0]
     assert line_detect_result.class_id == 2
     assert line_detect_result.text == "foo bak"
+
+
+class TestTesseractRotationTransformer:
+    """
+    Test TesseractRotationTransformer
+    """
+
+    @staticmethod
+    @pytest.mark.basic
+    @patch(
+        "deepdoctection.extern.tessocr.predict_rotation",
+        MagicMock(
+            return_value={
+                "Orientation confidence": "8.70",
+                "Orientation in degrees": "180",
+                "Page number": "0",
+                "Rotate": "180",
+                "Script": "Latin",
+                "Script confidence": "4.62",
+            }
+        ),
+    )
+    def test_tesseract_rotation_transformer_predicts_image(np_image: ImageType) -> None:
+        """
+        TesseractRotationTransformer calls predict and returns correct DetectionResult
+        """
+
+        # Arrange
+        tess = TesseractRotationTransformer()
+
+        # Act
+        result = tess.predict(np_image)
+
+        # Assert
+        assert result.angle == 180.0
+        assert result.score == 8.70
+
+    @staticmethod
+    @pytest.mark.basic
+    def test_tesseract_rotation_transformer_rotates_image(
+        np_image: ImageType, angle_detection_result: DetectionResult
+    ) -> None:
+        """
+        TesseractRotationTransformer rotates image according to angle_detection_result
+        """
+
+        # Arrange
+        tess = TesseractRotationTransformer()
+
+        # Act
+        np_output = tess.transform(np_image, angle_detection_result)
+
+        # Assert
+        assert np_output.shape[0] == np_image.shape[1]
+        assert np_output.shape[1] == np_image.shape[0]
```

### Comparing `deepdoctection-0.30/tests/extern/test_texocr.py` & `deepdoctection-0.31/tests/extern/test_texocr.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/extern/test_tpdetect.py` & `deepdoctection-0.31/tests/extern/test_tpdetect.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/__init__.py` & `deepdoctection-0.31/tests/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/conftest.py` & `deepdoctection-0.31/tests/mapper/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/data.py` & `deepdoctection-0.31/tests/mapper/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,16 +664,16 @@
 @dataclass
 class DatapointCoco:
     """
     Class for datapoint in coco annotation format
     """
 
     dp = _SAMPLE_COCO
-    white_image: ImageType = np.ones((794, 596, 3), dtype=np.int32) * 255  # type: ignore
-    white_image_string = convert_np_array_to_b64(white_image)
+    white_image = np.ones((794, 596, 3), dtype=np.uint8) * 255
+    white_image_string = convert_np_array_to_b64(white_image)  # type: ignore
     categories = {
         "1": LayoutType.text,
         "2": LayoutType.title,
         "3": LayoutType.table,
         "4": LayoutType.figure,
         "5": LayoutType.list,
     }
@@ -682,15 +682,15 @@
     def get_white_image(self, path: str, type_id: str = "np") -> Optional[Union[str, ImageType]]:
         """
         white image
         :return: np.array
         """
         if path == self.dp["file_name"]:
             if type_id == "np":
-                return self.white_image
+                return self.white_image # type: ignore
             return self.white_image_string
         return None
 
     def get_number_anns(self) -> int:
         """
         number of annotations
         """
@@ -733,25 +733,25 @@
     Class for datapoint in pubtabnet annotation format
     """
 
     dp = _SAMPLE_PUBTABNET
     categories = {"1": LayoutType.cell, "2": TableType.item, "3": LayoutType.table, "4": LayoutType.word}
     categories_as_names = {v: k for k, v in categories.items()}
     first_ann_box = Box(475, 162, 10, 9)
-    white_image: ImageType = np.ones((1334, 996, 3), dtype=np.int32) * 255  # type: ignore
-    white_image_string = convert_np_array_to_b64(white_image)
+    white_image = np.ones((1334, 996, 3), dtype=np.uint8) * 255
+    white_image_string = convert_np_array_to_b64(white_image)  # type: ignore
 
     def get_white_image(self, path: str, type_id: str = "np") -> Union[str, ImageType]:
         """
         white image
         :return: np.array
         """
         assert path is not None
         if type_id == "np":
-            return self.white_image
+            return self.white_image  # type: ignore
         return self.white_image_string
 
     def get_width(self) -> float:
         """
         width
         """
         return self.white_image.shape[1]
```

### Comparing `deepdoctection-0.30/tests/mapper/test_cats.py` & `deepdoctection-0.31/tests/mapper/test_cats.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_cocostruct.py` & `deepdoctection-0.31/tests/mapper/test_cocostruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_d2struct.py` & `deepdoctection-0.31/tests/mapper/test_d2struct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_hfstruct.py` & `deepdoctection-0.31/tests/mapper/test_hfstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_iiitar13k.py` & `deepdoctection-0.31/tests/mapper/test_iiitar13k.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_laylmstruct.py` & `deepdoctection-0.31/tests/mapper/test_laylmstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_misc.py` & `deepdoctection-0.31/tests/mapper/test_misc.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_prodigystruct.py` & `deepdoctection-0.31/tests/mapper/test_prodigystruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_pubstruct.py` & `deepdoctection-0.31/tests/mapper/test_pubstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_tpstruct.py` & `deepdoctection-0.31/tests/mapper/test_tpstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_utils.py` & `deepdoctection-0.31/tests/mapper/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/mapper/test_xfundstruct.py` & `deepdoctection-0.31/tests/mapper/test_xfundstruct.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/__init__.py` & `deepdoctection-0.31/tests/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_anngen.py` & `deepdoctection-0.31/tests/pipe/test_anngen.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def test_set_image_annotation(
         dp_image: Image, layout_detect_results: List[DetectionResult], layout_annotations: List[ImageAnnotation]
     ) -> None:
         """
         test set_image_annotation
         """
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="d0b8e9f3", model_id="test_model")
         dp_manager.datapoint = dp_image
 
         # Act
         ann_id = dp_manager.set_image_annotation(layout_detect_results[0])
 
         # Assert
         assert ann_id is not None
@@ -59,15 +59,15 @@
     @staticmethod
     @mark.basic
     def test_set_image_annotation_with_image(dp_image: Image, layout_detect_results: List[DetectionResult]) -> None:
         """
         test set_image_annotation with image_ann_to_image
         """
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="test_service", model_id="test_model")
         dp_manager.datapoint = dp_image
 
         # Act
         dp_manager.set_image_annotation(layout_detect_results[0], to_image=True)
 
         # Assert
         ann = dp_manager.datapoint.get_annotation()
@@ -78,15 +78,15 @@
     @mark.basic
     def test_set_image_annotation_to_image_ann(dp_image: Image, layout_detect_results: List[DetectionResult]) -> None:
         """
         test set_image_annotation with ann to image ann
         """
 
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="test_service", model_id="test_model")
         dp_manager.datapoint = dp_image
         img_ann_id = dp_manager.set_image_annotation(layout_detect_results[0], to_image=True)
 
         # Act
         ann_id = dp_manager.set_image_annotation(layout_detect_results[2], to_annotation_id=img_ann_id)
 
         # Assert
@@ -102,15 +102,15 @@
     @mark.basic
     def test_set_category_annotation(dp_image: Image, layout_detect_results: List[DetectionResult]) -> None:
         """
         test set_category_annotation
         """
 
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="test_service", model_id="test_model")
         dp_manager.datapoint = dp_image
         ann_id = dp_manager.set_image_annotation(layout_detect_results[0])
 
         # Act
         assert ann_id is not None
         dp_manager.set_category_annotation(get_type("foo"), 5, get_type("FOO"), ann_id, 0.8)
 
@@ -126,15 +126,15 @@
     @mark.basic
     def test_set_container_annotation(dp_image: Image, layout_detect_results: List[DetectionResult]) -> None:
         """
         test set_container_annotation
         """
 
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="test_service", model_id="test_model")
         dp_manager.datapoint = dp_image
         ann_id = dp_manager.set_image_annotation(layout_detect_results[0])
 
         # Act
         assert ann_id is not None
         cont_ann_id = dp_manager.set_container_annotation(
             get_type("foo"), 5, get_type("FOO"), ann_id, "hello world", 0.8
@@ -154,15 +154,15 @@
     @mark.basic
     def test_summary_annotation(dp_image: Image, layout_detect_results: List[DetectionResult]) -> None:
         """
         test summary_annotation
         """
 
         # Arrange
-        dp_manager = DatapointManager()
+        dp_manager = DatapointManager(service_id="test_service", model_id="test_model")
         dp_manager.datapoint = dp_image
         ann_id = dp_manager.set_image_annotation(layout_detect_results[0], to_image=True)
 
         # Act
         summ_id_1 = dp_manager.set_summary_annotation(get_type("foo"), get_type("foo"), 1)
         summ_id_2 = dp_manager.set_summary_annotation(get_type("bak"), get_type("bak"), 2, annotation_id=ann_id)
         ann = dp_manager.datapoint.get_annotation(annotation_ids=ann_id)
```

### Comparing `deepdoctection-0.30/tests/pipe/test_cell.py` & `deepdoctection-0.31/tests/pipe/test_cell.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._cell_detector = MagicMock(spec=ObjectDetector)
+        self._cell_detector.model_id = "test_model"
         self._cell_detector.name = "mock_cell_detector"
 
         self.sub_image_layout_service = SubImageLayoutService(self._cell_detector, LayoutType.table)
 
     @mark.basic
     def test_pass_datapoint(
         self,
@@ -117,7 +118,27 @@
         local_box_ftsc = first_table_second_cell.get_bounding_box(first_table_ann.annotation_id)
         assert local_box_ftsc == first_table_second_cell.bounding_box
 
         global_box_stfc = second_table_first_cell.get_bounding_box(dp.image_id)
         assert global_box_stfc == exp_global_boxes_scd_table[0]
         local_box_stfc = second_table_first_cell.get_bounding_box(second_table_ann.annotation_id)
         assert local_box_stfc == second_table_first_cell.bounding_box
+
+    def test_pass_datapoint_when_sub_images_do_not_have_a_crop(
+        self,
+        dp_image_with_layout_anns: Image,
+        cell_detect_results: List[List[DetectionResult]],
+    ) -> None:
+        """If an sub image does not have a crop, a ValueError was raised previously. Now it should be fixed."""
+
+        # Arrange
+        self._cell_detector.predict = MagicMock(side_effect=cell_detect_results)
+        for ann in dp_image_with_layout_anns.get_annotation():
+            if ann.image is not None:
+                ann.image.clear_image()
+
+        # Act
+
+        try:
+            self.sub_image_layout_service.pass_datapoint(dp_image_with_layout_anns)
+        except ValueError:
+            assert False, "ValueError was raised, because the sub image does not have a crop"
```

### Comparing `deepdoctection-0.30/tests/pipe/test_common.py` & `deepdoctection-0.31/tests/pipe/test_common.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_language.py` & `deepdoctection-0.31/tests/pipe/test_language.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_layout.py` & `deepdoctection-0.31/tests/pipe/test_layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._layout_detector = MagicMock(spec=ObjectDetector)
         self._layout_detector.name = "mock_cell_detector"
+        self._layout_detector.model_id = "test_model"
         self.image_layout_service = ImageLayoutService(self._layout_detector, to_image=True)
 
     @mark.basic
     def test_pass_datapoint(
         self, dp_image: Image, layout_detect_results: DetectionResult, layout_annotations: ImageAnnotation
     ) -> None:
         """
```

### Comparing `deepdoctection-0.30/tests/pipe/test_lm.py` & `deepdoctection-0.31/tests/pipe/test_lm.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_order.py` & `deepdoctection-0.31/tests/pipe/test_order.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_refine.py` & `deepdoctection-0.31/tests/pipe/test_refine.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_registry.py` & `deepdoctection-0.31/tests/pipe/test_registry.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_segment.py` & `deepdoctection-0.31/tests/pipe/test_segment.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/pipe/test_text.py` & `deepdoctection-0.31/tests/pipe/test_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._text_extract_detector = MagicMock(spec=ObjectDetector)
         self._text_extract_detector.name = "mock_text_extractor"
+        self._text_extract_detector.model_id = "test_model"
         self.text_extraction_service = TextExtractionService(self._text_extract_detector)
 
     @mark.basic
     def test_integration_pipeline_component(
         self, dp_image_fully_segmented_fully_tiled: Image, word_detect_result: List[DetectionResult]
     ) -> None:
         """
@@ -74,14 +75,15 @@
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._text_extract_detector = MagicMock(spec=PdfMiner)
         self._text_extract_detector.name = "mock_pdfminer"
+        self._text_extract_detector.model_id = "test_model"
         self.text_extraction_service = TextExtractionService(self._text_extract_detector)
 
     @mark.basic
     def test_integration_pipeline_component(
         self, dp_image_fully_segmented_fully_tiled: Image, word_detect_result: List[DetectionResult]
     ) -> None:
         """
@@ -109,14 +111,15 @@
     """
     Testing TextExtractionService does not build when instantiating with a PdfMiner and passing some ROI
     """
 
     # Arrange
     text_extract_detector = MagicMock(spec=PdfMiner)
     text_extract_detector.name = "mock_pdfminer"
+    text_extract_detector.model_id = "test_model"
 
     # Act and Assert
     with raises(TypeError):
         TextExtractionService(text_extract_detector, extract_from_roi=LayoutType.table)
 
 
 class TestTextExtractionServiceWithSubImage:
@@ -128,14 +131,15 @@
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._text_extract_detector = MagicMock(spec=ObjectDetector, accepts_batch=False)
         self._text_extract_detector.name = "mock_text_extractor"
+        self._text_extract_detector.model_id = "test_model"
         self.text_extraction_service = TextExtractionService(
             self._text_extract_detector, extract_from_roi=LayoutType.table
         )
 
     @mark.basic
     def test_integration_pipeline_component(
         self,
```

### Comparing `deepdoctection-0.30/tests/pipe/test_transform.py` & `deepdoctection-0.31/tests/pipe/test_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,29 @@
 import numpy as np
 from numpy.testing import assert_array_equal
 from pytest import mark
 
 from deepdoctection.datapoint.image import Image
 from deepdoctection.extern.base import ImageTransformer
 from deepdoctection.pipe.transform import SimpleTransformService
+from deepdoctection.utils.settings import PageType
 
 
 class TestSimpleTransformService:
     """
     Test SimpleTransformService
     """
 
     def setup_method(self) -> None:
         """
         setup necessary components
         """
 
         self._transform_predictor = MagicMock(spec=ImageTransformer)
+        self._transform_predictor.possible_category = MagicMock(return_value=PageType.angle)
         self._transform_predictor.name = "mock_transform"
         self.simple_transform = SimpleTransformService(self._transform_predictor)
 
     @mark.basic
     def test_pass_datapoint(self, dp_image: Image) -> None:
         """
         test pass_datapoint
```

### Comparing `deepdoctection-0.30/tests/test_utils.py` & `deepdoctection-0.31/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/train/__init__.py` & `deepdoctection-0.31/tests/train/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/train/conftest.py` & `deepdoctection-0.31/tests/train/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/train/test_d2_frcnn_train.py` & `deepdoctection-0.31/tests/train/test_d2_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests/train/test_tp_frcnn_train.py` & `deepdoctection-0.31/tests/train/test_tp_frcnn_train.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests_d2/__init__.py` & `deepdoctection-0.31/tests_d2/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests_d2/conftest.py` & `deepdoctection-0.31/tests_d2/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdoctection-0.30/tests_d2/test_d2detect.py` & `deepdoctection-0.31/tests_d2/test_d2detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         # Arrange, Act & Assert
         with raises(ImportError):
             D2FrcnnDetector(path_yaml=path_to_d2_frcnn_yaml,path_weights="",categories=categories)
 
     @staticmethod
     @mark.pt_deps
-    @patch("deepdoctection.extern.d2detect.D2FrcnnDetector.set_model", MagicMock(return_value=MagicMock))
+    @patch("deepdoctection.extern.d2detect.D2FrcnnDetector._set_model", MagicMock(return_value=MagicMock))
     @patch("deepdoctection.extern.d2detect.D2FrcnnDetector._instantiate_d2_predictor", MagicMock())
     def test_d2_frcnn_predicts_image(path_to_d2_frcnn_yaml: str, categories: Dict[str,ObjectTypes],
                                      np_image: ImageType)-> None:
         """
         D2 FRCNN calls predict_image and post processes DetectionResult correctly, e.g. adding class names
         """
```

