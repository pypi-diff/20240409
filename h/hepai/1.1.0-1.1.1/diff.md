# Comparing `tmp/hepai-1.1.0.tar.gz` & `tmp/hepai-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepai-1.1.0.tar", last modified: Wed Mar 27 06:52:39 2024, max compression
+gzip compressed data, was "hepai-1.1.1.tar", last modified: Tue Apr  9 07:28:31 2024, max compression
```

## Comparing `hepai-1.1.0.tar` & `hepai-1.1.1.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.524726 hepai-1.1.0/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.1.0/MANIFEST.in
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5402 2024-03-27 06:52:39.524726 hepai-1.1.0/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4619 2024-03-26 09:59:20.000000 hepai-1.1.0/README.md
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1468 2024-03-26 10:12:46.000000 hepai-1.1.0/hai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2201 2024-03-25 11:14:31.000000 hepai-1.1.0/hai/apis/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/basic/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       83 2023-10-24 09:29:42.000000 hepai-1.1.0/hai/apis/basic/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/basic/argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/basic/base.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/basic/grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/basic/registry.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/basic/utils.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/hub/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.1.0/hai/apis/hub/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.1.0/hai/apis/hub/hubs.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/modules/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/modules/ResNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/modules/ResNet/ResNet.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/modules/ResNet/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/modules/UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/modules/UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.1.0/hai/apis/modules/UNet/argparse_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.1.0/hai/apis/modules/UNet/evaluate_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.1.0/hai/apis/modules/UNet/predict_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.1.0/hai/apis/modules/UNet/train_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/modules/UNet/unet_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/modules/YOLOv5/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/apis/modules/YOLOv5/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.1.0/hai/apis/modules/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      103 2024-03-25 11:33:22.000000 hepai-1.1.0/hai/apis/openai_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/workers_api/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.1.0/hai/apis/workers_api/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.516726 hepai-1.1.0/hai/apis/workers_api/llm/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.1.0/hai/apis/workers_api/llm/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2953 2023-11-09 05:34:58.000000 hepai-1.1.0/hai/apis/workers_api/llm/llm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.1.0/hai/apis/workers_api/llm/tokenizer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8453 2024-03-08 06:44:02.000000 hepai-1.1.0/hai/apis/workers_api/model.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/apis/workers_api/nougat/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2024-03-08 06:44:02.000000 hepai-1.1.0/hai/apis/workers_api/nougat/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      470 2024-03-08 06:44:02.000000 hepai-1.1.0/hai/apis/workers_api/nougat/pdf_process.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/apis/workers_api/sam/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-08-07 05:23:27.000000 hepai-1.1.0/hai/apis/workers_api/sam/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2164 2023-10-12 04:36:05.000000 hepai-1.1.0/hai/apis/workers_api/sam/pre_process.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5139 2023-08-04 16:18:52.000000 hepai-1.1.0/hai/apis/workers_api/sam/seg_via_sam.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/configs/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/configs/Base/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.1.0/hai/configs/Base/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/configs/Base/hai_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/configs/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/configs/uaii_deepsort_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/configs/uaii_seyolov5_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/configs/uaii_stream_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/configs/urls/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.1.0/hai/configs/urls/datasets.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.1.0/hai/configs/urls/hub_models.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/configs/visible_loader_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.1.0/hai/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/detection/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.1.0/hai/modules/detection/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.1.0/hai/modules/exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/exporter/images_exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/modules/exporter/images_exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.1.0/hai/modules/loader/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/loader/images_loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/modules/loader/images_loader/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.1.0/hai/modules/loader/images_loader/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.1.0/hai/modules/loader/images_loader/dataset_torch.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.1.0/hai/modules/loader/images_loader/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.1.0/hai/modules/model_hub.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/segmentation/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/evaluate.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/hubconf.py
--rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/predict.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/train.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.1.0/hai/modules/segmentation/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/testor/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.1.0/hai/testor/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/testor/test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      495 2023-10-23 01:04:23.000000 hepai-1.1.0/hai/testor/test_ip_connectable.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/testor/test_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      965 2023-10-23 01:10:57.000000 hepai-1.1.0/hai/testor/test_request_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.1.0/hai/testor/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/actuator/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.1.0/hai/uaii/actuator/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.1.0/hai/uaii/actuator/trainer.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/cli/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.1.0/hai/uaii/cli/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4118 2023-05-11 12:36:29.000000 hepai-1.1.0/hai/uaii/cli/cli_functions.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/uaii/cli/cli_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/datasets/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/datasets/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.1.0/hai/uaii/datasets/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8478 2024-03-08 06:41:21.000000 hepai-1.1.0/hai/uaii/datasets/dataset_utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/datasets/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.1.0/hai/uaii/datasets/datasets_hub.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.1.0/hai/uaii/datasets/uaii_loaders.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     7616 2024-03-27 06:48:57.000000 hepai-1.1.0/hai/uaii/hepai_object.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/registry/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.1.0/hai/uaii/registry/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.1.0/hai/uaii/registry/init_register.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.1.0/hai/uaii/registry/registy.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/registry/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/registry/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/registry/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/registry/utils/general.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.1.0/hai/uaii/server/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/grpc/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/grpc/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/example/grpc-client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/example/grpc-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/example/hello_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/example/hello_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_secure_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_secure_server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_xai_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/grpc/grpc_xai_server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/nacos/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/commons.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/exception.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/files.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/listener.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/params.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos/timer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/nacos-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/nacos/request_test.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/server/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.1.0/hai/uaii/server/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/stream/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/base_input.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.1.0/hai/uaii/stream/base_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/base_output.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/base_queue.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/rabbit_qm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.1.0/hai/uaii/stream/stream.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/stream/streams.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.1.0/hai/uaii/uaii_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.0/hai/uaii/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.1.0/hai/uaii/utils/arbitrary_import.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.1.0/hai/uaii/utils/base_uaii.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15290 2023-05-10 16:19:50.000000 hepai-1.1.0/hai/uaii/utils/config_loader.py
--rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.1.0/hai/uaii/utils/fake_argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.1.0/hai/uaii/utils/general.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5268 2023-10-24 09:29:02.000000 hepai-1.1.0/hai/uaii/utils/hai_hf_parser.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    18952 2023-06-29 12:25:38.000000 hepai-1.1.0/hai/uaii/utils/hf_argparser.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hai/uaii/worker/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-05-18 13:37:30.000000 hepai-1.1.0/hai/uaii/worker/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2186 2023-06-02 07:05:51.000000 hepai-1.1.0/hai/uaii/worker/base_worker_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2665 2023-10-12 05:00:04.000000 hepai-1.1.0/hai/uaii/worker/run_worker.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       65 2023-05-18 13:37:30.000000 hepai-1.1.0/hai/uaii/worker/usage.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1561 2023-07-03 15:23:11.000000 hepai-1.1.0/hai/uaii/worker/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    16594 2023-10-19 08:28:21.000000 hepai-1.1.0/hai/uaii/worker/worker.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2024-03-27 06:52:11.000000 hepai-1.1.0/hai/version.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.520726 hepai-1.1.0/hepai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2024-03-25 11:12:53.000000 hepai-1.1.0/hepai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-03-27 06:52:39.524726 hepai-1.1.0/hepai.egg-info/
--rw-r--r--   0 zzd       (1000) zzd       (1000)     5402 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5252 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/SOURCES.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/dependency_links.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/entry_points.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       89 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/requires.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       10 2024-03-27 06:52:39.000000 hepai-1.1.0/hepai.egg-info/top_level.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2024-03-27 06:52:39.524726 hepai-1.1.0/setup.cfg
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4828 2024-03-08 07:06:54.000000 hepai-1.1.0/setup.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.967648 hepai-1.1.1/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.1.1/MANIFEST.in
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5402 2024-04-09 07:28:31.967648 hepai-1.1.1/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4619 2024-03-26 09:59:20.000000 hepai-1.1.1/README.md
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1468 2024-03-27 11:58:18.000000 hepai-1.1.1/hai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2201 2024-03-25 11:14:31.000000 hepai-1.1.1/hai/apis/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/basic/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       83 2023-10-24 09:29:42.000000 hepai-1.1.1/hai/apis/basic/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/basic/argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/basic/base.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/basic/grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/basic/registry.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/basic/utils.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/hub/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.1.1/hai/apis/hub/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.1.1/hai/apis/hub/hubs.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/modules/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/modules/ResNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/modules/ResNet/ResNet.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/modules/ResNet/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/modules/UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/modules/UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.1.1/hai/apis/modules/UNet/argparse_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.1.1/hai/apis/modules/UNet/evaluate_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.1.1/hai/apis/modules/UNet/predict_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.1.1/hai/apis/modules/UNet/train_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/modules/UNet/unet_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/modules/YOLOv5/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/apis/modules/YOLOv5/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.1.1/hai/apis/modules/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      103 2024-03-25 11:33:22.000000 hepai-1.1.1/hai/apis/openai_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/workers_api/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.1.1/hai/apis/workers_api/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/workers_api/llm/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.1.1/hai/apis/workers_api/llm/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2953 2023-11-09 05:34:58.000000 hepai-1.1.1/hai/apis/workers_api/llm/llm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.1.1/hai/apis/workers_api/llm/tokenizer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8547 2024-03-27 12:29:22.000000 hepai-1.1.1/hai/apis/workers_api/model.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/workers_api/nougat/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2024-03-08 06:44:02.000000 hepai-1.1.1/hai/apis/workers_api/nougat/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      470 2024-03-08 06:44:02.000000 hepai-1.1.1/hai/apis/workers_api/nougat/pdf_process.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/apis/workers_api/sam/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-08-07 05:23:27.000000 hepai-1.1.1/hai/apis/workers_api/sam/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2164 2023-10-12 04:36:05.000000 hepai-1.1.1/hai/apis/workers_api/sam/pre_process.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5139 2023-08-04 16:18:52.000000 hepai-1.1.1/hai/apis/workers_api/sam/seg_via_sam.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/configs/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/configs/Base/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.1.1/hai/configs/Base/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/configs/Base/hai_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/configs/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/configs/uaii_deepsort_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/configs/uaii_seyolov5_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/configs/uaii_stream_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.959648 hepai-1.1.1/hai/configs/urls/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.1.1/hai/configs/urls/datasets.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.1.1/hai/configs/urls/hub_models.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/configs/visible_loader_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.1.1/hai/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/detection/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.1.1/hai/modules/detection/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.1.1/hai/modules/exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/exporter/images_exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/modules/exporter/images_exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.1.1/hai/modules/loader/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/loader/images_loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/modules/loader/images_loader/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.1.1/hai/modules/loader/images_loader/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.1.1/hai/modules/loader/images_loader/dataset_torch.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.1.1/hai/modules/loader/images_loader/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.1.1/hai/modules/model_hub.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/segmentation/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/evaluate.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/hubconf.py
+-rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/predict.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/train.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.1.1/hai/modules/segmentation/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/testor/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.1.1/hai/testor/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/testor/test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      495 2023-10-23 01:04:23.000000 hepai-1.1.1/hai/testor/test_ip_connectable.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/testor/test_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      965 2023-10-23 01:10:57.000000 hepai-1.1.1/hai/testor/test_request_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.1.1/hai/testor/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/actuator/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.1.1/hai/uaii/actuator/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.1.1/hai/uaii/actuator/trainer.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/cli/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.1.1/hai/uaii/cli/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4118 2023-05-11 12:36:29.000000 hepai-1.1.1/hai/uaii/cli/cli_functions.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/uaii/cli/cli_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/datasets/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/datasets/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.1.1/hai/uaii/datasets/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8478 2024-03-08 06:41:21.000000 hepai-1.1.1/hai/uaii/datasets/dataset_utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/datasets/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.1.1/hai/uaii/datasets/datasets_hub.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.1.1/hai/uaii/datasets/uaii_loaders.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8211 2024-04-09 07:27:37.000000 hepai-1.1.1/hai/uaii/hepai_object.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/registry/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.1.1/hai/uaii/registry/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.1.1/hai/uaii/registry/init_register.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.1.1/hai/uaii/registry/registy.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/registry/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/registry/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/registry/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/registry/utils/general.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.1.1/hai/uaii/server/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/grpc/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/grpc/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/example/grpc-client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/example/grpc-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/example/hello_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/example/hello_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_secure_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_secure_server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_xai_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/grpc/grpc_xai_server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/nacos/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/commons.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/exception.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/files.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/listener.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/params.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos/timer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/nacos-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/nacos/request_test.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/server/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.1.1/hai/uaii/server/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/stream/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/base_input.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.1.1/hai/uaii/stream/base_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/base_output.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/base_queue.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/rabbit_qm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.1.1/hai/uaii/stream/stream.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/stream/streams.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.1.1/hai/uaii/uaii_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.1.1/hai/uaii/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.1.1/hai/uaii/utils/arbitrary_import.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.1.1/hai/uaii/utils/base_uaii.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15290 2023-05-10 16:19:50.000000 hepai-1.1.1/hai/uaii/utils/config_loader.py
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.1.1/hai/uaii/utils/fake_argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.1.1/hai/uaii/utils/general.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5268 2023-10-24 09:29:02.000000 hepai-1.1.1/hai/uaii/utils/hai_hf_parser.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    18952 2023-06-29 12:25:38.000000 hepai-1.1.1/hai/uaii/utils/hf_argparser.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hai/uaii/worker/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-05-18 13:37:30.000000 hepai-1.1.1/hai/uaii/worker/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2273 2024-03-27 11:21:40.000000 hepai-1.1.1/hai/uaii/worker/base_worker_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3070 2024-03-27 12:20:34.000000 hepai-1.1.1/hai/uaii/worker/run_worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       65 2023-05-18 13:37:30.000000 hepai-1.1.1/hai/uaii/worker/usage.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1561 2023-07-03 15:23:11.000000 hepai-1.1.1/hai/uaii/worker/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17031 2024-03-27 12:23:25.000000 hepai-1.1.1/hai/uaii/worker/worker.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2024-04-09 07:27:54.000000 hepai-1.1.1/hai/version.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hepai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2024-03-25 11:12:53.000000 hepai-1.1.1/hepai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2024-04-09 07:28:31.963648 hepai-1.1.1/hepai.egg-info/
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     5402 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5252 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/entry_points.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       89 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/requires.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       10 2024-04-09 07:28:31.000000 hepai-1.1.1/hepai.egg-info/top_level.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2024-04-09 07:28:31.967648 hepai-1.1.1/setup.cfg
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4828 2024-03-08 07:06:54.000000 hepai-1.1.1/setup.py
```

### Comparing `hepai-1.1.0/PKG-INFO` & `hepai-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.0
+Version: 1.1.1
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.0 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.1 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `hepai-1.1.0/README.md` & `hepai-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/__init__.py` & `hepai-1.1.1/hai/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/__init__.py` & `hepai-1.1.1/hai/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/hub/hubs.py` & `hepai-1.1.1/hai/apis/hub/hubs.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/ResNet/ResNet.py` & `hepai-1.1.1/hai/apis/modules/ResNet/ResNet.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/__init__.py` & `hepai-1.1.1/hai/apis/modules/UNet/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/argparse_config.py` & `hepai-1.1.1/hai/apis/modules/UNet/argparse_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/evaluate_api.py` & `hepai-1.1.1/hai/apis/modules/UNet/evaluate_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/predict_api.py` & `hepai-1.1.1/hai/apis/modules/UNet/predict_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/train_api.py` & `hepai-1.1.1/hai/apis/modules/UNet/train_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/modules/UNet/unet_api.py` & `hepai-1.1.1/hai/apis/modules/UNet/unet_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/workers_api/llm/llm.py` & `hepai-1.1.1/hai/apis/workers_api/llm/llm.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/workers_api/model.py` & `hepai-1.1.1/hai/apis/workers_api/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
             api_key = os.environ.get("HEPAI_API_KEY", None)
         if api_key is None:
             raise ValueError(f"""            
 The HepAI API-KEY is required. You can set it via `hai.api_key=xxx` in your code, or set the environment variable `HEPAI_API_KEY` via `export HEPAI_API_KEY=xxx`.
 Alternatively, it can be provided by passing in the `api_key` parameter when calling the method.
 """)
         return api_key
+    
+
+    @staticmethod
+    def list_models(**kwargs):
+        return HaiModel.list(**kwargs)
 
     @staticmethod
     def list(**kwargs):
         """
         List all models on HepAI Platform.
         :param refresh: Whether to refresh the model list, default is False.
         :param return_all_info: Whether to return all information of the models, default is False.
```

