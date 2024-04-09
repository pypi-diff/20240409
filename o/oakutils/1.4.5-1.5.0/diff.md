# Comparing `tmp/oakutils-1.4.5.tar.gz` & `tmp/oakutils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakutils-1.4.5.tar", last modified: Fri Mar  1 14:55:40 2024, max compression
+gzip compressed data, was "oakutils-1.5.0.tar", last modified: Tue Apr  9 04:01:05 2024, max compression
```

## Comparing `oakutils-1.4.5.tar` & `oakutils-1.5.0.tar`

### file list

```diff
@@ -1,1269 +1,1269 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.526765 oakutils-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-01 14:55:34.000000 oakutils-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-01 14:55:34.000000 oakutils-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-03-01 14:55:40.526765 oakutils-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-01 14:55:34.000000 oakutils-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-01 14:55:34.000000 oakutils-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 14:55:40.526765 oakutils-1.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.246764 oakutils-1.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.254764 oakutils-1.4.5/src/oakutils/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/_api_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    32764 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/_legacy_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/_webcam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.254764 oakutils-1.4.5/src/oakutils/aruco/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/aruco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/aruco/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/aruco/localizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/aruco/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.254764 oakutils-1.4.5/src/oakutils/blobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.254764 oakutils-1.4.5/src/oakutils/blobs/_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.254764 oakutils-1.4.5/src/oakutils/blobs/_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/_compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.258764 oakutils-1.4.5/src/oakutils/blobs/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/closing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/dilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/erosion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/gftt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/harris.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/opening.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/sobel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.258764 oakutils-1.4.5/src/oakutils/blobs/definitions/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/definitions/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.258764 oakutils-1.4.5/src/oakutils/blobs/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.310764 oakutils-1.4.5/src/oakutils/blobs/models/shave1/
--rw-r--r--   0 runner    (1001) docker     (127)   132792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)   169400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)   164088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)   168952 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)   164280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)   163832 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)   159992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)   160952 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)   168120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)   167672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)   163064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)   158648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)   134136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    30584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37688 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32632 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)   131512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)   160888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)   168056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)   167672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)   162488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)   158584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)   159608 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)   166776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)   161528 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)   166328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)   161656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)   161208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)   157304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    70840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    77944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72696 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    77496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    68536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    69496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    76664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    71416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    76216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    71544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    71224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    67192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    42616 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    46840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    67448 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    64824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48760 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    67064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    64376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    56440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    62456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51832 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    62136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51000 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    45048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    44536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    50104 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59448 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    56696 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    46328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48696 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    45752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    66488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    63800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59448 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55864 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    61304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58552 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    50616 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    66168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    63416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    53112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    55480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    52216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    61496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    50744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    51896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    61176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    48056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    50424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47864 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57144 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    54392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    50040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    44088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    43512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25144 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17592 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)    41016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    70456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    77624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    77176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    72184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    68152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    69176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    76344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    71032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    75896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    71224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    70904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    42296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.354765 oakutils-1.4.5/src/oakutils/blobs/models/shave2/
--rw-r--r--   0 runner    (1001) docker     (127)    47928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49144 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    46520 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58616 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59000 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57592 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57720 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    33208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29880 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.394765 oakutils-1.4.5/src/oakutils/blobs/models/shave3/
--rw-r--r--   0 runner    (1001) docker     (127)    47928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    60856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    49144 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    46520 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58616 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59000 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57592 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57720 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    57784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    58232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    33208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    29880 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    24568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.438765 oakutils-1.4.5/src/oakutils/blobs/models/shave4/
--rw-r--r--   0 runner    (1001) docker     (127)    30200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.478765 oakutils-1.4.5/src/oakutils/blobs/models/shave5/
--rw-r--r--   0 runner    (1001) docker     (127)    30200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    31480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.510765 oakutils-1.4.5/src/oakutils/blobs/models/shave6/
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTT.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36856 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    30328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    27704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Harris.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35000 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35256 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    35960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    34040 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    34168 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    34360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    28920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Hessian.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16632 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17272 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15096 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/PointCloud.blob
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/Sobel.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_11x11.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_13x13.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_15x15.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_3x3.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_5x5.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_7x7.blob
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_9x9.blob
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelGray.blob
--rw-r--r--   0 runner    (1001) docker     (127)    40478 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/blobs/models/shave6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.510765 oakutils-1.4.5/src/oakutils/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/calibration/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/calibration/_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.514765 oakutils-1.4.5/src/oakutils/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/filters/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/filters/wls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.514765 oakutils-1.4.5/src/oakutils/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/color_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/image_manip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/mobilenet_detection_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.514765 oakutils-1.4.5/src/oakutils/nodes/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/gftt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/harris.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/models/sobel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/mono_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/stereo_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/xin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/xout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/nodes/yolo_detection_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.518766 oakutils-1.4.5/src/oakutils/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/optimizer/_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/optimizer/_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/optimizer/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.518766 oakutils-1.4.5/src/oakutils/point_clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/point_clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/point_clouds/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/point_clouds/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/point_clouds/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.518766 oakutils-1.4.5/src/oakutils/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/tools/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.518766 oakutils-1.4.5/src/oakutils/vpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/vpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/vpu/_model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-03-01 14:55:34.000000 oakutils-1.4.5/src/oakutils/vpu/_vpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:55:40.518766 oakutils-1.4.5/src/oakutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-03-01 14:55:40.000000 oakutils-1.4.5/src/oakutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    71120 2024-03-01 14:55:40.000000 oakutils-1.4.5/src/oakutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 14:55:40.000000 oakutils-1.4.5/src/oakutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-01 14:55:40.000000 oakutils-1.4.5/src/oakutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 14:55:40.000000 oakutils-1.4.5/src/oakutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.892082 oakutils-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 04:00:54.000000 oakutils-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 04:00:54.000000 oakutils-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-09 04:01:05.892082 oakutils-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-09 04:00:54.000000 oakutils-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-09 04:00:54.000000 oakutils-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:01:05.892082 oakutils-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.616083 oakutils-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.620083 oakutils-1.5.0/src/oakutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/_api_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32764 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/_legacy_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/_webcam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.620083 oakutils-1.5.0/src/oakutils/aruco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/aruco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/aruco/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/aruco/localizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/aruco/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.620083 oakutils-1.5.0/src/oakutils/blobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.624083 oakutils-1.5.0/src/oakutils/blobs/_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.624083 oakutils-1.5.0/src/oakutils/blobs/_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/_compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.624083 oakutils-1.5.0/src/oakutils/blobs/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/closing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/dilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/erosion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/gftt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/harris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/opening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/sobel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.628083 oakutils-1.5.0/src/oakutils/blobs/definitions/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/definitions/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.628083 oakutils-1.5.0/src/oakutils/blobs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.676083 oakutils-1.5.0/src/oakutils/blobs/models/shave1/
+-rw-r--r--   0 runner    (1001) docker     (127)   132792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   169400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   164088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   168952 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   164280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   163832 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   159992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   160952 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   168120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   167672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   163064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   158648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   134136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    30584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37688 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32632 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   131512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   160888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   168056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   167672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   162488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   158584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   159608 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   166776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   161528 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   166328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   161656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   161208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   157304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    70840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    77944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72696 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    77496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    68536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    69496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    76664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    71416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    76216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    71544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    71224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    67192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    42616 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    46840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    67448 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    64824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48760 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    67064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    64376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    56440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    62456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51832 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    62136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51000 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    45048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    44536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    50104 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59448 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    56696 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    46328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48696 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    45752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    66488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    63800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59448 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55864 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    61304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58552 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    50616 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    56888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    66168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    63416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    53112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    55480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    52216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    61496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    50744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    51896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    61176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    48056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    50424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47864 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57144 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    54392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    50040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    44088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    43512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25144 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17592 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    41016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    70456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    77624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    77176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    72184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    68152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    69176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    76344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    71032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    75896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    71224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    70904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    66936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    42296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.716083 oakutils-1.5.0/src/oakutils/blobs/models/shave2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49144 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    46520 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58616 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59000 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57592 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57720 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    33208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29880 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.756083 oakutils-1.5.0/src/oakutils/blobs/models/shave3/
+-rw-r--r--   0 runner    (1001) docker     (127)    47928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    60856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    49144 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    46520 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58616 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59000 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    59576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57592 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57720 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    57784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    58232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    47800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    33208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    29880 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    24568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.796083 oakutils-1.5.0/src/oakutils/blobs/models/shave4/
+-rw-r--r--   0 runner    (1001) docker     (127)    30200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.840082 oakutils-1.5.0/src/oakutils/blobs/models/shave5/
+-rw-r--r--   0 runner    (1001) docker     (127)    30200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    38520 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    31480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.880082 oakutils-1.5.0/src/oakutils/blobs/models/shave6/
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTT.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36856 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    37304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    30328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    27704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Harris.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35000 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35256 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35512 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    35960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    34040 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    34168 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    34360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    28920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Hessian.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17848 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16632 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17272 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15096 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    21560 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/PointCloud.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/Sobel.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_11x11.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_13x13.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_15x15.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_3x3.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_5x5.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_7x7.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_9x9.blob
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelGray.blob
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/blobs/models/shave6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.880082 oakutils-1.5.0/src/oakutils/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/calibration/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21304 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/calibration/_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.880082 oakutils-1.5.0/src/oakutils/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/filters/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/filters/wls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.880082 oakutils-1.5.0/src/oakutils/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/color_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/image_manip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/mobilenet_detection_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils/nodes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/gftt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/harris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/models/sobel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/mono_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17261 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/stereo_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/xin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/xout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/nodes/yolo_detection_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/optimizer/_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/optimizer/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/optimizer/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils/point_clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/point_clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/point_clouds/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/point_clouds/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/point_clouds/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/tools/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils/vpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/vpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/vpu/_model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-04-09 04:00:54.000000 oakutils-1.5.0/src/oakutils/vpu/_vpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:01:05.884082 oakutils-1.5.0/src/oakutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-09 04:01:05.000000 oakutils-1.5.0/src/oakutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    71120 2024-04-09 04:01:05.000000 oakutils-1.5.0/src/oakutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:01:05.000000 oakutils-1.5.0/src/oakutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 04:01:05.000000 oakutils-1.5.0/src/oakutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 04:01:05.000000 oakutils-1.5.0/src/oakutils.egg-info/top_level.txt
```

### Comparing `oakutils-1.4.5/LICENSE` & `oakutils-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/PKG-INFO` & `oakutils-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakutils
-Version: 1.4.5
+Version: 1.5.0
 Author-email: Justin Davis <davisjustin302@gmail.com>
 Maintainer-email: Justin Davis <davisjustin302@gmail.com>
 Project-URL: Homepage, https://github.com/justincdavis/oakutils
 Project-URL: Bug Tracker, https://github.com/justincdavis/oakutils/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -35,18 +35,20 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Typing :: Typed
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: depthai>=2.24
 Requires-Dist: numpy<2.0,>=1.20
