# Comparing `tmp/Ais-cryoET-1.0.22.tar.gz` & `tmp/Ais-cryoET-1.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ais-cryoET-1.0.22.tar", last modified: Thu Mar 28 11:25:28 2024, max compression
+gzip compressed data, was "Ais-cryoET-1.0.23.tar", last modified: Thu Mar 28 11:32:11 2024, max compression
```

## Comparing `Ais-cryoET-1.0.22.tar` & `Ais-cryoET-1.0.23.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.460660 Ais-cryoET-1.0.22/
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:27.751045 Ais-cryoET-1.0.22/Ais/
--rw-rw-rw-   0        0        0    36025 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.030897 Ais-cryoET-1.0.22/Ais/core/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/__init__.py
--rw-rw-rw-   0        0        0     5069 2024-03-28 11:24:40.000000 Ais-cryoET-1.0.22/Ais/core/config.py
--rw-rw-rw-   0        0        0     1637 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.22/Ais/core/extract.py
--rw-rw-rw-   0        0        0     2640 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/open_in_blender.py
--rw-rw-rw-   0        0        0      625 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/open_in_chimerax.py
--rw-rw-rw-   0        0        0    17600 2023-12-13 11:43:47.000000 Ais-cryoET-1.0.22/Ais/core/opengl_classes.py
--rw-rw-rw-   0        0        0    33046 2024-02-08 12:56:17.000000 Ais-cryoET-1.0.22/Ais/core/se_frame.py
--rw-rw-rw-   0        0        0    24255 2024-03-26 11:05:39.000000 Ais-cryoET-1.0.22/Ais/core/se_model.py
--rw-rw-rw-   0        0        0   192280 2024-03-28 11:17:34.000000 Ais-cryoET-1.0.22/Ais/core/segmentation_editor.py
--rw-rw-rw-   0        0        0      331 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/settings.py
--rw-rw-rw-   0        0        0      130 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/settings.txt
--rw-rw-rw-   0        0        0       98 2024-01-02 10:33:08.000000 Ais-cryoET-1.0.22/Ais/core/start.py
--rw-rw-rw-   0        0        0    22298 2024-03-28 11:18:29.000000 Ais-cryoET-1.0.22/Ais/core/util.py
--rw-rw-rw-   0        0        0     2572 2023-12-21 15:04:18.000000 Ais-cryoET-1.0.22/Ais/core/widgets.py
--rw-rw-rw-   0        0        0     7894 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/core/window.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.090862 Ais-cryoET-1.0.22/Ais/icons/
--rw-rw-rw-   0        0        0  1098617 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_1024.png
--rw-rw-rw-   0        0        0    19430 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_128.png
--rw-rw-rw-   0        0        0  2960366 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_2048.png
--rw-rw-rw-   0        0        0   134990 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_256.png
--rw-rw-rw-   0        0        0   401274 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_512.png
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/__init__.py
--rw-rw-rw-   0        0        0     8843 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_blender_256.png
--rw-rw-rw-   0        0        0    30131 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_chimerax_256.png
--rw-rw-rw-   0        0        0     1563 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_close_256.png
--rw-rw-rw-   0        0        0      954 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_crop_256.png
--rw-rw-rw-   0        0        0     5113 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_obj_256.png
--rw-rw-rw-   0        0        0      784 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/icons/icon_stop_256.png
--rw-rw-rw-   0        0        0     2001 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.22/Ais/main.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.390702 Ais-cryoET-1.0.22/Ais/models/
--rw-rw-rw-   0        0        0       15 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/__init__.py
--rw-rw-rw-   0        0        0      819 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/eman2.py
--rw-rw-rw-   0        0        0     1359 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/inceptionnet.py
--rw-rw-rw-   0        0        0     2149 2024-02-06 08:17:58.000000 Ais-cryoET-1.0.22/Ais/models/model_template.py
--rw-rw-rw-   0        0        0     7759 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/pix2pix.py
--rw-rw-rw-   0        0        0     1562 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/resnet.py
--rw-rw-rw-   0        0        0     1166 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/unet_deep.py
--rw-rw-rw-   0        0        0      973 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/unet_dropout.py
--rw-rw-rw-   0        0        0      889 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/unet_lite.py
--rw-rw-rw-   0        0        0     1559 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/vggnet.py
--rw-rw-rw-   0        0        0     1568 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/models/vggnet_plus.py
--rw-rw-rw-   0        0        0      207 2024-01-02 08:48:52.000000 Ais-cryoET-1.0.22/Ais/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.440672 Ais-cryoET-1.0.22/Ais/shaders/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/__init__.py
--rw-rw-rw-   0        0        0      372 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/ce_line_shader.glsl
--rw-rw-rw-   0        0        0      725 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_binary_segmentation_shader.glsl
--rw-rw-rw-   0        0        0      424 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_border_shader.glsl
--rw-rw-rw-   0        0        0      929 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_compute_kernel_filter.glsl
--rw-rw-rw-   0        0        0      808 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_compute_mix.glsl
--rw-rw-rw-   0        0        0      487 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_depth_mask_shader.glsl
--rw-rw-rw-   0        0        0      696 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_float_segmentation_shader.glsl
--rw-rw-rw-   0        0        0      649 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_icon_shader.glsl
--rw-rw-rw-   0        0        0      286 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_line_3d_shader.glsl
--rw-rw-rw-   0        0        0      449 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_overlay_blend_shader.glsl
--rw-rw-rw-   0        0        0     3359 2023-11-30 12:28:22.000000 Ais-cryoET-1.0.22/Ais/shaders/se_overlay_ray_trace_shader.glsl
--rw-rw-rw-   0        0        0     1188 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_overlay_shader.glsl
--rw-rw-rw-   0        0        0      454 2024-01-02 13:56:12.000000 Ais-cryoET-1.0.22/Ais/shaders/se_particle_shader.glsl
--rw-rw-rw-   0        0        0      827 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_quad_3d_shader.glsl
--rw-rw-rw-   0        0        0     1019 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.22/Ais/shaders/se_quad_shader.glsl
--rw-rw-rw-   0        0        0     1950 2023-12-03 15:17:59.000000 Ais-cryoET-1.0.22/Ais/shaders/se_surface_model_shader.glsl
-drwxrwxrwx   0        0        0        0 2024-03-28 11:25:28.460660 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/
--rw-rw-rw-   0        0        0      328 2024-03-28 11:25:26.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1861 2024-03-28 11:25:27.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 11:25:26.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-03-28 11:25:26.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2024-03-28 11:25:26.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-28 11:25:26.000000 Ais-cryoET-1.0.22/Ais_cryoET.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-10-23 08:03:57.000000 Ais-cryoET-1.0.22/MANIFEST.in
--rw-rw-rw-   0        0        0      328 2024-03-28 11:25:28.460660 Ais-cryoET-1.0.22/PKG-INFO
--rw-rw-rw-   0        0        0     4706 2023-12-14 16:04:51.000000 Ais-cryoET-1.0.22/README.md
--rw-rw-rw-   0        0        0       42 2024-03-28 11:25:28.460660 Ais-cryoET-1.0.22/setup.cfg
--rw-rw-rw-   0        0        0     1218 2024-03-28 11:25:17.000000 Ais-cryoET-1.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.352032 Ais-cryoET-1.0.23/
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.128874 Ais-cryoET-1.0.23/Ais/
+-rw-rw-rw-   0        0        0    36025 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.195081 Ais-cryoET-1.0.23/Ais/core/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/__init__.py
+-rw-rw-rw-   0        0        0     5069 2024-03-28 11:32:03.000000 Ais-cryoET-1.0.23/Ais/core/config.py
+-rw-rw-rw-   0        0        0     1637 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.23/Ais/core/extract.py
+-rw-rw-rw-   0        0        0     2640 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/open_in_blender.py
+-rw-rw-rw-   0        0        0      625 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/open_in_chimerax.py
+-rw-rw-rw-   0        0        0    17600 2023-12-13 11:43:47.000000 Ais-cryoET-1.0.23/Ais/core/opengl_classes.py
+-rw-rw-rw-   0        0        0    33046 2024-02-08 12:56:17.000000 Ais-cryoET-1.0.23/Ais/core/se_frame.py
+-rw-rw-rw-   0        0        0    24255 2024-03-26 11:05:39.000000 Ais-cryoET-1.0.23/Ais/core/se_model.py
+-rw-rw-rw-   0        0        0   192280 2024-03-28 11:17:34.000000 Ais-cryoET-1.0.23/Ais/core/segmentation_editor.py
+-rw-rw-rw-   0        0        0      331 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/settings.py
+-rw-rw-rw-   0        0        0      130 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/settings.txt
+-rw-rw-rw-   0        0        0       98 2024-01-02 10:33:08.000000 Ais-cryoET-1.0.23/Ais/core/start.py
+-rw-rw-rw-   0        0        0    22298 2024-03-28 11:18:29.000000 Ais-cryoET-1.0.23/Ais/core/util.py
+-rw-rw-rw-   0        0        0     2572 2023-12-21 15:04:18.000000 Ais-cryoET-1.0.23/Ais/core/widgets.py
+-rw-rw-rw-   0        0        0     7894 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/window.py
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.239023 Ais-cryoET-1.0.23/Ais/icons/
+-rw-rw-rw-   0        0        0  1098617 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_1024.png
+-rw-rw-rw-   0        0        0    19430 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_128.png
+-rw-rw-rw-   0        0        0  2960366 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_2048.png
+-rw-rw-rw-   0        0        0   134990 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_256.png
+-rw-rw-rw-   0        0        0   401274 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_512.png
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/__init__.py
+-rw-rw-rw-   0        0        0     8843 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_blender_256.png
+-rw-rw-rw-   0        0        0    30131 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_chimerax_256.png
+-rw-rw-rw-   0        0        0     1563 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_close_256.png
+-rw-rw-rw-   0        0        0      954 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_crop_256.png
+-rw-rw-rw-   0        0        0     5113 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_obj_256.png
+-rw-rw-rw-   0        0        0      784 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_stop_256.png
+-rw-rw-rw-   0        0        0     2001 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.23/Ais/main.py
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.280130 Ais-cryoET-1.0.23/Ais/models/
+-rw-rw-rw-   0        0        0       15 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/eman2.py
+-rw-rw-rw-   0        0        0     1359 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/inceptionnet.py
+-rw-rw-rw-   0        0        0     2149 2024-02-06 08:17:58.000000 Ais-cryoET-1.0.23/Ais/models/model_template.py
+-rw-rw-rw-   0        0        0     7759 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/pix2pix.py
+-rw-rw-rw-   0        0        0     1562 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/resnet.py
+-rw-rw-rw-   0        0        0     1166 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_deep.py
+-rw-rw-rw-   0        0        0      973 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_dropout.py
+-rw-rw-rw-   0        0        0      889 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_lite.py
+-rw-rw-rw-   0        0        0     1559 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/vggnet.py
+-rw-rw-rw-   0        0        0     1568 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/vggnet_plus.py
+-rw-rw-rw-   0        0        0      207 2024-01-02 08:48:52.000000 Ais-cryoET-1.0.23/Ais/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.332069 Ais-cryoET-1.0.23/Ais/shaders/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/ce_line_shader.glsl
+-rw-rw-rw-   0        0        0      725 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_binary_segmentation_shader.glsl
+-rw-rw-rw-   0        0        0      424 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_border_shader.glsl
+-rw-rw-rw-   0        0        0      929 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_compute_kernel_filter.glsl
+-rw-rw-rw-   0        0        0      808 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_compute_mix.glsl
+-rw-rw-rw-   0        0        0      487 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_depth_mask_shader.glsl
+-rw-rw-rw-   0        0        0      696 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_float_segmentation_shader.glsl
+-rw-rw-rw-   0        0        0      649 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_icon_shader.glsl
+-rw-rw-rw-   0        0        0      286 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_line_3d_shader.glsl
+-rw-rw-rw-   0        0        0      449 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_blend_shader.glsl
+-rw-rw-rw-   0        0        0     3359 2023-11-30 12:28:22.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_ray_trace_shader.glsl
+-rw-rw-rw-   0        0        0     1188 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_shader.glsl
+-rw-rw-rw-   0        0        0      454 2024-01-02 13:56:12.000000 Ais-cryoET-1.0.23/Ais/shaders/se_particle_shader.glsl
+-rw-rw-rw-   0        0        0      827 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_quad_3d_shader.glsl
+-rw-rw-rw-   0        0        0     1019 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_quad_shader.glsl
+-rw-rw-rw-   0        0        0     1950 2023-12-03 15:17:59.000000 Ais-cryoET-1.0.23/Ais/shaders/se_surface_model_shader.glsl
+drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.348038 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/
+-rw-rw-rw-   0        0        0     5068 2024-03-28 11:32:10.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-28 11:32:10.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-10-23 08:03:57.000000 Ais-cryoET-1.0.23/MANIFEST.in
+-rw-rw-rw-   0        0        0     5068 2024-03-28 11:32:11.348038 Ais-cryoET-1.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     4706 2023-12-14 16:04:51.000000 Ais-cryoET-1.0.23/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-28 11:32:11.352032 Ais-cryoET-1.0.23/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2024-03-28 11:31:06.000000 Ais-cryoET-1.0.23/setup.py
```

### Comparing `Ais-cryoET-1.0.22/Ais/LICENSE.txt` & `Ais-cryoET-1.0.23/Ais/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/config.py` & `Ais-cryoET-1.0.23/Ais/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import platform
 
 # TODO: .tif files as input
 
 frozen = False
 root = os.path.dirname(os.path.dirname(__file__))
 app_name = "Ais"