### Comparing `hepai-1.1.0/hai/apis/workers_api/sam/pre_process.py` & `hepai-1.1.1/hai/apis/workers_api/sam/pre_process.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/apis/workers_api/sam/seg_via_sam.py` & `hepai-1.1.1/hai/apis/workers_api/sam/seg_via_sam.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/configs/uaii_seyolov5_config.py` & `hepai-1.1.1/hai/configs/uaii_seyolov5_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/configs/uaii_stream_config.py` & `hepai-1.1.1/hai/configs/uaii_stream_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/configs/urls/datasets.json` & `hepai-1.1.1/hai/configs/urls/datasets.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/configs/urls/hub_models.json` & `hepai-1.1.1/hai/configs/urls/hub_models.json`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/configs/visible_loader_config.py` & `hepai-1.1.1/hai/configs/visible_loader_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/exporter/images_exporter/__init__.py` & `hepai-1.1.1/hai/modules/exporter/images_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/loader/images_loader/__init__.py` & `hepai-1.1.1/hai/modules/loader/images_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/loader/images_loader/dataloader.py` & `hepai-1.1.1/hai/modules/loader/images_loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/loader/images_loader/dataset_torch.py` & `hepai-1.1.1/hai/modules/loader/images_loader/dataset_torch.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/loader/images_loader/datasets.py` & `hepai-1.1.1/hai/modules/loader/images_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/model_hub.py` & `hepai-1.1.1/hai/modules/model_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/evaluate.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/hubconf.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/hubconf.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/predict.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/predict.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/train.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/train.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/modules/segmentation/Pytorch_UNet/utils/utils.py` & `hepai-1.1.1/hai/modules/segmentation/Pytorch_UNet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/testor/test_request_model.py` & `hepai-1.1.1/hai/testor/test_request_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/cli/cli_functions.py` & `hepai-1.1.1/hai/uaii/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/cli/cli_main.py` & `hepai-1.1.1/hai/uaii/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/datasets/dataloader.py` & `hepai-1.1.1/hai/uaii/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/datasets/dataset_utils.py` & `hepai-1.1.1/hai/uaii/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/datasets/datasets.py` & `hepai-1.1.1/hai/uaii/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/datasets/datasets_hub.py` & `hepai-1.1.1/hai/uaii/datasets/datasets_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/datasets/uaii_loaders.py` & `hepai-1.1.1/hai/uaii/datasets/uaii_loaders.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/hepai_object.py` & `hepai-1.1.1/hai/uaii/hepai_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,37 +21,40 @@
         ChatCompletionChunk,
         Stream,
     )
     from openai._utils import (
         required_args, maybe_transform
     )
     from openai._base_client import make_request_options