-Requires-Dist: open3d>=0.18.0
 Requires-Dist: opencv-contrib-python>=4.9.0
+Requires-Dist: cv2ext>=0.0.10
 Requires-Dist: typing_extensions>=4.9.0
 Requires-Dist: setuptools>=57.0.0
+Provides-Extra: o3d
+Requires-Dist: open3d>=0.18.0; extra == "o3d"
 Provides-Extra: compiler
 Requires-Dist: kornia>=0.6.0; extra == "compiler"
 Requires-Dist: torch>=1.9.0; extra == "compiler"
 Requires-Dist: onnx>=1.15.0; extra == "compiler"
 Requires-Dist: onnxruntime>=1.15.0; extra == "compiler"
 Requires-Dist: onnxsim>=0.4.33; extra == "compiler"
 Requires-Dist: blobconverter==1.4.3; extra == "compiler"
@@ -64,14 +66,15 @@
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.1.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: myst_parser>=1.0.0; extra == "docs"
 Provides-Extra: dev
+Requires-Dist: oakutils[o3d]; extra == "dev"
 Requires-Dist: oakutils[compiler]; extra == "dev"
 Requires-Dist: oakutils[ci]; extra == "dev"
 Requires-Dist: oakutils[test]; extra == "dev"
 Requires-Dist: oakutils[docs]; extra == "dev"
 Requires-Dist: twine>=4.0.0; extra == "dev"
 Requires-Dist: wheel>=0.37.0; extra == "dev"
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
```

### Comparing `oakutils-1.4.5/README.md` & `oakutils-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/pyproject.toml` & `oakutils-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oakutils"
-version = "1.4.5"
+version = "1.5.0"
 authors = [
   {name="Justin Davis", email="davisjustin302@gmail.com"},
 ]
 maintainers = [
   {name="Justin Davis", email="davisjustin302@gmail.com"},
 ]
 readme = "README.md"
