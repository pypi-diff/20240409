# Comparing `tmp/mlcvzoo_base-5.7.1.tar.gz` & `tmp/mlcvzoo_base-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_base-5.7.1.tar", max compression
+gzip compressed data, was "mlcvzoo_base-5.7.2.tar", max compression
```

## Comparing `mlcvzoo_base-5.7.1.tar` & `mlcvzoo_base-5.7.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    11412 2024-02-16 17:28:05.431315 mlcvzoo_base-5.7.1/LICENSE
--rw-r--r--   0        0        0      547 2024-02-16 17:28:05.431315 mlcvzoo_base-5.7.1/README.md
--rw-r--r--   0        0        0      244 2024-02-19 16:37:12.015977 mlcvzoo_base-5.7.1/mlcvzoo_base/__init__.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/__init__.py
--rw-r--r--   0        0        0     1021 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/configuration.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/__init__.py
--rw-r--r--   0        0        0    11270 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation.py
--rw-r--r--   0        0        0      998 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_attributes.py
--rw-r--r--   0        0        0     2429 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_builder.py
--rw-r--r--   0        0        0    26718 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_class_mapper.py
--rw-r--r--   0        0        0     1130 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_parser.py
--rw-r--r--   0        0        0      975 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_writer.py
--rw-r--r--   0        0        0     6502 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/bounding_box.py
--rw-r--r--   0        0        0    13370 2024-02-19 16:22:08.070513 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/box.py
--rw-r--r--   0        0        0     2734 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/class_identifier.py
--rw-r--r--   0        0        0     5253 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/classification.py
--rw-r--r--   0        0        0     3941 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/dataset_info.py
--rw-r--r--   0        0        0     3268 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/ocr_perception.py
--rw-r--r--   0        0        0    12051 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/segmentation.py
--rw-r--r--   0        0        0      457 2024-02-19 16:22:08.070513 mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/types.py
--rw-r--r--   0        0        0      906 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/exceptions.py
--rw-r--r--   0        0        0     5029 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/interfaces.py
--rw-r--r--   0        0        0    13224 2024-02-16 17:28:05.439315 mlcvzoo_base-5.7.1/mlcvzoo_base/api/model.py
--rw-r--r--   0        0        0     2656 2024-02-21 16:04:58.144943 mlcvzoo_base-5.7.1/mlcvzoo_base/api/registry.py
--rw-r--r--   0        0        0      482 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/api/structs.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/__init__.py
--rw-r--r--   0        0        0     8464 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/annotation_handler_config.py
--rw-r--r--   0        0        0     3942 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/class_mapping_config.py
--rw-r--r--   0        0        0      656 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/config_registry.py
--rw-r--r--   0        0        0      772 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/device_query.py
--rw-r--r--   0        0        0     1692 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/mlfow_config.py
--rw-r--r--   0        0        0     3093 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/model_config.py
--rw-r--r--   0        0        0     2589 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/reduction_mapping_config.py
--rw-r--r--   0        0        0     3889 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/replacement_config.py
--rw-r--r--   0        0        0     3939 2024-02-19 16:22:08.070513 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/structs.py
--rw-r--r--   0        0        0     7286 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/utils.py
--rw-r--r--   0        0        0      628 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/visualization_config.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/__init__.py
--rw-r--r--   0        0        0      256 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
--rw-r--r--   0        0        0     9091 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
--rw-r--r--   0        0        0     7137 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
--rw-r--r--   0        0        0     2458 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
--rw-r--r--   0        0        0     8862 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
--rw-r--r--   0        0        0     8308 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
--rw-r--r--   0        0        0    14648 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_handler.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
--rw-r--r--   0        0        0     3409 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
--rw-r--r--   0        0        0     8168 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
--rw-r--r--   0        0        0    13949 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
--rw-r--r--   0        0        0     7839 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
--rw-r--r--   0        0        0    10617 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
--rw-r--r--   0        0        0     9355 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
--rw-r--r--   0        0        0    14717 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
--rw-r--r--   0        0        0     9282 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
--rw-r--r--   0        0        0     4097 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
--rw-r--r--   0        0        0      501 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/structs.py
--rw-r--r--   0        0        0    11234 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/utils.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/__init__.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/__init__.py
--rw-r--r--   0        0        0     2227 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/configuration.py
--rw-r--r--   0        0        0     6836 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/data_classes.py
--rw-r--r--   0        0        0    54147 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
--rw-r--r--   0        0        0    15943 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
--rw-r--r--   0        0        0     4134 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
--rw-r--r--   0        0        0      633 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/structs.py
--rw-r--r--   0        0        0    15700 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/utils.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/__init__.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/mlflow/__init__.py
--rw-r--r--   0        0        0     7255 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
--rw-r--r--   0        0        0     1676 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/mlflow/utils.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/__init__.py
--rw-r--r--   0        0        0      257 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/constants.py
--rw-r--r--   0        0        0    10705 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/model_registry.py
--rw-r--r--   0        0        0      196 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/read_from_file/__init__.py
--rw-r--r--   0        0        0     1540 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/read_from_file/configuration.py
--rw-r--r--   0        0        0    10713 2024-02-16 17:28:05.443316 mlcvzoo_base-5.7.1/mlcvzoo_base/models/read_from_file/model.py
--rw-r--r--   0        0        0        0 2024-02-21 16:21:24.051852 mlcvzoo_base-5.7.1/mlcvzoo_base/py.typed
--rw-r--r--   0        0        0        0 2024-02-21 16:21:24.051852 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/__init__.py
--rw-r--r--   0        0        0     1078 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
--rw-r--r--   0        0        0      138 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
--rw-r--r--   0        0        0      249 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
--rw-r--r--   0        0        0     1774 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
--rw-r--r--   0        0        0     1117 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/LICENSE.txt
--rw-r--r--   0        0        0      108 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/README.md
--rw-r--r--   0        0        0      296 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/__init__.py
--rw-r--r--   0        0        0     2794 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/perspective.py
--rw-r--r--   0        0        0     3744 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
--rw-r--r--   0        0        0      127 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/README.md
--rw-r--r--   0        0        0      249 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
--rw-r--r--   0        0        0     1649 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
--rw-r--r--   0        0        0      488 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/__init__.py
--rw-r--r--   0        0        0     4751 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/annotation_utils.py
--rw-r--r--   0        0        0     2353 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/common_utils.py
--rw-r--r--   0        0        0    11836 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/draw_utils.py
--rw-r--r--   0        0        0     5992 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/file_utils.py
--rw-r--r--   0        0        0     5852 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/gpu_util.py
--rw-r--r--   0        0        0     3009 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/implicit_path_replacements.py
--rw-r--r--   0        0        0     2435 2024-02-16 17:28:05.447316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/versioning_utils.py
--rw-r--r--   0        0        0     3811 2024-02-16 17:28:05.451316 mlcvzoo_base-5.7.1/mlcvzoo_base/utils/xml_utils.py
--rw-r--r--   0        0        0     4025 2024-02-21 16:21:06.571233 mlcvzoo_base-5.7.1/pyproject.toml
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 mlcvzoo_base-5.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2024-03-04 08:38:20.164380 mlcvzoo_base-5.7.2/LICENSE
+-rw-r--r--   0        0        0      547 2024-03-25 17:33:12.630680 mlcvzoo_base-5.7.2/README.md
+-rw-r--r--   0        0        0      244 2024-04-05 08:00:50.573919 mlcvzoo_base-5.7.2/mlcvzoo_base/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/__init__.py
+-rw-r--r--   0        0        0     1021 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/configuration.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/__init__.py
+-rw-r--r--   0        0        0    11278 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation.py
+-rw-r--r--   0        0        0      998 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_attributes.py
+-rw-r--r--   0        0        0     2429 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_builder.py
+-rw-r--r--   0        0        0    26718 2024-04-05 08:00:50.573919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_class_mapper.py
+-rw-r--r--   0        0        0     1130 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_parser.py
+-rw-r--r--   0        0        0      975 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_writer.py
+-rw-r--r--   0        0        0     6558 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/bounding_box.py
+-rw-r--r--   0        0        0    13370 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/box.py
+-rw-r--r--   0        0        0     2734 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/class_identifier.py
+-rw-r--r--   0        0        0     5309 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/classification.py
+-rw-r--r--   0        0        0     3941 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/dataset_info.py
+-rw-r--r--   0        0        0     3268 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/ocr_perception.py
+-rw-r--r--   0        0        0    12107 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/segmentation.py
+-rw-r--r--   0        0        0      457 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/types.py
+-rw-r--r--   0        0        0      906 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/exceptions.py
+-rw-r--r--   0        0        0     5029 2024-03-28 09:50:55.622541 mlcvzoo_base-5.7.2/mlcvzoo_base/api/interfaces.py
+-rw-r--r--   0        0        0    13224 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/api/model.py
+-rw-r--r--   0        0        0     2656 2024-03-27 06:44:37.840931 mlcvzoo_base-5.7.2/mlcvzoo_base/api/registry.py
+-rw-r--r--   0        0        0      482 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/api/structs.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/__init__.py
+-rw-r--r--   0        0        0     8464 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/annotation_handler_config.py
+-rw-r--r--   0        0        0     3942 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/class_mapping_config.py
+-rw-r--r--   0        0        0      655 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/config_registry.py
+-rw-r--r--   0        0        0      772 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/device_query.py
+-rw-r--r--   0        0        0     1692 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/mlfow_config.py
+-rw-r--r--   0        0        0     3093 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/model_config.py
+-rw-r--r--   0        0        0     2589 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/reduction_mapping_config.py
+-rw-r--r--   0        0        0     3889 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/replacement_config.py
+-rw-r--r--   0        0        0     3939 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/structs.py
+-rw-r--r--   0        0        0     7286 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/utils.py
+-rw-r--r--   0        0        0      628 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/visualization_config.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
+-rw-r--r--   0        0        0     9091 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
+-rw-r--r--   0        0        0     7138 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
+-rw-r--r--   0        0        0     2458 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
+-rw-r--r--   0        0        0     9143 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
+-rw-r--r--   0        0        0     8308 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
+-rw-r--r--   0        0        0    14648 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_handler.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
+-rw-r--r--   0        0        0     3409 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
+-rw-r--r--   0        0        0     8168 2024-03-04 08:38:20.176380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
+-rw-r--r--   0        0        0    13949 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
+-rw-r--r--   0        0        0     7839 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
+-rw-r--r--   0        0        0    10838 2024-04-05 12:20:58.421516 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
+-rw-r--r--   0        0        0     9355 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
+-rw-r--r--   0        0        0    14717 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
+-rw-r--r--   0        0        0     9282 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
+-rw-r--r--   0        0        0     4097 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
+-rw-r--r--   0        0        0      501 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/structs.py
+-rw-r--r--   0        0        0    11234 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/utils.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/__init__.py
+-rw-r--r--   0        0        0     2227 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/configuration.py
+-rw-r--r--   0        0        0     6836 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/data_classes.py
+-rw-r--r--   0        0        0    54147 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
+-rw-r--r--   0        0        0    15943 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
+-rw-r--r--   0        0        0     4134 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
+-rw-r--r--   0        0        0      633 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/structs.py
+-rw-r--r--   0        0        0    15700 2024-04-05 08:00:50.577919 mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/utils.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/__init__.py
+-rw-r--r--   0        0        0     7255 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
+-rw-r--r--   0        0        0     1676 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/utils.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/__init__.py
+-rw-r--r--   0        0        0      257 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/constants.py
+-rw-r--r--   0        0        0    10705 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/models/model_registry.py
+-rw-r--r--   0        0        0      196 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/__init__.py
+-rw-r--r--   0        0        0     1540 2024-03-04 08:38:20.180380 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/configuration.py
+-rw-r--r--   0        0        0    10713 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/model.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:55:53.034324 mlcvzoo_base-5.7.2/mlcvzoo_base/py.typed
+-rw-r--r--   0        0        0        0 2024-04-09 09:55:53.034324 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/__init__.py
+-rw-r--r--   0        0        0     1078 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
+-rw-r--r--   0        0        0      138 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
+-rw-r--r--   0        0        0      249 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
+-rw-r--r--   0        0        0     1774 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
+-rw-r--r--   0        0        0     1117 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/LICENSE.txt
+-rw-r--r--   0        0        0      108 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/README.md
+-rw-r--r--   0        0        0      296 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/__init__.py
+-rw-r--r--   0        0        0     2794 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/perspective.py
+-rw-r--r--   0        0        0     3744 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
+-rw-r--r--   0        0        0      127 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/README.md
+-rw-r--r--   0        0        0      249 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
+-rw-r--r--   0        0        0     1649 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
+-rw-r--r--   0        0        0      488 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/__init__.py
+-rw-r--r--   0        0        0     4751 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/annotation_utils.py
+-rw-r--r--   0        0        0     2353 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/common_utils.py
+-rw-r--r--   0        0        0    11836 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/draw_utils.py
+-rw-r--r--   0        0        0     5992 2024-04-05 08:00:50.581919 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/file_utils.py
+-rw-r--r--   0        0        0     5852 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/gpu_util.py
+-rw-r--r--   0        0        0     3009 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/implicit_path_replacements.py
+-rw-r--r--   0        0        0     2435 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/versioning_utils.py
+-rw-r--r--   0        0        0     3811 2024-03-04 08:38:20.184381 mlcvzoo_base-5.7.2/mlcvzoo_base/utils/xml_utils.py
+-rw-r--r--   0        0        0     4025 2024-04-09 09:55:34.725685 mlcvzoo_base-5.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 mlcvzoo_base-5.7.2/PKG-INFO
```

### Comparing `mlcvzoo_base-5.7.1/LICENSE` & `mlcvzoo_base-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/README.md` & `mlcvzoo_base-5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/configuration.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,16 +297,16 @@
         bounding_boxes: Optional[List[BoundingBox]] = None,
         segmentations: Optional[List[Segmentation]] = None,
     ) -> BaseAnnotation:
         return BaseAnnotation(
             image_path=self.image_path,
             annotation_path=self.image_path,
             image_shape=self.image_shape,
-            classifications=classifications
-            if classifications is not None
-            else self.classifications,
+            classifications=(
+                classifications if classifications is not None else self.classifications
+            ),
             bounding_boxes=bounding_boxes if bounding_boxes is not None else self.bounding_boxes,
             segmentations=segmentations if segmentations is not None else self.segmentations,
             image_dir=self.image_dir,
             annotation_dir=self.annotation_dir,
             replacement_string=self.replacement_string,
         )
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_attributes.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_attributes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_class_mapper.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_class_mapper.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/annotation_writer.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/bounding_box.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,22 @@
                 "model_class_id": self.model_class_identifier.class_id,
                 "model_class_name": self.model_class_identifier.class_name,
                 "score": self.score,
             }
         else:
             return {
                 "box": self.box if raw_type else self.box.to_dict(),
-                "class_identifier": self.class_identifier
-                if raw_type
-                else self.class_identifier.to_dict(),
-                "model_class_identifier": self.model_class_identifier
-                if raw_type
-                else self.model_class_identifier.to_dict(),
+                "class_identifier": (
+                    self.class_identifier if raw_type else self.class_identifier.to_dict()
+                ),
+                "model_class_identifier": (
+                    self.model_class_identifier
+                    if raw_type
+                    else self.model_class_identifier.to_dict()
+                ),
                 "score": self.score,
                 "difficult": self.difficult,
                 "occluded": self.occluded,
                 "background": self.background,
                 "content": self.content,
             }
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/box.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/box.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/class_identifier.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/class_identifier.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/classification.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,22 @@
                 "class_name": self.class_name,
                 "model_class_id": self.model_class_identifier.class_id,
                 "model_class_name": self.model_class_identifier.class_name,
                 "score": self.score,
             }
         else:
             return {
-                "class_identifier": self.class_identifier
-                if raw_type
-                else self.class_identifier.to_dict(),
-                "model_class_identifier": self.model_class_identifier
-                if raw_type
-                else self.model_class_identifier.to_dict(),
+                "class_identifier": (
+                    self.class_identifier if raw_type else self.class_identifier.to_dict()
+                ),
+                "model_class_identifier": (
+                    self.model_class_identifier
+                    if raw_type
+                    else self.model_class_identifier.to_dict()
+                ),
                 "score": self.score,
             }
 
     @staticmethod
     def from_dict(input_dict: Dict[str, Any], reduced: bool = False) -> Classification:
         # fmt: off
         if reduced:
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/dataset_info.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/ocr_perception.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/ocr_perception.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/data/segmentation.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/data/segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,20 +135,22 @@
                 "model_class_name": self.model_class_identifier.class_name,
                 "score": self.score,
             }
         else:
             return {
                 "box": _box,
                 "polygon": self.polygon,
-                "class_identifier": self.class_identifier
-                if raw_type
-                else self.class_identifier.to_dict(),
-                "model_class_identifier": self.model_class_identifier
-                if raw_type
-                else self.model_class_identifier.to_dict(),
+                "class_identifier": (
+                    self.class_identifier if raw_type else self.class_identifier.to_dict()
+                ),
+                "model_class_identifier": (
+                    self.model_class_identifier
+                    if raw_type
+                    else self.model_class_identifier.to_dict()
+                ),
                 "score": self.score,
                 "difficult": self.difficult,
                 "occluded": self.occluded,
                 "background": self.background,
                 "content": self.content,
             }
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/exceptions.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/interfaces.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/model.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/api/registry.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/api/registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/annotation_handler_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/annotation_handler_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/class_mapping_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/class_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/config_registry.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/config_registry.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,13 @@
 
 from mlcvzoo_base.api.registry import MLCVZooRegistry
 
 logger = logging.getLogger(__name__)
 
 
 class ConfigRegistry(MLCVZooRegistry[Type[BaseConfigClass]]):