-    
 except:
-    sys.path.append(str(here.parent.parent))
-    from repos.openai_python.src.openai import OpenAI
-    from repos.openai_python.src.openai import ( NOT_GIVEN, Timeout, NotGiven)
-    from repos.openai_python.src.openai._types import Headers, Query, Body
-    from repos.openai_python.src.openai.types import Completion
-    from repos.openai_python.src.openai import resources
-    from repos.openai_python.src.openai.resources import Completions, Chat
-    from repos.openai_python.src.openai.resources.chat.completions import (
-        ChatCompletionMessageParam,
-        completion_create_params,
-        ChatCompletionToolChoiceOptionParam,
-        ChatCompletionToolParam,
-        ChatCompletion,
-        ChatCompletionChunk,
-        Stream,
-    )
-    from repos.openai_python.src.openai._utils import (
-        required_args, maybe_transform
-    )
-    from repos.openai_python.src.openai._base_client import make_request_options
+    try:
+        sys.path.append(str(here.parent.parent))
+        from repos.openai_python.src.openai import OpenAI
+        from repos.openai_python.src.openai import ( NOT_GIVEN, Timeout, NotGiven)
+        from repos.openai_python.src.openai._types import Headers, Query, Body
+        from repos.openai_python.src.openai.types import Completion
+        from repos.openai_python.src.openai import resources
+        from repos.openai_python.src.openai.resources import Completions, Chat
+        from repos.openai_python.src.openai.resources.chat.completions import (
+            ChatCompletionMessageParam,
+            completion_create_params,
+            ChatCompletionToolChoiceOptionParam,
+            ChatCompletionToolParam,
+            ChatCompletion,
+            ChatCompletionChunk,
+            Stream,
+        )
+        from repos.openai_python.src.openai._utils import (
+            required_args, maybe_transform
+        )
+        from repos.openai_python.src.openai._base_client import make_request_options
+    except:
+        raise ImportError("Can't find openai module, please install it first by `pip install openai --upgrade`.")
 