@@ -43,25 +43,28 @@
     "Intended Audience :: End Users/Desktop",
     "Typing :: Typed",
 ]
 requires-python=">=3.8, <3.12"
 dependencies = [
     "depthai>=2.24",
     "numpy>=1.20,<2.0",
-    "open3d>=0.18.0",
     "opencv-contrib-python>=4.9.0",
+    "cv2ext>=0.0.10",
     "typing_extensions>=4.9.0",
     "setuptools>=57.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/justincdavis/oakutils"
 "Bug Tracker" = "https://github.com/justincdavis/oakutils/issues"
 
 [project.optional-dependencies]
+o3d = [
+    "open3d>=0.18.0",
+]
 compiler = [
     "kornia>=0.6.0",
     "torch>=1.9.0",
     "onnx>=1.15.0",
     "onnxruntime>=1.15.0",
     "onnxsim>=0.4.33",
     "blobconverter==1.4.3",
@@ -83,27 +86,28 @@
 ]
 docs = [
     "sphinx>=6.1.0",
     "sphinx-rtd-theme>=1.3.0",
     "myst_parser>=1.0.0",
 ]
 dev = [
+    "oakutils[o3d]",
     "oakutils[compiler]",
     "oakutils[ci]",
     "oakutils[test]",
     "oakutils[docs]",
     "twine>=4.0.0",
     "wheel>=0.37.0",
     "bumpver>=2023.1126",
     "pyclean>=2.7.0",
     "pyright>=1.1.348",
 ]
 
 [tool.bumpver]
-current_version = "1.4.5"
+current_version = "1.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `oakutils-1.4.5/src/oakutils/__init__.py` & `oakutils-1.5.0/src/oakutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     A class for reading frames from an OAK using the same interface as cv2.VideoCapture.
 VPU
     A class for using the onboard VPU as a standalone processor.
 """
 from __future__ import annotations
 
 # setup the logger before importing anything else
+import contextlib
 import logging
 import os
 import sys
 
 
 # Created from answer by Dennis at:
 # https://stackoverflow.com/questions/7621897/python-logging-module-globally
@@ -131,30 +132,34 @@
     nodes,
     optimizer,
     point_clouds,
     tools,
     vpu,
 )
 from ._api_camera import ApiCamera
-from ._legacy_camera import LegacyCamera
 from ._webcam import Webcam
 from .vpu import VPU
 
 __all__ = [
     "VPU",
     "ApiCamera",
-    "LegacyCamera",
     "Webcam",
     "aruco",
     "blobs",
     "calibration",
     "filters",
     "nodes",
     "optimizer",
     "point_clouds",
     "set_log_level",
     "tools",
     "vpu",
 ]
-__version__ = "1.4.5"
+
+with contextlib.suppress(ImportError):
+    from ._legacy_camera import LegacyCamera
+
+    __all__ += ["LegacyCamera"]
+
+__version__ = "1.5.0"
 
 _log.info(f"Initialized oakutils with version {__version__}")
```

### Comparing `oakutils-1.4.5/src/oakutils/_api_camera.py` & `oakutils-1.5.0/src/oakutils/_api_camera.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,36 +24,43 @@
 import atexit
 import contextlib
 from functools import partial
 from threading import Condition, Thread
 from typing import TYPE_CHECKING, Callable, Iterable
 
 import depthai as dai
+from typing_extensions import TypeAlias
 
 from .calibration import CalibrationData, get_camera_calibration
-from .point_clouds import PointCloudVisualizer
 from .tools.display import DisplayManager, get_smaller_size
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
+try:
+    from .point_clouds import PointCloudVisualizer
+except ImportError:
+    PointCloudVisualizer = None  # type: ignore[assignment, misc]
+
+PCVisualizer: TypeAlias = "PointCloudVisualizer | None"  # type: ignore[name-defined]
+
 
 class ApiCamera:
     """
     A lightweight class for creating custom pipelines using callbacks.
 
     Attributes
     ----------
     pipeline:
         The pipeline for the camera
     calibration : CalibrationData
         The calibration info for the camera
     displays : DisplayManager
         The display manager for the camera
-    pcv : PointCloudVisualizer
+    pcv : PCVisualizer
         The point cloud visualizer for the camera
 
     Methods
     -------
     start(blocking=False)
         Start the camera.
     stop()
@@ -109,15 +116,15 @@
 
         # handle custom displays directly for API stuff without visualize
         self._display_size: tuple[int, int] = get_smaller_size(
             self._color_size,
             self._mono_size,
         )
         self._displays: DisplayManager | None = None
-        self._pcv: PointCloudVisualizer | None = None
+        self._pcv: PCVisualizer | None = None
 
         # thread for reading camera
         self._started = False
         self._stopped: bool = False
         self._thread: Thread = Thread(target=self._run, daemon=True)
         self._start_condition: Condition = Condition()
         self._stop_condition: Condition = Condition()
@@ -156,17 +163,27 @@
     def displays(self: Self) -> DisplayManager:
         """Use to get the display manager."""
         if self._displays is None:
             self._displays = DisplayManager(display_size=self._display_size)
         return self._displays
 
     @property
-    def pcv(self: Self) -> PointCloudVisualizer:
-        """Use to get the point cloud visualizer."""
-        if self._pcv is None:
+    def pcv(self: Self) -> PCVisualizer | None:
+        """
+        Use to get the point cloud visualizer.
+
+        If open3d is not installed, this will always return None.
+
+        Returns
+        -------
+        PointCloudVisualizer | None
+            The point cloud visualizer.
+
+        """
+        if self._pcv is None and PointCloudVisualizer is not None:
             self._pcv = PointCloudVisualizer(window_size=self._display_size)
         return self._pcv
 
     def start(self: Self, *, blocking: bool | None = None) -> None:
         """Use to start the camera. To be done after all api calls are made."""
         if blocking is None:
             blocking = False
```

### Comparing `oakutils-1.4.5/src/oakutils/_legacy_camera.py` & `oakutils-1.5.0/src/oakutils/_legacy_camera.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/_webcam.py` & `oakutils-1.5.0/src/oakutils/_webcam.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/aruco/__init__.py` & `oakutils-1.5.0/src/oakutils/aruco/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/aruco/finder.py` & `oakutils-1.5.0/src/oakutils/aruco/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,18 @@
             image = cv2.undistort(
                 image,
                 self._K,
                 self._D,
                 None,
                 self._K,
             )
-        corners, ids, _ = cv2.aruco.detectMarkers(image, self._adict)
+        corners, ids, _ = cv2.aruco.detectMarkers(image, self._adict)  # type: ignore[attr-defined]
         ret_val: list[tuple[int, np.ndarray, np.ndarray, np.ndarray, np.ndarray]] = []
         for idx, corner in enumerate(corners):
-            rvecs, tvecs, _ = cv2.aruco.estimatePoseSingleMarkers(
+            rvecs, tvecs, _ = cv2.aruco.estimatePoseSingleMarkers(  # type: ignore[attr-defined]
                 [corner],
                 self._marker_size,
                 self._K,
                 self._D,
             )
             try:
                 rvec = rvecs[0]
```

### Comparing `oakutils-1.4.5/src/oakutils/aruco/localizer.py` & `oakutils-1.5.0/src/oakutils/aruco/localizer.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/aruco/stream.py` & `oakutils-1.5.0/src/oakutils/aruco/stream.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_cache/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/blob.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/blob.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/compile.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/compile.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/onnx.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/onnx.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/paths.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/paths.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/torch.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/torch.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/_compiler/utils.py` & `oakutils-1.5.0/src/oakutils/blobs/_compiler/utils.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/abstract_model.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/abstract_model.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/closing.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/closing.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/dilation.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/dilation.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/erosion.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/erosion.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/gaussian.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/gaussian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/gftt.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/gftt.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/harris.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/harris.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/hessian.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/hessian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/laplacian.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/laplacian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/opening.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/opening.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/point_cloud.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/point_cloud.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/sobel.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/sobel.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/utils/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/utils/conversion.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/definitions/utils/types.py` & `oakutils-1.5.0/src/oakutils/blobs/definitions/utils/types.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave1/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave1"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave2/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave2"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave3/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave3"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave4/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave4/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave4"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave5/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave5"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTT.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTT.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GFTTGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GFTTGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/GaussianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/GaussianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Gaussian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Gaussian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Harris.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Harris.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HarrisGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HarrisGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Hessian.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Hessian.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/HessianGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/HessianGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlurGray_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_11x11_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_13x13_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_15x15_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_3x3_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_5x5_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_7x7_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianBlur_9x9_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/LaplacianGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/LaplacianGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Laplacian_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Laplacian_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/PointCloud.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/PointCloud.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/Sobel.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/Sobel.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlurGray_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlurGray_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_11x11.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_11x11.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_13x13.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_13x13.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_15x15.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_15x15.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_3x3.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_3x3.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_5x5.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_5x5.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_7x7.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_7x7.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelBlur_9x9.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelBlur_9x9.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/SobelGray.blob` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/SobelGray.blob`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/blobs/models/shave6/__init__.py` & `oakutils-1.5.0/src/oakutils/blobs/models/shave6/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,24 @@
 
 from pathlib import Path
 
 import pkg_resources
 
 _RELATIVE_BLOB_FOLDER = Path("oakutils") / "blobs" / "models" / "shave6"
 _PACKAGE_LOCATION = pkg_resources.get_distribution("oakutils").location
+if _PACKAGE_LOCATION is None:
+    err_msg = "Could not find package location"
+    raise RuntimeError(err_msg)
+_PACKAGE_LOCATION_PATH = Path(_PACKAGE_LOCATION)
+if not _PACKAGE_LOCATION_PATH.exists():
+    err_msg = "Package location does not exist"
+    raise RuntimeError(err_msg)
+if not _PACKAGE_LOCATION_PATH.is_dir():
+    err_msg = "Package location is not a directory"
+    raise RuntimeError(err_msg)
 _BLOB_FOLDER = Path(_PACKAGE_LOCATION) / _RELATIVE_BLOB_FOLDER
 
 GFTT = Path(Path(_BLOB_FOLDER) / "GFTT.blob").resolve()
 GFTTBLURGRAY_11X11 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_11x11.blob").resolve()
 GFTTBLURGRAY_13X13 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_13x13.blob").resolve()
 GFTTBLURGRAY_15X15 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_15x15.blob").resolve()
 GFTTBLURGRAY_3X3 = Path(Path(_BLOB_FOLDER) / "GFTTBlurGray_3x3.blob").resolve()
```

### Comparing `oakutils-1.4.5/src/oakutils/calibration/__init__.py` & `oakutils-1.5.0/src/oakutils/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/calibration/_classes.py` & `oakutils-1.5.0/src/oakutils/calibration/_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,29 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
+from typing_extensions import TypeAlias
+
 if TYPE_CHECKING:
     import numpy as np
-    import open3d as o3d  # type: ignore[import]
+
+try:
+    import open3d as o3d  # type: ignore[import-not-found, import-untyped]
+
+    PinholeCameraIntrinsicType: o3d.camera.PinholeCameraIntrinsic = (
+        o3d.camera.PinholeCameraIntrinsic
+    )
+except ImportError:
+    PinholeCameraIntrinsicType = None
+
+PinholeCameraIntrinsic: TypeAlias = "PinholeCameraIntrinsicType | None"  # type: ignore[name-defined]
 
 
 @dataclass(frozen=True)
 class MonoCalibrationData:
     """
     Class to store calibration data for a mono camera.
 
@@ -54,15 +66,15 @@
         Homography matrix.
     valid_region : Optional[Tuple[int, int, int, int]], optional
         Valid region of the calibration generated by cv2.stereoRectify.
     map_1 : Optional[np.ndarray], optional
         Map 1 for undistortion generated by cv2.initUndistortRectifyMap.
     map_2 : Optional[np.ndarray], optional
         Map 2 for undistortion generated by cv2.initUndistortRectifyMap.
-    pinhole : Optional[o3d.camera.PinholeCameraIntrinsic], optional
+    pinhole : Optional[PinholeCameraIntrinsic], optional
         o3d pinhole camera intrinsic.
 
     """
 
     size: tuple[int, int]
     K: np.ndarray
     D: np.ndarray
@@ -74,15 +86,15 @@
     fov_rad: float
     R: np.ndarray
     T: np.ndarray
     H: np.ndarray
     valid_region: tuple[int, int, int, int] | None = None
     map_1: np.ndarray | None = None
     map_2: np.ndarray | None = None
-    pinhole: o3d.camera.PinholeCameraIntrinsic | None = None
+    pinhole: PinholeCameraIntrinsic | None = None
 
 
 @dataclass(frozen=True)
 class StereoCalibrationData:
     """
     Class to store calibration data for stereo cameras.
 
@@ -126,15 +138,15 @@
         R2 matrix generated by cv2.stereoRectify.
     P1 : Optional[np.ndarray], optional
         P1 matrix generated by cv2.stereoRectify.
     P2 : Optional[np.ndarray], optional
         P2 matrix generated by cv2.stereoRectify.
     valid_region_primary : Optional[Tuple[int, int, int, int]], optional
         Valid region of the primary camera.
-    pinhole_primary : Optional[o3d.camera.PinholeCameraIntrinsic], optional
+    pinhole_primary : Optional[PinholeCameraIntrinsic], optional
         o3d pinhole camera intrinsic for the primary camera.
 
     See Also
     --------
     MonoCalibrationData : Class to store calibration data for a mono camera.
 
     """
@@ -156,15 +168,15 @@
     Q_primary: np.ndarray | None = None
     Q_cv2: np.ndarray | None = None
     R1_cv2: np.ndarray | None = None
     R2_cv2: np.ndarray | None = None
     P1: np.ndarray | None = None
     P2: np.ndarray | None = None
     valid_region_primary: tuple[int, int, int, int] | None = None
-    pinhole_primary: o3d.camera.PinholeCameraIntrinsic | None = None
+    pinhole_primary: PinholeCameraIntrinsic | None = None
 
 
 @dataclass(frozen=True)
 class ColorCalibrationData:
     """
     Class to store calibration data for a color camera.
 
@@ -192,15 +204,15 @@
         Projection matrix.
     valid_region : Optional[Tuple[int, int, int, int]], optional
         Valid region of the calibration generated by cv2.getOptimalNewCameraMatrix.
     map_1 : Optional[np.ndarray], optional
         Map 1 for undistortion generated by cv2.initUndistortRectifyMap.
     map_2 : Optional[np.ndarray], optional
         Map 2 for undistortion generated by cv2.initUndistortRectifyMap.
-    pinhole : Optional[o3d.camera.PinholeCameraIntrinsic], optional
+    pinhole : Optional[PinholeCameraIntrinsic], optional
         o3d pinhole camera intrinsic.
 
     """
 
     size: tuple[int, int]
     K: np.ndarray
     D: np.ndarray
@@ -210,15 +222,15 @@
     cy: float
     fov: float
     fov_rad: float
     P: np.ndarray | None = None
     valid_region: tuple[int, int, int, int] | None = None
     map_1: np.ndarray | None = None
     map_2: np.ndarray | None = None
-    pinhole: o3d.camera.PinholeCameraIntrinsic | None = None
+    pinhole: PinholeCameraIntrinsic | None = None
 
 
 @dataclass(frozen=True)
 class CalibrationData:
     """
     An object to store calibration data for an entire OAK camera.
```

### Comparing `oakutils-1.4.5/src/oakutils/calibration/_funcs.py` & `oakutils-1.5.0/src/oakutils/calibration/_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 import cv2  # type: ignore[import]
 import depthai as dai
 import numpy as np
-import open3d as o3d  # type: ignore[import]
+
+try:
+    import open3d as o3d  # type: ignore[import]
+
+    PinholeCameraIntrinsic = o3d.camera.PinholeCameraIntrinsic
+except ImportError:
+    PinholeCameraIntrinsic = None
 
 from ._classes import (
     CalibrationData,
     ColorCalibrationData,
     MonoCalibrationData,
     StereoCalibrationData,
 )
@@ -507,22 +513,24 @@
         data.rgb.K,
         data.rgb.D,
         None,  # pyright: ignore[reportArgumentType]
         p_rgb,
         rgb_size,
         cv2.CV_16SC2,  # type: ignore[attr-defined]
     )  # type: ignore[call-overload]
-    pinhole_rgb = o3d.camera.PinholeCameraIntrinsic(
-        width=rgb_size[0],
-        height=rgb_size[1],
-        fx=data.rgb.fx,
-        fy=data.rgb.fy,
-        cx=data.rgb.cx,
-        cy=data.rgb.cy,
-    )
+    pinhole_rgb = None
+    if PinholeCameraIntrinsic is not None:
+        pinhole_rgb = PinholeCameraIntrinsic(
+            width=rgb_size[0],
+            height=rgb_size[1],
+            fx=data.rgb.fx,
+            fy=data.rgb.fy,
+            cx=data.rgb.cx,
+            cy=data.rgb.cy,
+        )
 
     # add the pinhole data and maps to the data.rgb object
     rgb = ColorCalibrationData(
         size=data.rgb.size,
         K=data.rgb.K,
         D=data.rgb.D,
         fx=data.rgb.fx,
@@ -575,30 +583,34 @@
     valid_region_primary = (
         valid_region_left if is_primary_mono_left else valid_region_right
     )
     map_1_primary = map_left_1 if is_primary_mono_left else map_right_1
     map_2_primary = map_left_2 if is_primary_mono_left else map_right_2
 
     # create o3d PinholeCameraIntrinsic objects for left, right, and primary mono cams
-    pinhole_left = o3d.camera.PinholeCameraIntrinsic(
-        width=mono_size[0],
-        height=mono_size[1],
-        fx=data.left.fx,
-        fy=data.left.fy,
-        cx=data.left.cx,
-        cy=data.left.cy,
-    )
-    pinhole_right = o3d.camera.PinholeCameraIntrinsic(
-        width=mono_size[0],
-        height=mono_size[1],
-        fx=data.right.fx,
-        fy=data.right.fy,
-        cx=data.right.cx,
-        cy=data.right.cy,
-    )
+    pinhole_left = None
+    if PinholeCameraIntrinsic is not None:
+        pinhole_left = PinholeCameraIntrinsic(
+            width=mono_size[0],
+            height=mono_size[1],
+            fx=data.left.fx,
+            fy=data.left.fy,
+            cx=data.left.cx,
+            cy=data.left.cy,
+        )
+    pinhole_right = None
+    if PinholeCameraIntrinsic is not None:
+        pinhole_right = PinholeCameraIntrinsic(
+            width=mono_size[0],
+            height=mono_size[1],
+            fx=data.right.fx,
+            fy=data.right.fy,
+            cx=data.right.cx,
+            cy=data.right.cy,
+        )
     pinhole_primary = pinhole_left if is_primary_mono_left else pinhole_right
 
     # add the data to the data.left, data.right, and data.primary objects
     left = MonoCalibrationData(
         size=data.left.size,
         K=data.left.K,
         D=data.left.D,
```

### Comparing `oakutils-1.4.5/src/oakutils/filters/__init__.py` & `oakutils-1.5.0/src/oakutils/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/filters/smoothing.py` & `oakutils-1.5.0/src/oakutils/filters/smoothing.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/filters/wls.py` & `oakutils-1.5.0/src/oakutils/filters/wls.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         """
         self._data: StereoCalibrationData = cam_data
         self._lambda: int = lamb
         self._sigma: float = sigma
         self._disp_levels: int = disp_levels
         self._depth_scale_left: float | None = None
         self._depth_scale_right: float | None = None
-        self._filter = cv2.ximgproc.createDisparityWLSFilterGeneric(
+        self._filter = cv2.ximgproc.createDisparityWLSFilterGeneric(  # type: ignore[attr-defined]
             use_confidence=False,
         )
         self._filter.setLambda(self._lambda)
         self._filter.setSigmaColor(self._sigma)
 
     @property
     def lamb(self: Self) -> int:
```

### Comparing `oakutils-1.4.5/src/oakutils/nodes/__init__.py` & `oakutils-1.5.0/src/oakutils/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/_misc.py` & `oakutils-1.5.0/src/oakutils/nodes/_misc.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/color_camera.py` & `oakutils-1.5.0/src/oakutils/nodes/color_camera.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/image_manip.py` & `oakutils-1.5.0/src/oakutils/nodes/image_manip.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/imu.py` & `oakutils-1.5.0/src/oakutils/nodes/imu.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/mobilenet_detection_network.py` & `oakutils-1.5.0/src/oakutils/nodes/mobilenet_detection_network.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/__init__.py` & `oakutils-1.5.0/src/oakutils/nodes/models/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/_load.py` & `oakutils-1.5.0/src/oakutils/nodes/models/_load.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/_parsing.py` & `oakutils-1.5.0/src/oakutils/nodes/models/_parsing.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/gaussian.py` & `oakutils-1.5.0/src/oakutils/nodes/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/gftt.py` & `oakutils-1.5.0/src/oakutils/nodes/models/gftt.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/harris.py` & `oakutils-1.5.0/src/oakutils/nodes/models/harris.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/hessian.py` & `oakutils-1.5.0/src/oakutils/nodes/models/hessian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/laplacian.py` & `oakutils-1.5.0/src/oakutils/nodes/models/laplacian.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/point_cloud.py` & `oakutils-1.5.0/src/oakutils/nodes/models/point_cloud.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/models/sobel.py` & `oakutils-1.5.0/src/oakutils/nodes/models/sobel.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/mono_camera.py` & `oakutils-1.5.0/src/oakutils/nodes/mono_camera.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/neural_network.py` & `oakutils-1.5.0/src/oakutils/nodes/neural_network.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/stereo_depth.py` & `oakutils-1.5.0/src/oakutils/nodes/stereo_depth.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/xin.py` & `oakutils-1.5.0/src/oakutils/nodes/xin.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/xout.py` & `oakutils-1.5.0/src/oakutils/nodes/xout.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/nodes/yolo_detection_network.py` & `oakutils-1.5.0/src/oakutils/nodes/yolo_detection_network.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/optimizer/__init__.py` & `oakutils-1.5.0/src/oakutils/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/optimizer/_grid_search.py` & `oakutils-1.5.0/src/oakutils/optimizer/_grid_search.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/optimizer/_optimizer.py` & `oakutils-1.5.0/src/oakutils/optimizer/_optimizer.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/optimizer/objective.py` & `oakutils-1.5.0/src/oakutils/optimizer/objective.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/point_clouds/__init__.py` & `oakutils-1.5.0/src/oakutils/point_clouds/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 """
 Moudule for creating, filtering, and visualizing point clouds.
 
+Module contents will only be populated if the 'open3d' package is installed.
+This is to reduce the minimun required dependencies for the 'oakutils' package.
+Since the 'open3d' package is not required for all operations and it is a
+large package, it is not included in the 'oakutils' package dependencies
+by default.
+
 Submoudles
 ----------
 callbacks
     Callbacks for point cloud creation and filtering.
 
 Classes
 -------
@@ -33,26 +39,35 @@
 get_point_cloud_from_depth_image
     Use to create a point cloud from a depth image.
 get_point_cloud_from_rgb_depth_image
     Use to create a point cloud from a RGB and depth image.
 create_point_cloud
     Use to create a point cloud from a RGB and depth image as a callback.
 """
-from . import callbacks
-from ._classes import PointCloudVisualizer
-from ._funcs import (
-    filter_point_cloud,
-    get_point_cloud_from_depth_image,
-    get_point_cloud_from_np_buffer,
-    get_point_cloud_from_rgb_depth_image,
-)
-from .callbacks import create_point_cloud
-
-__all__ = [
-    "PointCloudVisualizer",
-    "callbacks",
-    "create_point_cloud",
-    "filter_point_cloud",
-    "get_point_cloud_from_depth_image",
-    "get_point_cloud_from_np_buffer",
-    "get_point_cloud_from_rgb_depth_image",
-]
+import logging
+
+_log = logging.getLogger(__name__)
+
+try:
+    from . import callbacks
+    from ._classes import PointCloudVisualizer
+    from ._funcs import (
+        filter_point_cloud,
+        get_point_cloud_from_depth_image,
+        get_point_cloud_from_np_buffer,
+        get_point_cloud_from_rgb_depth_image,
+    )
+    from .callbacks import create_point_cloud
+
+    __all__ = [
+        "PointCloudVisualizer",
+        "callbacks",
+        "create_point_cloud",
+        "filter_point_cloud",
+        "get_point_cloud_from_depth_image",
+        "get_point_cloud_from_np_buffer",
+        "get_point_cloud_from_rgb_depth_image",
+    ]
+except ImportError:
+    _log.warning(
+        "The 'open3d' package is not installed. Point cloud submodule will not be available.",
+    )
```

### Comparing `oakutils-1.4.5/src/oakutils/point_clouds/_classes.py` & `oakutils-1.5.0/src/oakutils/point_clouds/_classes.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/point_clouds/_funcs.py` & `oakutils-1.5.0/src/oakutils/point_clouds/_funcs.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/point_clouds/callbacks.py` & `oakutils-1.5.0/src/oakutils/point_clouds/callbacks.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/__init__.py` & `oakutils-1.5.0/src/oakutils/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/depth.py` & `oakutils-1.5.0/src/oakutils/tools/depth.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/display.py` & `oakutils-1.5.0/src/oakutils/tools/display.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,71 +27,26 @@
     Orders the given resolutions from smallest to largest.
 get_smaller_size
     Gets the smaller size of the two given sizes.
 """
 from __future__ import annotations
 
 import atexit
-import contextlib
-import time
 from collections import defaultdict
-from threading import Thread
 from typing import TYPE_CHECKING, Callable, Iterable
 
 import cv2  # type: ignore[import]
+from cv2ext import Display
 
 if TYPE_CHECKING:
     import depthai as dai
     import numpy as np
     from typing_extensions import Self
 
 
-class _Display:
-    def __init__(self: Self, name: str, fps: int = 15) -> None:
-        self._name = name
-        self._fps = fps
-        self._delay_time: float = 1 / fps
-        self._frame: np.ndarray | None = None
-        self._stopped = False
-        self._thread = Thread(target=self._run)
-        atexit.register(self.stop)
-        self._thread.start()
-
-    @property
-    def fps(self: Self) -> int:
-        return self._fps
-
-    @fps.setter
-    def fps(self: Self, fps: int) -> None:
-        self._fps = fps
-        self._delay_time = 1 / fps
-
-    def __call__(self: Self, frame: np.ndarray) -> None:
-        self._frame = frame
-
-    def __del__(self: Self) -> None:
-        self.stop()
-
-    def stop(self: Self) -> None:
-        self._stopped = True
-        with contextlib.suppress(RuntimeError):
-            self._thread.join()
-
-    def _run(self: Self) -> None:
-        while not self._stopped:
-            if self._frame is not None:
-                s = time.time()
-                cv2.imshow(self._name, self._frame)
-                self._frame = None
-                e = time.time()
-                cv2.waitKey(max(1, int((self._delay_time - (e - s)) * 1000)))
-            time.sleep(self._delay_time)
-        cv2.destroyWindow(self._name)
-
-
 class DisplayManager:
     """Used in the Camera class to display all the image streams."""
 
     def __init__(
         self: Self,
         fps: int = 30,
         display_size: tuple[int, int] = (640, 480),
@@ -103,15 +58,15 @@
         ----------
         fps : int, optional
             The fps of the display manager, by default 30
         display_size : Tuple[int, int], optional
             The size of the display, by default (640, 480)
 
         """
-        self._displays: dict[str, _Display] = {}
+        self._displays: dict[str, Display] = {}
         self._transforms: dict[str, Callable] = defaultdict(lambda: lambda x: x)
         self._display_size = display_size
         self._fps = fps
         atexit.register(self._stop)
 
     @property
     def fps(self: Self) -> int:
@@ -134,48 +89,54 @@
         Parameters
         ----------
         fps : int
             The fps to set the display manager to
 
         """
         self._fps = fps
-        for display in self._displays.values():
-            display.fps = fps
 
     def _stop(self: Self) -> None:
         for display in self._displays.values():
             display.stop()
 
     def stop(self: Self) -> None:
         """Use to stop the display manager."""
         self._stop()
 
     def _update(self: Self, name: str, frame: np.ndarray) -> None:
         if (
             frame.shape[1] != self._display_size[0]
             or frame.shape[0] != self._display_size[1]
         ):
-            frame = cv2.resize(frame, self._display_size)
+            frame = cv2.resize(
+                frame,
+                self._display_size,
+                interpolation=cv2.INTER_LINEAR,
+            )
         try:
             self._displays[name](frame)
         except KeyError:
-            self._displays[name] = _Display(name, self._fps)
+            self._displays[name] = Display(name, fps=self._fps)
             self._displays[name](frame)
 
-    def set_transform(self: Self, name: str, transform: Callable) -> None:
+    def set_transform(
+        self: Self,
+        name: str,
+        transform: Callable[[np.ndarray], np.ndarray],
+    ) -> None:
         """
         Use to set a transform for the given name.
 
         A transform should take in an np.ndarray and return an np.ndarray.
 
         Parameters
         ----------
         name : str
             The name of the transform
-        transform : Callable
+        transform : Callable[[np.ndarray], np.ndarray]
             The transform to set
 
         """
         self._transforms[name] = transform
 
     def update(
         self: Self,
```

### Comparing `oakutils-1.4.5/src/oakutils/tools/parsing.py` & `oakutils-1.5.0/src/oakutils/tools/parsing.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/pixel.py` & `oakutils-1.5.0/src/oakutils/tools/pixel.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/spatial.py` & `oakutils-1.5.0/src/oakutils/tools/spatial.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/tools/transform.py` & `oakutils-1.5.0/src/oakutils/tools/transform.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/vpu/__init__.py` & `oakutils-1.5.0/src/oakutils/vpu/__init__.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/vpu/_model_data.py` & `oakutils-1.5.0/src/oakutils/vpu/_model_data.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils/vpu/_vpu.py` & `oakutils-1.5.0/src/oakutils/vpu/_vpu.py`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils.egg-info/PKG-INFO` & `oakutils-1.5.0/src/oakutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakutils
-Version: 1.4.5
+Version: 1.5.0
 Author-email: Justin Davis <davisjustin302@gmail.com>
 Maintainer-email: Justin Davis <davisjustin302@gmail.com>
 Project-URL: Homepage, https://github.com/justincdavis/oakutils
 Project-URL: Bug Tracker, https://github.com/justincdavis/oakutils/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -35,18 +35,20 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Typing :: Typed
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: depthai>=2.24
 Requires-Dist: numpy<2.0,>=1.20
-Requires-Dist: open3d>=0.18.0
 Requires-Dist: opencv-contrib-python>=4.9.0
+Requires-Dist: cv2ext>=0.0.10
 Requires-Dist: typing_extensions>=4.9.0
 Requires-Dist: setuptools>=57.0.0
+Provides-Extra: o3d
+Requires-Dist: open3d>=0.18.0; extra == "o3d"
 Provides-Extra: compiler
 Requires-Dist: kornia>=0.6.0; extra == "compiler"
 Requires-Dist: torch>=1.9.0; extra == "compiler"
 Requires-Dist: onnx>=1.15.0; extra == "compiler"
 Requires-Dist: onnxruntime>=1.15.0; extra == "compiler"
 Requires-Dist: onnxsim>=0.4.33; extra == "compiler"
 Requires-Dist: blobconverter==1.4.3; extra == "compiler"
@@ -64,14 +66,15 @@
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.1.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: myst_parser>=1.0.0; extra == "docs"
 Provides-Extra: dev
+Requires-Dist: oakutils[o3d]; extra == "dev"
 Requires-Dist: oakutils[compiler]; extra == "dev"
 Requires-Dist: oakutils[ci]; extra == "dev"
 Requires-Dist: oakutils[test]; extra == "dev"
 Requires-Dist: oakutils[docs]; extra == "dev"
 Requires-Dist: twine>=4.0.0; extra == "dev"
 Requires-Dist: wheel>=0.37.0; extra == "dev"
 Requires-Dist: bumpver>=2023.1126; extra == "dev"
```

### Comparing `oakutils-1.4.5/src/oakutils.egg-info/SOURCES.txt` & `oakutils-1.5.0/src/oakutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oakutils-1.4.5/src/oakutils.egg-info/requires.txt` & `oakutils-1.5.0/src/oakutils.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 depthai>=2.24
 numpy<2.0,>=1.20
-open3d>=0.18.0
 opencv-contrib-python>=4.9.0
+cv2ext>=0.0.10
 typing_extensions>=4.9.0
 setuptools>=57.0.0
 
 [ci]
 pyupgrade>=3.10
 black>=24.0
 isort>=5.10
@@ -22,14 +22,15 @@
 onnxsim>=0.4.33
 blobconverter==1.4.3
 requests>=2.25.0
 boto3>=1.34.37
 botocore>=1.34.37
 
 [dev]
+oakutils[o3d]
 oakutils[compiler]
 oakutils[ci]
 oakutils[test]
 oakutils[docs]
 twine>=4.0.0
 wheel>=0.37.0
 bumpver>=2023.1126
@@ -37,9 +38,12 @@
 pyright>=1.1.348
 
 [docs]
 sphinx>=6.1.0
 sphinx-rtd-theme>=1.3.0
 myst_parser>=1.0.0
 
+[o3d]
+open3d>=0.18.0
+
 [test]
 pytest>=6.2.0
```