-
     """
     Class to provide a registry for configuration constructors
     """
 
     def __init__(self) -> None:
         MLCVZooRegistry.__init__(self)
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/device_query.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/device_query.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/mlfow_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/mlfow_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/model_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/model_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/reduction_mapping_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/reduction_mapping_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/replacement_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/replacement_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/structs.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/configuration/visualization_config.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/configuration/visualization_config.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             replacement_string=replacement_string,
         )
 
         try:
             AnnotationBuilder._check_annotation(annotation=annotation)
         except ValueError as value_error:
             logger.exception(
-                f"{value_error}, in a future version, the whole annotation will be skipped!"
+                "%s, in a future version, the whole annotation will be skipped!", value_error
             )
 
         annotation = replace_index_by_dir(
             annotation=annotation,
         )
 
         annotation = ensure_abspath(annotation=annotation)
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
 from mlcvzoo_base.api.data.annotation_builder import AnnotationBuilder
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
 from mlcvzoo_base.api.data.bounding_box import BoundingBox
 from mlcvzoo_base.api.data.box import Box
 from mlcvzoo_base.api.data.class_identifier import ClassIdentifier
-from mlcvzoo_base.api.exceptions import ForbiddenClassError
+from mlcvzoo_base.api.exceptions import ClassMappingNotFoundError
 from mlcvzoo_base.configuration.structs import ObjectDetectionBBoxFormats
 from mlcvzoo_base.data_preparation.structs import MOTChallengeFormats
 from mlcvzoo_base.data_preparation.utils import ensure_abspath
 
 logger = logging.getLogger(__name__)
 
 