+from hai.apis.workers_api.model import HaiModel
 
 DEFAULT_MAX_RETRIES = 2
 
 class HaiCompletions(Completions):
 
     @required_args(["messages", "model"], ["messages", "model", "stream"])
     def create(
@@ -184,8 +187,19 @@
             _strict_response_validation=_strict_response_validation,
         )
 
         self.completions = HaiCompletions(client=self)
         self.chat = HaiChat(client=self)
         pass
 
+    def list_models(self, **kwargs):
+        api_key = kwargs.pop("api_key", self.api_key)
+        host = kwargs.pop("host", self.base_url.host)
+        port = kwargs.pop("port", self.base_url.port)
+        return HaiModel.list(
+            api_key=api_key,
+            host=host,
+            port=port,
+            **kwargs,
+        )
+
```

### Comparing `hepai-1.1.0/hai/uaii/registry/init_register.py` & `hepai-1.1.1/hai/uaii/registry/init_register.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/registry/registy.py` & `hepai-1.1.1/hai/uaii/registry/registy.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/registry/utils/general.py` & `hepai-1.1.1/hai/uaii/registry/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/__init__.py` & `hepai-1.1.1/hai/uaii/server/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/example/grpc-client.py` & `hepai-1.1.1/hai/uaii/server/grpc/example/grpc-client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/example/grpc-test.py` & `hepai-1.1.1/hai/uaii/server/grpc/example/grpc-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/example/hello_pb2.py` & `hepai-1.1.1/hai/uaii/server/grpc/example/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/example/hello_pb2_grpc.py` & `hepai-1.1.1/hai/uaii/server/grpc/example/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_pb2.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_pb2_grpc.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_secure_client.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_secure_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_secure_server.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_secure_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_xai_client.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_xai_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/grpc/grpc_xai_server.py` & `hepai-1.1.1/hai/uaii/server/grpc/grpc_xai_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/client.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/commons.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/commons.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/files.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/files.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/listener.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/listener.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/params.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/params.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos/timer.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos/timer.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/nacos-test.py` & `hepai-1.1.1/hai/uaii/server/nacos/nacos-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/nacos/request_test.py` & `hepai-1.1.1/hai/uaii/server/nacos/request_test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/socket/example/client.py` & `hepai-1.1.1/hai/uaii/server/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/socket/example/server.py` & `hepai-1.1.1/hai/uaii/server/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/server/socket/server.py` & `hepai-1.1.1/hai/uaii/server/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/socket/example/client.py` & `hepai-1.1.1/hai/uaii/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/socket/example/server.py` & `hepai-1.1.1/hai/uaii/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/socket/server.py` & `hepai-1.1.1/hai/uaii/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/stream/base_input.py` & `hepai-1.1.1/hai/uaii/stream/base_input.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/stream/base_module.py` & `hepai-1.1.1/hai/uaii/stream/base_module.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/stream/base_output.py` & `hepai-1.1.1/hai/uaii/stream/base_output.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/stream/stream.py` & `hepai-1.1.1/hai/uaii/stream/stream.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/stream/streams.py` & `hepai-1.1.1/hai/uaii/stream/streams.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/uaii_main.py` & `hepai-1.1.1/hai/uaii/uaii_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/arbitrary_import.py` & `hepai-1.1.1/hai/uaii/utils/arbitrary_import.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/base_uaii.py` & `hepai-1.1.1/hai/uaii/utils/base_uaii.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/config_loader.py` & `hepai-1.1.1/hai/uaii/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/fake_argparse.py` & `hepai-1.1.1/hai/uaii/utils/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/general.py` & `hepai-1.1.1/hai/uaii/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/hai_hf_parser.py` & `hepai-1.1.1/hai/uaii/utils/hai_hf_parser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/utils/hf_argparser.py` & `hepai-1.1.1/hai/uaii/utils/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/worker/base_worker_model.py` & `hepai-1.1.1/hai/uaii/worker/base_worker_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         worker = MyWorker()
         worker.start()
     """
     def __init__(self, **kwargs) -> None:
         self.name = kwargs.pop('name', "hepai/worker-base-model")
         self.trainable = kwargs.pop('trainable', False)
         self.inferable = kwargs.pop('inferable', False)
+        self.allowd_functions = ['inference', 'train', 'evaluate', "chat_completions"]
 
     @staticmethod
     def convert(ret):
         for x in ret:
             yield x
 
     @staticmethod
```

### Comparing `hepai-1.1.0/hai/uaii/worker/run_worker.py` & `hepai-1.1.1/hai/uaii/worker/run_worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-import hai
-# from hai import BaseWorkerModel
+
+import os, sys
+from pathlib import Path    
+here = Path(__file__).parent
+try:
+    import hepai
+except:
+    sys.path.insert(0, f'{here.parent.parent.parent}')
+    import hepai
 from worker import WorkerWarper
 from base_worker_model import BaseWorkerModel
 from dataclasses import dataclass, field
 
 
 class WorkerModel(BaseWorkerModel):
     def __init__(self, name, **kwargs):
@@ -13,19 +20,21 @@
     def inference(self, **kwargs):
         # 自己的执行逻辑, 例如: # 
         input = kwargs.pop('input', None)
         output = [1, 2, 3, 4, 5]  # 修改为自己的输出
         return output, input
         # for i in output:
         #     yield i  # 可以return返回python的基础类型或yield生成器
+    
+    def chat_completions(self, **kwargs):
+        pass
+        raise NotImplementedError("Please implement this method")
 
-def run_worker(**kwargs):
-    # worker_args = hai.parse_args_into_dataclasses(WorkerArgs)  # 解析参数
-    model_args, worker_args = hai.parse_args_into_dataclasses((ModelArgs, WorkerArgs))  # 解析多个参数类
-    # print(worker_args)
+def run_worker(model_args, worker_args, **kwargs):
+    
     model = WorkerModel(  # 获取模型
         name=model_args.name
         # 此处可以传入其他参数
         )
     
     if worker_args.test:
         ret = model.inference(input='test')
@@ -54,14 +63,18 @@
     host: str = "0.0.0.0"  # worker的地址，0.0.0.0表示外部可访问，127.0.0.1表示只有本机可访问
     port: str = "auto"  # worker的端口，默认从42902开始自动分配
     controller_address: str = "http://aiapi.ihep.ac.cn:42901"  # 控制器的地址
     worker_address: str = "auto"  # 默认是http://<ip>:<port>
     limit_model_concurrency: int = 5  # 限制模型的并发请求
     stream_interval: float = 0.  # 额外的流式响应间隔
     no_register: bool = False  # 不注册到控制器
-    permissions: str = 'groups: all'  # 模型的权限授予，分为用户和组，用;分隔，例如：需要授权给所有组、a用户、b用户：'groups: all; users: a, b; owner: c'
+    permissions: str = 'groups: PAYG'  # 模型的权限授予，分为用户和组，用;分隔，例如：需要授权给所有组、a用户、b用户：'groups: all; users: a, b; owner: c'
     description: str = 'This is a demo worker in HeiAI-Distributed Deploy Framework'  # 模型的描述
     author: str = 'hepai'  # 模型的作者
     test: bool = False  # 测试模式，不会真正启动worker，只会打印参数
 
 if __name__ == '__main__':
-    run_worker()
+    # worker_args = hai.parse_args_into_dataclasses(WorkerArgs)  # 解析参数
+    model_args, worker_args = hepai.parse_args_into_dataclasses((ModelArgs, WorkerArgs))  # 解析多个参数类
+    # print(worker_args)
+    worker_args.controller_address = "http://ainpu.ihep.ac.cn:21601"
+    run_worker(model_args=model_args, worker_args=worker_args)
```

### Comparing `hepai-1.1.0/hai/uaii/worker/utils.py` & `hepai-1.1.1/hai/uaii/worker/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/hai/uaii/worker/worker.py` & `hepai-1.1.1/hai/uaii/worker/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     sys.path.append(str(here.parent.parent.parent))
     from hai.uaii.worker.utils import auto_port, auto_worker_address, pretty_print_semaphore
     from hai.uaii.worker.base_worker_model import BaseWorkerModel
 
 
 GB = 1 << 30
 
-logger = dm.get_logger('base_worker.py')
+logger = dm.get_logger('worker.py')
 global_counter = 0
 model_semaphore = None
 WORKER_HEART_BEAT_INTERVAL = 30
 
 
 def heart_beat_worker(controller):
     while True:
@@ -229,15 +229,34 @@
             # raise ValueError(f"Generator is empty: {e} {type(e)}")
         try:
             next(generator)
             raise ValueError("Generator should only have one element")
         except StopIteration:
             pass
         return content
-
+    
+    def unified_gate(self, **kwargs):
+        """
+        统一入口
+        """
+        assert "function" in kwargs, "function is required"
+        function = kwargs.pop("function")
+        try:
+            if hasattr(self.model, function) and callable(getattr(self.model, function)):
+                return getattr(self.model, function)(**kwargs)
+            else:
+                raise ValueError(f"Function {function} does not exist or is not callable in the model")
+        except Exception as e:
+            error_info = f'{type(e)} {e}'
+            logger.error(f'error_info: {error_info}\n {traceback.format_exc()}')
+            ret = {
+                "message": error_info,
+                "status_code": 42904, 
+            }
+            return ret
     
     def generate_stream_gate(self, **params):
         """
         生成流式响应的门
         :param params:
                 model: 模型名
                 其他参数