-version = "1.0.22"
+version = "1.0.23"
 license = "GNU GPL v3"
 log_title = "Ais.log"
 log_path = os.path.join(root, log_title)
 
 filetype_segmentation = ".scns"
 filetype_traindata = ".scnt"
 filetype_semodel = ".scnm"
```

### Comparing `Ais-cryoET-1.0.22/Ais/core/extract.py` & `Ais-cryoET-1.0.23/Ais/core/extract.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/open_in_blender.py` & `Ais-cryoET-1.0.23/Ais/core/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/open_in_chimerax.py` & `Ais-cryoET-1.0.23/Ais/core/open_in_chimerax.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/opengl_classes.py` & `Ais-cryoET-1.0.23/Ais/core/opengl_classes.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/se_frame.py` & `Ais-cryoET-1.0.23/Ais/core/se_frame.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/se_model.py` & `Ais-cryoET-1.0.23/Ais/core/se_model.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/segmentation_editor.py` & `Ais-cryoET-1.0.23/Ais/core/segmentation_editor.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/util.py` & `Ais-cryoET-1.0.23/Ais/core/util.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/widgets.py` & `Ais-cryoET-1.0.23/Ais/core/widgets.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/core/window.py` & `Ais-cryoET-1.0.23/Ais/core/window.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_1024.png` & `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_1024.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_128.png` & `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_128.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_2048.png` & `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_2048.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_256.png` & `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/LOGO_Pom_512.png` & `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_512.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_blender_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_blender_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_chimerax_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_chimerax_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_close_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_close_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_crop_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_crop_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_obj_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_obj_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/icons/icon_stop_256.png` & `Ais-cryoET-1.0.23/Ais/icons/icon_stop_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/main.py` & `Ais-cryoET-1.0.23/Ais/main.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/eman2.py` & `Ais-cryoET-1.0.23/Ais/models/eman2.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/inceptionnet.py` & `Ais-cryoET-1.0.23/Ais/models/inceptionnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/model_template.py` & `Ais-cryoET-1.0.23/Ais/models/model_template.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/pix2pix.py` & `Ais-cryoET-1.0.23/Ais/models/pix2pix.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/resnet.py` & `Ais-cryoET-1.0.23/Ais/models/resnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/unet_deep.py` & `Ais-cryoET-1.0.23/Ais/models/unet_deep.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/unet_dropout.py` & `Ais-cryoET-1.0.23/Ais/models/unet_dropout.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/unet_lite.py` & `Ais-cryoET-1.0.23/Ais/models/unet_lite.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/vggnet.py` & `Ais-cryoET-1.0.23/Ais/models/vggnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/models/vggnet_plus.py` & `Ais-cryoET-1.0.23/Ais/models/vggnet_plus.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_binary_segmentation_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_binary_segmentation_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_compute_kernel_filter.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_compute_kernel_filter.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_compute_mix.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_compute_mix.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_float_segmentation_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_float_segmentation_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_icon_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_icon_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_overlay_ray_trace_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_overlay_ray_trace_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_overlay_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_overlay_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_quad_3d_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_quad_3d_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_quad_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_quad_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais/shaders/se_surface_model_shader.glsl` & `Ais-cryoET-1.0.23/Ais/shaders/se_surface_model_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/Ais_cryoET.egg-info/SOURCES.txt` & `Ais-cryoET-1.0.23/Ais_cryoET.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.22/README.md` & `Ais-cryoET-1.0.23/README.md`

 * *Files identical despite different names*