@@ -88,15 +88,15 @@
 
         annotation = ensure_abspath(annotation=annotation)
 
         try:
             AnnotationBuilder._check_annotation(annotation=annotation)
         except ValueError as value_error:
             logger.exception(
-                f"{value_error}, in a future version, the whole annotation will be skipped!"
+                "%s, in a future version, the whole annotation will be skipped!", value_error
             )
 
         return annotation
 
     def __parse_bounding_boxes(
         self,
     ) -> List[BoundingBox]:
@@ -171,15 +171,21 @@
             try:
                 class_id = self.mapper.map_annotation_class_name_to_model_class_id(
                     class_name=mot_class_name
                 )
                 class_name = self.mapper.map_annotation_class_name_to_model_class_name(
                     class_name=mot_class_name
                 )
-            except ForbiddenClassError:
+            except ClassMappingNotFoundError:
+                logger.debug(
+                    "Could not find a valid class-mapping for class-name '%s'. "
+                    "BndBox will be skipped, mot-line= '%s'",
+                    mot_class_name,
+                    mot_annotation_line,
+                )
                 continue
 
             # Note:
             #  - in GT data "confidence score" indicates whether an entry is considered for
             #    training
             #  - Whereas in pre-annotated data it indicates how confident the detector was
             #    that this instance is of the specified class [1,100]
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_handler.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Dict, List
 
 import cv2
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
 from mlcvzoo_base.api.data.annotation_parser import AnnotationParser