@@ -304,15 +323,15 @@
 import asyncio
 
 
 class WorkerAPP(FastAPI):
 
     def __init__(self):
         super().__init__()
-        self._worker = None
+        self._worker: Worker = None
 
     @property
     def worker(self):
         if self._worker is None:
             raise ValueError(
                 f"worker is not initialized, \
                 please call `WorkerAPP.worker = BaseWorker(**kwargs)` first")
@@ -324,14 +343,28 @@
         
 app = WorkerAPP()  # It's a FastAPI instance
 
 
 def release_model_semaphore():
     model_semaphore.release()
 
+@app.post("/worker_unified_gate")
+async def app_unified_gate(request: Request):
+    global model_semaphore, global_counter
+    global_counter += 1
+    params = await request.json()
+    if model_semaphore is None:
+        model_semaphore = asyncio.Semaphore(
+            app.worker.limit_model_concurrency)
+    await model_semaphore.acquire()
+    ret = app.worker.unified_gate(**params)
+    background_tasks = BackgroundTasks()  # 背景任务
+    background_tasks.add_task(release_model_semaphore)  # 释放锁
+    return ret
+
 @app.post("/worker_generate_stream")
 async def generate_stream(request: Request):
     global model_semaphore, global_counter
     global_counter += 1
     params = await request.json()
 
     if model_semaphore is None:
@@ -361,36 +394,20 @@
 
 
 @app.post("/worker_get_status")
 async def get_status(request: Request):
     return app.worker.get_status()
 
 
-# def get_args():
-#     parser = argparse.ArgumentParser()
-#     parser.add_argument("--host", type=str, default="127.0.0.1")
-#     parser.add_argument("--port", type=str, default='auto')
-#     parser.add_argument("--controller-address", type=str,
-#         default="http://127.0.0.1:42901")
-#     parser.add_argument("--worker-address", type=str,
-#         default="auto")
-#     parser.add_argument("--limit-model-concurrency", type=int, default=5, help="限制模型的并发请求")
-#     parser.add_argument("--stream-interval", type=int, default=0., help="额外的流式响应间隔")
-#     parser.add_argument("--no-register", action="store_true", help="不注册到控制器")
-#     parser.add_argument("--permissions", type=str, default='group: all', 
-#         help="模型权限授予谁,写法：'user: <user1>; user: <user2>; group: <group1>, ...'")
-#     args = parser.parse_args()
-#     logger.info(f"Args: {args}")
-#     return args
-
-    
 def run_worker(model=None, worker_args=None, daemon=False, test=False, **kwargs):
     args = worker_args or WorkerArgs()
     # print(f'worker args: {args}')