+from mlcvzoo_base.api.exceptions import ForbiddenClassError
 from mlcvzoo_base.configuration.annotation_handler_config import (
     AnnotationHandlerMOTInputDataConfig,
 )
 from mlcvzoo_base.configuration.class_mapping_config import (
     ClassMappingConfig,
     ClassMappingModelClassesConfig,
 )
@@ -142,14 +143,20 @@
             for image_id, image_path in enumerate(image_paths):
                 # MOT image IDs start with 1
                 mot_image_id = image_id + 1
                 if mot_image_id not in annotation_line_dict:
                     continue
 
                 image = cv2.imread(image_path)
+                if image is None:
+                    logger.warning(
+                        "Could not read image from path='%s', annotation will be skipped",
+                        image_path,
+                    )
+                    continue
                 image_shape = image.shape
 
                 replacement_string = AnnotationParser.csv_directory_replacement_string.format(
                     dataset_count
                 )
 
                 mot_builder = MOTAnnotationBuilder(
@@ -166,28 +173,23 @@
                     annotation = mot_builder.build(
                         image_path=image_path,
                         annotation_path=input_data.annotation_path,
                         image_dir=input_data.image_dir,
                         annotation_dir=os.path.dirname(input_data.annotation_path),
                         replacement_string=replacement_string,
                     )
-
                     _input_data_annotations.append(annotation)
-
-                except ValueError as error:
-                    logger.warning(
-                        "%s, annotation from path %s will be skipped",
-                        str(error),
-                        input_data.annotation_path,
-                    )
+                except (ValueError, ForbiddenClassError) as error:
+                    logger.warning("%s, annotation will be skipped", str(error))
                     continue
 
             logger.info(
-                f"Parsed {len(_input_data_annotations)} "
-                f"from mot file '{input_data.annotation_path}'"
+                "Parsed %i annotations from mot file '%s'",
+                len(_input_data_annotations),
+                input_data.annotation_path,
             )
             annotations.extend(_input_data_annotations)
 
         return annotations
 
     @staticmethod
     def create_mot__2015_class_mapping() -> ClassMappingConfig:
```

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/data_preparation/utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/data_preparation/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/configuration.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/data_classes.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/metrics_computation.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/metrics_logging.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/model_evaluation.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/structs.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/evaluation/object_detection/utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/evaluation/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/mlflow/mlflow_runner.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/metrics/mlflow/utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/metrics/mlflow/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/models/model_registry.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/models/model_registry.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/models/read_from_file/configuration.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/models/read_from_file/model.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/models/read_from_file/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/LICENSE.txt` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/imutils/perspective.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/imutils/perspective.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/annotation_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/common_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/draw_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/file_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/gpu_util.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/gpu_util.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/implicit_path_replacements.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/implicit_path_replacements.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/versioning_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/versioning_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/mlcvzoo_base/utils/xml_utils.py` & `mlcvzoo_base-5.7.2/mlcvzoo_base/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.7.1/pyproject.toml` & `mlcvzoo_base-5.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlcvzoo_base"
 description = "MLCVZoo Base Package"
-version = "5.7.1"
+version = "5.7.2"
 license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mlcvzoo_base-5.7.1/PKG-INFO` & `mlcvzoo_base-5.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-base
-Version: 5.7.1
+Version: 5.7.2
 Summary: MLCVZoo Base Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base
 License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