-    args.port = auto_port(args.port, start=42902)
+    if args.port == "auto":
+        start_port = args.__dict__.get("start_port", 42902)
+        args.port = auto_port(args.port, start=start_port)
     args.worker_address = auto_worker_address(args.worker_address, args.host, args.port)
     logger.info(f"Worker address: {args.worker_address}")
     if test:
         args.controller_address = "http://chat.ihep.ac.cn:4444"
 
     # 更新
     for k, v in kwargs.items():
@@ -436,15 +453,14 @@
     stream_interval: float = 0.  # 额外的流式响应间隔
     no_register: bool = False  # 不注册到控制器
     permissions: str = 'groups: all'  # 模型的权限授予，分为用户和组，用;分隔
     description: str = None  # 模型的描述
     author: str = None  # 模型的作者
 
 
-
 class WorkerWarper:
 
     @staticmethod
     def start(**kwargs):
         """
         运行一个hepai的worker
         :param model: BaseWorkerModel = None, 模型
```

### Comparing `hepai-1.1.0/hepai.egg-info/PKG-INFO` & `hepai-1.1.1/hepai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.1.0
+Version: 1.1.1
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.1.0 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.1.1 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `hepai-1.1.0/hepai.egg-info/SOURCES.txt` & `hepai-1.1.1/hepai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hepai-1.1.0/setup.py` & `hepai-1.1.1/setup.py`

 * *Files identical despite different names*

