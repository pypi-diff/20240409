# Comparing `tmp/pyuploadcare-5.0.1.tar.gz` & `tmp/pyuploadcare-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuploadcare-5.0.1.tar", max compression
+gzip compressed data, was "pyuploadcare-5.1.0.tar", max compression
```

## Comparing `pyuploadcare-5.0.1.tar` & `pyuploadcare-5.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1082 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/LICENSE
--rw-r--r--   0        0        0    10031 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/README.md
--rw-r--r--   0        0        0     2105 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyproject.toml
--rw-r--r--   0        0        0      439 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/__init__.py
--rw-r--r--   0        0        0      205 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/__init__.py
--rw-r--r--   0        0        0     3563 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/addon_entities.py
--rw-r--r--   0        0        0    19659 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/api.py
--rw-r--r--   0        0        0     2901 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/auth.py
--rw-r--r--   0        0        0     8405 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/base.py
--rw-r--r--   0        0        0     8818 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/client.py
--rw-r--r--   0        0        0     7515 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/entities.py
--rw-r--r--   0        0        0     1001 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/metadata.py
--rw-r--r--   0        0        0     2293 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/responses.py
--rw-r--r--   0        0        0      447 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/api/utils.py
--rw-r--r--   0        0        0    31115 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/client.py
--rw-r--r--   0        0        0      841 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/conf.py
--rw-r--r--   0        0        0      193 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/dj/__init__.py
--rw-r--r--   0        0        0      568 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/dj/client.py
--rw-r--r--   0        0        0     4605 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/dj/conf.py
--rw-r--r--   0        0        0     7002 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/dj/forms.py
--rw-r--r--   0        0        0     6211 2024-03-02 19:48:05.986126 pyuploadcare-5.0.1/pyuploadcare/dj/models.py
--rw-r--r--   0        0        0   211187 2024-03-02 19:48:05.990126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/blocks.min.js
--rw-r--r--   0        0        0    99732 2024-03-02 19:48:05.990126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-inline.min.css
--rw-r--r--   0        0        0    31029 2024-03-02 19:48:05.990126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-minimal.min.css
--rw-r--r--   0        0        0    99036 2024-03-02 19:48:05.990126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-regular.min.css
--rw-r--r--   0        0        0   384057 2024-03-02 19:48:05.990126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js
--rw-r--r--   0        0        0   296023 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/uploadcare.min.js
--rw-r--r--   0        0        0     2190 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/dj/subclassing.py
--rw-r--r--   0        0        0     1294 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/dj/templates/uploadcare/forms/widgets/file.html
--rw-r--r--   0        0        0     2224 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/exceptions.py
--rw-r--r--   0        0        0     1898 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/helpers.py
--rw-r--r--   0        0        0        0 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/__init__.py
--rw-r--r--   0        0        0     2861 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/base.py
--rw-r--r--   0        0        0    19846 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/file.py
--rw-r--r--   0        0        0     7094 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/file_group.py
--rw-r--r--   0        0        0     2241 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/file_list.py
--rw-r--r--   0        0        0     1400 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/group_list.py
--rw-r--r--   0        0        0      730 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/resources/utils.py
--rw-r--r--   0        0        0     5904 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/secure_url.py
--rw-r--r--   0        0        0        0 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/transformations/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/transformations/base.py
--rw-r--r--   0        0        0      729 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/transformations/document.py
--rw-r--r--   0        0        0    10674 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/transformations/image.py
--rw-r--r--   0        0        0     1648 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/transformations/video.py
--rwxr-xr-x   0        0        0        0 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/__init__.py
--rw-r--r--   0        0        0     1676 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/convert_document.py
--rw-r--r--   0        0        0     1048 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/convert_video.py
--rw-r--r--   0        0        0      539 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/create_group.py
--rw-r--r--   0        0        0     1034 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/create_webhook.py
--rw-r--r--   0        0        0      984 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/delete_files.py
--rw-r--r--   0        0        0      398 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/delete_webhook.py
--rw-r--r--   0        0        0      439 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/get_file.py
--rw-r--r--   0        0        0      461 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/get_project.py
--rw-r--r--   0        0        0     3255 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/helpers.py
--rw-r--r--   0        0        0     1406 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/list_files.py
--rw-r--r--   0        0        0      934 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/list_groups.py
--rw-r--r--   0        0        0      456 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/list_webhooks.py
--rw-r--r--   0        0        0     1186 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/store_files.py
--rw-r--r--   0        0        0     8801 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/sync.py
--rw-r--r--   0        0        0     1490 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/update_webhook.py
--rw-r--r--   0        0        0     1456 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/upload.py
--rw-r--r--   0        0        0     2987 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/upload_from_url.py
--rw-r--r--   0        0        0     3928 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/main.py
--rw-r--r--   0        0        0     2282 2024-03-02 19:48:05.994126 pyuploadcare-5.0.1/pyuploadcare/ucare_cli/settings.py
--rw-r--r--   0        0        0    11239 1970-01-01 00:00:00.000000 pyuploadcare-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/LICENSE
+-rw-r--r--   0        0        0    10031 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/README.md
+-rw-r--r--   0        0        0     2104 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0      439 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/__init__.py
+-rw-r--r--   0        0        0     3563 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/addon_entities.py
+-rw-r--r--   0        0        0    20206 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/api.py
+-rw-r--r--   0        0        0     2901 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/auth.py
+-rw-r--r--   0        0        0     8341 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/base.py
+-rw-r--r--   0        0        0     8818 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/client.py
+-rw-r--r--   0        0        0     7697 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/entities.py
+-rw-r--r--   0        0        0     1001 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/metadata.py
+-rw-r--r--   0        0        0     2289 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/responses.py
+-rw-r--r--   0        0        0      447 2024-04-09 12:31:45.849128 pyuploadcare-5.1.0/pyuploadcare/api/utils.py
+-rw-r--r--   0        0        0    31619 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/client.py
+-rw-r--r--   0        0        0      841 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/conf.py
+-rw-r--r--   0        0        0      193 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/__init__.py
+-rw-r--r--   0        0        0      568 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/client.py
+-rw-r--r--   0        0        0     4605 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/conf.py
+-rw-r--r--   0        0        0     7002 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/forms.py
+-rw-r--r--   0        0        0     6211 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/models.py
+-rw-r--r--   0        0        0   212189 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/blocks.min.js
+-rw-r--r--   0        0        0    99455 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-inline.min.css
+-rw-r--r--   0        0        0    30752 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-minimal.min.css
+-rw-r--r--   0        0        0    98759 2024-04-09 12:31:45.853128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-regular.min.css
+-rw-r--r--   0        0        0   384057 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js
+-rw-r--r--   0        0        0   296023 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js
+-rw-r--r--   0        0        0     2190 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/dj/subclassing.py
+-rw-r--r--   0        0        0     1304 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/dj/templates/uploadcare/forms/widgets/file.html
+-rw-r--r--   0        0        0     2224 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/exceptions.py
+-rw-r--r--   0        0        0     1898 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/__init__.py
+-rw-r--r--   0        0        0     2861 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/base.py
+-rw-r--r--   0        0        0    19999 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/file.py
+-rw-r--r--   0        0        0     7094 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/file_group.py
+-rw-r--r--   0        0        0     2241 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/file_list.py
+-rw-r--r--   0        0        0     1400 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/group_list.py
+-rw-r--r--   0        0        0      730 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/resources/utils.py
+-rw-r--r--   0        0        0     5904 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/secure_url.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/transformations/__init__.py
+-rw-r--r--   0        0        0     1605 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/transformations/base.py
+-rw-r--r--   0        0        0      729 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/transformations/document.py
+-rw-r--r--   0        0        0    19617 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/transformations/image.py
+-rw-r--r--   0        0        0     1648 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/transformations/video.py
+-rwxr-xr-x   0        0        0        0 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/convert_document.py
+-rw-r--r--   0        0        0     1048 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/convert_video.py
+-rw-r--r--   0        0        0      539 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/create_group.py
+-rw-r--r--   0        0        0     1034 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/create_webhook.py
+-rw-r--r--   0        0        0      984 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/delete_files.py
+-rw-r--r--   0        0        0      398 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/delete_webhook.py
+-rw-r--r--   0        0        0      439 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/get_file.py
+-rw-r--r--   0        0        0      461 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/get_project.py
+-rw-r--r--   0        0        0     3255 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/helpers.py
+-rw-r--r--   0        0        0     1406 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/list_files.py
+-rw-r--r--   0        0        0      934 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/list_groups.py
+-rw-r--r--   0        0        0      456 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/list_webhooks.py
+-rw-r--r--   0        0        0     1186 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/store_files.py
+-rw-r--r--   0        0        0     8801 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/sync.py
+-rw-r--r--   0        0        0     1490 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/update_webhook.py
+-rw-r--r--   0        0        0     1456 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/upload.py
+-rw-r--r--   0        0        0     2987 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/upload_from_url.py
+-rw-r--r--   0        0        0     3928 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/main.py
+-rw-r--r--   0        0        0     2282 2024-04-09 12:31:45.857128 pyuploadcare-5.1.0/pyuploadcare/ucare_cli/settings.py
+-rw-r--r--   0        0        0    11239 1970-01-01 00:00:00.000000 pyuploadcare-5.1.0/PKG-INFO
```

### Comparing `pyuploadcare-5.0.1/LICENSE` & `pyuploadcare-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/README.md` & `pyuploadcare-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyproject.toml` & `pyuploadcare-5.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyuploadcare"
-version = "5.0.1"
+version = "5.1.0"
 description = "Python library for Uploadcare.com"
 authors = ["Uploadcare Inc <hello@uploadcare.com>"]
 readme = "README.md"
 homepage = "https://uploadcare.com"
 repository = "https://github.com/uploadcare/pyuploadcare"
 classifiers = [
         'Development Status :: 5 - Production/Stable',
@@ -34,15 +34,15 @@
 Django = {version = ">=2.2", optional = true}
 
 [tool.poetry.extras]
 django = ["Django"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4"
-black = "^23.12.0"
+black = "^24.3.0"
 isort = "^5.13.2"
 flake8 = "^6.1.0"
 mypy = "^1.7.1"
 flake8-print = "^5.0.0"
 pytest-vcr = "^1.0.2"
 vcrpy = "^5.1.0"
 yarl = "^1.9.4"
@@ -59,15 +59,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
-target-version = ['py39']
+target-version = ['py38']
 exclude = '''
 (
   \.eggs
   |\.git
   |\.hg
   |\.mypy_cache
   |\.nox
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/addon_entities.py` & `pyuploadcare-5.1.0/pyuploadcare/api/addon_entities.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/api.py` & `pyuploadcare-5.1.0/pyuploadcare/api/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -513,17 +513,17 @@
         json_response = self._client.get(url).json()
         response = self._parse_response(json_response, response_class).root  # type: ignore
         return cast(str, response)
 
 
 class AddonsAPI(API):
     resource_type = "addons"
-    request_type: Type[
+    request_type: Type[AddonExecutionGeneralRequestData] = (
         AddonExecutionGeneralRequestData
-    ] = AddonExecutionGeneralRequestData
+    )
     response_classes = {
         "execute": responses.AddonExecuteResponse,
         "status": responses.AddonResponse,
     }
 
     def _get_request_data(
         self,
@@ -570,7 +570,23 @@
         query = dict(request_id=str(request_id))
         url = self._build_url(suffix=suffix, query_parameters=query)
         response_class = self._get_response_class("status")
 
         json_response = self._client.get(url).json()
         response = self._parse_response(json_response, response_class)
         return cast(responses.AddonResponse, response)
+
+
+class URLAPI(API):
+    resource_type = ""
+    response_classes = {
+        "detect_faces": entities.ImageInfoWithFaces,
+    }
+
+    def detect_faces(
+        self, file_uuid: Union[UUID, str]
+    ) -> entities.ImageInfoWithFaces:
+        url = self._build_url(file_uuid, suffix="detect_faces/")
+        response_class = self._get_response_class("detect_faces")
+        json_response = self._client.get(url).json()
+        response = self._parse_response(json_response, response_class)
+        return cast(entities.ImageInfoWithFaces, response)
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/auth.py` & `pyuploadcare-5.1.0/pyuploadcare/api/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from datetime import datetime, timezone
 from typing import Generator, Union
 
 from httpx import Auth, Request, Response
 from httpx._utils import to_bytes, to_str
 
 
-class AuthBase(Auth):
-    ...
+class AuthBase(Auth): ...
 
 
 class UploadcareSimpleAuth(AuthBase):
     def __init__(
         self,
         public_key: Union[str, bytes],
         secret_key: Union[str, bytes],
@@ -24,17 +23,17 @@
 
     def auth_flow(
         self, request: Request
     ) -> Generator[Request, Response, None]:
         if "Content-Type" not in request.headers:
             request.headers["Content-Type"] = "application/json"
 
-        request.headers[
-            "Accept"
-        ] = f"application/vnd.uploadcare-v{self.api_version}+json"
+        request.headers["Accept"] = (
+            f"application/vnd.uploadcare-v{self.api_version}+json"
+        )
         request.headers["Authorization"] = self._build_auth_header(
             request, self.public_key, self.secret_key
         )
         yield request
 
     def _build_auth_header(
         self,
@@ -52,17 +51,17 @@
         self, request: Request
     ) -> Generator[Request, Response, None]:
         formated_date_time = self._formated_date_time()
 
         if "Content-Type" not in request.headers:
             request.headers["Content-Type"] = "application/json"
 
-        request.headers[
-            "Accept"
-        ] = f"application/vnd.uploadcare-v{self.api_version}+json"
+        request.headers["Accept"] = (
+            f"application/vnd.uploadcare-v{self.api_version}+json"
+        )
         request.headers["Authorization"] = self._build_auth_header(
             request, self.public_key, self.secret_key, formated_date_time
         )
         request.headers["Date"] = formated_date_time
         yield request
 
     def _formated_date_time(self):
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/base.py` & `pyuploadcare-5.1.0/pyuploadcare/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,57 +114,49 @@
     response_classes: Dict[str, Union[Type[Response], Type[Entity]]]
     _client: Client
 
     def _parse_response(
         self,
         raw_resource: Dict[str, Any],
         response_class: Type[ResponseOrEntity],
-    ) -> ResponseOrEntity:
-        ...
+    ) -> ResponseOrEntity: ...
 
     def _build_url(
         self,
         resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None,
         base: Optional[str] = None,
         suffix: Optional[str] = None,
         query_parameters: Optional[Dict[str, Any]] = None,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     def _get_response_class(
         self, action: str
-    ) -> Union[Type[Response], Type[Entity]]:
-        ...
+    ) -> Union[Type[Response], Type[Entity]]: ...
 
-    def _post(self, data: Optional[Dict] = None) -> Dict[str, Any]:
-        ...
+    def _post(self, data: Optional[Dict] = None) -> Dict[str, Any]: ...
 
     def _get(
         self,
         resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None,
         **query_parameters,
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     def _put(
         self,
         resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None,
         data: Optional[Dict] = None,
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     def _delete(
         self, resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def _delete_with_response(
         self, resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
 
 class RetrieveMixin(APIProtocol):
     def retrieve(
         self,
         resource_uuid: Optional[Union[UUID, str, UUIDEntity]] = None,
         include_appdata: bool = False,
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/client.py` & `pyuploadcare-5.1.0/pyuploadcare/api/client.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/entities.py` & `pyuploadcare-5.1.0/pyuploadcare/api/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
 from uuid import UUID
 
 from pydantic import BaseModel, EmailStr, Field, PrivateAttr
-from typing_extensions import Annotated, Literal
+from typing_extensions import Annotated, Literal, NamedTuple
 
 from .metadata import META_KEY_MAX_LEN, META_KEY_PATTERN, META_VALUE_MAX_LEN
 
 
-class Entity(BaseModel):
-    ...
+class Entity(BaseModel): ...
 
 
 class IDEntity(Entity):
     id: UUID
 
 
 class UUIDEntity(Entity):
@@ -48,35 +47,46 @@
 
 
 class GEOPoint(Entity):
     latitude: float
     longitude: float
 
 
+class Face(NamedTuple):
+    x: int
+    y: int
+    width: int
+    height: int
+
+
 WebhookEvent = Literal[
     "file.uploaded",
     "file.infected",  # it will be deprecated in favor of info_upldated in the future updates
     "file.stored",
     "file.deleted",
     "file.info_updated",
 ]
 
 
 class ImageInfo(Entity):
-    color_mode: ColorMode
+    color_mode: Optional[ColorMode] = None
     orientation: Optional[int] = None
     format: str
-    sequence: bool
+    sequence: Optional[bool] = None
     height: int
     width: int
     geo_location: Optional[GEOPoint] = None
     datetime_original: Optional[datetime] = None
     dpi: Optional[Tuple[int, int]] = None
 
 
+class ImageInfoWithFaces(ImageInfo):
+    faces: List[Face]
+
+
 class AudioStreamInfo(Entity):
     bitrate: Optional[Decimal] = None
     codec: Optional[str] = None
     sample_rate: Optional[Decimal] = None
     profile: Optional[str] = None
     channels: Optional[int] = None
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/metadata.py` & `pyuploadcare-5.1.0/pyuploadcare/api/metadata.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/api/responses.py` & `pyuploadcare-5.1.0/pyuploadcare/api/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     FileInfo,
     GroupInfo,
     MetadataDict,
     VideoConvertInfo,
 )
 
 
-class Response(BaseModel):
-    ...
+class Response(BaseModel): ...
 
 
 class EntityListResponse(Response):
     results: List[Entity]
 
 
 class PaginatedResponse(EntityListResponse):
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/client.py` & `pyuploadcare-5.1.0/pyuploadcare/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     GroupsAPI,
     MetadataAPI,
     ProjectAPI,
     UploadAPI,
     VideoConvertAPI,
     WebhooksAPI,
 )
+from pyuploadcare.api.api import URLAPI
 from pyuploadcare.api.auth import UploadcareAuth
 from pyuploadcare.api.client import Client
 from pyuploadcare.api.entities import ProjectInfo, Webhook, WebhookEvent
 from pyuploadcare.exceptions import DuplicateFileError, InvalidParamError
 from pyuploadcare.helpers import (
     extracts_uuids,
     get_file_size,
@@ -146,14 +147,27 @@
             ),
             timeout=timeout,
             user_agent_extension=user_agent_extension,
             retry_throttled=retry_throttled,
             public_key=public_key,
         )
 
+        self.cdn_client = Client(
+            base_url=cdn_base,
+            verify=(
+                DEFAULT_SSL_CONTEXT
+                if verify_upload_ssl is True
+                else verify_upload_ssl
+            ),
+            timeout=timeout,
+            user_agent_extension=user_agent_extension,
+            retry_throttled=retry_throttled,
+            public_key=public_key,
+        )
+
         api_config = {
             "public_key": public_key,
             "secret_key": secret_key,
             "signed_uploads_ttl": signed_uploads_ttl,
         }
         self.upload_api = UploadAPI(client=self.upload_client, **api_config)  # type: ignore
         self.files_api = FilesAPI(client=self.rest_client, **api_config)  # type: ignore
@@ -164,14 +178,15 @@
         self.document_convert_api = DocumentConvertAPI(
             client=self.rest_client, **api_config  # type: ignore
         )
         self.webhooks_api = WebhooksAPI(client=self.rest_client, **api_config)  # type: ignore
         self.project_api = ProjectAPI(client=self.rest_client, **api_config)  # type: ignore
         self.metadata_api = MetadataAPI(client=self.rest_client, **api_config)  # type: ignore
         self.addons_api = AddonsAPI(client=self.rest_client, **api_config)  # type: ignore
+        self.url_api = URLAPI(client=self.cdn_client, **api_config)
 
     def file(
         self,
         cdn_url_or_file_id: Union[str, UUID],
         file_info: Optional[Dict[str, Any]] = None,
     ) -> File:
         """File resource for working with user-uploaded files.
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/conf.py` & `pyuploadcare-5.1.0/pyuploadcare/conf.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/client.py` & `pyuploadcare-5.1.0/pyuploadcare/dj/client.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/conf.py` & `pyuploadcare-5.1.0/pyuploadcare/dj/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     "secret": "",
     "cdn_base": None,
     "upload_base_url": None,
     "signed_uploads": False,
     "use_legacy_widget": False,
     "use_hosted_assets": True,
     "widget": {
-        "version": "0.33.2",
+        "version": "0.36.0",
         "variant": "regular",
         "build": "min",
         "options": {},
         "override_js_url": None,
         "override_css_url": {
             "regular": None,
             "inline": None,
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/forms.py` & `pyuploadcare-5.1.0/pyuploadcare/dj/forms.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/models.py` & `pyuploadcare-5.1.0/pyuploadcare/dj/models.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/blocks.min.js` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/blocks.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,44 +19,44 @@
  * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  * SOFTWARE.
  * 
  */
-var rn = Object.defineProperty;
-var nn = (s, i, t) => i in s ? rn(s, i, {
+var nn = Object.defineProperty;
+var on = (s, i, t) => i in s ? nn(s, i, {
     enumerable: !0,
     configurable: !0,
     writable: !0,
     value: t
 }) : s[i] = t;
-var h = (s, i, t) => (nn(s, typeof i != "symbol" ? i + "" : i, t), t);
-var on = Object.defineProperty,
-    ln = (s, i, t) => i in s ? on(s, i, {
+var h = (s, i, t) => (on(s, typeof i != "symbol" ? i + "" : i, t), t);
+var an = Object.defineProperty,
+    ln = (s, i, t) => i in s ? an(s, i, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: t
     }) : s[i] = t,
-    $i = (s, i, t) => (ln(s, typeof i != "symbol" ? i + "" : i, t), t);
+    Ii = (s, i, t) => (ln(s, typeof i != "symbol" ? i + "" : i, t), t);
 
-function an(s) {
+function cn(s) {
     let i = t => {
         var e;
         for (let r in t)((e = t[r]) == null ? void 0 : e.constructor) === Object && (t[r] = i(t[r]));
         return {
             ...t
         }
     };
     return i(s)
 }
 var E = class {
     constructor(s) {
-        s.constructor === Object ? this.store = an(s) : (this._storeIsProxy = !0, this.store = s), this.callbackMap = Object.create(null)
+        s.constructor === Object ? this.store = cn(s) : (this._storeIsProxy = !0, this.store = s), this.callbackMap = Object.create(null)
     }
     static warn(s, i) {
         console.warn(`Symbiote Data: cannot ${s}. Prop name: ` + i)
     }
     read(s) {
         return !this._storeIsProxy && !this.store.hasOwnProperty(s) ? (E.warn("read", s), null) : this.store[s]
     }
@@ -97,15 +97,15 @@
         E.globalStore.delete(s)
     }
     static getCtx(s, i = !0) {
         return E.globalStore.get(s) || (i && console.warn('State: wrong context UID - "' + s + '"'), null)
     }
 };
 E.globalStore = new Map;
-var C = Object.freeze({
+var v = Object.freeze({
         BIND_ATTR: "set",
         ATTR_BIND_PRFX: "@",
         EXT_DATA_CTX_PRFX: "*",
         NAMED_DATA_CTX_SPLTR: "/",
         CTX_NAME_ATTR: "ctx-name",
         CTX_OWNER_ATTR: "ctx-owner",
         CSS_CTX_PROP: "--ctx-name",
@@ -114,91 +114,91 @@
         REPEAT_ATTR: "repeat",
         REPEAT_ITEM_TAG_ATTR: "repeat-item-tag",
         SET_LATER_KEY: "__toSetLater__",
         USE_TPL: "use-template",
         ROOT_STYLE_ATTR_NAME: "sym-component"
     }),
     bs = "1234567890QWERTYUIOPASDFGHJKLZXCVBNMqwertyuiopasdfghjklzxcvbnm",
-    cn = bs.length - 1,
+    hn = bs.length - 1,
     Yt = class {
         static generate(s = "XXXXXXXXX-XXX") {
             let i = "";
-            for (let t = 0; t < s.length; t++) i += s[t] === "-" ? s[t] : bs.charAt(Math.random() * cn);
+            for (let t = 0; t < s.length; t++) i += s[t] === "-" ? s[t] : bs.charAt(Math.random() * hn);
             return i
         }
     };
 
 function ys(s, i, t) {
     let e = !0,
         r, n = i.split(".");
-    return n.forEach((o, l) => {
-        l < n.length - 1 ? s = s[o] : r = o
+    return n.forEach((o, a) => {
+        a < n.length - 1 ? s = s[o] : r = o
     }), s ? s[r] = t : e = !1, e
 }
 
-function hn(s) {
+function un(s) {
     return s.split("-").map((i, t) => i && t ? i[0].toUpperCase() + i.slice(1) : i).join("").split("_").map((i, t) => i && t ? i.toUpperCase() : i).join("")
 }
 
-function un(s, i) {
-    [...s.querySelectorAll(`[${C.REPEAT_ATTR}]`)].forEach(t => {
-        let e = t.getAttribute(C.REPEAT_ITEM_TAG_ATTR),
+function dn(s, i) {
+    [...s.querySelectorAll(`[${v.REPEAT_ATTR}]`)].forEach(t => {
+        let e = t.getAttribute(v.REPEAT_ITEM_TAG_ATTR),
             r;
         if (e && (r = window.customElements.get(e)), !r) {
             r = class extends i.BaseComponent {
                 constructor() {
                     super(), e || (this.style.display = "contents")
                 }
             };
             let o = t.innerHTML;
             r.template = o, r.reg(e)
         }
         for (; t.firstChild;) t.firstChild.remove();
-        let n = t.getAttribute(C.REPEAT_ATTR);
+        let n = t.getAttribute(v.REPEAT_ATTR);
         i.sub(n, o => {
             if (!o) {
                 for (; t.firstChild;) t.firstChild.remove();
                 return
             }
-            let l = [...t.children],
-                a, c = u => {
+            let a = [...t.children],
+                l, c = u => {
                     u.forEach((p, m) => {
-                        if (l[m])
-                            if (l[m].set$) setTimeout(() => {
-                                l[m].set$(p)
+                        if (a[m])
+                            if (a[m].set$) setTimeout(() => {
+                                a[m].set$(p)
                             });
                             else
-                                for (let f in p) l[m][f] = p[f];
+                                for (let f in p) a[m][f] = p[f];
                         else {
-                            a || (a = new DocumentFragment);
+                            l || (l = new DocumentFragment);
                             let f = new r;
-                            Object.assign(f.init$, p), a.appendChild(f)
+                            Object.assign(f.init$, p), l.appendChild(f)
                         }
-                    }), a && t.appendChild(a);
-                    let d = l.slice(u.length, l.length);
+                    }), l && t.appendChild(l);
+                    let d = a.slice(u.length, a.length);
                     for (let p of d) p.remove()
                 };
             if (o.constructor === Array) c(o);
             else if (o.constructor === Object) {
                 let u = [];
                 for (let d in o) {
                     let p = o[d];
                     Object.defineProperty(p, "_KEY_", {
                         value: d,
                         enumerable: !0
                     }), u.push(p)
                 }
                 c(u)
             } else console.warn("Symbiote repeat data type error:"), console.log(o)
-        }), t.removeAttribute(C.REPEAT_ATTR), t.removeAttribute(C.REPEAT_ITEM_TAG_ATTR)
+        }), t.removeAttribute(v.REPEAT_ATTR), t.removeAttribute(v.REPEAT_ITEM_TAG_ATTR)
     })
 }
 var gs = "__default__";
 
-function dn(s, i) {
+function pn(s, i) {
     if (i.shadowRoot) return;
     let t = [...s.querySelectorAll("slot")];
     if (!t.length) return;
     let e = {};
     t.forEach(r => {
         let n = r.getAttribute("name") || gs;
         e[n] = {
@@ -214,112 +214,112 @@
         else if (r.slot.childNodes.length) {
             let n = document.createDocumentFragment();
             n.append(...r.slot.childNodes), r.slot.parentNode.replaceChild(n, r.slot)
         } else r.slot.remove()
     })
 }
 
-function pn(s, i) {
-    [...s.querySelectorAll(`[${C.EL_REF_ATTR}]`)].forEach(t => {
-        let e = t.getAttribute(C.EL_REF_ATTR);
-        i.ref[e] = t, t.removeAttribute(C.EL_REF_ATTR)
+function fn(s, i) {
+    [...s.querySelectorAll(`[${v.EL_REF_ATTR}]`)].forEach(t => {
+        let e = t.getAttribute(v.EL_REF_ATTR);
+        i.ref[e] = t, t.removeAttribute(v.EL_REF_ATTR)
     })
 }
 
-function fn(s, i) {
-    [...s.querySelectorAll(`[${C.BIND_ATTR}]`)].forEach(t => {
-        let r = t.getAttribute(C.BIND_ATTR).split(";");
+function mn(s, i) {
+    [...s.querySelectorAll(`[${v.BIND_ATTR}]`)].forEach(t => {
+        let r = t.getAttribute(v.BIND_ATTR).split(";");
         [...t.attributes].forEach(n => {
             if (n.name.startsWith("-") && n.value) {
-                let o = hn(n.name.replace("-", ""));
+                let o = un(n.name.replace("-", ""));
                 r.push(o + ":" + n.value), t.removeAttribute(n.name)
             }
         }), r.forEach(n => {
             if (!n) return;
             let o = n.split(":").map(u => u.trim()),
-                l = o[0],
-                a;
-            l.indexOf(C.ATTR_BIND_PRFX) === 0 && (a = !0, l = l.replace(C.ATTR_BIND_PRFX, ""));
+                a = o[0],
+                l;
+            a.indexOf(v.ATTR_BIND_PRFX) === 0 && (l = !0, a = a.replace(v.ATTR_BIND_PRFX, ""));
             let c = o[1].split(",").map(u => u.trim());
             for (let u of c) {
                 let d;
                 u.startsWith("!!") ? (d = "double", u = u.replace("!!", "")) : u.startsWith("!") && (d = "single", u = u.replace("!", "")), i.sub(u, p => {
-                    d === "double" ? p = !!p : d === "single" && (p = !p), a ? (p == null ? void 0 : p.constructor) === Boolean ? p ? t.setAttribute(l, "") : t.removeAttribute(l) : t.setAttribute(l, p) : ys(t, l, p) || (t[C.SET_LATER_KEY] || (t[C.SET_LATER_KEY] = Object.create(null)), t[C.SET_LATER_KEY][l] = p)
+                    d === "double" ? p = !!p : d === "single" && (p = !p), l ? (p == null ? void 0 : p.constructor) === Boolean ? p ? t.setAttribute(a, "") : t.removeAttribute(a) : t.setAttribute(a, p) : ys(t, a, p) || (t[v.SET_LATER_KEY] || (t[v.SET_LATER_KEY] = Object.create(null)), t[v.SET_LATER_KEY][a] = p)
                 })
             }
-        }), t.removeAttribute(C.BIND_ATTR)
+        }), t.removeAttribute(v.BIND_ATTR)
     })
 }
-var xe = "{{",
+var Ae = "{{",
     Kt = "}}",
-    mn = "skip-text";
+    gn = "skip-text";
 
-function gn(s) {
+function _n(s) {
     let i, t = [],
         e = document.createTreeWalker(s, NodeFilter.SHOW_TEXT, {
             acceptNode: r => {
                 var n;
-                return !((n = r.parentElement) != null && n.hasAttribute(mn)) && r.textContent.includes(xe) && r.textContent.includes(Kt) && 1
+                return !((n = r.parentElement) != null && n.hasAttribute(gn)) && r.textContent.includes(Ae) && r.textContent.includes(Kt) && 1
             }
         });
     for (; i = e.nextNode();) t.push(i);
     return t
 }
-var _n = function(s, i) {
-        gn(s).forEach(e => {
+var bn = function(s, i) {
+        _n(s).forEach(e => {
             let r = [],
                 n;
-            for (; e.textContent.includes(Kt);) e.textContent.startsWith(xe) ? (n = e.textContent.indexOf(Kt) + Kt.length, e.splitText(n), r.push(e)) : (n = e.textContent.indexOf(xe), e.splitText(n)), e = e.nextSibling;
+            for (; e.textContent.includes(Kt);) e.textContent.startsWith(Ae) ? (n = e.textContent.indexOf(Kt) + Kt.length, e.splitText(n), r.push(e)) : (n = e.textContent.indexOf(Ae), e.splitText(n)), e = e.nextSibling;
             r.forEach(o => {
-                let l = o.textContent.replace(xe, "").replace(Kt, "");
-                o.textContent = "", i.sub(l, a => {
-                    o.textContent = a
+                let a = o.textContent.replace(Ae, "").replace(Kt, "");
+                o.textContent = "", i.sub(a, l => {
+                    o.textContent = l
                 })
             })
         })
     },
-    bn = [un, dn, pn, fn, _n],
-    Te = "'",
-    Nt = '"',
-    yn = /\\([0-9a-fA-F]{1,6} ?)/g;
-
-function vn(s) {
-    return (s[0] === Nt || s[0] === Te) && (s[s.length - 1] === Nt || s[s.length - 1] === Te)
-}
+    yn = [dn, pn, fn, mn, bn],
+    xe = "'",
+    Mt = '"',
+    vn = /\\([0-9a-fA-F]{1,6} ?)/g;
 
 function Cn(s) {
-    return (s[0] === Nt || s[0] === Te) && (s = s.slice(1)), (s[s.length - 1] === Nt || s[s.length - 1] === Te) && (s = s.slice(0, -1)), s
+    return (s[0] === Mt || s[0] === xe) && (s[s.length - 1] === Mt || s[s.length - 1] === xe)
 }
 
 function wn(s) {
+    return (s[0] === Mt || s[0] === xe) && (s = s.slice(1)), (s[s.length - 1] === Mt || s[s.length - 1] === xe) && (s = s.slice(0, -1)), s
+}
+
+function En(s) {
     let i = "",
         t = "";
     for (var e = 0; e < s.length; e++) {
         let r = s[e + 1];
         s[e] === "\\" && r === '"' ? (i += '\\"', e++) : s[e] === '"' && t !== "\\" ? i += '\\"' : i += s[e], t = s[e]
     }
     return i
 }
 
 function An(s) {
     let i = s;
-    vn(s) && (i = Cn(i), i = i.replace(yn, (t, e) => String.fromCodePoint(parseInt(e.trim(), 16))), i = i.replaceAll(`\\
-`, "\\n"), i = wn(i), i = Nt + i + Nt);
+    Cn(s) && (i = wn(i), i = i.replace(vn, (t, e) => String.fromCodePoint(parseInt(e.trim(), 16))), i = i.replaceAll(`\\
+`, "\\n"), i = En(i), i = Mt + i + Mt);
     try {
         return JSON.parse(i)
     } catch {
         throw new Error(`Failed to parse CSS property value: ${i}. Original input: ${s}`)
     }
 }
 var _s = 0,
-    Mt = null,
+    Rt = null,
     ct = null,
     gt = class extends HTMLElement {
         constructor() {
-            super(), $i(this, "updateCssData", () => {
+            super(), Ii(this, "updateCssData", () => {
                 var s;
                 this.dropCssDataCache(), (s = this.__boundCssProps) == null || s.forEach(i => {
                     let t = this.getCssData(this.__extractCssName(i), !0);
                     t !== null && this.$[i] !== t && (this.$[i] = t)
                 })
             }), this.init$ = Object.create(null), this.cssInit$ = Object.create(null), this.tplProcessors = new Set, this.ref = Object.create(null), this.allSubs = new Set, this.pauseRender = !1, this.renderShadow = !1, this.readyToDestroy = !0, this.processInnerHtml = !1, this.allowCustomTemplate = !1, this.ctxOwner = !1
         }
@@ -332,15 +332,15 @@
             this.__initialized || (this.__initialized = !0, (s = this.initCallback) == null || s.call(this))
         }
         render(s, i = this.renderShadow) {
             let t;
             if ((i || this.constructor.__shadowStylesUrl) && !this.shadowRoot && this.attachShadow({
                     mode: "open"
                 }), this.allowCustomTemplate) {
-                let r = this.getAttribute(C.USE_TPL);
+                let r = this.getAttribute(v.USE_TPL);
                 if (r) {
                     let n = this.getRootNode(),
                         o = (n == null ? void 0 : n.querySelector(r)) || document.querySelector(r);
                     o ? s = o.content.cloneNode(!0) : console.warn(`Symbiote template "${r}" is not found...`)
                 }
             }
             if (this.processInnerHtml)
@@ -362,35 +362,35 @@
                 r.rel = "stylesheet", r.href = this.constructor.__shadowStylesUrl, r.onload = e, this.shadowRoot.prepend(r)
             } else e()
         }
         addTemplateProcessor(s) {
             this.tplProcessors.add(s)
         }
         get autoCtxName() {
-            return this.__autoCtxName || (this.__autoCtxName = Yt.generate(), this.style.setProperty(C.CSS_CTX_PROP, `'${this.__autoCtxName}'`)), this.__autoCtxName
+            return this.__autoCtxName || (this.__autoCtxName = Yt.generate(), this.style.setProperty(v.CSS_CTX_PROP, `'${this.__autoCtxName}'`)), this.__autoCtxName
         }
         get cssCtxName() {
-            return this.getCssData(C.CSS_CTX_PROP, !0)
+            return this.getCssData(v.CSS_CTX_PROP, !0)
         }
         get ctxName() {
             var s;
-            let i = ((s = this.getAttribute(C.CTX_NAME_ATTR)) == null ? void 0 : s.trim()) || this.cssCtxName || this.__cachedCtxName || this.autoCtxName;
+            let i = ((s = this.getAttribute(v.CTX_NAME_ATTR)) == null ? void 0 : s.trim()) || this.cssCtxName || this.__cachedCtxName || this.autoCtxName;
             return this.__cachedCtxName = i, i
         }
         get localCtx() {
             return this.__localCtx || (this.__localCtx = E.registerCtx({}, this)), this.__localCtx
         }
         get nodeCtx() {
             return E.getCtx(this.ctxName, !1) || E.registerCtx({}, this.ctxName)
         }
         static __parseProp(s, i) {
             let t, e;
-            if (s.startsWith(C.EXT_DATA_CTX_PRFX)) t = i.nodeCtx, e = s.replace(C.EXT_DATA_CTX_PRFX, "");
-            else if (s.includes(C.NAMED_DATA_CTX_SPLTR)) {
-                let r = s.split(C.NAMED_DATA_CTX_SPLTR);
+            if (s.startsWith(v.EXT_DATA_CTX_PRFX)) t = i.nodeCtx, e = s.replace(v.EXT_DATA_CTX_PRFX, "");
+            else if (s.includes(v.NAMED_DATA_CTX_SPLTR)) {
+                let r = s.split(v.NAMED_DATA_CTX_SPLTR);
                 t = E.getCtx(r[0]), e = r[1]
             } else t = i.localCtx, e = s;
             return {
                 ctx: t,
                 name: e
             }
         }
@@ -437,73 +437,73 @@
         set$(s, i = !1) {
             for (let t in s) {
                 let e = s[t];
                 i || ![String, Number, Boolean].includes(e == null ? void 0 : e.constructor) ? this.$[t] = e : this.$[t] !== e && (this.$[t] = e)
             }
         }
         get __ctxOwner() {
-            return this.ctxOwner || this.hasAttribute(C.CTX_OWNER_ATTR) && this.getAttribute(C.CTX_OWNER_ATTR) !== "false"
+            return this.ctxOwner || this.hasAttribute(v.CTX_OWNER_ATTR) && this.getAttribute(v.CTX_OWNER_ATTR) !== "false"
         }
         __initDataCtx() {
             let s = this.constructor.__attrDesc;
             if (s)
                 for (let i of Object.values(s)) Object.keys(this.init$).includes(i) || (this.init$[i] = "");
             for (let i in this.init$)
-                if (i.startsWith(C.EXT_DATA_CTX_PRFX)) this.nodeCtx.add(i.replace(C.EXT_DATA_CTX_PRFX, ""), this.init$[i], this.__ctxOwner);
-                else if (i.includes(C.NAMED_DATA_CTX_SPLTR)) {
-                let t = i.split(C.NAMED_DATA_CTX_SPLTR),
+                if (i.startsWith(v.EXT_DATA_CTX_PRFX)) this.nodeCtx.add(i.replace(v.EXT_DATA_CTX_PRFX, ""), this.init$[i], this.__ctxOwner);
+                else if (i.includes(v.NAMED_DATA_CTX_SPLTR)) {
+                let t = i.split(v.NAMED_DATA_CTX_SPLTR),
                     e = t[0].trim(),
                     r = t[1].trim();
                 if (e && r) {
                     let n = E.getCtx(e, !1);
                     n || (n = E.registerCtx({}, e)), n.add(r, this.init$[i])
                 }
             } else this.localCtx.add(i, this.init$[i]);
             for (let i in this.cssInit$) this.bindCssData(i, this.cssInit$[i]);
             this.__dataCtxInitialized = !0
         }
         connectedCallback() {
             var s;
             if (this.isConnected) {
                 if (this.__disconnectTimeout && window.clearTimeout(this.__disconnectTimeout), !this.connectedOnce) {
-                    let i = (s = this.getAttribute(C.CTX_NAME_ATTR)) == null ? void 0 : s.trim();
-                    if (i && this.style.setProperty(C.CSS_CTX_PROP, `'${i}'`), this.__initDataCtx(), this[C.SET_LATER_KEY]) {
-                        for (let t in this[C.SET_LATER_KEY]) ys(this, t, this[C.SET_LATER_KEY][t]);
-                        delete this[C.SET_LATER_KEY]
+                    let i = (s = this.getAttribute(v.CTX_NAME_ATTR)) == null ? void 0 : s.trim();
+                    if (i && this.style.setProperty(v.CSS_CTX_PROP, `'${i}'`), this.__initDataCtx(), this[v.SET_LATER_KEY]) {
+                        for (let t in this[v.SET_LATER_KEY]) ys(this, t, this[v.SET_LATER_KEY][t]);
+                        delete this[v.SET_LATER_KEY]
                     }
                     this.initChildren = [...this.childNodes];
-                    for (let t of bn) this.addTemplateProcessor(t);
+                    for (let t of yn) this.addTemplateProcessor(t);
                     if (this.pauseRender) this.__initCallback();
                     else if (this.constructor.__rootStylesLink) {
                         let t = this.getRootNode();
                         if (!t) return;
-                        if (t == null ? void 0 : t.querySelector(`link[${C.ROOT_STYLE_ATTR_NAME}="${this.constructor.is}"]`)) {
+                        if (t == null ? void 0 : t.querySelector(`link[${v.ROOT_STYLE_ATTR_NAME}="${this.constructor.is}"]`)) {
                             this.render();
                             return
                         }
                         let r = this.constructor.__rootStylesLink.cloneNode(!0);
-                        r.setAttribute(C.ROOT_STYLE_ATTR_NAME, this.constructor.is), r.onload = () => {
+                        r.setAttribute(v.ROOT_STYLE_ATTR_NAME, this.constructor.is), r.onload = () => {
                             this.render()
                         }, t.nodeType === Node.DOCUMENT_NODE ? t.head.appendChild(r) : t.prepend(r)
                     } else this.render()
                 }
                 this.connectedOnce = !0
             }
         }
         destroyCallback() {}
         disconnectedCallback() {
             this.connectedOnce && (this.dropCssDataCache(), this.readyToDestroy && (this.__disconnectTimeout && window.clearTimeout(this.__disconnectTimeout), this.__disconnectTimeout = window.setTimeout(() => {
                 this.destroyCallback();
                 for (let s of this.allSubs) s.remove(), this.allSubs.delete(s);
                 for (let s of this.tplProcessors) this.tplProcessors.delete(s);
-                ct == null || ct.delete(this.updateCssData), ct != null && ct.size || (Mt == null || Mt.disconnect(), Mt = null, ct = null)
+                ct == null || ct.delete(this.updateCssData), ct != null && ct.size || (Rt == null || Rt.disconnect(), Rt = null, ct = null)
             }, 100)))
         }
         static reg(s, i = !1) {
-            s || (_s++, s = `${C.AUTO_TAG_PRFX}-${_s}`), this.__tag = s;
+            s || (_s++, s = `${v.AUTO_TAG_PRFX}-${_s}`), this.__tag = s;
             let t = window.customElements.get(s);
             if (t) {
                 !i && t !== this && console.warn([`Element with tag name "${s}" already registered.`, `You're trying to override it with another class "${this.name}".`, "This is most likely a mistake.", "New element will not be registered."].join(`
 `));
                 return
             }
             window.customElements.define(s, i ? class extends this {} : this)
@@ -532,19 +532,19 @@
             }
             return this.__cssDataCache[s]
         }
         __extractCssName(s) {
             return s.split("--").map((i, t) => t === 0 ? "" : i).join("--")
         }
         __initStyleAttrObserver() {
-            ct || (ct = new Set), ct.add(this.updateCssData), Mt || (Mt = new MutationObserver(s => {
+            ct || (ct = new Set), ct.add(this.updateCssData), Rt || (Rt = new MutationObserver(s => {
                 s[0].type === "attributes" && ct.forEach(i => {
                     i()
                 })
-            }), Mt.observe(document, {
+            }), Rt.observe(document, {
                 childList: !0,
                 subtree: !0,
                 attributes: !0,
                 attributeFilter: ["style"]
             }))
         }
         bindCssData(s, i = "") {
@@ -579,17 +579,17 @@
                     }),
                     t = URL.createObjectURL(i),
                     e = document.createElement("link");
                 e.href = t, e.rel = "stylesheet", this.__rootStylesLink = e
             }
         }
     },
-    Dt = gt;
-$i(Dt, "template");
-var Si = class {
+    Nt = gt;
+Ii(Nt, "template");
+var $i = class {
     static _print(s) {
         console.warn(s)
     }
     static setDefaultTitle(s) {
         this.defaultTitle = s
     }
     static setRoutingMap(s) {
@@ -627,15 +627,15 @@
         } else if (!i && this.defaultRoute) {
             this.applyRoute(this.defaultRoute);
             return
         } else if (!i) {
             this._print(`Route "${s.route}" not found...`);
             return
         }
-        let t = new CustomEvent(Si.routingEventName, {
+        let t = new CustomEvent($i.routingEventName, {
             detail: {
                 route: s.route,
                 options: Object.assign(i || {}, s.options)
             }
         });
         window.dispatchEvent(t)
     }
@@ -669,63 +669,63 @@
         return window.addEventListener(this.routingEventName, e => {
             var r;
             t.multiPub({
                 route: e.detail.route,
                 options: e.detail.options,
                 title: ((r = e.detail.options) == null ? void 0 : r.title) || this.defaultTitle || ""
             })
-        }), Si.notify(), this.initPopstateListener(), t
+        }), $i.notify(), this.initPopstateListener(), t
     }
     static initPopstateListener() {
         this.__onPopstate || (this.__onPopstate = () => {
             this.notify()
         }, window.addEventListener("popstate", this.__onPopstate))
     }
     static removePopstateListener() {
         window.removeEventListener("popstate", this.__onPopstate), this.__onPopstate = null
     }
 };
-Si.appMap = Object.create(null);
+$i.appMap = Object.create(null);
 
-function Ii(s, i) {
+function ki(s, i) {
     for (let t in i) t.includes("-") ? s.style.setProperty(t, i[t]) : s.style[t] = i[t]
 }
 
-function En(s, i) {
+function xn(s, i) {
     for (let t in i) i[t].constructor === Boolean ? i[t] ? s.setAttribute(t, "") : s.removeAttribute(t) : s.setAttribute(t, i[t])
 }
 
 function Jt(s = {
     tag: "div"
 }) {
     let i = document.createElement(s.tag);
-    if (s.attributes && En(i, s.attributes), s.styles && Ii(i, s.styles), s.properties)
+    if (s.attributes && xn(i, s.attributes), s.styles && ki(i, s.styles), s.properties)
         for (let t in s.properties) i[t] = s.properties[t];
     return s.processors && s.processors.forEach(t => {
         t(i)
     }), s.children && s.children.forEach(t => {
         let e = Jt(t);
         i.appendChild(e)
     }), i
 }
 var vs = "idb-store-ready",
-    xn = "symbiote-db",
-    Tn = "symbiote-idb-update_",
-    Sn = class {
+    Tn = "symbiote-db",
+    Sn = "symbiote-idb-update_",
+    $n = class {
         _notifyWhenReady(s = null) {
             window.dispatchEvent(new CustomEvent(vs, {
                 detail: {
                     dbName: this.name,
                     storeName: this.storeName,
                     event: s
                 }
             }))
         }
         get _updEventName() {
-            return Tn + this.name
+            return Sn + this.name
         }
         _getUpdateEvent(s) {
             return new CustomEvent(this._updEventName, {
                 detail: {
                     key: this.name,
                     newValue: s
                 }
@@ -766,19 +766,19 @@
         }
         write(s, i, t = !1) {
             let e = {
                     _key: s,
                     _value: i
                 },
                 n = this.db.transaction(this.storeName, "readwrite").objectStore(this.storeName).put(e);
-            return new Promise((o, l) => {
-                n.onsuccess = a => {
-                    t || this._notifySubscribers(s), o(a.target.result)
-                }, n.onerror = a => {
-                    l(a)
+            return new Promise((o, a) => {
+                n.onsuccess = l => {
+                    t || this._notifySubscribers(s), o(l.target.result)
+                }, n.onerror = l => {
+                    a(l)
                 }
             })
         }
         delete(s, i = !1) {
             let e = this.db.transaction(this.storeName, "readwrite").objectStore(this.storeName).delete(s);
             return new Promise((r, n) => {
                 e.onsuccess = o => {
@@ -812,24 +812,24 @@
             window.removeEventListener("storage", this._updateHandler), this._subscriptionsMap = null, Cs.clear(this.name)
         }
     },
     Cs = class {
         static get readyEventName() {
             return vs
         }
-        static open(s = xn, i = "store") {
+        static open(s = Tn, i = "store") {
             let t = s + "/" + i;
-            return this._reg[t] || (this._reg[t] = new Sn(s, i)), this._reg[t]
+            return this._reg[t] || (this._reg[t] = new $n(s, i)), this._reg[t]
         }
         static clear(s) {
             window.indexedDB.deleteDatabase(s);
             for (let i in this._reg) i.split("/")[0] === s && delete this._reg[i]
         }
     };
-$i(Cs, "_reg", Object.create(null));
+Ii(Cs, "_reg", Object.create(null));
 var $ = Object.freeze({
         FILE_ADDED: "file-added",
         FILE_REMOVED: "file-removed",
         FILE_UPLOAD_START: "file-upload-start",
         FILE_UPLOAD_PROGRESS: "file-upload-progress",
         FILE_UPLOAD_SUCCESS: "file-upload-success",
         FILE_UPLOAD_FAILED: "file-upload-failed",
@@ -842,15 +842,15 @@
         COMMON_UPLOAD_START: "common-upload-start",
         COMMON_UPLOAD_PROGRESS: "common-upload-progress",
         COMMON_UPLOAD_SUCCESS: "common-upload-success",
         COMMON_UPLOAD_FAILED: "common-upload-failed",
         CHANGE: "change",
         GROUP_CREATED: "group-created"
     }),
-    Se = class {
+    Te = class {
         constructor(i) {
             h(this, "_timeoutStore", new Map);
             h(this, "_targets", new Set);
             h(this, "_debugPrint", null);
             this._debugPrint = i
         }
         bindTarget(i) {
@@ -914,99 +914,99 @@
                 capture: !0
             }), document.documentElement.style.removeProperty(ws)
         }
     };
 h($t, "clientsRegistry", new Set), h($t, "flush", k(() => {
     document.documentElement.style.setProperty(ws, `${window.innerHeight}px`)
 }, 100));
-var $e = (s, i) => new Intl.PluralRules(s).select(i);
-var $n = s => s,
-    ki = "{{",
-    Es = "}}",
-    As = "plural:";
+var Se = (s, i) => new Intl.PluralRules(s).select(i);
+var In = s => s,
+    Oi = "{{",
+    As = "}}",
+    Es = "plural:";
 
 function Zt(s, i, t = {}) {
     var o;
     let {
-        openToken: e = ki,
-        closeToken: r = Es,
-        transform: n = $n
+        openToken: e = Oi,
+        closeToken: r = As,
+        transform: n = In
     } = t;
-    for (let l in i) {
-        let a = (o = i[l]) == null ? void 0 : o.toString();
-        s = s.replaceAll(e + l + r, typeof a == "string" ? n(a) : a)
+    for (let a in i) {
+        let l = (o = i[a]) == null ? void 0 : o.toString();
+        s = s.replaceAll(e + a + r, typeof l == "string" ? n(l) : l)
     }
     return s
 }
 
 function xs(s) {
     let i = [],
-        t = s.indexOf(ki);
+        t = s.indexOf(Oi);
     for (; t !== -1;) {
-        let e = s.indexOf(Es, t),
+        let e = s.indexOf(As, t),
             r = s.substring(t + 2, e);
-        if (r.startsWith(As)) {
-            let n = s.substring(t + 2, e).replace(As, ""),
+        if (r.startsWith(Es)) {
+            let n = s.substring(t + 2, e).replace(Es, ""),
                 o = n.substring(0, n.indexOf("(")),
-                l = n.substring(n.indexOf("(") + 1, n.indexOf(")"));
+                a = n.substring(n.indexOf("(") + 1, n.indexOf(")"));
             i.push({
                 variable: r,
                 pluralKey: o,
-                countVariable: l
+                countVariable: a
             })
         }
-        t = s.indexOf(ki, e)
+        t = s.indexOf(Oi, e)
     }
     return i
 }
 var ht = s => {
     var i;
     return (i = s.match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)) == null ? void 0 : i.map(t => t.toLowerCase()).join("-")
 };
-var Ie = ({
+var $e = ({
     element: s,
     attribute: i,
     onSuccess: t,
     onTimeout: e,
     timeout: r = 300
 }) => {
     let n = s.getAttribute(i);
     if (n !== null) {
         t(n);
         return
     }
     let o = new MutationObserver(c => {
         let u = c[c.length - 1];
-        a(u)
+        l(u)
     });
     o.observe(s, {
         attributes: !0,
         attributeFilter: [i]
     });
-    let l = setTimeout(() => {
+    let a = setTimeout(() => {
             o.disconnect(), e()
         }, r),
-        a = c => {
+        l = c => {
             let u = s.getAttribute(i);
-            c.type === "attributes" && c.attributeName === i && u !== null && (clearTimeout(l), o.disconnect(), t(u))
+            c.type === "attributes" && c.attributeName === i && u !== null && (clearTimeout(a), o.disconnect(), t(u))
         }
 };
 var Ts = new Set;
 
 function It(s) {
     Ts.has(s) || (Ts.add(s), console.warn(s))
 }
 
 function Ss(s) {
     return Object.prototype.toString.call(s) === "[object Object]"
 }
-var In = /\W|_/g;
+var kn = /\W|_/g;
 
-function kn(s) {
-    return s.split(In).map((i, t) => i.charAt(0)[t > 0 ? "toUpperCase" : "toLowerCase"]() + i.slice(1)).join("")
+function On(s) {
+    return s.split(kn).map((i, t) => i.charAt(0)[t > 0 ? "toUpperCase" : "toLowerCase"]() + i.slice(1)).join("")
 }
 
 function $s(s, {
     ignoreKeys: i
 } = {
     ignoreKeys: []
 }) {
@@ -1031,21 +1031,21 @@
             t[e] = r;
             continue
         }
         Ss(r) ? r = pt(r, {
             ignoreKeys: i
         }) : Array.isArray(r) && (r = $s(r, {
             ignoreKeys: i
-        })), t[kn(e)] = r
+        })), t[On(e)] = r
     }
     return t
 }
-var On = s => new Promise(i => setTimeout(i, s));
+var Pn = s => new Promise(i => setTimeout(i, s));
 
-function Ni({
+function Di({
     libraryName: s,
     libraryVersion: i,
     userAgent: t,
     publicKey: e = "",
     integration: r = ""
 }) {
     let n = "JavaScript";
@@ -1054,284 +1054,284 @@
         publicKey: e,
         libraryName: s,
         libraryVersion: i,
         languageName: n,
         integration: r
     });
     let o = [s, i, e].filter(Boolean).join("/"),
-        l = [n, r].filter(Boolean).join("; ");
-    return `${o} (${l})`
+        a = [n, r].filter(Boolean).join("; ");
+    return `${o} (${a})`
 }
-var Pn = {
+var Ln = {
     factor: 2,
     time: 100
 };
 
-function Ln(s, i = Pn) {
+function Un(s, i = Ln) {
     let t = 0;
 
     function e(r) {
         let n = Math.round(i.time * i.factor ** t);
         return r({
             attempt: t,
-            retry: l => On(l != null ? l : n).then(() => (t += 1, e(r)))
+            retry: a => Pn(a != null ? a : n).then(() => (t += 1, e(r)))
         })
     }
     return e(s)
 }
 var Qt = class extends Error {},
-    Ft = class s extends Qt {
+    Dt = class s extends Qt {
         constructor(t) {
             super();
             h(this, "originalProgressEvent");
             this.name = "NetworkError", this.message = "Network error", Object.setPrototypeOf(this, s.prototype), this.originalProgressEvent = t
         }
     },
-    Oe = (s, i) => {
+    ke = (s, i) => {
         s && (s.aborted ? Promise.resolve().then(i) : s.addEventListener("abort", () => i(), {
             once: !0
         }))
     },
     _t = class s extends Qt {
         constructor(t = "Request canceled") {
             super(t);
             h(this, "isCancel", !0);
             this.name = "CancelError", Object.setPrototypeOf(this, s.prototype)
         }
     },
-    Un = 500,
+    Rn = 500,
     ks = ({
         check: s,
-        interval: i = Un,
+        interval: i = Rn,
         timeout: t,
         signal: e
     }) => new Promise((r, n) => {
-        let o, l;
-        Oe(e, () => {
+        let o, a;
+        ke(e, () => {
             o && clearTimeout(o), n(new _t("Poll cancelled"))
-        }), t && (l = setTimeout(() => {
+        }), t && (a = setTimeout(() => {
             o && clearTimeout(o), n(new _t("Timed out"))
         }, t));
-        let a = () => {
+        let l = () => {
             try {
                 Promise.resolve(s(e)).then(c => {
-                    c ? (l && clearTimeout(l), r(c)) : o = setTimeout(a, i)
+                    c ? (a && clearTimeout(a), r(c)) : o = setTimeout(l, i)
                 }).catch(c => {
-                    l && clearTimeout(l), n(c)
+                    a && clearTimeout(a), n(c)
                 })
             } catch (c) {
-                l && clearTimeout(l), n(c)
+                a && clearTimeout(a), n(c)
             }
         };
-        o = setTimeout(a, 0)
+        o = setTimeout(l, 0)
     }),
     S = {
         baseCDN: "https://ucarecdn.com",
         baseURL: "https://upload.uploadcare.com",
         maxContentLength: 50 * 1024 * 1024,
         retryThrottledRequestMaxTimes: 1,
         retryNetworkErrorMaxTimes: 3,
         multipartMinFileSize: 25 * 1024 * 1024,
         multipartChunkSize: 5 * 1024 * 1024,
         multipartMinLastPartSize: 1024 * 1024,
         maxConcurrentRequests: 4,
         pollingTimeoutMilliseconds: 1e4,
         pusherKey: "79ae88bd931ea68464d9"
     },
-    Pe = "application/octet-stream",
+    Oe = "application/octet-stream",
     Os = "original",
     bt = ({
         method: s,
         url: i,
         data: t,
         headers: e = {},
         signal: r,
         onProgress: n
-    }) => new Promise((o, l) => {
-        let a = new XMLHttpRequest,
+    }) => new Promise((o, a) => {
+        let l = new XMLHttpRequest,
             c = (s == null ? void 0 : s.toUpperCase()) || "GET",
             u = !1;
-        a.open(c, i, !0), e && Object.entries(e).forEach(d => {
+        l.open(c, i, !0), e && Object.entries(e).forEach(d => {
             let [p, m] = d;
-            typeof m != "undefined" && !Array.isArray(m) && a.setRequestHeader(p, m)
-        }), a.responseType = "text", Oe(r, () => {
-            u = !0, a.abort(), l(new _t)
-        }), a.onload = () => {
-            if (a.status != 200) l(new Error(`Error ${a.status}: ${a.statusText}`));
+            typeof m != "undefined" && !Array.isArray(m) && l.setRequestHeader(p, m)
+        }), l.responseType = "text", ke(r, () => {
+            u = !0, l.abort(), a(new _t)
+        }), l.onload = () => {
+            if (l.status != 200) a(new Error(`Error ${l.status}: ${l.statusText}`));
             else {
                 let d = {
                         method: c,
                         url: i,
                         data: t,
                         headers: e || void 0,
                         signal: r,
                         onProgress: n
                     },
-                    p = a.getAllResponseHeaders().trim().split(/[\r\n]+/),
+                    p = l.getAllResponseHeaders().trim().split(/[\r\n]+/),
                     m = {};
-                p.forEach(function(b) {
-                    let x = b.split(": "),
-                        v = x.shift(),
-                        A = x.join(": ");
-                    v && typeof v != "undefined" && (m[v] = A)
+                p.forEach(function(y) {
+                    let x = y.split(": "),
+                        T = x.shift(),
+                        w = x.join(": ");
+                    T && typeof T != "undefined" && (m[T] = w)
                 });
-                let f = a.response,
-                    _ = a.status;
+                let f = l.response,
+                    _ = l.status;
                 o({
                     request: d,
                     data: f,
                     headers: m,
                     status: _
                 })
             }
-        }, a.onerror = d => {
-            u || l(new Ft(d))
-        }, n && typeof n == "function" && (a.upload.onprogress = d => {
+        }, l.onerror = d => {
+            u || a(new Dt(d))
+        }, n && typeof n == "function" && (l.upload.onprogress = d => {
             d.lengthComputable ? n({
                 isComputable: !0,
                 value: d.loaded / d.total
             }) : n({
                 isComputable: !1
             })
-        }), t ? a.send(t) : a.send()
+        }), t ? l.send(t) : l.send()
     });
 
-function Rn(s, ...i) {
+function Mn(s, ...i) {
     return s
 }
-var Mn = ({
+var Nn = ({
         name: s
     }) => s ? [s] : [],
-    Nn = Rn,
-    Dn = () => new FormData,
+    Dn = Mn,
+    Fn = () => new FormData,
     Ps = s => !1,
-    Le = s => typeof Blob != "undefined" && s instanceof Blob,
-    Ue = s => typeof File != "undefined" && s instanceof File,
-    Re = s => !!s && typeof s == "object" && !Array.isArray(s) && "uri" in s && typeof s.uri == "string",
-    Bt = s => Le(s) || Ue(s) || Ps() || Re(s),
-    Fn = s => typeof s == "string" || typeof s == "number" || typeof s == "undefined",
-    Bn = s => !!s && typeof s == "object" && !Array.isArray(s),
-    zn = s => !!s && typeof s == "object" && "data" in s && Bt(s.data);
+    Pe = s => typeof Blob != "undefined" && s instanceof Blob,
+    Le = s => typeof File != "undefined" && s instanceof File,
+    Ue = s => !!s && typeof s == "object" && !Array.isArray(s) && "uri" in s && typeof s.uri == "string",
+    Ft = s => Pe(s) || Le(s) || Ps() || Ue(s),
+    Bn = s => typeof s == "string" || typeof s == "number" || typeof s == "undefined",
+    zn = s => !!s && typeof s == "object" && !Array.isArray(s),
+    Vn = s => !!s && typeof s == "object" && "data" in s && Ft(s.data);
 
 function Ls(s, i, t) {
     if (Array.isArray(t))
         for (let e of t) Ls(s, `${i}[]`, e);
-    else if (zn(t)) {
+    else if (Vn(t)) {
         let {
             name: e,
             contentType: r
-        } = t, n = Nn(t.data, e, r != null ? r : Pe), o = Mn({
+        } = t, n = Dn(t.data, e, r != null ? r : Oe), o = Nn({
             name: e,
             contentType: r
         });
         s.push([i, n, ...o])
-    } else if (Bn(t))
+    } else if (zn(t))
         for (let [e, r] of Object.entries(t)) typeof r != "undefined" && s.push([`${i}[${e}]`, String(r)]);
-    else Fn(t) && t && s.push([i, t.toString()])
+    else Bn(t) && t && s.push([i, t.toString()])
 }
 
-function Vn(s) {
+function jn(s) {
     let i = [];
     for (let [t, e] of Object.entries(s)) Ls(i, t, e);
     return i
 }
 
-function Me(s) {
-    let i = Dn(),
-        t = Vn(s);
+function Re(s) {
+    let i = Fn(),
+        t = jn(s);
     for (let e of t) {
         let [r, n, ...o] = e;
         i.append(r, n, ...o)
     }
     return i
 }
-var D = class s extends Qt {
+var F = class s extends Qt {
         constructor(t, e, r, n, o) {
             super();
             h(this, "code");
             h(this, "request");
             h(this, "response");
             h(this, "headers");
             this.name = "UploadError", this.message = t, this.code = e, this.request = r, this.response = n, this.headers = o, Object.setPrototypeOf(this, s.prototype)
         }
     },
-    jn = s => {
+    Hn = s => {
         let i = new URLSearchParams;
         for (let [t, e] of Object.entries(s)) e && typeof e == "object" && !Array.isArray(e) ? Object.entries(e).filter(r => {
             var n;
             return (n = r[1]) != null ? n : !1
         }).forEach(r => i.set(`${t}[${r[0]}]`, String(r[1]))) : Array.isArray(e) ? e.forEach(r => {
             i.append(`${t}[]`, r)
         }) : typeof e == "string" && e ? i.set(t, e) : typeof e == "number" && i.set(t, e.toString());
         return i.toString()
     },
     ut = (s, i, t) => {
         let e = new URL(s);
-        return e.pathname = (e.pathname + i).replace("//", "/"), t && (e.search = jn(t)), e.toString()
+        return e.pathname = (e.pathname + i).replace("//", "/"), t && (e.search = Hn(t)), e.toString()
     },
-    Hn = "6.13.0",
-    Gn = "UploadcareUploadClient",
-    Wn = Hn;
+    Gn = "6.14.1",
+    Wn = "UploadcareUploadClient",
+    Xn = Gn;
 
 function kt(s) {
-    return Ni({
-        libraryName: Gn,
-        libraryVersion: Wn,
+    return Di({
+        libraryName: Wn,
+        libraryVersion: Xn,
         ...s
     })
 }
-var Xn = "RequestThrottledError",
+var qn = "RequestThrottledError",
     Is = 15e3,
-    qn = 1e3;
+    Kn = 1e3;
 
-function Kn(s) {
+function Yn(s) {
     let {
         headers: i
     } = s || {};
     if (!i || typeof i["retry-after"] != "string") return Is;
     let t = parseInt(i["retry-after"], 10);
     return Number.isFinite(t) ? t * 1e3 : Is
 }
 
 function yt(s, i) {
     let {
         retryThrottledRequestMaxTimes: t,
         retryNetworkErrorMaxTimes: e
     } = i;
-    return Ln(({
+    return Un(({
         attempt: r,
         retry: n
     }) => s().catch(o => {
-        if ("response" in o && (o == null ? void 0 : o.code) === Xn && r < t) return n(Kn(o));
-        if (o instanceof Ft && r < e) return n((r + 1) * qn);
+        if ("response" in o && (o == null ? void 0 : o.code) === qn && r < t) return n(Yn(o));
+        if (o instanceof Dt && r < e) return n((r + 1) * Kn);
         throw o
     }))
 }
 var Us = s => {
         let i = "";
-        return (Le(s) || Ue(s) || Re(s)) && (i = s.type), i || Pe
+        return (Pe(s) || Le(s) || Ue(s)) && (i = s.type), i || Oe
     },
     Rs = s => {
         let i = "";
-        return Ue(s) && s.name ? i = s.name : Le(s) || Ps() ? i = "" : Re(s) && s.name && (i = s.name), i || Os
+        return Le(s) && s.name ? i = s.name : Pe(s) || Ps() ? i = "" : Ue(s) && s.name && (i = s.name), i || Os
     };
 
-function Di(s) {
+function Fi(s) {
     return typeof s == "undefined" || s === "auto" ? "auto" : s ? "1" : "0"
 }
 
-function Yn(s, {
+function Jn(s, {
     publicKey: i,
     fileName: t,
     contentType: e,
     baseURL: r = S.baseURL,
     secureSignature: n,
     secureExpire: o,
-    store: l,
-    signal: a,
+    store: a,
+    signal: l,
     onProgress: c,
     source: u = "local",
     integration: d,
     userAgent: p,
     retryThrottledRequestMaxTimes: m = S.retryThrottledRequestMaxTimes,
     retryNetworkErrorMaxTimes: f = S.retryNetworkErrorMaxTimes,
     metadata: _
@@ -1344,56 +1344,56 @@
         headers: {
             "X-UC-User-Agent": kt({
                 publicKey: i,
                 integration: d,
                 userAgent: p
             })
         },
-        data: Me({
+        data: Re({
             file: {
                 data: s,
                 name: t || Rs(s),
                 contentType: e || Us(s)
             },
             UPLOADCARE_PUB_KEY: i,
-            UPLOADCARE_STORE: Di(l),
+            UPLOADCARE_STORE: Fi(a),
             signature: n,
             expire: o,
             source: u,
             metadata: _
         }),
-        signal: a,
+        signal: l,
         onProgress: c
     }).then(({
-        data: b,
+        data: y,
         headers: x,
-        request: v
+        request: T
     }) => {
-        let A = pt(JSON.parse(b));
-        if ("error" in A) throw new D(A.error.content, A.error.errorCode, v, A, x);
-        return A
+        let w = pt(JSON.parse(y));
+        if ("error" in w) throw new F(w.error.content, w.error.errorCode, T, w, x);
+        return w
     }), {
         retryNetworkErrorMaxTimes: f,
         retryThrottledRequestMaxTimes: m
     })
 }
-var Li;
+var Ui;
 (function(s) {
     s.Token = "token", s.FileInfo = "file_info"
-})(Li || (Li = {}));
+})(Ui || (Ui = {}));
 
-function Jn(s, {
+function Zn(s, {
     publicKey: i,
     baseURL: t = S.baseURL,
     store: e,
     fileName: r,
     checkForUrlDuplicates: n,
     saveUrlForRecurrentUploads: o,
-    secureSignature: l,
-    secureExpire: a,
+    secureSignature: a,
+    secureExpire: l,
     source: c = "url",
     signal: u,
     integration: d,
     userAgent: p,
     retryThrottledRequestMaxTimes: m = S.retryThrottledRequestMaxTimes,
     retryNetworkErrorMaxTimes: f = S.retryNetworkErrorMaxTimes,
     metadata: _
@@ -1407,51 +1407,51 @@
                 userAgent: p
             })
         },
         url: ut(t, "/from_url/", {
             jsonerrors: 1,
             pub_key: i,
             source_url: s,
-            store: Di(e),
+            store: Fi(e),
             filename: r,
             check_URL_duplicates: n ? 1 : void 0,
             save_URL_duplicates: o ? 1 : void 0,
-            signature: l,
-            expire: a,
+            signature: a,
+            expire: l,
             source: c,
             metadata: _
         }),
         signal: u
     }).then(({
-        data: b,
+        data: y,
         headers: x,
-        request: v
+        request: T
     }) => {
-        let A = pt(JSON.parse(b));
-        if ("error" in A) throw new D(A.error.content, A.error.errorCode, v, A, x);
-        return A
+        let w = pt(JSON.parse(y));
+        if ("error" in w) throw new F(w.error.content, w.error.errorCode, T, w, x);
+        return w
     }), {
         retryNetworkErrorMaxTimes: f,
         retryThrottledRequestMaxTimes: m
     })
 }
 var H;
 (function(s) {
     s.Unknown = "unknown", s.Waiting = "waiting", s.Progress = "progress", s.Error = "error", s.Success = "success"
 })(H || (H = {}));
-var Zn = s => "status" in s && s.status === H.Error;
+var Qn = s => "status" in s && s.status === H.Error;
 
-function Qn(s, {
+function to(s, {
     publicKey: i,
     baseURL: t = S.baseURL,
     signal: e,
     integration: r,
     userAgent: n,
     retryThrottledRequestMaxTimes: o = S.retryThrottledRequestMaxTimes,
-    retryNetworkErrorMaxTimes: l = S.retryNetworkErrorMaxTimes
+    retryNetworkErrorMaxTimes: a = S.retryNetworkErrorMaxTimes
 } = {}) {
     return yt(() => bt({
         method: "GET",
         headers: i ? {
             "X-UC-User-Agent": kt({
                 publicKey: i,
                 integration: r,
@@ -1460,84 +1460,84 @@
         } : void 0,
         url: ut(t, "/from_url/status/", {
             jsonerrors: 1,
             token: s
         }),
         signal: e
     }).then(({
-        data: a,
+        data: l,
         headers: c,
         request: u
     }) => {
-        let d = pt(JSON.parse(a));
-        if ("error" in d && !Zn(d)) throw new D(d.error.content, d.error.errorCode, u, d, c);
+        let d = pt(JSON.parse(l));
+        if ("error" in d && !Qn(d)) throw new F(d.error.content, d.error.errorCode, u, d, c);
         return d
     }), {
-        retryNetworkErrorMaxTimes: l,
+        retryNetworkErrorMaxTimes: a,
         retryThrottledRequestMaxTimes: o
     })
 }
 
-function to(s, {
+function eo(s, {
     publicKey: i,
     baseURL: t = S.baseURL,
     jsonpCallback: e,
     secureSignature: r,
     secureExpire: n,
     signal: o,
-    source: l,
-    integration: a,
+    source: a,
+    integration: l,
     userAgent: c,
     retryThrottledRequestMaxTimes: u = S.retryThrottledRequestMaxTimes,
     retryNetworkErrorMaxTimes: d = S.retryNetworkErrorMaxTimes
 }) {
     return yt(() => bt({
         method: "POST",
         headers: {
             "X-UC-User-Agent": kt({
                 publicKey: i,
-                integration: a,
+                integration: l,
                 userAgent: c
             })
         },
         url: ut(t, "/group/", {
             jsonerrors: 1
         }),
-        data: Me({
+        data: Re({
             files: s,
             callback: e,
             pub_key: i,
             signature: r,
             expire: n,
-            source: l
+            source: a
         }),
         signal: o
     }).then(({
         data: p,
         headers: m,
         request: f
     }) => {
         let _ = pt(JSON.parse(p));
-        if ("error" in _) throw new D(_.error.content, _.error.errorCode, f, _, m);
+        if ("error" in _) throw new F(_.error.content, _.error.errorCode, f, _, m);
         return _
     }), {
         retryNetworkErrorMaxTimes: d,
         retryThrottledRequestMaxTimes: u
     })
 }
 
 function Ms(s, {
     publicKey: i,
     baseURL: t = S.baseURL,
     signal: e,
     source: r,
     integration: n,
     userAgent: o,
-    retryThrottledRequestMaxTimes: l = S.retryThrottledRequestMaxTimes,
-    retryNetworkErrorMaxTimes: a = S.retryNetworkErrorMaxTimes
+    retryThrottledRequestMaxTimes: a = S.retryThrottledRequestMaxTimes,
+    retryNetworkErrorMaxTimes: l = S.retryNetworkErrorMaxTimes
 }) {
     return yt(() => bt({
         method: "GET",
         headers: {
             "X-UC-User-Agent": kt({
                 publicKey: i,
                 integration: n,
@@ -1553,31 +1553,31 @@
         signal: e
     }).then(({
         data: c,
         headers: u,
         request: d
     }) => {
         let p = pt(JSON.parse(c));
-        if ("error" in p) throw new D(p.error.content, p.error.errorCode, d, p, u);
+        if ("error" in p) throw new F(p.error.content, p.error.errorCode, d, p, u);
         return p
     }), {
-        retryThrottledRequestMaxTimes: l,
-        retryNetworkErrorMaxTimes: a
+        retryThrottledRequestMaxTimes: a,
+        retryNetworkErrorMaxTimes: l
     })
 }
 
-function eo(s, {
+function io(s, {
     publicKey: i,
     contentType: t,
     fileName: e,
     multipartChunkSize: r = S.multipartChunkSize,
     baseURL: n = "",
     secureSignature: o,
-    secureExpire: l,
-    store: a,
+    secureExpire: a,
+    store: l,
     signal: c,
     source: u = "local",
     integration: d,
     userAgent: p,
     retryThrottledRequestMaxTimes: m = S.retryThrottledRequestMaxTimes,
     retryNetworkErrorMaxTimes: f = S.retryNetworkErrorMaxTimes,
     metadata: _
@@ -1590,142 +1590,142 @@
         headers: {
             "X-UC-User-Agent": kt({
                 publicKey: i,
                 integration: d,
                 userAgent: p
             })
         },
-        data: Me({
+        data: Re({
             filename: e || Os,
             size: s,
-            content_type: t || Pe,
+            content_type: t || Oe,
             part_size: r,
-            UPLOADCARE_STORE: Di(a),
+            UPLOADCARE_STORE: Fi(l),
             UPLOADCARE_PUB_KEY: i,
             signature: o,
-            expire: l,
+            expire: a,
             source: u,
             metadata: _
         }),
         signal: c
     }).then(({
-        data: b,
+        data: y,
         headers: x,
-        request: v
+        request: T
     }) => {
-        let A = pt(JSON.parse(b));
-        if ("error" in A) throw new D(A.error.content, A.error.errorCode, v, A, x);
-        return A.parts = Object.keys(A.parts).map(V => A.parts[V]), A
+        let w = pt(JSON.parse(y));
+        if ("error" in w) throw new F(w.error.content, w.error.errorCode, T, w, x);
+        return w.parts = Object.keys(w.parts).map(V => w.parts[Number(V)]), w
     }), {
         retryThrottledRequestMaxTimes: m,
         retryNetworkErrorMaxTimes: f
     })
 }
 
-function io(s, i, {
+function so(s, i, {
     contentType: t,
     signal: e,
     onProgress: r,
     retryThrottledRequestMaxTimes: n = S.retryThrottledRequestMaxTimes,
     retryNetworkErrorMaxTimes: o = S.retryNetworkErrorMaxTimes
 }) {
     return yt(() => bt({
         method: "PUT",
         url: i,
         data: s,
         onProgress: r,
         signal: e,
         headers: {
-            "Content-Type": t || Pe
+            "Content-Type": t || Oe
         }
-    }).then(l => (r && r({
+    }).then(a => (r && r({
         isComputable: !0,
         value: 1
-    }), l)).then(({
-        status: l
+    }), a)).then(({
+        status: a
     }) => ({
-        code: l
+        code: a
     })), {
         retryThrottledRequestMaxTimes: n,
         retryNetworkErrorMaxTimes: o
     })
 }
 
-function so(s, {
+function ro(s, {
     publicKey: i,
     baseURL: t = S.baseURL,
     source: e = "local",
     signal: r,
     integration: n,
     userAgent: o,
-    retryThrottledRequestMaxTimes: l = S.retryThrottledRequestMaxTimes,
-    retryNetworkErrorMaxTimes: a = S.retryNetworkErrorMaxTimes
+    retryThrottledRequestMaxTimes: a = S.retryThrottledRequestMaxTimes,
+    retryNetworkErrorMaxTimes: l = S.retryNetworkErrorMaxTimes
 }) {
     return yt(() => bt({
         method: "POST",
         url: ut(t, "/multipart/complete/", {
             jsonerrors: 1
         }),
         headers: {
             "X-UC-User-Agent": kt({
                 publicKey: i,
                 integration: n,
                 userAgent: o
             })
         },
-        data: Me({
+        data: Re({
             uuid: s,
             UPLOADCARE_PUB_KEY: i,
             source: e
         }),
         signal: r
     }).then(({
         data: c,
         headers: u,
         request: d
     }) => {
         let p = pt(JSON.parse(c));
-        if ("error" in p) throw new D(p.error.content, p.error.errorCode, d, p, u);
+        if ("error" in p) throw new F(p.error.content, p.error.errorCode, d, p, u);
         return p
     }), {
-        retryThrottledRequestMaxTimes: l,
-        retryNetworkErrorMaxTimes: a
+        retryThrottledRequestMaxTimes: a,
+        retryNetworkErrorMaxTimes: l
     })
 }
 
-function Fi(s, {
+function Bi(s, {
     publicKey: i,
     baseURL: t,
     source: e,
     integration: r,
     userAgent: n,
     retryThrottledRequestMaxTimes: o,
-    retryNetworkErrorMaxTimes: l,
-    signal: a,
+    retryNetworkErrorMaxTimes: a,
+    signal: l,
     onProgress: c
 }) {
     return ks({
         check: u => Ms(s, {
             publicKey: i,
             baseURL: t,
             signal: u,
             source: e,
             integration: r,
             userAgent: n,
             retryThrottledRequestMaxTimes: o,
-            retryNetworkErrorMaxTimes: l
+            retryNetworkErrorMaxTimes: a
         }).then(d => d.isReady ? d : (c && c({
             isComputable: !0,
             value: 1
         }), !1)),
-        signal: a
+        signal: l
     })
 }
 
-function ro(s) {
+function no(s) {
     return "defaultEffects" in s
 }
 var dt = class {
         constructor(i, {
             baseCDN: t = S.baseCDN,
             fileName: e
         } = {}) {
@@ -1743,85 +1743,85 @@
             h(this, "contentInfo", null);
             h(this, "metadata", null);
             h(this, "s3Bucket", null);
             h(this, "defaultEffects", null);
             let {
                 uuid: r,
                 s3Bucket: n
-            } = i, o = ut(t, `${r}/`), l = n ? ut(`https://${n}.s3.amazonaws.com/`, `${r}/${i.filename}`) : null;
-            this.uuid = r, this.name = e || i.filename, this.size = i.size, this.isStored = i.isStored, this.isImage = i.isImage, this.mimeType = i.mimeType, this.cdnUrl = o, this.originalFilename = i.originalFilename, this.imageInfo = i.imageInfo, this.videoInfo = i.videoInfo, this.contentInfo = i.contentInfo, this.metadata = i.metadata || null, this.s3Bucket = n || null, this.s3Url = l, ro(i) && (this.defaultEffects = i.defaultEffects)
+            } = i, o = ut(t, `${r}/`), a = n ? ut(`https://${n}.s3.amazonaws.com/`, `${r}/${i.filename}`) : null;
+            this.uuid = r, this.name = e || i.filename, this.size = i.size, this.isStored = i.isStored, this.isImage = i.isImage, this.mimeType = i.mimeType, this.cdnUrl = o, this.originalFilename = i.originalFilename, this.imageInfo = i.imageInfo, this.videoInfo = i.videoInfo, this.contentInfo = i.contentInfo, this.metadata = i.metadata || null, this.s3Bucket = n || null, this.s3Url = a, no(i) && (this.defaultEffects = i.defaultEffects)
         }
     },
-    no = (s, {
+    oo = (s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
         secureSignature: r,
         secureExpire: n,
         store: o,
-        contentType: l,
-        signal: a,
+        contentType: a,
+        signal: l,
         onProgress: c,
         source: u,
         integration: d,
         userAgent: p,
         retryThrottledRequestMaxTimes: m,
         retryNetworkErrorMaxTimes: f,
         baseCDN: _,
-        metadata: b
-    }) => Yn(s, {
+        metadata: y
+    }) => Jn(s, {
         publicKey: i,
         fileName: t,
-        contentType: l,
+        contentType: a,
         baseURL: e,
         secureSignature: r,
         secureExpire: n,
         store: o,
-        signal: a,
+        signal: l,
         onProgress: c,
         source: u,
         integration: d,
         userAgent: p,
         retryThrottledRequestMaxTimes: m,
         retryNetworkErrorMaxTimes: f,
-        metadata: b
+        metadata: y
     }).then(({
         file: x
-    }) => Fi(x, {
+    }) => Bi(x, {
         publicKey: i,
         baseURL: e,
         source: u,
         integration: d,
         userAgent: p,
         retryThrottledRequestMaxTimes: m,
         retryNetworkErrorMaxTimes: f,
         onProgress: c,
-        signal: a
+        signal: l
     })).then(x => new dt(x, {
         baseCDN: _
     })),
-    oo = (s, {
+    ao = (s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
         signal: r,
         onProgress: n,
         source: o,
-        integration: l,
-        userAgent: a,
+        integration: a,
+        userAgent: l,
         retryThrottledRequestMaxTimes: c,
         retryNetworkErrorMaxTimes: u,
         baseCDN: d
     }) => Ms(s, {
         publicKey: i,
         baseURL: e,
         signal: r,
         source: o,
-        integration: l,
-        userAgent: a,
+        integration: a,
+        userAgent: l,
         retryThrottledRequestMaxTimes: c,
         retryNetworkErrorMaxTimes: u
     }).then(p => new dt(p, {
         baseCDN: d,
         fileName: t
     })).then(p => (n && n({
         isComputable: !0,
@@ -1830,71 +1830,71 @@
     lo = (s, {
         signal: i
     } = {}) => {
         let t = null,
             e = null,
             r = s.map(() => new AbortController),
             n = o => () => {
-                e = o, r.forEach((l, a) => a !== o && l.abort())
+                e = o, r.forEach((a, l) => l !== o && a.abort())
             };
-        return Oe(i, () => {
+        return ke(i, () => {
             r.forEach(o => o.abort())
-        }), Promise.all(s.map((o, l) => {
-            let a = n(l);
+        }), Promise.all(s.map((o, a) => {
+            let l = n(a);
             return Promise.resolve().then(() => o({
-                stopRace: a,
-                signal: r[l].signal
-            })).then(c => (a(), c)).catch(c => (t = c, null))
+                stopRace: l,
+                signal: r[a].signal
+            })).then(c => (l(), c)).catch(c => (t = c, null))
         })).then(o => {
             if (e === null) throw t;
             return o[e]
         })
     },
-    ao = window.WebSocket,
-    Ui = class {
+    co = window.WebSocket,
+    Ri = class {
         constructor() {
             h(this, "events", Object.create({}))
         }
         emit(i, t) {
             var e;
             (e = this.events[i]) == null || e.forEach(r => r(t))
         }
         on(i, t) {
             this.events[i] = this.events[i] || [], this.events[i].push(t)
         }
         off(i, t) {
             t ? this.events[i] = this.events[i].filter(e => e !== t) : this.events[i] = []
         }
     },
-    co = (s, i) => s === "success" ? {
+    ho = (s, i) => s === "success" ? {
         status: H.Success,
         ...i
     } : s === "progress" ? {
         status: H.Progress,
         ...i
     } : {
         status: H.Error,
         ...i
     },
-    Ri = class {
+    Mi = class {
         constructor(i, t = 3e4) {
             h(this, "key");
             h(this, "disconnectTime");
             h(this, "ws");
             h(this, "queue", []);
             h(this, "isConnected", !1);
             h(this, "subscribers", 0);
-            h(this, "emmitter", new Ui);
+            h(this, "emmitter", new Ri);
             h(this, "disconnectTimeoutId", null);
             this.key = i, this.disconnectTime = t
         }
         connect() {
             if (this.disconnectTimeoutId && clearTimeout(this.disconnectTimeoutId), !this.isConnected && !this.ws) {
                 let i = `wss://ws.pusherapp.com/app/${this.key}?protocol=5&client=js&version=1.12.2`;
-                this.ws = new ao(i), this.ws.addEventListener("error", t => {
+                this.ws = new co(i), this.ws.addEventListener("error", t => {
                     this.emmitter.emit("error", new Error(t.message))
                 }), this.emmitter.on("connected", () => {
                     this.isConnected = !0, this.queue.forEach(t => this.send(t.event, t.data)), this.queue = []
                 }), this.ws.addEventListener("message", t => {
                     let e = JSON.parse(t.data.toString());
                     switch (e.event) {
                         case "pusher:connection_established": {
@@ -1904,15 +1904,15 @@
                         case "pusher:ping": {
                             this.send("pusher:pong", {});
                             break
                         }
                         case "progress":
                         case "success":
                         case "fail":
-                            this.emmitter.emit(e.channel, co(e.event, JSON.parse(e.data)))
+                            this.emmitter.emit(e.channel, ho(e.event, JSON.parse(e.data)))
                     }
                 })
             }
         }
         disconnect() {
             let i = () => {
                 var t;
@@ -1952,416 +1952,416 @@
                 };
             this.emmitter.off(t), this.isConnected ? this.send(e.event, e.data) : this.queue = this.queue.filter(r => r.data.channel !== t), this.subscribers === 0 && this.disconnect()
         }
         onError(i) {
             return this.emmitter.on("error", i), () => this.emmitter.off("error", i)
         }
     },
-    Oi = null,
-    Bi = s => {
-        if (!Oi) {
+    Pi = null,
+    zi = s => {
+        if (!Pi) {
             let i = typeof window == "undefined" ? 0 : 3e4;
-            Oi = new Ri(s, i)
+            Pi = new Mi(s, i)
         }
-        return Oi
+        return Pi
     },
-    ho = s => {
-        Bi(s).connect()
+    uo = s => {
+        zi(s).connect()
     };
 
-function uo({
+function po({
     token: s,
     publicKey: i,
     baseURL: t,
     integration: e,
     userAgent: r,
     retryThrottledRequestMaxTimes: n,
     retryNetworkErrorMaxTimes: o,
-    onProgress: l,
-    signal: a
+    onProgress: a,
+    signal: l
 }) {
     return ks({
-        check: c => Qn(s, {
+        check: c => to(s, {
             publicKey: i,
             baseURL: t,
             integration: e,
             userAgent: r,
             retryThrottledRequestMaxTimes: n,
             retryNetworkErrorMaxTimes: o,
             signal: c
         }).then(u => {
             switch (u.status) {
                 case H.Error:
-                    return new D(u.error, u.errorCode);
+                    return new F(u.error, u.errorCode);
                 case H.Waiting:
                     return !1;
                 case H.Unknown:
-                    return new D(`Token "${s}" was not found.`);
+                    return new F(`Token "${s}" was not found.`);
                 case H.Progress:
-                    return l && (u.total === "unknown" ? l({
+                    return a && (u.total === "unknown" ? a({
                         isComputable: !1
-                    }) : l({
+                    }) : a({
                         isComputable: !0,
                         value: u.done / u.total
                     })), !1;
                 case H.Success:
-                    return l && l({
+                    return a && a({
                         isComputable: !0,
                         value: u.done / u.total
                     }), u;
                 default:
                     throw new Error("Unknown status")
             }
         }),
-        signal: a
+        signal: l
     })
 }
-var po = ({
+var fo = ({
         token: s,
         pusherKey: i,
         signal: t,
         onProgress: e
     }) => new Promise((r, n) => {
-        let o = Bi(i),
-            l = o.onError(n),
-            a = () => {
-                l(), o.unsubscribe(s)
+        let o = zi(i),
+            a = o.onError(n),
+            l = () => {
+                a(), o.unsubscribe(s)
             };
-        Oe(t, () => {
-            a(), n(new _t("pusher cancelled"))
+        ke(t, () => {
+            l(), n(new _t("pusher cancelled"))
         }), o.subscribe(s, c => {
             switch (c.status) {
                 case H.Progress: {
                     e && (c.total === "unknown" ? e({
                         isComputable: !1
                     }) : e({
                         isComputable: !0,
                         value: c.done / c.total
                     }));
                     break
                 }
                 case H.Success: {
-                    a(), e && e({
+                    l(), e && e({
                         isComputable: !0,
                         value: c.done / c.total
                     }), r(c);
                     break
                 }
                 case H.Error:
-                    a(), n(new D(c.msg, c.error_code))
+                    l(), n(new F(c.msg, c.error_code))
             }
         })
     }),
-    fo = (s, {
+    mo = (s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
         baseCDN: r,
         checkForUrlDuplicates: n,
         saveUrlForRecurrentUploads: o,
-        secureSignature: l,
-        secureExpire: a,
+        secureSignature: a,
+        secureExpire: l,
         store: c,
         signal: u,
         onProgress: d,
         source: p,
         integration: m,
         userAgent: f,
         retryThrottledRequestMaxTimes: _,
-        pusherKey: b = S.pusherKey,
+        pusherKey: y = S.pusherKey,
         metadata: x
-    }) => Promise.resolve(ho(b)).then(() => Jn(s, {
+    }) => Promise.resolve(uo(y)).then(() => Zn(s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
         checkForUrlDuplicates: n,
         saveUrlForRecurrentUploads: o,
-        secureSignature: l,
-        secureExpire: a,
+        secureSignature: a,
+        secureExpire: l,
         store: c,
         signal: u,
         source: p,
         integration: m,
         userAgent: f,
         retryThrottledRequestMaxTimes: _,
         metadata: x
-    })).catch(v => {
-        let A = Bi(b);
-        return A == null || A.disconnect(), Promise.reject(v)
-    }).then(v => v.type === Li.FileInfo ? v : lo([({
-        signal: A
-    }) => uo({
-        token: v.token,
+    })).catch(T => {
+        let w = zi(y);
+        return w == null || w.disconnect(), Promise.reject(T)
+    }).then(T => T.type === Ui.FileInfo ? T : lo([({
+        signal: w
+    }) => po({
+        token: T.token,
         publicKey: i,
         baseURL: e,
         integration: m,
         userAgent: f,
         retryThrottledRequestMaxTimes: _,
         onProgress: d,
-        signal: A
+        signal: w
     }), ({
-        signal: A
-    }) => po({
-        token: v.token,
-        pusherKey: b,
-        signal: A,
+        signal: w
+    }) => fo({
+        token: T.token,
+        pusherKey: y,
+        signal: w,
         onProgress: d
     })], {
         signal: u
-    })).then(v => {
-        if (v instanceof D) throw v;
-        return v
-    }).then(v => Fi(v.uuid, {
+    })).then(T => {
+        if (T instanceof F) throw T;
+        return T
+    }).then(T => Bi(T.uuid, {
         publicKey: i,
         baseURL: e,
         integration: m,
         userAgent: f,
         retryThrottledRequestMaxTimes: _,
         onProgress: d,
         signal: u
-    })).then(v => new dt(v, {
+    })).then(T => new dt(T, {
         baseCDN: r
     })),
-    Pi = new WeakMap,
-    mo = async s => {
-        if (Pi.has(s)) return Pi.get(s);
+    Li = new WeakMap,
+    go = async s => {
+        if (Li.has(s)) return Li.get(s);
         let i = await fetch(s.uri).then(t => t.blob());
-        return Pi.set(s, i), i
+        return Li.set(s, i), i
     }, Ns = async s => {
-        if (Ue(s) || Le(s)) return s.size;
-        if (Re(s)) return (await mo(s)).size;
+        if (Le(s) || Pe(s)) return s.size;
+        if (Ue(s)) return (await go(s)).size;
         throw new Error("Unknown file type. Cannot determine file size.")
-    }, go = (s, i = S.multipartMinFileSize) => s >= i, Ds = s => {
+    }, _o = (s, i = S.multipartMinFileSize) => s >= i, Ds = s => {
         let i = "[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}",
             t = new RegExp(i);
-        return !Bt(s) && t.test(s)
-    }, zi = s => {
+        return !Ft(s) && t.test(s)
+    }, Vi = s => {
         let i = "^(?:\\w+:)?\\/\\/([^\\s\\.]+\\.\\S{2}|localhost[\\:?\\d]*)\\S*$",
             t = new RegExp(i);
-        return !Bt(s) && t.test(s)
-    }, _o = (s, i) => new Promise((t, e) => {
+        return !Ft(s) && t.test(s)
+    }, bo = (s, i) => new Promise((t, e) => {
         let r = [],
             n = !1,
             o = i.length,
-            l = [...i],
-            a = () => {
-                let c = i.length - l.length,
-                    u = l.shift();
+            a = [...i],
+            l = () => {
+                let c = i.length - a.length,
+                    u = a.shift();
                 u && u().then(d => {
-                    n || (r[c] = d, o -= 1, o ? a() : t(r))
+                    n || (r[c] = d, o -= 1, o ? l() : t(r))
                 }).catch(d => {
                     n = !0, e(d)
                 })
             };
-        for (let c = 0; c < s; c++) a()
-    }), bo = (s, i, t, e) => {
+        for (let c = 0; c < s; c++) l()
+    }), yo = (s, i, t, e) => {
         let r = e * i,
             n = Math.min(r + e, t);
         return s.slice(r, n)
-    }, yo = async (s, i, t) => e => bo(s, e, i, t), vo = (s, i, {
+    }, vo = async (s, i, t) => e => yo(s, e, i, t), Co = (s, i, {
         publicKey: t,
         contentType: e,
         onProgress: r,
         signal: n,
         integration: o,
-        retryThrottledRequestMaxTimes: l,
-        retryNetworkErrorMaxTimes: a
-    }) => io(s, i, {
+        retryThrottledRequestMaxTimes: a,
+        retryNetworkErrorMaxTimes: l
+    }) => so(s, i, {
         publicKey: t,
         contentType: e,
         onProgress: r,
         signal: n,
         integration: o,
-        retryThrottledRequestMaxTimes: l,
-        retryNetworkErrorMaxTimes: a
-    }), Co = async (s, {
+        retryThrottledRequestMaxTimes: a,
+        retryNetworkErrorMaxTimes: l
+    }), wo = async (s, {
         publicKey: i,
         fileName: t,
         fileSize: e,
         baseURL: r,
         secureSignature: n,
         secureExpire: o,
-        store: l,
-        signal: a,
+        store: a,
+        signal: l,
         onProgress: c,
         source: u,
         integration: d,
         userAgent: p,
         retryThrottledRequestMaxTimes: m,
         retryNetworkErrorMaxTimes: f,
         contentType: _,
-        multipartChunkSize: b = S.multipartChunkSize,
+        multipartChunkSize: y = S.multipartChunkSize,
         maxConcurrentRequests: x = S.maxConcurrentRequests,
-        baseCDN: v,
-        metadata: A
+        baseCDN: T,
+        metadata: w
     }) => {
         let V = e != null ? e : await Ns(s),
-            lt, St = (U, j) => {
+            at, St = (U, j) => {
                 if (!c) return;
-                lt || (lt = Array(U).fill(0));
-                let Z = tt => tt.reduce((at, Ti) => at + Ti, 0);
+                at || (at = Array(U).fill(0));
+                let Z = tt => tt.reduce((lt, Si) => lt + Si, 0);
                 return tt => {
-                    tt.isComputable && (lt[j] = tt.value, c({
+                    tt.isComputable && (at[j] = tt.value, c({
                         isComputable: !0,
-                        value: Z(lt) / U
+                        value: Z(at) / U
                     }))
                 }
             };
-        return _ || (_ = Us(s)), eo(V, {
+        return _ || (_ = Us(s)), io(V, {
             publicKey: i,
             contentType: _,
             fileName: t || Rs(s),
             baseURL: r,
             secureSignature: n,
             secureExpire: o,
-            store: l,
-            signal: a,
+            store: a,
+            signal: l,
             source: u,
             integration: d,
             userAgent: p,
             retryThrottledRequestMaxTimes: m,
             retryNetworkErrorMaxTimes: f,
-            metadata: A
+            metadata: w
         }).then(async ({
             uuid: U,
             parts: j
         }) => {
-            let Z = await yo(s, V, b);
-            return Promise.all([U, _o(x, j.map((tt, at) => () => vo(Z(at), tt, {
+            let Z = await vo(s, V, y);
+            return Promise.all([U, bo(x, j.map((tt, lt) => () => Co(Z(lt), tt, {
                 publicKey: i,
                 contentType: _,
-                onProgress: St(j.length, at),
-                signal: a,
+                onProgress: St(j.length, lt),
+                signal: l,
                 integration: d,
                 retryThrottledRequestMaxTimes: m,
                 retryNetworkErrorMaxTimes: f
             })))])
-        }).then(([U]) => so(U, {
+        }).then(([U]) => ro(U, {
             publicKey: i,
             baseURL: r,
             source: u,
             integration: d,
             userAgent: p,
             retryThrottledRequestMaxTimes: m,
             retryNetworkErrorMaxTimes: f
-        })).then(U => U.isReady ? U : Fi(U.uuid, {
+        })).then(U => U.isReady ? U : Bi(U.uuid, {
             publicKey: i,
             baseURL: r,
             source: u,
             integration: d,
             userAgent: p,
             retryThrottledRequestMaxTimes: m,
             retryNetworkErrorMaxTimes: f,
             onProgress: c,
-            signal: a
+            signal: l
         })).then(U => new dt(U, {
-            baseCDN: v
+            baseCDN: T
         }))
     };
-async function Vi(s, {
+async function ji(s, {
     publicKey: i,
     fileName: t,
     baseURL: e = S.baseURL,
     secureSignature: r,
     secureExpire: n,
     store: o,
-    signal: l,
-    onProgress: a,
+    signal: a,
+    onProgress: l,
     source: c,
     integration: u,
     userAgent: d,
     retryThrottledRequestMaxTimes: p,
     retryNetworkErrorMaxTimes: m,
     contentType: f,
     multipartMinFileSize: _,
-    multipartChunkSize: b,
+    multipartChunkSize: y,
     maxConcurrentRequests: x,
-    baseCDN: v = S.baseCDN,
-    checkForUrlDuplicates: A,
+    baseCDN: T = S.baseCDN,
+    checkForUrlDuplicates: w,
     saveUrlForRecurrentUploads: V,
-    pusherKey: lt,
+    pusherKey: at,
     metadata: St
 }) {
-    if (Bt(s)) {
+    if (Ft(s)) {
         let U = await Ns(s);
-        return go(U, _) ? Co(s, {
+        return _o(U, _) ? wo(s, {
             publicKey: i,
             contentType: f,
-            multipartChunkSize: b,
+            multipartChunkSize: y,
             fileSize: U,
             fileName: t,
             baseURL: e,
             secureSignature: r,
             secureExpire: n,
             store: o,
-            signal: l,
-            onProgress: a,
+            signal: a,
+            onProgress: l,
             source: c,
             integration: u,
             userAgent: d,
             maxConcurrentRequests: x,
             retryThrottledRequestMaxTimes: p,
             retryNetworkErrorMaxTimes: m,
-            baseCDN: v,
+            baseCDN: T,
             metadata: St
-        }) : no(s, {
+        }) : oo(s, {
             publicKey: i,
             fileName: t,
             contentType: f,
             baseURL: e,
             secureSignature: r,
             secureExpire: n,
             store: o,
-            signal: l,
-            onProgress: a,
+            signal: a,
+            onProgress: l,
             source: c,
             integration: u,
             userAgent: d,
             retryThrottledRequestMaxTimes: p,
             retryNetworkErrorMaxTimes: m,
-            baseCDN: v,
+            baseCDN: T,
             metadata: St
         })
     }
-    if (zi(s)) return fo(s, {
+    if (Vi(s)) return mo(s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
-        baseCDN: v,
-        checkForUrlDuplicates: A,
+        baseCDN: T,
+        checkForUrlDuplicates: w,
         saveUrlForRecurrentUploads: V,
         secureSignature: r,
         secureExpire: n,
         store: o,
-        signal: l,
-        onProgress: a,
+        signal: a,
+        onProgress: l,
         source: c,
         integration: u,
         userAgent: d,
         retryThrottledRequestMaxTimes: p,
         retryNetworkErrorMaxTimes: m,
-        pusherKey: lt,
+        pusherKey: at,
         metadata: St
     });
-    if (Ds(s)) return oo(s, {
+    if (Ds(s)) return ao(s, {
         publicKey: i,
         fileName: t,
         baseURL: e,
-        signal: l,
-        onProgress: a,
+        signal: a,
+        onProgress: l,
         source: c,
         integration: u,
         userAgent: d,
         retryThrottledRequestMaxTimes: p,
         retryNetworkErrorMaxTimes: m,
-        baseCDN: v
+        baseCDN: T
     });
     throw new TypeError(`File uploading from "${s}" is not supported`)
 }
-var Mi = class {
+var Ni = class {
         constructor(i, {
             baseCDN: t = S.baseCDN
         } = {}) {
             h(this, "uuid");
             h(this, "filesCount");
             h(this, "totalSize");
             h(this, "isStored");
@@ -2373,110 +2373,110 @@
             this.uuid = i.id, this.filesCount = i.filesCount;
             let e = i.files.filter(Boolean);
             this.totalSize = Object.values(e).reduce((r, n) => r + n.size, 0), this.isStored = !!i.datetimeStored, this.isImage = !!Object.values(e).filter(r => r.isImage).length, this.cdnUrl = i.cdnUrl, this.files = e.map(r => new dt(r, {
                 baseCDN: t
             })), this.createdAt = i.datetimeCreated, this.storedAt = i.datetimeStored
         }
     },
-    wo = s => {
+    Eo = s => {
         for (let i of s)
-            if (!Bt(i)) return !1;
+            if (!Ft(i)) return !1;
         return !0
     },
     Ao = s => {
         for (let i of s)
             if (!Ds(i)) return !1;
         return !0
     },
-    Eo = s => {
+    xo = s => {
         for (let i of s)
-            if (!zi(i)) return !1;
+            if (!Vi(i)) return !1;
         return !0
     };
 
 function Fs(s, {
     publicKey: i,
     fileName: t,
     baseURL: e = S.baseURL,
     secureSignature: r,
     secureExpire: n,
     store: o,
-    signal: l,
-    onProgress: a,
+    signal: a,
+    onProgress: l,
     source: c,
     integration: u,
     userAgent: d,
     retryThrottledRequestMaxTimes: p,
     retryNetworkErrorMaxTimes: m,
     contentType: f,
     multipartChunkSize: _ = S.multipartChunkSize,
-    baseCDN: b = S.baseCDN,
+    baseCDN: y = S.baseCDN,
     checkForUrlDuplicates: x,
-    saveUrlForRecurrentUploads: v,
-    jsonpCallback: A
+    saveUrlForRecurrentUploads: T,
+    jsonpCallback: w
 }) {
-    if (!wo(s) && !Eo(s) && !Ao(s)) throw new TypeError(`Group uploading from "${s}" is not supported`);
-    let V, lt = !0,
+    if (!Eo(s) && !xo(s) && !Ao(s)) throw new TypeError(`Group uploading from "${s}" is not supported`);
+    let V, at = !0,
         St = s.length,
         U = (j, Z) => {
-            if (!a) return;
+            if (!l) return;
             V || (V = Array(j).fill(0));
-            let tt = at => at.reduce((Ti, sn) => Ti + sn) / j;
-            return at => {
-                if (!at.isComputable || !lt) {
-                    lt = !1, a({
+            let tt = lt => lt.reduce((Si, rn) => Si + rn) / j;
+            return lt => {
+                if (!lt.isComputable || !at) {
+                    at = !1, l({
                         isComputable: !1
                     });
                     return
                 }
-                V[Z] = at.value, a({
+                V[Z] = lt.value, l({
                     isComputable: !0,
                     value: tt(V)
                 })
             }
         };
-    return Promise.all(s.map((j, Z) => Bt(j) || zi(j) ? Vi(j, {
+    return Promise.all(s.map((j, Z) => Ft(j) || Vi(j) ? ji(j, {
         publicKey: i,
         fileName: t,
         baseURL: e,
         secureSignature: r,
         secureExpire: n,
         store: o,
-        signal: l,
+        signal: a,
         onProgress: U(St, Z),
         source: c,
         integration: u,
         userAgent: d,
         retryThrottledRequestMaxTimes: p,
         retryNetworkErrorMaxTimes: m,
         contentType: f,
         multipartChunkSize: _,
-        baseCDN: b,
+        baseCDN: y,
         checkForUrlDuplicates: x,
-        saveUrlForRecurrentUploads: v
-    }).then(tt => tt.uuid) : j)).then(j => to(j, {
+        saveUrlForRecurrentUploads: T
+    }).then(tt => tt.uuid) : j)).then(j => eo(j, {
         publicKey: i,
         baseURL: e,
-        jsonpCallback: A,
+        jsonpCallback: w,
         secureSignature: r,
         secureExpire: n,
-        signal: l,
+        signal: a,
         source: c,
         integration: u,
         userAgent: d,
         retryThrottledRequestMaxTimes: p,
         retryNetworkErrorMaxTimes: m
-    }).then(Z => new Mi(Z, {
-        baseCDN: b
-    })).then(Z => (a && a({
+    }).then(Z => new Ni(Z, {
+        baseCDN: y
+    })).then(Z => (l && l({
         isComputable: !0,
         value: 1
     }), Z)))
 }
-var ke = class {
+var Ie = class {
     constructor(i) {
         h(this, "_concurrency", 1);
         h(this, "_pending", []);
         h(this, "_running", 0);
         h(this, "_resolvers", new Map);
         h(this, "_rejectors", new Map);
         this._concurrency = i
@@ -2508,38 +2508,38 @@
     set concurrency(i) {
         this._concurrency = i, this._run()
     }
     get concurrency() {
         return this._concurrency
     }
 };
-var ji = () => ({
+var Hi = () => ({
         "*blocksRegistry": new Set,
         "*eventEmitter": null
     }),
-    Hi = s => ({
-        ...ji(),
+    Gi = s => ({
+        ...Hi(),
         "*currentActivity": "",
         "*currentActivityParams": {},
         "*history": [],
         "*historyBack": null,
         "*closeModal": () => {
             s.set$({
                 "*modalActive": !1,
                 "*currentActivity": ""
             })
         }
     }),
-    Ne = s => ({
-        ...Hi(s),
+    Me = s => ({
+        ...Gi(s),
         "*commonProgress": 0,
         "*uploadList": [],
         "*focusedEntry": null,
         "*uploadMetadata": null,
-        "*uploadQueue": new ke(1),
+        "*uploadQueue": new Ie(1),
         "*uploadCollection": null,
         "*collectionErrors": [],
         "*collectionState": null,
         "*groupInfo": null,
         "*uploadTrigger": new Set
     });
 
@@ -2553,40 +2553,40 @@
         }
         let n = "l10n:" + e;
         i.__l10nKeys.push(n), i.add(n, e), i.sub(n, o => {
             t[r] = i.l10n(o)
         }), t.removeAttribute("l10n")
     })
 }
-var F = s => `*cfg/${s}`;
-var Gi = "lr-",
-    w = class extends Dt {
+var B = s => `*cfg/${s}`;
+var Wi = "lr-",
+    C = class extends Nt {
         constructor() {
             super();
             h(this, "requireCtxName", !1);
             h(this, "allowCustomTemplate", !0);
             h(this, "activityType", null);
-            h(this, "init$", ji());
+            h(this, "init$", Hi());
             h(this, "updateCtxCssData", () => {
                 It("Using CSS variables for configuration is deprecated. Please use `lr-config` instead. See migration guide: https://uploadcare.com/docs/file-uploader/migration-to-0.25.0/");
                 let t = this.$["*blocksRegistry"];
                 for (let e of t) e.isConnected && e.updateCssData()
             });
             this.addTemplateProcessor(Bs), this.__l10nKeys = []
         }
         l10n(t, e = {}) {
             if (!t) return "";
             let r = this.getCssData("--l10n-" + t, !0) || t,
                 n = xs(r);
-            for (let l of n) e[l.variable] = this.pluralize(l.pluralKey, Number(e[l.countVariable]));
+            for (let a of n) e[a.variable] = this.pluralize(a.pluralKey, Number(e[a.countVariable]));
             return Zt(r, e)
         }
         pluralize(t, e) {
             let r = this.l10n("locale-name") || "en-US",
-                n = $e(r, e);
+                n = Se(r, e);
             return this.l10n(`${t}__${n}`)
         }
         emit(t, e, r) {
             let n = this.has("*eventEmitter") && this.$["*eventEmitter"];
             n && n.emit(t, e, r)
         }
         applyL10nKey(t, e) {
@@ -2609,30 +2609,30 @@
                 this.$["*currentActivity"] = t;
                 return
             }
             console.warn(`Activity type "${t}" not found in the context`)
         }
         connectedCallback() {
             let t = this.constructor.className;
-            t && this.classList.toggle(`${Gi}${t}`, !0), this.hasAttribute("retpl") && (this.constructor.template = null, this.processInnerHtml = !0), this.requireCtxName ? Ie({
+            t && this.classList.toggle(`${Wi}${t}`, !0), this.hasAttribute("retpl") && (this.constructor.template = null, this.processInnerHtml = !0), this.requireCtxName ? $e({
                 element: this,
                 attribute: "ctx-name",
                 onSuccess: () => {
                     super.connectedCallback()
                 },
                 onTimeout: () => {
                     console.error("Attribute `ctx-name` is required and it is not set.")
                 }
             }) : super.connectedCallback(), $t.registerClient(this)
         }
         disconnectedCallback() {
             super.disconnectedCallback(), $t.unregisterClient(this)
         }
         initCallback() {
-            this.$["*blocksRegistry"].add(this), this.$["*eventEmitter"] || (this.$["*eventEmitter"] = new Se(this.debugPrint.bind(this)))
+            this.$["*blocksRegistry"].add(this), this.$["*eventEmitter"] || (this.$["*eventEmitter"] = new Te(this.debugPrint.bind(this)))
         }
         destroyCallback() {
             let t = this.$["*blocksRegistry"];
             t.delete(this), E.deleteCtx(this), t.size === 0 && setTimeout(() => {
                 this.destroyCtxCallback()
             }, 0)
         }
@@ -2640,17 +2640,17 @@
             E.deleteCtx(this.ctxName)
         }
         fileSizeFmt(t, e = 2) {
             let r = ["B", "KB", "MB", "GB", "TB"],
                 n = c => this.getCssData("--l10n-unit-" + c.toLowerCase(), !0) || c;
             if (t === 0) return `0 ${n(r[0])}`;
             let o = 1024,
-                l = e < 0 ? 0 : e,
-                a = Math.floor(Math.log(t) / Math.log(o));
-            return parseFloat((t / o ** a).toFixed(l)) + " " + n(r[a])
+                a = e < 0 ? 0 : e,
+                l = Math.floor(Math.log(t) / Math.log(o));
+            return parseFloat((t / o ** l).toFixed(a)) + " " + n(r[l])
         }
         proxyUrl(t) {
             let e = this.cfg.secureDeliveryProxy;
             return e ? Zt(e, {
                 previewUrl: t
             }, {
                 transform: r => window.encodeURIComponent(r)
@@ -2664,29 +2664,29 @@
         }
         get cfg() {
             if (!this.__cfgProxy) {
                 let t = Object.create(null);
                 this.__cfgProxy = new Proxy(t, {
                     set: (e, r, n) => {
                         if (typeof r != "string") return !1;
-                        let o = F(r);
+                        let o = B(r);
                         return this.$[o] = n, !0
                     },
                     get: (e, r) => {
-                        let n = F(r),
+                        let n = B(r),
                             o = this.parseCfgProp(n);
                         return o.ctx.has(o.name) ? o.ctx.read(o.name) : (It("Using CSS variables for configuration is deprecated. Please use `lr-config` instead. See migration guide: https://uploadcare.com/docs/file-uploader/migration-to-0.25.0/"), this.getCssData(`--cfg-${ht(r)}`))
                     }
                 })
             }
             return this.__cfgProxy
         }
         subConfigValue(t, e) {
-            let r = this.parseCfgProp(F(t));
-            r.ctx.has(r.name) ? this.sub(F(t), e) : (this.bindCssData(`--cfg-${ht(t)}`), this.sub(`--cfg-${ht(t)}`, e))
+            let r = this.parseCfgProp(B(t));
+            r.ctx.has(r.name) ? this.sub(B(t), e) : (this.bindCssData(`--cfg-${ht(t)}`), this.sub(`--cfg-${ht(t)}`, e))
         }
         debugPrint(...t) {
             if (!this.cfg.debug) return;
             let e = t;
             if (typeof(t == null ? void 0 : t[0]) == "function") {
                 let r = t[0];
                 e = r()
@@ -2697,25 +2697,25 @@
             return this.ctxName
         }
         static reg(t) {
             if (!t) {
                 super.reg();
                 return
             }
-            super.reg(t.startsWith(Gi) ? t : Gi + t)
+            super.reg(t.startsWith(Wi) ? t : Wi + t)
         }
     };
-h(w, "StateConsumerScope", null), h(w, "className", "");
+h(C, "StateConsumerScope", null), h(C, "className", "");
 var zs = "active",
     te = "___ACTIVITY_IS_ACTIVE___",
-    Q = class Q extends w {
+    Q = class Q extends C {
         constructor() {
             super(...arguments);
             h(this, "historyTracked", !1);
-            h(this, "init$", Hi(this));
+            h(this, "init$", Gi(this));
             h(this, "_debouncedHistoryFlush", k(this._historyFlush.bind(this), 10))
         }
         _deactivate() {
             var e;
             let t = Q._activityRegistry[this.activityKey];
             this[te] = !1, this.removeAttribute(zs), (e = t == null ? void 0 : t.deactivateCallback) == null || e.call(t)
         }
@@ -2780,16 +2780,16 @@
             var e;
             let t = this.$["*history"];
             if (t) {
                 let r = t.pop();
                 for (; r === this.activityType;) r = t.pop();
                 let n = !!r;
                 if (r) {
-                    let l = [...this.$["*blocksRegistry"]].find(a => a.activityType === r);
-                    n = (e = l == null ? void 0 : l.couldOpenActivity) != null ? e : !1
+                    let a = [...this.$["*blocksRegistry"]].find(l => l.activityType === r);
+                    n = (e = a == null ? void 0 : a.couldOpenActivity) != null ? e : !1
                 }
                 r = n ? r : void 0, this.$["*currentActivity"] = r, this.$["*history"] = t, r || this.setOrAddState("*modalActive", !1)
             }
         }
     };
 h(Q, "_activityRegistry", Object.create(null));
 var g = Q;
@@ -2801,54 +2801,54 @@
     URL: "url",
     CONFIRMATION: "confirmation",
     CLOUD_IMG_EDIT: "cloud-image-edit",
     EXTERNAL: "external",
     DETAILS: "details"
 });
 var ee = 33.333333333333336,
-    y = 1,
-    Wi = 24,
+    b = 1,
+    Xi = 24,
     Vs = 6;
 
 function Ot(s, i) {
     for (let t in i) s.setAttributeNS(null, t, i[t].toString())
 }
 
-function K(s, i = {}) {
+function Y(s, i = {}) {
     let t = document.createElementNS("http://www.w3.org/2000/svg", s);
     return Ot(t, i), t
 }
 
 function js(s, i, t) {
     let {
         x: e,
         y: r,
         width: n,
         height: o
-    } = s, l = i.includes("w") ? 0 : 1, a = i.includes("n") ? 0 : 1, c = [-1, 1][l], u = [-1, 1][a], d = [e + l * n + 1.5 * c, r + a * o + 1.5 * u - 24 * t * u], p = [e + l * n + 1.5 * c, r + a * o + 1.5 * u], m = [e + l * n - 24 * t * c + 1.5 * c, r + a * o + 1.5 * u];
+    } = s, a = i.includes("w") ? 0 : 1, l = i.includes("n") ? 0 : 1, c = [-1, 1][a], u = [-1, 1][l], d = [e + a * n + 1.5 * c, r + l * o + 1.5 * u - 24 * t * u], p = [e + a * n + 1.5 * c, r + l * o + 1.5 * u], m = [e + a * n - 24 * t * c + 1.5 * c, r + l * o + 1.5 * u];
     return {
         d: `M ${d[0]} ${d[1]} L ${p[0]} ${p[1]} L ${m[0]} ${m[1]}`,
         center: p
     }
 }
 
 function Hs(s, i, t) {
     let {
         x: e,
         y: r,
         width: n,
         height: o
-    } = s, l = ["n", "s"].includes(i) ? .5 : {
+    } = s, a = ["n", "s"].includes(i) ? .5 : {
         w: 0,
         e: 1
-    } [i], a = ["w", "e"].includes(i) ? .5 : {
+    } [i], l = ["w", "e"].includes(i) ? .5 : {
         n: 0,
         s: 1
-    } [i], c = [-1, 1][l], u = [-1, 1][a], d, p;
-    ["n", "s"].includes(i) ? (d = [e + l * n - 34 * t / 2, r + a * o + 1.5 * u], p = [e + l * n + 34 * t / 2, r + a * o + 1.5 * u]) : (d = [e + l * n + 1.5 * c, r + a * o - 34 * t / 2], p = [e + l * n + 1.5 * c, r + a * o + 34 * t / 2]);
+    } [i], c = [-1, 1][a], u = [-1, 1][l], d, p;
+    ["n", "s"].includes(i) ? (d = [e + a * n - 34 * t / 2, r + l * o + 1.5 * u], p = [e + a * n + 34 * t / 2, r + l * o + 1.5 * u]) : (d = [e + a * n + 1.5 * c, r + l * o - 34 * t / 2], p = [e + a * n + 1.5 * c, r + l * o + 34 * t / 2]);
     let m = `M ${d[0]} ${d[1]} L ${p[0]} ${p[1]}`,
         f = [p[0] - (p[0] - d[0]) / 2, p[1] - (p[1] - d[1]) / 2];
     return {
         d: m,
         center: f
     }
 }
@@ -2858,219 +2858,219 @@
 }
 
 function Ws({
     rect: s,
     delta: [i, t],
     imageBox: e
 }) {
-    return Vt({
+    return zt({
         ...s,
         x: s.x + i,
         y: s.y + t
     }, e)
 }
 
-function Vt(s, i) {
+function zt(s, i) {
     let {
         x: t
     } = s, {
         y: e
     } = s;
     return s.x < i.x ? t = i.x : s.x + s.width > i.x + i.width && (t = i.x + i.width - s.width), s.y < i.y ? e = i.y : s.y + s.height > i.y + i.height && (e = i.y + i.height - s.height), {
         ...s,
         x: t,
         y: e
     }
 }
 
-function xo({
+function To({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [, r] = i, {
         y: n,
         width: o,
-        height: l
+        height: a
     } = s;
-    n += r, l -= r, t && (o = l * t);
-    let a = s.x + s.width / 2 - o / 2;
-    return n <= e.y && (n = e.y, l = s.y + s.height - n, t && (o = l * t, a = s.x + s.width / 2 - o / 2)), a <= e.x && (a = e.x, n = s.y + s.height - l), a + o >= e.x + e.width && (a = Math.max(e.x, e.x + e.width - o), o = e.x + e.width - a, t && (l = o / t), n = s.y + s.height - l), l < y && (l = y, t && (o = l * t, a = s.x + s.width / 2 - o / 2), n = s.y + s.height - l), o < y && (o = y, t && (l = o / t, a = s.x + s.width / 2 - o / 2), n = s.y + s.height - l), {
-        x: a,
+    n += r, a -= r, t && (o = a * t);
+    let l = s.x + s.width / 2 - o / 2;
+    return n <= e.y && (n = e.y, a = s.y + s.height - n, t && (o = a * t, l = s.x + s.width / 2 - o / 2)), l <= e.x && (l = e.x, n = s.y + s.height - a), l + o >= e.x + e.width && (l = Math.max(e.x, e.x + e.width - o), o = e.x + e.width - l, t && (a = o / t), n = s.y + s.height - a), a < b && (a = b, t && (o = a * t, l = s.x + s.width / 2 - o / 2), n = s.y + s.height - a), o < b && (o = b, t && (a = o / t, l = s.x + s.width / 2 - o / 2), n = s.y + s.height - a), {
+        x: l,
         y: n,
         width: o,
-        height: l
+        height: a
     }
 }
 
-function To({
+function So({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r] = i, {
         x: n,
         width: o,
-        height: l
+        height: a
     } = s;
-    n += r, o -= r, t && (l = o / t);
-    let a = s.y + s.height / 2 - l / 2;
-    return n <= e.x && (n = e.x, o = s.x + s.width - n, t && (l = o / t, a = s.y + s.height / 2 - l / 2)), a <= e.y && (a = e.y, n = s.x + s.width - o), a + l >= e.y + e.height && (a = Math.max(e.y, e.y + e.height - l), l = e.y + e.height - a, t && (o = l * t), n = s.x + s.width - o), l < y && (l = y, t && (o = l * t), a = s.y + s.height / 2 - l / 2, n = s.x + s.width - o), o < y && (o = y, t && (l = o / t), a = s.y + s.height / 2 - l / 2, n = s.x + s.width - o), {
+    n += r, o -= r, t && (a = o / t);
+    let l = s.y + s.height / 2 - a / 2;
+    return n <= e.x && (n = e.x, o = s.x + s.width - n, t && (a = o / t, l = s.y + s.height / 2 - a / 2)), l <= e.y && (l = e.y, n = s.x + s.width - o), l + a >= e.y + e.height && (l = Math.max(e.y, e.y + e.height - a), a = e.y + e.height - l, t && (o = a * t), n = s.x + s.width - o), a < b && (a = b, t && (o = a * t), l = s.y + s.height / 2 - a / 2, n = s.x + s.width - o), o < b && (o = b, t && (a = o / t), l = s.y + s.height / 2 - a / 2, n = s.x + s.width - o), {
         x: n,
-        y: a,
+        y: l,
         width: o,
-        height: l
+        height: a
     }
 }
 
-function So({
+function $o({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [, r] = i, {
         y: n,
         width: o,
-        height: l
+        height: a
     } = s;
-    l += r, t && (o = l * t);
-    let a = s.x + s.width / 2 - o / 2;
-    return n + l >= e.y + e.height && (l = e.y + e.height - n, t && (o = l * t), a = s.x + s.width / 2 - o / 2), a <= e.x && (a = e.x, n = s.y), a + o >= e.x + e.width && (a = Math.max(e.x, e.x + e.width - o), o = e.x + e.width - a, t && (l = o / t), n = s.y), l < y && (l = y, t && (o = l * t), a = s.x + s.width / 2 - o / 2), o < y && (o = y, t && (l = o / t), a = s.x + s.width / 2 - o / 2), {
-        x: a,
+    a += r, t && (o = a * t);
+    let l = s.x + s.width / 2 - o / 2;
+    return n + a >= e.y + e.height && (a = e.y + e.height - n, t && (o = a * t), l = s.x + s.width / 2 - o / 2), l <= e.x && (l = e.x, n = s.y), l + o >= e.x + e.width && (l = Math.max(e.x, e.x + e.width - o), o = e.x + e.width - l, t && (a = o / t), n = s.y), a < b && (a = b, t && (o = a * t), l = s.x + s.width / 2 - o / 2), o < b && (o = b, t && (a = o / t), l = s.x + s.width / 2 - o / 2), {
+        x: l,
         y: n,
         width: o,
-        height: l
+        height: a
     }
 }
 
-function $o({
+function Io({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r] = i, {
         x: n,
         width: o,
-        height: l
+        height: a
     } = s;
-    o += r, t && (l = o / t);
-    let a = s.y + s.height / 2 - l / 2;
-    return n + o >= e.x + e.width && (o = e.x + e.width - n, t && (l = o / t), a = s.y + s.height / 2 - l / 2), a <= e.y && (a = e.y, n = s.x), a + l >= e.y + e.height && (a = Math.max(e.y, e.y + e.height - l), l = e.y + e.height - a, t && (o = l * t), n = s.x), l < y && (l = y, t && (o = l * t), a = s.y + s.height / 2 - l / 2), o < y && (o = y, t && (l = o / t), a = s.y + s.height / 2 - l / 2), {
+    o += r, t && (a = o / t);
+    let l = s.y + s.height / 2 - a / 2;
+    return n + o >= e.x + e.width && (o = e.x + e.width - n, t && (a = o / t), l = s.y + s.height / 2 - a / 2), l <= e.y && (l = e.y, n = s.x), l + a >= e.y + e.height && (l = Math.max(e.y, e.y + e.height - a), a = e.y + e.height - l, t && (o = a * t), n = s.x), a < b && (a = b, t && (o = a * t), l = s.y + s.height / 2 - a / 2), o < b && (o = b, t && (a = o / t), l = s.y + s.height / 2 - a / 2), {
         x: n,
-        y: a,
+        y: l,
         width: o,
-        height: l
+        height: a
     }
 }
 
-function Io({
+function ko({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r, n] = i, {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     } = s;
-    return o + r < e.x && (r = e.x - o), l + n < e.y && (n = e.y - l), o += r, a -= r, l += n, c -= n, t && Math.abs(a / c) > t ? (n = a / t - c, c += n, l -= n, l <= e.y && (c = c - (e.y - l), a = c * t, o = s.x + s.width - a, l = e.y)) : t && (r = c * t - a, a = a + r, o -= r, o <= e.x && (a = a - (e.x - o), c = a / t, o = e.x, l = s.y + s.height - c)), c < y && (c = y, t && (a = c * t), o = s.x + s.width - a, l = s.y + s.height - c), a < y && (a = y, t && (c = a / t), o = s.x + s.width - a, l = s.y + s.height - c), {
+    return o + r < e.x && (r = e.x - o), a + n < e.y && (n = e.y - a), o += r, l -= r, a += n, c -= n, t && Math.abs(l / c) > t ? (n = l / t - c, c += n, a -= n, a <= e.y && (c = c - (e.y - a), l = c * t, o = s.x + s.width - l, a = e.y)) : t && (r = c * t - l, l = l + r, o -= r, o <= e.x && (l = l - (e.x - o), c = l / t, o = e.x, a = s.y + s.height - c)), c < b && (c = b, t && (l = c * t), o = s.x + s.width - l, a = s.y + s.height - c), l < b && (l = b, t && (c = l / t), o = s.x + s.width - l, a = s.y + s.height - c), {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     }
 }
 
-function ko({
+function Oo({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r, n] = i, {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     } = s;
-    return o + a + r > e.x + e.width && (r = e.x + e.width - o - a), l + n < e.y && (n = e.y - l), a += r, l += n, c -= n, t && Math.abs(a / c) > t ? (n = a / t - c, c += n, l -= n, l <= e.y && (c = c - (e.y - l), a = c * t, o = s.x, l = e.y)) : t && (r = c * t - a, a += r, o + a >= e.x + e.width && (a = e.x + e.width - o, c = a / t, o = e.x + e.width - a, l = s.y + s.height - c)), c < y && (c = y, t && (a = c * t), l = s.y + s.height - c), a < y && (a = y, t && (c = a / t), l = s.y + s.height - c), {
+    return o + l + r > e.x + e.width && (r = e.x + e.width - o - l), a + n < e.y && (n = e.y - a), l += r, a += n, c -= n, t && Math.abs(l / c) > t ? (n = l / t - c, c += n, a -= n, a <= e.y && (c = c - (e.y - a), l = c * t, o = s.x, a = e.y)) : t && (r = c * t - l, l += r, o + l >= e.x + e.width && (l = e.x + e.width - o, c = l / t, o = e.x + e.width - l, a = s.y + s.height - c)), c < b && (c = b, t && (l = c * t), a = s.y + s.height - c), l < b && (l = b, t && (c = l / t), a = s.y + s.height - c), {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     }
 }
 
-function Oo({
+function Po({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r, n] = i, {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     } = s;
-    return o + r < e.x && (r = e.x - o), l + c + n > e.y + e.height && (n = e.y + e.height - l - c), o += r, a -= r, c += n, t && Math.abs(a / c) > t ? (n = a / t - c, c += n, l + c >= e.y + e.height && (c = e.y + e.height - l, a = c * t, o = s.x + s.width - a, l = e.y + e.height - c)) : t && (r = c * t - a, a += r, o -= r, o <= e.x && (a = a - (e.x - o), c = a / t, o = e.x, l = s.y)), c < y && (c = y, t && (a = c * t), o = s.x + s.width - a), a < y && (a = y, t && (c = a / t), o = s.x + s.width - a), {
+    return o + r < e.x && (r = e.x - o), a + c + n > e.y + e.height && (n = e.y + e.height - a - c), o += r, l -= r, c += n, t && Math.abs(l / c) > t ? (n = l / t - c, c += n, a + c >= e.y + e.height && (c = e.y + e.height - a, l = c * t, o = s.x + s.width - l, a = e.y + e.height - c)) : t && (r = c * t - l, l += r, o -= r, o <= e.x && (l = l - (e.x - o), c = l / t, o = e.x, a = s.y)), c < b && (c = b, t && (l = c * t), o = s.x + s.width - l), l < b && (l = b, t && (c = l / t), o = s.x + s.width - l), {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     }
 }
 
-function Po({
+function Lo({
     rect: s,
     delta: i,
     aspectRatio: t,
     imageBox: e
 }) {
     let [r, n] = i, {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     } = s;
-    return o + a + r > e.x + e.width && (r = e.x + e.width - o - a), l + c + n > e.y + e.height && (n = e.y + e.height - l - c), a += r, c += n, t && Math.abs(a / c) > t ? (n = a / t - c, c += n, l + c >= e.y + e.height && (c = e.y + e.height - l, a = c * t, o = s.x, l = e.y + e.height - c)) : t && (r = c * t - a, a += r, o + a >= e.x + e.width && (a = e.x + e.width - o, c = a / t, o = e.x + e.width - a, l = s.y)), c < y && (c = y, t && (a = c * t)), a < y && (a = y, t && (c = a / t)), {
+    return o + l + r > e.x + e.width && (r = e.x + e.width - o - l), a + c + n > e.y + e.height && (n = e.y + e.height - a - c), l += r, c += n, t && Math.abs(l / c) > t ? (n = l / t - c, c += n, a + c >= e.y + e.height && (c = e.y + e.height - a, l = c * t, o = s.x, a = e.y + e.height - c)) : t && (r = c * t - l, l += r, o + l >= e.x + e.width && (l = e.x + e.width - o, c = l / t, o = e.x + e.width - l, a = s.y)), c < b && (c = b, t && (l = c * t)), l < b && (l = b, t && (c = l / t)), {
         x: o,
-        y: l,
-        width: a,
+        y: a,
+        width: l,
         height: c
     }
 }
 
 function Xs({
     direction: s,
     ...i
 }) {
     switch (s) {
         case "n":
-            return xo(i);
-        case "w":
             return To(i);
-        case "s":
+        case "w":
             return So(i);
-        case "e":
+        case "s":
             return $o(i);
-        case "nw":
+        case "e":
             return Io(i);
-        case "ne":
+        case "nw":
             return ko(i);
-        case "sw":
+        case "ne":
             return Oo(i);
-        case "se":
+        case "sw":
             return Po(i);
+        case "se":
+            return Lo(i);
         default:
             return i.rect
     }
 }
 
 function qs(s, [i, t]) {
     return s.x <= i && i <= s.x + s.width && s.y <= t && t <= s.y + s.height
@@ -3080,15 +3080,15 @@
     return s.x >= i.x && s.y >= i.y && s.x + s.width <= i.x + i.width && s.y + s.height <= i.y + i.height
 }
 
 function Ys(s, i) {
     return Math.abs(s.width / s.height - i) < .1
 }
 
-function jt({
+function Vt({
     width: s,
     height: i
 }, t) {
     let e = t / 90 % 2 !== 0;
     return {
         width: e ? i : s,
         height: e ? s : i
@@ -3096,87 +3096,87 @@
 }
 
 function Js(s, i, t) {
     let e = s / i,
         r, n;
     e > t ? (r = Math.round(i * t), n = i) : (r = s, n = Math.round(s / t));
     let o = Math.round((s - r) / 2),
-        l = Math.round((i - n) / 2);
-    return o + r > s && (r = s - o), l + n > i && (n = i - l), {
+        a = Math.round((i - n) / 2);
+    return o + r > s && (r = s - o), a + n > i && (n = i - a), {
         x: o,
-        y: l,
+        y: a,
         width: r,
         height: n
     }
 }
 
-function Ht(s) {
+function jt(s) {
     return {
         x: Math.round(s.x),
         y: Math.round(s.y),
         width: Math.round(s.width),
         height: Math.round(s.height)
     }
 }
 
 function vt(s, i, t) {
     return Math.min(Math.max(s, i), t)
 }
-var Fe = s => {
+var De = s => {
     if (!s) return [];
     let [i, t] = s.split(":").map(Number);
     if (!Number.isFinite(i) || !Number.isFinite(t)) {
         console.error(`Invalid crop preset: ${s}`);
         return
     }
     return [{
         type: "aspect-ratio",
         width: i,
         height: t
     }]
 };
-var Y = Object.freeze({
+var G = Object.freeze({
     LOCAL: "local",
     DROP_AREA: "drop-area",
     URL_TAB: "url-tab",
     CAMERA: "camera",
     EXTERNAL: "external",
     API: "js-api"
 });
 var Zs = s => s ? s.split(",").map(i => i.trim()) : [],
-    Pt = s => s ? s.join(",") : "";
-var Be = "blocks",
-    ze = "0.33.2";
+    Ht = s => s ? s.join(",") : "";
+var Fe = "blocks",
+    Be = "0.36.0";
 
 function Qs(s) {
-    return Ni({
+    return Di({
         ...s,
-        libraryName: Be,
-        libraryVersion: ze
+        libraryName: Fe,
+        libraryVersion: Be
     })
 }
 var tr = ({
         type: s,
         message: i,
         ...t
     }) => ({
         type: s,
         message: i,
         ...t
     }),
-    Lt = tr,
-    Ve = tr;
+    Pt = tr,
+    ze = tr;
 var er = s => {
         if (typeof s != "string" || !s) return "";
         let i = s.trim();
         return i.startsWith("-/") ? i = i.slice(2) : i.startsWith("/") && (i = i.slice(1)), i.endsWith("/") && (i = i.slice(0, i.length - 1)), i
     },
-    je = (...s) => s.filter(i => typeof i == "string" && i).map(i => er(i)).join("/-/"),
+    Ve = (...s) => s.filter(i => typeof i == "string" && i).map(i => er(i)).join("/-/"),
     R = (...s) => {
-        let i = je(...s);
+        let i = Ve(...s);
         return i ? `-/${i}/` : ""
     };
 
 function ir(s) {
     let i = new URL(s),
         t = i.pathname + i.search + i.hash,
         e = t.lastIndexOf("http"),
@@ -3201,76 +3201,76 @@
         e = t.pathname.indexOf("/-/");
     return e === -1 ? [] : t.pathname.substring(e).split("/-/").filter(Boolean).map(n => er(n))
 }
 
 function nr(s) {
     let i = new URL(s),
         t = ir(s),
-        e = or(t) ? lr(t).pathname : t;
+        e = or(t) ? ar(t).pathname : t;
     return i.pathname = i.pathname.replace(e, ""), i.search = "", i.hash = "", i.toString()
 }
 
 function or(s) {
     return s.startsWith("http")
 }
 
-function lr(s) {
+function ar(s) {
     let i = new URL(s);
     return {
         pathname: i.origin + i.pathname || "",
         search: i.search || "",
         hash: i.hash || ""
     }
 }
 var O = (s, i, t) => {
         let e = new URL(nr(s));
         if (t = t || ir(s), e.pathname.startsWith("//") && (e.pathname = e.pathname.replace("//", "/")), or(t)) {
-            let r = lr(t);
+            let r = ar(t);
             e.pathname = e.pathname + (i || "") + (r.pathname || ""), e.search = r.search, e.hash = r.hash
         } else e.pathname = e.pathname + (i || "") + (t || "");
         return e.toString()
     },
     Ct = (s, i) => {
         let t = new URL(s);
         return t.pathname = i + "/", t.toString()
     };
 var M = (s, i = ",") => s.trim().split(i).map(t => t.trim()).filter(t => t.length > 0);
-var ie = ["image/*", "image/heif", "image/heif-sequence", "image/heic", "image/heic-sequence", "image/avif", "image/avif-sequence", ".heif", ".heifs", ".heic", ".heics", ".avif", ".avifs"],
-    Xi = s => s ? s.filter(i => typeof i == "string").map(i => M(i)).flat() : [],
-    qi = (s, i) => i.some(t => t.endsWith("*") ? (t = t.replace("*", ""), s.startsWith(t)) : s === t),
-    ar = (s, i) => i.some(t => t.startsWith(".") ? s.toLowerCase().endsWith(t.toLowerCase()) : !1),
-    se = s => {
+var je = ["image/*", "image/heif", "image/heif-sequence", "image/heic", "image/heic-sequence", "image/avif", "image/avif-sequence", ".heif", ".heifs", ".heic", ".heics", ".avif", ".avifs"],
+    qi = s => s ? s.filter(i => typeof i == "string").map(i => M(i)).flat() : [],
+    Ki = (s, i) => i.some(t => t.endsWith("*") ? (t = t.replace("*", ""), s.startsWith(t)) : s === t),
+    lr = (s, i) => i.some(t => t.startsWith(".") ? s.toLowerCase().endsWith(t.toLowerCase()) : !1),
+    ie = s => {
         let i = s == null ? void 0 : s.type;
-        return i ? qi(i, ie) : !1
+        return i ? Ki(i, je) : !1
     };
 var it = 1e3,
-    Ut = Object.freeze({
+    Lt = Object.freeze({
         AUTO: "auto",
         BYTE: "byte",
         KB: "kb",
         MB: "mb",
         GB: "gb",
         TB: "tb",
         PB: "pb"
     }),
-    re = s => Math.ceil(s * 100) / 100,
-    cr = (s, i = Ut.AUTO) => {
-        let t = i === Ut.AUTO;
-        if (i === Ut.BYTE || t && s < it ** 1) {
-            let e = $e("en-US", s),
+    se = s => Math.ceil(s * 100) / 100,
+    cr = (s, i = Lt.AUTO) => {
+        let t = i === Lt.AUTO;
+        if (i === Lt.BYTE || t && s < it ** 1) {
+            let e = Se("en-US", s),
                 r = {
                     one: "byte",
                     other: "bytes"
                 } [e];
             return `${s} ${r}`
         }
-        return i === Ut.KB || t && s < it ** 2 ? `${re(s/it**1)} KB` : i === Ut.MB || t && s < it ** 3 ? `${re(s/it**2)} MB` : i === Ut.GB || t && s < it ** 4 ? `${re(s/it**3)} GB` : i === Ut.TB || t && s < it ** 5 ? `${re(s/it**4)} TB` : `${re(s/it**5)} PB`
+        return i === Lt.KB || t && s < it ** 2 ? `${se(s/it**1)} KB` : i === Lt.MB || t && s < it ** 3 ? `${se(s/it**2)} MB` : i === Lt.GB || t && s < it ** 4 ? `${se(s/it**3)} GB` : i === Lt.TB || t && s < it ** 5 ? `${se(s/it**4)} TB` : `${se(s/it**5)} PB`
     };
 var hr = "[Typed State] Wrong property name: ",
-    Lo = "[Typed State] Wrong property type: ",
+    Uo = "[Typed State] Wrong property type: ",
     He = class {
         constructor(i, t) {
             this.__typedSchema = i, this.__ctxId = t || Yt.generate(), this.__schema = Object.keys(i).reduce((e, r) => (e[r] = i[r].value, e), {}), this.__data = E.registerCtx(this.__schema, this.__ctxId)
         }
         get uid() {
             return this.__ctxId
         }
@@ -3280,15 +3280,15 @@
                 return
             }
             let e = this.__typedSchema[i];
             if ((t == null ? void 0 : t.constructor) === e.type || t instanceof e.type || e.nullable && t === null) {
                 this.__data.pub(i, t);
                 return
             }
-            console.warn(Lo + i)
+            console.warn(Uo + i)
         }
         setMultipleValues(i) {
             for (let t in i) this.setValue(t, i[t])
         }
         getValue(i) {
             if (!this.__typedSchema.hasOwnProperty(i)) {
                 console.warn(hr + i);
@@ -3395,15 +3395,15 @@
         let e = JSON.stringify(t);
         if (i.has(e)) return i.get(e);
         let r = s(...t);
         return i.set(e, r), r
     }
 };
 
-function Uo(s) {
+function Ro(s) {
     let i = !1;
     return setTimeout(() => {
         i = !0
     }, 0), e => (...r) => (i && It(s), e(...r))
 }
 
 function dr(s) {
@@ -3422,20 +3422,20 @@
             allEntries: () => s.getOutputData(),
             successEntries: () => t.allEntries.filter(r => r.status === "success"),
             failedEntries: () => t.allEntries.filter(r => r.status === "failed"),
             uploadingEntries: () => t.allEntries.filter(r => r.status === "uploading"),
             idleEntries: () => t.allEntries.filter(r => r.status === "idle")
         },
         t = {},
-        e = Uo("You're trying to access the OutputCollectionState asynchronously. In this case, the data you retrieve will be newer than it was when the OutputCollectionState was created or when the event was dispatched. If you want to retain the state at a specific moment in time, you should use the spread operator like this: `{...outputCollectionState}` or `{...e.detail}`");
+        e = Ro("You're trying to access the OutputCollectionState asynchronously. In this case, the data you retrieve will be newer than it was when the OutputCollectionState was created or when the event was dispatched. If you want to retain the state at a specific moment in time, you should use the spread operator like this: `{...outputCollectionState}` or `{...e.detail}`");
     for (let [r, n] of Object.entries(i)) {
         let o = r,
-            a = ur(e(n));
+            l = ur(e(n));
         Object.defineProperty(t, o, {
-            get: a,
+            get: l,
             enumerable: !0
         })
     }
     return t
 }
 var pr = Object.freeze({
     file: {
@@ -3536,71 +3536,72 @@
         nullable: !0
     },
     isRemoved: {
         type: Boolean,
         value: !1
     }
 });
-var We = (s, i) => {
-    let t, e, r, n = (...o) => {
-        t ? (clearTimeout(e), e = setTimeout(() => {
-            Date.now() - r >= i && (s(...o), r = Date.now())
-        }, Math.max(i - (Date.now() - r), 0))) : (s(...o), r = Date.now(), t = !0)
-    };
-    return Object.defineProperty(n, "cancel", {
-        configurable: !1,
-        writable: !1,
-        enumerable: !1,
-        value: () => {
-            clearTimeout(e)
+var Mo = /[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}/i,
+    No = new RegExp(`^/?(${Mo.source})(?:/(-/(?:[^/]+/)+)?([^/]*))?$`, "i"),
+    fr = ({
+        url: s,
+        cdnBase: i
+    }) => {
+        let t = new URL(i),
+            e = new URL(s);
+        if (t.host !== e.host) return null;
+        let [, r, n, o] = No.exec(e.pathname);
+        return {
+            uuid: r,
+            cdnUrlModifiers: n || "",
+            filename: o || null
         }
-    }), n
-};
-var T = class s extends g {
+    };
+var A = class s extends g {
     constructor() {
         super(...arguments);
         h(this, "couldBeCtxOwner", !1);
         h(this, "isCtxOwner", !1);
-        h(this, "init$", Ne(this));
+        h(this, "init$", Me(this));
         h(this, "__initialUploadMetadata", null);
         h(this, "_fileValidators", [this._validateIsImage.bind(this), this._validateFileType.bind(this), this._validateMaxSizeLimit.bind(this), this._validateUploadError.bind(this)]);
         h(this, "_collectionValidators", [t => {
             let e = t.size,
                 r = this.cfg.multiple ? this.cfg.multipleMin : 0,
                 n = this.cfg.multiple ? this.cfg.multipleMax : 1;
             if (r && e < r) {
                 let o = this.l10n("files-count-limit-error-too-few", {
                     min: r,
                     max: n,
                     total: e
                 });
-                return Ve({
+                return ze({
                     type: "TOO_FEW_FILES",
                     message: o,
                     total: e,
                     min: r,
                     max: n
                 })
             }
             if (n && e > n) {
                 let o = this.l10n("files-count-limit-error-too-many", {
                     min: r,
                     max: n,
                     total: e
                 });
-                return Ve({
+                return ze({
                     type: "TOO_MANY_FILES",
                     message: o,
                     total: e,
                     min: r,
                     max: n
                 })
             }
         }, t => {
-            if (t.items().some(e => t.readProp(e, "errors").length > 0)) return Ve({
+            if (t.items().some(e => t.readProp(e, "errors").length > 0)) return ze({
                 type: "SOME_FILES_HAS_ERRORS",
                 message: this.l10n("some-files-were-not-uploaded")
             })
         }]);
         h(this, "uploadAll", () => {
             let t = this.uploadCollection.items().filter(e => {
                 let r = this.uploadCollection.read(e);
@@ -3635,62 +3636,62 @@
                 r = [...new Set(Object.entries(t).filter(([n]) => ["uploadError", "fileInfo"].includes(n)).map(([, n]) => [...n]).flat())];
             if (r.length > 0 && setTimeout(() => {
                     this._runFileValidators(r)
                 }), t.uploadProgress) {
                 for (let n of t.uploadProgress) {
                     let {
                         isUploading: o,
-                        silent: l
+                        silent: a
                     } = E.getCtx(n).store;
-                    o && !l && this.emit($.FILE_UPLOAD_PROGRESS, this.getOutputItem(n))
+                    o && !a && this.emit($.FILE_UPLOAD_PROGRESS, this.getOutputItem(n))
                 }
                 this._flushCommonUploadProgress()
             }
             if (t.isUploading)
                 for (let n of t.isUploading) {
                     let {
                         isUploading: o,
-                        silent: l
+                        silent: a
                     } = E.getCtx(n).store;
-                    o && !l && this.emit($.FILE_UPLOAD_START, this.getOutputItem(n))
+                    o && !a && this.emit($.FILE_UPLOAD_START, this.getOutputItem(n))
                 }
             if (t.fileInfo) {
-                for (let l of t.fileInfo) {
+                for (let a of t.fileInfo) {
                     let {
-                        fileInfo: a,
+                        fileInfo: l,
                         silent: c
-                    } = E.getCtx(l).store;
-                    a && !c && this.emit($.FILE_UPLOAD_SUCCESS, this.getOutputItem(l))
+                    } = E.getCtx(a).store;
+                    l && !c && this.emit($.FILE_UPLOAD_SUCCESS, this.getOutputItem(a))
                 }
                 this.cfg.cropPreset && this.setInitialCrop();
-                let n = e.findItems(l => !!l.getValue("fileInfo"));
-                e.findItems(l => l.getValue("errors").length > 0).length === 0 && e.size === n.length && this.emit($.COMMON_UPLOAD_SUCCESS, this.getOutputCollectionState())
+                let n = e.findItems(a => !!a.getValue("fileInfo"));
+                e.findItems(a => a.getValue("errors").length > 0).length === 0 && e.size === n.length && this.emit($.COMMON_UPLOAD_SUCCESS, this.getOutputCollectionState())
             }
             if (t.errors)
                 for (let n of t.errors) {
                     let {
                         errors: o
                     } = E.getCtx(n).store;
                     o.length > 0 && (this.emit($.FILE_UPLOAD_FAILED, this.getOutputItem(n)), this.emit($.COMMON_UPLOAD_FAILED, () => this.getOutputCollectionState(), {
                         debounce: !0
                     }))
                 }
             t.cdnUrl && ([...t.cdnUrl].filter(o => {
-                var l;
-                return !!((l = this.uploadCollection.read(o)) != null && l.getValue("cdnUrl"))
+                var a;
+                return !!((a = this.uploadCollection.read(o)) != null && a.getValue("cdnUrl"))
             }).forEach(o => {
                 this.emit($.FILE_URL_CHANGED, this.getOutputItem(o))
             }), this.$["*groupInfo"] = null)
         });
         h(this, "_flushCommonUploadProgress", () => {
             let t = 0,
                 r = [...this.$["*uploadTrigger"]].filter(o => !!this.uploadCollection.read(o));
             r.forEach(o => {
-                let l = this.uploadCollection.readProp(o, "uploadProgress");
-                t += l
+                let a = this.uploadCollection.readProp(o, "uploadProgress");
+                t += a
             });
             let n = r.length ? Math.round(t / r.length) : 0;
             this.$["*commonProgress"] !== n && (this.$["*commonProgress"] = n, this.emit($.COMMON_UPLOAD_PROGRESS, this.getOutputCollectionState()))
         })
     }
     setUploadMetadata(t) {
         It("setUploadMetadata is deprecated. Use `metadata` instance property on `lr-config` block instead. See migration guide: https://uploadcare.com/docs/file-uploader/migration-to-0.25.0/"), this.connectedOnce ? this.$["*uploadMetadata"] = t : this.__initialUploadMetadata = t
@@ -3725,87 +3726,117 @@
         fileName: r,
         source: n
     } = {}) {
         let o = this.uploadCollection.add({
             externalUrl: t,
             fileName: r != null ? r : null,
             silent: e != null ? e : !1,
-            source: n != null ? n : Y.API
+            source: n != null ? n : G.API
         });
         return this.getOutputItem(o)
     }
     addFileFromUuid(t, {
         silent: e,
         fileName: r,
         source: n
     } = {}) {
         let o = this.uploadCollection.add({
             uuid: t,
             fileName: r != null ? r : null,
             silent: e != null ? e : !1,
-            source: n != null ? n : Y.API
+            source: n != null ? n : G.API
         });
         return this.getOutputItem(o)
     }
+    addFileFromCdnUrl(t, {
+        silent: e,
+        fileName: r,
+        source: n
+    } = {}) {
+        var l;
+        let o = fr({
+            url: t,
+            cdnBase: this.cfg.cdnCname
+        });
+        if (!o) throw new Error("Invalid CDN URL");
+        let a = this.uploadCollection.add({
+            uuid: o.uuid,
+            cdnUrl: t,
+            cdnUrlModifiers: o.cdnUrlModifiers,
+            fileName: (l = r != null ? r : o.filename) != null ? l : null,
+            silent: e != null ? e : !1,
+            source: n != null ? n : G.API
+        });
+        return this.getOutputItem(a)
+    }
     addFileFromObject(t, {
         silent: e,
         fileName: r,
         source: n,
         fullPath: o
     } = {}) {
-        let l = this.uploadCollection.add({
+        let a = this.uploadCollection.add({
             file: t,
-            isImage: se(t),
+            isImage: ie(t),
             mimeType: t.type,
             fileName: r != null ? r : t.name,
             fileSize: t.size,
             silent: e != null ? e : !1,
-            source: n != null ? n : Y.API,
+            source: n != null ? n : G.API,
             fullPath: o != null ? o : null
         });
-        return this.getOutputItem(l)
+        return this.getOutputItem(a)
     }
     addFiles(t) {
         return console.warn("`addFiles` method is deprecated. Please use `addFileFromObject`, `addFileFromUrl` or `addFileFromUuid` instead."), t.map(e => {
             let r = this.uploadCollection.add({
                 file: e,
-                isImage: se(e),
+                isImage: ie(e),
                 mimeType: e.type,
                 fileName: e.name,
                 fileSize: e.size
             });
             return this.getOutputItem(r)
         })
     }
+    removeFileByInternalId(t) {
+        if (!this.uploadCollection.read(t)) throw new Error(`File with internalId ${t} not found`);
+        this.uploadCollection.remove(t)
+    }
+    removeAllFiles() {
+        this.uploadCollection.clearAll()
+    }
     openSystemDialog(t = {}) {
         var r;
-        let e = Pt(Xi([(r = this.cfg.accept) != null ? r : "", ...this.cfg.imgOnly ? ie : []]));
-        this.cfg.accept && this.cfg.imgOnly && console.warn("There could be a mistake.\nBoth `accept` and `imgOnly` parameters are set.\nThe value of `accept` will be concatenated with the internal image mime types list."), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.multiple = this.cfg.multiple, t.captureCamera ? (this.fileInput.capture = "", this.fileInput.accept = Pt(ie)) : this.fileInput.accept = e, this.fileInput.dispatchEvent(new MouseEvent("click")), this.fileInput.onchange = () => {
+        let e = Ht(qi([(r = this.cfg.accept) != null ? r : "", ...this.cfg.imgOnly ? je : []]));
+        this.cfg.accept && this.cfg.imgOnly && console.warn("There could be a mistake.\nBoth `accept` and `imgOnly` parameters are set.\nThe value of `accept` will be concatenated with the internal image mime types list."), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.multiple = this.cfg.multiple, t.captureCamera ? (this.fileInput.capture = this.cfg.cameraCapture, this.fileInput.accept = "image/*") : this.fileInput.accept = e, this.fileInput.dispatchEvent(new MouseEvent("click")), this.fileInput.onchange = () => {
             [...this.fileInput.files].forEach(n => this.addFileFromObject(n, {
-                source: Y.LOCAL
+                source: t.captureCamera ? G.CAMERA : G.LOCAL
             })), this.$["*currentActivity"] = g.activities.UPLOAD_LIST, this.setOrAddState("*modalActive", !0), this.fileInput.value = "", this.fileInput = null
         }
     }
     get sourceList() {
         let t = [];
         return this.cfg.sourceList && (t = M(this.cfg.sourceList)), t
     }
     initFlow(t = !1) {
         var e;
         if (this.uploadCollection.size > 0 && !t) this.set$({
             "*currentActivity": g.activities.UPLOAD_LIST
         }), this.setOrAddState("*modalActive", !0);
         else if (((e = this.sourceList) == null ? void 0 : e.length) === 1) {
             let r = this.sourceList[0];
-            r === "local" ? (this.$["*currentActivity"] = g.activities.UPLOAD_LIST, this == null || this.openSystemDialog()) : (Object.values(s.extSrcList).includes(r) ? this.set$({
-                "*currentActivityParams": {
-                    externalSourceType: r
-                },
-                "*currentActivity": g.activities.EXTERNAL
-            }) : this.$["*currentActivity"] = r, this.setOrAddState("*modalActive", !0))
+            if (r === "local") {
+                this.$["*currentActivity"] = g.activities.UPLOAD_LIST, this == null || this.openSystemDialog();
+                return
+            }
+            let n = this.$["*blocksRegistry"],
+                o = l => "type" in l && l.type === r,
+                a = [...n].find(o);
+            a == null || a.activate(), this.$["*currentActivity"] && this.setOrAddState("*modalActive", !0)
         } else this.set$({
             "*currentActivity": g.activities.START_FROM
         }), this.setOrAddState("*modalActive", !0)
     }
     doneFlow() {
         this.set$({
             "*currentActivity": this.doneActivity,
@@ -3814,70 +3845,70 @@
     }
     get uploadCollection() {
         return this.$["*uploadCollection"]
     }
     _validateFileType(t) {
         let e = this.cfg.imgOnly,
             r = this.cfg.accept,
-            n = Xi([...e ? ie : [], r]);
+            n = qi([...e ? je : [], r]);
         if (!n.length) return;
         let o = t.mimeType,
-            l = t.name;
-        if (!o || !l) return;
-        let a = qi(o, n),
-            c = ar(l, n);
-        if (!a && !c) return Lt({
+            a = t.name;
+        if (!o || !a) return;
+        let l = Ki(o, n),
+            c = lr(a, n);
+        if (!l && !c) return Pt({
             type: "FORBIDDEN_FILE_TYPE",
             message: this.l10n("file-type-not-allowed"),
             entry: t
         })
     }
     _validateMaxSizeLimit(t) {
         let e = this.cfg.maxLocalFileSizeBytes,
             r = t.size;
-        if (e && r && r > e) return Lt({
+        if (e && r && r > e) return Pt({
             type: "FILE_SIZE_EXCEEDED",
             message: this.l10n("files-max-size-limit-error", {
                 maxFileSize: cr(e)
             }),
             entry: t
         })
     }
     _validateUploadError(t, e) {
         let r = e == null ? void 0 : e.getValue("uploadError");
         if (r) {
-            if (r instanceof D) return Lt({
+            if (r instanceof F) return Pt({
                 type: "UPLOAD_ERROR",
                 message: r.message,
                 entry: t,
                 error: r
             });
-            if (r instanceof Ft) return Lt({
+            if (r instanceof Dt) return Pt({
                 type: "NETWORK_ERROR",
                 message: r.message,
                 entry: t,
                 error: r
             });
             {
                 let n = r instanceof Error ? r : new Error("Unknown error", {
                     cause: r
                 });
-                return Lt({
+                return Pt({
                     type: "UNKNOWN_ERROR",
                     message: n.message,
                     entry: t,
                     error: n
                 })
             }
         }
     }
     _validateIsImage(t) {
         let e = this.cfg.imgOnly,
             r = t.isImage;
-        if (!(!e || r) && !(!t.fileInfo && t.externalUrl) && !(!t.fileInfo && !t.mimeType)) return Lt({
+        if (!(!e || r) && !(!t.fileInfo && t.externalUrl) && !(!t.fileInfo && !t.mimeType)) return Pt({
             type: "NOT_AN_IMAGE",
             message: this.l10n("images-only-accepted"),
             entry: t
         })
     }
     _runFileValidatorsForEntry(t) {
         let e = this.getOutputItem(t.uid),
@@ -3904,45 +3935,45 @@
         }
         this.$["*collectionErrors"] = e, e.length > 0 && this.emit($.COMMON_UPLOAD_FAILED, () => this.getOutputCollectionState(), {
             debounce: !0
         })
     }
     async _createGroup(t) {
         let e = this.getUploadClientOptions(),
-            r = t.allEntries.map(a => a.uuid + (a.cdnUrlModifiers ? `/${a.cdnUrlModifiers}` : "")),
+            r = t.allEntries.map(l => l.uuid + (l.cdnUrlModifiers ? `/${l.cdnUrlModifiers}` : "")),
             n = new AbortController,
             o = await Fs(r, {
                 ...e,
                 signal: n.signal
             });
         if (this.$["*collectionState"] !== t) {
             n.abort();
             return
         }
         this.$["*groupInfo"] = o;
-        let l = this.getOutputCollectionState();
-        this.emit($.GROUP_CREATED, l), this.emit($.CHANGE, () => this.getOutputCollectionState(), {
+        let a = this.getOutputCollectionState();
+        this.emit($.GROUP_CREATED, a), this.emit($.CHANGE, () => this.getOutputCollectionState(), {
             debounce: !0
-        }), this.$["*collectionState"] = l
+        }), this.$["*collectionState"] = a
     }
     setInitialCrop() {
-        let t = Fe(this.cfg.cropPreset);
+        let t = De(this.cfg.cropPreset);
         if (t) {
             let [e] = t, r = this.uploadCollection.findItems(n => {
                 var o;
                 return n.getValue("fileInfo") && n.getValue("isImage") && !((o = n.getValue("cdnUrlModifiers")) != null && o.includes("/crop/"))
             }).map(n => this.uploadCollection.read(n));
             for (let n of r) {
                 let o = n.getValue("fileInfo"),
                     {
-                        width: l,
-                        height: a
+                        width: a,
+                        height: l
                     } = o.imageInfo,
                     c = e.width / e.height,
-                    u = Js(l, a, c),
+                    u = Js(a, l, c),
                     d = R(`crop/${u.width}x${u.height}/${u.x},${u.y}`, "preview");
                 n.setMultipleValues({
                     cdnUrlModifiers: d,
                     cdnUrl: O(n.getValue("cdnUrl"), d)
                 }), this.uploadCollection.size === 1 && this.cfg.useCloudImageEditor && this.hasBlockInCtx(p => p.activityType === g.activities.CLOUD_IMG_EDIT) && (this.$["*focusedEntry"] = n, this.$["*currentActivity"] = g.activities.CLOUD_IMG_EDIT)
             }
         }
@@ -3972,33 +4003,33 @@
             maxConcurrentRequests: this.cfg.multipartMaxConcurrentRequests,
             multipartMaxAttempts: this.cfg.multipartMaxAttempts,
             checkForUrlDuplicates: !!this.cfg.checkForUrlDuplicates,
             saveUrlForRecurrentUploads: !!this.cfg.saveUrlForRecurrentUploads
         }
     }
     getOutputItem(t) {
-        var l, a, c, u, d, p, m, f, _, b;
+        var a, l, c, u, d, p, m, f, _, y;
         let e = E.getCtx(t).store,
             r = e.fileInfo,
             n = e.isRemoved ? "removed" : e.errors.length > 0 ? "failed" : e.fileInfo ? "success" : e.isUploading ? "uploading" : "idle";
         return {
-            uuid: (a = (l = r == null ? void 0 : r.uuid) != null ? l : e.uuid) != null ? a : null,
+            uuid: (l = (a = r == null ? void 0 : r.uuid) != null ? a : e.uuid) != null ? l : null,
             internalId: t,
             name: (c = r == null ? void 0 : r.originalFilename) != null ? c : e.fileName,
             size: (u = r == null ? void 0 : r.size) != null ? u : e.fileSize,
             isImage: (d = r == null ? void 0 : r.isImage) != null ? d : e.isImage,
             mimeType: (p = r == null ? void 0 : r.mimeType) != null ? p : e.mimeType,
             file: e.file,
             externalUrl: e.externalUrl,
             cdnUrlModifiers: e.cdnUrlModifiers,
             cdnUrl: (f = (m = e.cdnUrl) != null ? m : r == null ? void 0 : r.cdnUrl) != null ? f : null,
             fullPath: e.fullPath,
             uploadProgress: e.uploadProgress,
             fileInfo: r != null ? r : null,
-            metadata: (b = (_ = e.metadata) != null ? _ : r == null ? void 0 : r.metadata) != null ? b : null,
+            metadata: (y = (_ = e.metadata) != null ? _ : r == null ? void 0 : r.metadata) != null ? y : null,
             isSuccess: n === "success",
             isUploading: n === "uploading",
             isFailed: n === "failed",
             isRemoved: n === "removed",
             errors: e.errors,
             status: n
         }
@@ -4006,216 +4037,217 @@
     getOutputData(t) {
         return (t ? this.uploadCollection.findItems(t) : this.uploadCollection.items()).map(n => this.getOutputItem(n))
     }
     getOutputCollectionState() {
         return dr(this)
     }
 };
-T.extSrcList = Object.freeze({
+A.extSrcList = Object.freeze({
     FACEBOOK: "facebook",
     DROPBOX: "dropbox",
     GDRIVE: "gdrive",
     GPHOTOS: "gphotos",
     INSTAGRAM: "instagram",
     FLICKR: "flickr",
     VK: "vk",
     EVERNOTE: "evernote",
     BOX: "box",
     ONEDRIVE: "onedrive",
     HUDDLE: "huddle"
 });
-T.sourceTypes = Object.freeze({
+A.sourceTypes = Object.freeze({
     LOCAL: "local",
     URL: "url",
     CAMERA: "camera",
     DRAW: "draw",
-    ...T.extSrcList
+    ...A.extSrcList
 });
-var X = Object.freeze({
+var q = Object.freeze({
         brightness: 0,
         exposure: 0,
         gamma: 100,
         contrast: 0,
         saturation: 0,
         vibrance: 0,
         warmth: 0,
         enhance: 0,
         filter: 0,
         rotate: 0,
         mirror: !1,
         flip: !1,
         crop: void 0
     }),
-    mr = ["enhance", "brightness", "exposure", "gamma", "contrast", "saturation", "vibrance", "warmth", "filter", "mirror", "flip", "rotate", "crop"];
+    gr = ["enhance", "brightness", "exposure", "gamma", "contrast", "saturation", "vibrance", "warmth", "filter", "mirror", "flip", "rotate", "crop"];
 
-function Ro(s, i) {
+function Do(s, i) {
     if (typeof i == "number") {
         let t = i;
-        return X[s] !== t ? `${s}/${t}` : ""
+        return q[s] !== t ? `${s}/${t}` : ""
     }
     if (typeof i == "boolean") {
         let t = i;
-        return X[s] !== t ? `${s}` : ""
+        return q[s] !== t ? `${s}` : ""
     }
     if (s === "filter" && i) {
         let {
             name: t,
             amount: e
         } = i;
-        return X.filter === e ? "" : `${s}/${t}/${e}`
+        return q.filter === e ? "" : `${s}/${t}/${e}`
     }
     if (s === "crop" && i) {
         let {
             dimensions: t,
             coords: e
         } = i;
         return `${s}/${t.join("x")}/${e.join(",")}`
     }
     return ""
 }
 
 function wt(s) {
-    return je(...mr.filter(i => typeof s[i] != "undefined" && s[i] !== null).map(i => {
+    return Ve(...gr.filter(i => typeof s[i] != "undefined" && s[i] !== null).map(i => {
         let t = s[i];
-        return Ro(i, t)
+        return Do(i, t)
     }).filter(i => !!i))
 }
-var Xe = je("format/auto", "progressive/yes"),
+var We = Ve("format/auto", "progressive/yes"),
     ft = ([s]) => typeof s != "undefined" ? Number(s) : void 0,
-    fr = () => !0,
-    Mo = ([s, i]) => ({
+    mr = () => !0,
+    Fo = ([s, i]) => ({
         name: s,
         amount: typeof i != "undefined" ? Number(i) : 100
     }),
-    No = ([s, i]) => {
+    Bo = ([s, i]) => {
         if (!/\d+x\d+/.test(s) || !/\d+,\d+/.test(i)) throw new Error("Crop by aspect ratio, percentage or alignment shortcuts is not supported.");
         return {
             dimensions: M(s, "x").map(Number),
             coords: M(i).map(Number)
         }
     },
-    Do = Object.freeze({
+    zo = Object.freeze({
         enhance: ft,
         brightness: ft,
         exposure: ft,
         gamma: ft,
         contrast: ft,
         saturation: ft,
         vibrance: ft,
         warmth: ft,
-        filter: Mo,
-        mirror: fr,
-        flip: fr,
+        filter: Fo,
+        mirror: mr,
+        flip: mr,
         rotate: ft,
-        crop: No
+        crop: Bo
     });
 
-function gr(s) {
+function _r(s) {
     let i = {};
     for (let t of s) {
         let [e, ...r] = t.split("/");
-        if (!mr.includes(e)) continue;
+        if (!gr.includes(e)) continue;
         let n = e,
-            o = Do[n];
+            o = zo[n];
         try {
-            let l = o(r);
-            i[n] = l
-        } catch (l) {
-            console.warn([`Failed to parse URL operation "${t}". It will be ignored.`, l instanceof Error ? `Error message: "${l.message}"` : l, "If you need this functionality, please feel free to open an issue at https://github.com/uploadcare/blocks/issues/new"].join(` `))
+            let a = o(r);
+            i[n] = a
+        } catch (a) {
+            console.warn([`Failed to parse URL operation "${t}". It will be ignored.`, a instanceof Error ? `Error message: "${a.message}"` : a, "If you need this functionality, please feel free to open an issue at https://github.com/uploadcare/blocks/issues/new"].join(` `))
         }
     }
     return i
 }
 var P = Object.freeze({
         CROP: "crop",
         TUNING: "tuning",
         FILTERS: "filters"
     }),
-    G = [P.CROP, P.TUNING, P.FILTERS],
-    _r = ["brightness", "exposure", "gamma", "contrast", "saturation", "vibrance", "warmth", "enhance"],
-    br = ["adaris", "briaril", "calarel", "carris", "cynarel", "cyren", "elmet", "elonni", "enzana", "erydark", "fenralan", "ferand", "galen", "gavin", "gethriel", "iorill", "iothari", "iselva", "jadis", "lavra", "misiara", "namala", "nerion", "nethari", "pamaya", "sarnar", "sedis", "sewen", "sorahel", "sorlen", "tarian", "thellassan", "varriel", "varven", "vevera", "virkas", "yedis", "yllara", "zatvel", "zevcen"],
-    yr = ["rotate", "mirror", "flip"],
+    W = [P.CROP, P.TUNING, P.FILTERS],
+    br = ["brightness", "exposure", "gamma", "contrast", "saturation", "vibrance", "warmth", "enhance"],
+    yr = ["adaris", "briaril", "calarel", "carris", "cynarel", "cyren", "elmet", "elonni", "enzana", "erydark", "fenralan", "ferand", "galen", "gavin", "gethriel", "iorill", "iothari", "iselva", "jadis", "lavra", "misiara", "namala", "nerion", "nethari", "pamaya", "sarnar", "sedis", "sewen", "sorahel", "sorlen", "tarian", "thellassan", "varriel", "varven", "vevera", "virkas", "yedis", "yllara", "zatvel", "zevcen"],
+    vr = ["rotate", "mirror", "flip"],
     st = Object.freeze({
         brightness: {
-            zero: X.brightness,
+            zero: q.brightness,
             range: [-100, 100],
             keypointsNumber: 2
         },
         exposure: {
-            zero: X.exposure,
+            zero: q.exposure,
             range: [-500, 500],
             keypointsNumber: 2
         },
         gamma: {
-            zero: X.gamma,
+            zero: q.gamma,
             range: [0, 1e3],
             keypointsNumber: 2
         },
         contrast: {
-            zero: X.contrast,
+            zero: q.contrast,
             range: [-100, 500],
             keypointsNumber: 2
         },
         saturation: {
-            zero: X.saturation,
+            zero: q.saturation,
             range: [-100, 500],
             keypointsNumber: 1
         },
         vibrance: {
-            zero: X.vibrance,
+            zero: q.vibrance,
             range: [-100, 500],
             keypointsNumber: 1
         },
         warmth: {
-            zero: X.warmth,
+            zero: q.warmth,
             range: [-100, 100],
             keypointsNumber: 1
         },
         enhance: {
-            zero: X.enhance,
+            zero: q.enhance,
             range: [0, 100],
             keypointsNumber: 1
         },
         filter: {
-            zero: X.filter,
+            zero: q.filter,
             range: [0, 100],
             keypointsNumber: 1
         }
     });
-var Fo = "https://ucarecdn.com",
-    Bo = "https://upload.uploadcare.com",
-    zo = "https://social.uploadcare.com",
-    At = {
+var Vo = "https://ucarecdn.com",
+    jo = "https://upload.uploadcare.com",
+    Ho = "https://social.uploadcare.com",
+    Et = {
         pubkey: "",
         multiple: !0,
         multipleMin: 0,
         multipleMax: Number.MAX_SAFE_INTEGER,
         confirmUpload: !1,
         imgOnly: !1,
         accept: "",
         externalSourcesPreferredTypes: "",
         store: "auto",
         cameraMirror: !1,
+        cameraCapture: "",
         sourceList: "local, url, camera, dropbox, gdrive",
-        cloudImageEditorTabs: Pt(G),
+        cloudImageEditorTabs: Ht(W),
         maxLocalFileSizeBytes: 0,
         thumbSize: 76,
         showEmptyList: !1,
         useLocalImageEditor: !1,
         useCloudImageEditor: !0,
         removeCopyright: !1,
         cropPreset: "",
         imageShrink: "",
         modalScrollLock: !0,
         modalBackdropStrokes: !1,
         sourceListWrap: !0,
         remoteTabSessionKey: "",
-        cdnCname: Fo,
-        baseUrl: Bo,
-        socialBaseUrl: zo,
+        cdnCname: Vo,
+        baseUrl: jo,
+        socialBaseUrl: Ho,
         secureSignature: "",
         secureExpire: "",
         secureDeliveryProxy: "",
         retryThrottledRequestMaxTimes: 1,
         multipartMinFileSize: 26214400,
         multipartChunkSize: 5242880,
         maxConcurrentRequests: 10,
@@ -4224,136 +4256,142 @@
         checkForUrlDuplicates: !1,
         saveUrlForRecurrentUploads: !1,
         groupOutput: !1,
         userAgentIntegration: "",
         debug: !1,
         metadata: null
     };
-var B = s => String(s),
+var D = s => String(s),
     rt = s => {
         let i = Number(s);
         if (Number.isNaN(i)) throw new Error(`Invalid number: "${s}"`);
         return i
     },
     I = s => {
         if (typeof s == "undefined" || s === null) return !1;
         if (typeof s == "boolean") return s;
         if (s === "true" || s === "") return !0;
         if (s === "false") return !1;
         throw new Error(`Invalid boolean: "${s}"`)
     },
-    Vo = s => s === "auto" ? s : I(s),
-    jo = {
-        pubkey: B,
+    Go = s => s === "auto" ? s : I(s),
+    Wo = s => {
+        let i = D(s);
+        if (i !== "user" && i !== "environment" && i !== "") throw new Error(`Invalid "cameraCapture" value: "${i}"`);
+        return i
+    },
+    Xo = {
+        pubkey: D,
         multiple: I,
         multipleMin: rt,
         multipleMax: rt,
         confirmUpload: I,
         imgOnly: I,
-        accept: B,
-        externalSourcesPreferredTypes: B,
-        store: Vo,
+        accept: D,
+        externalSourcesPreferredTypes: D,
+        store: Go,
         cameraMirror: I,
-        sourceList: B,
+        cameraCapture: Wo,
+        sourceList: D,
         maxLocalFileSizeBytes: rt,
         thumbSize: rt,
         showEmptyList: I,
         useLocalImageEditor: I,
         useCloudImageEditor: I,
-        cloudImageEditorTabs: B,
+        cloudImageEditorTabs: D,
         removeCopyright: I,
-        cropPreset: B,
-        imageShrink: B,
+        cropPreset: D,
+        imageShrink: D,
         modalScrollLock: I,
         modalBackdropStrokes: I,
         sourceListWrap: I,
-        remoteTabSessionKey: B,
-        cdnCname: B,
-        baseUrl: B,
-        socialBaseUrl: B,
-        secureSignature: B,
-        secureExpire: B,
-        secureDeliveryProxy: B,
+        remoteTabSessionKey: D,
+        cdnCname: D,
+        baseUrl: D,
+        socialBaseUrl: D,
+        secureSignature: D,
+        secureExpire: D,
+        secureDeliveryProxy: D,
         retryThrottledRequestMaxTimes: rt,
         multipartMinFileSize: rt,
         multipartChunkSize: rt,
         maxConcurrentRequests: rt,
         multipartMaxConcurrentRequests: rt,
         multipartMaxAttempts: rt,
         checkForUrlDuplicates: I,
         saveUrlForRecurrentUploads: I,
         groupOutput: I,
-        userAgentIntegration: B,
+        userAgentIntegration: D,
         debug: I
     },
-    vr = (s, i) => {
+    Cr = (s, i) => {
         if (!(typeof i == "undefined" || i === null)) try {
-            return jo[s](i)
+            return Xo[s](i)
         } catch (t) {
-            return console.error(`Invalid value for config key "${s}".`, t), At[s]
+            return console.error(`Invalid value for config key "${s}".`, t), Et[s]
         }
     };
-var ne = Object.keys(At),
-    Ho = ["metadata"],
-    Go = s => Ho.includes(s),
-    qe = ne.filter(s => !Go(s)),
-    Wo = {
-        ...Object.fromEntries(qe.map(s => [ht(s), s])),
-        ...Object.fromEntries(qe.map(s => [s.toLowerCase(), s]))
-    },
-    Xo = {
-        ...Object.fromEntries(ne.map(s => [ht(s), F(s)])),
-        ...Object.fromEntries(ne.map(s => [s.toLowerCase(), F(s)]))
+var re = Object.keys(Et),
+    qo = ["metadata"],
+    Ko = s => qo.includes(s),
+    Xe = re.filter(s => !Ko(s)),
+    Yo = {
+        ...Object.fromEntries(Xe.map(s => [ht(s), s])),
+        ...Object.fromEntries(Xe.map(s => [s.toLowerCase(), s]))
+    },
+    Jo = {
+        ...Object.fromEntries(re.map(s => [ht(s), B(s)])),
+        ...Object.fromEntries(re.map(s => [s.toLowerCase(), B(s)]))
     },
-    Ke = class extends w {
+    qe = class extends C {
         constructor() {
             super();
             h(this, "requireCtxName", !0);
             h(this, "_debugPrint", k(() => {
                 let t = Object.create(null);
-                for (let e of ne) t[e] = this.$[F(e)];
+                for (let e of re) t[e] = this.$[B(e)];
                 this.debugPrint("config", t)
             }, 0));
             this.init$ = {
                 ...this.init$,
-                ...Object.fromEntries(Object.entries(At).map(([t, e]) => [F(t), e]))
+                ...Object.fromEntries(Object.entries(Et).map(([t, e]) => [B(t), e]))
             }
         }
         initCallback() {
             super.initCallback();
             let t = this;
-            for (let e of qe) this.sub(F(e), r => {
-                r !== At[e] && (t[e] = r)
+            for (let e of Xe) this.sub(B(e), r => {
+                r !== Et[e] && (t[e] = r)
             }, !1);
-            for (let e of ne) {
+            for (let e of re) {
                 let r = "__" + e;
                 t[r] = t[e], Object.defineProperty(this, e, {
                     set: n => {
-                        if (t[r] = n, qe.includes(e)) {
+                        if (t[r] = n, Xe.includes(e)) {
                             let o = [...new Set([ht(e), e.toLowerCase()])];
-                            for (let l of o) typeof n == "undefined" || n === null ? this.removeAttribute(l) : this.setAttribute(l, n.toString())
+                            for (let a of o) typeof n == "undefined" || n === null ? this.removeAttribute(a) : this.setAttribute(a, n.toString())
                         }
-                        this.$[F(e)] !== n && (typeof n == "undefined" || n === null ? this.$[F(e)] = At[e] : this.$[F(e)] = n)
+                        this.$[B(e)] !== n && (typeof n == "undefined" || n === null ? this.$[B(e)] = Et[e] : this.$[B(e)] = n)
                     },
-                    get: () => this.$[F(e)]
+                    get: () => this.$[B(e)]
                 }), typeof t[e] != "undefined" && t[e] !== null && (t[e] = t[r])
             }
         }
         attributeChangedCallback(t, e, r) {
             if (e === r) return;
-            let n = Wo[t],
-                o = vr(n, r),
-                l = o != null ? o : At[n],
-                a = this;
-            a[n] = l
+            let n = Yo[t],
+                o = Cr(n, r),
+                a = o != null ? o : Et[n],
+                l = this;
+            l[n] = a
         }
     };
-Ke.bindAttributes(Xo);
-var qo = Ke;
-var oe = class extends w {
+qe.bindAttributes(Jo);
+var Zo = qe;
+var ne = class extends C {
     constructor() {
         super(...arguments);
         h(this, "init$", {
             ...this.init$,
             name: "",
             path: "",
             size: "24",
@@ -4369,34 +4407,34 @@
             if (!t) return;
             t.trimStart().startsWith("<") ? (this.setAttribute("raw", ""), this.ref.svg.innerHTML = t) : (this.removeAttribute("raw"), this.ref.svg.innerHTML = `<path fill-rule="evenodd" d="${t}"></path>`)
         }), this.sub("size", t => {
             this.$.viewBox = `0 0 ${t} ${t}`
         })
     }
 };
-oe.template = `<svg ref="svg" xmlns="http://www.w3.org/2000/svg" set="@viewBox: viewBox; @height: size; @width: size"></svg>`;
-oe.bindAttributes({
+ne.template = `<svg ref="svg" xmlns="http://www.w3.org/2000/svg" set="@viewBox: viewBox; @height: size; @width: size"></svg>`;
+ne.bindAttributes({
     name: "name",
     size: "size"
 });
-var Cr = s => [...new Set(s)];
-var wr = s => Object.entries(s).filter(([i, t]) => t !== void 0 && t !== "").map(([i, t]) => i === "cdn-operations" || i === "analytics" ? t : `${i}/${t}`);
-var Ko = "https://ucarecdn.com",
-    le = Object.freeze({
+var wr = s => [...new Set(s)];
+var Er = s => Object.entries(s).filter(([i, t]) => t !== void 0 && t !== "").map(([i, t]) => i === "cdn-operations" || i === "analytics" ? t : `${i}/${t}`);
+var Qo = "https://ucarecdn.com",
+    oe = Object.freeze({
         "dev-mode": {},
         pubkey: {},
         uuid: {},
         src: {},
         lazy: {
             default: 1
         },
         intersection: {},
         breakpoints: {},
         "cdn-cname": {
-            default: Ko
+            default: Qo
         },
         "proxy-cname": {},
         "secure-delivery-proxy": {},
         "hi-res-support": {
             default: 1
         },
         "ultra-res-support": {},
@@ -4406,47 +4444,47 @@
         quality: {},
         "is-background-for": {},
         "is-preview-blur": {
             default: 1
         }
     });
 var Gt = "--lr-img-",
-    Ki = "unresolved";
-var Yi = !window.location.host.trim() || window.location.host.includes(":") || window.location.hostname.includes("localhost"),
-    Ji = 3e3,
-    Zi = 5e3,
-    Qi = Object.freeze({
+    Yi = "unresolved";
+var Ji = !window.location.host.trim() || window.location.host.includes(":") || window.location.hostname.includes("localhost"),
+    Zi = 3e3,
+    Qi = 5e3,
+    ts = Object.freeze({
         PREVIEW: "PREVIEW",
         MAIN: "MAIN"
     });
-var Er = Object.create(null),
+var xr = Object.create(null),
     Ar;
-for (let s in le) Er[Gt + s] = ((Ar = le[s]) == null ? void 0 : Ar.default) || "";
-var Ye = class extends Dt {
+for (let s in oe) xr[Gt + s] = ((Ar = oe[s]) == null ? void 0 : Ar.default) || "";
+var Ke = class extends Nt {
     constructor() {
         super(...arguments);
-        h(this, "cssInit$", Er)
+        h(this, "cssInit$", xr)
     }
     $$(t) {
         return this.$[Gt + t]
     }
     set$$(t) {
         for (let e in t) this.$[Gt + e] = t[e]
     }
     sub$$(t, e) {
         this.sub(Gt + t, r => {
             r === null || r === "" || e(r)
         })
     }
     analyticsParams() {
-        return `-/@clib/${Be}/${ze}/lr-img/`
+        return `-/@clib/${Fe}/${Be}/lr-img/`
     }
     initAttributes(t) {
         [...this.attributes].forEach(e => {
-            le[e.name] || t.setAttribute(e.name, e.value)
+            oe[e.name] || t.setAttribute(e.name, e.value)
         })
     }
     initIntersection(t, e) {
         let r = {
             root: null,
             rootMargin: "0px"
         };
@@ -4458,55 +4496,55 @@
     }
     destroyCallback() {
         super.destroyCallback(), this._isnObserver && (this._observed.forEach(t => {
             this._isnObserver.unobserve(t)
         }), this._isnObserver = null), E.deleteCtx(this)
     }
     static get observedAttributes() {
-        return Object.keys(le)
+        return Object.keys(oe)
     }
     attributeChangedCallback(t, e, r) {
         window.setTimeout(() => {
             this.$[Gt + t] = r
         })
     }
 };
-var Qe = class extends Ye {
+var Ze = class extends Ke {
     constructor() {
         super(...arguments);
         h(this, "_img", new Image);
         h(this, "_imgPreview", new Image)
     }
     _fmtAbs(t) {
-        return !t.includes("//") && !Yi && (t = new URL(t, document.baseURI).href), t
+        return !t.includes("//") && !Ji && (t = new URL(t, document.baseURI).href), t
     }
     _validateSize(t) {
         if ((t == null ? void 0 : t.trim()) !== "") {
             let e = t.match(/\d+/)[0],
                 r = t.match(/[a-zA-Z]+/)[0],
                 n = parseInt(e, 10);
-            if (Number(n) > Zi && this.hasFormatJPG) return Zi + r;
-            if (Number(n) > Ji && !this.hasFormatJPG) return Ji + r
+            if (Number(n) > Qi && this.hasFormatJPG) return Qi + r;
+            if (Number(n) > Zi && !this.hasFormatJPG) return Zi + r
         }
         return t
     }
     _getCdnModifiers(t, e) {
         let r = {
             format: this.$$("format"),
             quality: this.$$("quality"),
             resize: this._validateSize(t),
             blur: e,
             "cdn-operations": this.$$("cdn-operations"),
             analytics: this.analyticsParams()
         };
-        return R(...wr(r))
+        return R(...Er(r))
     }
     _getUrlBase(t = "", e = "") {
         if (this.$$("src").startsWith("data:") || this.$$("src").startsWith("blob:")) return this.$$("src");
-        if (Yi && this.$$("src") && !this.$$("src").includes("//")) return this._proxyUrl(this.$$("src"));
+        if (Ji && this.$$("src") && !this.$$("src").includes("//")) return this._proxyUrl(this.$$("src"));
         let r = this._getCdnModifiers(t, e);
         if (this.$$("src").startsWith(this.$$("cdn-cname"))) return O(this.$$("src"), r);
         if (this.$$("cdn-cname") && this.$$("uuid")) return this._proxyUrl(O(Ct(this.$$("cdn-cname"), this.$$("uuid")), r));
         if (this.$$("uuid")) return this._proxyUrl(O(Ct(this.$$("cdn-cname"), this.$$("uuid")), r));
         if (this.$$("proxy-cname")) return this._proxyUrl(O(this.$$("proxy-cname"), r, this._fmtAbs(this.$$("src"))));
         if (this.$$("pubkey")) return this._proxyUrl(O(`https://${this.$$("pubkey")}.ucr.io/`, r, this._fmtAbs(this.$$("src"))))
     }
@@ -4516,16 +4554,16 @@
         }, {
             transform: r => window.encodeURIComponent(r)
         }) : t
     }
     _getElSize(t, e = 1, r = !0) {
         let n = t.getBoundingClientRect(),
             o = e * Math.round(n.width),
-            l = r ? "" : e * Math.round(n.height);
-        return o || l ? `${o||""}x${l||""}` : null
+            a = r ? "" : e * Math.round(n.height);
+        return o || a ? `${o||""}x${a||""}` : null
     }
     _setupEventProxy(t) {
         let e = n => {
                 n.stopPropagation();
                 let o = new Event(n.type, n);
                 this.dispatchEvent(o)
             },
@@ -4535,31 +4573,31 @@
     get img() {
         return this.hasPreviewImage || (this._setupConfigForImage({
             elNode: this._img
         }), this.appendChild(this._img)), this._img
     }
     get currentImg() {
         return this.hasPreviewImage ? {
-            type: Qi.PREVIEW,
+            type: ts.PREVIEW,
             img: this._imgPreview
         } : {
-            type: Qi.MAIN,
+            type: ts.MAIN,
             img: this.img
         }
     }
     get hasPreviewImage() {
         return this.$$("is-preview-blur")
     }
     get bgSelector() {
         return this.$$("is-background-for")
     }
     get breakpoints() {
         if (this.$$("breakpoints")) {
             let t = M(this.$$("breakpoints"));
-            return Cr(t.map(e => parseInt(e, 10)))
+            return wr(t.map(e => parseInt(e, 10)))
         } else return null
     }
     get hasFormatJPG() {
         return this.$$("format").toLowerCase() === "jpeg"
     }
     renderBg(t) {
         let e = new Set;
@@ -4602,16 +4640,16 @@
         src: t,
         srcset: e,
         elNode: r
     }) {
         return new Promise((n, o) => {
             this._setupConfigForImage({
                 elNode: r
-            }), r.setAttribute(Ki, ""), r.addEventListener("load", () => {
-                r.removeAttribute(Ki), n(r)
+            }), r.setAttribute(Yi, ""), r.addEventListener("load", () => {
+                r.removeAttribute(Yi), n(r)
             }), r.addEventListener("error", () => {
                 o(!1)
             }), this._appendURL({
                 elNode: r,
                 src: t,
                 srcset: e
             })
@@ -4650,26 +4688,26 @@
             this.hasPreviewImage && await ((e = this._imgPreview) == null ? void 0 : e.remove()), this.appendChild(this._img)
         }
     }
     init() {
         this.bgSelector ? this.renderBackground() : this.renderImage()
     }
 };
-var ts = class extends Qe {
+var es = class extends Ze {
     initCallback() {
         super.initCallback(), this.sub$$("src", () => {
             this.init()
         }), this.sub$$("uuid", () => {
             this.init()
         }), this.sub$$("lazy", i => {
             !this.$$("is-background-for") && !this.$$("is-preview-blur") && (this.img.loading = i ? "lazy" : "eager")
         })
     }
 };
-var ae = class extends T {
+var ae = class extends A {
     constructor() {
         super();
         h(this, "couldBeCtxOwner", !0);
         this.init$ = {
             ...this.init$,
             "*simpleButtonText": "",
             withDropZone: !0,
@@ -4686,27 +4724,27 @@
         })
     }
 };
 ae.template = `<lr-drop-area set="@disabled: !withDropZone"><button type="button" set="onclick: onClick"><lr-icon name="upload"></lr-icon><span>{{*simpleButtonText}}</span><slot></slot><div class="visual-drop-area"></div></button></lr-drop-area>`;
 ae.bindAttributes({
     dropzone: null
 });
-var ti = class extends g {
+var Qe = class extends g {
     constructor() {
         super(...arguments);
         h(this, "historyTracked", !0);
         h(this, "activityType", "start-from")
     }
     initCallback() {
         super.initCallback(), this.registerActivity(this.activityType)
     }
 };
-ti.template = '<div class="content"><slot></slot></div>';
+Qe.template = '<div class="content"><slot></slot></div>';
 
-function Yo(s) {
+function ta(s) {
     return new Promise(i => {
         typeof window.FileReader != "function" && i(!1);
         try {
             let t = new FileReader;
             t.onerror = () => {
                 i(!0)
             };
@@ -4716,62 +4754,62 @@
             t.onloadend = e, t.onprogress = e, t.readAsDataURL(s)
         } catch {
             i(!1)
         }
     })
 }
 
-function Jo(s, i) {
+function ea(s, i) {
     return new Promise(t => {
         let e = 0,
             r = [],
-            n = l => {
-                l || (console.warn("Unexpectedly received empty content entry", {
+            n = a => {
+                a || (console.warn("Unexpectedly received empty content entry", {
                     scope: "drag-and-drop"
-                }), t(null)), l.isFile ? (e++, l.file(a => {
+                }), t(null)), a.isFile ? (e++, a.file(l => {
                     e--;
-                    let c = new File([a], a.name, {
-                        type: a.type || i
+                    let c = new File([l], l.name, {
+                        type: l.type || i
                     });
                     r.push({
                         type: "file",
                         file: c,
-                        fullPath: l.fullPath
+                        fullPath: a.fullPath
                     }), e === 0 && t(r)
-                })) : l.isDirectory && o(l.createReader())
+                })) : a.isDirectory && o(a.createReader())
             },
-            o = l => {
-                e++, l.readEntries(a => {
+            o = a => {
+                e++, a.readEntries(l => {
                     e--;
-                    for (let c of a) n(c);
+                    for (let c of l) n(c);
                     e === 0 && t(r)
                 })
             };
         n(s)
     })
 }
 
-function xr(s) {
+function Tr(s) {
     let i = [],
         t = [];
     for (let e = 0; e < s.items.length; e++) {
         let r = s.items[e];
         if (r)
             if (r.kind === "file") {
                 let n = r.type;
                 if (typeof r.webkitGetAsEntry == "function" || typeof r.getAsEntry == "function") {
-                    let l = typeof r.webkitGetAsEntry == "function" ? r.webkitGetAsEntry() : r.getAsEntry();
-                    t.push(Jo(l, n).then(a => {
-                        a && i.push(...a)
+                    let a = typeof r.webkitGetAsEntry == "function" ? r.webkitGetAsEntry() : r.getAsEntry();
+                    t.push(ea(a, n).then(l => {
+                        l && i.push(...l)
                     }));
                     continue
                 }
                 let o = r.getAsFile();
-                o && t.push(Yo(o).then(l => {
-                    l || i.push({
+                o && t.push(ta(o).then(a => {
+                    a || i.push({
                         type: "file",
                         file: o
                     })
                 }))
             } else r.kind === "string" && r.type.match("^text/uri-list") && t.push(new Promise(n => {
                 r.getAsString(o => {
                     i.push({
@@ -4785,76 +4823,76 @@
 }
 var z = {
         ACTIVE: 0,
         INACTIVE: 1,
         NEAR: 2,
         OVER: 3
     },
-    Tr = ["focus"],
-    Zo = 100,
-    es = new Map;
+    Sr = ["focus"],
+    ia = 100,
+    is = new Map;
 
-function Qo(s, i) {
+function sa(s, i) {
     let t = Math.max(Math.min(s[0], i.x + i.width), i.x),
         e = Math.max(Math.min(s[1], i.y + i.height), i.y);
     return Math.sqrt((s[0] - t) * (s[0] - t) + (s[1] - e) * (s[1] - e))
 }
 
-function is(s) {
+function ss(s) {
     let i = 0,
         t = document.body,
         e = new Set,
         r = f => e.add(f),
         n = z.INACTIVE,
         o = f => {
             s.shouldIgnore() && f !== z.INACTIVE || (n !== f && e.forEach(_ => _(f)), n = f)
         },
-        l = () => i > 0;
+        a = () => i > 0;
     r(f => s.onChange(f));
-    let a = () => {
+    let l = () => {
             i = 0, o(z.INACTIVE)
         },
         c = () => {
             i += 1, n === z.INACTIVE && o(z.ACTIVE)
         },
         u = () => {
-            i -= 1, l() || o(z.INACTIVE)
+            i -= 1, a() || o(z.INACTIVE)
         },
         d = f => {
             f.preventDefault(), i = 0, o(z.INACTIVE)
         },
         p = f => {
             if (s.shouldIgnore()) return;
-            l() || (i += 1);
+            a() || (i += 1);
             let _ = [f.x, f.y],
-                b = s.element.getBoundingClientRect(),
-                x = Math.floor(Qo(_, b)),
-                v = x < Zo,
-                A = f.composedPath().includes(s.element);
-            es.set(s.element, x);
-            let V = Math.min(...es.values()) === x;
-            A && V ? (f.preventDefault(), o(z.OVER)) : o(v && V ? z.NEAR : z.ACTIVE)
+                y = s.element.getBoundingClientRect(),
+                x = Math.floor(sa(_, y)),
+                T = x < ia,
+                w = f.composedPath().includes(s.element);
+            is.set(s.element, x);
+            let V = Math.min(...is.values()) === x;
+            w && V ? (f.preventDefault(), o(z.OVER)) : o(T && V ? z.NEAR : z.ACTIVE)
         },
         m = async f => {
             if (s.shouldIgnore()) return;
             f.preventDefault();
-            let _ = await xr(f.dataTransfer);
+            let _ = await Tr(f.dataTransfer);
             s.onItems(_), o(z.INACTIVE)
         };
-    return t.addEventListener("drop", d), t.addEventListener("dragleave", u), t.addEventListener("dragenter", c), t.addEventListener("dragover", p), s.element.addEventListener("drop", m), Tr.forEach(f => {
-        window.addEventListener(f, a)
+    return t.addEventListener("drop", d), t.addEventListener("dragleave", u), t.addEventListener("dragenter", c), t.addEventListener("dragover", p), s.element.addEventListener("drop", m), Sr.forEach(f => {
+        window.addEventListener(f, l)
     }), () => {
-        es.delete(s.element), t.removeEventListener("drop", d), t.removeEventListener("dragleave", u), t.removeEventListener("dragenter", c), t.removeEventListener("dragover", p), s.element.removeEventListener("drop", m), Tr.forEach(f => {
-            window.removeEventListener(f, a)
+        is.delete(s.element), t.removeEventListener("drop", d), t.removeEventListener("dragleave", u), t.removeEventListener("dragenter", c), t.removeEventListener("dragover", p), s.element.removeEventListener("drop", m), Sr.forEach(f => {
+            window.removeEventListener(f, l)
         })
     }
 }
-var Sr = "lr-drop-area",
-    Wt = `${Sr}/registry`,
-    ce = class extends T {
+var $r = "lr-drop-area",
+    Wt = `${$r}/registry`,
+    le = class extends A {
         constructor() {
             super(), this.init$ = {
                 ...this.init$,
                 state: z.INACTIVE,
                 withIcon: !1,
                 isClickable: !1,
                 isFullscreen: !1,
@@ -4892,50 +4930,50 @@
                 })
             }), this.defineAccessor("text", t => {
                 typeof t == "string" ? this.set$({
                     text: this.l10n(t) || t
                 }) : this.set$({
                     text: this.l10n("drop-files-here")
                 })
-            }), this._destroyDropzone = is({
+            }), this._destroyDropzone = ss({
                 element: this,
                 shouldIgnore: () => this._shouldIgnore(),
                 onChange: t => {
                     this.$.state = t
                 },
                 onItems: t => {
                     t.length && (t.forEach(e => {
                         e.type === "url" ? this.addFileFromUrl(e.url, {
-                            source: Y.DROP_AREA
+                            source: G.DROP_AREA
                         }) : e.type === "file" && this.addFileFromObject(e.file, {
-                            source: Y.DROP_AREA,
+                            source: G.DROP_AREA,
                             fullPath: e.fullPath
                         })
                     }), this.uploadCollection.size && (this.set$({
                         "*currentActivity": g.activities.UPLOAD_LIST
                     }), this.setOrAddState("*modalActive", !0)))
                 }
             });
             let i = this.ref["content-wrapper"];
-            i && (this._destroyContentWrapperDropzone = is({
+            i && (this._destroyContentWrapperDropzone = ss({
                 element: i,
                 onChange: t => {
                     var r;
                     let e = (r = Object.entries(z).find(([, n]) => n === t)) == null ? void 0 : r[0].toLowerCase();
                     e && i.setAttribute("drag-state", e)
                 },
                 onItems: () => {},
                 shouldIgnore: () => this._shouldIgnore()
             })), this.sub("state", t => {
                 var r;
                 let e = (r = Object.entries(z).find(([, n]) => n === t)) == null ? void 0 : r[0].toLowerCase();
                 e && this.setAttribute("drag-state", e)
             }), this.subConfigValue("sourceList", t => {
                 let e = M(t);
-                this.$.isEnabled = e.includes(T.sourceTypes.LOCAL), this.$.isVisible = this.$.isEnabled || !this.querySelector("[data-default-slot]")
+                this.$.isEnabled = e.includes(A.sourceTypes.LOCAL), this.$.isVisible = this.$.isEnabled || !this.querySelector("[data-default-slot]")
             }), this.sub("isVisible", t => {
                 this.toggleAttribute("hidden", !t)
             }), this.sub("isClickable", t => {
                 this.toggleAttribute("clickable", t)
             }), this.$.isClickable && (this._onAreaClicked = () => {
                 this.openSystemDialog()
             }, this.addEventListener("click", this._onAreaClicked))
@@ -4949,61 +4987,60 @@
                 e = this.uploadCollection.size;
             return !(i && t && e >= t || !i && e > 0)
         }
         destroyCallback() {
             var t, e;
             super.destroyCallback();
             let i = this.$[Wt];
-            i && (i.delete(this), i.size === 0 && E.deleteCtx(Sr)), (t = this._destroyDropzone) == null || t.call(this), (e = this._destroyContentWrapperDropzone) == null || e.call(this), this._onAreaClicked && this.removeEventListener("click", this._onAreaClicked)
+            i && (i.delete(this), i.size === 0 && E.deleteCtx($r)), (t = this._destroyDropzone) == null || t.call(this), (e = this._destroyContentWrapperDropzone) == null || e.call(this), this._onAreaClicked && this.removeEventListener("click", this._onAreaClicked)
         }
     };
-ce.template = `<slot><div data-default-slot hidden></div><div ref="content-wrapper" class="content-wrapper" set="@hidden: !isVisible"><div class="icon-container" set="@hidden: !withIcon"><lr-icon name="default"></lr-icon><lr-icon name="arrow-down"></lr-icon></div><span class="text">{{text}}</span></div></slot>`;
-ce.bindAttributes({
+le.template = `<slot><div data-default-slot hidden></div><div ref="content-wrapper" class="content-wrapper" set="@hidden: !isVisible"><div class="icon-container" set="@hidden: !withIcon"><lr-icon name="default"></lr-icon><lr-icon name="arrow-down"></lr-icon></div><span class="text">{{text}}</span></div></slot>`;
+le.bindAttributes({
     "with-icon": null,
     clickable: null,
     text: null,
     fullscreen: null,
     disabled: null
 });
-var tl = "src-type-",
-    he = class extends T {
+var ra = "src-type-",
+    ce = class extends A {
         constructor() {
-            super(...arguments);
+            super();
             h(this, "couldBeCtxOwner", !0);
+            h(this, "type");
             h(this, "_registeredTypes", {});
-            h(this, "init$", {
+            this.init$ = {
                 ...this.init$,
                 iconName: "default"
-            })
+            }
         }
         initTypes() {
             this.registerType({
-                type: T.sourceTypes.LOCAL,
-                onClick: () => {
-                    this.openSystemDialog()
-                }
+                type: A.sourceTypes.LOCAL,
+                activate: () => (this.openSystemDialog(), !1)
             }), this.registerType({
-                type: T.sourceTypes.URL,
+                type: A.sourceTypes.URL,
                 activity: g.activities.URL,
                 textKey: "from-url"
             }), this.registerType({
-                type: T.sourceTypes.CAMERA,
+                type: A.sourceTypes.CAMERA,
                 activity: g.activities.CAMERA,
-                onClick: () => {
-                    var e = document.createElement("input").capture !== void 0;
-                    return e && this.openSystemDialog({
+                activate: () => {
+                    let t = "capture" in document.createElement("input");
+                    return t && this.openSystemDialog({
                         captureCamera: !0
-                    }), !e
+                    }), !t
                 }
             }), this.registerType({
                 type: "draw",
                 activity: g.activities.DRAW,
                 icon: "edit-draw"
             });
-            for (let t of Object.values(T.extSrcList)) this.registerType({
+            for (let t of Object.values(A.extSrcList)) this.registerType({
                 type: t,
                 activity: g.activities.EXTERNAL,
                 activityParams: {
                     externalSourceType: t
                 }
             })
         }
@@ -5014,436 +5051,444 @@
         }
         registerType(t) {
             this._registeredTypes[t.type] = t
         }
         getType(t) {
             return this._registeredTypes[t]
         }
+        activate() {
+            if (!this.type) return;
+            let t = this._registeredTypes[this.type],
+                {
+                    activity: e,
+                    activate: r,
+                    activityParams: n = {}
+                } = t;
+            (r ? r() : !!e) && this.set$({
+                "*currentActivityParams": n,
+                "*currentActivity": e
+            })
+        }
         applyType(t) {
             let e = this._registeredTypes[t];
             if (!e) {
                 console.warn("Unsupported source type: " + t);
                 return
             }
             let {
                 textKey: r = t,
-                icon: n = t,
-                activity: o,
-                onClick: l,
-                activityParams: a = {}
+                icon: n = t
             } = e;
-            this.applyL10nKey("src-type", `${tl}${r}`), this.$.iconName = n, this.onclick = c => {
-                (l ? l(c) : !!o) && this.set$({
-                    "*currentActivityParams": a,
-                    "*currentActivity": o
-                })
+            this.applyL10nKey("src-type", `${ra}${r}`), this.$.iconName = n, this.onclick = () => {
+                this.activate()
             }
         }
     };
-he.template = `<lr-icon set="@name: iconName"></lr-icon><div class="txt" l10n="src-type"></div>`;
-he.bindAttributes({
+ce.template = `<lr-icon set="@name: iconName"></lr-icon><div class="txt" l10n="src-type"></div>`;
+ce.bindAttributes({
     type: null
 });
-var ss = class extends w {
+var rs = class extends C {
     initCallback() {
         super.initCallback(), this.subConfigValue("sourceList", i => {
             let t = M(i),
                 e = "";
             t.forEach(r => {
                 e += `<lr-source-btn type="${r}"></lr-source-btn>`
             }), this.cfg.sourceListWrap ? this.innerHTML = e : this.outerHTML = e
         })
     }
 };
-var el = [1, 3],
-    il = [192, 193, 194, 195, 197, 198, 199, 201, 202, 203, 205, 206, 207],
-    $r = {
+var ei = () => {
+        let s = [];
+        return {
+            stack: s,
+            promiseReadJpegChunks: t => new Promise((e, r) => {
+                let n = 2,
+                    o = (c, u) => {
+                        let d = new FileReader;
+                        d.addEventListener("load", () => {
+                            u(new DataView(d.result))
+                        }), d.addEventListener("error", p => {
+                            r(`Reader error: ${p}`)
+                        }), d.readAsArrayBuffer(c)
+                    },
+                    a = () => o(t.slice(n, n + 128), c => {
+                        let u, d, p;
+                        for (u = d = 0, p = c.byteLength; p >= 0 ? d < p : d > p; u = p >= 0 ? ++d : --d)
+                            if (c.getUint8(u) === 255) {
+                                n += u;
+                                break
+                            } l()
+                    }),
+                    l = () => {
+                        let c = n;
+                        return o(t.slice(n, n += 4), u => {
+                            if (u.byteLength !== 4 || u.getUint8(0) !== 255) {
+                                r("Corrupted");
+                                return
+                            }
+                            let d = u.getUint8(1);
+                            if (d === 218) {
+                                e(!0);
+                                return
+                            }
+                            let p = u.getUint16(2) - 2;
+                            return o(t.slice(n, n += p), m => {
+                                if (m.byteLength !== p) {
+                                    r("Corrupted");
+                                    return
+                                }
+                                s.push({
+                                    startPos: c,
+                                    length: p,
+                                    marker: d,
+                                    view: m
+                                }), a()
+                            })
+                        })
+                    };
+                FileReader && DataView || r("Not Support"), o(t.slice(0, 2), c => {
+                    c.getUint16(0) !== 65496 && r("Not jpeg"), a()
+                })
+            })
+        }
+    },
+    na = async s => {
+        let i = [],
+            {
+                promiseReadJpegChunks: t,
+                stack: e
+            } = ei();
+        return await t(s), e.forEach(({
+            marker: r,
+            view: n
+        }) => {
+            r === 226 && n.getUint32(0) === 1229144927 && n.getUint32(4) === 1347571526 && n.getUint32(8) === 1229735168 && i.push(n)
+        }), i
+    }, kr = async (s, i, t) => {
+        {
+            let e = [],
+                r = [],
+                {
+                    promiseReadJpegChunks: n,
+                    stack: o
+                } = ei();
+            await n(s), o.forEach(c => {
+                if (c.marker === i) return e.push(c.startPos), r.push(c.length)
+            });
+            let a = [s.slice(0, 2)];
+            for (let c of t) {
+                let u = new DataView(new ArrayBuffer(4));
+                u.setUint16(0, 65280 + i), u.setUint16(2, c.byteLength + 2), a.push(u.buffer), a.push(c)
+            }
+            let l = 2;
+            for (let c = 0; c < e.length; c++) e[c] > l && a.push(s.slice(l, e[c])), l = e[c] + r[c] + 4;
+            return a.push(s.slice(l, s.size)), new Blob(a, {
+                type: s.type
+            })
+        }
+    };
+var Or = (s, i) => kr(s, 226, i.map(t => t.buffer)),
+    oa = async s => {
+        try {
+            return await Or(s, [])
+        } catch (i) {
+            throw new Error(`Failed to strip ICC profile: ${i}`)
+        }
+    }, aa = (s, i, t) => new Promise((e, r) => {
+        let n = o => {
+            if (!o) {
+                r("Failed to convert canvas to blob");
+                return
+            }
+            e(o)
+        };
+        s.toBlob(n, i, t), s.width = s.height = 1
+    }), he = () => {
+        let s = document.createElement("canvas"),
+            i = s.getContext("2d");
+        return {
+            canvas: s,
+            ctx: i
+        }
+    }, la = s => {
+        let {
+            ctx: t,
+            canvas: e
+        } = he();
+        e.width = e.height = 50, t.drawImage(s, 0, 0, 50, 50);
+        let r = t.getImageData(0, 0, 50, 50).data;
+        e.width = e.height = 1;
+        for (let n = 3; n < r.length; n += 4)
+            if (r[n] < 254) return !0;
+        return !1
+    }, ca = async s => {
+        let i = null,
+            {
+                promiseReadJpegChunks: t,
+                stack: e
+            } = ei();
+        return await t(s), e.forEach(({
+            marker: r,
+            view: n
+        }) => {
+            if (!i && r === 225 && n.byteLength >= 14 && n.getUint32(0) === 1165519206 && n.getUint16(4) === 0) {
+                i = n;
+                return
+            }
+        }), i
+    }, ha = "data:image/jpg;base64,/9j/4AAQSkZJRgABAQEASABIAAD/4QA6RXhpZgAATU0AKgAAAAgAAwESAAMAAAABAAYAAAEoAAMAAAABAAIAAAITAAMAAAABAAEAAAAAAAD/2wBDAP//////////////////////////////////////////////////////////////////////////////////////wAALCAABAAIBASIA/8QAJgABAAAAAAAAAAAAAAAAAAAAAxABAAAAAAAAAAAAAAAAAAAAAP/aAAgBAQAAPwBH/9k=", ti, ua = () => new Promise(s => {
+        if (ti !== void 0) s(ti);
+        else {
+            let i = new Image;
+            i.addEventListener("load", () => {
+                ti = i.naturalWidth < i.naturalHeight, i.src = "//:0", s(ti)
+            }), i.src = ha
+        }
+    }), da = (s, i) => {
+        let t, e, r, n;
+        if (!s || s.byteLength < 14 || s.getUint32(0) !== 1165519206 || s.getUint16(4) !== 0) return;
+        if (s.getUint16(6) === 18761) e = !0;
+        else if (s.getUint16(6) === 19789) e = !1;
+        else return;
+        if (s.getUint16(8, e) !== 42) return;
+        r = 8 + s.getUint32(10, e);
+        let o = s.getUint16(r - 2, e);
+        for (t = 0, n = o; n >= 0 ? t < n : t > n; n >= 0 ? ++t : --t) {
+            if (s.byteLength < r + 10) return;
+            s.getUint16(r, e) === 274 && i(r + 8, e), r += 12
+        }
+    }, pa = (s, i) => {
+        da(s, (t, e) => s.setUint16(t, i, e))
+    }, fa = async (s, i, t) => (t && pa(i, 1), kr(s, 225, [i.buffer])), ma = (s, i) => new Promise((t, e) => {
+        i && (s.src = i), s.complete ? t(s) : (s.addEventListener("load", () => {
+            t(s)
+        }), s.addEventListener("error", () => {
+            e(new Error("Failed to load image. Probably not an image."))
+        }))
+    }), ga = s => ma(new Image, s), _a = [1, 3], ba = [192, 193, 194, 195, 197, 198, 199, 201, 202, 203, 205, 206, 207], Ir = {
         squareSide: [Math.floor(Math.sqrt(5 * 1e3 * 1e3)), 4096, 8192, 11180, 10836, 11402, 14188, 16384],
         dimension: [4096, 8192, 16384, 32767, 65535]
-    },
-    Ir = (s, i) => {
+    }, ya = async s => {
+        let i = !1,
+            {
+                promiseReadJpegChunks: t,
+                stack: e
+            } = ei();
+        return await t(s).then(() => (e.forEach(({
+            marker: r,
+            view: n
+        }) => {
+            if (!i && ba.indexOf(r) >= 0) {
+                let o = n.getUint8(5);
+                _a.indexOf(o) < 0 && (i = !0)
+            }
+        }), i)).catch(() => i)
+    }, Pr = (s, i) => {
         let t = {};
         return (...e) => {
             let r = i(e, t);
             return r in t ? t[r] : t[r] = s(...e)
         }
-    },
-    kr = (s, i) => {
+    }, Lr = (s, i) => {
         let [t] = s, e = Object.keys(i).map(r => parseInt(r, 10)).sort((r, n) => r - n);
         for (let r = 0; r < e.length; r++) {
             let n = e[r],
                 o = !!i[n];
             if (n > t && o || n < t && !o) return n
         }
         return t
-    },
-    ue = () => {
-        let s = document.createElement("canvas"),
-            i = s.getContext("2d");
-        return {
-            canvas: s,
-            ctx: i
-        }
-    },
-    Et = {
+    }, At = {
         R: 55,
         G: 110,
         B: 165,
         A: 255
-    },
-    sl = `rgba(${Et.R}, ${Et.G}, ${Et.B}, ${Et.A/255})`,
-    Or = (s, i) => {
+    }, va = `rgba(${At.R}, ${At.G}, ${At.B}, ${At.A/255})`, Ur = (s, i) => {
         try {
             let t = [s - 1, i - 1, 1, 1],
                 {
                     canvas: e,
                     ctx: r
-                } = ue();
+                } = he();
             e.width = 1, e.height = 1;
             let {
                 canvas: n,
                 ctx: o
-            } = ue();
-            n.width = s, n.height = i, o && (o.fillStyle = sl, o.fillRect(...t), r.drawImage(n, s - 1, i - 1, 1, 1, 0, 0, 1, 1));
-            let l = r && r.getImageData(0, 0, 1, 1).data,
-                a = !1;
-            return l && (a = l[0] === Et.R && l[1] === Et.G && l[2] === Et.B && l[3] === Et.A), n.width = n.height = 1, a
+            } = he();
+            n.width = s, n.height = i, o && (o.fillStyle = va, o.fillRect(...t), r.drawImage(n, s - 1, i - 1, 1, 1, 0, 0, 1, 1));
+            let a = r && r.getImageData(0, 0, 1, 1).data,
+                l = !1;
+            return a && (l = a[0] === At.R && a[1] === At.G && a[2] === At.B && a[3] === At.A), n.width = n.height = 1, l
         } catch {
             return console.error(`Failed to test for max canvas size of ${s}x${i}.`), !1
         }
     };
 
-function Pr(s) {
+function Rr(s) {
     return (...i) => new Promise(t => {
         setTimeout(() => {
             let e = s(...i);
             t(e)
         }, 0)
     })
 }
-var rl = Pr(Ir(Or, kr)),
-    nl = Pr(Ir(Or, kr)),
-    Lr = (s, i) => new Promise((t, e) => {
-        let r = $r.squareSide.find(o => o * o >= s * i),
-            n = $r.dimension.find(o => o >= s && o >= i);
-        if (!r || !n) {
-            e();
-            return
-        }
-        Promise.all([rl(r, r), nl(n, 1)]).then(([o, l]) => {
-            o && l ? t(!0) : e()
-        })
-    }),
-    Ur = (s, i, t) => new Promise((e, r) => {
+var Ca = Rr(Pr(Ur, Lr)),
+    wa = Rr(Pr(Ur, Lr)),
+    Mr = async (s, i) => {
+        let t = Ir.squareSide.find(o => o * o >= s * i),
+            e = Ir.dimension.find(o => o >= s && o >= i);
+        if (!t || !e) throw new Error("Not supported");
+        let [r, n] = await Promise.all([Ca(t, t), wa(e, 1)]);
+        if (r && n) return !0;
+        throw new Error("Not supported")
+    }, Nr = async (s, i, t) => {
         try {
             let {
-                ctx: n,
-                canvas: o
-            } = ue();
-            o.width = i, o.height = t, n.imageSmoothingQuality = "high", n.drawImage(s, 0, 0, i, t), s.src = "//:0", s.width = s.height = 1, e(o)
-        } catch (n) {
-            r(`Failed to resize image. ${n}`)
+                ctx: e,
+                canvas: r
+            } = he();
+            return r.width = i, r.height = t, e.imageSmoothingQuality = "high", e.drawImage(s, 0, 0, i, t), s instanceof HTMLImageElement && (s.src = "//:0"), s instanceof HTMLCanvasElement && (s.width = s.height = 1), r
+        } catch (e) {
+            throw new Error("Canvas resize error", {
+                cause: e
+            })
         }
-    }),
-    ol = ({
+    }, Ea = ({
         img: s,
         targetW: i,
         targetH: t
-    }) => Ur(s, i, t),
-    ll = function(s, i, t, e) {
+    }) => Nr(s, i, t), Aa = function({
+        sourceW: s,
+        targetW: i,
+        targetH: t,
+        step: e
+    }) {
         let r = [],
             n = i,
             o = t;
         do r.push([n, o]), n = Math.round(n / e), o = Math.round(o / e); while (n < s * e);
         return r.reverse()
-    },
-    al = ({
+    }, xa = ({
         img: s,
         sourceW: i,
         targetW: t,
         targetH: e,
         step: r
-    }) => ll(i, t, e, r).reduce((o, [l, a]) => o.then(c => Lr(l, a).then(() => c).catch(() => Ur(c, l, a))).then(c => {
-        let u = (i - l) / (i - t);
-        return {
-            canvas: c,
-            progress: u
-        }
-    }), Promise.resolve(s)).then(({
-        canvas: o
-    }) => o).catch(o => Promise.reject(o)),
-    cl = () => /iPad|iPhone|iPod/.test(navigator.platform) ? !0 : navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform),
-    hl = navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform),
-    rs = .71,
-    ul = (s, i) => new Promise((t, e) => {
-        s.width * rs * s.height * rs < i.size && e("Not required");
-        let r = s.width,
-            n = s.height,
-            o = r / n,
-            l = Math.floor(Math.sqrt(i.size * o)),
-            a = Math.floor(i.size / Math.sqrt(i.size * o));
-        return Lr(l, a).then(() => {
+    }) => Aa({
+        sourceW: i,
+        targetW: t,
+        targetH: e,
+        step: r
+    }).reduce((o, [a, l]) => o.then(c => Mr(a, l).then(() => Nr(c, a, l)).catch(() => c)), Promise.resolve(s)), Ta = () => /iPad|iPhone|iPod/.test(navigator.platform) ? !0 : navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform), Sa = navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform), ns = .71, $a = (s, i) => {
+        if (s.width * ns * s.height * ns < i.size) throw new Error("Not required");
+        let t = s.width,
+            e = s.height,
+            r = t / e,
+            n = Math.floor(Math.sqrt(i.size * r)),
+            o = Math.floor(i.size / Math.sqrt(i.size * r));
+        return Mr(n, o).then(() => {
             let {
-                ctx: c
-            } = ue();
-            return "imageSmoothingQuality" in c && !cl() && !hl ? ol({
+                ctx: a
+            } = he();
+            return "imageSmoothingQuality" in a && !Ta() && !Sa ? Ea({
                 img: s,
-                targetW: l,
-                targetH: a
-            }) : al({
+                targetW: n,
+                targetH: o
+            }) : xa({
                 img: s,
-                sourceW: r,
-                targetW: l,
-                targetH: a,
-                step: rs
+                sourceW: t,
+                targetW: n,
+                targetH: o,
+                step: ns
             })
-        }).then(c => t(c)).catch(() => e("Not supported"))
-    }),
-    ii = () => {
-        let s = [];
-        return {
-            stack: s,
-            promiseReadJpegChunks: t => new Promise((e, r) => {
-                let n, o = (c, u) => {
-                        let d = new FileReader;
-                        d.addEventListener("load", () => {
-                            u(new DataView(d.result))
-                        }), d.addEventListener("error", p => {
-                            r(`Reader error: ${p}`)
-                        }), d.readAsArrayBuffer(c)
-                    },
-                    l = () => o(t.slice(n, n + 128), c => {
-                        let u, d, p;
-                        for (u = d = 0, p = c.byteLength; p >= 0 ? d < p : d > p; u = p >= 0 ? ++d : --d)
-                            if (c.getUint8(u) === 255) {
-                                n += u;
-                                break
-                            } return a()
-                    }),
-                    a = () => {
-                        let c = n;
-                        return o(t.slice(n, n += 4), u => {
-                            if (u.byteLength !== 4 || u.getUint8(0) !== 255) return r("Corrupted");
-                            let d = u == null ? void 0 : u.getUint8(1);
-                            if (d === 218) return e(!0);
-                            let p = u.getUint16(2) - 2;
-                            return o(t.slice(n, n += p), m => m.byteLength !== p ? r("Corrupted") : (s.push({
-                                startPos: c,
-                                length: p,
-                                marker: d,
-                                view: m
-                            }), l()))
-                        })
-                    };
-                FileReader && DataView || r("Not Support"), n = 2, o(t.slice(0, 2), function(c) {
-                    return c.getUint16(0) !== 65496 && r("Not jpeg"), l()
-                })
-            })
-        }
-    },
-    Rr = (s, i, t) => new Promise((e, r) => {
-        let n = [],
-            o = [],
-            {
-                promiseReadJpegChunks: l,
-                stack: a
-            } = ii();
-        return l(s).then(() => {
-            a.forEach(c => {
-                if (c.marker === i) return n.push(c.startPos), o.push(c.length)
-            })
-        }).then(() => {
-            let c = [s.slice(0, 2)];
-            for (let d of t) {
-                let p = new DataView(new ArrayBuffer(4));
-                p.setUint16(0, 65280 + i), p.setUint16(2, d.byteLength + 2), c.push(p.buffer), c.push(d)
-            }
-            let u = 2;
-            for (let d = 0; d < n.length; d++) n[d] > u && c.push(s.slice(u, n[d])), u = n[d] + o[d] + 4;
-            c.push(s.slice(u, s.size)), e(new Blob(c, {
-                type: s.type
-            }))
-        }).catch(() => r(s))
-    }).catch(() => s),
-    dl = 226,
-    Mr = (s, i) => Rr(s, dl, i.map(t => t.buffer)),
-    pl = (s, i) => new Promise((t, e) => {
-        i && (s.src = i), s.complete ? t(s) : (s.addEventListener("load", () => {
-            t(s)
-        }), s.addEventListener("error", () => {
-            e(s)
-        }))
-    }),
-    fl = s => pl(new Image, s),
-    ml = async s => {
+        }).catch(() => Promise.reject("Not supported"))
+    }, Dr = async (s, i) => {
         try {
-            let i = await Mr(s, []),
-                t = await fl(URL.createObjectURL(i));
-            return URL.revokeObjectURL(t.src), t
-        } catch (i) {
-            throw new Error(`Failed to strip ICC profile and not image ${i}`)
-        }
-    }, gl = async s => {
-        let i = !1,
-            {
-                promiseReadJpegChunks: t,
-                stack: e
-            } = ii();
-        return await t(s).then(() => (e.forEach(({
-            marker: r,
-            view: n
-        }) => {
-            if (!i && il.indexOf(r) >= 0) {
-                let o = n.getUint8(5);
-                el.indexOf(o) < 0 && (i = !0)
+            if (await ya(s)) throw new Error("Should skipped");
+            let e = await Promise.allSettled([ca(s), ua(), na(s)]),
+                n = !e.some(_ => _.status === "rejected"),
+                [o, a, l] = e,
+                c = await oa(s).catch(() => s),
+                u = await ga(URL.createObjectURL(c));
+            URL.revokeObjectURL(u.src);
+            let d = await $a(u, i),
+                p = "image/jpeg",
+                m = (i == null ? void 0 : i.quality) || .8;
+            !n && la(d) && (p = "image/png", m = void 0);
+            let f = await aa(d, p, m);
+            if (n && o.status === "fulfilled" && o.value) {
+                let _ = o.value,
+                    y = a.status === "fulfilled" ? a.value : !1;
+                f = await fa(f, _, y)
             }
-        }), i)).catch(() => i)
-    }, _l = (s, i, t, e) => s.toBlob(e, i, t), bl = s => {
-        let {
-            ctx: t,
-            canvas: e
-        } = ue();
-        e.width = e.height = 50, t.drawImage(s, 0, 0, 50, 50);
-        let r = t.getImageData(0, 0, 50, 50).data;
-        e.width = e.height = 1;
-        for (let n = 3; n < r.length; n += 4)
-            if (r[n] < 254) return !0;
-        return !1
-    }, yl = "data:image/jpg;base64,/9j/4AAQSkZJRgABAQEASABIAAD/4QA6RXhpZgAATU0AKgAAAAgAAwESAAMAAAABAAYAAAEoAAMAAAABAAIAAAITAAMAAAABAAEAAAAAAAD/2wBDAP//////////////////////////////////////////////////////////////////////////////////////wAALCAABAAIBASIA/8QAJgABAAAAAAAAAAAAAAAAAAAAAxABAAAAAAAAAAAAAAAAAAAAAP/aAAgBAQAAPwBH/9k=", ei, vl = () => new Promise(s => {
-        if (ei !== void 0) s(ei);
-        else {
-            let i = new Image;
-            i.addEventListener("load", () => {
-                ei = i.naturalWidth < i.naturalHeight, i.src = "//:0", s(ei)
-            }), i.src = yl
-        }
-    }), Cl = async s => {
-        let i = null,
-            {
-                promiseReadJpegChunks: t,
-                stack: e
-            } = ii();
-        return t(s).then(() => {
-            e.forEach(({
-                marker: r,
-                view: n
-            }) => (!i && r === 225 && n.byteLength >= 14 && n.getUint32(0) === 1165519206 && n.getUint16(4) === 0 && (i = n), i))
-        }).catch(() => i)
-    }, wl = async s => {
-        let i = [],
-            {
-                promiseReadJpegChunks: t,
-                stack: e
-            } = ii();
-        return await t(s).then(() => (e.forEach(({
-            marker: r,
-            view: n
-        }) => {
-            r === 226 && n.getUint32(0) === 1229144927 && n.getUint32(4) === 1347571526 && n.getUint32(8) === 1229735168 && i.push(n)
-        }), i)).catch(() => i)
-    }, Al = (s, i) => {
-        let t, e, r, n;
-        if (!s || s.byteLength < 14 || s.getUint32(0) !== 1165519206 || s.getUint16(4) !== 0) return null;
-        if (s.getUint16(6) === 18761) e = !0;
-        else if (s.getUint16(6) === 19789) e = !1;
-        else return null;
-        if (s.getUint16(8, e) !== 42) return null;
-        r = 8 + s.getUint32(10, e);
-        let o = s.getUint16(r - 2, e);
-        for (t = 0, n = o; n >= 0 ? t < n : t > n; n >= 0 ? ++t : --t) {
-            if (s.byteLength < r + 10) return null;
-            if (s.getUint16(r, e) === 274) return i(r + 8, e);
-            r += 12
-        }
-        return null
-    }, El = (s, i) => {
-        Al(s, (t, e) => s.setUint16(t, i, e))
-    }, xl = async (s, i, t) => (t && El(i, 1), Rr(s, 225, [i.buffer])), Nr = (s, i) => new Promise(async (t, e) => {
-        URL && DataView && Blob || e("Not support");
-        try {
-            let r = await gl(s).then(o => {
-                if (o) return e("Should skipped")
-            }).then(() => ml(s).catch(() => {
-                e("Failed to strip ICC profile and not image")
-            }));
-            Promise.allSettled([Cl(s), vl(), wl(s)]).then(async o => {
-                let l = o.some(p => p.status === "rejected"),
-                    [a, c, u] = o,
-                    d = !l;
-                return ul(r, i).then(async p => {
-                    let m = "image/jpeg",
-                        f = (i == null ? void 0 : i.quality) || .8;
-                    !d && bl(p) && (m = "image/png", f = void 0), _l(p, m, f, _ => {
-                        var x;
-                        p.width = p.height = 1;
-                        let b = Promise.resolve(_);
-                        a.value && (b = b.then(v => xl(v, a.value, c.value)).catch(() => _)), ((x = u == null ? void 0 : u.value) == null ? void 0 : x.length) > 0 && (b = b.then(v => Mr(v, u.value)).catch(() => _)), b.then(t).catch(() => t(_))
-                    })
-                }).catch(() => e(s))
+            return n && l.status === "fulfilled" && l.value.length > 0 && (f = await Or(f, l.value)), f
+        } catch (t) {
+            let e;
+            throw t instanceof Error && (e = t.message), typeof t == "string" && (e = t), new Error(`Failed to shrink image. ${e?`Message: "${e}".`:""}`, {
+                cause: t
             })
-        } catch (r) {
-            e(`Failed to shrink image: ${r}`)
         }
-    });
+    };
 
-function Dr(s) {
+function Fr(s) {
     let i = new Blob([s], {
         type: "image/svg+xml"
     });
     return URL.createObjectURL(i)
 }
 
-function Fr(s = "#fff", i = "rgba(0, 0, 0, .1)") {
-    return Dr(`<svg height="20" width="20" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><rect x="0" y="0" width="20" height="20" fill="${s}" /><rect x="0" y="0" width="10" height="10" fill="${i}" /><rect x="10" y="10" width="10" height="10" fill="${i}" /></svg>`)
+function Br(s = "#fff", i = "rgba(0, 0, 0, .1)") {
+    return Fr(`<svg height="20" width="20" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><rect x="0" y="0" width="20" height="20" fill="${s}" /><rect x="0" y="0" width="10" height="10" fill="${i}" /><rect x="10" y="10" width="10" height="10" fill="${i}" /></svg>`)
 }
 
-function de(s = "hsl(209, 21%, 65%)", i = 32, t = 32) {
-    return Dr(`<svg width="${i}" height="${t}" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" fill="${s}" d="M9.68848 8.70068C9.68848 8.42454 9.91233 8.20068 10.1885 8.20068H15.0885C15.2211 8.20068 15.3483 8.25336 15.442 8.34713L20.342 13.2471C20.4358 13.3409 20.4885 13.4681 20.4885 13.6007V21.3007C20.4885 21.5768 20.2646 21.8007 19.9885 21.8007H10.1885C9.91233 21.8007 9.68848 21.5768 9.68848 21.3007V8.70068ZM10.6885 9.20068V20.8007H19.4885V14.1007L15.0885 14.1007C14.8123 14.1007 14.5885 13.8768 14.5885 13.6007L14.5885 9.20068H10.6885ZM15.5885 9.90779L18.7814 13.1007L15.5885 13.1007L15.5885 9.90779Z"/></svg>`)
+function ue(s = "hsl(209, 21%, 65%)", i = 32, t = 32) {
+    return Fr(`<svg width="${i}" height="${t}" viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" fill="${s}" d="M9.68848 8.70068C9.68848 8.42454 9.91233 8.20068 10.1885 8.20068H15.0885C15.2211 8.20068 15.3483 8.25336 15.442 8.34713L20.342 13.2471C20.4358 13.3409 20.4885 13.4681 20.4885 13.6007V21.3007C20.4885 21.5768 20.2646 21.8007 19.9885 21.8007H10.1885C9.91233 21.8007 9.68848 21.5768 9.68848 21.3007V8.70068ZM10.6885 9.20068V20.8007H19.4885V14.1007L15.0885 14.1007C14.8123 14.1007 14.5885 13.8768 14.5885 13.6007L14.5885 9.20068H10.6885ZM15.5885 9.90779L18.7814 13.1007L15.5885 13.1007L15.5885 9.90779Z"/></svg>`)
 }
 
-function Br(s, i = 40) {
+function zr(s, i = 40) {
     if (s.type === "image/svg+xml") return URL.createObjectURL(s);
     let t = document.createElement("canvas"),
         e = t.getContext("2d"),
         r = new Image,
-        n = new Promise((o, l) => {
+        n = new Promise((o, a) => {
             r.onload = () => {
-                let a = r.height / r.width;
-                a > 1 ? (t.width = i, t.height = i * a) : (t.height = i, t.width = i / a), e.fillStyle = "rgb(240, 240, 240)", e.fillRect(0, 0, t.width, t.height), e.drawImage(r, 0, 0, t.width, t.height), t.toBlob(c => {
+                let l = r.height / r.width;
+                l > 1 ? (t.width = i, t.height = i * l) : (t.height = i, t.width = i / l), e.fillStyle = "rgb(240, 240, 240)", e.fillRect(0, 0, t.width, t.height), e.drawImage(r, 0, 0, t.width, t.height), t.toBlob(c => {
                     if (!c) {
-                        l();
+                        a();
                         return
                     }
                     let u = URL.createObjectURL(c);
                     o(u)
                 })
-            }, r.onerror = a => {
-                l(a)
+            }, r.onerror = l => {
+                a(l)
             }
         });
     return r.src = URL.createObjectURL(s), n
 }
-var Tl = /^([0-9]+)x([0-9]+)(?:\s+(\d{1,2}|100)%)?$/i,
-    zr = s => {
-        let i = Tl.exec(s == null ? void 0 : s.toLocaleLowerCase()) || [];
+var Ia = /^([0-9]+)x([0-9]+)(?:\s+(\d{1,2}|100)%)?$/i,
+    Vr = s => {
+        let i = Ia.exec(s == null ? void 0 : s.toLocaleLowerCase()) || [];
         if (!i.length) return !1;
         let t = i[1] * i[2],
             e = 16384 * 16384;
         return t > e ? (console.warn(`Shrinked size can not be larger than ${Math.floor(e/1e3/1e3)}MP. You have set ${i[1]}x${i[2]} (${Math.ceil(t/1e3/100)/10}MP).`), !1) : {
             quality: i[3] ? i[3] / 100 : void 0,
             size: t
         }
     };
 var J = Object.freeze({
         FINISHED: Symbol(0),
         FAILED: Symbol(1),
         UPLOADING: Symbol(2),
         IDLE: Symbol(3)
     }),
-    pe = class s extends T {
+    de = class s extends A {
         constructor() {
             super();
             h(this, "couldBeCtxOwner", !0);
             h(this, "pauseRender", !0);
             h(this, "_entrySubs", new Set);
             h(this, "_entry", null);
             h(this, "_isIntersecting", !1);
@@ -5454,15 +5499,14 @@
                 ...this.init$,
                 uid: "",
                 itemName: "",
                 errorText: "",
                 thumbUrl: "",
                 progressValue: 0,
                 progressVisible: !1,
-                progressUnknown: !1,
                 badgeIcon: "",
                 isFinished: !1,
                 isFailed: !1,
                 isUploading: !1,
                 isFocused: !1,
                 isEditable: !1,
                 state: J.IDLE,
@@ -5502,22 +5546,22 @@
                     n = this.proxyUrl(O(Ct(this.cfg.cdnCname, this._entry.getValue("uuid")), R(t.getValue("cdnUrlModifiers"), `scale_crop/${r}x${r}/center`))),
                     o = t.getValue("thumbUrl");
                 o !== n && (t.setValue("thumbUrl", n), o != null && o.startsWith("blob:") && URL.revokeObjectURL(o));
                 return
             }
             if (!t.getValue("thumbUrl"))
                 if ((e = t.getValue("file")) != null && e.type.includes("image")) try {
-                    let r = await Br(t.getValue("file"), this.cfg.thumbSize);
+                    let r = await zr(t.getValue("file"), this.cfg.thumbSize);
                     t.setValue("thumbUrl", r)
                 } catch {
                     let n = window.getComputedStyle(this).getPropertyValue("--clr-generic-file-icon");
-                    t.setValue("thumbUrl", de(n))
+                    t.setValue("thumbUrl", ue(n))
                 } else {
                     let r = window.getComputedStyle(this).getPropertyValue("--clr-generic-file-icon");
-                    t.setValue("thumbUrl", de(r))
+                    t.setValue("thumbUrl", ue(r))
                 }
         }
         _subEntry(t, e) {
             let r = this._entry.subscribe(t, n => {
                 this.isConnected && e(n)
             });
             this._entrySubs.add(r)
@@ -5551,22 +5595,22 @@
                 })
             }, this.sub("*uploadTrigger", t => {
                 t.has(this._entry.uid) && setTimeout(() => this.isConnected && this.upload())
             }), s.activeInstances.add(this)
         }
         _handleState(t) {
             var e, r, n, o;
-            this.set$({
+            t === J.FAILED ? this.$.badgeIcon = "badge-error" : t === J.FINISHED && (this.$.badgeIcon = "badge-success"), t === J.UPLOADING ? this.$.isFocused = !1 : this.$.progressValue = 0, this.set$({
                 isFailed: t === J.FAILED,
                 isUploading: t === J.UPLOADING,
                 isFinished: t === J.FINISHED,
                 progressVisible: t === J.UPLOADING,
                 isEditable: this.cfg.useCloudImageEditor && ((e = this._entry) == null ? void 0 : e.getValue("isImage")) && ((r = this._entry) == null ? void 0 : r.getValue("cdnUrl")),
                 errorText: (o = (n = this._entry.getValue("errors")) == null ? void 0 : n[0]) == null ? void 0 : o.message
-            }), t === J.FAILED ? this.$.badgeIcon = "badge-error" : t === J.FINISHED && (this.$.badgeIcon = "badge-success"), t === J.UPLOADING ? this.$.isFocused = !1 : this.$.progressValue = 0
+            })
         }
         destroyCallback() {
             super.destroyCallback(), s.activeInstances.delete(this), this._reset()
         }
         connectedCallback() {
             super.connectedCallback(), this._observer = new window.IntersectionObserver(this._observerCallback.bind(this), {
                 root: this.parentElement,
@@ -5575,77 +5619,76 @@
             }), this._observer.observe(this)
         }
         disconnectedCallback() {
             var t;
             super.disconnectedCallback(), this._debouncedGenerateThumb.cancel(), (t = this._observer) == null || t.disconnect()
         }
         _settingsOfShrink() {
-            return zr(this.cfg.imageShrink)
+            return Vr(this.cfg.imageShrink)
         }
         _processShrink(t) {
-            return Nr(t, this._settingsOfShrink())
+            return Dr(t, this._settingsOfShrink())
         }
         async upload() {
-            var r, n, o;
+            var r, n, o, a, l;
             let t = this._entry;
             if (!this.uploadCollection.read(t.uid) || t.getValue("fileInfo") || t.getValue("isUploading") || t.getValue("errors").length > 0) return;
             let e = this.cfg.multiple ? this.cfg.multipleMax : 1;
             if (!(e && this.uploadCollection.size > e)) {
-                this._debouncedCalculateState(), t.setValue("isUploading", !0), t.setValue("errors", []), !t.getValue("file") && t.getValue("externalUrl") && (this.$.progressUnknown = !0);
+                this._debouncedCalculateState(), t.setValue("isUploading", !0), t.setValue("errors", []);
                 try {
-                    let l = new AbortController;
-                    t.setValue("abortController", l);
-                    let a = async () => {
-                        let u = t.getValue("file");
-                        u && this.cfg.imageShrink && (u = await this._processShrink(u).catch(() => u));
-                        let d = u || t.getValue("externalUrl") || t.getValue("uuid"),
-                            m = {
+                    let c = new AbortController;
+                    t.setValue("abortController", c);
+                    let u = async () => {
+                        let p = t.getValue("file");
+                        p && this.cfg.imageShrink && (p = await this._processShrink(p).catch(() => p));
+                        let m = p || t.getValue("externalUrl") || t.getValue("uuid"),
+                            _ = {
                                 ...this.getUploadClientOptions(),
                                 fileName: t.getValue("fileName"),
                                 source: t.getValue("source"),
-                                onProgress: f => {
-                                    if (f.isComputable) {
-                                        let _ = f.value * 100;
-                                        t.setValue("uploadProgress", _)
+                                onProgress: y => {
+                                    if (y.isComputable) {
+                                        let x = y.value * 100;
+                                        t.setValue("uploadProgress", x)
                                     }
-                                    this.$.progressUnknown = !f.isComputable
                                 },
-                                signal: l.signal,
+                                signal: c.signal,
                                 metadata: await this.getMetadataFor(t.uid)
                             };
-                        return this.debugPrint("upload options", d, m), Vi(d, m)
-                    }, c = await this.$["*uploadQueue"].add(a);
+                        return this.debugPrint("upload options", m, _), ji(m, _)
+                    }, d = await this.$["*uploadQueue"].add(u);
                     t.setMultipleValues({
-                        fileInfo: c,
+                        fileInfo: d,
                         isUploading: !1,
-                        fileName: c.originalFilename,
-                        fileSize: c.size,
-                        isImage: c.isImage,
-                        mimeType: (o = (n = (r = c.contentInfo) == null ? void 0 : r.mime) == null ? void 0 : n.mime) != null ? o : c.mimeType,
-                        uuid: c.uuid,
-                        cdnUrl: c.cdnUrl,
-                        cdnUrlModifiers: "",
+                        fileName: d.originalFilename,
+                        fileSize: d.size,
+                        isImage: d.isImage,
+                        mimeType: (o = (n = (r = d.contentInfo) == null ? void 0 : r.mime) == null ? void 0 : n.mime) != null ? o : d.mimeType,
+                        uuid: d.uuid,
+                        cdnUrl: (a = t.getValue("cdnUrl")) != null ? a : d.cdnUrl,
+                        cdnUrlModifiers: (l = t.getValue("cdnUrlModifiers")) != null ? l : "",
                         uploadProgress: 100
                     }), t === this._entry && this._debouncedCalculateState()
-                } catch (l) {
-                    l instanceof _t && l.isCancel ? t.setMultipleValues({
+                } catch (c) {
+                    c instanceof _t && c.isCancel ? t.setMultipleValues({
                         isUploading: !1,
                         uploadProgress: 0
                     }) : t.setMultipleValues({
                         isUploading: !1,
                         uploadProgress: 0,
-                        uploadError: l
+                        uploadError: c
                     }), t === this._entry && this._debouncedCalculateState()
                 }
             }
         }
     };
-pe.template = `<div class="inner" set="@finished: isFinished; @uploading: isUploading; @failed: isFailed; @focused: isFocused"><div class="thumb" set="style.backgroundImage: thumbUrl"><div class="badge"><lr-icon set="@name: badgeIcon"></lr-icon></div></div><div class="file-name-wrapper"><span class="file-name" set="@title: itemName">{{itemName}}</span><span class="file-error" set="@hidden: !errorText">{{errorText}}</span></div><div class="file-actions"><button type="button" class="edit-btn mini-btn" set="onclick: onEdit; @hidden: !isEditable"><lr-icon name="edit-file"></lr-icon></button><button type="button" class="remove-btn mini-btn" set="onclick: onRemove;"><lr-icon name="remove-file"></lr-icon></button><button type="button" class="upload-btn mini-btn" set="onclick: onUpload;"><lr-icon name="upload"></lr-icon></button></div><lr-progress-bar class="progress-bar" set="value: progressValue; visible: progressVisible; unknown: progressUnknown" ></lr-progress-bar></div>`;
-pe.activeInstances = new Set;
-var fe = class extends w {
+de.template = `<div class="inner" set="@finished: isFinished; @uploading: isUploading; @failed: isFailed; @focused: isFocused"><div class="thumb" set="style.backgroundImage: thumbUrl"><div class="badge"><lr-icon set="@name: badgeIcon"></lr-icon></div></div><div class="file-name-wrapper"><span class="file-name" set="@title: itemName">{{itemName}}</span><span class="file-error" set="@hidden: !errorText">{{errorText}}</span></div><div class="file-actions"><button type="button" class="edit-btn mini-btn" set="onclick: onEdit; @hidden: !isEditable"><lr-icon name="edit-file"></lr-icon></button><button type="button" class="remove-btn mini-btn" set="onclick: onRemove;"><lr-icon name="remove-file"></lr-icon></button><button type="button" class="upload-btn mini-btn" set="onclick: onUpload;"><lr-icon name="upload"></lr-icon></button></div><lr-progress-bar class="progress-bar" set="value: progressValue; visible: progressVisible;"></lr-progress-bar></div>`;
+de.activeInstances = new Set;
+var pe = class extends C {
     constructor() {
         super();
         h(this, "_handleBackdropClick", () => {
             this._closeDialog()
         });
         h(this, "_closeDialog", () => {
             this.setOrAddState("*modalActive", !1)
@@ -5687,23 +5730,38 @@
             t ? this.show() : this.hide()
         })
     }
     destroyCallback() {
         super.destroyCallback(), document.body.style.overflow = "", this._mouseDownTarget = void 0, this.ref.dialog.removeEventListener("close", this._handleDialogClose), this.ref.dialog.removeEventListener("mousedown", this._handleDialogMouseDown), this.ref.dialog.removeEventListener("mouseup", this._handleDialogMouseUp)
     }
 };
-h(fe, "StateConsumerScope", "modal");
-fe.template = `<dialog ref="dialog"><slot></slot></dialog>`;
-var si = class extends T {
+h(pe, "StateConsumerScope", "modal");
+pe.template = `<dialog ref="dialog"><slot></slot></dialog>`;
+var ii = (s, i) => {
+    let t, e, r, n = (...o) => {
+        t ? (clearTimeout(e), e = setTimeout(() => {
+            Date.now() - r >= i && (s(...o), r = Date.now())
+        }, Math.max(i - (Date.now() - r), 0))) : (s(...o), r = Date.now(), t = !0)
+    };
+    return Object.defineProperty(n, "cancel", {
+        configurable: !1,
+        writable: !1,
+        enumerable: !1,
+        value: () => {
+            clearTimeout(e)
+        }
+    }), n
+};
+var si = class extends A {
     constructor() {
         super();
         h(this, "couldBeCtxOwner", !0);
         h(this, "historyTracked", !0);
         h(this, "activityType", g.activities.UPLOAD_LIST);
-        h(this, "_throttledHandleCollectionUpdate", We(() => {
+        h(this, "_throttledHandleCollectionUpdate", ii(() => {
             this.isConnected && (this._updateUploadsState(), !this.couldOpenActivity && this.$["*currentActivity"] === this.activityType && this.historyBack())
         }, 300));
         this.init$ = {
             ...this.init$,
             doneBtnVisible: !1,
             doneBtnEnabled: !1,
             uploadBtnVisible: !1,
@@ -5733,22 +5791,22 @@
                 succeed: t.successCount,
                 uploading: t.uploadingCount,
                 failed: t.failedCount
             },
             r = !t.errors.some(p => p.type === "TOO_MANY_FILES" || p.type === "TOO_FEW_FILES"),
             n = t.errors.some(p => p.type === "TOO_MANY_FILES"),
             o = t.totalCount === (this.cfg.multiple ? this.cfg.multipleMax : 1),
-            l = e.failed === 0,
-            a = !1,
+            a = e.failed === 0,
+            l = !1,
             c = !1,
             u = !1;
-        e.total - e.succeed - e.uploading - e.failed > 0 && r ? a = !0 : (c = !0, u = e.total === e.succeed && r && l), this.set$({
+        e.total - e.succeed - e.uploading - e.failed > 0 && r ? l = !0 : (c = !0, u = e.total === e.succeed && r && a), this.set$({
             doneBtnVisible: c,
             doneBtnEnabled: u,
-            uploadBtnVisible: a,
+            uploadBtnVisible: l,
             addMoreBtnEnabled: e.total === 0 || !n && !o,
             addMoreBtnVisible: !o || this.cfg.multiple,
             headerText: this._getHeaderText(e)
         })
     }
     _getHeaderText(t) {
         let e = r => {
@@ -5783,27 +5841,27 @@
         })
     }
     destroyCallback() {
         super.destroyCallback(), this.uploadCollection.unobserveProperties(this._throttledHandleCollectionUpdate)
     }
 };
 si.template = `<lr-activity-header><span class="header-text">{{headerText}}</span><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="no-files" set="@hidden: hasFiles"><slot name="empty"><span l10n="no-files"></span></slot></div><div class="files" repeat="*uploadList" repeat-item-tag="lr-file-item"></div><div class="common-error" set="@hidden: !commonErrorMessage; textContent: commonErrorMessage;"></div><div class="toolbar"><button type="button" class="cancel-btn secondary-btn" set="onclick: onCancel;" l10n="clear"></button><div class="toolbar-spacer"></div><button type="button" class="add-more-btn secondary-btn" set="onclick: onAdd; @disabled: !addMoreBtnEnabled; @hidden: !addMoreBtnVisible" ><lr-icon name="add"></lr-icon><span l10n="add-more"></span></button><button type="button" class="upload-btn primary-btn" set="@hidden: !uploadBtnVisible; onclick: onUpload;" l10n="upload" ></button><button type="button" class="done-btn primary-btn" set="@hidden: !doneBtnVisible; onclick: onDone; @disabled: !doneBtnEnabled" l10n="done" ></button></div><lr-drop-area ghost></lr-drop-area>`;
-var ri = class extends T {
+var ri = class extends A {
     constructor() {
         super(...arguments);
         h(this, "couldBeCtxOwner", !0);
         h(this, "activityType", g.activities.URL);
         h(this, "init$", {
             ...this.init$,
             importDisabled: !0,
             onUpload: t => {
                 t.preventDefault();
                 let e = this.ref.input.value;
                 this.addFileFromUrl(e, {
-                    source: Y.URL_TAB
+                    source: G.URL_TAB
                 }), this.$["*currentActivity"] = g.activities.UPLOAD_LIST
             },
             onCancel: () => {
                 this.historyBack()
             },
             onInput: t => {
                 let e = t.target.value;
@@ -5818,29 +5876,29 @@
             onActivate: () => {
                 this.ref.input.value = "", this.ref.input.focus()
             }
         })
     }
 };
 ri.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><div><lr-icon name="url"></lr-icon><span l10n="caption-from-url"></span></div><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><form class="content"><input placeholder="https://" class="url-input" type="text" ref="input" set="oninput: onInput" /><button type="submit" class="url-upload-btn primary-btn" set="onclick: onUpload; @disabled: importDisabled" ></button></form>`;
-var ns = () => typeof navigator.permissions != "undefined";
-var ni = class extends T {
+var os = () => typeof navigator.permissions != "undefined";
+var ni = class extends A {
     constructor() {
         super(...arguments);
         h(this, "couldBeCtxOwner", !0);
         h(this, "activityType", g.activities.CAMERA);
         h(this, "_unsubPermissions", null);
         h(this, "init$", {
             ...this.init$,
             video: null,
             videoTransformCss: null,
             shotBtnDisabled: !0,
             videoHidden: !0,
             messageHidden: !0,
-            requestBtnHidden: ns(),
+            requestBtnHidden: os(),
             l10nMessage: null,
             originalErrorMessage: null,
             cameraSelectOptions: null,
             cameraSelectHidden: !0,
             onCameraSelectChange: t => {
                 this._selectedCameraId = t.target.value, this._capture()
             },
@@ -5851,15 +5909,15 @@
                 this._shot()
             },
             onRequestPermissions: () => {
                 this._capture()
             }
         });
         h(this, "_onActivate", () => {
-            ns() && this._subscribePermissions(), this._capture()
+            os() && this._subscribePermissions(), this._capture()
         });
         h(this, "_onDeactivate", () => {
             this._unsubPermissions && this._unsubPermissions(), this._stopCapture()
         });
         h(this, "_handlePermissionsChange", () => {
             this._capture()
         });
@@ -5919,26 +5977,27 @@
     _stopCapture() {
         var t;
         this._capturing && ((t = this.$.video) == null || t.getTracks()[0].stop(), this.$.video = null, this._capturing = !1)
     }
     _shot() {
         this._canvas.height = this.ref.video.videoHeight, this._canvas.width = this.ref.video.videoWidth, this._ctx.drawImage(this.ref.video, 0, 0);
         let t = Date.now(),
-            e = `camera-${t}.png`;
-        this._canvas.toBlob(r => {
-            let n = new File([r], e, {
+            e = `camera-${t}.jpeg`,
+            r = "image/jpeg";
+        this._canvas.toBlob(n => {
+            let o = new File([n], e, {
                 lastModified: t,
-                type: "image/png"
+                type: r
             });
-            this.addFileFromObject(n, {
-                source: Y.CAMERA
+            this.addFileFromObject(o, {
+                source: G.CAMERA
             }), this.set$({
                 "*currentActivity": g.activities.UPLOAD_LIST
             })
-        })
+        }, r)
     }
     async initCallback() {
         super.initCallback(), this.registerActivity(this.activityType, {
             onActivate: this._onActivate,
             onDeactivate: this._onDeactivate
         }), this.subConfigValue("cameraMirror", t => {
             this.$.videoTransformCss = t ? "scaleX(-1)" : null
@@ -5949,28 +6008,29 @@
                 value: r.deviceId
             }));
             e.length > 1 && (this.$.cameraSelectOptions = e, this.$.cameraSelectHidden = !1)
         } catch {}
     }
 };
 ni.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><div set="@hidden: !cameraSelectHidden"><lr-icon name="camera"></lr-icon><span l10n="caption-camera"></span></div><lr-select class="camera-select" set="$.options: cameraSelectOptions; @hidden: cameraSelectHidden; onchange: onCameraSelectChange" ></lr-select><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="content"><video autoplay playsinline set="srcObject: video; style.transform: videoTransformCss; @hidden: videoHidden" ref="video" ></video><div class="message-box" set="@hidden: messageHidden"><span>{{l10nMessage}}</span><span>{{originalErrorMessage}}</span><button type="button" set="onclick: onRequestPermissions; @hidden: requestBtnHidden" l10n="camera-permissions-request" ></button></div><button type="button" class="shot-btn" set="onclick: onShot; @disabled: shotBtnDisabled"><lr-icon name="camera"></lr-icon></button></div>`;
-var os = class extends T {
-        constructor() {
-            super(...arguments);
-            h(this, "requireCtxName", !0)
-        }
-        initCallback() {
-            super.initCallback(), this.$["*eventEmitter"].bindTarget(this)
-        }
-        destroyCallback() {
-            super.destroyCallback(), this.$["*eventEmitter"].unbindTarget(this)
-        }
-    },
-    Sl = os;
-var oi = class extends T {
+var oi = class extends A {
+    constructor() {
+        super(...arguments);
+        h(this, "requireCtxName", !0)
+    }
+    initCallback() {
+        super.initCallback(), this.$["*eventEmitter"].bindTarget(this)
+    }
+    destroyCallback() {
+        super.destroyCallback(), this.$["*eventEmitter"].unbindTarget(this)
+    }
+};
+oi.EventType = $;
+var ka = oi;
+var ai = class extends A {
     constructor() {
         super(...arguments);
         h(this, "activityType", g.activities.DETAILS);
         h(this, "pauseRender", !0);
         h(this, "init$", {
             ...this.init$,
             checkerboard: !1,
@@ -5989,15 +6049,15 @@
             onCloudEdit: () => {
                 this.entry.getValue("uuid") && (this.$["*currentActivity"] = g.activities.CLOUD_IMG_EDIT)
             }
         })
     }
     showNonImageThumb() {
         let t = window.getComputedStyle(this).getPropertyValue("--clr-generic-file-icon"),
-            e = de(t, 108, 108);
+            e = ue(t, 108, 108);
         this.ref.filePreview.setImageUrl(e), this.set$({
             checkerboard: !1
         })
     }
     initCallback() {
         super.initCallback(), this.render(), this.$.fileSize = this.l10n("file-size-unknown"), this.registerActivity(this.activityType, {
             onDeactivate: () => {
@@ -6007,15 +6067,15 @@
             if (!t) return;
             this._entrySubs ? this._entrySubs.forEach(n => {
                 this._entrySubs.delete(n), n.remove()
             }) : this._entrySubs = new Set, this.entry = t;
             let e = t.getValue("file");
             if (e) {
                 this._file = e;
-                let n = se(this._file);
+                let n = ie(this._file);
                 n && !t.getValue("cdnUrl") && (this.ref.filePreview.setImageFile(this._file), this.set$({
                     checkerboard: !0
                 })), n || this.showNonImageThumb()
             }
             let r = (n, o) => {
                 this._entrySubs.add(this.entry.subscribe(n, o))
             };
@@ -6036,23 +6096,23 @@
                 n && (this.entry.getValue("uuid") || this.showNonImageThumb())
             }), r("cdnUrl", n => {
                 let o = this.cfg.useCloudImageEditor && n && this.entry.getValue("isImage");
                 if (n && this.ref.filePreview.clear(), this.set$({
                         cdnUrl: n,
                         cloudEditBtnHidden: !o
                     }), n && this.entry.getValue("isImage")) {
-                    let l = O(n, R("format/auto", "preview"));
-                    this.ref.filePreview.setImageUrl(this.proxyUrl(l))
+                    let a = O(n, R("format/auto", "preview"));
+                    this.ref.filePreview.setImageUrl(this.proxyUrl(a))
                 }
             })
         })
     }
 };
-oi.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><span l10n="caption-edit-file"></span><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="content"><lr-tabs tab-list="tab-view, tab-details"><div tab-ctx="tab-details" class="details"><div class="info-block"><div class="info-block_name" l10n="file-name"></div><input name="name-input" ref="file_name_input" set="value: fileName; oninput: onNameInput; @disabled: !!cdnUrl" type="text" /></div><div class="info-block"><div class="info-block_name" l10n="file-size"></div><div>{{fileSize}}</div></div><div class="info-block"><div class="info-block_name" l10n="cdn-url"></div><a class="cdn-link" target="_blank" set="@href: cdnUrl; @disabled: !cdnUrl">{{cdnUrl}}</a></div><div>{{errorTxt}}</div></div><lr-file-preview tab-ctx="tab-view" set="@checkerboard: checkerboard;" ref="filePreview"></lr-file-preview></lr-tabs><div class="toolbar" set="@edit-disabled: cloudEditBtnHidden"><button type="button" class="edit-btn secondary-btn" set="onclick: onCloudEdit; @hidden: cloudEditBtnHidden;"><lr-icon name="edit"></lr-icon><span l10n="edit-image"></span></button><button type="button" class="remove-btn secondary-btn" set="onclick: onRemove"><lr-icon name="remove"></lr-icon><span l10n="remove-from-list"></span></button><div></div><button type="button" class="back-btn primary-btn" set="onclick: onBack"><span l10n="ok"></span></button></div></div>`;
-var ls = class {
+ai.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><span l10n="caption-edit-file"></span><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="content"><lr-tabs tab-list="tab-view, tab-details"><div tab-ctx="tab-details" class="details"><div class="info-block"><div class="info-block_name" l10n="file-name"></div><input name="name-input" ref="file_name_input" set="value: fileName; oninput: onNameInput; @disabled: !!cdnUrl" type="text" /></div><div class="info-block"><div class="info-block_name" l10n="file-size"></div><div>{{fileSize}}</div></div><div class="info-block"><div class="info-block_name" l10n="cdn-url"></div><a class="cdn-link" target="_blank" set="@href: cdnUrl; @disabled: !cdnUrl">{{cdnUrl}}</a></div><div>{{errorTxt}}</div></div><lr-file-preview tab-ctx="tab-view" set="@checkerboard: checkerboard;" ref="filePreview"></lr-file-preview></lr-tabs><div class="toolbar" set="@edit-disabled: cloudEditBtnHidden"><button type="button" class="edit-btn secondary-btn" set="onclick: onCloudEdit; @hidden: cloudEditBtnHidden;"><lr-icon name="edit"></lr-icon><span l10n="edit-image"></span></button><button type="button" class="remove-btn secondary-btn" set="onclick: onRemove"><lr-icon name="remove"></lr-icon><span l10n="remove-from-list"></span></button><div></div><button type="button" class="back-btn primary-btn" set="onclick: onBack"><span l10n="ok"></span></button></div></div>`;
+var as = class {
         constructor() {
             h(this, "captionL10nStr", "confirm-your-action");
             h(this, "messageL10Str", "are-you-sure");
             h(this, "confirmL10nStr", "yes");
             h(this, "denyL10nStr", "no")
         }
         confirmAction() {
@@ -6062,15 +6122,15 @@
             this.historyBack()
         }
     },
     li = class extends g {
         constructor() {
             super(...arguments);
             h(this, "activityType", g.activities.CONFIRMATION);
-            h(this, "_defaults", new ls);
+            h(this, "_defaults", new as);
             h(this, "init$", {
                 ...this.init$,
                 activityCaption: "",
                 messageTxt: "",
                 confirmBtnTxt: "",
                 denyBtnTxt: "",
                 "*confirmation": null,
@@ -6097,21 +6157,20 @@
                         t.confirmAction()
                     }
                 })
             })
         }
     };
 li.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><span>{{activityCaption}}</span><button type="button" class="mini-btn close-btn" set="onclick: *closeModal"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="message">{{messageTxt}}</div><div class="toolbar"><button type="button" class="deny-btn secondary-btn" set="onclick: onDeny">{{denyBtnTxt}}</button><button type="button" class="confirm-btn primary-btn" set="onclick: onConfirm">{{confirmBtnTxt}}</button></div>`;
-var ai = class extends T {
+var ci = class extends A {
     constructor() {
         super(...arguments);
         h(this, "init$", {
             ...this.init$,
             visible: !1,
-            unknown: !1,
             value: 0,
             "*commonProgress": 0
         })
     }
     initCallback() {
         super.initCallback(), this._unobserveCollection = this.uploadCollection.observeProperties(() => {
             let t = this.uploadCollection.items().some(e => this.uploadCollection.read(e).getValue("isUploading"));
@@ -6123,50 +6182,55 @@
         })
     }
     destroyCallback() {
         var t;
         super.destroyCallback(), (t = this._unobserveCollection) == null || t.call(this)
     }
 };
-ai.template = `<lr-progress-bar set="visible: visible; unknown: unknown; value: value"></lr-progress-bar>`;
-var ci = class extends w {
+ci.template = '<lr-progress-bar set="visible: visible; value: value"></lr-progress-bar>';
+var hi = class extends C {
     constructor() {
         super(...arguments);
         h(this, "_value", 0);
-        h(this, "_unknownMode", !1);
         h(this, "init$", {
             ...this.init$,
             width: 0,
             opacity: 0
         })
     }
     initCallback() {
         super.initCallback(), this.defineAccessor("value", t => {
-            t !== void 0 && (this._value = t, this._unknownMode || this.style.setProperty("--l-width", this._value.toString()))
+            if (t === void 0) return;
+            let e = this._value;
+            if (this._value = t, t === 0 && e > 0) {
+                this.ref.line.addEventListener("transitionend", () => {
+                    this.style.setProperty("--l-width", this._value.toString())
+                });
+                return
+            }
+            this.style.setProperty("--l-width", this._value.toString())
         }), this.defineAccessor("visible", t => {
             this.ref.line.classList.toggle("progress--hidden", !t)
-        }), this.defineAccessor("unknown", t => {
-            this._unknownMode = t, this.ref.line.classList.toggle("progress--unknown", t)
         })
     }
 };
-ci.template = '<div ref="line" class="progress"></div>';
-var q = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
-var me = class extends w {
+hi.template = '<div ref="line" class="progress"></div>';
+var K = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
+var fe = class extends C {
     constructor() {
         super();
         h(this, "init$", {
             ...this.init$,
             checkerboard: !1,
-            src: q
+            src: K
         })
     }
     initCallback() {
         super.initCallback(), this.sub("checkerboard", () => {
-            this.style.backgroundImage = this.hasAttribute("checkerboard") ? `url(${Fr()})` : "unset"
+            this.style.backgroundImage = this.hasAttribute("checkerboard") ? `url(${Br()})` : "unset"
         })
     }
     destroyCallback() {
         super.destroyCallback(), URL.revokeObjectURL(this._lastObjectUrl)
     }
     setImage(t) {
         this.$.src = t.src
@@ -6175,109 +6239,109 @@
         let e = URL.createObjectURL(t);
         this.$.src = e, this._lastObjectUrl = e
     }
     setImageUrl(t) {
         this.$.src = t
     }
     clear() {
-        URL.revokeObjectURL(this._lastObjectUrl), this.$.src = q
+        URL.revokeObjectURL(this._lastObjectUrl), this.$.src = K
     }
 };
-me.template = '<lr-img class="img-view" ref="img" set="@src: src; style.aa: src;" />';
-me.bindAttributes({
+fe.template = '<lr-img class="img-view" ref="img" set="@src: src; style.aa: src;" />';
+fe.bindAttributes({
     checkerboard: "checkerboard"
 });
-var Vr = "--cfg-ctx-name",
-    L = class extends w {
+var jr = "--cfg-ctx-name",
+    L = class extends C {
         get cfgCssCtxName() {
-            return this.getCssData(Vr, !0)
+            return this.getCssData(jr, !0)
         }
         get cfgCtxName() {
             var t;
             let i = ((t = this.getAttribute("ctx-name")) == null ? void 0 : t.trim()) || this.cfgCssCtxName || this.__cachedCfgCtxName;
             if (!i) throw new Error(`ctx-name attribute is required for ${this.constructor.name}`);
             return this.__cachedCfgCtxName = i, i
         }
         connectedCallback() {
             var i;
             if (!this.connectedOnce) {
                 let t = (i = this.getAttribute("ctx-name")) == null ? void 0 : i.trim();
-                t && this.style.setProperty(Vr, `'${t}'`)
+                t && this.style.setProperty(jr, `'${t}'`)
             }
             super.connectedCallback()
         }
         parseCfgProp(i) {
             return {
                 ...super.parseCfgProp(i),
                 ctx: E.getCtx(this.cfgCtxName)
             }
         }
         get debugCtxName() {
             return this.cfgCtxName
         }
     };
 
-function jr(...s) {
+function Hr(...s) {
     return s.reduce((i, t) => {
         if (typeof t == "string") return i[t] = !0, i;
         for (let e of Object.keys(t)) i[e] = t[e];
         return i
     }, {})
 }
 
 function N(...s) {
-    let i = jr(...s);
+    let i = Hr(...s);
     return Object.keys(i).reduce((t, e) => (i[e] && t.push(e), t), []).join(" ")
 }
 
-function Hr(s, ...i) {
-    let t = jr(...i);
+function Gr(s, ...i) {
+    let t = Hr(...i);
     for (let e of Object.keys(t)) s.classList.toggle(e, t[e])
 }
-var Gr = s => {
-    if (!s) return G;
-    let i = Zs(s).filter(t => G.includes(t));
-    return i.length === 0 ? G : i
+var Wr = s => {
+    if (!s) return W;
+    let i = Zs(s).filter(t => W.includes(t));
+    return i.length === 0 ? W : i
 };
 
-function Wr(s) {
+function Xr(s) {
     return {
         "*originalUrl": null,
         "*faderEl": null,
         "*cropperEl": null,
         "*imgEl": null,
         "*imgContainerEl": null,
         "*networkProblems": !1,
         "*imageSize": null,
         "*editorTransformations": {},
         "*cropPresetList": [],
-        "*tabList": G,
+        "*tabList": W,
         "*tabId": P.CROP,
         entry: null,
         extension: null,
         editorMode: !1,
         modalCaption: "",
         isImage: !1,
         msg: "",
-        src: q,
+        src: K,
         fileType: "",
         showLoader: !1,
         uuid: null,
         cdnUrl: null,
         cropPreset: "",
-        tabs: Pt(G),
+        tabs: Ht(W),
         "presence.networkProblems": !1,
         "presence.modalCaption": !0,
         "presence.editorToolbar": !1,
         "presence.viewerToolbar": !0,
         "*on.retryNetwork": () => {
             let i = s.querySelectorAll("img");
             for (let t of i) {
                 let e = t.src;
-                t.src = q, t.src = e
+                t.src = K, t.src = e
             }
             s.$["*networkProblems"] = !1
         },
         "*on.apply": i => {
             if (!i) return;
             let t = s.$["*originalUrl"],
                 e = R(wt(i), "preview"),
@@ -6298,37 +6362,37 @@
             s.remove(), s.dispatchEvent(new CustomEvent("cancel", {
                 bubbles: !0,
                 composed: !0
             }))
         }
     }
 }
-var Xr = `<div class="wrapper wrapper_desktop"><lr-presence-toggle class="network_problems_splash" set="visible: presence.networkProblems;"><div class="network_problems_content"><div class="network_problems_icon"><lr-icon size="20" name="sad"></lr-icon></div><div class="network_problems_text">Network error</div></div><div class="network_problems_footer"><lr-btn-ui theme="primary" text="Retry" set="onclick: *on.retryNetwork"></lr-btn-ui></div></lr-presence-toggle><div class="viewport"><div class="file_type_outer"><div class="file_type">{{fileType}}</div></div><div class="image_container" ref="img-container-el"><img src="${q}" class="image image_visible_from_editor" ref="img-el" /><lr-editor-image-cropper ref="cropper-el"></lr-editor-image-cropper><lr-editor-image-fader ref="fader-el"></lr-editor-image-fader></div><div class="info_pan">{{msg}}</div></div><div class="toolbar"><lr-line-loader-ui set="active: showLoader"></lr-line-loader-ui><div class="toolbar_content toolbar_content__editor"><lr-editor-toolbar></lr-editor-toolbar></div></div></div>`;
+var qr = `<div class="wrapper wrapper_desktop"><lr-presence-toggle class="network_problems_splash" set="visible: presence.networkProblems;"><div class="network_problems_content"><div class="network_problems_icon"><lr-icon size="20" name="sad"></lr-icon></div><div class="network_problems_text">Network error</div></div><div class="network_problems_footer"><lr-btn-ui theme="primary" text="Retry" set="onclick: *on.retryNetwork"></lr-btn-ui></div></lr-presence-toggle><div class="viewport"><div class="file_type_outer"><div class="file_type">{{fileType}}</div></div><div class="image_container" ref="img-container-el"><img src="${K}" class="image image_visible_from_editor" ref="img-el" /><lr-editor-image-cropper ref="cropper-el"></lr-editor-image-cropper><lr-editor-image-fader ref="fader-el"></lr-editor-image-fader></div><div class="info_pan">{{msg}}</div></div><div class="toolbar"><lr-line-loader-ui set="active: showLoader"></lr-line-loader-ui><div class="toolbar_content toolbar_content__editor"><lr-editor-toolbar></lr-editor-toolbar></div></div></div>`;
 var nt = class extends L {
     constructor() {
         super();
         h(this, "_debouncedShowLoader", k(this._showLoader.bind(this), 300));
         this.init$ = {
             ...this.init$,
-            ...Wr(this)
+            ...Xr(this)
         }
     }
     get ctxName() {
         return this.autoCtxName
     }
     _showLoader(t) {
         this.$.showLoader = t
     }
     _waitForSize() {
         return new Promise((e, r) => {
             let n = setTimeout(() => {
                     r(new Error("[cloud-image-editor] timeout waiting for non-zero container size"))
                 }, 3e3),
-                o = new ResizeObserver(([l]) => {
-                    l.contentRect.width > 0 && l.contentRect.height > 0 && (e(), clearTimeout(n), o.disconnect())
+                o = new ResizeObserver(([a]) => {
+                    a.contentRect.width > 0 && a.contentRect.height > 0 && (e(), clearTimeout(n), o.disconnect())
                 });
             o.observe(this)
         })
     }
     initCallback() {
         super.initCallback(), this.$["*faderEl"] = this.ref["fader-el"], this.$["*cropperEl"] = this.ref["cropper-el"], this.$["*imgContainerEl"] = this.ref["img-container-el"], this.initEditor()
     }
@@ -6336,15 +6400,15 @@
         if (this.isConnected) {
             if (await this._waitForSize(), this.$.cdnUrl) {
                 let t = sr(this.$.cdnUrl),
                     e = Ct(this.$.cdnUrl, t);
                 if (e === this.$["*originalUrl"]) return;
                 this.$["*originalUrl"] = e;
                 let r = rr(this.$.cdnUrl),
-                    n = gr(r);
+                    n = _r(r);
                 this.$["*editorTransformations"] = n
             } else if (this.$.uuid) {
                 let t = Ct(this.cfg.cdnCname, this.$.uuid);
                 if (t === this.$["*originalUrl"]) return;
                 this.$["*originalUrl"] = t, this.$["*editorTransformations"] = {}
             } else throw new Error("No UUID nor CDN URL provided");
             this.$["*tabId"] === P.CROP ? this.$["*cropperEl"].deactivate({
@@ -6372,24 +6436,24 @@
         try {
             await this._waitForSize()
         } catch (t) {
             this.isConnected && console.error(t.message);
             return
         }
         this.ref["img-el"].addEventListener("load", () => {
-            this._imgLoading = !1, this._debouncedShowLoader(!1), this.$.src !== q && (this.$["*networkProblems"] = !1)
+            this._imgLoading = !1, this._debouncedShowLoader(!1), this.$.src !== K && (this.$["*networkProblems"] = !1)
         }), this.ref["img-el"].addEventListener("error", () => {
             this._imgLoading = !1, this._debouncedShowLoader(!1), this.$["*networkProblems"] = !0
         }), this.sub("src", t => {
             let e = this.ref["img-el"];
-            e.src !== t && (this._imgLoading = !0, e.src = t || q)
+            e.src !== t && (this._imgLoading = !0, e.src = t || K)
         }), this.sub("cropPreset", t => {
-            this.$["*cropPresetList"] = Fe(t)
+            this.$["*cropPresetList"] = De(t)
         }), this.sub("tabs", t => {
-            this.$["*tabList"] = Gr(t)
+            this.$["*tabList"] = Wr(t)
         }), this.sub("*tabId", t => {
             this.ref["img-el"].className = N("image", {
                 image_hidden_to_cropper: t === P.CROP,
                 image_hidden_effects: t !== P.CROP
             })
         }), this.classList.add("editor_ON"), this.sub("*networkProblems", t => {
             this.$["presence.networkProblems"] = t, this.$["presence.modalCaption"] = !t
@@ -6409,70 +6473,70 @@
                 bubbles: !0,
                 composed: !0
             }))
         }, !1), this.sub("uuid", t => t && this.updateImage()), this.sub("cdnUrl", t => t && this.updateImage())
     }
 };
 h(nt, "className", "cloud-image-editor");
-nt.template = Xr;
+nt.template = qr;
 nt.bindAttributes({
     uuid: "uuid",
     "cdn-url": "cdnUrl",
     "crop-preset": "cropPreset",
     tabs: "tabs"
 });
-var hi = class extends L {
+var ui = class extends L {
     constructor() {
         super(), this.init$ = {
             ...this.init$,
             dragging: !1
         }, this._handlePointerUp = this._handlePointerUp_.bind(this), this._handlePointerMove = this._handlePointerMove_.bind(this), this._handleSvgPointerMove = this._handleSvgPointerMove_.bind(this)
     }
     _shouldThumbBeDisabled(i) {
         let t = this.$["*imageBox"];
         if (!t) return;
-        if (i === "" && t.height <= y && t.width <= y) return !0;
-        let e = t.height <= y && (i.includes("n") || i.includes("s")),
-            r = t.width <= y && (i.includes("e") || i.includes("w"));
+        if (i === "" && t.height <= b && t.width <= b) return !0;
+        let e = t.height <= b && (i.includes("n") || i.includes("s")),
+            r = t.width <= b && (i.includes("e") || i.includes("w"));
         return e || r
     }
     _createBackdrop() {
         let i = this.$["*cropBox"];
         if (!i) return;
         let {
             x: t,
             y: e,
             width: r,
             height: n
-        } = i, o = this.ref["svg-el"], l = K("mask", {
+        } = i, o = this.ref["svg-el"], a = Y("mask", {
             id: "backdrop-mask"
-        }), a = K("rect", {
+        }), l = Y("rect", {
             x: 0,
             y: 0,
             width: "100%",
             height: "100%",
             fill: "white"
-        }), c = K("rect", {
+        }), c = Y("rect", {
             x: t,
             y: e,
             width: r,
             height: n,
             fill: "black"
         });
-        l.appendChild(a), l.appendChild(c);
-        let u = K("rect", {
+        a.appendChild(l), a.appendChild(c);
+        let u = Y("rect", {
             x: 0,
             y: 0,
             width: "100%",
             height: "100%",
             fill: "var(--color-image-background)",
             "fill-opacity": .85,
             mask: "url(#backdrop-mask)"
         });
-        o.appendChild(u), o.appendChild(l), this._backdropMask = l, this._backdropMaskInner = c
+        o.appendChild(u), o.appendChild(a), this._backdropMask = a, this._backdropMaskInner = c
     }
     _resizeBackdrop() {
         this._backdropMask && (this._backdropMask.style.display = "none", window.requestAnimationFrame(() => {
             this._backdropMask && (this._backdropMask.style.display = "block")
         }))
     }
     _updateBackdrop() {
@@ -6496,38 +6560,38 @@
         if (!(!i || !this._frameGuides || !this._frameThumbs)) {
             for (let t of Object.values(this._frameThumbs)) {
                 let {
                     direction: e,
                     pathNode: r,
                     interactionNode: n,
                     groupNode: o
-                } = t, l = e === "", a = e.length === 2, {
+                } = t, a = e === "", l = e.length === 2, {
                     x: c,
                     y: u,
                     width: d,
                     height: p
                 } = i;
-                if (l) {
+                if (a) {
                     let f = {
                         x: c + d / 3,
                         y: u + p / 3,
                         width: d / 3,
                         height: p / 3
                     };
                     Ot(n, f)
                 } else {
                     let f = vt(Math.min(d, p) / (24 * 2 + 34) / 2, 0, 1),
                         {
                             d: _,
-                            center: b
-                        } = a ? js(i, e, f) : Hs(i, e, f),
-                        x = Math.max(Wi * vt(Math.min(d, p) / Wi / 3, 0, 1), Vs);
+                            center: y
+                        } = l ? js(i, e, f) : Hs(i, e, f),
+                        x = Math.max(Xi * vt(Math.min(d, p) / Xi / 3, 0, 1), Vs);
                     Ot(n, {
-                        x: b[0] - x,
-                        y: b[1] - x,
+                        x: y[0] - x,
+                        y: y[1] - x,
                         width: x * 2,
                         height: x * 2
                     }), Ot(r, {
                         d: _
                     })
                 }
                 let m = this._shouldThumbBeDisabled(e);
@@ -6545,60 +6609,60 @@
         }
     }
     _createThumbs() {
         let i = {};
         for (let t = 0; t < 3; t++)
             for (let e = 0; e < 3; e++) {
                 let r = `${["n","","s"][t]}${["w","","e"][e]}`,
-                    n = K("g");
+                    n = Y("g");
                 n.classList.add("thumb"), n.setAttribute("with-effects", "");
-                let o = K("rect", {
+                let o = Y("rect", {
                         fill: "transparent"
                     }),
-                    l = K("path", {
+                    a = Y("path", {
                         stroke: "currentColor",
                         fill: "none",
                         "stroke-width": 3
                     });
-                n.appendChild(l), n.appendChild(o), i[r] = {
+                n.appendChild(a), n.appendChild(o), i[r] = {
                     direction: r,
-                    pathNode: l,
+                    pathNode: a,
                     interactionNode: o,
                     groupNode: n
                 }, o.addEventListener("pointerdown", this._handlePointerDown.bind(this, r))
             }
         return i
     }
     _createGuides() {
-        let i = K("svg"),
-            t = K("rect", {
+        let i = Y("svg"),
+            t = Y("rect", {
                 x: 0,
                 y: 0,
                 width: "100%",
                 height: "100%",
                 fill: "none",
                 stroke: "#000000",
                 "stroke-width": 1,
                 "stroke-opacity": .5
             });
         i.appendChild(t);
         for (let e = 1; e <= 2; e++) {
-            let r = K("line", {
+            let r = Y("line", {
                 x1: `${ee*e}%`,
                 y1: "0%",
                 x2: `${ee*e}%`,
                 y2: "100%",
                 stroke: "#000000",
                 "stroke-width": 1,
                 "stroke-opacity": .3
             });
             i.appendChild(r)
         }
         for (let e = 1; e <= 2; e++) {
-            let r = K("line", {
+            let r = Y("line", {
                 x1: "0%",
                 y1: `${ee*e}%`,
                 x2: "100%",
                 y2: `${ee*e}%`,
                 stroke: "#000000",
                 "stroke-width": 1,
                 "stroke-opacity": .3
@@ -6624,17 +6688,17 @@
         let e = this._frameThumbs[i];
         if (this._shouldThumbBeDisabled(i)) return;
         let r = this.$["*cropBox"],
             {
                 x: n,
                 y: o
             } = this.ref["svg-el"].getBoundingClientRect(),
-            l = t.x - n,
-            a = t.y - o;
-        this.$.dragging = !0, this._draggingThumb = e, this._dragStartPoint = [l, a], this._dragStartCrop = {
+            a = t.x - n,
+            l = t.y - o;
+        this.$.dragging = !0, this._draggingThumb = e, this._dragStartPoint = [a, l], this._dragStartCrop = {
             ...r
         }
     }
     _handlePointerUp_(i) {
         this._updateCursor(), this.$.dragging && (i.stopPropagation(), i.preventDefault(), this.$.dragging = !1)
     }
     _handlePointerMove_(i) {
@@ -6643,42 +6707,42 @@
         let t = this.ref["svg-el"],
             {
                 x: e,
                 y: r
             } = t.getBoundingClientRect(),
             n = i.x - e,
             o = i.y - r,
-            l = n - this._dragStartPoint[0],
-            a = o - this._dragStartPoint[1],
+            a = n - this._dragStartPoint[0],
+            l = o - this._dragStartPoint[1],
             {
                 direction: c
             } = this._draggingThumb,
-            u = this._calcCropBox(c, [l, a]);
+            u = this._calcCropBox(c, [a, l]);
         u && (this.$["*cropBox"] = u)
     }
     _calcCropBox(i, t) {
         var c, u;
-        let [e, r] = t, n = this.$["*imageBox"], o = (c = this._dragStartCrop) != null ? c : this.$["*cropBox"], l = (u = this.$["*cropPresetList"]) == null ? void 0 : u[0], a = l ? l.width / l.height : void 0;
+        let [e, r] = t, n = this.$["*imageBox"], o = (c = this._dragStartCrop) != null ? c : this.$["*cropBox"], a = (u = this.$["*cropPresetList"]) == null ? void 0 : u[0], l = a ? a.width / a.height : void 0;
         if (i === "" ? o = Ws({
                 rect: o,
                 delta: [e, r],
                 imageBox: n
             }) : o = Xs({
                 rect: o,
                 delta: [e, r],
                 direction: i,
-                aspectRatio: a,
+                aspectRatio: l,
                 imageBox: n
             }), !Object.values(o).every(d => Number.isFinite(d) && d >= 0)) {
             console.error("CropFrame is trying to create invalid rectangle", {
                 payload: o
             });
             return
         }
-        return Vt(Ht(o), this.$["*imageBox"])
+        return zt(jt(o), this.$["*imageBox"])
     }
     _handleSvgPointerMove_(i) {
         if (!this._frameThumbs) return;
         let t = Object.values(this._frameThumbs).find(e => {
             if (this._shouldThumbBeDisabled(e.direction)) return !1;
             let n = e.interactionNode.getBoundingClientRect(),
                 o = {
@@ -6710,30 +6774,30 @@
     }
     initCallback() {
         super.initCallback(), this._createBackdrop(), this._createFrame(), this.sub("*imageBox", () => {
             this._resizeBackdrop(), window.requestAnimationFrame(() => {
                 this._render()
             })
         }), this.sub("*cropBox", i => {
-            i && (this._guidesHidden = i.height <= y || i.width <= y, window.requestAnimationFrame(() => {
+            i && (this._guidesHidden = i.height <= b || i.width <= b, window.requestAnimationFrame(() => {
                 this._render()
             }))
         }), this.sub("dragging", i => {
             this._frameGuides && this._frameGuides.setAttribute("class", N({
                 "guides--hidden": this._guidesHidden,
                 "guides--visible": !this._guidesHidden && i,
                 "guides--semi-hidden": !this._guidesHidden && !i
             }))
         }), this.ref["svg-el"].addEventListener("pointermove", this._handleSvgPointerMove, !0), document.addEventListener("pointermove", this._handlePointerMove, !0), document.addEventListener("pointerup", this._handlePointerUp, !0)
     }
     destroyCallback() {
         super.destroyCallback(), document.removeEventListener("pointermove", this._handlePointerMove), document.removeEventListener("pointerup", this._handlePointerUp)
     }
 };
-hi.template = '<svg class="svg" ref="svg-el" xmlns="http://www.w3.org/2000/svg"></svg>';
+ui.template = '<svg class="svg" ref="svg-el" xmlns="http://www.w3.org/2000/svg"></svg>';
 var mt = class extends L {
     constructor() {
         super(...arguments);
         h(this, "init$", {
             ...this.init$,
             active: !1,
             title: "",
@@ -6752,39 +6816,39 @@
         }), this.sub("on.click", t => {
             this.onclick = t
         })
     }
 };
 mt.template = `<div class="before"></div><lr-icon size="20" set="@name: icon;"></lr-icon><div class="title" ref="title-el">{{title}}</div>`;
 
-function Il(s) {
+function Pa(s) {
     let i = s + 90;
     return i = i >= 360 ? 0 : i, i
 }
 
-function kl(s, i) {
-    return s === "rotate" ? Il(i) : ["mirror", "flip"].includes(s) ? !i : null
+function La(s, i) {
+    return s === "rotate" ? Pa(i) : ["mirror", "flip"].includes(s) ? !i : null
 }
-var ge = class extends mt {
+var me = class extends mt {
     initCallback() {
         super.initCallback(), this.defineAccessor("operation", i => {
             i && (this._operation = i, this.$.icon = i)
         }), this.$["on.click"] = i => {
             let t = this.$["*cropperEl"].getValue(this._operation),
-                e = kl(this._operation, t);
+                e = La(this._operation, t);
             this.$["*cropperEl"].setValue(this._operation, e)
         }
     }
 };
-var _e = {
+var ge = {
         FILTER: "filter",
         COLOR_OPERATION: "color_operation"
     },
     ot = "original",
-    ui = class extends L {
+    di = class extends L {
         constructor() {
             super(...arguments);
             h(this, "init$", {
                 ...this.init$,
                 disabled: !1,
                 min: 0,
                 max: 100,
@@ -6793,48 +6857,48 @@
                 zero: 0,
                 "on.input": t => {
                     this.$["*faderEl"].set(t), this.$.value = t
                 }
             })
         }
         setOperation(t, e) {
-            this._controlType = t === "filter" ? _e.FILTER : _e.COLOR_OPERATION, this._operation = t, this._iconName = t, this._title = t.toUpperCase(), this._filter = e, this._initializeValues(), this.$["*faderEl"].activate({
+            this._controlType = t === "filter" ? ge.FILTER : ge.COLOR_OPERATION, this._operation = t, this._iconName = t, this._title = t.toUpperCase(), this._filter = e, this._initializeValues(), this.$["*faderEl"].activate({
                 url: this.$["*originalUrl"],
                 operation: this._operation,
                 value: this._filter === ot ? void 0 : this.$.value,
                 filter: this._filter === ot ? void 0 : this._filter,
                 fromViewer: !1
             })
         }
         _initializeValues() {
             let {
                 range: t,
                 zero: e
             } = st[this._operation], [r, n] = t;
             this.$.min = r, this.$.max = n, this.$.zero = e;
             let o = this.$["*editorTransformations"][this._operation];
-            if (this._controlType === _e.FILTER) {
-                let l = n;
+            if (this._controlType === ge.FILTER) {
+                let a = n;
                 if (o) {
                     let {
-                        name: a,
+                        name: l,
                         amount: c
                     } = o;
-                    l = a === this._filter ? c : n
+                    a = l === this._filter ? c : n
                 }
-                this.$.value = l, this.$.defaultValue = l
+                this.$.value = a, this.$.defaultValue = a
             }
-            if (this._controlType === _e.COLOR_OPERATION) {
-                let l = typeof o != "undefined" ? o : e;
-                this.$.value = l, this.$.defaultValue = l
+            if (this._controlType === ge.COLOR_OPERATION) {
+                let a = typeof o != "undefined" ? o : e;
+                this.$.value = a, this.$.defaultValue = a
             }
         }
         apply() {
             let t;
-            this._controlType === _e.FILTER ? this._filter === ot ? t = null : t = {
+            this._controlType === ge.FILTER ? this._filter === ot ? t = null : t = {
                 name: this._filter,
                 amount: this.$.value
             } : t = this.$.value;
             let e = {
                 ...this.$["*editorTransformations"],
                 [this._operation]: t
             };
@@ -6850,33 +6914,33 @@
                 this._originalUrl = t
             }), this.sub("value", t => {
                 let e = `${this._filter||this._operation} ${t}`;
                 this.$["*operationTooltip"] = e
             })
         }
     };
-ui.template = `<lr-slider-ui ref="slider-el" set="disabled: disabled; min: min; max: max; defaultValue: defaultValue; zero: zero; onInput: on.input;" ></lr-slider-ui>`;
+di.template = `<lr-slider-ui ref="slider-el" set="disabled: disabled; min: min; max: max; defaultValue: defaultValue; zero: zero; onInput: on.input;" ></lr-slider-ui>`;
 
-function be(s) {
+function _e(s) {
     let i = new Image;
     return {
         promise: new Promise((r, n) => {
             i.src = s, i.onload = r, i.onerror = n
         }),
         image: i,
         cancel: () => {
-            i.naturalWidth === 0 && (i.src = q)
+            i.naturalWidth === 0 && (i.src = K)
         }
     }
 }
 
-function ye(s) {
+function be(s) {
     let i = [];
     for (let n of s) {
-        let o = be(n);
+        let o = _e(n);
         i.push(o)
     }
     let t = i.map(n => n.image);
     return {
         promise: Promise.allSettled(i.map(n => n.promise)),
         images: t,
         cancel: () => {
@@ -6901,31 +6965,31 @@
     }
     _previewSrc() {
         let t = parseInt(window.getComputedStyle(this).getPropertyValue("--l-base-min-width"), 10),
             e = window.devicePixelRatio,
             r = Math.ceil(e * t),
             n = e >= 2 ? "lightest" : "normal",
             o = 100,
-            l = {
+            a = {
                 ...this.$["*editorTransformations"]
             };
-        return l[this._operation] = this._filter !== ot ? {
+        return a[this._operation] = this._filter !== ot ? {
             name: this._filter,
             amount: o
-        } : void 0, O(this._originalUrl, R(Xe, wt(l), `quality/${n}`, `scale_crop/${r}x${r}/center`))
+        } : void 0, O(this._originalUrl, R(We, wt(a), `quality/${n}`, `scale_crop/${r}x${r}/center`))
     }
     _observerCallback(t, e) {
         if (t[0].isIntersecting) {
             let n = this.proxyUrl(this._previewSrc()),
                 o = this.ref["preview-el"],
                 {
-                    promise: l,
-                    cancel: a
-                } = be(n);
-            this._cancelPreload = a, l.catch(c => {
+                    promise: a,
+                    cancel: l
+                } = _e(n);
+            this._cancelPreload = l, a.catch(c => {
                 this.$["*networkProblems"] = !0, console.error("Failed to load image", {
                     error: c
                 })
             }).finally(() => {
                 o.style.backgroundImage = `url(${n})`, o.setAttribute("loaded", ""), e.unobserve(this)
             })
         } else this._cancelPreload && this._cancelPreload()
@@ -6959,15 +7023,15 @@
     }
     destroyCallback() {
         var t;
         super.destroyCallback(), (t = this._observer) == null || t.disconnect(), this._cancelPreload && this._cancelPreload()
     }
 };
 Xt.template = `<div class="before"></div><div class="preview" ref="preview-el"></div><lr-icon size="40" ref="icon-el" set="@name: icon; @size: iconSize;"></lr-icon>`;
-var ve = class extends mt {
+var ye = class extends mt {
     constructor() {
         super(...arguments);
         h(this, "_operation", "")
     }
     initCallback() {
         super.initCallback(), this.$["on.click"] = t => {
             this.$["*sliderEl"].setOperation(this._operation), this.$["*showSlider"] = !0, this.$["*currentOperation"] = this._operation
@@ -6979,40 +7043,40 @@
                 zero: e
             } = st[this._operation], r = t[this._operation], n = typeof r != "undefined" ? r !== e : !1;
             this.$.active = n
         })
     }
 };
 
-function qr(s, i) {
+function Kr(s, i) {
     let t = {};
     for (let e of i) {
         let r = s[e];
         (s.hasOwnProperty(e) || r !== void 0) && (t[e] = r)
     }
     return t
 }
 
 function qt(s, i, t) {
     let r = window.devicePixelRatio,
         n = Math.min(Math.ceil(i * r), 3e3),
         o = r >= 2 ? "lightest" : "normal";
-    return O(s, R(Xe, wt(t), `quality/${o}`, `stretch/off/-/resize/${n}x`))
+    return O(s, R(We, wt(t), `quality/${o}`, `stretch/off/-/resize/${n}x`))
 }
 
-function Ol(s) {
+function Ua(s) {
     return s ? [({
         dimensions: t,
         coords: e
     }) => [...t, ...e].every(r => Number.isInteger(r) && Number.isFinite(r)), ({
         dimensions: t,
         coords: e
     }) => t.every(r => r > 0) && e.every(r => r >= 0)].every(t => t(s)) : !0
 }
-var di = class extends L {
+var pi = class extends L {
     constructor() {
         super(), this.init$ = {
             ...this.init$,
             image: null,
             "*padding": 20,
             "*operations": {
                 rotate: 0,
@@ -7027,25 +7091,25 @@
             },
             "*cropBox": {
                 x: 0,
                 y: 0,
                 width: 0,
                 height: 0
             }
-        }, this._commitDebounced = k(this._commit.bind(this), 300), this._handleResizeThrottled = We(this._handleResize.bind(this), 100), this._imageSize = {
+        }, this._commitDebounced = k(this._commit.bind(this), 300), this._handleResizeThrottled = ii(this._handleResize.bind(this), 100), this._imageSize = {
             width: 0,
             height: 0
         }
     }
     _handleResize() {
         !this.isConnected || !this._isActive || (this._initCanvas(), this._syncTransformations(), this._alignImage(), this._alignCrop(), this._draw())
     }
     _syncTransformations() {
         let i = this.$["*editorTransformations"],
-            t = qr(i, Object.keys(this.$["*operations"])),
+            t = Kr(i, Object.keys(this.$["*operations"])),
             e = {
                 ...this.$["*operations"],
                 ...t
             };
         this.$["*operations"] = e
     }
     _initCanvas() {
@@ -7064,83 +7128,83 @@
             {
                 rotate: r
             } = e,
             n = {
                 width: this.offsetWidth,
                 height: this.offsetHeight
             },
-            o = jt({
+            o = Vt({
                 width: i.naturalWidth,
                 height: i.naturalHeight
             }, r),
-            l;
+            a;
         if (o.width > n.width - t * 2 || o.height > n.height - t * 2) {
-            let a = o.width / o.height,
+            let l = o.width / o.height,
                 c = n.width / n.height;
-            if (a > c) {
+            if (l > c) {
                 let u = n.width - t * 2,
-                    d = u / a,
+                    d = u / l,
                     p = 0 + t,
                     m = t + (n.height - t * 2) / 2 - d / 2;
-                l = {
+                a = {
                     x: p,
                     y: m,
                     width: u,
                     height: d
                 }
             } else {
                 let u = n.height - t * 2,
-                    d = u * a,
+                    d = u * l,
                     p = t + (n.width - t * 2) / 2 - d / 2,
                     m = 0 + t;
-                l = {
+                a = {
                     x: p,
                     y: m,
                     width: d,
                     height: u
                 }
             }
         } else {
             let {
-                width: a,
+                width: l,
                 height: c
-            } = o, u = t + (n.width - t * 2) / 2 - a / 2, d = t + (n.height - t * 2) / 2 - c / 2;
-            l = {
+            } = o, u = t + (n.width - t * 2) / 2 - l / 2, d = t + (n.height - t * 2) / 2 - c / 2;
+            a = {
                 x: u,
                 y: d,
-                width: a,
+                width: l,
                 height: c
             }
         }
-        this.$["*imageBox"] = Ht(l)
+        this.$["*imageBox"] = jt(a)
     }
     _alignCrop() {
         var d;
         let i = this.$["*cropBox"],
             t = this.$["*imageBox"],
             e = this.$["*operations"],
             {
                 rotate: r
             } = e,
             n = this.$["*editorTransformations"].crop,
             {
                 width: o,
-                x: l,
-                y: a
+                x: a,
+                y: l
             } = this.$["*imageBox"];
         if (n) {
             let {
                 dimensions: [p, m],
                 coords: [f, _]
             } = n, {
-                width: b
-            } = jt(this._imageSize, r), x = o / b;
-            i = Vt(Ht({
-                x: l + f * x,
-                y: a + _ * x,
+                width: y
+            } = Vt(this._imageSize, r), x = o / y;
+            i = zt(jt({
+                x: a + f * x,
+                y: l + _ * x,
                 width: p * x,
                 height: m * x
             }), this.$["*imageBox"])
         }
         let c = (d = this.$["*cropPresetList"]) == null ? void 0 : d[0],
             u = c ? c.width / c.height : void 0;
         if (!Ks(i, t) || u && !Ys(i, u)) {
@@ -7150,32 +7214,32 @@
             u && (p > u ? m = Math.min(t.height * u, t.width) : f = Math.min(t.width / u, t.height)), i = {
                 x: t.x + t.width / 2 - m / 2,
                 y: t.y + t.height / 2 - f / 2,
                 width: m,
                 height: f
             }
         }
-        this.$["*cropBox"] = Vt(Ht(i), this.$["*imageBox"])
+        this.$["*cropBox"] = zt(jt(i), this.$["*imageBox"])
     }
     _drawImage() {
         let i = this._ctx;
         if (!i) return;
         let t = this.$.image,
             e = this.$["*imageBox"],
             r = this.$["*operations"],
             {
                 mirror: n,
                 flip: o,
-                rotate: l
+                rotate: a
             } = r,
-            a = jt({
+            l = Vt({
                 width: e.width,
                 height: e.height
-            }, l);
-        i.save(), i.translate(e.x + e.width / 2, e.y + e.height / 2), i.rotate(l * Math.PI * -1 / 180), i.scale(n ? -1 : 1, o ? -1 : 1), i.drawImage(t, -a.width / 2, -a.height / 2, a.width, a.height), i.restore()
+            }, a);
+        i.save(), i.translate(e.x + e.width / 2, e.y + e.height / 2), i.rotate(a * Math.PI * -1 / 180), i.scale(n ? -1 : 1, o ? -1 : 1), i.drawImage(t, -l.width / 2, -l.height / 2, l.width, l.height), i.restore()
     }
     _draw() {
         if (!this._isActive || !this.$.image || !this._canvas || !this._ctx) return;
         let i = this._canvas;
         this._ctx.clearRect(0, 0, i.width, i.height), this._drawImage()
     }
     _animateIn({
@@ -7197,78 +7261,78 @@
                 rotate: r
             } = e,
             {
                 width: n,
                 height: o
             } = t,
             {
-                width: l,
-                height: a
-            } = jt(this._imageSize, r),
+                width: a,
+                height: l
+            } = Vt(this._imageSize, r),
             {
                 width: c,
                 height: u
             } = i,
-            d = n / l,
-            p = o / a;
-        return [vt(Math.round(c / d), 1, l), vt(Math.round(u / p), 1, a)]
+            d = n / a,
+            p = o / l;
+        return [vt(Math.round(c / d), 1, a), vt(Math.round(u / p), 1, l)]
     }
     _getCropTransformation() {
         let i = this.$["*cropBox"],
             t = this.$["*imageBox"],
             e = this.$["*operations"],
             {
                 rotate: r
             } = e,
             {
                 width: n,
                 height: o,
-                x: l,
-                y: a
+                x: a,
+                y: l
             } = t,
             {
                 width: c,
                 height: u
-            } = jt(this._imageSize, r),
+            } = Vt(this._imageSize, r),
             {
                 x: d,
                 y: p
             } = i,
             m = n / c,
             f = o / u,
             _ = this._getCropDimensions(),
-            b = {
+            y = {
                 dimensions: _,
-                coords: [vt(Math.round((d - l) / m), 0, c - _[0]), vt(Math.round((p - a) / f), 0, u - _[1])]
+                coords: [vt(Math.round((d - a) / m), 0, c - _[0]), vt(Math.round((p - l) / f), 0, u - _[1])]
             };
-        if (!Ol(b)) {
+        if (!Ua(y)) {
             console.error("Cropper is trying to create invalid crop object", {
-                payload: b
+                payload: y
             });
             return
         }
-        if (!(_[0] === c && _[1] === u)) return b
+        if (!(_[0] === c && _[1] === u)) return y
     }
     _commit() {
         if (!this.isConnected) return;
         let i = this.$["*operations"],
             {
                 rotate: t,
                 mirror: e,
                 flip: r
             } = i,
             n = this._getCropTransformation(),
-            l = {
+            a = {
                 ...this.$["*editorTransformations"],
                 crop: n,
                 rotate: t,
                 mirror: e,
                 flip: r
             };
-        this.$["*editorTransformations"] = l
+        this.$["*editorTransformations"] = a
     }
     setValue(i, t) {
         this.$["*operations"] = {
             ...this.$["*operations"],
             [i]: t
         }, this._isActive && (this._alignImage(), this._alignCrop(), this._draw())
     }
@@ -7332,24 +7396,24 @@
             flip: void 0,
             mirror: void 0
         };
         let r = this.proxyUrl(qt(i, e, t)),
             {
                 promise: n,
                 cancel: o,
-                image: l
-            } = be(r),
-            a = this._handleImageLoading(r);
-        return l.addEventListener("load", a, {
+                image: a
+            } = _e(r),
+            l = this._handleImageLoading(r);
+        return a.addEventListener("load", l, {
             once: !0
-        }), l.addEventListener("error", a, {
+        }), a.addEventListener("error", l, {
             once: !0
-        }), this._cancelPreload && this._cancelPreload(), this._cancelPreload = o, n.then(() => l).catch(c => (console.error("Failed to load image", {
+        }), this._cancelPreload && this._cancelPreload(), this._cancelPreload = o, n.then(() => a).catch(c => (console.error("Failed to load image", {
             error: c
-        }), this.$["*networkProblems"] = !0, Promise.resolve(l)))
+        }), this.$["*networkProblems"] = !0, Promise.resolve(a)))
     }
     _handleImageLoading(i) {
         let t = "crop",
             e = this.$["*loadingOperations"];
         return e.get(t) || e.set(t, new Map), e.get(t).get(i) || (e.set(t, e.get(t).set(i, !0)), this.$["*loadingOperations"] = e), () => {
             var r;
             (r = e == null ? void 0 : e.get(t)) != null && r.has(i) && (e.get(t).delete(i), this.$["*loadingOperations"] = e)
@@ -7371,47 +7435,47 @@
         }, 0)
     }
     destroyCallback() {
         var i;
         super.destroyCallback(), (i = this._observer) == null || i.disconnect()
     }
 };
-di.template = `<canvas class="canvas" ref="canvas-el"></canvas><lr-crop-frame ref="frame-el"></lr-crop-frame>`;
+pi.template = `<canvas class="canvas" ref="canvas-el"></canvas><lr-crop-frame ref="frame-el"></lr-crop-frame>`;
 
-function as(s, i, t) {
+function ls(s, i, t) {
     let e = Array(t);
     t--;
     for (let r = t; r >= 0; r--) e[r] = Math.ceil((r * i + (t - r) * s) / t);
     return e
 }
 
-function Pl(s) {
+function Ra(s) {
     return s.reduce((i, t, e) => e < s.length - 1 ? [...i, [t, s[e + 1]]] : i, [])
 }
 
-function Ll(s, i, t) {
-    let e = Pl(s).find(([r, n]) => r <= i && i <= n);
+function Ma(s, i, t) {
+    let e = Ra(s).find(([r, n]) => r <= i && i <= n);
     return s.map(r => {
         let n = Math.abs(e[0] - e[1]),
             o = Math.abs(i - e[0]) / n;
         return e[0] === r ? i > t ? 1 : 1 - o : e[1] === r ? i >= t ? o : 1 : 0
     })
 }
 
-function Ul(s, i) {
+function Na(s, i) {
     return s.map((t, e) => t < i ? s.length - e : e)
 }
 
-function Kr(s, i) {
+function Yr(s, i) {
     let t = st[s].keypointsNumber,
         {
             range: e,
             zero: r
         } = st[s];
-    return [...new Set([...as(e[0], r, t + 1), ...as(r, e[1], t + 1), r, i])].sort((n, o) => n - o)
+    return [...new Set([...ls(e[0], r, t + 1), ...ls(r, e[1], t + 1), r, i])].sort((n, o) => n - o)
 }
 var cs = class extends L {
     constructor() {
         super(), this._isActive = !1, this._hidden = !0, this._addKeypointDebounced = k(this._addKeypoint.bind(this), 600), this.classList.add("inactive_to_cropper")
     }
     _handleImageLoading(i) {
         let t = this._operation,
@@ -7459,30 +7523,30 @@
             value: t
         }
     }
     _isSame(i, t) {
         return this._operation === i && this._filter === t
     }
     _addKeypoint(i, t, e) {
-        let r = () => !this._isSame(i, t) || this._value !== e || !!this._keypoints.find(a => a.value === e);
+        let r = () => !this._isSame(i, t) || this._value !== e || !!this._keypoints.find(l => l.value === e);
         if (r()) return;
         let n = this._constructKeypoint(i, e),
             o = new Image;
         o.src = n.src;
-        let l = this._handleImageLoading(n.src);
-        o.addEventListener("load", l, {
+        let a = this._handleImageLoading(n.src);
+        o.addEventListener("load", a, {
             once: !0
-        }), o.addEventListener("error", l, {
+        }), o.addEventListener("error", a, {
             once: !0
         }), n.image = o, o.classList.add("fader-image"), o.addEventListener("load", () => {
             if (r()) return;
-            let a = this._keypoints,
-                c = a.findIndex(d => d.value > e),
-                u = c < a.length ? a[c].image : null;
-            !this._container || u && !this._container.contains(u) || (a.splice(c, 0, n), this._container.insertBefore(o, u), this._update(i, e))
+            let l = this._keypoints,
+                c = l.findIndex(d => d.value > e),
+                u = c < l.length ? l[c].image : null;
+            !this._container || u && !this._container.contains(u) || (l.splice(c, 0, n), this._container.insertBefore(o, u), this._update(i, e))
         }, {
             once: !0
         }), o.addEventListener("error", () => {
             this.$["*networkProblems"] = !0
         }, {
             once: !0
         })
@@ -7490,16 +7554,16 @@
     set(i) {
         i = typeof i == "string" ? parseInt(i, 10) : i, this._update(this._operation, i), this._addKeypointDebounced(this._operation, this._filter, i)
     }
     _update(i, t) {
         this._operation = i, this._value = t;
         let {
             zero: e
-        } = st[i], r = this._keypoints.map(l => l.value), n = Ll(r, t, e), o = Ul(r, e);
-        for (let [l, a] of Object.entries(this._keypoints)) a.opacity = n[l], a.zIndex = o[l];
+        } = st[i], r = this._keypoints.map(a => a.value), n = Ma(r, t, e), o = Na(r, e);
+        for (let [a, l] of Object.entries(this._keypoints)) l.opacity = n[a], l.zIndex = o[a];
         this._flush()
     }
     _createPreviewImage() {
         let i = new Image;
         return i.classList.add("fader-image", "fader-image--preview"), i.style.opacity = "0", i
     }
     async _initNodes() {
@@ -7508,24 +7572,24 @@
         let t = document.createElement("div");
         i.appendChild(t);
         let e = this._keypoints.map(c => c.src),
             {
                 images: r,
                 promise: n,
                 cancel: o
-            } = ye(e);
+            } = be(e);
         r.forEach(c => {
             let u = this._handleImageLoading(c.src);
             c.addEventListener("load", u), c.addEventListener("error", u)
         }), this._cancelLastImages = () => {
             o(), this._cancelLastImages = void 0
         };
-        let l = this._operation,
-            a = this._filter;
-        await n, this._isActive && this._isSame(l, a) && (this._container && this._container.remove(), this._container = t, this._keypoints.forEach((c, u) => {
+        let a = this._operation,
+            l = this._filter;
+        await n, this._isActive && this._isSame(a, l) && (this._container && this._container.remove(), this._container = t, this._keypoints.forEach((c, u) => {
             let d = r[u];
             d.classList.add("fader-image"), c.image = d, this._container.appendChild(d)
         }), this.appendChild(i), this._flush())
     }
     setTransformations(i) {
         if (this._transformations = i, this._previewImage) {
             let t = this._imageSrc(),
@@ -7544,24 +7608,24 @@
     preload({
         url: i,
         filter: t,
         operation: e,
         value: r
     }) {
         this._cancelBatchPreload && this._cancelBatchPreload();
-        let o = Kr(e, r).map(a => this._imageSrc({
+        let o = Yr(e, r).map(l => this._imageSrc({
                 url: i,
                 filter: t,
                 operation: e,
-                value: a
+                value: l
             })),
             {
-                cancel: l
-            } = ye(o);
-        this._cancelBatchPreload = l
+                cancel: a
+            } = be(o);
+        this._cancelBatchPreload = a
     }
     _setOriginalSrc(i) {
         let t = this._previewImage || this._createPreviewImage();
         if (!this.contains(t) && this.appendChild(t), this._previewImage = t, t.src === i) {
             t.style.opacity = "1", t.style.transform = "scale(1)", this.className = N({
                 active_from_viewer: this._fromViewer,
                 active_from_cropper: !this._fromViewer,
@@ -7591,22 +7655,22 @@
         url: i,
         operation: t,
         value: e,
         filter: r,
         fromViewer: n
     }) {
         if (this._isActive = !0, this._hidden = !1, this._url = i, this._operation = t || "initial", this._value = e, this._filter = r, this._fromViewer = n, typeof e != "number" && !r) {
-            let l = this._imageSrc({
+            let a = this._imageSrc({
                 operation: t,
                 value: e
             });
-            this._setOriginalSrc(l), this._container && this._container.remove();
+            this._setOriginalSrc(a), this._container && this._container.remove();
             return
         }
-        this._keypoints = Kr(t, e).map(l => this._constructKeypoint(t, l)), this._update(t, e), this._initNodes()
+        this._keypoints = Yr(t, e).map(a => this._constructKeypoint(t, a)), this._update(t, e), this._initNodes()
     }
     deactivate({
         hide: i = !0
     } = {}) {
         this._isActive = !1, this._cancelLastImages && this._cancelLastImages(), this._cancelBatchPreload && this._cancelBatchPreload(), i && !this._hidden ? (this._hidden = !0, this._previewImage && (this._previewImage.style.transform = "scale(1)"), this.className = N({
             active_from_viewer: !1,
             active_from_cropper: !1,
@@ -7614,68 +7678,68 @@
         }), this.addEventListener("transitionend", () => {
             this._container && this._container.remove()
         }, {
             once: !0
         })) : this._container && this._container.remove()
     }
 };
-var Rl = 1,
-    pi = class extends L {
+var Da = 1,
+    fi = class extends L {
         initCallback() {
             super.initCallback(), this.addEventListener("wheel", i => {
                 i.preventDefault();
                 let {
                     deltaY: t,
                     deltaX: e
                 } = i;
-                Math.abs(e) > Rl ? this.scrollLeft += e : this.scrollLeft += t
+                Math.abs(e) > Da ? this.scrollLeft += e : this.scrollLeft += t
             })
         }
     };
-pi.template = " <slot></slot> ";
+fi.template = " <slot></slot> ";
 
-function Ml(s) {
+function Fa(s) {
     return `<lr-presence-toggle class="tab-toggle" set="visible: presence.tabToggle.${s}; styles: presence.tabToggleStyles;"><lr-btn-ui theme="boring" ref="tab-toggle-${s}" data-id="${s}" icon="${s}" tabindex="0" set="onclick: on.clickTab;" ></lr-btn-ui></lr-presence-toggle>`
 }
 
-function Nl(s) {
+function Ba(s) {
     return `<lr-presence-toggle class="tab-content" set="visible: presence.tabContent.${s}; styles: presence.tabContentStyles"><lr-editor-scroller hidden-scrollbar><div class="controls-list_align"><div class="controls-list_inner" ref="controls-list-${s}"></div></div></lr-editor-scroller></lr-presence-toggle>`
 }
-var fi = class extends L {
+var mi = class extends L {
     constructor() {
         super();
         h(this, "_updateInfoTooltip", k(() => {
-            var o, l;
+            var o, a;
             let t = this.$["*editorTransformations"],
                 e = this.$["*currentOperation"],
                 r = "",
                 n = !1;
             if (this.$["*tabId"] === P.FILTERS)
                 if (n = !0, this.$["*currentFilter"] && ((o = t == null ? void 0 : t.filter) == null ? void 0 : o.name) === this.$["*currentFilter"]) {
-                    let a = ((l = t == null ? void 0 : t.filter) == null ? void 0 : l.amount) || 100;
-                    r = this.l10n(this.$["*currentFilter"]) + " " + a
+                    let l = ((a = t == null ? void 0 : t.filter) == null ? void 0 : a.amount) || 100;
+                    r = this.l10n(this.$["*currentFilter"]) + " " + l
                 } else r = this.l10n(ot);
             else if (this.$["*tabId"] === P.TUNING && e) {
                 n = !0;
-                let a = (t == null ? void 0 : t[e]) || st[e].zero;
-                r = e + " " + a
+                let l = (t == null ? void 0 : t[e]) || st[e].zero;
+                r = e + " " + l
             }
             n && (this.$["*operationTooltip"] = r), this.ref["tooltip-el"].classList.toggle("info-tooltip_visible", n)
         }, 0));
         this.init$ = {
             ...this.init$,
             "*sliderEl": null,
             "*loadingOperations": new Map,
             "*showSlider": !1,
             "*currentFilter": ot,
             "*currentOperation": null,
             showLoader: !1,
-            filters: br,
-            colorOperations: _r,
-            cropOperations: yr,
+            filters: yr,
+            colorOperations: br,
+            cropOperations: vr,
             "*operationTooltip": null,
             "l10n.cancel": this.l10n("cancel"),
             "l10n.apply": this.l10n("apply"),
             "presence.mainToolbar": !0,
             "presence.subToolbar": !1,
             "presence.tabToggles": !0,
             "presence.tabContent.crop": !1,
@@ -7724,23 +7788,23 @@
             }
         }, this._debouncedShowLoader = k(this._showLoader.bind(this), 500)
     }
     _onSliderClose() {
         this.$["*showSlider"] = !1, this.$["*tabId"] === P.TUNING && this.ref["tooltip-el"].classList.toggle("info-tooltip_visible", !1)
     }
     _createOperationControl(t) {
-        let e = new ve;
+        let e = new ye;
         return e.operation = t, e
     }
     _createFilterControl(t) {
         let e = new Xt;
         return e.filter = t, e
     }
     _createToggleControl(t) {
-        let e = new ge;
+        let e = new me;
         return e.operation = t, e
     }
     _renderControlsList(t) {
         let e = this.ref[`controls-list-${t}`],
             r = document.createDocumentFragment();
         t === P.CROP ? this.$.cropOperations.forEach(n => {
             let o = this._createToggleControl(n);
@@ -7760,15 +7824,15 @@
     }) {
         this.$["*tabId"] = t, t === P.CROP ? (this.$["*faderEl"].deactivate(), this.$["*cropperEl"].activate(this.$["*imageSize"], {
             fromViewer: e
         })) : (this.$["*faderEl"].activate({
             url: this.$["*originalUrl"],
             fromViewer: e
         }), this.$["*cropperEl"].deactivate());
-        for (let r of G) {
+        for (let r of W) {
             let n = r === t,
                 o = this.ref[`tab-toggle-${r}`];
             o.active = n, n ? (this._renderControlsList(t), this._syncTabIndicator()) : this._unmountTabControls(r), this.$[`presence.tabContent.${r}`] = n
         }
     }
     _unmountTabControls(t) {
         let e = this.ref[`controls-list-${t}`];
@@ -7782,15 +7846,15 @@
     _preloadEditedImage() {
         if (this.$["*imgContainerEl"] && this.$["*originalUrl"]) {
             let t = this.$["*imgContainerEl"].offsetWidth,
                 e = this.proxyUrl(qt(this.$["*originalUrl"], t, this.$["*editorTransformations"]));
             this._cancelPreload && this._cancelPreload();
             let {
                 cancel: r
-            } = ye([e]);
+            } = be([e]);
             this._cancelPreload = () => {
                 r(), this._cancelPreload = void 0
             }
         }
     }
     _showLoader(t) {
         this.$.showLoader = t
@@ -7827,27 +7891,27 @@
                     }
             }
             this._debouncedShowLoader(e)
         }), this.sub("*showSlider", t => {
             this.$["presence.subToolbar"] = t, this.$["presence.mainToolbar"] = !t
         }), this.sub("*tabList", t => {
             this.$["presence.tabToggles"] = t.length > 1;
-            for (let e of G) {
+            for (let e of W) {
                 this.$[`presence.tabToggle.${e}`] = t.includes(e);
                 let r = this.ref[`tab-toggle-${e}`];
                 r.style.gridColumn = t.indexOf(e) + 1
             }
             t.includes(this.$["*tabId"]) || this._activateTab(t[0], {
                 fromViewer: !1
             })
         }), this._updateInfoTooltip()
     }
 };
-fi.template = `<lr-line-loader-ui set="active: showLoader"></lr-line-loader-ui><div class="info-tooltip_container"><div class="info-tooltip_wrapper"><div ref="tooltip-el" class="info-tooltip info-tooltip_hidden">{{*operationTooltip}}</div></div></div><div class="toolbar-container"><lr-presence-toggle class="sub-toolbar" set="visible: presence.mainToolbar; styles: presence.subTopToolbarStyles"><div class="tab-content-row">${G.map(Nl).join("")}</div><div class="controls-row"><lr-btn-ui theme="boring" icon="closeMax" set="onclick: on.cancel"></lr-btn-ui><lr-presence-toggle class="tab-toggles" set="visible: presence.tabToggles; styles: presence.tabTogglesStyles"><div ref="tabs-indicator" class="tab-toggles_indicator"></div> ${G.map(Ml).join("")} </lr-presence-toggle><lr-btn-ui theme="primary" icon="done" set="onclick: on.apply"></lr-btn-ui></div></lr-presence-toggle><lr-presence-toggle class="sub-toolbar" set="visible: presence.subToolbar; styles: presence.subBottomToolbarStyles"><div class="slider"><lr-editor-slider ref="slider-el"></lr-editor-slider></div><div class="controls-row"><lr-btn-ui theme="boring" set="@text: l10n.cancel; onclick: on.cancelSlider;"></lr-btn-ui><lr-btn-ui theme="primary" set="@text: l10n.apply; onclick: on.applySlider;"></lr-btn-ui></div></lr-presence-toggle></div>`;
-var Ce = class extends w {
+mi.template = `<lr-line-loader-ui set="active: showLoader"></lr-line-loader-ui><div class="info-tooltip_container"><div class="info-tooltip_wrapper"><div ref="tooltip-el" class="info-tooltip info-tooltip_hidden">{{*operationTooltip}}</div></div></div><div class="toolbar-container"><lr-presence-toggle class="sub-toolbar" set="visible: presence.mainToolbar; styles: presence.subTopToolbarStyles"><div class="tab-content-row">${W.map(Ba).join("")}</div><div class="controls-row"><lr-btn-ui theme="boring" icon="closeMax" set="onclick: on.cancel"></lr-btn-ui><lr-presence-toggle class="tab-toggles" set="visible: presence.tabToggles; styles: presence.tabTogglesStyles"><div ref="tabs-indicator" class="tab-toggles_indicator"></div> ${W.map(Fa).join("")} </lr-presence-toggle><lr-btn-ui theme="primary" icon="done" set="onclick: on.apply"></lr-btn-ui></div></lr-presence-toggle><lr-presence-toggle class="sub-toolbar" set="visible: presence.subToolbar; styles: presence.subBottomToolbarStyles"><div class="slider"><lr-editor-slider ref="slider-el"></lr-editor-slider></div><div class="controls-row"><lr-btn-ui theme="boring" set="@text: l10n.cancel; onclick: on.cancelSlider;"></lr-btn-ui><lr-btn-ui theme="primary" set="@text: l10n.apply; onclick: on.applySlider;"></lr-btn-ui></div></lr-presence-toggle></div>`;
+var ve = class extends C {
     constructor() {
         super(), this._iconReversed = !1, this._iconSingle = !1, this._iconHidden = !1, this.init$ = {
             ...this.init$,
             text: "",
             icon: "",
             iconCss: this._iconCss(),
             theme: null
@@ -7872,22 +7936,22 @@
             this._iconSingle = !1
         }), this.setAttribute("role", "button"), this.tabIndex === -1 && (this.tabIndex = 0), this.hasAttribute("theme") || this.setAttribute("theme", "default")
     }
     set reverse(i) {
         this.hasAttribute("reverse") ? (this.style.flexDirection = "row-reverse", this._iconReversed = !0) : (this._iconReversed = !1, this.style.flexDirection = null)
     }
 };
-Ce.bindAttributes({
+ve.bindAttributes({
     text: "text",
     icon: "icon",
     reverse: "reverse",
     theme: "theme"
 });
-Ce.template = `<lr-icon size="20" set="className: iconCss; @name: icon;"></lr-icon><div class="text">{{text}}</div>`;
-var mi = class extends w {
+ve.template = `<lr-icon size="20" set="className: iconCss; @name: icon;"></lr-icon><div class="text">{{text}}</div>`;
+var gi = class extends C {
     constructor() {
         super(), this._active = !1, this._handleTransitionEndRight = () => {
             let i = this.ref["line-el"];
             i.style.transition = "initial", i.style.opacity = "0", i.style.transform = "translateX(-101%)", this._active && this._start()
         }
     }
     initCallback() {
@@ -7904,41 +7968,41 @@
             once: !0
         })
     }
     _stop() {
         this._active = !1
     }
 };
-mi.template = `<div class="inner"><div class="line" ref="line-el"></div></div>`;
-var gi = {
+gi.template = `<div class="inner"><div class="line" ref="line-el"></div></div>`;
+var _i = {
         transition: "transition",
         visible: "visible",
         hidden: "hidden"
     },
-    _i = class extends w {
+    bi = class extends C {
         constructor() {
-            super(), this._visible = !1, this._visibleStyle = gi.visible, this._hiddenStyle = gi.hidden, this._externalTransitions = !1, this.defineAccessor("styles", i => {
+            super(), this._visible = !1, this._visibleStyle = _i.visible, this._hiddenStyle = _i.hidden, this._externalTransitions = !1, this.defineAccessor("styles", i => {
                 i && (this._externalTransitions = !0, this._visibleStyle = i.visible, this._hiddenStyle = i.hidden)
             }), this.defineAccessor("visible", i => {
                 typeof i == "boolean" && (this._visible = i, this._handleVisible())
             })
         }
         _handleVisible() {
-            this.style.visibility = this._visible ? "inherit" : "hidden", Hr(this, {
-                [gi.transition]: !this._externalTransitions,
+            this.style.visibility = this._visible ? "inherit" : "hidden", Gr(this, {
+                [_i.transition]: !this._externalTransitions,
                 [this._visibleStyle]: this._visible,
                 [this._hiddenStyle]: !this._visible
             }), this.setAttribute("aria-hidden", this._visible ? "false" : "true")
         }
         initCallback() {
-            super.initCallback(), this.setAttribute("hidden", ""), this._externalTransitions || this.classList.add(gi.transition), this._handleVisible(), setTimeout(() => this.removeAttribute("hidden"), 0)
+            super.initCallback(), this.setAttribute("hidden", ""), this._externalTransitions || this.classList.add(_i.transition), this._handleVisible(), setTimeout(() => this.removeAttribute("hidden"), 0)
         }
     };
-_i.template = " <slot></slot> ";
-var bi = class extends w {
+bi.template = " <slot></slot> ";
+var yi = class extends C {
     constructor() {
         super();
         h(this, "init$", {
             ...this.init$,
             disabled: !1,
             min: 0,
             max: 100,
@@ -8012,32 +8076,32 @@
         let e = this.ref["steps-el"],
             {
                 width: r
             } = e.getBoundingClientRect(),
             n = Math.ceil(r / 2),
             o = Math.ceil(n / 15) - 2;
         if (this._stepsCount === o) return;
-        let l = document.createDocumentFragment(),
-            a = document.createElement("div"),
+        let a = document.createDocumentFragment(),
+            l = document.createElement("div"),
             c = document.createElement("div");
-        a.className = "minor-step", c.className = "border-step", l.appendChild(c);
-        for (let d = 0; d < o; d++) l.appendChild(a.cloneNode());
-        l.appendChild(c.cloneNode());
-        for (let d = 0; d < o; d++) l.appendChild(a.cloneNode());
-        l.appendChild(c.cloneNode());
+        l.className = "minor-step", c.className = "border-step", a.appendChild(c);
+        for (let d = 0; d < o; d++) a.appendChild(l.cloneNode());
+        a.appendChild(c.cloneNode());
+        for (let d = 0; d < o; d++) a.appendChild(l.cloneNode());
+        a.appendChild(c.cloneNode());
         let u = document.createElement("div");
-        u.className = "zero-dot", l.appendChild(u), this._zeroDotEl = u, e.innerHTML = "", e.appendChild(l), this._stepsCount = o
+        u.className = "zero-dot", a.appendChild(u), this._zeroDotEl = u, e.innerHTML = "", e.appendChild(a), this._stepsCount = o
     }
     destroyCallback() {
         var t;
         (t = this._observer) == null || t.disconnect()
     }
 };
-bi.template = `<div class="steps" ref="steps-el"></div><div ref="thumb-el" class="thumb"></div><input class="input" type="range" ref="input-el" tabindex="0" set="oninput: on.sliderInput; onchange: on.sliderChange; @min: min; @max: max; @value: defaultValue;" />`;
-var hs = class extends T {
+yi.template = `<div class="steps" ref="steps-el"></div><div ref="thumb-el" class="thumb"></div><input class="input" type="range" ref="input-el" tabindex="0" set="oninput: on.sliderInput; onchange: on.sliderChange; @min: min; @max: max; @value: defaultValue;" />`;
+var hs = class extends A {
     constructor() {
         super();
         h(this, "couldBeCtxOwner", !0);
         h(this, "activityType", g.activities.CLOUD_IMG_EDIT);
         this.init$ = {
             ...this.init$,
             cdnUrl: null
@@ -8070,53 +8134,53 @@
     }
     mountEditor() {
         let t = new nt,
             e = this.$.cdnUrl,
             r = this.cfg.cropPreset,
             n = this.cfg.cloudImageEditorTabs;
         t.setAttribute("ctx-name", this.ctxName), t.setAttribute("cdn-url", e), r && t.setAttribute("crop-preset", r), n && t.setAttribute("tabs", n), t.addEventListener("apply", o => {
-            let l = o;
-            this.handleApply(l), this.debugPrint('editor event "apply"', l.detail)
+            let a = o;
+            this.handleApply(a), this.debugPrint('editor event "apply"', a.detail)
         }), t.addEventListener("cancel", o => {
-            let l = o;
-            this.handleCancel(), this.debugPrint('editor event "cancel"', l.detail)
+            let a = o;
+            this.handleCancel(), this.debugPrint('editor event "cancel"', a.detail)
         }), t.addEventListener("change", o => {
-            let l = o;
-            this.debugPrint('editor event "change"', l.detail)
+            let a = o;
+            this.debugPrint('editor event "change"', a.detail)
         }), this.innerHTML = "", this.appendChild(t), this._mounted = !0, this._instance = t
     }
     unmountEditor() {
         this._instance = void 0, this.innerHTML = ""
     }
 };
-var Dl = function(s) {
+var za = function(s) {
         return s.replace(/[\\-\\[]\/\{\}\(\)\*\+\?\.\\\^\$\|]/g, "\\$&")
     },
-    Yr = function(s, i = "i") {
-        let t = s.split("*").map(Dl);
+    Jr = function(s, i = "i") {
+        let t = s.split("*").map(za);
         return new RegExp("^" + t.join(".+") + "$", i)
     };
-var Fl = s => Object.keys(s).reduce((t, e) => {
+var Va = s => Object.keys(s).reduce((t, e) => {
     let r = s[e],
-        n = Object.keys(r).reduce((o, l) => {
-            let a = r[l];
-            return o + `${l}: ${a};`
+        n = Object.keys(r).reduce((o, a) => {
+            let l = r[a];
+            return o + `${a}: ${l};`
         }, "");
     return t + `${e}{${n}}`
 }, "");
 
-function Jr({
+function Zr({
     textColor: s,
     backgroundColor: i,
     linkColor: t,
     linkColorHover: e,
     shadeColor: r
 }) {
     let n = `solid 1px ${r}`;
-    return Fl({
+    return Va({
         body: {
             color: s,
             "background-color": i
         },
         ".side-bar": {
             background: "inherit",
             "border-right": n
@@ -8188,27 +8252,27 @@
         return
     }
     if ((i == null ? void 0 : i.type) in xt) {
         let t = xt[i.type];
         for (let [e, r] of t) s.source === e && r(i)
     }
 });
-var Zr = function(s, i, t) {
+var Qr = function(s, i, t) {
         s in xt || (xt[s] = []), xt[s].push([i, t])
     },
-    Qr = function(s, i) {
+    tn = function(s, i) {
         s in xt && (xt[s] = xt[s].filter(t => t[0] !== i))
     };
 
-function tn(s) {
+function en(s) {
     let i = [];
     for (let [t, e] of Object.entries(s)) e == null || typeof e == "string" && e.length === 0 || i.push(`${t}=${encodeURIComponent(e)}`);
     return i.join("&")
 }
-var yi = class extends T {
+var vi = class extends A {
     constructor() {
         super();
         h(this, "couldBeCtxOwner", !0);
         h(this, "activityType", g.activities.EXTERNAL);
         h(this, "_iframe", null);
         h(this, "updateCssData", () => {
             this.isActivityActive && (this._inheritedUpdateCssData(), this.applyStyles())
@@ -8261,17 +8325,17 @@
             this.$.multiple = t
         })
     }
     extractUrlFromMessage(t) {
         if (t.alternatives) {
             let e = M(this.cfg.externalSourcesPreferredTypes);
             for (let r of e) {
-                let n = Yr(r);
-                for (let [o, l] of Object.entries(t.alternatives))
-                    if (n.test(o)) return l
+                let n = Jr(r);
+                for (let [o, a] of Object.entries(t.alternatives))
+                    if (n.test(o)) return a
             }
         }
         return t.url
     }
     sendMessage(t) {
         var e, r;
         (r = (e = this._iframe) == null ? void 0 : e.contentWindow) == null || r.postMessage(JSON.stringify(t), "*")
@@ -8291,53 +8355,53 @@
             textColor: this.getCssValue("--clr-txt"),
             shadeColor: this.getCssValue("--clr-shade-lv1"),
             linkColor: "#157cfc",
             linkColorHover: "#3891ff"
         };
         this.sendMessage({
             type: "embed-css",
-            style: Jr(t)
+            style: Zr(t)
         })
     }
     remoteUrl() {
-        var l, a;
+        var a, l;
         let t = this.cfg.pubkey,
             e = "false",
             {
                 externalSourceType: r
             } = this.activityParams,
             n = {
-                lang: ((a = (l = this.getCssData("--l10n-locale-name")) == null ? void 0 : l.split("-")) == null ? void 0 : a[0]) || "en",
+                lang: ((l = (a = this.getCssData("--l10n-locale-name")) == null ? void 0 : a.split("-")) == null ? void 0 : l[0]) || "en",
                 public_key: t,
                 images_only: e,
                 pass_window_open: !1,
                 session_key: this.cfg.remoteTabSessionKey
             },
             o = new URL(this.cfg.socialBaseUrl);
-        return o.pathname = `/window3/${r}`, o.search = tn(n), o.toString()
+        return o.pathname = `/window3/${r}`, o.search = en(n), o.toString()
     }
     mountIframe() {
         let t = Jt({
             tag: "iframe",
             attributes: {
                 src: this.remoteUrl(),
                 marginheight: 0,
                 marginwidth: 0,
                 frameborder: 0,
                 allowTransparency: !0
             }
         });
-        t.addEventListener("load", this.handleIframeLoad.bind(this)), this.ref.iframeWrapper.innerHTML = "", this.ref.iframeWrapper.appendChild(t), Zr("file-selected", t.contentWindow, this.handleFileSelected.bind(this)), this._iframe = t, this.$.selectedList = []
+        t.addEventListener("load", this.handleIframeLoad.bind(this)), this.ref.iframeWrapper.innerHTML = "", this.ref.iframeWrapper.appendChild(t), Qr("file-selected", t.contentWindow, this.handleFileSelected.bind(this)), this._iframe = t, this.$.selectedList = []
     }
     unmountIframe() {
-        this._iframe && Qr("file-selected", this._iframe.contentWindow), this.ref.iframeWrapper.innerHTML = "", this._iframe = null, this.$.selectedList = [], this.$.counter = 0
+        this._iframe && tn("file-selected", this._iframe.contentWindow), this.ref.iframeWrapper.innerHTML = "", this._iframe = null, this.$.selectedList = [], this.$.counter = 0
     }
 };
-yi.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><div><lr-icon set="@name: activityIcon"></lr-icon><span>{{activityCaption}}</span></div><button type="button" class="mini-btn close-btn" set="onclick: *historyBack"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="content"><div ref="iframeWrapper" class="iframe-wrapper"></div><div class="toolbar"><button type="button" class="cancel-btn secondary-btn" set="onclick: onCancel" l10n="cancel"></button><div></div><div set="@hidden: !multiple" class="selected-counter"><span l10n="selected-count"></span>{{counter}}</div><button type="button" class="done-btn primary-btn" set="onclick: onDone; @disabled: !counter"><lr-icon name="check"></lr-icon></button></div></div>`;
-var we = class extends w {
+vi.template = `<lr-activity-header><button type="button" class="mini-btn" set="onclick: *historyBack"><lr-icon name="back"></lr-icon></button><div><lr-icon set="@name: activityIcon"></lr-icon><span>{{activityCaption}}</span></div><button type="button" class="mini-btn close-btn" set="onclick: *historyBack"><lr-icon name="close"></lr-icon></button></lr-activity-header><div class="content"><div ref="iframeWrapper" class="iframe-wrapper"></div><div class="toolbar"><button type="button" class="cancel-btn secondary-btn" set="onclick: onCancel" l10n="cancel"></button><div></div><div set="@hidden: !multiple" class="selected-counter"><span l10n="selected-count"></span>{{counter}}</div><button type="button" class="done-btn primary-btn" set="onclick: onDone; @disabled: !counter"><lr-icon name="check"></lr-icon></button></div></div>`;
+var Ce = class extends C {
     setCurrentTab(i) {
         if (!i) return;
         [...this.ref.context.querySelectorAll("[tab-ctx]")].forEach(e => {
             e.getAttribute("tab-ctx") === i ? e.removeAttribute("hidden") : e.setAttribute("hidden", "")
         });
         for (let e in this._tabMap) e === i ? this._tabMap[e].setAttribute("current", "") : this._tabMap[e].removeAttribute("current")
     }
@@ -8359,72 +8423,72 @@
                 r.textContent = this.l10n(e), this.ref.row.appendChild(r), this._tabMap[e] = r
             })
         }), this.defineAccessor("default", i => {
             this.setCurrentTab(i)
         }), this.hasAttribute("default") || this.setCurrentTab(Object.keys(this._tabMap)[0])
     }
 };
-we.bindAttributes({
+Ce.bindAttributes({
     "tab-list": null,
     default: null
 });
-we.template = `<div ref="row" class="tabs-row"></div><div ref="context" class="tabs-context"><slot></slot></div>`;
-var us = class extends T {
+Ce.template = `<div ref="row" class="tabs-row"></div><div ref="context" class="tabs-context"><slot></slot></div>`;
+var us = class extends A {
     constructor() {
         super(...arguments);
         h(this, "requireCtxName", !0)
     }
     _createValidationInput() {
         let t = document.createElement("input");
-        return t.type = "text", t.name = this.ctxName, t.required = this.cfg.multipleMin > 0, t.tabIndex = -1, Ii(t, {
+        return t.type = "text", t.name = this.ctxName, t.required = this.cfg.multipleMin > 0, t.tabIndex = -1, ki(t, {
             opacity: 0,
             height: 0,
             width: 0
         }), t
     }
     initCallback() {
         super.initCallback(), this._validationInputElement = this._createValidationInput(), this.appendChild(this._validationInputElement), this.sub("*collectionState", t => {
             var e;
             {
                 if (this._dynamicInputsContainer || (this._dynamicInputsContainer = document.createElement("div"), this.appendChild(this._dynamicInputsContainer)), !this._validationInputElement) {
-                    let l = this._createValidationInput();
-                    this.appendChild(l), this._validationInputElement = l
+                    let a = this._createValidationInput();
+                    this.appendChild(a), this._validationInputElement = a
                 }
                 if (this._dynamicInputsContainer.innerHTML = "", t.status === "uploading" || t.status === "idle") {
                     this._validationInputElement.value = "", this._validationInputElement.setCustomValidity("");
                     return
                 }
                 if (t.status === "failed") {
-                    let l = (e = t.errors[0]) == null ? void 0 : e.message;
-                    this._validationInputElement.value = "", this._validationInputElement.setCustomValidity(l);
+                    let a = (e = t.errors[0]) == null ? void 0 : e.message;
+                    this._validationInputElement.value = "", this._validationInputElement.setCustomValidity(a);
                     return
                 }
                 let r = t.group ? t.group : null;
                 if (r) {
                     this._validationInputElement.value = r.cdnUrl, this._validationInputElement.setCustomValidity("");
                     return
                 }
-                let n = t.allEntries.map(l => l.cdnUrl);
+                let n = t.allEntries.map(a => a.cdnUrl);
                 if (!this.cfg.multiple && n.length === 1) {
                     this._validationInputElement.value = n[0], this._validationInputElement.setCustomValidity("");
                     return
                 }
                 this._validationInputElement.remove(), this._validationInputElement = null;
                 let o = new DocumentFragment;
-                for (let l of n) {
-                    let a = document.createElement("input");
-                    a.type = "hidden", a.name = `${this.ctxName}[]`, a.value = l, o.appendChild(a)
+                for (let a of n) {
+                    let l = document.createElement("input");
+                    l.type = "hidden", l.name = `${this.ctxName}[]`, l.value = a, o.appendChild(l)
                 }
                 this._dynamicInputsContainer.replaceChildren(o)
             }
         }, !1)
     }
 };
 var ds = class extends g {};
-var vi = class extends w {
+var Ci = class extends C {
     constructor() {
         super(...arguments);
         h(this, "init$", {
             ...this.init$,
             currentText: "",
             options: [],
             selectHtml: "",
@@ -8441,43 +8505,43 @@
             let e = "";
             t == null || t.forEach(n => {
                 e += `<option value="${n.value}">${n.text}</option>`
             }), this.$.selectHtml = e
         })
     }
 };
-vi.template = `<button> {{currentText}} <lr-icon name="select"></lr-icon><select ref="select" set="innerHTML: selectHtml; onchange: onSelect"></select></button>`;
-var W = {
+Ci.template = `<button> {{currentText}} <lr-icon name="select"></lr-icon><select ref="select" set="innerHTML: selectHtml; onchange: onSelect"></select></button>`;
+var X = {
         PLAY: "play",
         PAUSE: "pause",
         FS_ON: "fullscreen-on",
         FS_OFF: "fullscreen-off",
         VOL_ON: "unmute",
         VOL_OFF: "mute",
         CAP_ON: "captions",
         CAP_OFF: "captions-off"
     },
-    en = {
+    sn = {
         requestFullscreen: s => {
             s.requestFullscreen ? s.requestFullscreen() : s.webkitRequestFullscreen && s.webkitRequestFullscreen()
         },
         exitFullscreen: () => {
             document.exitFullscreen ? document.exitFullscreen() : document.webkitExitFullscreen && document.webkitExitFullscreen()
         }
     },
-    Ae = class s extends w {
+    we = class s extends C {
         constructor() {
             super(...arguments);
             h(this, "init$", {
                 ...this.init$,
                 src: "",
-                ppIcon: W.PLAY,
-                fsIcon: W.FS_ON,
-                volIcon: W.VOL_ON,
-                capIcon: W.CAP_OFF,
+                ppIcon: X.PLAY,
+                fsIcon: X.FS_ON,
+                volIcon: X.VOL_ON,
+                capIcon: X.CAP_OFF,
                 totalTime: "00:00",
                 currentTime: "00:00",
                 progressCssWidth: "0",
                 hasSubtitles: !1,
                 volumeDisabled: !1,
                 volumeValue: 0,
                 onPP: () => {
@@ -8502,21 +8566,21 @@
                 }
             })
         }
         togglePlay() {
             this._video.paused || this._video.ended ? this._video.play() : this._video.pause()
         }
         toggleFullscreen() {
-            (document.fullscreenElement || document.webkitFullscreenElement) === this ? en.exitFullscreen() : en.requestFullscreen(this)
+            (document.fullscreenElement || document.webkitFullscreenElement) === this ? sn.exitFullscreen() : sn.requestFullscreen(this)
         }
         toggleCaptions() {
-            this.$.capIcon === W.CAP_OFF ? (this.$.capIcon = W.CAP_ON, this._video.textTracks[0].mode = "showing", window.localStorage.setItem(s.is + ":captions", "1")) : (this.$.capIcon = W.CAP_OFF, this._video.textTracks[0].mode = "hidden", window.localStorage.removeItem(s.is + ":captions"))
+            this.$.capIcon === X.CAP_OFF ? (this.$.capIcon = X.CAP_ON, this._video.textTracks[0].mode = "showing", window.localStorage.setItem(s.is + ":captions", "1")) : (this.$.capIcon = X.CAP_OFF, this._video.textTracks[0].mode = "hidden", window.localStorage.removeItem(s.is + ":captions"))
         }
         toggleSound() {
-            this.$.volIcon === W.VOL_ON ? (this.$.volIcon = W.VOL_OFF, this.$.volumeDisabled = !0, this._video.muted = !0) : (this.$.volIcon = W.VOL_ON, this.$.volumeDisabled = !1, this._video.muted = !1)
+            this.$.volIcon === X.VOL_ON ? (this.$.volIcon = X.VOL_OFF, this.$.volumeDisabled = !0, this._video.muted = !0) : (this.$.volIcon = X.VOL_ON, this.$.volumeDisabled = !1, this._video.muted = !1)
         }
         setVolume(t) {
             window.localStorage.setItem(s.is + ":volume", t);
             let e = t ? t / 100 : 0;
             this._video.volume = e
         }
         get progress() {
@@ -8546,19 +8610,19 @@
             let t = ["autoplay", "loop", "muted"];
             [...this.attributes].forEach(e => {
                 t.includes(e.name) && this._video.setAttribute(e.name, e.value)
             })
         }
         initCallback() {
             super.initCallback(), this._video = this.ref.video, this._castAttributes(), this._video.addEventListener("play", () => {
-                this.$.ppIcon = W.PAUSE, this.setAttribute("playback", "")
+                this.$.ppIcon = X.PAUSE, this.setAttribute("playback", "")
             }), this._video.addEventListener("pause", () => {
-                this.$.ppIcon = W.PLAY, this.removeAttribute("playback")
+                this.$.ppIcon = X.PLAY, this.removeAttribute("playback")
             }), this.addEventListener("fullscreenchange", e => {
-                console.log(e), document.fullscreenElement === this ? this.$.fsIcon = W.FS_OFF : this.$.fsIcon = W.FS_ON
+                console.log(e), document.fullscreenElement === this ? this.$.fsIcon = X.FS_OFF : this.$.fsIcon = X.FS_ON
             }), this.sub("src", e => {
                 if (!e) return;
                 let r = this._getUrl(e);
                 this._video.src = r
             }), this.sub("video", async e => {
                 if (!e) return;
                 let r = await (await window.fetch(this._getUrl(e))).json();
@@ -8578,22 +8642,22 @@
             let t = window.localStorage.getItem(s.is + ":volume");
             if (t) {
                 let e = parseFloat(t);
                 this.setVolume(e), this.$.volumeValue = e
             }
         }
     };
-Ae.template = `<div class="video-wrapper"><video ref="video" preload="metadata" crossorigin="anonymous"></video></div><div class="toolbar"><div class="progress" ref="progress" set -onclick="progressClicked"><div class="bar" set -style.width="progressCssWidth"></div></div><div class="tb-block"><button set -onclick="onPP"><lr-icon set -@name="ppIcon"></lr-icon></button><div class="timer">{{currentTime}} / {{totalTime}}</div></div><div class="tb-block"><button set -onclick="onCap" -@hidden="!hasSubtitles"><lr-icon set -@name="capIcon"></lr-icon></button><button set -onclick="onMute"><lr-icon set -@name="volIcon"></lr-icon></button><lr-range type="range" set -onchange="onVolChange" -@disabled="volumeDisabled" -value="volumeValue"></lr-range><button set -onclick="onFs"><lr-icon set -@name="fsIcon"></lr-icon></button></div></div>`;
-Ae.bindAttributes({
+we.template = `<div class="video-wrapper"><video ref="video" preload="metadata" crossorigin="anonymous"></video></div><div class="toolbar"><div class="progress" ref="progress" set -onclick="progressClicked"><div class="bar" set -style.width="progressCssWidth"></div></div><div class="tb-block"><button set -onclick="onPP"><lr-icon set -@name="ppIcon"></lr-icon></button><div class="timer">{{currentTime}} / {{totalTime}}</div></div><div class="tb-block"><button set -onclick="onCap" -@hidden="!hasSubtitles"><lr-icon set -@name="capIcon"></lr-icon></button><button set -onclick="onMute"><lr-icon set -@name="volIcon"></lr-icon></button><lr-range type="range" set -onchange="onVolChange" -@disabled="volumeDisabled" -value="volumeValue"></lr-range><button set -onclick="onFs"><lr-icon set -@name="fsIcon"></lr-icon></button></div></div>`;
+we.bindAttributes({
     video: "video",
     src: "src"
 });
-var Bl = "css-src";
+var ja = "css-src";
 
-function Ci(s) {
+function wi(s) {
     return class extends s {
         constructor() {
             super(...arguments);
             h(this, "renderShadow", !0);
             h(this, "pauseRender", !0);
             h(this, "requireCtxName", !0)
         }
@@ -8603,17 +8667,17 @@
             let t = this.constructor.__shadowStylesUrl,
                 e = this.shadowRoot.querySelector(`link[href="${t}"]`);
             e && await new Promise((r, n) => {
                 e.addEventListener("load", r), e.addEventListener("error", n)
             })
         }
         initCallback() {
-            super.initCallback(), this.setAttribute("hidden", ""), Ie({
+            super.initCallback(), this.setAttribute("hidden", ""), $e({
                 element: this,
-                attribute: Bl,
+                attribute: ja,
                 onSuccess: t => {
                     this.attachShadow({
                         mode: "open"
                     });
                     let e = document.createElement("link");
                     e.rel = "stylesheet", e.type = "text/css", e.href = t, e.onload = () => {
                         window.requestAnimationFrame(async () => {
@@ -8626,28 +8690,28 @@
                 onTimeout: () => {
                     console.error("Attribute `css-src` is required and it is not set. See migration guide: https://uploadcare.com/docs/file-uploader/migration-to-0.25.0/")
                 }
             })
         }
     }
 }
-var Ee = class extends Ci(w) {};
-var wi = class extends w {
+var Ee = class extends wi(C) {};
+var Ei = class extends C {
     initCallback() {
         super.initCallback(), this.subConfigValue("removeCopyright", i => {
             this.toggleAttribute("hidden", !!i)
         })
     }
 };
-h(wi, "template", `<a href="https://uploadcare.com/?utm_source=copyright&utm_medium=referral&utm_campaign=v4" target="_blank noopener" class="credits" >Powered by Uploadcare</a >`);
+h(Ei, "template", `<a href="https://uploadcare.com/?utm_source=copyright&utm_medium=referral&utm_campaign=v4" target="_blank noopener" class="credits" >Powered by Uploadcare</a >`);
 var Tt = class extends Ee {
     constructor() {
         super(...arguments);
         h(this, "requireCtxName", !0);
-        h(this, "init$", Ne(this));
+        h(this, "init$", Me(this));
         h(this, "_template", null)
     }
     static set template(t) {
         this._template = t + "<slot></slot>"
     }
     static get template() {
         return this._template
@@ -8659,15 +8723,15 @@
             this._lastModalActive !== i && this.emit(i ? $.MODAL_OPEN : $.MODAL_CLOSE, void 0, {
                 debounce: !0
             }), this._lastModalActive = i
         }, !1)
     }
 };
 Ai.template = `<lr-simple-btn></lr-simple-btn><lr-modal strokes block-body-scrolling><lr-start-from><lr-drop-area with-icon clickable></lr-drop-area><lr-source-list wrap></lr-source-list><button type="button" l10n="start-from-cancel" class="secondary-btn" set="onclick: *historyBack"></button><lr-copyright></lr-copyright></lr-start-from><lr-upload-list></lr-upload-list><lr-camera-source></lr-camera-source><lr-url-source></lr-url-source><lr-external-source></lr-external-source><lr-cloud-image-editor-activity></lr-cloud-image-editor-activity></lr-modal><lr-progress-bar-common></lr-progress-bar-common>`;
-var Ei = class extends Tt {
+var xi = class extends Tt {
     constructor() {
         super(...arguments);
         h(this, "pauseRender", !0)
     }
     shadowReadyCallback() {
         let t = this.ref.uBlock;
         this.sub("*currentActivity", e => {
@@ -8677,16 +8741,16 @@
         }), this.subConfigValue("sourceList", e => {
             e !== "local" && (this.cfg.sourceList = "local")
         }), this.subConfigValue("confirmUpload", e => {
             e !== !1 && (this.cfg.confirmUpload = !1)
         })
     }
 };
-Ei.template = `<lr-start-from><lr-drop-area clickable l10n="choose-file"></lr-drop-area><lr-copyright></lr-copyright></lr-start-from><lr-upload-list ref="uBlock"></lr-upload-list>`;
-var xi = class extends Tt {
+xi.template = `<lr-start-from><lr-drop-area clickable l10n="choose-file"></lr-drop-area><lr-copyright></lr-copyright></lr-start-from><lr-upload-list ref="uBlock"></lr-upload-list>`;
+var Ti = class extends Tt {
     constructor() {
         super(), this.init$ = {
             ...this.init$,
             couldCancel: !1,
             cancel: () => {
                 this.couldHistoryBack ? this.$["*historyBack"]() : this.couldShowList && (this.$["*currentActivity"] = g.activities.UPLOAD_LIST)
             }
@@ -8706,16 +8770,16 @@
         }), this.sub("*uploadList", t => {
             (t == null ? void 0 : t.length) > 0 && this.$["*currentActivity"] === (i.initActivity || g.activities.START_FROM) && (this.$["*currentActivity"] = g.activities.UPLOAD_LIST)
         }), this.sub("*history", () => {
             this.$.couldCancel = this.couldHistoryBack || this.couldShowList
         })
     }
 };
-xi.template = `<lr-start-from><lr-drop-area with-icon clickable></lr-drop-area><lr-source-list wrap></lr-source-list><button type="button" l10n="start-from-cancel" class="cancel-btn secondary-btn" set="onclick: cancel; @hidden: !couldCancel" ></button><lr-copyright></lr-copyright></lr-start-from><lr-upload-list ref="uBlock"></lr-upload-list><lr-camera-source></lr-camera-source><lr-url-source></lr-url-source><lr-external-source></lr-external-source><lr-progress-bar></lr-progress-bar><lr-cloud-image-editor-activity></lr-cloud-image-editor-activity>`;
-var ps = class extends Ci(nt) {
+Ti.template = `<lr-start-from><lr-drop-area with-icon clickable></lr-drop-area><lr-source-list wrap></lr-source-list><button type="button" l10n="start-from-cancel" class="cancel-btn secondary-btn" set="onclick: cancel; @hidden: !couldCancel" ></button><lr-copyright></lr-copyright></lr-start-from><lr-upload-list ref="uBlock"></lr-upload-list><lr-camera-source></lr-camera-source><lr-url-source></lr-url-source><lr-external-source></lr-external-source><lr-progress-bar></lr-progress-bar><lr-cloud-image-editor-activity></lr-cloud-image-editor-activity>`;
+var ps = class extends wi(nt) {
     shadowReadyCallback() {
         this.__shadowReady = !0, this.$["*faderEl"] = this.ref["fader-el"], this.$["*cropperEl"] = this.ref["cropper-el"], this.$["*imgContainerEl"] = this.ref["img-container-el"], this.initEditor()
     }
     async initEditor() {
         this.__shadowReady && await super.initEditor()
     }
 };
@@ -8723,15 +8787,15 @@
 function fs(s) {
     for (let i in s) {
         let t = [...i].reduce((e, r) => (r.toUpperCase() === r && (r = "-" + r.toLowerCase()), e += r), "");
         t.startsWith("-") && (t = t.replace("-", "")), t.startsWith("lr-") || (t = "lr-" + t), s[i].reg && s[i].reg(t)
     }
 }
 var ms = "LR";
-async function zl(s, i = !1) {
+async function Ha(s, i = !1) {
     return new Promise((t, e) => {
         if (typeof document != "object") {
             t(null);
             return
         }
         if (typeof window == "object" && window[ms]) {
             t(window[ms]);
@@ -8743,9 +8807,9 @@
         }, r.onload = () => {
             let n = window[ms];
             i && fs(n), t(n)
         }, document.head.appendChild(r)
     })
 }
 export {
-    g as ActivityBlock, ds as ActivityHeader, Dt as BaseComponent, w as Block, ni as CameraSource, ps as CloudImageEditor, hs as CloudImageEditorActivity, nt as CloudImageEditorBlock, qo as Config, li as ConfirmationDialog, wi as Copyright, hi as CropFrame, E as Data, ce as DropArea, ge as EditorCropButtonControl, Xt as EditorFilterControl, di as EditorImageCropper, cs as EditorImageFader, ve as EditorOperationControl, pi as EditorScroller, ui as EditorSlider, fi as EditorToolbar, yi as ExternalSource, pe as FileItem, me as FilePreview, xi as FileUploaderInline, Ei as FileUploaderMinimal, Ai as FileUploaderRegular, us as FormInput, oe as Icon, ts as Img, mi as LineLoaderUi, Ce as LrBtnUi, fe as Modal, Be as PACKAGE_NAME, ze as PACKAGE_VERSION, _i as PresenceToggle, ci as ProgressBar, ai as ProgressBarCommon, vi as Select, Ee as ShadowWrapper, ae as SimpleBtn, bi as SliderUi, he as SourceBtn, ss as SourceList, ti as StartFrom, we as Tabs, Sl as UploadCtxProvider, oi as UploadDetails, si as UploadList, T as UploaderBlock, ri as UrlSource, Ae as Video, zl as connectBlocksFrom, fs as registerBlocks, Ci as shadowed, ht as toKebabCase
+    g as ActivityBlock, ds as ActivityHeader, Nt as BaseComponent, C as Block, ni as CameraSource, ps as CloudImageEditor, hs as CloudImageEditorActivity, nt as CloudImageEditorBlock, Zo as Config, li as ConfirmationDialog, Ei as Copyright, ui as CropFrame, E as Data, le as DropArea, me as EditorCropButtonControl, Xt as EditorFilterControl, pi as EditorImageCropper, cs as EditorImageFader, ye as EditorOperationControl, fi as EditorScroller, di as EditorSlider, mi as EditorToolbar, vi as ExternalSource, de as FileItem, fe as FilePreview, Ti as FileUploaderInline, xi as FileUploaderMinimal, Ai as FileUploaderRegular, us as FormInput, ne as Icon, es as Img, gi as LineLoaderUi, ve as LrBtnUi, pe as Modal, Fe as PACKAGE_NAME, Be as PACKAGE_VERSION, bi as PresenceToggle, hi as ProgressBar, ci as ProgressBarCommon, Ci as Select, Ee as ShadowWrapper, ae as SimpleBtn, yi as SliderUi, ce as SourceBtn, rs as SourceList, Qe as StartFrom, Ce as Tabs, ka as UploadCtxProvider, ai as UploadDetails, si as UploadList, A as UploaderBlock, ri as UrlSource, we as Video, Ha as connectBlocksFrom, fs as registerBlocks, wi as shadowed, ht as toKebabCase
 };
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-inline.min.css` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-inline.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-file: "m2.89453 1.2012c0-.473389.38376-.857145.85714-.857145h8.40003c.2273 0 .4453.090306.6061.251051l8.4 8.400004c.1607.16074.251.37876.251.60609v13.2c0 .4734-.3837.8571-.8571.8571h-16.80003c-.47338 0-.85714-.3837-.85714-.8571zm1.71429.85714v19.88576h15.08568v-11.4858h-7.5428c-.4734 0-.8572-.3837-.8572-.8571v-7.54286zm8.39998 1.21218 5.4736 5.47353-5.4736.00001z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-collapse: "M3.11572 12C3.11572 11.5858 3.45151 11.25 3.86572 11.25H20.1343C20.5485 11.25 20.8843 11.5858 20.8843 12C20.8843 12.4142 20.5485 12.75 20.1343 12.75H3.86572C3.45151 12.75 3.11572 12.4142 3.11572 12Z";--icon-expand: "M12.0001 8.33716L3.53033 16.8068C3.23743 17.0997 2.76256 17.0997 2.46967 16.8068C2.17678 16.5139 2.17678 16.0391 2.46967 15.7462L11.0753 7.14067C11.1943 7.01825 11.3365 6.92067 11.4936 6.8536C11.6537 6.78524 11.826 6.75 12.0001 6.75C12.1742 6.75 12.3465 6.78524 12.5066 6.8536C12.6637 6.92067 12.8059 7.01826 12.925 7.14068L21.5304 15.7462C21.8233 16.0391 21.8233 16.5139 21.5304 16.8068C21.2375 17.0997 20.7627 17.0997 20.4698 16.8068L12.0001 8.33716Z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-local: "m3 3.75c-.82843 0-1.5.67157-1.5 1.5v13.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-9.75c0-.82843-.6716-1.5-1.5-1.5h-9c-.2634 0-.5076-.13822-.6431-.36413l-2.03154-3.38587zm-3 1.5c0-1.65685 1.34315-3 3-3h6.75c.2634 0 .5076.13822.6431.36413l2.0315 3.38587h8.5754c1.6569 0 3 1.34315 3 3v9.75c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3z";--icon-url: "m19.1099 3.67026c-1.7092-1.70917-4.5776-1.68265-6.4076.14738l-2.2212 2.22122c-.2929.29289-.7678.29289-1.0607 0-.29289-.29289-.29289-.76777 0-1.06066l2.2212-2.22122c2.376-2.375966 6.1949-2.481407 8.5289-.14738l1.2202 1.22015c2.334 2.33403 2.2286 6.15294-.1474 8.52895l-2.2212 2.2212c-.2929.2929-.7678.2929-1.0607 0s-.2929-.7678 0-1.0607l2.2212-2.2212c1.8301-1.83003 1.8566-4.69842.1474-6.40759zm-3.3597 4.57991c.2929.29289.2929.76776 0 1.06066l-6.43918 6.43927c-.29289.2928-.76777.2928-1.06066 0-.29289-.2929-.29289-.7678 0-1.0607l6.43924-6.43923c.2929-.2929.7677-.2929 1.0606 0zm-9.71158 1.17048c.29289.29289.29289.76775 0 1.06065l-2.22123 2.2212c-1.83002 1.8301-1.85654 4.6984-.14737 6.4076l1.22015 1.2202c1.70917 1.7091 4.57756 1.6826 6.40763-.1474l2.2212-2.2212c.2929-.2929.7677-.2929 1.0606 0s.2929.7677 0 1.0606l-2.2212 2.2212c-2.37595 2.376-6.19486 2.4815-8.52889.1474l-1.22015-1.2201c-2.334031-2.3341-2.22859-6.153.14737-8.5289l2.22123-2.22125c.29289-.2929.76776-.2929 1.06066 0z";--icon-camera: "m7.65 2.55c.14164-.18885.36393-.3.6-.3h7.5c.2361 0 .4584.11115.6.3l2.025 2.7h2.625c1.6569 0 3 1.34315 3 3v10.5c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3v-10.5c0-1.65685 1.34315-3 3-3h2.625zm.975 1.2-2.025 2.7c-.14164.18885-.36393.3-.6.3h-3c-.82843 0-1.5.67157-1.5 1.5v10.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-10.5c0-.82843-.6716-1.5-1.5-1.5h-3c-.2361 0-.4584-.11115-.6-.3l-2.025-2.7zm3.375 6c-1.864 0-3.375 1.511-3.375 3.375s1.511 3.375 3.375 3.375 3.375-1.511 3.375-3.375-1.511-3.375-3.375-3.375zm-4.875 3.375c0-2.6924 2.18261-4.875 4.875-4.875 2.6924 0 4.875 2.1826 4.875 4.875s-2.1826 4.875-4.875 4.875c-2.69239 0-4.875-2.1826-4.875-4.875z";--icon-dots: "M16,12A2,2 0 0,1 18,10A2,2 0 0,1 20,12A2,2 0 0,1 18,14A2,2 0 0,1 16,12M10,12A2,2 0 0,1 12,10A2,2 0 0,1 14,12A2,2 0 0,1 12,14A2,2 0 0,1 10,12M4,12A2,2 0 0,1 6,10A2,2 0 0,1 8,12A2,2 0 0,1 6,14A2,2 0 0,1 4,12Z";--icon-back: "M20.251 12.0001C20.251 12.4143 19.9152 12.7501 19.501 12.7501L6.06696 12.7501L11.7872 18.6007C12.0768 18.8968 12.0715 19.3717 11.7753 19.6613C11.4791 19.9508 11.0043 19.9455 10.7147 19.6493L4.13648 12.9213C4.01578 12.8029 3.91947 12.662 3.85307 12.5065C3.78471 12.3464 3.74947 12.1741 3.74947 12C3.74947 11.8259 3.78471 11.6536 3.85307 11.4935C3.91947 11.338 4.01578 11.1971 4.13648 11.0787L10.7147 4.35068C11.0043 4.0545 11.4791 4.04916 11.7753 4.33873C12.0715 4.62831 12.0768 5.10315 11.7872 5.39932L6.06678 11.2501L19.501 11.2501C19.9152 11.2501 20.251 11.5859 20.251 12.0001Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-edit: "M3.96371 14.4792c-.15098.151-.25578.3419-.3021.5504L2.52752 20.133c-.17826.8021.53735 1.5177 1.33951 1.3395l5.10341-1.1341c.20844-.0463.39934-.1511.55032-.3021l8.05064-8.0507-5.557-5.55702-8.05069 8.05062ZM13.4286 5.01437l5.557 5.55703 2.0212-2.02111c.6576-.65765.6576-1.72393 0-2.38159l-3.1755-3.17546c-.6577-.65765-1.7239-.65765-2.3816 0l-2.0211 2.02113Z";--icon-detail: "M5,3C3.89,3 3,3.89 3,5V19C3,20.11 3.89,21 5,21H19C20.11,21 21,20.11 21,19V5C21,3.89 20.11,3 19,3H5M5,5H19V19H5V5M7,7V9H17V7H7M7,11V13H17V11H7M7,15V17H14V15H7Z";--icon-select: "M7,10L12,15L17,10H7Z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-fullscreen: "M5,5H10V7H7V10H5V5M14,5H19V10H17V7H14V5M17,14H19V19H14V17H17V14M10,17V19H5V14H7V17H10Z";--icon-fullscreen-exit: "M14,14H19V16H16V19H14V14M5,14H10V19H8V16H5V14M8,5H10V10H5V8H8V5M19,8V10H14V5H16V8H19Z";--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-about: "M11.152 14.12v.1h1.523v-.1c.007-.409.053-.752.138-1.028.086-.277.22-.517.405-.72.188-.202.434-.397.735-.586.32-.191.593-.412.82-.66.232-.249.41-.531.533-.847.125-.32.187-.678.187-1.076 0-.579-.137-1.085-.41-1.518a2.717 2.717 0 0 0-1.14-1.018c-.49-.245-1.062-.367-1.715-.367-.597 0-1.142.114-1.636.34-.49.228-.884.564-1.182 1.008-.299.44-.46.98-.485 1.619h1.62c.024-.377.118-.684.282-.922.163-.241.369-.419.617-.532.25-.114.51-.17.784-.17.301 0 .575.063.82.191.248.124.447.302.597.533.149.23.223.504.223.82 0 .263-.05.502-.149.72-.1.216-.234.408-.405.574a3.48 3.48 0 0 1-.575.453c-.33.199-.613.42-.847.66-.234.242-.415.558-.543.949-.125.39-.19.916-.197 1.577ZM11.205 17.15c.21.206.46.31.75.31.196 0 .374-.049.534-.144.16-.096.287-.224.383-.384.1-.163.15-.343.15-.538a1 1 0 0 0-.32-.746 1.019 1.019 0 0 0-.746-.314c-.291 0-.542.105-.751.314-.21.206-.314.455-.314.746 0 .295.104.547.314.756ZM24 12c0 6.627-5.373 12-12 12S0 18.627 0 12 5.373 0 12 0s12 5.373 12 12Zm-1.5 0c0 5.799-4.701 10.5-10.5 10.5S1.5 17.799 1.5 12 6.201 1.5 12 1.5 22.5 6.201 22.5 12Z";--icon-edit-rotate: "M16.89,15.5L18.31,16.89C19.21,15.73 19.76,14.39 19.93,13H17.91C17.77,13.87 17.43,14.72 16.89,15.5M13,17.9V19.92C14.39,19.75 15.74,19.21 16.9,18.31L15.46,16.87C14.71,17.41 13.87,17.76 13,17.9M19.93,11C19.76,9.61 19.21,8.27 18.31,7.11L16.89,8.53C17.43,9.28 17.77,10.13 17.91,11M15.55,5.55L11,1V4.07C7.06,4.56 4,7.92 4,12C4,16.08 7.05,19.44 11,19.93V17.91C8.16,17.43 6,14.97 6,12C6,9.03 8.16,6.57 11,6.09V10L15.55,5.55Z";--icon-edit-flip-v: "M3 15V17H5V15M15 19V21H17V19M19 3H5C3.9 3 3 3.9 3 5V9H5V5H19V9H21V5C21 3.9 20.1 3 19 3M21 19H19V21C20.1 21 21 20.1 21 19M1 11V13H23V11M7 19V21H9V19M19 15V17H21V15M11 19V21H13V19M3 19C3 20.1 3.9 21 5 21V19Z";--icon-edit-flip-h: "M15 21H17V19H15M19 9H21V7H19M3 5V19C3 20.1 3.9 21 5 21H9V19H5V5H9V3H5C3.9 3 3 3.9 3 5M19 3V5H21C21 3.9 20.1 3 19 3M11 23H13V1H11M19 17H21V15H19M15 5H17V3H15M19 13H21V11H19M19 21C20.1 21 21 20.1 21 19H19Z";--icon-edit-brightness: "M12,18A6,6 0 0,1 6,12A6,6 0 0,1 12,6A6,6 0 0,1 18,12A6,6 0 0,1 12,18M20,15.31L23.31,12L20,8.69V4H15.31L12,0.69L8.69,4H4V8.69L0.69,12L4,15.31V20H8.69L12,23.31L15.31,20H20V15.31Z";--icon-edit-contrast: "M12,20C9.79,20 7.79,19.1 6.34,17.66L17.66,6.34C19.1,7.79 20,9.79 20,12A8,8 0 0,1 12,20M6,8H8V6H9.5V8H11.5V9.5H9.5V11.5H8V9.5H6M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,16H17V14.5H12V16Z";--icon-edit-saturation: "M3,13A9,9 0 0,0 12,22C12,17 7.97,13 3,13M12,5.5A2.5,2.5 0 0,1 14.5,8A2.5,2.5 0 0,1 12,10.5A2.5,2.5 0 0,1 9.5,8A2.5,2.5 0 0,1 12,5.5M5.6,10.25A2.5,2.5 0 0,0 8.1,12.75C8.63,12.75 9.12,12.58 9.5,12.31C9.5,12.37 9.5,12.43 9.5,12.5A2.5,2.5 0 0,0 12,15A2.5,2.5 0 0,0 14.5,12.5C14.5,12.43 14.5,12.37 14.5,12.31C14.88,12.58 15.37,12.75 15.9,12.75C17.28,12.75 18.4,11.63 18.4,10.25C18.4,9.25 17.81,8.4 16.97,8C17.81,7.6 18.4,6.74 18.4,5.75C18.4,4.37 17.28,3.25 15.9,3.25C15.37,3.25 14.88,3.41 14.5,3.69C14.5,3.63 14.5,3.56 14.5,3.5A2.5,2.5 0 0,0 12,1A2.5,2.5 0 0,0 9.5,3.5C9.5,3.56 9.5,3.63 9.5,3.69C9.12,3.41 8.63,3.25 8.1,3.25A2.5,2.5 0 0,0 5.6,5.75C5.6,6.74 6.19,7.6 7.03,8C6.19,8.4 5.6,9.25 5.6,10.25M12,22A9,9 0 0,0 21,13C16,13 12,17 12,22Z";--icon-edit-crop: "M7,17V1H5V5H1V7H5V17A2,2 0 0,0 7,19H17V23H19V19H23V17M17,15H19V7C19,5.89 18.1,5 17,5H9V7H17V15Z";--icon-edit-text: "M18.5,4L19.66,8.35L18.7,8.61C18.25,7.74 17.79,6.87 17.26,6.43C16.73,6 16.11,6 15.5,6H13V16.5C13,17 13,17.5 13.33,17.75C13.67,18 14.33,18 15,18V19H9V18C9.67,18 10.33,18 10.67,17.75C11,17.5 11,17 11,16.5V6H8.5C7.89,6 7.27,6 6.74,6.43C6.21,6.87 5.75,7.74 5.3,8.61L4.34,8.35L5.5,4H18.5Z";--icon-edit-draw: "m21.879394 2.1631238c-1.568367-1.62768627-4.136546-1.53831744-5.596267.1947479l-8.5642801 10.1674753c-1.4906533-.224626-3.061232.258204-4.2082427 1.448604-1.0665468 1.106968-1.0997707 2.464806-1.1203996 3.308068-.00142.05753-.00277.113001-.00439.16549-.02754.894146-.08585 1.463274-.5821351 2.069648l-.80575206.98457.88010766.913285c1.0539516 1.093903 2.6691689 1.587048 4.1744915 1.587048 1.5279113 0 3.2235468-.50598 4.4466094-1.775229 1.147079-1.190514 1.612375-2.820653 1.395772-4.367818l9.796763-8.8879697c1.669907-1.5149954 1.75609-4.1802333.187723-5.8079195zm-16.4593821 13.7924592c.8752943-.908358 2.2944227-.908358 3.1697054 0 .8752942.908358.8752942 2.381259 0 3.289617-.5909138.61325-1.5255389.954428-2.53719.954428-.5223687 0-.9935663-.09031-1.3832112-.232762.3631253-.915463.3952949-1.77626.4154309-2.429737.032192-1.045425.072224-1.308557.3352649-1.581546z";--icon-edit-guides: "M1.39,18.36L3.16,16.6L4.58,18L5.64,16.95L4.22,15.54L5.64,14.12L8.11,16.6L9.17,15.54L6.7,13.06L8.11,11.65L9.53,13.06L10.59,12L9.17,10.59L10.59,9.17L13.06,11.65L14.12,10.59L11.65,8.11L13.06,6.7L14.47,8.11L15.54,7.05L14.12,5.64L15.54,4.22L18,6.7L19.07,5.64L16.6,3.16L18.36,1.39L22.61,5.64L5.64,22.61L1.39,18.36Z";--icon-edit-color: "M17.5,12A1.5,1.5 0 0,1 16,10.5A1.5,1.5 0 0,1 17.5,9A1.5,1.5 0 0,1 19,10.5A1.5,1.5 0 0,1 17.5,12M14.5,8A1.5,1.5 0 0,1 13,6.5A1.5,1.5 0 0,1 14.5,5A1.5,1.5 0 0,1 16,6.5A1.5,1.5 0 0,1 14.5,8M9.5,8A1.5,1.5 0 0,1 8,6.5A1.5,1.5 0 0,1 9.5,5A1.5,1.5 0 0,1 11,6.5A1.5,1.5 0 0,1 9.5,8M6.5,12A1.5,1.5 0 0,1 5,10.5A1.5,1.5 0 0,1 6.5,9A1.5,1.5 0 0,1 8,10.5A1.5,1.5 0 0,1 6.5,12M12,3A9,9 0 0,0 3,12A9,9 0 0,0 12,21A1.5,1.5 0 0,0 13.5,19.5C13.5,19.11 13.35,18.76 13.11,18.5C12.88,18.23 12.73,17.88 12.73,17.5A1.5,1.5 0 0,1 14.23,16H16A5,5 0 0,0 21,11C21,6.58 16.97,3 12,3Z";--icon-edit-resize: "M10.59,12L14.59,8H11V6H18V13H16V9.41L12,13.41V16H20V4H8V12H10.59M22,2V18H12V22H2V12H6V2H22M10,14H4V20H10V14Z";--icon-external-source-placeholder: "M6.341 3.27a10.5 10.5 0 0 1 5.834-1.77.75.75 0 0 0 0-1.5 12 12 0 1 0 12 12 .75.75 0 0 0-1.5 0A10.5 10.5 0 1 1 6.34 3.27Zm14.145 1.48a.75.75 0 1 0-1.06-1.062L9.925 13.19V7.95a.75.75 0 1 0-1.5 0V15c0 .414.336.75.75.75h7.05a.75.75 0 0 0 0-1.5h-5.24l9.501-9.5Z";--icon-facebook: "m12 1.5c-5.79901 0-10.5 4.70099-10.5 10.5 0 4.9427 3.41586 9.0888 8.01562 10.2045v-6.1086h-2.13281c-.41421 0-.75-.3358-.75-.75v-3.2812c0-.4142.33579-.75.75-.75h2.13281v-1.92189c0-.95748.22571-2.51089 1.38068-3.6497 1.1934-1.17674 3.1742-1.71859 6.2536-1.05619.3455.07433.5923.3798.5923.73323v2.75395c0 .41422-.3358.75-.75.75-.6917 0-1.2029.02567-1.5844.0819-.3865.05694-.5781.13711-.675.20223-.1087.07303-.2367.20457-.2367 1.02837v1.0781h2.3906c.2193 0 .4275.0959.57.2626.1425.1666.205.3872.1709.6038l-.5156 3.2813c-.0573.3647-.3716.6335-.7409.6335h-1.875v6.1058c4.5939-1.1198 8.0039-5.2631 8.0039-10.2017 0-5.79901-4.701-10.5-10.5-10.5zm-12 10.5c0-6.62744 5.37256-12 12-12 6.6274 0 12 5.37256 12 12 0 5.9946-4.3948 10.9614-10.1384 11.8564-.2165.0337-.4369-.0289-.6033-.1714s-.2622-.3506-.2622-.5697v-7.7694c0-.4142.3358-.75.75-.75h1.9836l.28-1.7812h-2.2636c-.4142 0-.75-.3358-.75-.75v-1.8281c0-.82854.0888-1.72825.9-2.27338.3631-.24396.8072-.36961 1.293-.4412.3081-.0454.6583-.07238 1.0531-.08618v-1.39629c-2.4096-.40504-3.6447.13262-4.2928.77165-.7376.72735-.9338 1.79299-.9338 2.58161v2.67189c0 .4142-.3358.75-.75.75h-2.13279v1.7812h2.13279c.4142 0 .75.3358.75.75v7.7712c0 .219-.0956.427-.2619.5695-.1662.1424-.3864.2052-.6028.1717-5.74968-.8898-10.1509-5.8593-10.1509-11.8583z";--icon-dropbox: "m6.01895 1.92072c.24583-.15659.56012-.15658.80593.00003l5.17512 3.29711 5.1761-3.29714c.2458-.15659.5601-.15658.8059.00003l5.5772 3.55326c.2162.13771.347.37625.347.63253 0 .25629-.1308.49483-.347.63254l-4.574 2.91414 4.574 2.91418c.2162.1377.347.3762.347.6325s-.1308.4948-.347.6325l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.1761-3.2971-5.17512 3.2971c-.24581.1566-.5601.1566-.80593 0l-5.578142-3.5532c-.216172-.1377-.347058-.3763-.347058-.6326s.130886-.4949.347058-.6326l4.574772-2.91408-4.574772-2.91411c-.216172-.1377-.347058-.37626-.347058-.63257 0-.2563.130886-.49486.347058-.63256zm.40291 8.61518-4.18213 2.664 4.18213 2.664 4.18144-2.664zm6.97504 2.664 4.1821 2.664 4.1814-2.664-4.1814-2.664zm2.7758-3.54668-4.1727 2.65798-4.17196-2.65798 4.17196-2.658zm1.4063-.88268 4.1814-2.664-4.1814-2.664-4.1821 2.664zm-6.9757-2.664-4.18144-2.664-4.18213 2.664 4.18213 2.664zm-4.81262 12.43736c.22254-.3494.68615-.4522 1.03551-.2297l5.17521 3.2966 5.1742-3.2965c.3493-.2226.813-.1198 1.0355.2295.2226.3494.1198.813-.2295 1.0355l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.57819-3.5532c-.34936-.2226-.45216-.6862-.22963-1.0355z";--icon-gdrive: "m7.73633 1.81806c.13459-.22968.38086-.37079.64707-.37079h7.587c.2718 0 .5223.14697.6548.38419l7.2327 12.94554c.1281.2293.1269.5089-.0031.7371l-3.7935 6.6594c-.1334.2342-.3822.3788-.6517.3788l-14.81918.0004c-.26952 0-.51831-.1446-.65171-.3788l-3.793526-6.6598c-.1327095-.233-.130949-.5191.004617-.7504zm.63943 1.87562-6.71271 11.45452 2.93022 5.1443 6.65493-11.58056zm3.73574 6.52652-2.39793 4.1727 4.78633.0001zm4.1168 4.1729 5.6967-.0002-6.3946-11.44563h-5.85354zm5.6844 1.4998h-13.06111l-2.96515 5.1598 13.08726-.0004z";--icon-gphotos: "M12.51 0c-.702 0-1.272.57-1.272 1.273V7.35A6.381 6.381 0 0 0 0 11.489c0 .703.57 1.273 1.273 1.273H7.35A6.381 6.381 0 0 0 11.488 24c.704 0 1.274-.57 1.274-1.273V16.65A6.381 6.381 0 0 0 24 12.51c0-.703-.57-1.273-1.273-1.273H16.65A6.381 6.381 0 0 0 12.511 0Zm.252 11.232V1.53a4.857 4.857 0 0 1 0 9.702Zm-1.53.006H1.53a4.857 4.857 0 0 1 9.702 0Zm1.536 1.524a4.857 4.857 0 0 0 9.702 0h-9.702Zm-6.136 4.857c0-2.598 2.04-4.72 4.606-4.85v9.7a4.857 4.857 0 0 1-4.606-4.85Z";--icon-instagram: "M6.225 12a5.775 5.775 0 1 1 11.55 0 5.775 5.775 0 0 1-11.55 0zM12 7.725a4.275 4.275 0 1 0 0 8.55 4.275 4.275 0 0 0 0-8.55zM18.425 6.975a1.4 1.4 0 1 0 0-2.8 1.4 1.4 0 0 0 0 2.8zM11.958.175h.084c2.152 0 3.823 0 5.152.132 1.35.134 2.427.41 3.362 1.013a7.15 7.15 0 0 1 2.124 2.124c.604.935.88 2.012 1.013 3.362.132 1.329.132 3 .132 5.152v.084c0 2.152 0 3.823-.132 5.152-.134 1.35-.41 2.427-1.013 3.362a7.15 7.15 0 0 1-2.124 2.124c-.935.604-2.012.88-3.362 1.013-1.329.132-3 .132-5.152.132h-.084c-2.152 0-3.824 0-5.153-.132-1.35-.134-2.427-.409-3.36-1.013a7.15 7.15 0 0 1-2.125-2.124C.716 19.62.44 18.544.307 17.194c-.132-1.329-.132-3-.132-5.152v-.084c0-2.152 0-3.823.132-5.152.133-1.35.409-2.427 1.013-3.362A7.15 7.15 0 0 1 3.444 1.32C4.378.716 5.456.44 6.805.307c1.33-.132 3-.132 5.153-.132zM6.953 1.799c-1.234.123-2.043.36-2.695.78A5.65 5.65 0 0 0 2.58 4.26c-.42.65-.657 1.46-.78 2.695C1.676 8.2 1.675 9.797 1.675 12c0 2.203 0 3.8.124 5.046.123 1.235.36 2.044.78 2.696a5.649 5.649 0 0 0 1.68 1.678c.65.421 1.46.658 2.694.78 1.247.124 2.844.125 5.047.125s3.8 0 5.046-.124c1.235-.123 2.044-.36 2.695-.78a5.648 5.648 0 0 0 1.68-1.68c.42-.65.657-1.46.78-2.694.123-1.247.124-2.844.124-5.047s-.001-3.8-.125-5.046c-.122-1.235-.359-2.044-.78-2.695a5.65 5.65 0 0 0-1.679-1.68c-.651-.42-1.46-.657-2.695-.78-1.246-.123-2.843-.124-5.046-.124-2.203 0-3.8 0-5.047.124z";--icon-flickr: "M5.95874 7.92578C3.66131 7.92578 1.81885 9.76006 1.81885 11.9994C1.81885 14.2402 3.66145 16.0744 5.95874 16.0744C8.26061 16.0744 10.1039 14.2396 10.1039 11.9994C10.1039 9.76071 8.26074 7.92578 5.95874 7.92578ZM0.318848 11.9994C0.318848 8.91296 2.85168 6.42578 5.95874 6.42578C9.06906 6.42578 11.6039 8.91232 11.6039 11.9994C11.6039 15.0877 9.06919 17.5744 5.95874 17.5744C2.85155 17.5744 0.318848 15.0871 0.318848 11.9994ZM18.3898 7.92578C16.0878 7.92578 14.2447 9.76071 14.2447 11.9994C14.2447 14.2396 16.088 16.0744 18.3898 16.0744C20.6886 16.0744 22.531 14.2401 22.531 11.9994C22.531 9.76019 20.6887 7.92578 18.3898 7.92578ZM12.7447 11.9994C12.7447 8.91232 15.2795 6.42578 18.3898 6.42578C21.4981 6.42578 24.031 8.91283 24.031 11.9994C24.031 15.0872 21.4982 17.5744 18.3898 17.5744C15.2794 17.5744 12.7447 15.0877 12.7447 11.9994Z";--icon-vk: var(--icon-external-source-placeholder);--icon-evernote: "M9.804 2.27v-.048c.055-.263.313-.562.85-.562h.44c.142 0 .325.014.526.033.066.009.124.023.267.06l.13.032h.002c.319.079.515.275.644.482a1.461 1.461 0 0 1 .16.356l.004.012a.75.75 0 0 0 .603.577l1.191.207a1988.512 1988.512 0 0 0 2.332.402c.512.083 1.1.178 1.665.442.64.3 1.19.795 1.376 1.77.548 2.931.657 5.829.621 8a39.233 39.233 0 0 1-.125 2.602 17.518 17.518 0 0 1-.092.849.735.735 0 0 0-.024.112c-.378 2.705-1.269 3.796-2.04 4.27-.746.457-1.53.451-2.217.447h-.192c-.46 0-1.073-.23-1.581-.635-.518-.412-.763-.87-.763-1.217 0-.45.188-.688.355-.786.161-.095.436-.137.796.087a.75.75 0 1 0 .792-1.274c-.766-.476-1.64-.52-2.345-.108-.7.409-1.098 1.188-1.098 2.08 0 .996.634 1.84 1.329 2.392.704.56 1.638.96 2.515.96l.185.002c.667.009 1.874.025 3.007-.67 1.283-.786 2.314-2.358 2.733-5.276.01-.039.018-.078.022-.105.011-.061.023-.14.034-.23.023-.184.051-.445.079-.772.055-.655.111-1.585.13-2.704.037-2.234-.074-5.239-.647-8.301v-.002c-.294-1.544-1.233-2.391-2.215-2.85-.777-.363-1.623-.496-2.129-.576-.097-.015-.18-.028-.25-.041l-.006-.001-1.99-.345-.761-.132a2.93 2.93 0 0 0-.182-.338A2.532 2.532 0 0 0 12.379.329l-.091-.023a3.967 3.967 0 0 0-.493-.103L11.769.2a7.846 7.846 0 0 0-.675-.04h-.44c-.733 0-1.368.284-1.795.742L2.416 7.431c-.468.428-.751 1.071-.751 1.81 0 .02 0 .041.003.062l.003.034c.017.21.038.468.096.796.107.715.275 1.47.391 1.994.029.13.055.245.075.342l.002.008c.258 1.141.641 1.94.978 2.466.168.263.323.456.444.589a2.808 2.808 0 0 0 .192.194c1.536 1.562 3.713 2.196 5.731 2.08.13-.005.35-.032.537-.073a2.627 2.627 0 0 0 .652-.24c.425-.26.75-.661.992-1.046.184-.294.342-.61.473-.915.197.193.412.357.627.493a5.022 5.022 0 0 0 1.97.709l.023.002.018.003.11.016c.088.014.205.035.325.058l.056.014c.088.022.164.04.235.061a1.736 1.736 0 0 1 .145.048l.03.014c.765.34 1.302 1.09 1.302 1.871a.75.75 0 0 0 1.5 0c0-1.456-.964-2.69-2.18-3.235-.212-.103-.5-.174-.679-.217l-.063-.015a10.616 10.616 0 0 0-.606-.105l-.02-.003-.03-.003h-.002a3.542 3.542 0 0 1-1.331-.485c-.471-.298-.788-.692-.828-1.234a.75.75 0 0 0-1.48-.106l-.001.003-.004.017a8.23 8.23 0 0 1-.092.352 9.963 9.963 0 0 1-.298.892c-.132.34-.29.68-.47.966-.174.276-.339.454-.478.549a1.178 1.178 0 0 1-.221.072 1.949 1.949 0 0 1-.241.036h-.013l-.032.002c-1.684.1-3.423-.437-4.604-1.65a.746.746 0 0 0-.053-.05L4.84 14.6a1.348 1.348 0 0 1-.07-.073 2.99 2.99 0 0 1-.293-.392c-.242-.379-.558-1.014-.778-1.985a54.1 54.1 0 0 0-.083-.376 27.494 27.494 0 0 1-.367-1.872l-.003-.02a6.791 6.791 0 0 1-.08-.67c.004-.277.086-.475.2-.609l.067-.067a.63.63 0 0 1 .292-.145h.05c.18 0 1.095.055 2.013.115l1.207.08.534.037a.747.747 0 0 0 .052.002c.782 0 1.349-.206 1.759-.585l.005-.005c.553-.52.622-1.225.622-1.76V6.24l-.026-.565A774.97 774.97 0 0 1 9.885 4.4c-.042-.961-.081-1.939-.081-2.13ZM4.995 6.953a251.126 251.126 0 0 1 2.102.137l.508.035c.48-.004.646-.122.715-.185.07-.068.146-.209.147-.649l-.024-.548a791.69 791.69 0 0 1-.095-2.187L4.995 6.953Zm16.122 9.996ZM15.638 11.626a.75.75 0 0 0 1.014.31 2.04 2.04 0 0 1 .304-.089 1.84 1.84 0 0 1 .544-.039c.215.023.321.06.37.085.033.016.039.026.047.04a.75.75 0 0 0 1.289-.767c-.337-.567-.906-.783-1.552-.85a3.334 3.334 0 0 0-1.002.062c-.27.056-.531.14-.705.234a.75.75 0 0 0-.31 1.014Z";--icon-box: "M1.01 4.148a.75.75 0 0 1 .75.75v4.348a4.437 4.437 0 0 1 2.988-1.153c1.734 0 3.23.992 3.978 2.438a4.478 4.478 0 0 1 3.978-2.438c2.49 0 4.488 2.044 4.488 4.543 0 2.5-1.999 4.544-4.488 4.544a4.478 4.478 0 0 1-3.978-2.438 4.478 4.478 0 0 1-3.978 2.438C2.26 17.18.26 15.135.26 12.636V4.898a.75.75 0 0 1 .75-.75Zm.75 8.488c0 1.692 1.348 3.044 2.988 3.044s2.989-1.352 2.989-3.044c0-1.691-1.349-3.043-2.989-3.043S1.76 10.945 1.76 12.636Zm10.944-3.043c-1.64 0-2.988 1.352-2.988 3.043 0 1.692 1.348 3.044 2.988 3.044s2.988-1.352 2.988-3.044c0-1.69-1.348-3.043-2.988-3.043Zm4.328-1.23a.75.75 0 0 1 1.052.128l2.333 2.983 2.333-2.983a.75.75 0 0 1 1.181.924l-2.562 3.277 2.562 3.276a.75.75 0 1 1-1.181.924l-2.333-2.983-2.333 2.983a.75.75 0 1 1-1.181-.924l2.562-3.276-2.562-3.277a.75.75 0 0 1 .129-1.052Z";--icon-onedrive: "M13.616 4.147a7.689 7.689 0 0 0-7.642 3.285A6.299 6.299 0 0 0 1.455 17.3c.684.894 2.473 2.658 5.17 2.658h12.141c.95 0 1.882-.256 2.697-.743.815-.486 1.514-1.247 1.964-2.083a5.26 5.26 0 0 0-3.713-7.612 7.69 7.69 0 0 0-6.098-5.373ZM3.34 17.15c.674.63 1.761 1.308 3.284 1.308h12.142a3.76 3.76 0 0 0 2.915-1.383l-7.494-4.489L3.34 17.15Zm10.875-6.25 2.47-1.038a5.239 5.239 0 0 1 1.427-.389 6.19 6.19 0 0 0-10.3-1.952 6.338 6.338 0 0 1 2.118.813l4.285 2.567Zm4.55.033c-.512 0-1.019.104-1.489.307l-.006.003-1.414.594 6.521 3.906a3.76 3.76 0 0 0-3.357-4.8l-.254-.01ZM4.097 9.617A4.799 4.799 0 0 1 6.558 8.9c.9 0 1.84.25 2.587.713l3.4 2.037-10.17 4.28a4.799 4.799 0 0 1 1.721-6.312Z";--icon-huddle: "M6.204 2.002c-.252.23-.357.486-.357.67V21.07c0 .15.084.505.313.812.208.28.499.477.929.477.519 0 .796-.174.956-.365.178-.212.286-.535.286-.924v-.013l.117-6.58c.004-1.725 1.419-3.883 3.867-3.883 1.33 0 2.332.581 2.987 1.364.637.762.95 1.717.95 2.526v6.47c0 .392.11.751.305.995.175.22.468.41 1.008.41.52 0 .816-.198 1.002-.437.207-.266.31-.633.31-.969V14.04c0-2.81-1.943-5.108-4.136-5.422a5.971 5.971 0 0 0-3.183.41c-.912.393-1.538.96-1.81 1.489a.75.75 0 0 1-1.417-.344v-7.5c0-.587-.47-1.031-1.242-1.031-.315 0-.638.136-.885.36ZM5.194.892A2.844 2.844 0 0 1 7.09.142c1.328 0 2.742.867 2.742 2.53v5.607a6.358 6.358 0 0 1 1.133-.629 7.47 7.47 0 0 1 3.989-.516c3.056.436 5.425 3.482 5.425 6.906v6.914c0 .602-.177 1.313-.627 1.89-.47.605-1.204 1.016-2.186 1.016-.96 0-1.698-.37-2.179-.973-.46-.575-.633-1.294-.633-1.933v-6.469c0-.456-.19-1.071-.602-1.563-.394-.471-.986-.827-1.836-.827-1.447 0-2.367 1.304-2.367 2.39v.014l-.117 6.58c-.001.64-.177 1.333-.637 1.881-.48.57-1.2.9-2.105.9-.995 0-1.7-.5-2.132-1.081-.41-.552-.61-1.217-.61-1.708V2.672c0-.707.366-1.341.847-1.78Z"}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-tabs{display:grid;grid-template-rows:min-content minmax(var(--ui-size),auto);height:100%;overflow:hidden;color:var(--clr-txt-lightest)}lr-tabs>.tabs-row{display:flex;grid-template-columns:minmax();background-color:var(--clr-background-light)}lr-tabs>.tabs-context{overflow-y:auto}lr-tabs .tabs-row>.tab{display:flex;flex-grow:1;align-items:center;justify-content:center;height:var(--ui-size);border-bottom:var(--border-light);cursor:pointer;transition:var(--transition-duration)}lr-tabs .tabs-row>.tab[current]{color:var(--clr-txt);border-color:var(--clr-txt)}lr-range{position:relative;display:inline-flex;align-items:center;justify-content:center;height:var(--ui-size)}lr-range datalist{display:none}lr-range input{width:100%;height:100%;opacity:0}lr-range .track-wrapper{position:absolute;right:10px;left:10px;display:flex;align-items:center;justify-content:center;height:2px;user-select:none;pointer-events:none}lr-range .track{position:absolute;right:0;left:0;display:flex;align-items:center;justify-content:center;height:2px;background-color:currentColor;border-radius:2px;opacity:.5}lr-range .slider{position:absolute;width:16px;height:16px;background-color:currentColor;border-radius:100%;transform:translate(-50%)}lr-range .bar{position:absolute;left:0;height:100%;background-color:currentColor;border-radius:2px}lr-range .caption{position:absolute;display:inline-flex;justify-content:center}lr-color{position:relative;display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size);overflow:hidden;background-color:var(--clr-background);cursor:pointer}lr-color[current]{background-color:var(--clr-txt)}lr-color input[type=color]{position:absolute;display:block;width:100%;height:100%;opacity:0}lr-color .current-color{position:absolute;width:50%;height:50%;border:2px solid #fff;border-radius:100%;pointer-events:none}lr-config{display:none}lr-simple-btn{position:relative;display:inline-flex}lr-simple-btn button{padding-left:.2em!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-simple-btn button lr-icon svg{transform:scale(.8)}lr-simple-btn button:hover{background-color:var(--clr-btn-bgr-secondary-hover)}lr-simple-btn button:active{background-color:var(--clr-btn-bgr-secondary-active)}lr-simple-btn>lr-drop-area{display:contents}lr-simple-btn .visual-drop-area{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;padding:var(--gap-min);border:var(--border-dashed);border-radius:inherit;opacity:0;transition:border-color var(--transition-duration) ease,background-color var(--transition-duration) ease,opacity var(--transition-duration) ease}lr-simple-btn .visual-drop-area:before{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;color:var(--clr-txt-light);background-color:var(--clr-background);border-radius:inherit;content:var(--l10n-drop-files-here)}lr-simple-btn>lr-drop-area[drag-state=active] .visual-drop-area{background-color:var(--clr-accent-lightest);opacity:1}lr-simple-btn>lr-drop-area[drag-state=inactive] .visual-drop-area{background-color:var(--clr-shade-lv1);opacity:0}lr-simple-btn>lr-drop-area[drag-state=near] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent-light);opacity:1}lr-simple-btn>lr-drop-area[drag-state=over] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent);opacity:1}lr-simple-btn>:where(lr-drop-area[drag-state=active],lr-drop-area[drag-state=near],lr-drop-area[drag-state=over]) button{box-shadow:none}lr-simple-btn>lr-drop-area:after{content:""}lr-source-btn{display:flex;align-items:center;margin-bottom:var(--gap-min);padding:var(--gap-min) var(--gap-mid);color:var(--clr-txt-mid);border-radius:var(--border-radius-element);cursor:pointer;transition-duration:var(--transition-duration);transition-property:background-color,color;user-select:none}lr-source-btn:hover{color:var(--clr-accent);background-color:var(--clr-accent-lightest)}lr-source-btn:active{color:var(--clr-accent);background-color:var(--clr-accent-light)}lr-source-btn lr-icon{display:inline-flex;flex-grow:1;justify-content:center;min-width:var(--ui-size);margin-right:var(--gap-mid);opacity:.8}lr-source-btn[type=local]>.txt:after{content:var(--l10n-local-files)}lr-source-btn[type=camera]>.txt:after{content:var(--l10n-camera)}lr-source-btn[type=url]>.txt:after{content:var(--l10n-from-url)}lr-source-btn[type=other]>.txt:after{content:var(--l10n-other)}lr-source-btn .txt{display:flex;align-items:center;box-sizing:border-box;width:100%;height:var(--ui-size);padding:0;white-space:nowrap;border:none}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-modal{--modal-max-content-height: calc(var(--uploadcare-blocks-window-height, 100vh) - 4 * var(--gap-mid) - var(--ui-size));--modal-content-height-fill: var(--uploadcare-blocks-window-height, 100vh)}lr-modal[dialog-fallback]{--lr-z-max: 2147483647;position:fixed;z-index:var(--lr-z-max);display:flex;align-items:center;justify-content:center;width:100vw;height:100vh;pointer-events:none;inset:0}lr-modal[dialog-fallback] dialog[open]{z-index:var(--lr-z-max);pointer-events:auto}lr-modal[dialog-fallback] dialog[open]+.backdrop{position:fixed;top:0;left:0;z-index:calc(var(--lr-z-max) - 1);align-items:center;justify-content:center;width:100vw;height:100vh;background-color:var(--clr-curtain);pointer-events:auto}lr-modal[strokes][dialog-fallback] dialog[open]+.backdrop{background-image:var(--modal-backdrop-background-image)}@supports selector(dialog::backdrop){lr-modal>dialog::backdrop{background-color:#0000001a}lr-modal[strokes]>dialog::backdrop{background-image:var(--modal-backdrop-background-image)}}lr-modal>dialog[open]{transform:translateY(0);visibility:visible;opacity:1}lr-modal>dialog:not([open]){transform:translateY(20px);visibility:hidden;opacity:0}lr-modal>dialog{display:flex;flex-direction:column;width:max-content;max-width:min(calc(100% - var(--gap-mid) * 2),calc(var(--modal-max-w) - var(--gap-mid) * 2));min-height:var(--ui-size);max-height:calc(var(--modal-max-h) - var(--gap-mid) * 2);margin:auto;padding:0;overflow:hidden;background-color:var(--clr-background-light);border:0;border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:transform calc(var(--transition-duration) * 2)}@media only screen and (max-width: 430px),only screen and (max-height: 600px){lr-modal>dialog>.content{height:var(--modal-max-content-height)}}lr-url-source{display:block;background-color:var(--clr-background-light)}lr-modal lr-url-source{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-url-source>.content{display:grid;grid-gap:var(--gap-small);grid-template-columns:1fr min-content;padding:var(--gap-mid);padding-top:0}lr-url-source .url-input{display:flex}lr-url-source .url-upload-btn:after{content:var(--l10n-upload-url)}lr-camera-source{position:relative;display:flex;flex-direction:column;width:100%;height:100%;max-height:100%;overflow:hidden;background-color:var(--clr-background-light);border-radius:var(--border-radius-element)}lr-modal lr-camera-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:100vh;max-height:var(--modal-max-content-height)}lr-camera-source.initialized{height:max-content}@media only screen and (max-width: 430px){lr-camera-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-camera-source video{display:block;width:100%;max-height:100%;object-fit:contain;object-position:center center;background-color:var(--clr-background-dark);border-radius:var(--border-radius-element)}lr-camera-source .toolbar{position:absolute;bottom:0;display:flex;justify-content:space-between;width:100%;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-camera-source .content{display:flex;flex:1;justify-content:center;width:100%;padding:var(--gap-mid);padding-top:0;overflow:hidden}lr-camera-source .message-box{--padding: calc(var(--gap-max) * 2);display:flex;flex-direction:column;grid-gap:var(--gap-max);align-items:center;justify-content:center;padding:var(--padding) var(--padding) 0 var(--padding);color:var(--clr-txt)}lr-camera-source .message-box button{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary)}lr-camera-source .shot-btn{position:absolute;bottom:var(--gap-max);width:calc(var(--ui-size) * 1.8);height:calc(var(--ui-size) * 1.8);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;opacity:.85;transition:var(--transition-duration) ease}lr-camera-source .shot-btn:hover{transform:scale(1.05);opacity:1}lr-camera-source .shot-btn:active{background-color:var(--clr-txt-mid);opacity:1}lr-camera-source .shot-btn[disabled]{bottom:calc(var(--gap-max) * -1 - var(--gap-mid) - var(--ui-size) * 2)}lr-camera-source .shot-btn lr-icon svg{width:calc(var(--ui-size) / 1.5);height:calc(var(--ui-size) / 1.5)}lr-external-source{display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--clr-background-light);overflow:hidden}lr-modal lr-external-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height)}lr-external-source>.content{position:relative;display:grid;flex:1;grid-template-rows:1fr min-content}@media only screen and (max-width: 430px){lr-external-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-external-source iframe{display:block;width:100%;height:100%;border:none}lr-external-source .iframe-wrapper{overflow:hidden}lr-external-source .toolbar{display:grid;grid-gap:var(--gap-mid);grid-template-columns:max-content 1fr max-content max-content;align-items:center;width:100%;padding:var(--gap-mid);border-top:var(--border-light)}lr-external-source .back-btn{padding-left:0}lr-external-source .back-btn:after{content:var(--l10n-back)}lr-external-source .selected-counter{display:flex;grid-gap:var(--gap-mid);align-items:center;justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt-light)}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-upload-details{display:flex;flex-direction:column;width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height);overflow:hidden;background-color:var(--clr-background-light)}lr-upload-details>.content{position:relative;display:grid;flex:1;grid-template-rows:auto min-content}lr-upload-details lr-tabs .tabs-context{position:relative}lr-upload-details .toolbar{display:grid;grid-template-columns:min-content min-content 1fr min-content;gap:var(--gap-mid);padding:var(--gap-mid);border-top:var(--border-light)}lr-upload-details .toolbar[edit-disabled]{display:flex;justify-content:space-between}lr-upload-details .remove-btn{padding-left:.5em}lr-upload-details .detail-btn{padding-left:0;color:var(--clr-txt);background-color:var(--clr-background)}lr-upload-details .edit-btn{padding-left:.5em}lr-upload-details .details{padding:var(--gap-max)}lr-upload-details .info-block{padding-top:var(--gap-max);padding-bottom:calc(var(--gap-max) + var(--gap-table));color:var(--clr-txt);border-bottom:var(--border-light)}lr-upload-details .info-block:first-of-type{padding-top:0}lr-upload-details .info-block:last-of-type{border-bottom:none}lr-upload-details .info-block>.info-block_name{margin-bottom:.4em;color:var(--clr-txt-light);font-size:.8em}lr-upload-details .cdn-link[disabled]{pointer-events:none}lr-upload-details .cdn-link[disabled]:before{filter:grayscale(1);content:var(--l10n-not-uploaded-yet)}lr-file-preview{position:absolute;inset:0;display:flex;align-items:center;justify-content:center}lr-file-preview>lr-img{display:contents}lr-file-preview>lr-img>.img-view{position:absolute;inset:0;width:100%;max-width:100%;height:100%;max-height:100%;object-fit:scale-down}lr-confirmation-dialog{display:block;padding:var(--gap-mid);padding-top:var(--gap-max)}lr-confirmation-dialog .message{display:flex;justify-content:center;padding:var(--gap-mid);padding-bottom:var(--gap-max);font-weight:500;font-size:1.1em}lr-confirmation-dialog .toolbar{display:grid;grid-template-columns:1fr 1fr;gap:var(--gap-mid);margin-top:var(--gap-mid)}lr-progress-bar-common{position:fixed;right:0;bottom:0;left:0;z-index:10000;display:block;height:var(--gap-mid);background-color:var(--clr-background);transition:opacity .3s}lr-progress-bar-common:not([active]){opacity:0;pointer-events:none}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--unknown{width:100%;transform-origin:0% 50%;animation:lr-indeterminateAnimation 1s infinite linear}lr-progress-bar .progress--hidden{opacity:0}@keyframes lr-indeterminateAnimation{0%{transform:translate(0) scaleX(0)}40%{transform:translate(0) scaleX(.4)}to{transform:translate(100%) scaleX(.5)}}lr-activity-header{display:flex;gap:var(--gap-mid);justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt);font-weight:500;font-size:1em;line-height:var(--ui-size)}lr-activity-header lr-icon{height:var(--ui-size)}lr-activity-header>*{display:flex;align-items:center}lr-activity-header button{display:inline-flex;align-items:center;justify-content:center;color:var(--clr-txt-mid)}lr-activity-header button:hover{background-color:var(--clr-background)}lr-activity-header button:active{background-color:var(--clr-background-dark)}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:host(.lr-cloud-image-editor) lr-icon,.lr-cloud-image-editor lr-icon{display:flex;align-items:center;justify-content:center;width:100%;height:100%}:host(.lr-cloud-image-editor) lr-icon svg,.lr-cloud-image-editor lr-icon svg{width:unset;height:unset}:host(.lr-cloud-image-editor) lr-icon:not([raw]) path,.lr-cloud-image-editor lr-icon:not([raw]) path{stroke-linejoin:round;fill:none;stroke:currentColor;stroke-width:1.2}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--icon-rotate: "M13.5.399902L12 1.9999l1.5 1.6M12.0234 2H14.4C16.3882 2 18 3.61178 18 5.6V8M4 17h9c.5523 0 1-.4477 1-1V7c0-.55228-.4477-1-1-1H4c-.55228 0-1 .44771-1 1v9c0 .5523.44771 1 1 1z";--icon-mirror: "M5.00042.399902l-1.5 1.599998 1.5 1.6M15.0004.399902l1.5 1.599998-1.5 1.6M3.51995 2H16.477M8.50042 16.7V6.04604c0-.30141-.39466-.41459-.5544-.159L1.28729 16.541c-.12488.1998.01877.459.2544.459h6.65873c.16568 0 .3-.1343.3-.3zm2.99998 0V6.04604c0-.30141.3947-.41459.5544-.159L18.7135 16.541c.1249.1998-.0187.459-.2544.459h-6.6587c-.1657 0-.3-.1343-.3-.3z";--icon-flip: "M19.6001 4.99993l-1.6-1.5-1.6 1.5m3.2 9.99997l-1.6 1.5-1.6-1.5M18 3.52337V16.4765M3.3 8.49993h10.654c.3014 0 .4146-.39466.159-.5544L3.459 1.2868C3.25919 1.16192 3 1.30557 3 1.5412v6.65873c0 .16568.13432.3.3.3zm0 2.99997h10.654c.3014 0 .4146.3947.159.5544L3.459 18.7131c-.19981.1248-.459-.0188-.459-.2544v-6.6588c0-.1657.13432-.3.3-.3z";--icon-sad: "M2 17c4.41828-4 11.5817-4 16 0M16.5 5c0 .55228-.4477 1-1 1s-1-.44772-1-1 .4477-1 1-1 1 .44772 1 1zm-11 0c0 .55228-.44772 1-1 1s-1-.44772-1-1 .44772-1 1-1 1 .44772 1 1z";--icon-closeMax: "M3 3l14 14m0-14L3 17";--icon-crop: "M20 14H7.00513C6.45001 14 6 13.55 6 12.9949V0M0 6h13.0667c.5154 0 .9333.41787.9333.93333V20M14.5.399902L13 1.9999l1.5 1.6M13 2h2c1.6569 0 3 1.34315 3 3v2M5.5 19.5999l1.5-1.6-1.5-1.6M7 18H5c-1.65685 0-3-1.3431-3-3v-2";--icon-tuning: "M8 10h11M1 10h4M1 4.5h11m3 0h4m-18 11h11m3 0h4M12 4.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M5 10a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M12 15.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0";--icon-filters: "M4.5 6.5a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m-3.5 6a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m7 0a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0";--icon-done: "M1 10.6316l5.68421 5.6842L19 4";--icon-original: "M0 40L40-.00000133";--icon-slider: "M0 10h11m0 0c0 1.1046.8954 2 2 2s2-.8954 2-2m-4 0c0-1.10457.8954-2 2-2s2 .89543 2 2m0 0h5";--icon-exposure: "M10 20v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M5 10a5 5 0 1010 0 5 5 0 10-10 0";--icon-contrast: "M2 10a8 8 0 1016 0 8 8 0 10-16 0m8-8v16m8-8h-8m7.5977 2.5H10m6.24 2.5H10m7.6-7.5H10M16.2422 5H10";--icon-brightness: "M15 10c0 2.7614-2.2386 5-5 5m5-5c0-2.76142-2.2386-5-5-5m5 5h-5m0 5c-2.76142 0-5-2.2386-5-5 0-2.76142 2.23858-5 5-5m0 10V5m0 15v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M14.3242 7.5H10m4.3242 5H10";--icon-gamma: "M17 3C9 6 2.5 11.5 2.5 17.5m0 0h1m-1 0v-1m14 1h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3-14v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1";--icon-enhance: "M19 13h-2m0 0c-2.2091 0-4-1.7909-4-4m4 4c-2.2091 0-4 1.7909-4 4m0-8V7m0 2c0 2.2091-1.7909 4-4 4m-2 0h2m0 0c2.2091 0 4 1.7909 4 4m0 0v2M8 8.5H6.5m0 0c-1.10457 0-2-.89543-2-2m2 2c-1.10457 0-2 .89543-2 2m0-4V5m0 1.5c0 1.10457-.89543 2-2 2M1 8.5h1.5m0 0c1.10457 0 2 .89543 2 2m0 0V12M12 3h-1m0 0c-.5523 0-1-.44772-1-1m1 1c-.5523 0-1 .44772-1 1m0-2V1m0 1c0 .55228-.44772 1-1 1M8 3h1m0 0c.55228 0 1 .44772 1 1m0 0v1";--icon-saturation: '    <circle cx="10.0006" cy="10.0001" r="9" transform="rotate(90 10.0006 10.0001)" fill="url(#paint0_linear)"/>     <defs>       <linearGradient id="paint0_linear" x1="10.0006" y1="1.00009" x2="10.0006" y2="19.0001" gradientUnits="userSpaceOnUse">         <stop stop-color="#DE15FF"/>         <stop offset=".203125" stop-color="#0029FF"/>         <stop offset=".479167" stop-color="#2AE4F0"/>         <stop offset=".604167" stop-color="#15EF11"/>         <stop offset=".75" stop-color="#FAE528"/>         <stop offset="1" stop-color="#EB2A2A"/>       </linearGradient>     </defs>  ';--icon-warmth: '    <path d="M7.5 13.0505l.42854.4199.17146-.1749v-.245h-.6zm5 0h-.6v.245l.1715.1749.4285-.4199zM8.1 3.5c0-1.04934.85066-1.9 1.9-1.9V.4C8.28792.4 6.9 1.78792 6.9 3.5h1.2zm0 9.5505V3.5H6.9v9.5505h1.2zM7.1 15.5c0-.7904.31539-1.5059.82854-2.0296l-.85708-.8398C6.34742 13.3694 5.9 14.3831 5.9 15.5h1.2zm2.9 2.9c-1.60163 0-2.9-1.2984-2.9-2.9H5.9c0 2.2644 1.83563 4.1 4.1 4.1v-1.2zm2.9-2.9c0 1.6016-1.2984 2.9-2.9 2.9v1.2c2.2644 0 4.1-1.8356 4.1-4.1h-1.2zm-.8285-2.0296c.5131.5237.8285 1.2392.8285 2.0296h1.2c0-1.1169-.4474-2.1306-1.1715-2.8694l-.857.8398zM11.9 3.5v9.5505h1.2V3.5h-1.2zM10 1.6c1.0493 0 1.9.85066 1.9 1.9h1.2c0-1.71208-1.3879-3.1-3.1-3.1v1.2z" fill="currentColor"/>    <path d="M10 14V8" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/>    <path d="M14 3h3m-3 3h3m-3 3h3m-8 6.5a1 1 0 102 0 1 1 0 10-2 0" stroke="currentColor" stroke-width="1.2"/>  ';--icon-vibrance: '  <path d="M2.125 5.6407c-.71643 1.29152-1.12439 2.77782-1.12439 4.3594 0 1.5816.40796 3.0679 1.12439 4.3594V5.6407z" fill="url(#paint0_linear)"/>  <path d="M2.875 15.4986V4.5016c.50222-.64987 1.09136-1.22915 1.75-1.72041V17.219c-.65864-.4912-1.24778-1.0705-1.75-1.7204z" fill="url(#paint1_linear)"/>  <path d="M5.375 17.722c.54811.3291 1.13415.6014 1.75.8089V1.46929c-.61585.20751-1.20189.47984-1.75.80888V17.722z" fill="url(#paint2_linear)"/>  <path d="M7.875 1.25258V18.7476c.56442.1367 1.14962.2202 1.75.2448V1.0078c-.60038.02465-1.18558.10811-1.75.24478z" fill="url(#paint3_linear)"/>  <path d="M10.375 1.00775V18.9925c.6004-.0246 1.1856-.108 1.75-.2446V1.25228c-.5644-.13658-1.1496-.21996-1.75-.24453z" fill="url(#paint4_linear)"/>  <path d="M12.875 1.46887V18.5313c.6158-.2074 1.2019-.4796 1.75-.8085V2.27744c-.5481-.32893-1.1342-.60115-1.75-.80857z" fill="url(#paint5_linear)"/>  <path d="M15.375 2.78028V17.2199c.6586-.491 1.2477-1.0701 1.75-1.7197V4.50002c-.5023-.64963-1.0914-1.22868-1.75-1.71974z" fill="url(#paint6_linear)"/>  <path d="M17.875 5.6385v8.7232c.7172-1.292 1.1256-2.7791 1.1256-4.3616 0-1.58248-.4084-3.06956-1.1256-4.3616z" fill="url(#paint7_linear)"/>  <defs>    <linearGradient id="paint0_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint1_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint2_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint3_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint4_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint5_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint6_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint7_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>  </defs>  '}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--l10n-cancel: "Cancel";--l10n-apply: "Apply";--l10n-brightness: "Brightness";--l10n-exposure: "Exposure";--l10n-gamma: "Gamma";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-vibrance: "Vibrance";--l10n-warmth: "Warmth";--l10n-enhance: "Enhance";--l10n-original: "Original"}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--rgb-primary-accent: 6, 2, 196;--rgb-text-base: 0, 0, 0;--rgb-text-accent-contrast: 255, 255, 255;--rgb-fill-contrast: 255, 255, 255;--rgb-fill-shaded: 245, 245, 245;--rgb-shadow: 0, 0, 0;--rgb-error: 209, 81, 81;--opacity-shade-mid: .2;--color-primary-accent: rgb(var(--rgb-primary-accent));--color-text-base: rgb(var(--rgb-text-base));--color-text-accent-contrast: rgb(var(--rgb-text-accent-contrast));--color-text-soft: rgb(var(--rgb-fill-contrast));--color-text-error: rgb(var(--rgb-error));--color-fill-contrast: rgb(var(--rgb-fill-contrast));--color-modal-backdrop: rgba(var(--rgb-fill-shaded), .95);--color-image-background: rgba(var(--rgb-fill-shaded));--color-outline: rgba(var(--rgb-text-base), var(--opacity-shade-mid));--color-underline: rgba(var(--rgb-text-base), .08);--color-shade: rgba(var(--rgb-text-base), .02);--color-focus-ring: var(--color-primary-accent);--color-input-placeholder: rgba(var(--rgb-text-base), .32);--color-error: rgb(var(--rgb-error));--font-size-ui: 16px;--font-size-title: 18px;--font-weight-title: 500;--font-size-soft: 14px;--size-touch-area: 40px;--size-panel-heading: 66px;--size-ui-min-width: 130px;--size-line-width: 1px;--size-modal-width: 650px;--border-radius-connect: 2px;--border-radius-editor: 3px;--border-radius-thumb: 4px;--border-radius-ui: 5px;--border-radius-base: 6px;--cldtr-gap-min: 5px;--cldtr-gap-mid-1: 10px;--cldtr-gap-mid-2: 15px;--cldtr-gap-max: 20px;--opacity-min: var(--opacity-shade-mid);--opacity-mid: .1;--opacity-max: .05;--transition-duration-2: var(--transition-duration-all, .2s);--transition-duration-3: var(--transition-duration-all, .3s);--transition-duration-4: var(--transition-duration-all, .4s);--transition-duration-5: var(--transition-duration-all, .5s);--shadow-base: 0px 5px 15px rgba(var(--rgb-shadow), .1), 0px 1px 4px rgba(var(--rgb-shadow), .15);--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading);--transparent-pixel: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=);display:block;width:100%;height:100%;max-height:100%}:host(.lr-cloud-image-editor) :is([can-handle-paste]:hover,[can-handle-paste]:focus),.lr-cloud-image-editor :is([can-handle-paste]:hover,[can-handle-paste]:focus){--can-handle-paste: "true"}:host(.lr-cloud-image-editor) :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover),.lr-cloud-image-editor :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover){--filter-effect: var(--hover-filter) !important;--opacity-effect: var(--hover-opacity) !important;--color-effect: var(--hover-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex]:active,[with-effects]:active),.lr-cloud-image-editor :is([tabindex]:active,[with-effects]:active){--filter-effect: var(--down-filter) !important;--opacity-effect: var(--down-opacity) !important;--color-effect: var(--down-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex][active],[with-effects][active]),.lr-cloud-image-editor :is([tabindex][active],[with-effects][active]){--filter-effect: var(--active-filter) !important;--opacity-effect: var(--active-opacity) !important;--color-effect: var(--active-color-rgb) !important}:host(.lr-cloud-image-editor) [hidden-scrollbar]::-webkit-scrollbar,.lr-cloud-image-editor [hidden-scrollbar]::-webkit-scrollbar{display:none}:host(.lr-cloud-image-editor) [hidden-scrollbar],.lr-cloud-image-editor [hidden-scrollbar]{-ms-overflow-style:none;scrollbar-width:none}:host(.lr-cloud-image-editor.editor_ON),.lr-cloud-image-editor.editor_ON{--modal-header-opacity: 0;--modal-header-height: 0px;--modal-toolbar-height: calc(var(--size-panel-heading) * 2)}:host(.lr-cloud-image-editor.editor_OFF),.lr-cloud-image-editor.editor_OFF{--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading)}:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-min-img-height: var(--modal-toolbar-height);--l-max-img-height: 100%;--l-edit-button-width: 120px;--l-toolbar-horizontal-padding: var(--cldtr-gap-mid-1);position:relative;display:grid;grid-template-rows:minmax(var(--l-min-img-height),var(--l-max-img-height)) minmax(var(--modal-toolbar-height),auto);height:100%;overflow:hidden;overflow-y:auto}@media only screen and (max-width: 800px){:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-edit-button-width: 70px;--l-toolbar-horizontal-padding: var(--cldtr-gap-min)}}:host(.lr-cloud-image-editor)>.wrapper>.viewport,.lr-cloud-image-editor>.wrapper>.viewport{display:flex;align-items:center;justify-content:center;overflow:hidden}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image{--viewer-image-opacity: 1;position:absolute;top:0;left:0;z-index:10;display:block;box-sizing:border-box;width:100%;height:100%;object-fit:scale-down;background-color:var(--color-image-background);transform:scale(1);opacity:var(--viewer-image-opacity);user-select:none;pointer-events:auto}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_visible_viewer,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_visible_viewer{transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-4)}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper{--viewer-image-opacity: 0;background-image:var(--transparent-pixel);transform:scale(1);transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_effects,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_effects{--viewer-image-opacity: 0;transform:scale(1);transition:opacity var(--transition-duration-3) cubic-bezier(.5,0,1,1),transform var(--transition-duration-4);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container,.lr-cloud-image-editor>.wrapper>.viewport>.image_container{position:relative;display:block;width:100%;height:100%;background-color:var(--color-image-background);transition:var(--transition-duration-3)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar,.lr-cloud-image-editor>.wrapper>.toolbar{position:relative;transition:.3s}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content{position:absolute;bottom:0;left:0;box-sizing:border-box;width:100%;height:var(--modal-toolbar-height);min-height:var(--size-panel-heading);background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer{display:flex;align-items:center;justify-content:space-between;height:var(--size-panel-heading);padding-right:var(--l-toolbar-horizontal-padding);padding-left:var(--l-toolbar-horizontal-padding)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor{display:flex}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.info_pan,.lr-cloud-image-editor>.wrapper>.viewport>.info_pan{position:absolute;user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer{position:absolute;z-index:2;display:flex;max-width:120px;transform:translate(-40px);user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer>.file_type,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer>.file_type{padding:4px .8em}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash,.lr-cloud-image-editor>.wrapper>.network_problems_splash{position:absolute;z-index:4;display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content{display:flex;flex:1;flex-direction:column;align-items:center;justify-content:center}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon{display:flex;align-items:center;justify-content:center;width:40px;height:40px;color:rgba(var(--rgb-text-base),.6);background-color:rgba(var(--rgb-fill-shaded));border-radius:50%}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text{margin-top:var(--cldtr-gap-max);font-size:var(--font-size-ui)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_footer,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_footer{display:flex;align-items:center;justify-content:center;height:var(--size-panel-heading)}lr-crop-frame>.svg{position:absolute;top:0;left:0;z-index:2;width:100%;height:100%;border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);opacity:inherit;transition:var(--transition-duration-3)}lr-crop-frame>.thumb{--idle-color-rgb: var(--color-text-base);--hover-color-rgb: var(--color-primary-accent);--focus-color-rgb: var(--color-primary-accent);--down-color-rgb: var(--color-primary-accent);--color-effect: var(--idle-color-rgb);color:var(--color-effect);transition:color var(--transition-duration-3),opacity var(--transition-duration-3)}lr-crop-frame>.thumb--visible{opacity:1;pointer-events:auto}lr-crop-frame>.thumb--hidden{opacity:0;pointer-events:none}lr-crop-frame>.guides{transition:var(--transition-duration-3)}lr-crop-frame>.guides--hidden{opacity:0}lr-crop-frame>.guides--semi-hidden{opacity:.2}lr-crop-frame>.guides--visible{opacity:1}lr-editor-button-control,lr-editor-crop-button-control,lr-editor-filter-control,lr-editor-operation-control{--l-base-min-width: 40px;--l-base-height: var(--l-base-min-width);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--filter-effect: var(--idle-filter);--idle-color-rgb: var(--rgb-text-base);--idle-opacity: .05;--idle-filter: 1;--hover-color-rgb: var(--idle-color-rgb);--hover-opacity: .08;--hover-filter: .8;--down-color-rgb: var(--hover-color-rgb);--down-opacity: .12;--down-filter: .6;position:relative;display:grid;grid-template-columns:var(--l-base-min-width) auto;align-items:center;height:var(--l-base-height);color:rgba(var(--idle-color-rgb));outline:none;cursor:pointer;transition:var(--l-width-transition)}lr-editor-button-control.active,lr-editor-operation-control.active,lr-editor-crop-button-control.active,lr-editor-filter-control.active{--idle-color-rgb: var(--rgb-primary-accent)}lr-editor-filter-control.not_active .preview[loaded]{opacity:1}lr-editor-filter-control.active .preview{opacity:0}lr-editor-button-control.not_active,lr-editor-operation-control.not_active,lr-editor-crop-button-control.not_active,lr-editor-filter-control.not_active{--idle-color-rgb: var(--rgb-text-base)}lr-editor-button-control>.before,lr-editor-operation-control>.before,lr-editor-crop-button-control>.before,lr-editor-filter-control>.before{position:absolute;right:0;left:0;z-index:-1;width:100%;height:100%;background-color:rgba(var(--color-effect),var(--opacity-effect));border-radius:var(--border-radius-editor);transition:var(--transition-duration-3)}lr-editor-button-control>.title,lr-editor-operation-control>.title,lr-editor-crop-button-control>.title,lr-editor-filter-control>.title{padding-right:var(--cldtr-gap-mid-1);font-size:.7em;letter-spacing:1.004px;text-transform:uppercase}lr-editor-filter-control>.preview{position:absolute;right:0;left:0;z-index:1;width:100%;height:var(--l-base-height);background-repeat:no-repeat;background-size:contain;border-radius:var(--border-radius-editor);opacity:0;filter:brightness(var(--filter-effect));transition:var(--transition-duration-3)}lr-editor-filter-control>.original-icon{color:var(--color-text-base);opacity:.3}lr-editor-image-cropper{position:absolute;top:0;left:0;z-index:10;display:block;width:100%;height:100%;opacity:0;pointer-events:none;touch-action:none}lr-editor-image-cropper.active_from_editor{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.active_from_viewer{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.inactive_to_editor{opacity:0;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1),opacity var(--transition-duration-3) calc(var(--transition-duration-3) + .05s);pointer-events:none}lr-editor-image-cropper>.canvas{position:absolute;top:0;left:0;z-index:1;display:block;width:100%;height:100%}lr-editor-image-fader{position:absolute;top:0;left:0;display:block;width:100%;height:100%}lr-editor-image-fader.active_from_viewer{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-start);pointer-events:auto}lr-editor-image-fader.active_from_cropper{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:auto}lr-editor-image-fader.inactive_to_cropper{z-index:3;transform:scale(1);opacity:0;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}lr-editor-image-fader .fader-image{position:absolute;top:0;left:0;display:block;width:100%;height:100%;object-fit:scale-down;transform:scale(1);user-select:none;content-visibility:auto}lr-editor-image-fader .fader-image--preview{background-color:var(--color-image-background);border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);transform:scale(1);opacity:0;transition:var(--transition-duration-3)}lr-editor-scroller{display:flex;align-items:center;width:100%;height:100%;overflow-x:scroll}lr-editor-slider{display:flex;align-items:center;justify-content:center;width:100%;height:66px}lr-editor-toolbar{position:relative;width:100%;height:100%}@media only screen and (max-width: 600px){lr-editor-toolbar{--l-tab-gap: var(--cldtr-gap-mid-1);--l-slider-padding: var(--cldtr-gap-min);--l-controls-padding: var(--cldtr-gap-min)}}@media only screen and (min-width: 601px){lr-editor-toolbar{--l-tab-gap: calc(var(--cldtr-gap-mid-1) + var(--cldtr-gap-max));--l-slider-padding: var(--cldtr-gap-mid-1);--l-controls-padding: var(--cldtr-gap-mid-1)}}lr-editor-toolbar>.toolbar-container{position:relative;width:100%;height:100%;overflow:hidden}lr-editor-toolbar>.toolbar-container>.sub-toolbar{position:absolute;display:grid;grid-template-rows:1fr 1fr;width:100%;height:100%;background-color:var(--color-fill-contrast);transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-3) ease-in-out,visibility var(--transition-duration-3) ease-in-out}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--visible{transform:translateY(0);opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--top-hidden{transform:translateY(100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--bottom-hidden{transform:translateY(-100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row{display:flex;align-items:center;justify-content:space-between;padding-right:var(--l-controls-padding);padding-left:var(--l-controls-padding)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles{position:relative;display:grid;grid-auto-flow:column;grid-gap:0px var(--l-tab-gap);align-items:center;height:100%}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggles_indicator{position:absolute;bottom:0;left:0;width:var(--size-touch-area);height:2px;background-color:var(--color-primary-accent);transform:translate(0);transition:transform var(--transition-duration-3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row{position:relative}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content{position:absolute;top:0;left:0;display:flex;width:100%;height:100%;overflow:hidden;opacity:0;content-visibility:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--visible{opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--hidden{opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--visible{display:contents}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles.tab-toggles--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_align{display:grid;grid-template-areas:". inner .";grid-template-columns:1fr auto 1fr;box-sizing:border-box;min-width:100%;padding-left:var(--cldtr-gap-max)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner{display:grid;grid-area:inner;grid-auto-flow:column;grid-gap:calc((var(--cldtr-gap-min) - 1px) * 3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner:last-child{padding-right:var(--cldtr-gap-max)}lr-editor-toolbar .controls-list_last-item{margin-right:var(--cldtr-gap-max)}lr-editor-toolbar .info-tooltip_container{position:absolute;display:flex;align-items:flex-start;justify-content:center;width:100%;height:100%}lr-editor-toolbar .info-tooltip_wrapper{position:absolute;top:calc(-100% - var(--cldtr-gap-mid-2));display:flex;flex-direction:column;justify-content:flex-end;height:100%;pointer-events:none}lr-editor-toolbar .info-tooltip{z-index:3;padding-top:calc(var(--cldtr-gap-min) / 2);padding-right:var(--cldtr-gap-min);padding-bottom:calc(var(--cldtr-gap-min) / 2);padding-left:var(--cldtr-gap-min);color:var(--color-text-base);font-size:.7em;letter-spacing:1px;text-transform:uppercase;background-color:var(--color-text-accent-contrast);border-radius:var(--border-radius-editor);transform:translateY(100%);opacity:0;transition:var(--transition-duration-3)}lr-editor-toolbar .info-tooltip_visible{transform:translateY(0);opacity:1}lr-editor-toolbar .slider{padding-right:var(--l-slider-padding);padding-left:var(--l-slider-padding)}lr-btn-ui{--filter-effect: var(--idle-brightness);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--l-transition-effect: var(--css-transition, color var(--transition-duration-2), filter var(--transition-duration-2));display:inline-flex;align-items:center;box-sizing:var(--css-box-sizing, border-box);height:var(--css-height, var(--size-touch-area));padding-right:var(--css-padding-right, var(--cldtr-gap-mid-1));padding-left:var(--css-padding-left, var(--cldtr-gap-mid-1));color:rgba(var(--color-effect),var(--opacity-effect));outline:none;cursor:pointer;filter:brightness(var(--filter-effect));transition:var(--l-transition-effect);user-select:none}lr-btn-ui .text{white-space:nowrap}lr-btn-ui .icon{display:flex;align-items:center;justify-content:center;color:rgba(var(--color-effect),var(--opacity-effect));filter:brightness(var(--filter-effect));transition:var(--l-transition-effect)}lr-btn-ui .icon_left{margin-right:var(--cldtr-gap-mid-1);margin-left:0}lr-btn-ui .icon_right{margin-right:0;margin-left:var(--cldtr-gap-mid-1)}lr-btn-ui .icon_single{margin-right:0;margin-left:0}lr-btn-ui .icon_hidden{display:none;margin:0}lr-btn-ui.primary{--idle-color-rgb: var(--rgb-primary-accent);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--idle-color-rgb);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.boring{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-text-base);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: 1;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.default{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-primary-accent);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-line-loader-ui{position:absolute;top:0;left:0;z-index:9999;width:100%;height:2px;opacity:.5}lr-line-loader-ui .inner{width:25%;max-width:200px;height:100%}lr-line-loader-ui .line{width:100%;height:100%;background-color:var(--color-primary-accent);transform:translate(-101%);transition:transform 1s}lr-slider-ui{--l-thumb-size: 24px;--l-zero-dot-size: 5px;--l-zero-dot-offset: 2px;--idle-color-rgb: var(--rgb-text-base);--hover-color-rgb: var(--rgb-primary-accent);--down-color-rgb: var(--rgb-primary-accent);--color-effect: var(--idle-color-rgb);--l-color: rgb(var(--color-effect));position:relative;display:flex;align-items:center;justify-content:center;width:100%;height:calc(var(--l-thumb-size) + (var(--l-zero-dot-size) + var(--l-zero-dot-offset)) * 2)}lr-slider-ui .thumb{position:absolute;left:0;width:var(--l-thumb-size);height:var(--l-thumb-size);background-color:var(--l-color);border-radius:50%;transform:translate(0);opacity:1;transition:opacity var(--transition-duration-2)}lr-slider-ui .steps{position:absolute;display:flex;align-items:center;justify-content:space-between;box-sizing:border-box;width:100%;height:100%;padding-right:calc(var(--l-thumb-size) / 2);padding-left:calc(var(--l-thumb-size) / 2)}lr-slider-ui .border-step{width:0px;height:10px;border-right:1px solid var(--l-color);opacity:.6;transition:var(--transition-duration-2)}lr-slider-ui .minor-step{width:0px;height:4px;border-right:1px solid var(--l-color);opacity:.2;transition:var(--transition-duration-2)}lr-slider-ui .zero-dot{position:absolute;top:calc(100% - var(--l-zero-dot-offset) * 2);left:calc(var(--l-thumb-size) / 2 - var(--l-zero-dot-size) / 2);width:var(--l-zero-dot-size);height:var(--l-zero-dot-size);background-color:var(--color-primary-accent);border-radius:50%;opacity:0;transition:var(--transition-duration-3)}lr-slider-ui .input{position:absolute;width:calc(100% - 10px);height:100%;margin:0;cursor:pointer;opacity:0}lr-presence-toggle.transition{transition:opacity var(--transition-duration-3),visibility var(--transition-duration-3)}lr-presence-toggle.visible{opacity:1;pointer-events:inherit}lr-presence-toggle.hidden{opacity:0;pointer-events:none}ctx-provider{--color-text-base: black;--color-primary-accent: blue;display:flex;align-items:center;justify-content:center;width:190px;height:40px;padding-right:10px;padding-left:10px;background-color:#f5f5f5;border-radius:3px}lr-cloud-image-editor-activity{position:relative;display:flex;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light)}lr-modal lr-cloud-image-editor-activity{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%)}lr-select{display:inline-flex}lr-select>button{position:relative;display:inline-flex;align-items:center;padding-right:0!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-select>button>select{position:absolute;display:block;width:100%;height:100%;opacity:0}:host{flex:1}lr-start-from{height:100%;container-type:inline-size}.lr-wgt-common,:host{--cfg-done-activity: "start-from";--cfg-init-activity: "start-from"}lr-activity-header:after{width:var(--ui-size);height:var(--ui-size);content:""}lr-activity-header .close-btn{display:none}@container (min-width: 500px){lr-start-from .content{grid-template-columns:1fr max-content;height:100%}lr-start-from lr-copyright{grid-column:2}lr-start-from lr-drop-area{grid-row:span 3}lr-start-from:has(lr-copyright[hidden]) lr-drop-area{grid-row:span 2}lr-start-from:has(.cancel-btn[hidden]) lr-drop-area{grid-row:span 2}lr-start-from:has(lr-copyright[hidden]):has(.cancel-btn[hidden]) lr-drop-area{grid-row:span 1}}
+:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-file: "m2.89453 1.2012c0-.473389.38376-.857145.85714-.857145h8.40003c.2273 0 .4453.090306.6061.251051l8.4 8.400004c.1607.16074.251.37876.251.60609v13.2c0 .4734-.3837.8571-.8571.8571h-16.80003c-.47338 0-.85714-.3837-.85714-.8571zm1.71429.85714v19.88576h15.08568v-11.4858h-7.5428c-.4734 0-.8572-.3837-.8572-.8571v-7.54286zm8.39998 1.21218 5.4736 5.47353-5.4736.00001z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-collapse: "M3.11572 12C3.11572 11.5858 3.45151 11.25 3.86572 11.25H20.1343C20.5485 11.25 20.8843 11.5858 20.8843 12C20.8843 12.4142 20.5485 12.75 20.1343 12.75H3.86572C3.45151 12.75 3.11572 12.4142 3.11572 12Z";--icon-expand: "M12.0001 8.33716L3.53033 16.8068C3.23743 17.0997 2.76256 17.0997 2.46967 16.8068C2.17678 16.5139 2.17678 16.0391 2.46967 15.7462L11.0753 7.14067C11.1943 7.01825 11.3365 6.92067 11.4936 6.8536C11.6537 6.78524 11.826 6.75 12.0001 6.75C12.1742 6.75 12.3465 6.78524 12.5066 6.8536C12.6637 6.92067 12.8059 7.01826 12.925 7.14068L21.5304 15.7462C21.8233 16.0391 21.8233 16.5139 21.5304 16.8068C21.2375 17.0997 20.7627 17.0997 20.4698 16.8068L12.0001 8.33716Z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-local: "m3 3.75c-.82843 0-1.5.67157-1.5 1.5v13.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-9.75c0-.82843-.6716-1.5-1.5-1.5h-9c-.2634 0-.5076-.13822-.6431-.36413l-2.03154-3.38587zm-3 1.5c0-1.65685 1.34315-3 3-3h6.75c.2634 0 .5076.13822.6431.36413l2.0315 3.38587h8.5754c1.6569 0 3 1.34315 3 3v9.75c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3z";--icon-url: "m19.1099 3.67026c-1.7092-1.70917-4.5776-1.68265-6.4076.14738l-2.2212 2.22122c-.2929.29289-.7678.29289-1.0607 0-.29289-.29289-.29289-.76777 0-1.06066l2.2212-2.22122c2.376-2.375966 6.1949-2.481407 8.5289-.14738l1.2202 1.22015c2.334 2.33403 2.2286 6.15294-.1474 8.52895l-2.2212 2.2212c-.2929.2929-.7678.2929-1.0607 0s-.2929-.7678 0-1.0607l2.2212-2.2212c1.8301-1.83003 1.8566-4.69842.1474-6.40759zm-3.3597 4.57991c.2929.29289.2929.76776 0 1.06066l-6.43918 6.43927c-.29289.2928-.76777.2928-1.06066 0-.29289-.2929-.29289-.7678 0-1.0607l6.43924-6.43923c.2929-.2929.7677-.2929 1.0606 0zm-9.71158 1.17048c.29289.29289.29289.76775 0 1.06065l-2.22123 2.2212c-1.83002 1.8301-1.85654 4.6984-.14737 6.4076l1.22015 1.2202c1.70917 1.7091 4.57756 1.6826 6.40763-.1474l2.2212-2.2212c.2929-.2929.7677-.2929 1.0606 0s.2929.7677 0 1.0606l-2.2212 2.2212c-2.37595 2.376-6.19486 2.4815-8.52889.1474l-1.22015-1.2201c-2.334031-2.3341-2.22859-6.153.14737-8.5289l2.22123-2.22125c.29289-.2929.76776-.2929 1.06066 0z";--icon-camera: "m7.65 2.55c.14164-.18885.36393-.3.6-.3h7.5c.2361 0 .4584.11115.6.3l2.025 2.7h2.625c1.6569 0 3 1.34315 3 3v10.5c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3v-10.5c0-1.65685 1.34315-3 3-3h2.625zm.975 1.2-2.025 2.7c-.14164.18885-.36393.3-.6.3h-3c-.82843 0-1.5.67157-1.5 1.5v10.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-10.5c0-.82843-.6716-1.5-1.5-1.5h-3c-.2361 0-.4584-.11115-.6-.3l-2.025-2.7zm3.375 6c-1.864 0-3.375 1.511-3.375 3.375s1.511 3.375 3.375 3.375 3.375-1.511 3.375-3.375-1.511-3.375-3.375-3.375zm-4.875 3.375c0-2.6924 2.18261-4.875 4.875-4.875 2.6924 0 4.875 2.1826 4.875 4.875s-2.1826 4.875-4.875 4.875c-2.69239 0-4.875-2.1826-4.875-4.875z";--icon-dots: "M16,12A2,2 0 0,1 18,10A2,2 0 0,1 20,12A2,2 0 0,1 18,14A2,2 0 0,1 16,12M10,12A2,2 0 0,1 12,10A2,2 0 0,1 14,12A2,2 0 0,1 12,14A2,2 0 0,1 10,12M4,12A2,2 0 0,1 6,10A2,2 0 0,1 8,12A2,2 0 0,1 6,14A2,2 0 0,1 4,12Z";--icon-back: "M20.251 12.0001C20.251 12.4143 19.9152 12.7501 19.501 12.7501L6.06696 12.7501L11.7872 18.6007C12.0768 18.8968 12.0715 19.3717 11.7753 19.6613C11.4791 19.9508 11.0043 19.9455 10.7147 19.6493L4.13648 12.9213C4.01578 12.8029 3.91947 12.662 3.85307 12.5065C3.78471 12.3464 3.74947 12.1741 3.74947 12C3.74947 11.8259 3.78471 11.6536 3.85307 11.4935C3.91947 11.338 4.01578 11.1971 4.13648 11.0787L10.7147 4.35068C11.0043 4.0545 11.4791 4.04916 11.7753 4.33873C12.0715 4.62831 12.0768 5.10315 11.7872 5.39932L6.06678 11.2501L19.501 11.2501C19.9152 11.2501 20.251 11.5859 20.251 12.0001Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-edit: "M3.96371 14.4792c-.15098.151-.25578.3419-.3021.5504L2.52752 20.133c-.17826.8021.53735 1.5177 1.33951 1.3395l5.10341-1.1341c.20844-.0463.39934-.1511.55032-.3021l8.05064-8.0507-5.557-5.55702-8.05069 8.05062ZM13.4286 5.01437l5.557 5.55703 2.0212-2.02111c.6576-.65765.6576-1.72393 0-2.38159l-3.1755-3.17546c-.6577-.65765-1.7239-.65765-2.3816 0l-2.0211 2.02113Z";--icon-detail: "M5,3C3.89,3 3,3.89 3,5V19C3,20.11 3.89,21 5,21H19C20.11,21 21,20.11 21,19V5C21,3.89 20.11,3 19,3H5M5,5H19V19H5V5M7,7V9H17V7H7M7,11V13H17V11H7M7,15V17H14V15H7Z";--icon-select: "M7,10L12,15L17,10H7Z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-fullscreen: "M5,5H10V7H7V10H5V5M14,5H19V10H17V7H14V5M17,14H19V19H14V17H17V14M10,17V19H5V14H7V17H10Z";--icon-fullscreen-exit: "M14,14H19V16H16V19H14V14M5,14H10V19H8V16H5V14M8,5H10V10H5V8H8V5M19,8V10H14V5H16V8H19Z";--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-about: "M11.152 14.12v.1h1.523v-.1c.007-.409.053-.752.138-1.028.086-.277.22-.517.405-.72.188-.202.434-.397.735-.586.32-.191.593-.412.82-.66.232-.249.41-.531.533-.847.125-.32.187-.678.187-1.076 0-.579-.137-1.085-.41-1.518a2.717 2.717 0 0 0-1.14-1.018c-.49-.245-1.062-.367-1.715-.367-.597 0-1.142.114-1.636.34-.49.228-.884.564-1.182 1.008-.299.44-.46.98-.485 1.619h1.62c.024-.377.118-.684.282-.922.163-.241.369-.419.617-.532.25-.114.51-.17.784-.17.301 0 .575.063.82.191.248.124.447.302.597.533.149.23.223.504.223.82 0 .263-.05.502-.149.72-.1.216-.234.408-.405.574a3.48 3.48 0 0 1-.575.453c-.33.199-.613.42-.847.66-.234.242-.415.558-.543.949-.125.39-.19.916-.197 1.577ZM11.205 17.15c.21.206.46.31.75.31.196 0 .374-.049.534-.144.16-.096.287-.224.383-.384.1-.163.15-.343.15-.538a1 1 0 0 0-.32-.746 1.019 1.019 0 0 0-.746-.314c-.291 0-.542.105-.751.314-.21.206-.314.455-.314.746 0 .295.104.547.314.756ZM24 12c0 6.627-5.373 12-12 12S0 18.627 0 12 5.373 0 12 0s12 5.373 12 12Zm-1.5 0c0 5.799-4.701 10.5-10.5 10.5S1.5 17.799 1.5 12 6.201 1.5 12 1.5 22.5 6.201 22.5 12Z";--icon-edit-rotate: "M16.89,15.5L18.31,16.89C19.21,15.73 19.76,14.39 19.93,13H17.91C17.77,13.87 17.43,14.72 16.89,15.5M13,17.9V19.92C14.39,19.75 15.74,19.21 16.9,18.31L15.46,16.87C14.71,17.41 13.87,17.76 13,17.9M19.93,11C19.76,9.61 19.21,8.27 18.31,7.11L16.89,8.53C17.43,9.28 17.77,10.13 17.91,11M15.55,5.55L11,1V4.07C7.06,4.56 4,7.92 4,12C4,16.08 7.05,19.44 11,19.93V17.91C8.16,17.43 6,14.97 6,12C6,9.03 8.16,6.57 11,6.09V10L15.55,5.55Z";--icon-edit-flip-v: "M3 15V17H5V15M15 19V21H17V19M19 3H5C3.9 3 3 3.9 3 5V9H5V5H19V9H21V5C21 3.9 20.1 3 19 3M21 19H19V21C20.1 21 21 20.1 21 19M1 11V13H23V11M7 19V21H9V19M19 15V17H21V15M11 19V21H13V19M3 19C3 20.1 3.9 21 5 21V19Z";--icon-edit-flip-h: "M15 21H17V19H15M19 9H21V7H19M3 5V19C3 20.1 3.9 21 5 21H9V19H5V5H9V3H5C3.9 3 3 3.9 3 5M19 3V5H21C21 3.9 20.1 3 19 3M11 23H13V1H11M19 17H21V15H19M15 5H17V3H15M19 13H21V11H19M19 21C20.1 21 21 20.1 21 19H19Z";--icon-edit-brightness: "M12,18A6,6 0 0,1 6,12A6,6 0 0,1 12,6A6,6 0 0,1 18,12A6,6 0 0,1 12,18M20,15.31L23.31,12L20,8.69V4H15.31L12,0.69L8.69,4H4V8.69L0.69,12L4,15.31V20H8.69L12,23.31L15.31,20H20V15.31Z";--icon-edit-contrast: "M12,20C9.79,20 7.79,19.1 6.34,17.66L17.66,6.34C19.1,7.79 20,9.79 20,12A8,8 0 0,1 12,20M6,8H8V6H9.5V8H11.5V9.5H9.5V11.5H8V9.5H6M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,16H17V14.5H12V16Z";--icon-edit-saturation: "M3,13A9,9 0 0,0 12,22C12,17 7.97,13 3,13M12,5.5A2.5,2.5 0 0,1 14.5,8A2.5,2.5 0 0,1 12,10.5A2.5,2.5 0 0,1 9.5,8A2.5,2.5 0 0,1 12,5.5M5.6,10.25A2.5,2.5 0 0,0 8.1,12.75C8.63,12.75 9.12,12.58 9.5,12.31C9.5,12.37 9.5,12.43 9.5,12.5A2.5,2.5 0 0,0 12,15A2.5,2.5 0 0,0 14.5,12.5C14.5,12.43 14.5,12.37 14.5,12.31C14.88,12.58 15.37,12.75 15.9,12.75C17.28,12.75 18.4,11.63 18.4,10.25C18.4,9.25 17.81,8.4 16.97,8C17.81,7.6 18.4,6.74 18.4,5.75C18.4,4.37 17.28,3.25 15.9,3.25C15.37,3.25 14.88,3.41 14.5,3.69C14.5,3.63 14.5,3.56 14.5,3.5A2.5,2.5 0 0,0 12,1A2.5,2.5 0 0,0 9.5,3.5C9.5,3.56 9.5,3.63 9.5,3.69C9.12,3.41 8.63,3.25 8.1,3.25A2.5,2.5 0 0,0 5.6,5.75C5.6,6.74 6.19,7.6 7.03,8C6.19,8.4 5.6,9.25 5.6,10.25M12,22A9,9 0 0,0 21,13C16,13 12,17 12,22Z";--icon-edit-crop: "M7,17V1H5V5H1V7H5V17A2,2 0 0,0 7,19H17V23H19V19H23V17M17,15H19V7C19,5.89 18.1,5 17,5H9V7H17V15Z";--icon-edit-text: "M18.5,4L19.66,8.35L18.7,8.61C18.25,7.74 17.79,6.87 17.26,6.43C16.73,6 16.11,6 15.5,6H13V16.5C13,17 13,17.5 13.33,17.75C13.67,18 14.33,18 15,18V19H9V18C9.67,18 10.33,18 10.67,17.75C11,17.5 11,17 11,16.5V6H8.5C7.89,6 7.27,6 6.74,6.43C6.21,6.87 5.75,7.74 5.3,8.61L4.34,8.35L5.5,4H18.5Z";--icon-edit-draw: "m21.879394 2.1631238c-1.568367-1.62768627-4.136546-1.53831744-5.596267.1947479l-8.5642801 10.1674753c-1.4906533-.224626-3.061232.258204-4.2082427 1.448604-1.0665468 1.106968-1.0997707 2.464806-1.1203996 3.308068-.00142.05753-.00277.113001-.00439.16549-.02754.894146-.08585 1.463274-.5821351 2.069648l-.80575206.98457.88010766.913285c1.0539516 1.093903 2.6691689 1.587048 4.1744915 1.587048 1.5279113 0 3.2235468-.50598 4.4466094-1.775229 1.147079-1.190514 1.612375-2.820653 1.395772-4.367818l9.796763-8.8879697c1.669907-1.5149954 1.75609-4.1802333.187723-5.8079195zm-16.4593821 13.7924592c.8752943-.908358 2.2944227-.908358 3.1697054 0 .8752942.908358.8752942 2.381259 0 3.289617-.5909138.61325-1.5255389.954428-2.53719.954428-.5223687 0-.9935663-.09031-1.3832112-.232762.3631253-.915463.3952949-1.77626.4154309-2.429737.032192-1.045425.072224-1.308557.3352649-1.581546z";--icon-edit-guides: "M1.39,18.36L3.16,16.6L4.58,18L5.64,16.95L4.22,15.54L5.64,14.12L8.11,16.6L9.17,15.54L6.7,13.06L8.11,11.65L9.53,13.06L10.59,12L9.17,10.59L10.59,9.17L13.06,11.65L14.12,10.59L11.65,8.11L13.06,6.7L14.47,8.11L15.54,7.05L14.12,5.64L15.54,4.22L18,6.7L19.07,5.64L16.6,3.16L18.36,1.39L22.61,5.64L5.64,22.61L1.39,18.36Z";--icon-edit-color: "M17.5,12A1.5,1.5 0 0,1 16,10.5A1.5,1.5 0 0,1 17.5,9A1.5,1.5 0 0,1 19,10.5A1.5,1.5 0 0,1 17.5,12M14.5,8A1.5,1.5 0 0,1 13,6.5A1.5,1.5 0 0,1 14.5,5A1.5,1.5 0 0,1 16,6.5A1.5,1.5 0 0,1 14.5,8M9.5,8A1.5,1.5 0 0,1 8,6.5A1.5,1.5 0 0,1 9.5,5A1.5,1.5 0 0,1 11,6.5A1.5,1.5 0 0,1 9.5,8M6.5,12A1.5,1.5 0 0,1 5,10.5A1.5,1.5 0 0,1 6.5,9A1.5,1.5 0 0,1 8,10.5A1.5,1.5 0 0,1 6.5,12M12,3A9,9 0 0,0 3,12A9,9 0 0,0 12,21A1.5,1.5 0 0,0 13.5,19.5C13.5,19.11 13.35,18.76 13.11,18.5C12.88,18.23 12.73,17.88 12.73,17.5A1.5,1.5 0 0,1 14.23,16H16A5,5 0 0,0 21,11C21,6.58 16.97,3 12,3Z";--icon-edit-resize: "M10.59,12L14.59,8H11V6H18V13H16V9.41L12,13.41V16H20V4H8V12H10.59M22,2V18H12V22H2V12H6V2H22M10,14H4V20H10V14Z";--icon-external-source-placeholder: "M6.341 3.27a10.5 10.5 0 0 1 5.834-1.77.75.75 0 0 0 0-1.5 12 12 0 1 0 12 12 .75.75 0 0 0-1.5 0A10.5 10.5 0 1 1 6.34 3.27Zm14.145 1.48a.75.75 0 1 0-1.06-1.062L9.925 13.19V7.95a.75.75 0 1 0-1.5 0V15c0 .414.336.75.75.75h7.05a.75.75 0 0 0 0-1.5h-5.24l9.501-9.5Z";--icon-facebook: "m12 1.5c-5.79901 0-10.5 4.70099-10.5 10.5 0 4.9427 3.41586 9.0888 8.01562 10.2045v-6.1086h-2.13281c-.41421 0-.75-.3358-.75-.75v-3.2812c0-.4142.33579-.75.75-.75h2.13281v-1.92189c0-.95748.22571-2.51089 1.38068-3.6497 1.1934-1.17674 3.1742-1.71859 6.2536-1.05619.3455.07433.5923.3798.5923.73323v2.75395c0 .41422-.3358.75-.75.75-.6917 0-1.2029.02567-1.5844.0819-.3865.05694-.5781.13711-.675.20223-.1087.07303-.2367.20457-.2367 1.02837v1.0781h2.3906c.2193 0 .4275.0959.57.2626.1425.1666.205.3872.1709.6038l-.5156 3.2813c-.0573.3647-.3716.6335-.7409.6335h-1.875v6.1058c4.5939-1.1198 8.0039-5.2631 8.0039-10.2017 0-5.79901-4.701-10.5-10.5-10.5zm-12 10.5c0-6.62744 5.37256-12 12-12 6.6274 0 12 5.37256 12 12 0 5.9946-4.3948 10.9614-10.1384 11.8564-.2165.0337-.4369-.0289-.6033-.1714s-.2622-.3506-.2622-.5697v-7.7694c0-.4142.3358-.75.75-.75h1.9836l.28-1.7812h-2.2636c-.4142 0-.75-.3358-.75-.75v-1.8281c0-.82854.0888-1.72825.9-2.27338.3631-.24396.8072-.36961 1.293-.4412.3081-.0454.6583-.07238 1.0531-.08618v-1.39629c-2.4096-.40504-3.6447.13262-4.2928.77165-.7376.72735-.9338 1.79299-.9338 2.58161v2.67189c0 .4142-.3358.75-.75.75h-2.13279v1.7812h2.13279c.4142 0 .75.3358.75.75v7.7712c0 .219-.0956.427-.2619.5695-.1662.1424-.3864.2052-.6028.1717-5.74968-.8898-10.1509-5.8593-10.1509-11.8583z";--icon-dropbox: "m6.01895 1.92072c.24583-.15659.56012-.15658.80593.00003l5.17512 3.29711 5.1761-3.29714c.2458-.15659.5601-.15658.8059.00003l5.5772 3.55326c.2162.13771.347.37625.347.63253 0 .25629-.1308.49483-.347.63254l-4.574 2.91414 4.574 2.91418c.2162.1377.347.3762.347.6325s-.1308.4948-.347.6325l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.1761-3.2971-5.17512 3.2971c-.24581.1566-.5601.1566-.80593 0l-5.578142-3.5532c-.216172-.1377-.347058-.3763-.347058-.6326s.130886-.4949.347058-.6326l4.574772-2.91408-4.574772-2.91411c-.216172-.1377-.347058-.37626-.347058-.63257 0-.2563.130886-.49486.347058-.63256zm.40291 8.61518-4.18213 2.664 4.18213 2.664 4.18144-2.664zm6.97504 2.664 4.1821 2.664 4.1814-2.664-4.1814-2.664zm2.7758-3.54668-4.1727 2.65798-4.17196-2.65798 4.17196-2.658zm1.4063-.88268 4.1814-2.664-4.1814-2.664-4.1821 2.664zm-6.9757-2.664-4.18144-2.664-4.18213 2.664 4.18213 2.664zm-4.81262 12.43736c.22254-.3494.68615-.4522 1.03551-.2297l5.17521 3.2966 5.1742-3.2965c.3493-.2226.813-.1198 1.0355.2295.2226.3494.1198.813-.2295 1.0355l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.57819-3.5532c-.34936-.2226-.45216-.6862-.22963-1.0355z";--icon-gdrive: "m7.73633 1.81806c.13459-.22968.38086-.37079.64707-.37079h7.587c.2718 0 .5223.14697.6548.38419l7.2327 12.94554c.1281.2293.1269.5089-.0031.7371l-3.7935 6.6594c-.1334.2342-.3822.3788-.6517.3788l-14.81918.0004c-.26952 0-.51831-.1446-.65171-.3788l-3.793526-6.6598c-.1327095-.233-.130949-.5191.004617-.7504zm.63943 1.87562-6.71271 11.45452 2.93022 5.1443 6.65493-11.58056zm3.73574 6.52652-2.39793 4.1727 4.78633.0001zm4.1168 4.1729 5.6967-.0002-6.3946-11.44563h-5.85354zm5.6844 1.4998h-13.06111l-2.96515 5.1598 13.08726-.0004z";--icon-gphotos: "M12.51 0c-.702 0-1.272.57-1.272 1.273V7.35A6.381 6.381 0 0 0 0 11.489c0 .703.57 1.273 1.273 1.273H7.35A6.381 6.381 0 0 0 11.488 24c.704 0 1.274-.57 1.274-1.273V16.65A6.381 6.381 0 0 0 24 12.51c0-.703-.57-1.273-1.273-1.273H16.65A6.381 6.381 0 0 0 12.511 0Zm.252 11.232V1.53a4.857 4.857 0 0 1 0 9.702Zm-1.53.006H1.53a4.857 4.857 0 0 1 9.702 0Zm1.536 1.524a4.857 4.857 0 0 0 9.702 0h-9.702Zm-6.136 4.857c0-2.598 2.04-4.72 4.606-4.85v9.7a4.857 4.857 0 0 1-4.606-4.85Z";--icon-instagram: "M6.225 12a5.775 5.775 0 1 1 11.55 0 5.775 5.775 0 0 1-11.55 0zM12 7.725a4.275 4.275 0 1 0 0 8.55 4.275 4.275 0 0 0 0-8.55zM18.425 6.975a1.4 1.4 0 1 0 0-2.8 1.4 1.4 0 0 0 0 2.8zM11.958.175h.084c2.152 0 3.823 0 5.152.132 1.35.134 2.427.41 3.362 1.013a7.15 7.15 0 0 1 2.124 2.124c.604.935.88 2.012 1.013 3.362.132 1.329.132 3 .132 5.152v.084c0 2.152 0 3.823-.132 5.152-.134 1.35-.41 2.427-1.013 3.362a7.15 7.15 0 0 1-2.124 2.124c-.935.604-2.012.88-3.362 1.013-1.329.132-3 .132-5.152.132h-.084c-2.152 0-3.824 0-5.153-.132-1.35-.134-2.427-.409-3.36-1.013a7.15 7.15 0 0 1-2.125-2.124C.716 19.62.44 18.544.307 17.194c-.132-1.329-.132-3-.132-5.152v-.084c0-2.152 0-3.823.132-5.152.133-1.35.409-2.427 1.013-3.362A7.15 7.15 0 0 1 3.444 1.32C4.378.716 5.456.44 6.805.307c1.33-.132 3-.132 5.153-.132zM6.953 1.799c-1.234.123-2.043.36-2.695.78A5.65 5.65 0 0 0 2.58 4.26c-.42.65-.657 1.46-.78 2.695C1.676 8.2 1.675 9.797 1.675 12c0 2.203 0 3.8.124 5.046.123 1.235.36 2.044.78 2.696a5.649 5.649 0 0 0 1.68 1.678c.65.421 1.46.658 2.694.78 1.247.124 2.844.125 5.047.125s3.8 0 5.046-.124c1.235-.123 2.044-.36 2.695-.78a5.648 5.648 0 0 0 1.68-1.68c.42-.65.657-1.46.78-2.694.123-1.247.124-2.844.124-5.047s-.001-3.8-.125-5.046c-.122-1.235-.359-2.044-.78-2.695a5.65 5.65 0 0 0-1.679-1.68c-.651-.42-1.46-.657-2.695-.78-1.246-.123-2.843-.124-5.046-.124-2.203 0-3.8 0-5.047.124z";--icon-flickr: "M5.95874 7.92578C3.66131 7.92578 1.81885 9.76006 1.81885 11.9994C1.81885 14.2402 3.66145 16.0744 5.95874 16.0744C8.26061 16.0744 10.1039 14.2396 10.1039 11.9994C10.1039 9.76071 8.26074 7.92578 5.95874 7.92578ZM0.318848 11.9994C0.318848 8.91296 2.85168 6.42578 5.95874 6.42578C9.06906 6.42578 11.6039 8.91232 11.6039 11.9994C11.6039 15.0877 9.06919 17.5744 5.95874 17.5744C2.85155 17.5744 0.318848 15.0871 0.318848 11.9994ZM18.3898 7.92578C16.0878 7.92578 14.2447 9.76071 14.2447 11.9994C14.2447 14.2396 16.088 16.0744 18.3898 16.0744C20.6886 16.0744 22.531 14.2401 22.531 11.9994C22.531 9.76019 20.6887 7.92578 18.3898 7.92578ZM12.7447 11.9994C12.7447 8.91232 15.2795 6.42578 18.3898 6.42578C21.4981 6.42578 24.031 8.91283 24.031 11.9994C24.031 15.0872 21.4982 17.5744 18.3898 17.5744C15.2794 17.5744 12.7447 15.0877 12.7447 11.9994Z";--icon-vk: var(--icon-external-source-placeholder);--icon-evernote: "M9.804 2.27v-.048c.055-.263.313-.562.85-.562h.44c.142 0 .325.014.526.033.066.009.124.023.267.06l.13.032h.002c.319.079.515.275.644.482a1.461 1.461 0 0 1 .16.356l.004.012a.75.75 0 0 0 .603.577l1.191.207a1988.512 1988.512 0 0 0 2.332.402c.512.083 1.1.178 1.665.442.64.3 1.19.795 1.376 1.77.548 2.931.657 5.829.621 8a39.233 39.233 0 0 1-.125 2.602 17.518 17.518 0 0 1-.092.849.735.735 0 0 0-.024.112c-.378 2.705-1.269 3.796-2.04 4.27-.746.457-1.53.451-2.217.447h-.192c-.46 0-1.073-.23-1.581-.635-.518-.412-.763-.87-.763-1.217 0-.45.188-.688.355-.786.161-.095.436-.137.796.087a.75.75 0 1 0 .792-1.274c-.766-.476-1.64-.52-2.345-.108-.7.409-1.098 1.188-1.098 2.08 0 .996.634 1.84 1.329 2.392.704.56 1.638.96 2.515.96l.185.002c.667.009 1.874.025 3.007-.67 1.283-.786 2.314-2.358 2.733-5.276.01-.039.018-.078.022-.105.011-.061.023-.14.034-.23.023-.184.051-.445.079-.772.055-.655.111-1.585.13-2.704.037-2.234-.074-5.239-.647-8.301v-.002c-.294-1.544-1.233-2.391-2.215-2.85-.777-.363-1.623-.496-2.129-.576-.097-.015-.18-.028-.25-.041l-.006-.001-1.99-.345-.761-.132a2.93 2.93 0 0 0-.182-.338A2.532 2.532 0 0 0 12.379.329l-.091-.023a3.967 3.967 0 0 0-.493-.103L11.769.2a7.846 7.846 0 0 0-.675-.04h-.44c-.733 0-1.368.284-1.795.742L2.416 7.431c-.468.428-.751 1.071-.751 1.81 0 .02 0 .041.003.062l.003.034c.017.21.038.468.096.796.107.715.275 1.47.391 1.994.029.13.055.245.075.342l.002.008c.258 1.141.641 1.94.978 2.466.168.263.323.456.444.589a2.808 2.808 0 0 0 .192.194c1.536 1.562 3.713 2.196 5.731 2.08.13-.005.35-.032.537-.073a2.627 2.627 0 0 0 .652-.24c.425-.26.75-.661.992-1.046.184-.294.342-.61.473-.915.197.193.412.357.627.493a5.022 5.022 0 0 0 1.97.709l.023.002.018.003.11.016c.088.014.205.035.325.058l.056.014c.088.022.164.04.235.061a1.736 1.736 0 0 1 .145.048l.03.014c.765.34 1.302 1.09 1.302 1.871a.75.75 0 0 0 1.5 0c0-1.456-.964-2.69-2.18-3.235-.212-.103-.5-.174-.679-.217l-.063-.015a10.616 10.616 0 0 0-.606-.105l-.02-.003-.03-.003h-.002a3.542 3.542 0 0 1-1.331-.485c-.471-.298-.788-.692-.828-1.234a.75.75 0 0 0-1.48-.106l-.001.003-.004.017a8.23 8.23 0 0 1-.092.352 9.963 9.963 0 0 1-.298.892c-.132.34-.29.68-.47.966-.174.276-.339.454-.478.549a1.178 1.178 0 0 1-.221.072 1.949 1.949 0 0 1-.241.036h-.013l-.032.002c-1.684.1-3.423-.437-4.604-1.65a.746.746 0 0 0-.053-.05L4.84 14.6a1.348 1.348 0 0 1-.07-.073 2.99 2.99 0 0 1-.293-.392c-.242-.379-.558-1.014-.778-1.985a54.1 54.1 0 0 0-.083-.376 27.494 27.494 0 0 1-.367-1.872l-.003-.02a6.791 6.791 0 0 1-.08-.67c.004-.277.086-.475.2-.609l.067-.067a.63.63 0 0 1 .292-.145h.05c.18 0 1.095.055 2.013.115l1.207.08.534.037a.747.747 0 0 0 .052.002c.782 0 1.349-.206 1.759-.585l.005-.005c.553-.52.622-1.225.622-1.76V6.24l-.026-.565A774.97 774.97 0 0 1 9.885 4.4c-.042-.961-.081-1.939-.081-2.13ZM4.995 6.953a251.126 251.126 0 0 1 2.102.137l.508.035c.48-.004.646-.122.715-.185.07-.068.146-.209.147-.649l-.024-.548a791.69 791.69 0 0 1-.095-2.187L4.995 6.953Zm16.122 9.996ZM15.638 11.626a.75.75 0 0 0 1.014.31 2.04 2.04 0 0 1 .304-.089 1.84 1.84 0 0 1 .544-.039c.215.023.321.06.37.085.033.016.039.026.047.04a.75.75 0 0 0 1.289-.767c-.337-.567-.906-.783-1.552-.85a3.334 3.334 0 0 0-1.002.062c-.27.056-.531.14-.705.234a.75.75 0 0 0-.31 1.014Z";--icon-box: "M1.01 4.148a.75.75 0 0 1 .75.75v4.348a4.437 4.437 0 0 1 2.988-1.153c1.734 0 3.23.992 3.978 2.438a4.478 4.478 0 0 1 3.978-2.438c2.49 0 4.488 2.044 4.488 4.543 0 2.5-1.999 4.544-4.488 4.544a4.478 4.478 0 0 1-3.978-2.438 4.478 4.478 0 0 1-3.978 2.438C2.26 17.18.26 15.135.26 12.636V4.898a.75.75 0 0 1 .75-.75Zm.75 8.488c0 1.692 1.348 3.044 2.988 3.044s2.989-1.352 2.989-3.044c0-1.691-1.349-3.043-2.989-3.043S1.76 10.945 1.76 12.636Zm10.944-3.043c-1.64 0-2.988 1.352-2.988 3.043 0 1.692 1.348 3.044 2.988 3.044s2.988-1.352 2.988-3.044c0-1.69-1.348-3.043-2.988-3.043Zm4.328-1.23a.75.75 0 0 1 1.052.128l2.333 2.983 2.333-2.983a.75.75 0 0 1 1.181.924l-2.562 3.277 2.562 3.276a.75.75 0 1 1-1.181.924l-2.333-2.983-2.333 2.983a.75.75 0 1 1-1.181-.924l2.562-3.276-2.562-3.277a.75.75 0 0 1 .129-1.052Z";--icon-onedrive: "M13.616 4.147a7.689 7.689 0 0 0-7.642 3.285A6.299 6.299 0 0 0 1.455 17.3c.684.894 2.473 2.658 5.17 2.658h12.141c.95 0 1.882-.256 2.697-.743.815-.486 1.514-1.247 1.964-2.083a5.26 5.26 0 0 0-3.713-7.612 7.69 7.69 0 0 0-6.098-5.373ZM3.34 17.15c.674.63 1.761 1.308 3.284 1.308h12.142a3.76 3.76 0 0 0 2.915-1.383l-7.494-4.489L3.34 17.15Zm10.875-6.25 2.47-1.038a5.239 5.239 0 0 1 1.427-.389 6.19 6.19 0 0 0-10.3-1.952 6.338 6.338 0 0 1 2.118.813l4.285 2.567Zm4.55.033c-.512 0-1.019.104-1.489.307l-.006.003-1.414.594 6.521 3.906a3.76 3.76 0 0 0-3.357-4.8l-.254-.01ZM4.097 9.617A4.799 4.799 0 0 1 6.558 8.9c.9 0 1.84.25 2.587.713l3.4 2.037-10.17 4.28a4.799 4.799 0 0 1 1.721-6.312Z";--icon-huddle: "M6.204 2.002c-.252.23-.357.486-.357.67V21.07c0 .15.084.505.313.812.208.28.499.477.929.477.519 0 .796-.174.956-.365.178-.212.286-.535.286-.924v-.013l.117-6.58c.004-1.725 1.419-3.883 3.867-3.883 1.33 0 2.332.581 2.987 1.364.637.762.95 1.717.95 2.526v6.47c0 .392.11.751.305.995.175.22.468.41 1.008.41.52 0 .816-.198 1.002-.437.207-.266.31-.633.31-.969V14.04c0-2.81-1.943-5.108-4.136-5.422a5.971 5.971 0 0 0-3.183.41c-.912.393-1.538.96-1.81 1.489a.75.75 0 0 1-1.417-.344v-7.5c0-.587-.47-1.031-1.242-1.031-.315 0-.638.136-.885.36ZM5.194.892A2.844 2.844 0 0 1 7.09.142c1.328 0 2.742.867 2.742 2.53v5.607a6.358 6.358 0 0 1 1.133-.629 7.47 7.47 0 0 1 3.989-.516c3.056.436 5.425 3.482 5.425 6.906v6.914c0 .602-.177 1.313-.627 1.89-.47.605-1.204 1.016-2.186 1.016-.96 0-1.698-.37-2.179-.973-.46-.575-.633-1.294-.633-1.933v-6.469c0-.456-.19-1.071-.602-1.563-.394-.471-.986-.827-1.836-.827-1.447 0-2.367 1.304-2.367 2.39v.014l-.117 6.58c-.001.64-.177 1.333-.637 1.881-.48.57-1.2.9-2.105.9-.995 0-1.7-.5-2.132-1.081-.41-.552-.61-1.217-.61-1.708V2.672c0-.707.366-1.341.847-1.78Z"}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-tabs{display:grid;grid-template-rows:min-content minmax(var(--ui-size),auto);height:100%;overflow:hidden;color:var(--clr-txt-lightest)}lr-tabs>.tabs-row{display:flex;grid-template-columns:minmax();background-color:var(--clr-background-light)}lr-tabs>.tabs-context{overflow-y:auto}lr-tabs .tabs-row>.tab{display:flex;flex-grow:1;align-items:center;justify-content:center;height:var(--ui-size);border-bottom:var(--border-light);cursor:pointer;transition:var(--transition-duration)}lr-tabs .tabs-row>.tab[current]{color:var(--clr-txt);border-color:var(--clr-txt)}lr-range{position:relative;display:inline-flex;align-items:center;justify-content:center;height:var(--ui-size)}lr-range datalist{display:none}lr-range input{width:100%;height:100%;opacity:0}lr-range .track-wrapper{position:absolute;right:10px;left:10px;display:flex;align-items:center;justify-content:center;height:2px;user-select:none;pointer-events:none}lr-range .track{position:absolute;right:0;left:0;display:flex;align-items:center;justify-content:center;height:2px;background-color:currentColor;border-radius:2px;opacity:.5}lr-range .slider{position:absolute;width:16px;height:16px;background-color:currentColor;border-radius:100%;transform:translate(-50%)}lr-range .bar{position:absolute;left:0;height:100%;background-color:currentColor;border-radius:2px}lr-range .caption{position:absolute;display:inline-flex;justify-content:center}lr-color{position:relative;display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size);overflow:hidden;background-color:var(--clr-background);cursor:pointer}lr-color[current]{background-color:var(--clr-txt)}lr-color input[type=color]{position:absolute;display:block;width:100%;height:100%;opacity:0}lr-color .current-color{position:absolute;width:50%;height:50%;border:2px solid #fff;border-radius:100%;pointer-events:none}lr-config{display:none}lr-simple-btn{position:relative;display:inline-flex}lr-simple-btn button{padding-left:.2em!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-simple-btn button lr-icon svg{transform:scale(.8)}lr-simple-btn button:hover{background-color:var(--clr-btn-bgr-secondary-hover)}lr-simple-btn button:active{background-color:var(--clr-btn-bgr-secondary-active)}lr-simple-btn>lr-drop-area{display:contents}lr-simple-btn .visual-drop-area{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;padding:var(--gap-min);border:var(--border-dashed);border-radius:inherit;opacity:0;transition:border-color var(--transition-duration) ease,background-color var(--transition-duration) ease,opacity var(--transition-duration) ease}lr-simple-btn .visual-drop-area:before{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;color:var(--clr-txt-light);background-color:var(--clr-background);border-radius:inherit;content:var(--l10n-drop-files-here)}lr-simple-btn>lr-drop-area[drag-state=active] .visual-drop-area{background-color:var(--clr-accent-lightest);opacity:1}lr-simple-btn>lr-drop-area[drag-state=inactive] .visual-drop-area{background-color:var(--clr-shade-lv1);opacity:0}lr-simple-btn>lr-drop-area[drag-state=near] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent-light);opacity:1}lr-simple-btn>lr-drop-area[drag-state=over] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent);opacity:1}lr-simple-btn>:where(lr-drop-area[drag-state=active],lr-drop-area[drag-state=near],lr-drop-area[drag-state=over]) button{box-shadow:none}lr-simple-btn>lr-drop-area:after{content:""}lr-source-btn{display:flex;align-items:center;margin-bottom:var(--gap-min);padding:var(--gap-min) var(--gap-mid);color:var(--clr-txt-mid);border-radius:var(--border-radius-element);cursor:pointer;transition-duration:var(--transition-duration);transition-property:background-color,color;user-select:none}lr-source-btn:hover{color:var(--clr-accent);background-color:var(--clr-accent-lightest)}lr-source-btn:active{color:var(--clr-accent);background-color:var(--clr-accent-light)}lr-source-btn lr-icon{display:inline-flex;flex-grow:1;justify-content:center;min-width:var(--ui-size);margin-right:var(--gap-mid);opacity:.8}lr-source-btn[type=local]>.txt:after{content:var(--l10n-local-files)}lr-source-btn[type=camera]>.txt:after{content:var(--l10n-camera)}lr-source-btn[type=url]>.txt:after{content:var(--l10n-from-url)}lr-source-btn[type=other]>.txt:after{content:var(--l10n-other)}lr-source-btn .txt{display:flex;align-items:center;box-sizing:border-box;width:100%;height:var(--ui-size);padding:0;white-space:nowrap;border:none}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-modal{--modal-max-content-height: calc(var(--uploadcare-blocks-window-height, 100vh) - 4 * var(--gap-mid) - var(--ui-size));--modal-content-height-fill: var(--uploadcare-blocks-window-height, 100vh)}lr-modal[dialog-fallback]{--lr-z-max: 2147483647;position:fixed;z-index:var(--lr-z-max);display:flex;align-items:center;justify-content:center;width:100vw;height:100vh;pointer-events:none;inset:0}lr-modal[dialog-fallback] dialog[open]{z-index:var(--lr-z-max);pointer-events:auto}lr-modal[dialog-fallback] dialog[open]+.backdrop{position:fixed;top:0;left:0;z-index:calc(var(--lr-z-max) - 1);align-items:center;justify-content:center;width:100vw;height:100vh;background-color:var(--clr-curtain);pointer-events:auto}lr-modal[strokes][dialog-fallback] dialog[open]+.backdrop{background-image:var(--modal-backdrop-background-image)}@supports selector(dialog::backdrop){lr-modal>dialog::backdrop{background-color:#0000001a}lr-modal[strokes]>dialog::backdrop{background-image:var(--modal-backdrop-background-image)}}lr-modal>dialog[open]{transform:translateY(0);visibility:visible;opacity:1}lr-modal>dialog:not([open]){transform:translateY(20px);visibility:hidden;opacity:0}lr-modal>dialog{display:flex;flex-direction:column;width:max-content;max-width:min(calc(100% - var(--gap-mid) * 2),calc(var(--modal-max-w) - var(--gap-mid) * 2));min-height:var(--ui-size);max-height:calc(var(--modal-max-h) - var(--gap-mid) * 2);margin:auto;padding:0;overflow:hidden;background-color:var(--clr-background-light);border:0;border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:transform calc(var(--transition-duration) * 2)}@media only screen and (max-width: 430px),only screen and (max-height: 600px){lr-modal>dialog>.content{height:var(--modal-max-content-height)}}lr-url-source{display:block;background-color:var(--clr-background-light)}lr-modal lr-url-source{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-url-source>.content{display:grid;grid-gap:var(--gap-small);grid-template-columns:1fr min-content;padding:var(--gap-mid);padding-top:0}lr-url-source .url-input{display:flex}lr-url-source .url-upload-btn:after{content:var(--l10n-upload-url)}lr-camera-source{position:relative;display:flex;flex-direction:column;width:100%;height:100%;max-height:100%;overflow:hidden;background-color:var(--clr-background-light);border-radius:var(--border-radius-element)}lr-modal lr-camera-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:100vh;max-height:var(--modal-max-content-height)}lr-camera-source.initialized{height:max-content}@media only screen and (max-width: 430px){lr-camera-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-camera-source video{display:block;width:100%;max-height:100%;object-fit:contain;object-position:center center;background-color:var(--clr-background-dark);border-radius:var(--border-radius-element)}lr-camera-source .toolbar{position:absolute;bottom:0;display:flex;justify-content:space-between;width:100%;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-camera-source .content{display:flex;flex:1;justify-content:center;width:100%;padding:var(--gap-mid);padding-top:0;overflow:hidden}lr-camera-source .message-box{--padding: calc(var(--gap-max) * 2);display:flex;flex-direction:column;grid-gap:var(--gap-max);align-items:center;justify-content:center;padding:var(--padding) var(--padding) 0 var(--padding);color:var(--clr-txt)}lr-camera-source .message-box button{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary)}lr-camera-source .shot-btn{position:absolute;bottom:var(--gap-max);width:calc(var(--ui-size) * 1.8);height:calc(var(--ui-size) * 1.8);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;opacity:.85;transition:var(--transition-duration) ease}lr-camera-source .shot-btn:hover{transform:scale(1.05);opacity:1}lr-camera-source .shot-btn:active{background-color:var(--clr-txt-mid);opacity:1}lr-camera-source .shot-btn[disabled]{bottom:calc(var(--gap-max) * -1 - var(--gap-mid) - var(--ui-size) * 2)}lr-camera-source .shot-btn lr-icon svg{width:calc(var(--ui-size) / 1.5);height:calc(var(--ui-size) / 1.5)}lr-external-source{display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--clr-background-light);overflow:hidden}lr-modal lr-external-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height)}lr-external-source>.content{position:relative;display:grid;flex:1;grid-template-rows:1fr min-content}@media only screen and (max-width: 430px){lr-external-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-external-source iframe{display:block;width:100%;height:100%;border:none}lr-external-source .iframe-wrapper{overflow:hidden}lr-external-source .toolbar{display:grid;grid-gap:var(--gap-mid);grid-template-columns:max-content 1fr max-content max-content;align-items:center;width:100%;padding:var(--gap-mid);border-top:var(--border-light)}lr-external-source .back-btn{padding-left:0}lr-external-source .back-btn:after{content:var(--l10n-back)}lr-external-source .selected-counter{display:flex;grid-gap:var(--gap-mid);align-items:center;justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt-light)}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-upload-details{display:flex;flex-direction:column;width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height);overflow:hidden;background-color:var(--clr-background-light)}lr-upload-details>.content{position:relative;display:grid;flex:1;grid-template-rows:auto min-content}lr-upload-details lr-tabs .tabs-context{position:relative}lr-upload-details .toolbar{display:grid;grid-template-columns:min-content min-content 1fr min-content;gap:var(--gap-mid);padding:var(--gap-mid);border-top:var(--border-light)}lr-upload-details .toolbar[edit-disabled]{display:flex;justify-content:space-between}lr-upload-details .remove-btn{padding-left:.5em}lr-upload-details .detail-btn{padding-left:0;color:var(--clr-txt);background-color:var(--clr-background)}lr-upload-details .edit-btn{padding-left:.5em}lr-upload-details .details{padding:var(--gap-max)}lr-upload-details .info-block{padding-top:var(--gap-max);padding-bottom:calc(var(--gap-max) + var(--gap-table));color:var(--clr-txt);border-bottom:var(--border-light)}lr-upload-details .info-block:first-of-type{padding-top:0}lr-upload-details .info-block:last-of-type{border-bottom:none}lr-upload-details .info-block>.info-block_name{margin-bottom:.4em;color:var(--clr-txt-light);font-size:.8em}lr-upload-details .cdn-link[disabled]{pointer-events:none}lr-upload-details .cdn-link[disabled]:before{filter:grayscale(1);content:var(--l10n-not-uploaded-yet)}lr-file-preview{position:absolute;inset:0;display:flex;align-items:center;justify-content:center}lr-file-preview>lr-img{display:contents}lr-file-preview>lr-img>.img-view{position:absolute;inset:0;width:100%;max-width:100%;height:100%;max-height:100%;object-fit:scale-down}lr-confirmation-dialog{display:block;padding:var(--gap-mid);padding-top:var(--gap-max)}lr-confirmation-dialog .message{display:flex;justify-content:center;padding:var(--gap-mid);padding-bottom:var(--gap-max);font-weight:500;font-size:1.1em}lr-confirmation-dialog .toolbar{display:grid;grid-template-columns:1fr 1fr;gap:var(--gap-mid);margin-top:var(--gap-mid)}lr-progress-bar-common{position:fixed;right:0;bottom:0;left:0;z-index:10000;display:block;height:var(--gap-mid);background-color:var(--clr-background);transition:opacity .3s}lr-progress-bar-common:not([active]){opacity:0;pointer-events:none}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--hidden{opacity:0}lr-activity-header{display:flex;gap:var(--gap-mid);justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt);font-weight:500;font-size:1em;line-height:var(--ui-size)}lr-activity-header lr-icon{height:var(--ui-size)}lr-activity-header>*{display:flex;align-items:center}lr-activity-header button{display:inline-flex;align-items:center;justify-content:center;color:var(--clr-txt-mid)}lr-activity-header button:hover{background-color:var(--clr-background)}lr-activity-header button:active{background-color:var(--clr-background-dark)}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:host(.lr-cloud-image-editor) lr-icon,.lr-cloud-image-editor lr-icon{display:flex;align-items:center;justify-content:center;width:100%;height:100%}:host(.lr-cloud-image-editor) lr-icon svg,.lr-cloud-image-editor lr-icon svg{width:unset;height:unset}:host(.lr-cloud-image-editor) lr-icon:not([raw]) path,.lr-cloud-image-editor lr-icon:not([raw]) path{stroke-linejoin:round;fill:none;stroke:currentColor;stroke-width:1.2}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--icon-rotate: "M13.5.399902L12 1.9999l1.5 1.6M12.0234 2H14.4C16.3882 2 18 3.61178 18 5.6V8M4 17h9c.5523 0 1-.4477 1-1V7c0-.55228-.4477-1-1-1H4c-.55228 0-1 .44771-1 1v9c0 .5523.44771 1 1 1z";--icon-mirror: "M5.00042.399902l-1.5 1.599998 1.5 1.6M15.0004.399902l1.5 1.599998-1.5 1.6M3.51995 2H16.477M8.50042 16.7V6.04604c0-.30141-.39466-.41459-.5544-.159L1.28729 16.541c-.12488.1998.01877.459.2544.459h6.65873c.16568 0 .3-.1343.3-.3zm2.99998 0V6.04604c0-.30141.3947-.41459.5544-.159L18.7135 16.541c.1249.1998-.0187.459-.2544.459h-6.6587c-.1657 0-.3-.1343-.3-.3z";--icon-flip: "M19.6001 4.99993l-1.6-1.5-1.6 1.5m3.2 9.99997l-1.6 1.5-1.6-1.5M18 3.52337V16.4765M3.3 8.49993h10.654c.3014 0 .4146-.39466.159-.5544L3.459 1.2868C3.25919 1.16192 3 1.30557 3 1.5412v6.65873c0 .16568.13432.3.3.3zm0 2.99997h10.654c.3014 0 .4146.3947.159.5544L3.459 18.7131c-.19981.1248-.459-.0188-.459-.2544v-6.6588c0-.1657.13432-.3.3-.3z";--icon-sad: "M2 17c4.41828-4 11.5817-4 16 0M16.5 5c0 .55228-.4477 1-1 1s-1-.44772-1-1 .4477-1 1-1 1 .44772 1 1zm-11 0c0 .55228-.44772 1-1 1s-1-.44772-1-1 .44772-1 1-1 1 .44772 1 1z";--icon-closeMax: "M3 3l14 14m0-14L3 17";--icon-crop: "M20 14H7.00513C6.45001 14 6 13.55 6 12.9949V0M0 6h13.0667c.5154 0 .9333.41787.9333.93333V20M14.5.399902L13 1.9999l1.5 1.6M13 2h2c1.6569 0 3 1.34315 3 3v2M5.5 19.5999l1.5-1.6-1.5-1.6M7 18H5c-1.65685 0-3-1.3431-3-3v-2";--icon-tuning: "M8 10h11M1 10h4M1 4.5h11m3 0h4m-18 11h11m3 0h4M12 4.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M5 10a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M12 15.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0";--icon-filters: "M4.5 6.5a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m-3.5 6a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m7 0a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0";--icon-done: "M1 10.6316l5.68421 5.6842L19 4";--icon-original: "M0 40L40-.00000133";--icon-slider: "M0 10h11m0 0c0 1.1046.8954 2 2 2s2-.8954 2-2m-4 0c0-1.10457.8954-2 2-2s2 .89543 2 2m0 0h5";--icon-exposure: "M10 20v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M5 10a5 5 0 1010 0 5 5 0 10-10 0";--icon-contrast: "M2 10a8 8 0 1016 0 8 8 0 10-16 0m8-8v16m8-8h-8m7.5977 2.5H10m6.24 2.5H10m7.6-7.5H10M16.2422 5H10";--icon-brightness: "M15 10c0 2.7614-2.2386 5-5 5m5-5c0-2.76142-2.2386-5-5-5m5 5h-5m0 5c-2.76142 0-5-2.2386-5-5 0-2.76142 2.23858-5 5-5m0 10V5m0 15v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M14.3242 7.5H10m4.3242 5H10";--icon-gamma: "M17 3C9 6 2.5 11.5 2.5 17.5m0 0h1m-1 0v-1m14 1h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3-14v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1";--icon-enhance: "M19 13h-2m0 0c-2.2091 0-4-1.7909-4-4m4 4c-2.2091 0-4 1.7909-4 4m0-8V7m0 2c0 2.2091-1.7909 4-4 4m-2 0h2m0 0c2.2091 0 4 1.7909 4 4m0 0v2M8 8.5H6.5m0 0c-1.10457 0-2-.89543-2-2m2 2c-1.10457 0-2 .89543-2 2m0-4V5m0 1.5c0 1.10457-.89543 2-2 2M1 8.5h1.5m0 0c1.10457 0 2 .89543 2 2m0 0V12M12 3h-1m0 0c-.5523 0-1-.44772-1-1m1 1c-.5523 0-1 .44772-1 1m0-2V1m0 1c0 .55228-.44772 1-1 1M8 3h1m0 0c.55228 0 1 .44772 1 1m0 0v1";--icon-saturation: '    <circle cx="10.0006" cy="10.0001" r="9" transform="rotate(90 10.0006 10.0001)" fill="url(#paint0_linear)"/>     <defs>       <linearGradient id="paint0_linear" x1="10.0006" y1="1.00009" x2="10.0006" y2="19.0001" gradientUnits="userSpaceOnUse">         <stop stop-color="#DE15FF"/>         <stop offset=".203125" stop-color="#0029FF"/>         <stop offset=".479167" stop-color="#2AE4F0"/>         <stop offset=".604167" stop-color="#15EF11"/>         <stop offset=".75" stop-color="#FAE528"/>         <stop offset="1" stop-color="#EB2A2A"/>       </linearGradient>     </defs>  ';--icon-warmth: '    <path d="M7.5 13.0505l.42854.4199.17146-.1749v-.245h-.6zm5 0h-.6v.245l.1715.1749.4285-.4199zM8.1 3.5c0-1.04934.85066-1.9 1.9-1.9V.4C8.28792.4 6.9 1.78792 6.9 3.5h1.2zm0 9.5505V3.5H6.9v9.5505h1.2zM7.1 15.5c0-.7904.31539-1.5059.82854-2.0296l-.85708-.8398C6.34742 13.3694 5.9 14.3831 5.9 15.5h1.2zm2.9 2.9c-1.60163 0-2.9-1.2984-2.9-2.9H5.9c0 2.2644 1.83563 4.1 4.1 4.1v-1.2zm2.9-2.9c0 1.6016-1.2984 2.9-2.9 2.9v1.2c2.2644 0 4.1-1.8356 4.1-4.1h-1.2zm-.8285-2.0296c.5131.5237.8285 1.2392.8285 2.0296h1.2c0-1.1169-.4474-2.1306-1.1715-2.8694l-.857.8398zM11.9 3.5v9.5505h1.2V3.5h-1.2zM10 1.6c1.0493 0 1.9.85066 1.9 1.9h1.2c0-1.71208-1.3879-3.1-3.1-3.1v1.2z" fill="currentColor"/>    <path d="M10 14V8" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/>    <path d="M14 3h3m-3 3h3m-3 3h3m-8 6.5a1 1 0 102 0 1 1 0 10-2 0" stroke="currentColor" stroke-width="1.2"/>  ';--icon-vibrance: '  <path d="M2.125 5.6407c-.71643 1.29152-1.12439 2.77782-1.12439 4.3594 0 1.5816.40796 3.0679 1.12439 4.3594V5.6407z" fill="url(#paint0_linear)"/>  <path d="M2.875 15.4986V4.5016c.50222-.64987 1.09136-1.22915 1.75-1.72041V17.219c-.65864-.4912-1.24778-1.0705-1.75-1.7204z" fill="url(#paint1_linear)"/>  <path d="M5.375 17.722c.54811.3291 1.13415.6014 1.75.8089V1.46929c-.61585.20751-1.20189.47984-1.75.80888V17.722z" fill="url(#paint2_linear)"/>  <path d="M7.875 1.25258V18.7476c.56442.1367 1.14962.2202 1.75.2448V1.0078c-.60038.02465-1.18558.10811-1.75.24478z" fill="url(#paint3_linear)"/>  <path d="M10.375 1.00775V18.9925c.6004-.0246 1.1856-.108 1.75-.2446V1.25228c-.5644-.13658-1.1496-.21996-1.75-.24453z" fill="url(#paint4_linear)"/>  <path d="M12.875 1.46887V18.5313c.6158-.2074 1.2019-.4796 1.75-.8085V2.27744c-.5481-.32893-1.1342-.60115-1.75-.80857z" fill="url(#paint5_linear)"/>  <path d="M15.375 2.78028V17.2199c.6586-.491 1.2477-1.0701 1.75-1.7197V4.50002c-.5023-.64963-1.0914-1.22868-1.75-1.71974z" fill="url(#paint6_linear)"/>  <path d="M17.875 5.6385v8.7232c.7172-1.292 1.1256-2.7791 1.1256-4.3616 0-1.58248-.4084-3.06956-1.1256-4.3616z" fill="url(#paint7_linear)"/>  <defs>    <linearGradient id="paint0_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint1_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint2_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint3_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint4_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint5_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint6_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint7_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>  </defs>  '}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--l10n-cancel: "Cancel";--l10n-apply: "Apply";--l10n-brightness: "Brightness";--l10n-exposure: "Exposure";--l10n-gamma: "Gamma";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-vibrance: "Vibrance";--l10n-warmth: "Warmth";--l10n-enhance: "Enhance";--l10n-original: "Original"}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--rgb-primary-accent: 6, 2, 196;--rgb-text-base: 0, 0, 0;--rgb-text-accent-contrast: 255, 255, 255;--rgb-fill-contrast: 255, 255, 255;--rgb-fill-shaded: 245, 245, 245;--rgb-shadow: 0, 0, 0;--rgb-error: 209, 81, 81;--opacity-shade-mid: .2;--color-primary-accent: rgb(var(--rgb-primary-accent));--color-text-base: rgb(var(--rgb-text-base));--color-text-accent-contrast: rgb(var(--rgb-text-accent-contrast));--color-text-soft: rgb(var(--rgb-fill-contrast));--color-text-error: rgb(var(--rgb-error));--color-fill-contrast: rgb(var(--rgb-fill-contrast));--color-modal-backdrop: rgba(var(--rgb-fill-shaded), .95);--color-image-background: rgba(var(--rgb-fill-shaded));--color-outline: rgba(var(--rgb-text-base), var(--opacity-shade-mid));--color-underline: rgba(var(--rgb-text-base), .08);--color-shade: rgba(var(--rgb-text-base), .02);--color-focus-ring: var(--color-primary-accent);--color-input-placeholder: rgba(var(--rgb-text-base), .32);--color-error: rgb(var(--rgb-error));--font-size-ui: 16px;--font-size-title: 18px;--font-weight-title: 500;--font-size-soft: 14px;--size-touch-area: 40px;--size-panel-heading: 66px;--size-ui-min-width: 130px;--size-line-width: 1px;--size-modal-width: 650px;--border-radius-connect: 2px;--border-radius-editor: 3px;--border-radius-thumb: 4px;--border-radius-ui: 5px;--border-radius-base: 6px;--cldtr-gap-min: 5px;--cldtr-gap-mid-1: 10px;--cldtr-gap-mid-2: 15px;--cldtr-gap-max: 20px;--opacity-min: var(--opacity-shade-mid);--opacity-mid: .1;--opacity-max: .05;--transition-duration-2: var(--transition-duration-all, .2s);--transition-duration-3: var(--transition-duration-all, .3s);--transition-duration-4: var(--transition-duration-all, .4s);--transition-duration-5: var(--transition-duration-all, .5s);--shadow-base: 0px 5px 15px rgba(var(--rgb-shadow), .1), 0px 1px 4px rgba(var(--rgb-shadow), .15);--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading);--transparent-pixel: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=);display:block;width:100%;height:100%;max-height:100%}:host(.lr-cloud-image-editor) :is([can-handle-paste]:hover,[can-handle-paste]:focus),.lr-cloud-image-editor :is([can-handle-paste]:hover,[can-handle-paste]:focus){--can-handle-paste: "true"}:host(.lr-cloud-image-editor) :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover),.lr-cloud-image-editor :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover){--filter-effect: var(--hover-filter) !important;--opacity-effect: var(--hover-opacity) !important;--color-effect: var(--hover-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex]:active,[with-effects]:active),.lr-cloud-image-editor :is([tabindex]:active,[with-effects]:active){--filter-effect: var(--down-filter) !important;--opacity-effect: var(--down-opacity) !important;--color-effect: var(--down-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex][active],[with-effects][active]),.lr-cloud-image-editor :is([tabindex][active],[with-effects][active]){--filter-effect: var(--active-filter) !important;--opacity-effect: var(--active-opacity) !important;--color-effect: var(--active-color-rgb) !important}:host(.lr-cloud-image-editor) [hidden-scrollbar]::-webkit-scrollbar,.lr-cloud-image-editor [hidden-scrollbar]::-webkit-scrollbar{display:none}:host(.lr-cloud-image-editor) [hidden-scrollbar],.lr-cloud-image-editor [hidden-scrollbar]{-ms-overflow-style:none;scrollbar-width:none}:host(.lr-cloud-image-editor.editor_ON),.lr-cloud-image-editor.editor_ON{--modal-header-opacity: 0;--modal-header-height: 0px;--modal-toolbar-height: calc(var(--size-panel-heading) * 2)}:host(.lr-cloud-image-editor.editor_OFF),.lr-cloud-image-editor.editor_OFF{--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading)}:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-min-img-height: var(--modal-toolbar-height);--l-max-img-height: 100%;--l-edit-button-width: 120px;--l-toolbar-horizontal-padding: var(--cldtr-gap-mid-1);position:relative;display:grid;grid-template-rows:minmax(var(--l-min-img-height),var(--l-max-img-height)) minmax(var(--modal-toolbar-height),auto);height:100%;overflow:hidden;overflow-y:auto}@media only screen and (max-width: 800px){:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-edit-button-width: 70px;--l-toolbar-horizontal-padding: var(--cldtr-gap-min)}}:host(.lr-cloud-image-editor)>.wrapper>.viewport,.lr-cloud-image-editor>.wrapper>.viewport{display:flex;align-items:center;justify-content:center;overflow:hidden}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image{--viewer-image-opacity: 1;position:absolute;top:0;left:0;z-index:10;display:block;box-sizing:border-box;width:100%;height:100%;object-fit:scale-down;background-color:var(--color-image-background);transform:scale(1);opacity:var(--viewer-image-opacity);user-select:none;pointer-events:auto}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_visible_viewer,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_visible_viewer{transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-4)}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper{--viewer-image-opacity: 0;background-image:var(--transparent-pixel);transform:scale(1);transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_effects,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_effects{--viewer-image-opacity: 0;transform:scale(1);transition:opacity var(--transition-duration-3) cubic-bezier(.5,0,1,1),transform var(--transition-duration-4);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container,.lr-cloud-image-editor>.wrapper>.viewport>.image_container{position:relative;display:block;width:100%;height:100%;background-color:var(--color-image-background);transition:var(--transition-duration-3)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar,.lr-cloud-image-editor>.wrapper>.toolbar{position:relative;transition:.3s}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content{position:absolute;bottom:0;left:0;box-sizing:border-box;width:100%;height:var(--modal-toolbar-height);min-height:var(--size-panel-heading);background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer{display:flex;align-items:center;justify-content:space-between;height:var(--size-panel-heading);padding-right:var(--l-toolbar-horizontal-padding);padding-left:var(--l-toolbar-horizontal-padding)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor{display:flex}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.info_pan,.lr-cloud-image-editor>.wrapper>.viewport>.info_pan{position:absolute;user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer{position:absolute;z-index:2;display:flex;max-width:120px;transform:translate(-40px);user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer>.file_type,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer>.file_type{padding:4px .8em}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash,.lr-cloud-image-editor>.wrapper>.network_problems_splash{position:absolute;z-index:4;display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content{display:flex;flex:1;flex-direction:column;align-items:center;justify-content:center}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon{display:flex;align-items:center;justify-content:center;width:40px;height:40px;color:rgba(var(--rgb-text-base),.6);background-color:rgba(var(--rgb-fill-shaded));border-radius:50%}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text{margin-top:var(--cldtr-gap-max);font-size:var(--font-size-ui)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_footer,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_footer{display:flex;align-items:center;justify-content:center;height:var(--size-panel-heading)}lr-crop-frame>.svg{position:absolute;top:0;left:0;z-index:2;width:100%;height:100%;border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);opacity:inherit;transition:var(--transition-duration-3)}lr-crop-frame>.thumb{--idle-color-rgb: var(--color-text-base);--hover-color-rgb: var(--color-primary-accent);--focus-color-rgb: var(--color-primary-accent);--down-color-rgb: var(--color-primary-accent);--color-effect: var(--idle-color-rgb);color:var(--color-effect);transition:color var(--transition-duration-3),opacity var(--transition-duration-3)}lr-crop-frame>.thumb--visible{opacity:1;pointer-events:auto}lr-crop-frame>.thumb--hidden{opacity:0;pointer-events:none}lr-crop-frame>.guides{transition:var(--transition-duration-3)}lr-crop-frame>.guides--hidden{opacity:0}lr-crop-frame>.guides--semi-hidden{opacity:.2}lr-crop-frame>.guides--visible{opacity:1}lr-editor-button-control,lr-editor-crop-button-control,lr-editor-filter-control,lr-editor-operation-control{--l-base-min-width: 40px;--l-base-height: var(--l-base-min-width);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--filter-effect: var(--idle-filter);--idle-color-rgb: var(--rgb-text-base);--idle-opacity: .05;--idle-filter: 1;--hover-color-rgb: var(--idle-color-rgb);--hover-opacity: .08;--hover-filter: .8;--down-color-rgb: var(--hover-color-rgb);--down-opacity: .12;--down-filter: .6;position:relative;display:grid;grid-template-columns:var(--l-base-min-width) auto;align-items:center;height:var(--l-base-height);color:rgba(var(--idle-color-rgb));outline:none;cursor:pointer;transition:var(--l-width-transition)}lr-editor-button-control.active,lr-editor-operation-control.active,lr-editor-crop-button-control.active,lr-editor-filter-control.active{--idle-color-rgb: var(--rgb-primary-accent)}lr-editor-filter-control.not_active .preview[loaded]{opacity:1}lr-editor-filter-control.active .preview{opacity:0}lr-editor-button-control.not_active,lr-editor-operation-control.not_active,lr-editor-crop-button-control.not_active,lr-editor-filter-control.not_active{--idle-color-rgb: var(--rgb-text-base)}lr-editor-button-control>.before,lr-editor-operation-control>.before,lr-editor-crop-button-control>.before,lr-editor-filter-control>.before{position:absolute;right:0;left:0;z-index:-1;width:100%;height:100%;background-color:rgba(var(--color-effect),var(--opacity-effect));border-radius:var(--border-radius-editor);transition:var(--transition-duration-3)}lr-editor-button-control>.title,lr-editor-operation-control>.title,lr-editor-crop-button-control>.title,lr-editor-filter-control>.title{padding-right:var(--cldtr-gap-mid-1);font-size:.7em;letter-spacing:1.004px;text-transform:uppercase}lr-editor-filter-control>.preview{position:absolute;right:0;left:0;z-index:1;width:100%;height:var(--l-base-height);background-repeat:no-repeat;background-size:contain;border-radius:var(--border-radius-editor);opacity:0;filter:brightness(var(--filter-effect));transition:var(--transition-duration-3)}lr-editor-filter-control>.original-icon{color:var(--color-text-base);opacity:.3}lr-editor-image-cropper{position:absolute;top:0;left:0;z-index:10;display:block;width:100%;height:100%;opacity:0;pointer-events:none;touch-action:none}lr-editor-image-cropper.active_from_editor{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.active_from_viewer{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.inactive_to_editor{opacity:0;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1),opacity var(--transition-duration-3) calc(var(--transition-duration-3) + .05s);pointer-events:none}lr-editor-image-cropper>.canvas{position:absolute;top:0;left:0;z-index:1;display:block;width:100%;height:100%}lr-editor-image-fader{position:absolute;top:0;left:0;display:block;width:100%;height:100%}lr-editor-image-fader.active_from_viewer{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-start);pointer-events:auto}lr-editor-image-fader.active_from_cropper{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:auto}lr-editor-image-fader.inactive_to_cropper{z-index:3;transform:scale(1);opacity:0;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}lr-editor-image-fader .fader-image{position:absolute;top:0;left:0;display:block;width:100%;height:100%;object-fit:scale-down;transform:scale(1);user-select:none;content-visibility:auto}lr-editor-image-fader .fader-image--preview{background-color:var(--color-image-background);border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);transform:scale(1);opacity:0;transition:var(--transition-duration-3)}lr-editor-scroller{display:flex;align-items:center;width:100%;height:100%;overflow-x:scroll}lr-editor-slider{display:flex;align-items:center;justify-content:center;width:100%;height:66px}lr-editor-toolbar{position:relative;width:100%;height:100%}@media only screen and (max-width: 600px){lr-editor-toolbar{--l-tab-gap: var(--cldtr-gap-mid-1);--l-slider-padding: var(--cldtr-gap-min);--l-controls-padding: var(--cldtr-gap-min)}}@media only screen and (min-width: 601px){lr-editor-toolbar{--l-tab-gap: calc(var(--cldtr-gap-mid-1) + var(--cldtr-gap-max));--l-slider-padding: var(--cldtr-gap-mid-1);--l-controls-padding: var(--cldtr-gap-mid-1)}}lr-editor-toolbar>.toolbar-container{position:relative;width:100%;height:100%;overflow:hidden}lr-editor-toolbar>.toolbar-container>.sub-toolbar{position:absolute;display:grid;grid-template-rows:1fr 1fr;width:100%;height:100%;background-color:var(--color-fill-contrast);transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-3) ease-in-out,visibility var(--transition-duration-3) ease-in-out}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--visible{transform:translateY(0);opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--top-hidden{transform:translateY(100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--bottom-hidden{transform:translateY(-100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row{display:flex;align-items:center;justify-content:space-between;padding-right:var(--l-controls-padding);padding-left:var(--l-controls-padding)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles{position:relative;display:grid;grid-auto-flow:column;grid-gap:0px var(--l-tab-gap);align-items:center;height:100%}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggles_indicator{position:absolute;bottom:0;left:0;width:var(--size-touch-area);height:2px;background-color:var(--color-primary-accent);transform:translate(0);transition:transform var(--transition-duration-3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row{position:relative}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content{position:absolute;top:0;left:0;display:flex;width:100%;height:100%;overflow:hidden;opacity:0;content-visibility:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--visible{opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--hidden{opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--visible{display:contents}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles.tab-toggles--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_align{display:grid;grid-template-areas:". inner .";grid-template-columns:1fr auto 1fr;box-sizing:border-box;min-width:100%;padding-left:var(--cldtr-gap-max)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner{display:grid;grid-area:inner;grid-auto-flow:column;grid-gap:calc((var(--cldtr-gap-min) - 1px) * 3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner:last-child{padding-right:var(--cldtr-gap-max)}lr-editor-toolbar .controls-list_last-item{margin-right:var(--cldtr-gap-max)}lr-editor-toolbar .info-tooltip_container{position:absolute;display:flex;align-items:flex-start;justify-content:center;width:100%;height:100%}lr-editor-toolbar .info-tooltip_wrapper{position:absolute;top:calc(-100% - var(--cldtr-gap-mid-2));display:flex;flex-direction:column;justify-content:flex-end;height:100%;pointer-events:none}lr-editor-toolbar .info-tooltip{z-index:3;padding-top:calc(var(--cldtr-gap-min) / 2);padding-right:var(--cldtr-gap-min);padding-bottom:calc(var(--cldtr-gap-min) / 2);padding-left:var(--cldtr-gap-min);color:var(--color-text-base);font-size:.7em;letter-spacing:1px;text-transform:uppercase;background-color:var(--color-text-accent-contrast);border-radius:var(--border-radius-editor);transform:translateY(100%);opacity:0;transition:var(--transition-duration-3)}lr-editor-toolbar .info-tooltip_visible{transform:translateY(0);opacity:1}lr-editor-toolbar .slider{padding-right:var(--l-slider-padding);padding-left:var(--l-slider-padding)}lr-btn-ui{--filter-effect: var(--idle-brightness);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--l-transition-effect: var(--css-transition, color var(--transition-duration-2), filter var(--transition-duration-2));display:inline-flex;align-items:center;box-sizing:var(--css-box-sizing, border-box);height:var(--css-height, var(--size-touch-area));padding-right:var(--css-padding-right, var(--cldtr-gap-mid-1));padding-left:var(--css-padding-left, var(--cldtr-gap-mid-1));color:rgba(var(--color-effect),var(--opacity-effect));outline:none;cursor:pointer;filter:brightness(var(--filter-effect));transition:var(--l-transition-effect);user-select:none}lr-btn-ui .text{white-space:nowrap}lr-btn-ui .icon{display:flex;align-items:center;justify-content:center;color:rgba(var(--color-effect),var(--opacity-effect));filter:brightness(var(--filter-effect));transition:var(--l-transition-effect)}lr-btn-ui .icon_left{margin-right:var(--cldtr-gap-mid-1);margin-left:0}lr-btn-ui .icon_right{margin-right:0;margin-left:var(--cldtr-gap-mid-1)}lr-btn-ui .icon_single{margin-right:0;margin-left:0}lr-btn-ui .icon_hidden{display:none;margin:0}lr-btn-ui.primary{--idle-color-rgb: var(--rgb-primary-accent);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--idle-color-rgb);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.boring{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-text-base);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: 1;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.default{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-primary-accent);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-line-loader-ui{position:absolute;top:0;left:0;z-index:9999;width:100%;height:2px;opacity:.5}lr-line-loader-ui .inner{width:25%;max-width:200px;height:100%}lr-line-loader-ui .line{width:100%;height:100%;background-color:var(--color-primary-accent);transform:translate(-101%);transition:transform 1s}lr-slider-ui{--l-thumb-size: 24px;--l-zero-dot-size: 5px;--l-zero-dot-offset: 2px;--idle-color-rgb: var(--rgb-text-base);--hover-color-rgb: var(--rgb-primary-accent);--down-color-rgb: var(--rgb-primary-accent);--color-effect: var(--idle-color-rgb);--l-color: rgb(var(--color-effect));position:relative;display:flex;align-items:center;justify-content:center;width:100%;height:calc(var(--l-thumb-size) + (var(--l-zero-dot-size) + var(--l-zero-dot-offset)) * 2)}lr-slider-ui .thumb{position:absolute;left:0;width:var(--l-thumb-size);height:var(--l-thumb-size);background-color:var(--l-color);border-radius:50%;transform:translate(0);opacity:1;transition:opacity var(--transition-duration-2)}lr-slider-ui .steps{position:absolute;display:flex;align-items:center;justify-content:space-between;box-sizing:border-box;width:100%;height:100%;padding-right:calc(var(--l-thumb-size) / 2);padding-left:calc(var(--l-thumb-size) / 2)}lr-slider-ui .border-step{width:0px;height:10px;border-right:1px solid var(--l-color);opacity:.6;transition:var(--transition-duration-2)}lr-slider-ui .minor-step{width:0px;height:4px;border-right:1px solid var(--l-color);opacity:.2;transition:var(--transition-duration-2)}lr-slider-ui .zero-dot{position:absolute;top:calc(100% - var(--l-zero-dot-offset) * 2);left:calc(var(--l-thumb-size) / 2 - var(--l-zero-dot-size) / 2);width:var(--l-zero-dot-size);height:var(--l-zero-dot-size);background-color:var(--color-primary-accent);border-radius:50%;opacity:0;transition:var(--transition-duration-3)}lr-slider-ui .input{position:absolute;width:calc(100% - 10px);height:100%;margin:0;cursor:pointer;opacity:0}lr-presence-toggle.transition{transition:opacity var(--transition-duration-3),visibility var(--transition-duration-3)}lr-presence-toggle.visible{opacity:1;pointer-events:inherit}lr-presence-toggle.hidden{opacity:0;pointer-events:none}ctx-provider{--color-text-base: black;--color-primary-accent: blue;display:flex;align-items:center;justify-content:center;width:190px;height:40px;padding-right:10px;padding-left:10px;background-color:#f5f5f5;border-radius:3px}lr-cloud-image-editor-activity{position:relative;display:flex;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light)}lr-modal lr-cloud-image-editor-activity{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%)}lr-select{display:inline-flex}lr-select>button{position:relative;display:inline-flex;align-items:center;padding-right:0!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-select>button>select{position:absolute;display:block;width:100%;height:100%;opacity:0}:host{flex:1}lr-start-from{height:100%;container-type:inline-size}.lr-wgt-common,:host{--cfg-done-activity: "start-from";--cfg-init-activity: "start-from"}lr-activity-header:after{width:var(--ui-size);height:var(--ui-size);content:""}lr-activity-header .close-btn{display:none}@container (min-width: 500px){lr-start-from .content{grid-template-columns:1fr max-content;height:100%}lr-start-from lr-copyright{grid-column:2}lr-start-from lr-drop-area{grid-row:span 3}lr-start-from:has(lr-copyright[hidden]) lr-drop-area{grid-row:span 2}lr-start-from:has(.cancel-btn[hidden]) lr-drop-area{grid-row:span 2}lr-start-from:has(lr-copyright[hidden]):has(.cancel-btn[hidden]) lr-drop-area{grid-row:span 1}}
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-minimal.min.css` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-minimal.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--unknown{width:100%;transform-origin:0% 50%;animation:lr-indeterminateAnimation 1s infinite linear}lr-progress-bar .progress--hidden{opacity:0}@keyframes lr-indeterminateAnimation{0%{transform:translate(0) scaleX(0)}40%{transform:translate(0) scaleX(.4)}to{transform:translate(100%) scaleX(.5)}}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z"}:where(.lr-wgt-common),:host{--cfg-multiple: 1;--cfg-confirm-upload: 0;--cfg-init-activity: "start-from";--cfg-done-activity: "upload-list";position:relative;display:block}lr-start-from .content{display:flex;flex-direction:column;gap:var(--gap-min);padding:0;overflow:hidden;align-items:center;background-color:transparent}lr-drop-area{display:flex;align-items:center;justify-content:center;width:100%;min-height:calc(var(--ui-size) + var(--gap-mid) * 2 + var(--gap-min) * 4);padding:0;line-height:140%;text-align:center;background-color:var(--clr-background);border-radius:var(--border-radius-frame)}lr-upload-list lr-activity-header{display:none}lr-upload-list>.toolbar{background-color:transparent}lr-upload-list{width:100%;height:unset;padding:var(--gap-small);background-color:transparent;border:var(--border-dashed);border-radius:var(--border-radius-frame)}lr-upload-list .files{padding:0}lr-upload-list .toolbar{display:block;padding:0}lr-upload-list .toolbar .cancel-btn,lr-upload-list .toolbar .upload-btn,lr-upload-list .toolbar .done-btn{display:none}lr-upload-list .toolbar .add-more-btn{width:100%;height:calc(var(--ui-size) + var(--gap-mid) * 2);margin-top:var(--gap-small);background-color:var(--clr-background)}lr-upload-list .toolbar .add-more-btn[disabled]{display:none}lr-upload-list .toolbar .add-more-btn:hover{background-color:var(--clr-background-dark)}lr-upload-list .toolbar .add-more-btn>span{display:none}lr-file-item{background-color:var(--clr-background);border-radius:var(--border-radius-element)}lr-file-item .edit-btn{display:none}lr-file-item lr-progress-bar{top:0!important;height:100%!important}lr-file-item lr-progress-bar .progress{background-color:var(--clr-accent-lightest);border-radius:var(--border-radius-element)}lr-upload-list lr-drop-area{width:100%;height:100%;margin:0;border-radius:var(--border-radius-frame)}lr-upload-list .common-error{margin:var(--gap-small) 0 0 0}
+:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--hidden{opacity:0}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z"}:where(.lr-wgt-common),:host{--cfg-multiple: 1;--cfg-confirm-upload: 0;--cfg-init-activity: "start-from";--cfg-done-activity: "upload-list";position:relative;display:block}lr-start-from .content{display:flex;flex-direction:column;gap:var(--gap-min);padding:0;overflow:hidden;align-items:center;background-color:transparent}lr-drop-area{display:flex;align-items:center;justify-content:center;width:100%;min-height:calc(var(--ui-size) + var(--gap-mid) * 2 + var(--gap-min) * 4);padding:0;line-height:140%;text-align:center;background-color:var(--clr-background);border-radius:var(--border-radius-frame)}lr-upload-list lr-activity-header{display:none}lr-upload-list>.toolbar{background-color:transparent}lr-upload-list{width:100%;height:unset;padding:var(--gap-small);background-color:transparent;border:var(--border-dashed);border-radius:var(--border-radius-frame)}lr-upload-list .files{padding:0}lr-upload-list .toolbar{display:block;padding:0}lr-upload-list .toolbar .cancel-btn,lr-upload-list .toolbar .upload-btn,lr-upload-list .toolbar .done-btn{display:none}lr-upload-list .toolbar .add-more-btn{width:100%;height:calc(var(--ui-size) + var(--gap-mid) * 2);margin-top:var(--gap-small);background-color:var(--clr-background)}lr-upload-list .toolbar .add-more-btn[disabled]{display:none}lr-upload-list .toolbar .add-more-btn:hover{background-color:var(--clr-background-dark)}lr-upload-list .toolbar .add-more-btn>span{display:none}lr-file-item{background-color:var(--clr-background);border-radius:var(--border-radius-element)}lr-file-item .edit-btn{display:none}lr-file-item lr-progress-bar{top:0!important;height:100%!important}lr-file-item lr-progress-bar .progress{background-color:var(--clr-accent-lightest);border-radius:var(--border-radius-element)}lr-upload-list lr-drop-area{width:100%;height:100%;margin:0;border-radius:var(--border-radius-frame)}lr-upload-list .common-error{margin:var(--gap-small) 0 0 0}
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/lr-file-uploader-regular.min.css` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/lr-file-uploader-regular.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-file: "m2.89453 1.2012c0-.473389.38376-.857145.85714-.857145h8.40003c.2273 0 .4453.090306.6061.251051l8.4 8.400004c.1607.16074.251.37876.251.60609v13.2c0 .4734-.3837.8571-.8571.8571h-16.80003c-.47338 0-.85714-.3837-.85714-.8571zm1.71429.85714v19.88576h15.08568v-11.4858h-7.5428c-.4734 0-.8572-.3837-.8572-.8571v-7.54286zm8.39998 1.21218 5.4736 5.47353-5.4736.00001z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-collapse: "M3.11572 12C3.11572 11.5858 3.45151 11.25 3.86572 11.25H20.1343C20.5485 11.25 20.8843 11.5858 20.8843 12C20.8843 12.4142 20.5485 12.75 20.1343 12.75H3.86572C3.45151 12.75 3.11572 12.4142 3.11572 12Z";--icon-expand: "M12.0001 8.33716L3.53033 16.8068C3.23743 17.0997 2.76256 17.0997 2.46967 16.8068C2.17678 16.5139 2.17678 16.0391 2.46967 15.7462L11.0753 7.14067C11.1943 7.01825 11.3365 6.92067 11.4936 6.8536C11.6537 6.78524 11.826 6.75 12.0001 6.75C12.1742 6.75 12.3465 6.78524 12.5066 6.8536C12.6637 6.92067 12.8059 7.01826 12.925 7.14068L21.5304 15.7462C21.8233 16.0391 21.8233 16.5139 21.5304 16.8068C21.2375 17.0997 20.7627 17.0997 20.4698 16.8068L12.0001 8.33716Z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-local: "m3 3.75c-.82843 0-1.5.67157-1.5 1.5v13.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-9.75c0-.82843-.6716-1.5-1.5-1.5h-9c-.2634 0-.5076-.13822-.6431-.36413l-2.03154-3.38587zm-3 1.5c0-1.65685 1.34315-3 3-3h6.75c.2634 0 .5076.13822.6431.36413l2.0315 3.38587h8.5754c1.6569 0 3 1.34315 3 3v9.75c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3z";--icon-url: "m19.1099 3.67026c-1.7092-1.70917-4.5776-1.68265-6.4076.14738l-2.2212 2.22122c-.2929.29289-.7678.29289-1.0607 0-.29289-.29289-.29289-.76777 0-1.06066l2.2212-2.22122c2.376-2.375966 6.1949-2.481407 8.5289-.14738l1.2202 1.22015c2.334 2.33403 2.2286 6.15294-.1474 8.52895l-2.2212 2.2212c-.2929.2929-.7678.2929-1.0607 0s-.2929-.7678 0-1.0607l2.2212-2.2212c1.8301-1.83003 1.8566-4.69842.1474-6.40759zm-3.3597 4.57991c.2929.29289.2929.76776 0 1.06066l-6.43918 6.43927c-.29289.2928-.76777.2928-1.06066 0-.29289-.2929-.29289-.7678 0-1.0607l6.43924-6.43923c.2929-.2929.7677-.2929 1.0606 0zm-9.71158 1.17048c.29289.29289.29289.76775 0 1.06065l-2.22123 2.2212c-1.83002 1.8301-1.85654 4.6984-.14737 6.4076l1.22015 1.2202c1.70917 1.7091 4.57756 1.6826 6.40763-.1474l2.2212-2.2212c.2929-.2929.7677-.2929 1.0606 0s.2929.7677 0 1.0606l-2.2212 2.2212c-2.37595 2.376-6.19486 2.4815-8.52889.1474l-1.22015-1.2201c-2.334031-2.3341-2.22859-6.153.14737-8.5289l2.22123-2.22125c.29289-.2929.76776-.2929 1.06066 0z";--icon-camera: "m7.65 2.55c.14164-.18885.36393-.3.6-.3h7.5c.2361 0 .4584.11115.6.3l2.025 2.7h2.625c1.6569 0 3 1.34315 3 3v10.5c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3v-10.5c0-1.65685 1.34315-3 3-3h2.625zm.975 1.2-2.025 2.7c-.14164.18885-.36393.3-.6.3h-3c-.82843 0-1.5.67157-1.5 1.5v10.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-10.5c0-.82843-.6716-1.5-1.5-1.5h-3c-.2361 0-.4584-.11115-.6-.3l-2.025-2.7zm3.375 6c-1.864 0-3.375 1.511-3.375 3.375s1.511 3.375 3.375 3.375 3.375-1.511 3.375-3.375-1.511-3.375-3.375-3.375zm-4.875 3.375c0-2.6924 2.18261-4.875 4.875-4.875 2.6924 0 4.875 2.1826 4.875 4.875s-2.1826 4.875-4.875 4.875c-2.69239 0-4.875-2.1826-4.875-4.875z";--icon-dots: "M16,12A2,2 0 0,1 18,10A2,2 0 0,1 20,12A2,2 0 0,1 18,14A2,2 0 0,1 16,12M10,12A2,2 0 0,1 12,10A2,2 0 0,1 14,12A2,2 0 0,1 12,14A2,2 0 0,1 10,12M4,12A2,2 0 0,1 6,10A2,2 0 0,1 8,12A2,2 0 0,1 6,14A2,2 0 0,1 4,12Z";--icon-back: "M20.251 12.0001C20.251 12.4143 19.9152 12.7501 19.501 12.7501L6.06696 12.7501L11.7872 18.6007C12.0768 18.8968 12.0715 19.3717 11.7753 19.6613C11.4791 19.9508 11.0043 19.9455 10.7147 19.6493L4.13648 12.9213C4.01578 12.8029 3.91947 12.662 3.85307 12.5065C3.78471 12.3464 3.74947 12.1741 3.74947 12C3.74947 11.8259 3.78471 11.6536 3.85307 11.4935C3.91947 11.338 4.01578 11.1971 4.13648 11.0787L10.7147 4.35068C11.0043 4.0545 11.4791 4.04916 11.7753 4.33873C12.0715 4.62831 12.0768 5.10315 11.7872 5.39932L6.06678 11.2501L19.501 11.2501C19.9152 11.2501 20.251 11.5859 20.251 12.0001Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-edit: "M3.96371 14.4792c-.15098.151-.25578.3419-.3021.5504L2.52752 20.133c-.17826.8021.53735 1.5177 1.33951 1.3395l5.10341-1.1341c.20844-.0463.39934-.1511.55032-.3021l8.05064-8.0507-5.557-5.55702-8.05069 8.05062ZM13.4286 5.01437l5.557 5.55703 2.0212-2.02111c.6576-.65765.6576-1.72393 0-2.38159l-3.1755-3.17546c-.6577-.65765-1.7239-.65765-2.3816 0l-2.0211 2.02113Z";--icon-detail: "M5,3C3.89,3 3,3.89 3,5V19C3,20.11 3.89,21 5,21H19C20.11,21 21,20.11 21,19V5C21,3.89 20.11,3 19,3H5M5,5H19V19H5V5M7,7V9H17V7H7M7,11V13H17V11H7M7,15V17H14V15H7Z";--icon-select: "M7,10L12,15L17,10H7Z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-fullscreen: "M5,5H10V7H7V10H5V5M14,5H19V10H17V7H14V5M17,14H19V19H14V17H17V14M10,17V19H5V14H7V17H10Z";--icon-fullscreen-exit: "M14,14H19V16H16V19H14V14M5,14H10V19H8V16H5V14M8,5H10V10H5V8H8V5M19,8V10H14V5H16V8H19Z";--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-about: "M11.152 14.12v.1h1.523v-.1c.007-.409.053-.752.138-1.028.086-.277.22-.517.405-.72.188-.202.434-.397.735-.586.32-.191.593-.412.82-.66.232-.249.41-.531.533-.847.125-.32.187-.678.187-1.076 0-.579-.137-1.085-.41-1.518a2.717 2.717 0 0 0-1.14-1.018c-.49-.245-1.062-.367-1.715-.367-.597 0-1.142.114-1.636.34-.49.228-.884.564-1.182 1.008-.299.44-.46.98-.485 1.619h1.62c.024-.377.118-.684.282-.922.163-.241.369-.419.617-.532.25-.114.51-.17.784-.17.301 0 .575.063.82.191.248.124.447.302.597.533.149.23.223.504.223.82 0 .263-.05.502-.149.72-.1.216-.234.408-.405.574a3.48 3.48 0 0 1-.575.453c-.33.199-.613.42-.847.66-.234.242-.415.558-.543.949-.125.39-.19.916-.197 1.577ZM11.205 17.15c.21.206.46.31.75.31.196 0 .374-.049.534-.144.16-.096.287-.224.383-.384.1-.163.15-.343.15-.538a1 1 0 0 0-.32-.746 1.019 1.019 0 0 0-.746-.314c-.291 0-.542.105-.751.314-.21.206-.314.455-.314.746 0 .295.104.547.314.756ZM24 12c0 6.627-5.373 12-12 12S0 18.627 0 12 5.373 0 12 0s12 5.373 12 12Zm-1.5 0c0 5.799-4.701 10.5-10.5 10.5S1.5 17.799 1.5 12 6.201 1.5 12 1.5 22.5 6.201 22.5 12Z";--icon-edit-rotate: "M16.89,15.5L18.31,16.89C19.21,15.73 19.76,14.39 19.93,13H17.91C17.77,13.87 17.43,14.72 16.89,15.5M13,17.9V19.92C14.39,19.75 15.74,19.21 16.9,18.31L15.46,16.87C14.71,17.41 13.87,17.76 13,17.9M19.93,11C19.76,9.61 19.21,8.27 18.31,7.11L16.89,8.53C17.43,9.28 17.77,10.13 17.91,11M15.55,5.55L11,1V4.07C7.06,4.56 4,7.92 4,12C4,16.08 7.05,19.44 11,19.93V17.91C8.16,17.43 6,14.97 6,12C6,9.03 8.16,6.57 11,6.09V10L15.55,5.55Z";--icon-edit-flip-v: "M3 15V17H5V15M15 19V21H17V19M19 3H5C3.9 3 3 3.9 3 5V9H5V5H19V9H21V5C21 3.9 20.1 3 19 3M21 19H19V21C20.1 21 21 20.1 21 19M1 11V13H23V11M7 19V21H9V19M19 15V17H21V15M11 19V21H13V19M3 19C3 20.1 3.9 21 5 21V19Z";--icon-edit-flip-h: "M15 21H17V19H15M19 9H21V7H19M3 5V19C3 20.1 3.9 21 5 21H9V19H5V5H9V3H5C3.9 3 3 3.9 3 5M19 3V5H21C21 3.9 20.1 3 19 3M11 23H13V1H11M19 17H21V15H19M15 5H17V3H15M19 13H21V11H19M19 21C20.1 21 21 20.1 21 19H19Z";--icon-edit-brightness: "M12,18A6,6 0 0,1 6,12A6,6 0 0,1 12,6A6,6 0 0,1 18,12A6,6 0 0,1 12,18M20,15.31L23.31,12L20,8.69V4H15.31L12,0.69L8.69,4H4V8.69L0.69,12L4,15.31V20H8.69L12,23.31L15.31,20H20V15.31Z";--icon-edit-contrast: "M12,20C9.79,20 7.79,19.1 6.34,17.66L17.66,6.34C19.1,7.79 20,9.79 20,12A8,8 0 0,1 12,20M6,8H8V6H9.5V8H11.5V9.5H9.5V11.5H8V9.5H6M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,16H17V14.5H12V16Z";--icon-edit-saturation: "M3,13A9,9 0 0,0 12,22C12,17 7.97,13 3,13M12,5.5A2.5,2.5 0 0,1 14.5,8A2.5,2.5 0 0,1 12,10.5A2.5,2.5 0 0,1 9.5,8A2.5,2.5 0 0,1 12,5.5M5.6,10.25A2.5,2.5 0 0,0 8.1,12.75C8.63,12.75 9.12,12.58 9.5,12.31C9.5,12.37 9.5,12.43 9.5,12.5A2.5,2.5 0 0,0 12,15A2.5,2.5 0 0,0 14.5,12.5C14.5,12.43 14.5,12.37 14.5,12.31C14.88,12.58 15.37,12.75 15.9,12.75C17.28,12.75 18.4,11.63 18.4,10.25C18.4,9.25 17.81,8.4 16.97,8C17.81,7.6 18.4,6.74 18.4,5.75C18.4,4.37 17.28,3.25 15.9,3.25C15.37,3.25 14.88,3.41 14.5,3.69C14.5,3.63 14.5,3.56 14.5,3.5A2.5,2.5 0 0,0 12,1A2.5,2.5 0 0,0 9.5,3.5C9.5,3.56 9.5,3.63 9.5,3.69C9.12,3.41 8.63,3.25 8.1,3.25A2.5,2.5 0 0,0 5.6,5.75C5.6,6.74 6.19,7.6 7.03,8C6.19,8.4 5.6,9.25 5.6,10.25M12,22A9,9 0 0,0 21,13C16,13 12,17 12,22Z";--icon-edit-crop: "M7,17V1H5V5H1V7H5V17A2,2 0 0,0 7,19H17V23H19V19H23V17M17,15H19V7C19,5.89 18.1,5 17,5H9V7H17V15Z";--icon-edit-text: "M18.5,4L19.66,8.35L18.7,8.61C18.25,7.74 17.79,6.87 17.26,6.43C16.73,6 16.11,6 15.5,6H13V16.5C13,17 13,17.5 13.33,17.75C13.67,18 14.33,18 15,18V19H9V18C9.67,18 10.33,18 10.67,17.75C11,17.5 11,17 11,16.5V6H8.5C7.89,6 7.27,6 6.74,6.43C6.21,6.87 5.75,7.74 5.3,8.61L4.34,8.35L5.5,4H18.5Z";--icon-edit-draw: "m21.879394 2.1631238c-1.568367-1.62768627-4.136546-1.53831744-5.596267.1947479l-8.5642801 10.1674753c-1.4906533-.224626-3.061232.258204-4.2082427 1.448604-1.0665468 1.106968-1.0997707 2.464806-1.1203996 3.308068-.00142.05753-.00277.113001-.00439.16549-.02754.894146-.08585 1.463274-.5821351 2.069648l-.80575206.98457.88010766.913285c1.0539516 1.093903 2.6691689 1.587048 4.1744915 1.587048 1.5279113 0 3.2235468-.50598 4.4466094-1.775229 1.147079-1.190514 1.612375-2.820653 1.395772-4.367818l9.796763-8.8879697c1.669907-1.5149954 1.75609-4.1802333.187723-5.8079195zm-16.4593821 13.7924592c.8752943-.908358 2.2944227-.908358 3.1697054 0 .8752942.908358.8752942 2.381259 0 3.289617-.5909138.61325-1.5255389.954428-2.53719.954428-.5223687 0-.9935663-.09031-1.3832112-.232762.3631253-.915463.3952949-1.77626.4154309-2.429737.032192-1.045425.072224-1.308557.3352649-1.581546z";--icon-edit-guides: "M1.39,18.36L3.16,16.6L4.58,18L5.64,16.95L4.22,15.54L5.64,14.12L8.11,16.6L9.17,15.54L6.7,13.06L8.11,11.65L9.53,13.06L10.59,12L9.17,10.59L10.59,9.17L13.06,11.65L14.12,10.59L11.65,8.11L13.06,6.7L14.47,8.11L15.54,7.05L14.12,5.64L15.54,4.22L18,6.7L19.07,5.64L16.6,3.16L18.36,1.39L22.61,5.64L5.64,22.61L1.39,18.36Z";--icon-edit-color: "M17.5,12A1.5,1.5 0 0,1 16,10.5A1.5,1.5 0 0,1 17.5,9A1.5,1.5 0 0,1 19,10.5A1.5,1.5 0 0,1 17.5,12M14.5,8A1.5,1.5 0 0,1 13,6.5A1.5,1.5 0 0,1 14.5,5A1.5,1.5 0 0,1 16,6.5A1.5,1.5 0 0,1 14.5,8M9.5,8A1.5,1.5 0 0,1 8,6.5A1.5,1.5 0 0,1 9.5,5A1.5,1.5 0 0,1 11,6.5A1.5,1.5 0 0,1 9.5,8M6.5,12A1.5,1.5 0 0,1 5,10.5A1.5,1.5 0 0,1 6.5,9A1.5,1.5 0 0,1 8,10.5A1.5,1.5 0 0,1 6.5,12M12,3A9,9 0 0,0 3,12A9,9 0 0,0 12,21A1.5,1.5 0 0,0 13.5,19.5C13.5,19.11 13.35,18.76 13.11,18.5C12.88,18.23 12.73,17.88 12.73,17.5A1.5,1.5 0 0,1 14.23,16H16A5,5 0 0,0 21,11C21,6.58 16.97,3 12,3Z";--icon-edit-resize: "M10.59,12L14.59,8H11V6H18V13H16V9.41L12,13.41V16H20V4H8V12H10.59M22,2V18H12V22H2V12H6V2H22M10,14H4V20H10V14Z";--icon-external-source-placeholder: "M6.341 3.27a10.5 10.5 0 0 1 5.834-1.77.75.75 0 0 0 0-1.5 12 12 0 1 0 12 12 .75.75 0 0 0-1.5 0A10.5 10.5 0 1 1 6.34 3.27Zm14.145 1.48a.75.75 0 1 0-1.06-1.062L9.925 13.19V7.95a.75.75 0 1 0-1.5 0V15c0 .414.336.75.75.75h7.05a.75.75 0 0 0 0-1.5h-5.24l9.501-9.5Z";--icon-facebook: "m12 1.5c-5.79901 0-10.5 4.70099-10.5 10.5 0 4.9427 3.41586 9.0888 8.01562 10.2045v-6.1086h-2.13281c-.41421 0-.75-.3358-.75-.75v-3.2812c0-.4142.33579-.75.75-.75h2.13281v-1.92189c0-.95748.22571-2.51089 1.38068-3.6497 1.1934-1.17674 3.1742-1.71859 6.2536-1.05619.3455.07433.5923.3798.5923.73323v2.75395c0 .41422-.3358.75-.75.75-.6917 0-1.2029.02567-1.5844.0819-.3865.05694-.5781.13711-.675.20223-.1087.07303-.2367.20457-.2367 1.02837v1.0781h2.3906c.2193 0 .4275.0959.57.2626.1425.1666.205.3872.1709.6038l-.5156 3.2813c-.0573.3647-.3716.6335-.7409.6335h-1.875v6.1058c4.5939-1.1198 8.0039-5.2631 8.0039-10.2017 0-5.79901-4.701-10.5-10.5-10.5zm-12 10.5c0-6.62744 5.37256-12 12-12 6.6274 0 12 5.37256 12 12 0 5.9946-4.3948 10.9614-10.1384 11.8564-.2165.0337-.4369-.0289-.6033-.1714s-.2622-.3506-.2622-.5697v-7.7694c0-.4142.3358-.75.75-.75h1.9836l.28-1.7812h-2.2636c-.4142 0-.75-.3358-.75-.75v-1.8281c0-.82854.0888-1.72825.9-2.27338.3631-.24396.8072-.36961 1.293-.4412.3081-.0454.6583-.07238 1.0531-.08618v-1.39629c-2.4096-.40504-3.6447.13262-4.2928.77165-.7376.72735-.9338 1.79299-.9338 2.58161v2.67189c0 .4142-.3358.75-.75.75h-2.13279v1.7812h2.13279c.4142 0 .75.3358.75.75v7.7712c0 .219-.0956.427-.2619.5695-.1662.1424-.3864.2052-.6028.1717-5.74968-.8898-10.1509-5.8593-10.1509-11.8583z";--icon-dropbox: "m6.01895 1.92072c.24583-.15659.56012-.15658.80593.00003l5.17512 3.29711 5.1761-3.29714c.2458-.15659.5601-.15658.8059.00003l5.5772 3.55326c.2162.13771.347.37625.347.63253 0 .25629-.1308.49483-.347.63254l-4.574 2.91414 4.574 2.91418c.2162.1377.347.3762.347.6325s-.1308.4948-.347.6325l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.1761-3.2971-5.17512 3.2971c-.24581.1566-.5601.1566-.80593 0l-5.578142-3.5532c-.216172-.1377-.347058-.3763-.347058-.6326s.130886-.4949.347058-.6326l4.574772-2.91408-4.574772-2.91411c-.216172-.1377-.347058-.37626-.347058-.63257 0-.2563.130886-.49486.347058-.63256zm.40291 8.61518-4.18213 2.664 4.18213 2.664 4.18144-2.664zm6.97504 2.664 4.1821 2.664 4.1814-2.664-4.1814-2.664zm2.7758-3.54668-4.1727 2.65798-4.17196-2.65798 4.17196-2.658zm1.4063-.88268 4.1814-2.664-4.1814-2.664-4.1821 2.664zm-6.9757-2.664-4.18144-2.664-4.18213 2.664 4.18213 2.664zm-4.81262 12.43736c.22254-.3494.68615-.4522 1.03551-.2297l5.17521 3.2966 5.1742-3.2965c.3493-.2226.813-.1198 1.0355.2295.2226.3494.1198.813-.2295 1.0355l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.57819-3.5532c-.34936-.2226-.45216-.6862-.22963-1.0355z";--icon-gdrive: "m7.73633 1.81806c.13459-.22968.38086-.37079.64707-.37079h7.587c.2718 0 .5223.14697.6548.38419l7.2327 12.94554c.1281.2293.1269.5089-.0031.7371l-3.7935 6.6594c-.1334.2342-.3822.3788-.6517.3788l-14.81918.0004c-.26952 0-.51831-.1446-.65171-.3788l-3.793526-6.6598c-.1327095-.233-.130949-.5191.004617-.7504zm.63943 1.87562-6.71271 11.45452 2.93022 5.1443 6.65493-11.58056zm3.73574 6.52652-2.39793 4.1727 4.78633.0001zm4.1168 4.1729 5.6967-.0002-6.3946-11.44563h-5.85354zm5.6844 1.4998h-13.06111l-2.96515 5.1598 13.08726-.0004z";--icon-gphotos: "M12.51 0c-.702 0-1.272.57-1.272 1.273V7.35A6.381 6.381 0 0 0 0 11.489c0 .703.57 1.273 1.273 1.273H7.35A6.381 6.381 0 0 0 11.488 24c.704 0 1.274-.57 1.274-1.273V16.65A6.381 6.381 0 0 0 24 12.51c0-.703-.57-1.273-1.273-1.273H16.65A6.381 6.381 0 0 0 12.511 0Zm.252 11.232V1.53a4.857 4.857 0 0 1 0 9.702Zm-1.53.006H1.53a4.857 4.857 0 0 1 9.702 0Zm1.536 1.524a4.857 4.857 0 0 0 9.702 0h-9.702Zm-6.136 4.857c0-2.598 2.04-4.72 4.606-4.85v9.7a4.857 4.857 0 0 1-4.606-4.85Z";--icon-instagram: "M6.225 12a5.775 5.775 0 1 1 11.55 0 5.775 5.775 0 0 1-11.55 0zM12 7.725a4.275 4.275 0 1 0 0 8.55 4.275 4.275 0 0 0 0-8.55zM18.425 6.975a1.4 1.4 0 1 0 0-2.8 1.4 1.4 0 0 0 0 2.8zM11.958.175h.084c2.152 0 3.823 0 5.152.132 1.35.134 2.427.41 3.362 1.013a7.15 7.15 0 0 1 2.124 2.124c.604.935.88 2.012 1.013 3.362.132 1.329.132 3 .132 5.152v.084c0 2.152 0 3.823-.132 5.152-.134 1.35-.41 2.427-1.013 3.362a7.15 7.15 0 0 1-2.124 2.124c-.935.604-2.012.88-3.362 1.013-1.329.132-3 .132-5.152.132h-.084c-2.152 0-3.824 0-5.153-.132-1.35-.134-2.427-.409-3.36-1.013a7.15 7.15 0 0 1-2.125-2.124C.716 19.62.44 18.544.307 17.194c-.132-1.329-.132-3-.132-5.152v-.084c0-2.152 0-3.823.132-5.152.133-1.35.409-2.427 1.013-3.362A7.15 7.15 0 0 1 3.444 1.32C4.378.716 5.456.44 6.805.307c1.33-.132 3-.132 5.153-.132zM6.953 1.799c-1.234.123-2.043.36-2.695.78A5.65 5.65 0 0 0 2.58 4.26c-.42.65-.657 1.46-.78 2.695C1.676 8.2 1.675 9.797 1.675 12c0 2.203 0 3.8.124 5.046.123 1.235.36 2.044.78 2.696a5.649 5.649 0 0 0 1.68 1.678c.65.421 1.46.658 2.694.78 1.247.124 2.844.125 5.047.125s3.8 0 5.046-.124c1.235-.123 2.044-.36 2.695-.78a5.648 5.648 0 0 0 1.68-1.68c.42-.65.657-1.46.78-2.694.123-1.247.124-2.844.124-5.047s-.001-3.8-.125-5.046c-.122-1.235-.359-2.044-.78-2.695a5.65 5.65 0 0 0-1.679-1.68c-.651-.42-1.46-.657-2.695-.78-1.246-.123-2.843-.124-5.046-.124-2.203 0-3.8 0-5.047.124z";--icon-flickr: "M5.95874 7.92578C3.66131 7.92578 1.81885 9.76006 1.81885 11.9994C1.81885 14.2402 3.66145 16.0744 5.95874 16.0744C8.26061 16.0744 10.1039 14.2396 10.1039 11.9994C10.1039 9.76071 8.26074 7.92578 5.95874 7.92578ZM0.318848 11.9994C0.318848 8.91296 2.85168 6.42578 5.95874 6.42578C9.06906 6.42578 11.6039 8.91232 11.6039 11.9994C11.6039 15.0877 9.06919 17.5744 5.95874 17.5744C2.85155 17.5744 0.318848 15.0871 0.318848 11.9994ZM18.3898 7.92578C16.0878 7.92578 14.2447 9.76071 14.2447 11.9994C14.2447 14.2396 16.088 16.0744 18.3898 16.0744C20.6886 16.0744 22.531 14.2401 22.531 11.9994C22.531 9.76019 20.6887 7.92578 18.3898 7.92578ZM12.7447 11.9994C12.7447 8.91232 15.2795 6.42578 18.3898 6.42578C21.4981 6.42578 24.031 8.91283 24.031 11.9994C24.031 15.0872 21.4982 17.5744 18.3898 17.5744C15.2794 17.5744 12.7447 15.0877 12.7447 11.9994Z";--icon-vk: var(--icon-external-source-placeholder);--icon-evernote: "M9.804 2.27v-.048c.055-.263.313-.562.85-.562h.44c.142 0 .325.014.526.033.066.009.124.023.267.06l.13.032h.002c.319.079.515.275.644.482a1.461 1.461 0 0 1 .16.356l.004.012a.75.75 0 0 0 .603.577l1.191.207a1988.512 1988.512 0 0 0 2.332.402c.512.083 1.1.178 1.665.442.64.3 1.19.795 1.376 1.77.548 2.931.657 5.829.621 8a39.233 39.233 0 0 1-.125 2.602 17.518 17.518 0 0 1-.092.849.735.735 0 0 0-.024.112c-.378 2.705-1.269 3.796-2.04 4.27-.746.457-1.53.451-2.217.447h-.192c-.46 0-1.073-.23-1.581-.635-.518-.412-.763-.87-.763-1.217 0-.45.188-.688.355-.786.161-.095.436-.137.796.087a.75.75 0 1 0 .792-1.274c-.766-.476-1.64-.52-2.345-.108-.7.409-1.098 1.188-1.098 2.08 0 .996.634 1.84 1.329 2.392.704.56 1.638.96 2.515.96l.185.002c.667.009 1.874.025 3.007-.67 1.283-.786 2.314-2.358 2.733-5.276.01-.039.018-.078.022-.105.011-.061.023-.14.034-.23.023-.184.051-.445.079-.772.055-.655.111-1.585.13-2.704.037-2.234-.074-5.239-.647-8.301v-.002c-.294-1.544-1.233-2.391-2.215-2.85-.777-.363-1.623-.496-2.129-.576-.097-.015-.18-.028-.25-.041l-.006-.001-1.99-.345-.761-.132a2.93 2.93 0 0 0-.182-.338A2.532 2.532 0 0 0 12.379.329l-.091-.023a3.967 3.967 0 0 0-.493-.103L11.769.2a7.846 7.846 0 0 0-.675-.04h-.44c-.733 0-1.368.284-1.795.742L2.416 7.431c-.468.428-.751 1.071-.751 1.81 0 .02 0 .041.003.062l.003.034c.017.21.038.468.096.796.107.715.275 1.47.391 1.994.029.13.055.245.075.342l.002.008c.258 1.141.641 1.94.978 2.466.168.263.323.456.444.589a2.808 2.808 0 0 0 .192.194c1.536 1.562 3.713 2.196 5.731 2.08.13-.005.35-.032.537-.073a2.627 2.627 0 0 0 .652-.24c.425-.26.75-.661.992-1.046.184-.294.342-.61.473-.915.197.193.412.357.627.493a5.022 5.022 0 0 0 1.97.709l.023.002.018.003.11.016c.088.014.205.035.325.058l.056.014c.088.022.164.04.235.061a1.736 1.736 0 0 1 .145.048l.03.014c.765.34 1.302 1.09 1.302 1.871a.75.75 0 0 0 1.5 0c0-1.456-.964-2.69-2.18-3.235-.212-.103-.5-.174-.679-.217l-.063-.015a10.616 10.616 0 0 0-.606-.105l-.02-.003-.03-.003h-.002a3.542 3.542 0 0 1-1.331-.485c-.471-.298-.788-.692-.828-1.234a.75.75 0 0 0-1.48-.106l-.001.003-.004.017a8.23 8.23 0 0 1-.092.352 9.963 9.963 0 0 1-.298.892c-.132.34-.29.68-.47.966-.174.276-.339.454-.478.549a1.178 1.178 0 0 1-.221.072 1.949 1.949 0 0 1-.241.036h-.013l-.032.002c-1.684.1-3.423-.437-4.604-1.65a.746.746 0 0 0-.053-.05L4.84 14.6a1.348 1.348 0 0 1-.07-.073 2.99 2.99 0 0 1-.293-.392c-.242-.379-.558-1.014-.778-1.985a54.1 54.1 0 0 0-.083-.376 27.494 27.494 0 0 1-.367-1.872l-.003-.02a6.791 6.791 0 0 1-.08-.67c.004-.277.086-.475.2-.609l.067-.067a.63.63 0 0 1 .292-.145h.05c.18 0 1.095.055 2.013.115l1.207.08.534.037a.747.747 0 0 0 .052.002c.782 0 1.349-.206 1.759-.585l.005-.005c.553-.52.622-1.225.622-1.76V6.24l-.026-.565A774.97 774.97 0 0 1 9.885 4.4c-.042-.961-.081-1.939-.081-2.13ZM4.995 6.953a251.126 251.126 0 0 1 2.102.137l.508.035c.48-.004.646-.122.715-.185.07-.068.146-.209.147-.649l-.024-.548a791.69 791.69 0 0 1-.095-2.187L4.995 6.953Zm16.122 9.996ZM15.638 11.626a.75.75 0 0 0 1.014.31 2.04 2.04 0 0 1 .304-.089 1.84 1.84 0 0 1 .544-.039c.215.023.321.06.37.085.033.016.039.026.047.04a.75.75 0 0 0 1.289-.767c-.337-.567-.906-.783-1.552-.85a3.334 3.334 0 0 0-1.002.062c-.27.056-.531.14-.705.234a.75.75 0 0 0-.31 1.014Z";--icon-box: "M1.01 4.148a.75.75 0 0 1 .75.75v4.348a4.437 4.437 0 0 1 2.988-1.153c1.734 0 3.23.992 3.978 2.438a4.478 4.478 0 0 1 3.978-2.438c2.49 0 4.488 2.044 4.488 4.543 0 2.5-1.999 4.544-4.488 4.544a4.478 4.478 0 0 1-3.978-2.438 4.478 4.478 0 0 1-3.978 2.438C2.26 17.18.26 15.135.26 12.636V4.898a.75.75 0 0 1 .75-.75Zm.75 8.488c0 1.692 1.348 3.044 2.988 3.044s2.989-1.352 2.989-3.044c0-1.691-1.349-3.043-2.989-3.043S1.76 10.945 1.76 12.636Zm10.944-3.043c-1.64 0-2.988 1.352-2.988 3.043 0 1.692 1.348 3.044 2.988 3.044s2.988-1.352 2.988-3.044c0-1.69-1.348-3.043-2.988-3.043Zm4.328-1.23a.75.75 0 0 1 1.052.128l2.333 2.983 2.333-2.983a.75.75 0 0 1 1.181.924l-2.562 3.277 2.562 3.276a.75.75 0 1 1-1.181.924l-2.333-2.983-2.333 2.983a.75.75 0 1 1-1.181-.924l2.562-3.276-2.562-3.277a.75.75 0 0 1 .129-1.052Z";--icon-onedrive: "M13.616 4.147a7.689 7.689 0 0 0-7.642 3.285A6.299 6.299 0 0 0 1.455 17.3c.684.894 2.473 2.658 5.17 2.658h12.141c.95 0 1.882-.256 2.697-.743.815-.486 1.514-1.247 1.964-2.083a5.26 5.26 0 0 0-3.713-7.612 7.69 7.69 0 0 0-6.098-5.373ZM3.34 17.15c.674.63 1.761 1.308 3.284 1.308h12.142a3.76 3.76 0 0 0 2.915-1.383l-7.494-4.489L3.34 17.15Zm10.875-6.25 2.47-1.038a5.239 5.239 0 0 1 1.427-.389 6.19 6.19 0 0 0-10.3-1.952 6.338 6.338 0 0 1 2.118.813l4.285 2.567Zm4.55.033c-.512 0-1.019.104-1.489.307l-.006.003-1.414.594 6.521 3.906a3.76 3.76 0 0 0-3.357-4.8l-.254-.01ZM4.097 9.617A4.799 4.799 0 0 1 6.558 8.9c.9 0 1.84.25 2.587.713l3.4 2.037-10.17 4.28a4.799 4.799 0 0 1 1.721-6.312Z";--icon-huddle: "M6.204 2.002c-.252.23-.357.486-.357.67V21.07c0 .15.084.505.313.812.208.28.499.477.929.477.519 0 .796-.174.956-.365.178-.212.286-.535.286-.924v-.013l.117-6.58c.004-1.725 1.419-3.883 3.867-3.883 1.33 0 2.332.581 2.987 1.364.637.762.95 1.717.95 2.526v6.47c0 .392.11.751.305.995.175.22.468.41 1.008.41.52 0 .816-.198 1.002-.437.207-.266.31-.633.31-.969V14.04c0-2.81-1.943-5.108-4.136-5.422a5.971 5.971 0 0 0-3.183.41c-.912.393-1.538.96-1.81 1.489a.75.75 0 0 1-1.417-.344v-7.5c0-.587-.47-1.031-1.242-1.031-.315 0-.638.136-.885.36ZM5.194.892A2.844 2.844 0 0 1 7.09.142c1.328 0 2.742.867 2.742 2.53v5.607a6.358 6.358 0 0 1 1.133-.629 7.47 7.47 0 0 1 3.989-.516c3.056.436 5.425 3.482 5.425 6.906v6.914c0 .602-.177 1.313-.627 1.89-.47.605-1.204 1.016-2.186 1.016-.96 0-1.698-.37-2.179-.973-.46-.575-.633-1.294-.633-1.933v-6.469c0-.456-.19-1.071-.602-1.563-.394-.471-.986-.827-1.836-.827-1.447 0-2.367 1.304-2.367 2.39v.014l-.117 6.58c-.001.64-.177 1.333-.637 1.881-.48.57-1.2.9-2.105.9-.995 0-1.7-.5-2.132-1.081-.41-.552-.61-1.217-.61-1.708V2.672c0-.707.366-1.341.847-1.78Z"}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-tabs{display:grid;grid-template-rows:min-content minmax(var(--ui-size),auto);height:100%;overflow:hidden;color:var(--clr-txt-lightest)}lr-tabs>.tabs-row{display:flex;grid-template-columns:minmax();background-color:var(--clr-background-light)}lr-tabs>.tabs-context{overflow-y:auto}lr-tabs .tabs-row>.tab{display:flex;flex-grow:1;align-items:center;justify-content:center;height:var(--ui-size);border-bottom:var(--border-light);cursor:pointer;transition:var(--transition-duration)}lr-tabs .tabs-row>.tab[current]{color:var(--clr-txt);border-color:var(--clr-txt)}lr-range{position:relative;display:inline-flex;align-items:center;justify-content:center;height:var(--ui-size)}lr-range datalist{display:none}lr-range input{width:100%;height:100%;opacity:0}lr-range .track-wrapper{position:absolute;right:10px;left:10px;display:flex;align-items:center;justify-content:center;height:2px;user-select:none;pointer-events:none}lr-range .track{position:absolute;right:0;left:0;display:flex;align-items:center;justify-content:center;height:2px;background-color:currentColor;border-radius:2px;opacity:.5}lr-range .slider{position:absolute;width:16px;height:16px;background-color:currentColor;border-radius:100%;transform:translate(-50%)}lr-range .bar{position:absolute;left:0;height:100%;background-color:currentColor;border-radius:2px}lr-range .caption{position:absolute;display:inline-flex;justify-content:center}lr-color{position:relative;display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size);overflow:hidden;background-color:var(--clr-background);cursor:pointer}lr-color[current]{background-color:var(--clr-txt)}lr-color input[type=color]{position:absolute;display:block;width:100%;height:100%;opacity:0}lr-color .current-color{position:absolute;width:50%;height:50%;border:2px solid #fff;border-radius:100%;pointer-events:none}lr-config{display:none}lr-simple-btn{position:relative;display:inline-flex}lr-simple-btn button{padding-left:.2em!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-simple-btn button lr-icon svg{transform:scale(.8)}lr-simple-btn button:hover{background-color:var(--clr-btn-bgr-secondary-hover)}lr-simple-btn button:active{background-color:var(--clr-btn-bgr-secondary-active)}lr-simple-btn>lr-drop-area{display:contents}lr-simple-btn .visual-drop-area{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;padding:var(--gap-min);border:var(--border-dashed);border-radius:inherit;opacity:0;transition:border-color var(--transition-duration) ease,background-color var(--transition-duration) ease,opacity var(--transition-duration) ease}lr-simple-btn .visual-drop-area:before{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;color:var(--clr-txt-light);background-color:var(--clr-background);border-radius:inherit;content:var(--l10n-drop-files-here)}lr-simple-btn>lr-drop-area[drag-state=active] .visual-drop-area{background-color:var(--clr-accent-lightest);opacity:1}lr-simple-btn>lr-drop-area[drag-state=inactive] .visual-drop-area{background-color:var(--clr-shade-lv1);opacity:0}lr-simple-btn>lr-drop-area[drag-state=near] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent-light);opacity:1}lr-simple-btn>lr-drop-area[drag-state=over] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent);opacity:1}lr-simple-btn>:where(lr-drop-area[drag-state=active],lr-drop-area[drag-state=near],lr-drop-area[drag-state=over]) button{box-shadow:none}lr-simple-btn>lr-drop-area:after{content:""}lr-source-btn{display:flex;align-items:center;margin-bottom:var(--gap-min);padding:var(--gap-min) var(--gap-mid);color:var(--clr-txt-mid);border-radius:var(--border-radius-element);cursor:pointer;transition-duration:var(--transition-duration);transition-property:background-color,color;user-select:none}lr-source-btn:hover{color:var(--clr-accent);background-color:var(--clr-accent-lightest)}lr-source-btn:active{color:var(--clr-accent);background-color:var(--clr-accent-light)}lr-source-btn lr-icon{display:inline-flex;flex-grow:1;justify-content:center;min-width:var(--ui-size);margin-right:var(--gap-mid);opacity:.8}lr-source-btn[type=local]>.txt:after{content:var(--l10n-local-files)}lr-source-btn[type=camera]>.txt:after{content:var(--l10n-camera)}lr-source-btn[type=url]>.txt:after{content:var(--l10n-from-url)}lr-source-btn[type=other]>.txt:after{content:var(--l10n-other)}lr-source-btn .txt{display:flex;align-items:center;box-sizing:border-box;width:100%;height:var(--ui-size);padding:0;white-space:nowrap;border:none}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-modal{--modal-max-content-height: calc(var(--uploadcare-blocks-window-height, 100vh) - 4 * var(--gap-mid) - var(--ui-size));--modal-content-height-fill: var(--uploadcare-blocks-window-height, 100vh)}lr-modal[dialog-fallback]{--lr-z-max: 2147483647;position:fixed;z-index:var(--lr-z-max);display:flex;align-items:center;justify-content:center;width:100vw;height:100vh;pointer-events:none;inset:0}lr-modal[dialog-fallback] dialog[open]{z-index:var(--lr-z-max);pointer-events:auto}lr-modal[dialog-fallback] dialog[open]+.backdrop{position:fixed;top:0;left:0;z-index:calc(var(--lr-z-max) - 1);align-items:center;justify-content:center;width:100vw;height:100vh;background-color:var(--clr-curtain);pointer-events:auto}lr-modal[strokes][dialog-fallback] dialog[open]+.backdrop{background-image:var(--modal-backdrop-background-image)}@supports selector(dialog::backdrop){lr-modal>dialog::backdrop{background-color:#0000001a}lr-modal[strokes]>dialog::backdrop{background-image:var(--modal-backdrop-background-image)}}lr-modal>dialog[open]{transform:translateY(0);visibility:visible;opacity:1}lr-modal>dialog:not([open]){transform:translateY(20px);visibility:hidden;opacity:0}lr-modal>dialog{display:flex;flex-direction:column;width:max-content;max-width:min(calc(100% - var(--gap-mid) * 2),calc(var(--modal-max-w) - var(--gap-mid) * 2));min-height:var(--ui-size);max-height:calc(var(--modal-max-h) - var(--gap-mid) * 2);margin:auto;padding:0;overflow:hidden;background-color:var(--clr-background-light);border:0;border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:transform calc(var(--transition-duration) * 2)}@media only screen and (max-width: 430px),only screen and (max-height: 600px){lr-modal>dialog>.content{height:var(--modal-max-content-height)}}lr-url-source{display:block;background-color:var(--clr-background-light)}lr-modal lr-url-source{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-url-source>.content{display:grid;grid-gap:var(--gap-small);grid-template-columns:1fr min-content;padding:var(--gap-mid);padding-top:0}lr-url-source .url-input{display:flex}lr-url-source .url-upload-btn:after{content:var(--l10n-upload-url)}lr-camera-source{position:relative;display:flex;flex-direction:column;width:100%;height:100%;max-height:100%;overflow:hidden;background-color:var(--clr-background-light);border-radius:var(--border-radius-element)}lr-modal lr-camera-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:100vh;max-height:var(--modal-max-content-height)}lr-camera-source.initialized{height:max-content}@media only screen and (max-width: 430px){lr-camera-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-camera-source video{display:block;width:100%;max-height:100%;object-fit:contain;object-position:center center;background-color:var(--clr-background-dark);border-radius:var(--border-radius-element)}lr-camera-source .toolbar{position:absolute;bottom:0;display:flex;justify-content:space-between;width:100%;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-camera-source .content{display:flex;flex:1;justify-content:center;width:100%;padding:var(--gap-mid);padding-top:0;overflow:hidden}lr-camera-source .message-box{--padding: calc(var(--gap-max) * 2);display:flex;flex-direction:column;grid-gap:var(--gap-max);align-items:center;justify-content:center;padding:var(--padding) var(--padding) 0 var(--padding);color:var(--clr-txt)}lr-camera-source .message-box button{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary)}lr-camera-source .shot-btn{position:absolute;bottom:var(--gap-max);width:calc(var(--ui-size) * 1.8);height:calc(var(--ui-size) * 1.8);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;opacity:.85;transition:var(--transition-duration) ease}lr-camera-source .shot-btn:hover{transform:scale(1.05);opacity:1}lr-camera-source .shot-btn:active{background-color:var(--clr-txt-mid);opacity:1}lr-camera-source .shot-btn[disabled]{bottom:calc(var(--gap-max) * -1 - var(--gap-mid) - var(--ui-size) * 2)}lr-camera-source .shot-btn lr-icon svg{width:calc(var(--ui-size) / 1.5);height:calc(var(--ui-size) / 1.5)}lr-external-source{display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--clr-background-light);overflow:hidden}lr-modal lr-external-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height)}lr-external-source>.content{position:relative;display:grid;flex:1;grid-template-rows:1fr min-content}@media only screen and (max-width: 430px){lr-external-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-external-source iframe{display:block;width:100%;height:100%;border:none}lr-external-source .iframe-wrapper{overflow:hidden}lr-external-source .toolbar{display:grid;grid-gap:var(--gap-mid);grid-template-columns:max-content 1fr max-content max-content;align-items:center;width:100%;padding:var(--gap-mid);border-top:var(--border-light)}lr-external-source .back-btn{padding-left:0}lr-external-source .back-btn:after{content:var(--l10n-back)}lr-external-source .selected-counter{display:flex;grid-gap:var(--gap-mid);align-items:center;justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt-light)}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-upload-details{display:flex;flex-direction:column;width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height);overflow:hidden;background-color:var(--clr-background-light)}lr-upload-details>.content{position:relative;display:grid;flex:1;grid-template-rows:auto min-content}lr-upload-details lr-tabs .tabs-context{position:relative}lr-upload-details .toolbar{display:grid;grid-template-columns:min-content min-content 1fr min-content;gap:var(--gap-mid);padding:var(--gap-mid);border-top:var(--border-light)}lr-upload-details .toolbar[edit-disabled]{display:flex;justify-content:space-between}lr-upload-details .remove-btn{padding-left:.5em}lr-upload-details .detail-btn{padding-left:0;color:var(--clr-txt);background-color:var(--clr-background)}lr-upload-details .edit-btn{padding-left:.5em}lr-upload-details .details{padding:var(--gap-max)}lr-upload-details .info-block{padding-top:var(--gap-max);padding-bottom:calc(var(--gap-max) + var(--gap-table));color:var(--clr-txt);border-bottom:var(--border-light)}lr-upload-details .info-block:first-of-type{padding-top:0}lr-upload-details .info-block:last-of-type{border-bottom:none}lr-upload-details .info-block>.info-block_name{margin-bottom:.4em;color:var(--clr-txt-light);font-size:.8em}lr-upload-details .cdn-link[disabled]{pointer-events:none}lr-upload-details .cdn-link[disabled]:before{filter:grayscale(1);content:var(--l10n-not-uploaded-yet)}lr-file-preview{position:absolute;inset:0;display:flex;align-items:center;justify-content:center}lr-file-preview>lr-img{display:contents}lr-file-preview>lr-img>.img-view{position:absolute;inset:0;width:100%;max-width:100%;height:100%;max-height:100%;object-fit:scale-down}lr-confirmation-dialog{display:block;padding:var(--gap-mid);padding-top:var(--gap-max)}lr-confirmation-dialog .message{display:flex;justify-content:center;padding:var(--gap-mid);padding-bottom:var(--gap-max);font-weight:500;font-size:1.1em}lr-confirmation-dialog .toolbar{display:grid;grid-template-columns:1fr 1fr;gap:var(--gap-mid);margin-top:var(--gap-mid)}lr-progress-bar-common{position:fixed;right:0;bottom:0;left:0;z-index:10000;display:block;height:var(--gap-mid);background-color:var(--clr-background);transition:opacity .3s}lr-progress-bar-common:not([active]){opacity:0;pointer-events:none}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--unknown{width:100%;transform-origin:0% 50%;animation:lr-indeterminateAnimation 1s infinite linear}lr-progress-bar .progress--hidden{opacity:0}@keyframes lr-indeterminateAnimation{0%{transform:translate(0) scaleX(0)}40%{transform:translate(0) scaleX(.4)}to{transform:translate(100%) scaleX(.5)}}lr-activity-header{display:flex;gap:var(--gap-mid);justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt);font-weight:500;font-size:1em;line-height:var(--ui-size)}lr-activity-header lr-icon{height:var(--ui-size)}lr-activity-header>*{display:flex;align-items:center}lr-activity-header button{display:inline-flex;align-items:center;justify-content:center;color:var(--clr-txt-mid)}lr-activity-header button:hover{background-color:var(--clr-background)}lr-activity-header button:active{background-color:var(--clr-background-dark)}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:host(.lr-cloud-image-editor) lr-icon,.lr-cloud-image-editor lr-icon{display:flex;align-items:center;justify-content:center;width:100%;height:100%}:host(.lr-cloud-image-editor) lr-icon svg,.lr-cloud-image-editor lr-icon svg{width:unset;height:unset}:host(.lr-cloud-image-editor) lr-icon:not([raw]) path,.lr-cloud-image-editor lr-icon:not([raw]) path{stroke-linejoin:round;fill:none;stroke:currentColor;stroke-width:1.2}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--icon-rotate: "M13.5.399902L12 1.9999l1.5 1.6M12.0234 2H14.4C16.3882 2 18 3.61178 18 5.6V8M4 17h9c.5523 0 1-.4477 1-1V7c0-.55228-.4477-1-1-1H4c-.55228 0-1 .44771-1 1v9c0 .5523.44771 1 1 1z";--icon-mirror: "M5.00042.399902l-1.5 1.599998 1.5 1.6M15.0004.399902l1.5 1.599998-1.5 1.6M3.51995 2H16.477M8.50042 16.7V6.04604c0-.30141-.39466-.41459-.5544-.159L1.28729 16.541c-.12488.1998.01877.459.2544.459h6.65873c.16568 0 .3-.1343.3-.3zm2.99998 0V6.04604c0-.30141.3947-.41459.5544-.159L18.7135 16.541c.1249.1998-.0187.459-.2544.459h-6.6587c-.1657 0-.3-.1343-.3-.3z";--icon-flip: "M19.6001 4.99993l-1.6-1.5-1.6 1.5m3.2 9.99997l-1.6 1.5-1.6-1.5M18 3.52337V16.4765M3.3 8.49993h10.654c.3014 0 .4146-.39466.159-.5544L3.459 1.2868C3.25919 1.16192 3 1.30557 3 1.5412v6.65873c0 .16568.13432.3.3.3zm0 2.99997h10.654c.3014 0 .4146.3947.159.5544L3.459 18.7131c-.19981.1248-.459-.0188-.459-.2544v-6.6588c0-.1657.13432-.3.3-.3z";--icon-sad: "M2 17c4.41828-4 11.5817-4 16 0M16.5 5c0 .55228-.4477 1-1 1s-1-.44772-1-1 .4477-1 1-1 1 .44772 1 1zm-11 0c0 .55228-.44772 1-1 1s-1-.44772-1-1 .44772-1 1-1 1 .44772 1 1z";--icon-closeMax: "M3 3l14 14m0-14L3 17";--icon-crop: "M20 14H7.00513C6.45001 14 6 13.55 6 12.9949V0M0 6h13.0667c.5154 0 .9333.41787.9333.93333V20M14.5.399902L13 1.9999l1.5 1.6M13 2h2c1.6569 0 3 1.34315 3 3v2M5.5 19.5999l1.5-1.6-1.5-1.6M7 18H5c-1.65685 0-3-1.3431-3-3v-2";--icon-tuning: "M8 10h11M1 10h4M1 4.5h11m3 0h4m-18 11h11m3 0h4M12 4.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M5 10a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M12 15.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0";--icon-filters: "M4.5 6.5a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m-3.5 6a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m7 0a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0";--icon-done: "M1 10.6316l5.68421 5.6842L19 4";--icon-original: "M0 40L40-.00000133";--icon-slider: "M0 10h11m0 0c0 1.1046.8954 2 2 2s2-.8954 2-2m-4 0c0-1.10457.8954-2 2-2s2 .89543 2 2m0 0h5";--icon-exposure: "M10 20v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M5 10a5 5 0 1010 0 5 5 0 10-10 0";--icon-contrast: "M2 10a8 8 0 1016 0 8 8 0 10-16 0m8-8v16m8-8h-8m7.5977 2.5H10m6.24 2.5H10m7.6-7.5H10M16.2422 5H10";--icon-brightness: "M15 10c0 2.7614-2.2386 5-5 5m5-5c0-2.76142-2.2386-5-5-5m5 5h-5m0 5c-2.76142 0-5-2.2386-5-5 0-2.76142 2.23858-5 5-5m0 10V5m0 15v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M14.3242 7.5H10m4.3242 5H10";--icon-gamma: "M17 3C9 6 2.5 11.5 2.5 17.5m0 0h1m-1 0v-1m14 1h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3-14v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1";--icon-enhance: "M19 13h-2m0 0c-2.2091 0-4-1.7909-4-4m4 4c-2.2091 0-4 1.7909-4 4m0-8V7m0 2c0 2.2091-1.7909 4-4 4m-2 0h2m0 0c2.2091 0 4 1.7909 4 4m0 0v2M8 8.5H6.5m0 0c-1.10457 0-2-.89543-2-2m2 2c-1.10457 0-2 .89543-2 2m0-4V5m0 1.5c0 1.10457-.89543 2-2 2M1 8.5h1.5m0 0c1.10457 0 2 .89543 2 2m0 0V12M12 3h-1m0 0c-.5523 0-1-.44772-1-1m1 1c-.5523 0-1 .44772-1 1m0-2V1m0 1c0 .55228-.44772 1-1 1M8 3h1m0 0c.55228 0 1 .44772 1 1m0 0v1";--icon-saturation: '    <circle cx="10.0006" cy="10.0001" r="9" transform="rotate(90 10.0006 10.0001)" fill="url(#paint0_linear)"/>     <defs>       <linearGradient id="paint0_linear" x1="10.0006" y1="1.00009" x2="10.0006" y2="19.0001" gradientUnits="userSpaceOnUse">         <stop stop-color="#DE15FF"/>         <stop offset=".203125" stop-color="#0029FF"/>         <stop offset=".479167" stop-color="#2AE4F0"/>         <stop offset=".604167" stop-color="#15EF11"/>         <stop offset=".75" stop-color="#FAE528"/>         <stop offset="1" stop-color="#EB2A2A"/>       </linearGradient>     </defs>  ';--icon-warmth: '    <path d="M7.5 13.0505l.42854.4199.17146-.1749v-.245h-.6zm5 0h-.6v.245l.1715.1749.4285-.4199zM8.1 3.5c0-1.04934.85066-1.9 1.9-1.9V.4C8.28792.4 6.9 1.78792 6.9 3.5h1.2zm0 9.5505V3.5H6.9v9.5505h1.2zM7.1 15.5c0-.7904.31539-1.5059.82854-2.0296l-.85708-.8398C6.34742 13.3694 5.9 14.3831 5.9 15.5h1.2zm2.9 2.9c-1.60163 0-2.9-1.2984-2.9-2.9H5.9c0 2.2644 1.83563 4.1 4.1 4.1v-1.2zm2.9-2.9c0 1.6016-1.2984 2.9-2.9 2.9v1.2c2.2644 0 4.1-1.8356 4.1-4.1h-1.2zm-.8285-2.0296c.5131.5237.8285 1.2392.8285 2.0296h1.2c0-1.1169-.4474-2.1306-1.1715-2.8694l-.857.8398zM11.9 3.5v9.5505h1.2V3.5h-1.2zM10 1.6c1.0493 0 1.9.85066 1.9 1.9h1.2c0-1.71208-1.3879-3.1-3.1-3.1v1.2z" fill="currentColor"/>    <path d="M10 14V8" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/>    <path d="M14 3h3m-3 3h3m-3 3h3m-8 6.5a1 1 0 102 0 1 1 0 10-2 0" stroke="currentColor" stroke-width="1.2"/>  ';--icon-vibrance: '  <path d="M2.125 5.6407c-.71643 1.29152-1.12439 2.77782-1.12439 4.3594 0 1.5816.40796 3.0679 1.12439 4.3594V5.6407z" fill="url(#paint0_linear)"/>  <path d="M2.875 15.4986V4.5016c.50222-.64987 1.09136-1.22915 1.75-1.72041V17.219c-.65864-.4912-1.24778-1.0705-1.75-1.7204z" fill="url(#paint1_linear)"/>  <path d="M5.375 17.722c.54811.3291 1.13415.6014 1.75.8089V1.46929c-.61585.20751-1.20189.47984-1.75.80888V17.722z" fill="url(#paint2_linear)"/>  <path d="M7.875 1.25258V18.7476c.56442.1367 1.14962.2202 1.75.2448V1.0078c-.60038.02465-1.18558.10811-1.75.24478z" fill="url(#paint3_linear)"/>  <path d="M10.375 1.00775V18.9925c.6004-.0246 1.1856-.108 1.75-.2446V1.25228c-.5644-.13658-1.1496-.21996-1.75-.24453z" fill="url(#paint4_linear)"/>  <path d="M12.875 1.46887V18.5313c.6158-.2074 1.2019-.4796 1.75-.8085V2.27744c-.5481-.32893-1.1342-.60115-1.75-.80857z" fill="url(#paint5_linear)"/>  <path d="M15.375 2.78028V17.2199c.6586-.491 1.2477-1.0701 1.75-1.7197V4.50002c-.5023-.64963-1.0914-1.22868-1.75-1.71974z" fill="url(#paint6_linear)"/>  <path d="M17.875 5.6385v8.7232c.7172-1.292 1.1256-2.7791 1.1256-4.3616 0-1.58248-.4084-3.06956-1.1256-4.3616z" fill="url(#paint7_linear)"/>  <defs>    <linearGradient id="paint0_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint1_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint2_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint3_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint4_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint5_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint6_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint7_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>  </defs>  '}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--l10n-cancel: "Cancel";--l10n-apply: "Apply";--l10n-brightness: "Brightness";--l10n-exposure: "Exposure";--l10n-gamma: "Gamma";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-vibrance: "Vibrance";--l10n-warmth: "Warmth";--l10n-enhance: "Enhance";--l10n-original: "Original"}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--rgb-primary-accent: 6, 2, 196;--rgb-text-base: 0, 0, 0;--rgb-text-accent-contrast: 255, 255, 255;--rgb-fill-contrast: 255, 255, 255;--rgb-fill-shaded: 245, 245, 245;--rgb-shadow: 0, 0, 0;--rgb-error: 209, 81, 81;--opacity-shade-mid: .2;--color-primary-accent: rgb(var(--rgb-primary-accent));--color-text-base: rgb(var(--rgb-text-base));--color-text-accent-contrast: rgb(var(--rgb-text-accent-contrast));--color-text-soft: rgb(var(--rgb-fill-contrast));--color-text-error: rgb(var(--rgb-error));--color-fill-contrast: rgb(var(--rgb-fill-contrast));--color-modal-backdrop: rgba(var(--rgb-fill-shaded), .95);--color-image-background: rgba(var(--rgb-fill-shaded));--color-outline: rgba(var(--rgb-text-base), var(--opacity-shade-mid));--color-underline: rgba(var(--rgb-text-base), .08);--color-shade: rgba(var(--rgb-text-base), .02);--color-focus-ring: var(--color-primary-accent);--color-input-placeholder: rgba(var(--rgb-text-base), .32);--color-error: rgb(var(--rgb-error));--font-size-ui: 16px;--font-size-title: 18px;--font-weight-title: 500;--font-size-soft: 14px;--size-touch-area: 40px;--size-panel-heading: 66px;--size-ui-min-width: 130px;--size-line-width: 1px;--size-modal-width: 650px;--border-radius-connect: 2px;--border-radius-editor: 3px;--border-radius-thumb: 4px;--border-radius-ui: 5px;--border-radius-base: 6px;--cldtr-gap-min: 5px;--cldtr-gap-mid-1: 10px;--cldtr-gap-mid-2: 15px;--cldtr-gap-max: 20px;--opacity-min: var(--opacity-shade-mid);--opacity-mid: .1;--opacity-max: .05;--transition-duration-2: var(--transition-duration-all, .2s);--transition-duration-3: var(--transition-duration-all, .3s);--transition-duration-4: var(--transition-duration-all, .4s);--transition-duration-5: var(--transition-duration-all, .5s);--shadow-base: 0px 5px 15px rgba(var(--rgb-shadow), .1), 0px 1px 4px rgba(var(--rgb-shadow), .15);--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading);--transparent-pixel: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=);display:block;width:100%;height:100%;max-height:100%}:host(.lr-cloud-image-editor) :is([can-handle-paste]:hover,[can-handle-paste]:focus),.lr-cloud-image-editor :is([can-handle-paste]:hover,[can-handle-paste]:focus){--can-handle-paste: "true"}:host(.lr-cloud-image-editor) :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover),.lr-cloud-image-editor :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover){--filter-effect: var(--hover-filter) !important;--opacity-effect: var(--hover-opacity) !important;--color-effect: var(--hover-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex]:active,[with-effects]:active),.lr-cloud-image-editor :is([tabindex]:active,[with-effects]:active){--filter-effect: var(--down-filter) !important;--opacity-effect: var(--down-opacity) !important;--color-effect: var(--down-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex][active],[with-effects][active]),.lr-cloud-image-editor :is([tabindex][active],[with-effects][active]){--filter-effect: var(--active-filter) !important;--opacity-effect: var(--active-opacity) !important;--color-effect: var(--active-color-rgb) !important}:host(.lr-cloud-image-editor) [hidden-scrollbar]::-webkit-scrollbar,.lr-cloud-image-editor [hidden-scrollbar]::-webkit-scrollbar{display:none}:host(.lr-cloud-image-editor) [hidden-scrollbar],.lr-cloud-image-editor [hidden-scrollbar]{-ms-overflow-style:none;scrollbar-width:none}:host(.lr-cloud-image-editor.editor_ON),.lr-cloud-image-editor.editor_ON{--modal-header-opacity: 0;--modal-header-height: 0px;--modal-toolbar-height: calc(var(--size-panel-heading) * 2)}:host(.lr-cloud-image-editor.editor_OFF),.lr-cloud-image-editor.editor_OFF{--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading)}:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-min-img-height: var(--modal-toolbar-height);--l-max-img-height: 100%;--l-edit-button-width: 120px;--l-toolbar-horizontal-padding: var(--cldtr-gap-mid-1);position:relative;display:grid;grid-template-rows:minmax(var(--l-min-img-height),var(--l-max-img-height)) minmax(var(--modal-toolbar-height),auto);height:100%;overflow:hidden;overflow-y:auto}@media only screen and (max-width: 800px){:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-edit-button-width: 70px;--l-toolbar-horizontal-padding: var(--cldtr-gap-min)}}:host(.lr-cloud-image-editor)>.wrapper>.viewport,.lr-cloud-image-editor>.wrapper>.viewport{display:flex;align-items:center;justify-content:center;overflow:hidden}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image{--viewer-image-opacity: 1;position:absolute;top:0;left:0;z-index:10;display:block;box-sizing:border-box;width:100%;height:100%;object-fit:scale-down;background-color:var(--color-image-background);transform:scale(1);opacity:var(--viewer-image-opacity);user-select:none;pointer-events:auto}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_visible_viewer,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_visible_viewer{transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-4)}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper{--viewer-image-opacity: 0;background-image:var(--transparent-pixel);transform:scale(1);transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_effects,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_effects{--viewer-image-opacity: 0;transform:scale(1);transition:opacity var(--transition-duration-3) cubic-bezier(.5,0,1,1),transform var(--transition-duration-4);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container,.lr-cloud-image-editor>.wrapper>.viewport>.image_container{position:relative;display:block;width:100%;height:100%;background-color:var(--color-image-background);transition:var(--transition-duration-3)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar,.lr-cloud-image-editor>.wrapper>.toolbar{position:relative;transition:.3s}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content{position:absolute;bottom:0;left:0;box-sizing:border-box;width:100%;height:var(--modal-toolbar-height);min-height:var(--size-panel-heading);background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer{display:flex;align-items:center;justify-content:space-between;height:var(--size-panel-heading);padding-right:var(--l-toolbar-horizontal-padding);padding-left:var(--l-toolbar-horizontal-padding)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor{display:flex}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.info_pan,.lr-cloud-image-editor>.wrapper>.viewport>.info_pan{position:absolute;user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer{position:absolute;z-index:2;display:flex;max-width:120px;transform:translate(-40px);user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer>.file_type,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer>.file_type{padding:4px .8em}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash,.lr-cloud-image-editor>.wrapper>.network_problems_splash{position:absolute;z-index:4;display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content{display:flex;flex:1;flex-direction:column;align-items:center;justify-content:center}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon{display:flex;align-items:center;justify-content:center;width:40px;height:40px;color:rgba(var(--rgb-text-base),.6);background-color:rgba(var(--rgb-fill-shaded));border-radius:50%}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text{margin-top:var(--cldtr-gap-max);font-size:var(--font-size-ui)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_footer,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_footer{display:flex;align-items:center;justify-content:center;height:var(--size-panel-heading)}lr-crop-frame>.svg{position:absolute;top:0;left:0;z-index:2;width:100%;height:100%;border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);opacity:inherit;transition:var(--transition-duration-3)}lr-crop-frame>.thumb{--idle-color-rgb: var(--color-text-base);--hover-color-rgb: var(--color-primary-accent);--focus-color-rgb: var(--color-primary-accent);--down-color-rgb: var(--color-primary-accent);--color-effect: var(--idle-color-rgb);color:var(--color-effect);transition:color var(--transition-duration-3),opacity var(--transition-duration-3)}lr-crop-frame>.thumb--visible{opacity:1;pointer-events:auto}lr-crop-frame>.thumb--hidden{opacity:0;pointer-events:none}lr-crop-frame>.guides{transition:var(--transition-duration-3)}lr-crop-frame>.guides--hidden{opacity:0}lr-crop-frame>.guides--semi-hidden{opacity:.2}lr-crop-frame>.guides--visible{opacity:1}lr-editor-button-control,lr-editor-crop-button-control,lr-editor-filter-control,lr-editor-operation-control{--l-base-min-width: 40px;--l-base-height: var(--l-base-min-width);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--filter-effect: var(--idle-filter);--idle-color-rgb: var(--rgb-text-base);--idle-opacity: .05;--idle-filter: 1;--hover-color-rgb: var(--idle-color-rgb);--hover-opacity: .08;--hover-filter: .8;--down-color-rgb: var(--hover-color-rgb);--down-opacity: .12;--down-filter: .6;position:relative;display:grid;grid-template-columns:var(--l-base-min-width) auto;align-items:center;height:var(--l-base-height);color:rgba(var(--idle-color-rgb));outline:none;cursor:pointer;transition:var(--l-width-transition)}lr-editor-button-control.active,lr-editor-operation-control.active,lr-editor-crop-button-control.active,lr-editor-filter-control.active{--idle-color-rgb: var(--rgb-primary-accent)}lr-editor-filter-control.not_active .preview[loaded]{opacity:1}lr-editor-filter-control.active .preview{opacity:0}lr-editor-button-control.not_active,lr-editor-operation-control.not_active,lr-editor-crop-button-control.not_active,lr-editor-filter-control.not_active{--idle-color-rgb: var(--rgb-text-base)}lr-editor-button-control>.before,lr-editor-operation-control>.before,lr-editor-crop-button-control>.before,lr-editor-filter-control>.before{position:absolute;right:0;left:0;z-index:-1;width:100%;height:100%;background-color:rgba(var(--color-effect),var(--opacity-effect));border-radius:var(--border-radius-editor);transition:var(--transition-duration-3)}lr-editor-button-control>.title,lr-editor-operation-control>.title,lr-editor-crop-button-control>.title,lr-editor-filter-control>.title{padding-right:var(--cldtr-gap-mid-1);font-size:.7em;letter-spacing:1.004px;text-transform:uppercase}lr-editor-filter-control>.preview{position:absolute;right:0;left:0;z-index:1;width:100%;height:var(--l-base-height);background-repeat:no-repeat;background-size:contain;border-radius:var(--border-radius-editor);opacity:0;filter:brightness(var(--filter-effect));transition:var(--transition-duration-3)}lr-editor-filter-control>.original-icon{color:var(--color-text-base);opacity:.3}lr-editor-image-cropper{position:absolute;top:0;left:0;z-index:10;display:block;width:100%;height:100%;opacity:0;pointer-events:none;touch-action:none}lr-editor-image-cropper.active_from_editor{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.active_from_viewer{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.inactive_to_editor{opacity:0;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1),opacity var(--transition-duration-3) calc(var(--transition-duration-3) + .05s);pointer-events:none}lr-editor-image-cropper>.canvas{position:absolute;top:0;left:0;z-index:1;display:block;width:100%;height:100%}lr-editor-image-fader{position:absolute;top:0;left:0;display:block;width:100%;height:100%}lr-editor-image-fader.active_from_viewer{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-start);pointer-events:auto}lr-editor-image-fader.active_from_cropper{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:auto}lr-editor-image-fader.inactive_to_cropper{z-index:3;transform:scale(1);opacity:0;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}lr-editor-image-fader .fader-image{position:absolute;top:0;left:0;display:block;width:100%;height:100%;object-fit:scale-down;transform:scale(1);user-select:none;content-visibility:auto}lr-editor-image-fader .fader-image--preview{background-color:var(--color-image-background);border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);transform:scale(1);opacity:0;transition:var(--transition-duration-3)}lr-editor-scroller{display:flex;align-items:center;width:100%;height:100%;overflow-x:scroll}lr-editor-slider{display:flex;align-items:center;justify-content:center;width:100%;height:66px}lr-editor-toolbar{position:relative;width:100%;height:100%}@media only screen and (max-width: 600px){lr-editor-toolbar{--l-tab-gap: var(--cldtr-gap-mid-1);--l-slider-padding: var(--cldtr-gap-min);--l-controls-padding: var(--cldtr-gap-min)}}@media only screen and (min-width: 601px){lr-editor-toolbar{--l-tab-gap: calc(var(--cldtr-gap-mid-1) + var(--cldtr-gap-max));--l-slider-padding: var(--cldtr-gap-mid-1);--l-controls-padding: var(--cldtr-gap-mid-1)}}lr-editor-toolbar>.toolbar-container{position:relative;width:100%;height:100%;overflow:hidden}lr-editor-toolbar>.toolbar-container>.sub-toolbar{position:absolute;display:grid;grid-template-rows:1fr 1fr;width:100%;height:100%;background-color:var(--color-fill-contrast);transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-3) ease-in-out,visibility var(--transition-duration-3) ease-in-out}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--visible{transform:translateY(0);opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--top-hidden{transform:translateY(100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--bottom-hidden{transform:translateY(-100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row{display:flex;align-items:center;justify-content:space-between;padding-right:var(--l-controls-padding);padding-left:var(--l-controls-padding)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles{position:relative;display:grid;grid-auto-flow:column;grid-gap:0px var(--l-tab-gap);align-items:center;height:100%}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggles_indicator{position:absolute;bottom:0;left:0;width:var(--size-touch-area);height:2px;background-color:var(--color-primary-accent);transform:translate(0);transition:transform var(--transition-duration-3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row{position:relative}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content{position:absolute;top:0;left:0;display:flex;width:100%;height:100%;overflow:hidden;opacity:0;content-visibility:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--visible{opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--hidden{opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--visible{display:contents}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles.tab-toggles--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_align{display:grid;grid-template-areas:". inner .";grid-template-columns:1fr auto 1fr;box-sizing:border-box;min-width:100%;padding-left:var(--cldtr-gap-max)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner{display:grid;grid-area:inner;grid-auto-flow:column;grid-gap:calc((var(--cldtr-gap-min) - 1px) * 3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner:last-child{padding-right:var(--cldtr-gap-max)}lr-editor-toolbar .controls-list_last-item{margin-right:var(--cldtr-gap-max)}lr-editor-toolbar .info-tooltip_container{position:absolute;display:flex;align-items:flex-start;justify-content:center;width:100%;height:100%}lr-editor-toolbar .info-tooltip_wrapper{position:absolute;top:calc(-100% - var(--cldtr-gap-mid-2));display:flex;flex-direction:column;justify-content:flex-end;height:100%;pointer-events:none}lr-editor-toolbar .info-tooltip{z-index:3;padding-top:calc(var(--cldtr-gap-min) / 2);padding-right:var(--cldtr-gap-min);padding-bottom:calc(var(--cldtr-gap-min) / 2);padding-left:var(--cldtr-gap-min);color:var(--color-text-base);font-size:.7em;letter-spacing:1px;text-transform:uppercase;background-color:var(--color-text-accent-contrast);border-radius:var(--border-radius-editor);transform:translateY(100%);opacity:0;transition:var(--transition-duration-3)}lr-editor-toolbar .info-tooltip_visible{transform:translateY(0);opacity:1}lr-editor-toolbar .slider{padding-right:var(--l-slider-padding);padding-left:var(--l-slider-padding)}lr-btn-ui{--filter-effect: var(--idle-brightness);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--l-transition-effect: var(--css-transition, color var(--transition-duration-2), filter var(--transition-duration-2));display:inline-flex;align-items:center;box-sizing:var(--css-box-sizing, border-box);height:var(--css-height, var(--size-touch-area));padding-right:var(--css-padding-right, var(--cldtr-gap-mid-1));padding-left:var(--css-padding-left, var(--cldtr-gap-mid-1));color:rgba(var(--color-effect),var(--opacity-effect));outline:none;cursor:pointer;filter:brightness(var(--filter-effect));transition:var(--l-transition-effect);user-select:none}lr-btn-ui .text{white-space:nowrap}lr-btn-ui .icon{display:flex;align-items:center;justify-content:center;color:rgba(var(--color-effect),var(--opacity-effect));filter:brightness(var(--filter-effect));transition:var(--l-transition-effect)}lr-btn-ui .icon_left{margin-right:var(--cldtr-gap-mid-1);margin-left:0}lr-btn-ui .icon_right{margin-right:0;margin-left:var(--cldtr-gap-mid-1)}lr-btn-ui .icon_single{margin-right:0;margin-left:0}lr-btn-ui .icon_hidden{display:none;margin:0}lr-btn-ui.primary{--idle-color-rgb: var(--rgb-primary-accent);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--idle-color-rgb);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.boring{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-text-base);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: 1;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.default{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-primary-accent);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-line-loader-ui{position:absolute;top:0;left:0;z-index:9999;width:100%;height:2px;opacity:.5}lr-line-loader-ui .inner{width:25%;max-width:200px;height:100%}lr-line-loader-ui .line{width:100%;height:100%;background-color:var(--color-primary-accent);transform:translate(-101%);transition:transform 1s}lr-slider-ui{--l-thumb-size: 24px;--l-zero-dot-size: 5px;--l-zero-dot-offset: 2px;--idle-color-rgb: var(--rgb-text-base);--hover-color-rgb: var(--rgb-primary-accent);--down-color-rgb: var(--rgb-primary-accent);--color-effect: var(--idle-color-rgb);--l-color: rgb(var(--color-effect));position:relative;display:flex;align-items:center;justify-content:center;width:100%;height:calc(var(--l-thumb-size) + (var(--l-zero-dot-size) + var(--l-zero-dot-offset)) * 2)}lr-slider-ui .thumb{position:absolute;left:0;width:var(--l-thumb-size);height:var(--l-thumb-size);background-color:var(--l-color);border-radius:50%;transform:translate(0);opacity:1;transition:opacity var(--transition-duration-2)}lr-slider-ui .steps{position:absolute;display:flex;align-items:center;justify-content:space-between;box-sizing:border-box;width:100%;height:100%;padding-right:calc(var(--l-thumb-size) / 2);padding-left:calc(var(--l-thumb-size) / 2)}lr-slider-ui .border-step{width:0px;height:10px;border-right:1px solid var(--l-color);opacity:.6;transition:var(--transition-duration-2)}lr-slider-ui .minor-step{width:0px;height:4px;border-right:1px solid var(--l-color);opacity:.2;transition:var(--transition-duration-2)}lr-slider-ui .zero-dot{position:absolute;top:calc(100% - var(--l-zero-dot-offset) * 2);left:calc(var(--l-thumb-size) / 2 - var(--l-zero-dot-size) / 2);width:var(--l-zero-dot-size);height:var(--l-zero-dot-size);background-color:var(--color-primary-accent);border-radius:50%;opacity:0;transition:var(--transition-duration-3)}lr-slider-ui .input{position:absolute;width:calc(100% - 10px);height:100%;margin:0;cursor:pointer;opacity:0}lr-presence-toggle.transition{transition:opacity var(--transition-duration-3),visibility var(--transition-duration-3)}lr-presence-toggle.visible{opacity:1;pointer-events:inherit}lr-presence-toggle.hidden{opacity:0;pointer-events:none}ctx-provider{--color-text-base: black;--color-primary-accent: blue;display:flex;align-items:center;justify-content:center;width:190px;height:40px;padding-right:10px;padding-left:10px;background-color:#f5f5f5;border-radius:3px}lr-cloud-image-editor-activity{position:relative;display:flex;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light)}lr-modal lr-cloud-image-editor-activity{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%)}lr-select{display:inline-flex}lr-select>button{position:relative;display:inline-flex;align-items:center;padding-right:0!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-select>button>select{position:absolute;display:block;width:100%;height:100%;opacity:0}
+:where(.lr-wgt-cfg,.lr-wgt-common),:host{--cfg-pubkey: "YOUR_PUBLIC_KEY";--cfg-multiple: 1;--cfg-multiple-min: 0;--cfg-multiple-max: 0;--cfg-confirm-upload: 0;--cfg-img-only: 0;--cfg-accept: "";--cfg-external-sources-preferred-types: "";--cfg-store: "auto";--cfg-camera-mirror: 1;--cfg-source-list: "local, url, camera, dropbox, gdrive";--cfg-max-local-file-size-bytes: 0;--cfg-thumb-size: 76;--cfg-show-empty-list: 0;--cfg-use-local-image-editor: 0;--cfg-use-cloud-image-editor: 1;--cfg-remove-copyright: 0;--cfg-modal-scroll-lock: 1;--cfg-modal-backdrop-strokes: 0;--cfg-source-list-wrap: 1;--cfg-init-activity: "start-from";--cfg-done-activity: "";--cfg-remote-tab-session-key: "";--cfg-cdn-cname: "https://ucarecdn.com";--cfg-base-url: "https://upload.uploadcare.com";--cfg-social-base-url: "https://social.uploadcare.com";--cfg-secure-signature: "";--cfg-secure-expire: "";--cfg-secure-delivery-proxy: "";--cfg-retry-throttled-request-max-times: 1;--cfg-multipart-min-file-size: 26214400;--cfg-multipart-chunk-size: 5242880;--cfg-max-concurrent-requests: 10;--cfg-multipart-max-concurrent-requests: 4;--cfg-multipart-max-attempts: 3;--cfg-check-for-url-duplicates: 0;--cfg-save-url-for-recurrent-uploads: 0;--cfg-group-output: 0;--cfg-user-agent-integration: ""}:where(.lr-wgt-icons,.lr-wgt-common),:host{--icon-default: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-file: "m2.89453 1.2012c0-.473389.38376-.857145.85714-.857145h8.40003c.2273 0 .4453.090306.6061.251051l8.4 8.400004c.1607.16074.251.37876.251.60609v13.2c0 .4734-.3837.8571-.8571.8571h-16.80003c-.47338 0-.85714-.3837-.85714-.8571zm1.71429.85714v19.88576h15.08568v-11.4858h-7.5428c-.4734 0-.8572-.3837-.8572-.8571v-7.54286zm8.39998 1.21218 5.4736 5.47353-5.4736.00001z";--icon-close: "m4.60395 4.60395c.29289-.2929.76776-.2929 1.06066 0l6.33539 6.33535 6.3354-6.33535c.2929-.2929.7677-.2929 1.0606 0 .2929.29289.2929.76776 0 1.06066l-6.3353 6.33539 6.3353 6.3354c.2929.2929.2929.7677 0 1.0606s-.7677.2929-1.0606 0l-6.3354-6.3353-6.33539 6.3353c-.2929.2929-.76777.2929-1.06066 0-.2929-.2929-.2929-.7677 0-1.0606l6.33535-6.3354-6.33535-6.33539c-.2929-.2929-.2929-.76777 0-1.06066z";--icon-collapse: "M3.11572 12C3.11572 11.5858 3.45151 11.25 3.86572 11.25H20.1343C20.5485 11.25 20.8843 11.5858 20.8843 12C20.8843 12.4142 20.5485 12.75 20.1343 12.75H3.86572C3.45151 12.75 3.11572 12.4142 3.11572 12Z";--icon-expand: "M12.0001 8.33716L3.53033 16.8068C3.23743 17.0997 2.76256 17.0997 2.46967 16.8068C2.17678 16.5139 2.17678 16.0391 2.46967 15.7462L11.0753 7.14067C11.1943 7.01825 11.3365 6.92067 11.4936 6.8536C11.6537 6.78524 11.826 6.75 12.0001 6.75C12.1742 6.75 12.3465 6.78524 12.5066 6.8536C12.6637 6.92067 12.8059 7.01826 12.925 7.14068L21.5304 15.7462C21.8233 16.0391 21.8233 16.5139 21.5304 16.8068C21.2375 17.0997 20.7627 17.0997 20.4698 16.8068L12.0001 8.33716Z";--icon-info: "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";--icon-error: "M13,13H11V7H13M13,17H11V15H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z";--icon-arrow-down: "m11.5009 23.0302c.2844.2533.7135.2533.9978 0l9.2899-8.2758c.3092-.2756.3366-.7496.0611-1.0589s-.7496-.3367-1.0589-.0612l-8.0417 7.1639v-19.26834c0-.41421-.3358-.749997-.75-.749997s-.75.335787-.75.749997v19.26704l-8.04025-7.1626c-.30928-.2755-.78337-.2481-1.05889.0612-.27553.3093-.24816.7833.06112 1.0589z";--icon-upload: "m11.5014.392135c.2844-.253315.7134-.253315.9978 0l6.7037 5.971925c.3093.27552.3366.74961.0611 1.05889-.2755.30929-.7496.33666-1.0589.06113l-5.4553-4.85982v13.43864c0 .4142-.3358.75-.75.75s-.75-.3358-.75-.75v-13.43771l-5.45427 4.85889c-.30929.27553-.78337.24816-1.0589-.06113-.27553-.30928-.24816-.78337.06113-1.05889zm-10.644466 16.336765c.414216 0 .749996.3358.749996.75v4.9139h20.78567v-4.9139c0-.4142.3358-.75.75-.75.4143 0 .75.3358.75.75v5.6639c0 .4143-.3357.75-.75.75h-22.285666c-.414214 0-.75-.3357-.75-.75v-5.6639c0-.4142.335786-.75.75-.75z";--icon-local: "m3 3.75c-.82843 0-1.5.67157-1.5 1.5v13.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-9.75c0-.82843-.6716-1.5-1.5-1.5h-9c-.2634 0-.5076-.13822-.6431-.36413l-2.03154-3.38587zm-3 1.5c0-1.65685 1.34315-3 3-3h6.75c.2634 0 .5076.13822.6431.36413l2.0315 3.38587h8.5754c1.6569 0 3 1.34315 3 3v9.75c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3z";--icon-url: "m19.1099 3.67026c-1.7092-1.70917-4.5776-1.68265-6.4076.14738l-2.2212 2.22122c-.2929.29289-.7678.29289-1.0607 0-.29289-.29289-.29289-.76777 0-1.06066l2.2212-2.22122c2.376-2.375966 6.1949-2.481407 8.5289-.14738l1.2202 1.22015c2.334 2.33403 2.2286 6.15294-.1474 8.52895l-2.2212 2.2212c-.2929.2929-.7678.2929-1.0607 0s-.2929-.7678 0-1.0607l2.2212-2.2212c1.8301-1.83003 1.8566-4.69842.1474-6.40759zm-3.3597 4.57991c.2929.29289.2929.76776 0 1.06066l-6.43918 6.43927c-.29289.2928-.76777.2928-1.06066 0-.29289-.2929-.29289-.7678 0-1.0607l6.43924-6.43923c.2929-.2929.7677-.2929 1.0606 0zm-9.71158 1.17048c.29289.29289.29289.76775 0 1.06065l-2.22123 2.2212c-1.83002 1.8301-1.85654 4.6984-.14737 6.4076l1.22015 1.2202c1.70917 1.7091 4.57756 1.6826 6.40763-.1474l2.2212-2.2212c.2929-.2929.7677-.2929 1.0606 0s.2929.7677 0 1.0606l-2.2212 2.2212c-2.37595 2.376-6.19486 2.4815-8.52889.1474l-1.22015-1.2201c-2.334031-2.3341-2.22859-6.153.14737-8.5289l2.22123-2.22125c.29289-.2929.76776-.2929 1.06066 0z";--icon-camera: "m7.65 2.55c.14164-.18885.36393-.3.6-.3h7.5c.2361 0 .4584.11115.6.3l2.025 2.7h2.625c1.6569 0 3 1.34315 3 3v10.5c0 1.6569-1.3431 3-3 3h-18c-1.65685 0-3-1.3431-3-3v-10.5c0-1.65685 1.34315-3 3-3h2.625zm.975 1.2-2.025 2.7c-.14164.18885-.36393.3-.6.3h-3c-.82843 0-1.5.67157-1.5 1.5v10.5c0 .8284.67157 1.5 1.5 1.5h18c.8284 0 1.5-.6716 1.5-1.5v-10.5c0-.82843-.6716-1.5-1.5-1.5h-3c-.2361 0-.4584-.11115-.6-.3l-2.025-2.7zm3.375 6c-1.864 0-3.375 1.511-3.375 3.375s1.511 3.375 3.375 3.375 3.375-1.511 3.375-3.375-1.511-3.375-3.375-3.375zm-4.875 3.375c0-2.6924 2.18261-4.875 4.875-4.875 2.6924 0 4.875 2.1826 4.875 4.875s-2.1826 4.875-4.875 4.875c-2.69239 0-4.875-2.1826-4.875-4.875z";--icon-dots: "M16,12A2,2 0 0,1 18,10A2,2 0 0,1 20,12A2,2 0 0,1 18,14A2,2 0 0,1 16,12M10,12A2,2 0 0,1 12,10A2,2 0 0,1 14,12A2,2 0 0,1 12,14A2,2 0 0,1 10,12M4,12A2,2 0 0,1 6,10A2,2 0 0,1 8,12A2,2 0 0,1 6,14A2,2 0 0,1 4,12Z";--icon-back: "M20.251 12.0001C20.251 12.4143 19.9152 12.7501 19.501 12.7501L6.06696 12.7501L11.7872 18.6007C12.0768 18.8968 12.0715 19.3717 11.7753 19.6613C11.4791 19.9508 11.0043 19.9455 10.7147 19.6493L4.13648 12.9213C4.01578 12.8029 3.91947 12.662 3.85307 12.5065C3.78471 12.3464 3.74947 12.1741 3.74947 12C3.74947 11.8259 3.78471 11.6536 3.85307 11.4935C3.91947 11.338 4.01578 11.1971 4.13648 11.0787L10.7147 4.35068C11.0043 4.0545 11.4791 4.04916 11.7753 4.33873C12.0715 4.62831 12.0768 5.10315 11.7872 5.39932L6.06678 11.2501L19.501 11.2501C19.9152 11.2501 20.251 11.5859 20.251 12.0001Z";--icon-remove: "m6.35673 9.71429c-.76333 0-1.35856.66121-1.27865 1.42031l1.01504 9.6429c.06888.6543.62067 1.1511 1.27865 1.1511h9.25643c.658 0 1.2098-.4968 1.2787-1.1511l1.015-9.6429c.0799-.7591-.5153-1.42031-1.2786-1.42031zm.50041-4.5v.32142h-2.57143c-.71008 0-1.28571.57564-1.28571 1.28572s.57563 1.28571 1.28571 1.28571h15.42859c.7101 0 1.2857-.57563 1.2857-1.28571s-.5756-1.28572-1.2857-1.28572h-2.5714v-.32142c0-1.77521-1.4391-3.21429-3.2143-3.21429h-3.8572c-1.77517 0-3.21426 1.43908-3.21426 3.21429zm7.07146-.64286c.355 0 .6428.28782.6428.64286v.32142h-5.14283v-.32142c0-.35504.28782-.64286.64283-.64286z";--icon-edit: "M3.96371 14.4792c-.15098.151-.25578.3419-.3021.5504L2.52752 20.133c-.17826.8021.53735 1.5177 1.33951 1.3395l5.10341-1.1341c.20844-.0463.39934-.1511.55032-.3021l8.05064-8.0507-5.557-5.55702-8.05069 8.05062ZM13.4286 5.01437l5.557 5.55703 2.0212-2.02111c.6576-.65765.6576-1.72393 0-2.38159l-3.1755-3.17546c-.6577-.65765-1.7239-.65765-2.3816 0l-2.0211 2.02113Z";--icon-detail: "M5,3C3.89,3 3,3.89 3,5V19C3,20.11 3.89,21 5,21H19C20.11,21 21,20.11 21,19V5C21,3.89 20.11,3 19,3H5M5,5H19V19H5V5M7,7V9H17V7H7M7,11V13H17V11H7M7,15V17H14V15H7Z";--icon-select: "M7,10L12,15L17,10H7Z";--icon-check: "m12 22c5.5228 0 10-4.4772 10-10 0-5.52285-4.4772-10-10-10-5.52285 0-10 4.47715-10 10 0 5.5228 4.47715 10 10 10zm4.7071-11.4929-5.9071 5.9071-3.50711-3.5071c-.39052-.3905-.39052-1.0237 0-1.4142.39053-.3906 1.02369-.3906 1.41422 0l2.09289 2.0929 4.4929-4.49294c.3905-.39052 1.0237-.39052 1.4142 0 .3905.39053.3905 1.02374 0 1.41424z";--icon-add: "M12.75 21C12.75 21.4142 12.4142 21.75 12 21.75C11.5858 21.75 11.25 21.4142 11.25 21V12.7499H3C2.58579 12.7499 2.25 12.4141 2.25 11.9999C2.25 11.5857 2.58579 11.2499 3 11.2499H11.25V3C11.25 2.58579 11.5858 2.25 12 2.25C12.4142 2.25 12.75 2.58579 12.75 3V11.2499H21C21.4142 11.2499 21.75 11.5857 21.75 11.9999C21.75 12.4141 21.4142 12.7499 21 12.7499H12.75V21Z";--icon-edit-file: "m12.1109 6c.3469-1.69213 1.8444-2.96484 3.6391-2.96484s3.2922 1.27271 3.6391 2.96484h2.314c.4142 0 .75.33578.75.75 0 .41421-.3358.75-.75.75h-2.314c-.3469 1.69213-1.8444 2.9648-3.6391 2.9648s-3.2922-1.27267-3.6391-2.9648h-9.81402c-.41422 0-.75001-.33579-.75-.75 0-.41422.33578-.75.75-.75zm3.6391-1.46484c-1.2232 0-2.2148.99162-2.2148 2.21484s.9916 2.21484 2.2148 2.21484 2.2148-.99162 2.2148-2.21484-.9916-2.21484-2.2148-2.21484zm-11.1391 11.96484c.34691-1.6921 1.84437-2.9648 3.6391-2.9648 1.7947 0 3.2922 1.2727 3.6391 2.9648h9.814c.4142 0 .75.3358.75.75s-.3358.75-.75.75h-9.814c-.3469 1.6921-1.8444 2.9648-3.6391 2.9648-1.79473 0-3.29219-1.2727-3.6391-2.9648h-2.31402c-.41422 0-.75-.3358-.75-.75s.33578-.75.75-.75zm3.6391-1.4648c-1.22322 0-2.21484.9916-2.21484 2.2148s.99162 2.2148 2.21484 2.2148 2.2148-.9916 2.2148-2.2148-.99158-2.2148-2.2148-2.2148z";--icon-remove-file: "m11.9554 3.29999c-.7875 0-1.5427.31281-2.0995.86963-.49303.49303-.79476 1.14159-.85742 1.83037h5.91382c-.0627-.68878-.3644-1.33734-.8575-1.83037-.5568-.55682-1.312-.86963-2.0994-.86963zm4.461 2.7c-.0656-1.08712-.5264-2.11657-1.3009-2.89103-.8381-.83812-1.9749-1.30897-3.1601-1.30897-1.1853 0-2.32204.47085-3.16016 1.30897-.77447.77446-1.23534 1.80391-1.30087 2.89103h-2.31966c-.03797 0-.07529.00282-.11174.00827h-1.98826c-.41422 0-.75.33578-.75.75 0 .41421.33578.75.75.75h1.35v11.84174c0 .7559.30026 1.4808.83474 2.0152.53448.5345 1.25939.8348 2.01526.8348h9.44999c.7559 0 1.4808-.3003 2.0153-.8348.5344-.5344.8347-1.2593.8347-2.0152v-11.84174h1.35c.4142 0 .75-.33579.75-.75 0-.41422-.3358-.75-.75-.75h-1.9883c-.0364-.00545-.0737-.00827-.1117-.00827zm-10.49169 1.50827v11.84174c0 .358.14223.7014.3954.9546.25318.2532.59656.3954.9546.3954h9.44999c.358 0 .7014-.1422.9546-.3954s.3954-.5966.3954-.9546v-11.84174z";--icon-trash-file: var(--icon-remove);--icon-upload-error: var(--icon-error);--icon-fullscreen: "M5,5H10V7H7V10H5V5M14,5H19V10H17V7H14V5M17,14H19V19H14V17H17V14M10,17V19H5V14H7V17H10Z";--icon-fullscreen-exit: "M14,14H19V16H16V19H14V14M5,14H10V19H8V16H5V14M8,5H10V10H5V8H8V5M19,8V10H14V5H16V8H19Z";--icon-badge-success: "M10.5 18.2044L18.0992 10.0207C18.6629 9.41362 18.6277 8.46452 18.0207 7.90082C17.4136 7.33711 16.4645 7.37226 15.9008 7.97933L10.5 13.7956L8.0992 11.2101C7.53549 10.603 6.5864 10.5679 5.97933 11.1316C5.37226 11.6953 5.33711 12.6444 5.90082 13.2515L10.5 18.2044Z";--icon-badge-error: "m13.6 18.4c0 .8837-.7164 1.6-1.6 1.6-.8837 0-1.6-.7163-1.6-1.6s.7163-1.6 1.6-1.6c.8836 0 1.6.7163 1.6 1.6zm-1.6-13.9c.8284 0 1.5.67157 1.5 1.5v7c0 .8284-.6716 1.5-1.5 1.5s-1.5-.6716-1.5-1.5v-7c0-.82843.6716-1.5 1.5-1.5z";--icon-about: "M11.152 14.12v.1h1.523v-.1c.007-.409.053-.752.138-1.028.086-.277.22-.517.405-.72.188-.202.434-.397.735-.586.32-.191.593-.412.82-.66.232-.249.41-.531.533-.847.125-.32.187-.678.187-1.076 0-.579-.137-1.085-.41-1.518a2.717 2.717 0 0 0-1.14-1.018c-.49-.245-1.062-.367-1.715-.367-.597 0-1.142.114-1.636.34-.49.228-.884.564-1.182 1.008-.299.44-.46.98-.485 1.619h1.62c.024-.377.118-.684.282-.922.163-.241.369-.419.617-.532.25-.114.51-.17.784-.17.301 0 .575.063.82.191.248.124.447.302.597.533.149.23.223.504.223.82 0 .263-.05.502-.149.72-.1.216-.234.408-.405.574a3.48 3.48 0 0 1-.575.453c-.33.199-.613.42-.847.66-.234.242-.415.558-.543.949-.125.39-.19.916-.197 1.577ZM11.205 17.15c.21.206.46.31.75.31.196 0 .374-.049.534-.144.16-.096.287-.224.383-.384.1-.163.15-.343.15-.538a1 1 0 0 0-.32-.746 1.019 1.019 0 0 0-.746-.314c-.291 0-.542.105-.751.314-.21.206-.314.455-.314.746 0 .295.104.547.314.756ZM24 12c0 6.627-5.373 12-12 12S0 18.627 0 12 5.373 0 12 0s12 5.373 12 12Zm-1.5 0c0 5.799-4.701 10.5-10.5 10.5S1.5 17.799 1.5 12 6.201 1.5 12 1.5 22.5 6.201 22.5 12Z";--icon-edit-rotate: "M16.89,15.5L18.31,16.89C19.21,15.73 19.76,14.39 19.93,13H17.91C17.77,13.87 17.43,14.72 16.89,15.5M13,17.9V19.92C14.39,19.75 15.74,19.21 16.9,18.31L15.46,16.87C14.71,17.41 13.87,17.76 13,17.9M19.93,11C19.76,9.61 19.21,8.27 18.31,7.11L16.89,8.53C17.43,9.28 17.77,10.13 17.91,11M15.55,5.55L11,1V4.07C7.06,4.56 4,7.92 4,12C4,16.08 7.05,19.44 11,19.93V17.91C8.16,17.43 6,14.97 6,12C6,9.03 8.16,6.57 11,6.09V10L15.55,5.55Z";--icon-edit-flip-v: "M3 15V17H5V15M15 19V21H17V19M19 3H5C3.9 3 3 3.9 3 5V9H5V5H19V9H21V5C21 3.9 20.1 3 19 3M21 19H19V21C20.1 21 21 20.1 21 19M1 11V13H23V11M7 19V21H9V19M19 15V17H21V15M11 19V21H13V19M3 19C3 20.1 3.9 21 5 21V19Z";--icon-edit-flip-h: "M15 21H17V19H15M19 9H21V7H19M3 5V19C3 20.1 3.9 21 5 21H9V19H5V5H9V3H5C3.9 3 3 3.9 3 5M19 3V5H21C21 3.9 20.1 3 19 3M11 23H13V1H11M19 17H21V15H19M15 5H17V3H15M19 13H21V11H19M19 21C20.1 21 21 20.1 21 19H19Z";--icon-edit-brightness: "M12,18A6,6 0 0,1 6,12A6,6 0 0,1 12,6A6,6 0 0,1 18,12A6,6 0 0,1 12,18M20,15.31L23.31,12L20,8.69V4H15.31L12,0.69L8.69,4H4V8.69L0.69,12L4,15.31V20H8.69L12,23.31L15.31,20H20V15.31Z";--icon-edit-contrast: "M12,20C9.79,20 7.79,19.1 6.34,17.66L17.66,6.34C19.1,7.79 20,9.79 20,12A8,8 0 0,1 12,20M6,8H8V6H9.5V8H11.5V9.5H9.5V11.5H8V9.5H6M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,16H17V14.5H12V16Z";--icon-edit-saturation: "M3,13A9,9 0 0,0 12,22C12,17 7.97,13 3,13M12,5.5A2.5,2.5 0 0,1 14.5,8A2.5,2.5 0 0,1 12,10.5A2.5,2.5 0 0,1 9.5,8A2.5,2.5 0 0,1 12,5.5M5.6,10.25A2.5,2.5 0 0,0 8.1,12.75C8.63,12.75 9.12,12.58 9.5,12.31C9.5,12.37 9.5,12.43 9.5,12.5A2.5,2.5 0 0,0 12,15A2.5,2.5 0 0,0 14.5,12.5C14.5,12.43 14.5,12.37 14.5,12.31C14.88,12.58 15.37,12.75 15.9,12.75C17.28,12.75 18.4,11.63 18.4,10.25C18.4,9.25 17.81,8.4 16.97,8C17.81,7.6 18.4,6.74 18.4,5.75C18.4,4.37 17.28,3.25 15.9,3.25C15.37,3.25 14.88,3.41 14.5,3.69C14.5,3.63 14.5,3.56 14.5,3.5A2.5,2.5 0 0,0 12,1A2.5,2.5 0 0,0 9.5,3.5C9.5,3.56 9.5,3.63 9.5,3.69C9.12,3.41 8.63,3.25 8.1,3.25A2.5,2.5 0 0,0 5.6,5.75C5.6,6.74 6.19,7.6 7.03,8C6.19,8.4 5.6,9.25 5.6,10.25M12,22A9,9 0 0,0 21,13C16,13 12,17 12,22Z";--icon-edit-crop: "M7,17V1H5V5H1V7H5V17A2,2 0 0,0 7,19H17V23H19V19H23V17M17,15H19V7C19,5.89 18.1,5 17,5H9V7H17V15Z";--icon-edit-text: "M18.5,4L19.66,8.35L18.7,8.61C18.25,7.74 17.79,6.87 17.26,6.43C16.73,6 16.11,6 15.5,6H13V16.5C13,17 13,17.5 13.33,17.75C13.67,18 14.33,18 15,18V19H9V18C9.67,18 10.33,18 10.67,17.75C11,17.5 11,17 11,16.5V6H8.5C7.89,6 7.27,6 6.74,6.43C6.21,6.87 5.75,7.74 5.3,8.61L4.34,8.35L5.5,4H18.5Z";--icon-edit-draw: "m21.879394 2.1631238c-1.568367-1.62768627-4.136546-1.53831744-5.596267.1947479l-8.5642801 10.1674753c-1.4906533-.224626-3.061232.258204-4.2082427 1.448604-1.0665468 1.106968-1.0997707 2.464806-1.1203996 3.308068-.00142.05753-.00277.113001-.00439.16549-.02754.894146-.08585 1.463274-.5821351 2.069648l-.80575206.98457.88010766.913285c1.0539516 1.093903 2.6691689 1.587048 4.1744915 1.587048 1.5279113 0 3.2235468-.50598 4.4466094-1.775229 1.147079-1.190514 1.612375-2.820653 1.395772-4.367818l9.796763-8.8879697c1.669907-1.5149954 1.75609-4.1802333.187723-5.8079195zm-16.4593821 13.7924592c.8752943-.908358 2.2944227-.908358 3.1697054 0 .8752942.908358.8752942 2.381259 0 3.289617-.5909138.61325-1.5255389.954428-2.53719.954428-.5223687 0-.9935663-.09031-1.3832112-.232762.3631253-.915463.3952949-1.77626.4154309-2.429737.032192-1.045425.072224-1.308557.3352649-1.581546z";--icon-edit-guides: "M1.39,18.36L3.16,16.6L4.58,18L5.64,16.95L4.22,15.54L5.64,14.12L8.11,16.6L9.17,15.54L6.7,13.06L8.11,11.65L9.53,13.06L10.59,12L9.17,10.59L10.59,9.17L13.06,11.65L14.12,10.59L11.65,8.11L13.06,6.7L14.47,8.11L15.54,7.05L14.12,5.64L15.54,4.22L18,6.7L19.07,5.64L16.6,3.16L18.36,1.39L22.61,5.64L5.64,22.61L1.39,18.36Z";--icon-edit-color: "M17.5,12A1.5,1.5 0 0,1 16,10.5A1.5,1.5 0 0,1 17.5,9A1.5,1.5 0 0,1 19,10.5A1.5,1.5 0 0,1 17.5,12M14.5,8A1.5,1.5 0 0,1 13,6.5A1.5,1.5 0 0,1 14.5,5A1.5,1.5 0 0,1 16,6.5A1.5,1.5 0 0,1 14.5,8M9.5,8A1.5,1.5 0 0,1 8,6.5A1.5,1.5 0 0,1 9.5,5A1.5,1.5 0 0,1 11,6.5A1.5,1.5 0 0,1 9.5,8M6.5,12A1.5,1.5 0 0,1 5,10.5A1.5,1.5 0 0,1 6.5,9A1.5,1.5 0 0,1 8,10.5A1.5,1.5 0 0,1 6.5,12M12,3A9,9 0 0,0 3,12A9,9 0 0,0 12,21A1.5,1.5 0 0,0 13.5,19.5C13.5,19.11 13.35,18.76 13.11,18.5C12.88,18.23 12.73,17.88 12.73,17.5A1.5,1.5 0 0,1 14.23,16H16A5,5 0 0,0 21,11C21,6.58 16.97,3 12,3Z";--icon-edit-resize: "M10.59,12L14.59,8H11V6H18V13H16V9.41L12,13.41V16H20V4H8V12H10.59M22,2V18H12V22H2V12H6V2H22M10,14H4V20H10V14Z";--icon-external-source-placeholder: "M6.341 3.27a10.5 10.5 0 0 1 5.834-1.77.75.75 0 0 0 0-1.5 12 12 0 1 0 12 12 .75.75 0 0 0-1.5 0A10.5 10.5 0 1 1 6.34 3.27Zm14.145 1.48a.75.75 0 1 0-1.06-1.062L9.925 13.19V7.95a.75.75 0 1 0-1.5 0V15c0 .414.336.75.75.75h7.05a.75.75 0 0 0 0-1.5h-5.24l9.501-9.5Z";--icon-facebook: "m12 1.5c-5.79901 0-10.5 4.70099-10.5 10.5 0 4.9427 3.41586 9.0888 8.01562 10.2045v-6.1086h-2.13281c-.41421 0-.75-.3358-.75-.75v-3.2812c0-.4142.33579-.75.75-.75h2.13281v-1.92189c0-.95748.22571-2.51089 1.38068-3.6497 1.1934-1.17674 3.1742-1.71859 6.2536-1.05619.3455.07433.5923.3798.5923.73323v2.75395c0 .41422-.3358.75-.75.75-.6917 0-1.2029.02567-1.5844.0819-.3865.05694-.5781.13711-.675.20223-.1087.07303-.2367.20457-.2367 1.02837v1.0781h2.3906c.2193 0 .4275.0959.57.2626.1425.1666.205.3872.1709.6038l-.5156 3.2813c-.0573.3647-.3716.6335-.7409.6335h-1.875v6.1058c4.5939-1.1198 8.0039-5.2631 8.0039-10.2017 0-5.79901-4.701-10.5-10.5-10.5zm-12 10.5c0-6.62744 5.37256-12 12-12 6.6274 0 12 5.37256 12 12 0 5.9946-4.3948 10.9614-10.1384 11.8564-.2165.0337-.4369-.0289-.6033-.1714s-.2622-.3506-.2622-.5697v-7.7694c0-.4142.3358-.75.75-.75h1.9836l.28-1.7812h-2.2636c-.4142 0-.75-.3358-.75-.75v-1.8281c0-.82854.0888-1.72825.9-2.27338.3631-.24396.8072-.36961 1.293-.4412.3081-.0454.6583-.07238 1.0531-.08618v-1.39629c-2.4096-.40504-3.6447.13262-4.2928.77165-.7376.72735-.9338 1.79299-.9338 2.58161v2.67189c0 .4142-.3358.75-.75.75h-2.13279v1.7812h2.13279c.4142 0 .75.3358.75.75v7.7712c0 .219-.0956.427-.2619.5695-.1662.1424-.3864.2052-.6028.1717-5.74968-.8898-10.1509-5.8593-10.1509-11.8583z";--icon-dropbox: "m6.01895 1.92072c.24583-.15659.56012-.15658.80593.00003l5.17512 3.29711 5.1761-3.29714c.2458-.15659.5601-.15658.8059.00003l5.5772 3.55326c.2162.13771.347.37625.347.63253 0 .25629-.1308.49483-.347.63254l-4.574 2.91414 4.574 2.91418c.2162.1377.347.3762.347.6325s-.1308.4948-.347.6325l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.1761-3.2971-5.17512 3.2971c-.24581.1566-.5601.1566-.80593 0l-5.578142-3.5532c-.216172-.1377-.347058-.3763-.347058-.6326s.130886-.4949.347058-.6326l4.574772-2.91408-4.574772-2.91411c-.216172-.1377-.347058-.37626-.347058-.63257 0-.2563.130886-.49486.347058-.63256zm.40291 8.61518-4.18213 2.664 4.18213 2.664 4.18144-2.664zm6.97504 2.664 4.1821 2.664 4.1814-2.664-4.1814-2.664zm2.7758-3.54668-4.1727 2.65798-4.17196-2.65798 4.17196-2.658zm1.4063-.88268 4.1814-2.664-4.1814-2.664-4.1821 2.664zm-6.9757-2.664-4.18144-2.664-4.18213 2.664 4.18213 2.664zm-4.81262 12.43736c.22254-.3494.68615-.4522 1.03551-.2297l5.17521 3.2966 5.1742-3.2965c.3493-.2226.813-.1198 1.0355.2295.2226.3494.1198.813-.2295 1.0355l-5.5772 3.5533c-.2458.1566-.5601.1566-.8059 0l-5.57819-3.5532c-.34936-.2226-.45216-.6862-.22963-1.0355z";--icon-gdrive: "m7.73633 1.81806c.13459-.22968.38086-.37079.64707-.37079h7.587c.2718 0 .5223.14697.6548.38419l7.2327 12.94554c.1281.2293.1269.5089-.0031.7371l-3.7935 6.6594c-.1334.2342-.3822.3788-.6517.3788l-14.81918.0004c-.26952 0-.51831-.1446-.65171-.3788l-3.793526-6.6598c-.1327095-.233-.130949-.5191.004617-.7504zm.63943 1.87562-6.71271 11.45452 2.93022 5.1443 6.65493-11.58056zm3.73574 6.52652-2.39793 4.1727 4.78633.0001zm4.1168 4.1729 5.6967-.0002-6.3946-11.44563h-5.85354zm5.6844 1.4998h-13.06111l-2.96515 5.1598 13.08726-.0004z";--icon-gphotos: "M12.51 0c-.702 0-1.272.57-1.272 1.273V7.35A6.381 6.381 0 0 0 0 11.489c0 .703.57 1.273 1.273 1.273H7.35A6.381 6.381 0 0 0 11.488 24c.704 0 1.274-.57 1.274-1.273V16.65A6.381 6.381 0 0 0 24 12.51c0-.703-.57-1.273-1.273-1.273H16.65A6.381 6.381 0 0 0 12.511 0Zm.252 11.232V1.53a4.857 4.857 0 0 1 0 9.702Zm-1.53.006H1.53a4.857 4.857 0 0 1 9.702 0Zm1.536 1.524a4.857 4.857 0 0 0 9.702 0h-9.702Zm-6.136 4.857c0-2.598 2.04-4.72 4.606-4.85v9.7a4.857 4.857 0 0 1-4.606-4.85Z";--icon-instagram: "M6.225 12a5.775 5.775 0 1 1 11.55 0 5.775 5.775 0 0 1-11.55 0zM12 7.725a4.275 4.275 0 1 0 0 8.55 4.275 4.275 0 0 0 0-8.55zM18.425 6.975a1.4 1.4 0 1 0 0-2.8 1.4 1.4 0 0 0 0 2.8zM11.958.175h.084c2.152 0 3.823 0 5.152.132 1.35.134 2.427.41 3.362 1.013a7.15 7.15 0 0 1 2.124 2.124c.604.935.88 2.012 1.013 3.362.132 1.329.132 3 .132 5.152v.084c0 2.152 0 3.823-.132 5.152-.134 1.35-.41 2.427-1.013 3.362a7.15 7.15 0 0 1-2.124 2.124c-.935.604-2.012.88-3.362 1.013-1.329.132-3 .132-5.152.132h-.084c-2.152 0-3.824 0-5.153-.132-1.35-.134-2.427-.409-3.36-1.013a7.15 7.15 0 0 1-2.125-2.124C.716 19.62.44 18.544.307 17.194c-.132-1.329-.132-3-.132-5.152v-.084c0-2.152 0-3.823.132-5.152.133-1.35.409-2.427 1.013-3.362A7.15 7.15 0 0 1 3.444 1.32C4.378.716 5.456.44 6.805.307c1.33-.132 3-.132 5.153-.132zM6.953 1.799c-1.234.123-2.043.36-2.695.78A5.65 5.65 0 0 0 2.58 4.26c-.42.65-.657 1.46-.78 2.695C1.676 8.2 1.675 9.797 1.675 12c0 2.203 0 3.8.124 5.046.123 1.235.36 2.044.78 2.696a5.649 5.649 0 0 0 1.68 1.678c.65.421 1.46.658 2.694.78 1.247.124 2.844.125 5.047.125s3.8 0 5.046-.124c1.235-.123 2.044-.36 2.695-.78a5.648 5.648 0 0 0 1.68-1.68c.42-.65.657-1.46.78-2.694.123-1.247.124-2.844.124-5.047s-.001-3.8-.125-5.046c-.122-1.235-.359-2.044-.78-2.695a5.65 5.65 0 0 0-1.679-1.68c-.651-.42-1.46-.657-2.695-.78-1.246-.123-2.843-.124-5.046-.124-2.203 0-3.8 0-5.047.124z";--icon-flickr: "M5.95874 7.92578C3.66131 7.92578 1.81885 9.76006 1.81885 11.9994C1.81885 14.2402 3.66145 16.0744 5.95874 16.0744C8.26061 16.0744 10.1039 14.2396 10.1039 11.9994C10.1039 9.76071 8.26074 7.92578 5.95874 7.92578ZM0.318848 11.9994C0.318848 8.91296 2.85168 6.42578 5.95874 6.42578C9.06906 6.42578 11.6039 8.91232 11.6039 11.9994C11.6039 15.0877 9.06919 17.5744 5.95874 17.5744C2.85155 17.5744 0.318848 15.0871 0.318848 11.9994ZM18.3898 7.92578C16.0878 7.92578 14.2447 9.76071 14.2447 11.9994C14.2447 14.2396 16.088 16.0744 18.3898 16.0744C20.6886 16.0744 22.531 14.2401 22.531 11.9994C22.531 9.76019 20.6887 7.92578 18.3898 7.92578ZM12.7447 11.9994C12.7447 8.91232 15.2795 6.42578 18.3898 6.42578C21.4981 6.42578 24.031 8.91283 24.031 11.9994C24.031 15.0872 21.4982 17.5744 18.3898 17.5744C15.2794 17.5744 12.7447 15.0877 12.7447 11.9994Z";--icon-vk: var(--icon-external-source-placeholder);--icon-evernote: "M9.804 2.27v-.048c.055-.263.313-.562.85-.562h.44c.142 0 .325.014.526.033.066.009.124.023.267.06l.13.032h.002c.319.079.515.275.644.482a1.461 1.461 0 0 1 .16.356l.004.012a.75.75 0 0 0 .603.577l1.191.207a1988.512 1988.512 0 0 0 2.332.402c.512.083 1.1.178 1.665.442.64.3 1.19.795 1.376 1.77.548 2.931.657 5.829.621 8a39.233 39.233 0 0 1-.125 2.602 17.518 17.518 0 0 1-.092.849.735.735 0 0 0-.024.112c-.378 2.705-1.269 3.796-2.04 4.27-.746.457-1.53.451-2.217.447h-.192c-.46 0-1.073-.23-1.581-.635-.518-.412-.763-.87-.763-1.217 0-.45.188-.688.355-.786.161-.095.436-.137.796.087a.75.75 0 1 0 .792-1.274c-.766-.476-1.64-.52-2.345-.108-.7.409-1.098 1.188-1.098 2.08 0 .996.634 1.84 1.329 2.392.704.56 1.638.96 2.515.96l.185.002c.667.009 1.874.025 3.007-.67 1.283-.786 2.314-2.358 2.733-5.276.01-.039.018-.078.022-.105.011-.061.023-.14.034-.23.023-.184.051-.445.079-.772.055-.655.111-1.585.13-2.704.037-2.234-.074-5.239-.647-8.301v-.002c-.294-1.544-1.233-2.391-2.215-2.85-.777-.363-1.623-.496-2.129-.576-.097-.015-.18-.028-.25-.041l-.006-.001-1.99-.345-.761-.132a2.93 2.93 0 0 0-.182-.338A2.532 2.532 0 0 0 12.379.329l-.091-.023a3.967 3.967 0 0 0-.493-.103L11.769.2a7.846 7.846 0 0 0-.675-.04h-.44c-.733 0-1.368.284-1.795.742L2.416 7.431c-.468.428-.751 1.071-.751 1.81 0 .02 0 .041.003.062l.003.034c.017.21.038.468.096.796.107.715.275 1.47.391 1.994.029.13.055.245.075.342l.002.008c.258 1.141.641 1.94.978 2.466.168.263.323.456.444.589a2.808 2.808 0 0 0 .192.194c1.536 1.562 3.713 2.196 5.731 2.08.13-.005.35-.032.537-.073a2.627 2.627 0 0 0 .652-.24c.425-.26.75-.661.992-1.046.184-.294.342-.61.473-.915.197.193.412.357.627.493a5.022 5.022 0 0 0 1.97.709l.023.002.018.003.11.016c.088.014.205.035.325.058l.056.014c.088.022.164.04.235.061a1.736 1.736 0 0 1 .145.048l.03.014c.765.34 1.302 1.09 1.302 1.871a.75.75 0 0 0 1.5 0c0-1.456-.964-2.69-2.18-3.235-.212-.103-.5-.174-.679-.217l-.063-.015a10.616 10.616 0 0 0-.606-.105l-.02-.003-.03-.003h-.002a3.542 3.542 0 0 1-1.331-.485c-.471-.298-.788-.692-.828-1.234a.75.75 0 0 0-1.48-.106l-.001.003-.004.017a8.23 8.23 0 0 1-.092.352 9.963 9.963 0 0 1-.298.892c-.132.34-.29.68-.47.966-.174.276-.339.454-.478.549a1.178 1.178 0 0 1-.221.072 1.949 1.949 0 0 1-.241.036h-.013l-.032.002c-1.684.1-3.423-.437-4.604-1.65a.746.746 0 0 0-.053-.05L4.84 14.6a1.348 1.348 0 0 1-.07-.073 2.99 2.99 0 0 1-.293-.392c-.242-.379-.558-1.014-.778-1.985a54.1 54.1 0 0 0-.083-.376 27.494 27.494 0 0 1-.367-1.872l-.003-.02a6.791 6.791 0 0 1-.08-.67c.004-.277.086-.475.2-.609l.067-.067a.63.63 0 0 1 .292-.145h.05c.18 0 1.095.055 2.013.115l1.207.08.534.037a.747.747 0 0 0 .052.002c.782 0 1.349-.206 1.759-.585l.005-.005c.553-.52.622-1.225.622-1.76V6.24l-.026-.565A774.97 774.97 0 0 1 9.885 4.4c-.042-.961-.081-1.939-.081-2.13ZM4.995 6.953a251.126 251.126 0 0 1 2.102.137l.508.035c.48-.004.646-.122.715-.185.07-.068.146-.209.147-.649l-.024-.548a791.69 791.69 0 0 1-.095-2.187L4.995 6.953Zm16.122 9.996ZM15.638 11.626a.75.75 0 0 0 1.014.31 2.04 2.04 0 0 1 .304-.089 1.84 1.84 0 0 1 .544-.039c.215.023.321.06.37.085.033.016.039.026.047.04a.75.75 0 0 0 1.289-.767c-.337-.567-.906-.783-1.552-.85a3.334 3.334 0 0 0-1.002.062c-.27.056-.531.14-.705.234a.75.75 0 0 0-.31 1.014Z";--icon-box: "M1.01 4.148a.75.75 0 0 1 .75.75v4.348a4.437 4.437 0 0 1 2.988-1.153c1.734 0 3.23.992 3.978 2.438a4.478 4.478 0 0 1 3.978-2.438c2.49 0 4.488 2.044 4.488 4.543 0 2.5-1.999 4.544-4.488 4.544a4.478 4.478 0 0 1-3.978-2.438 4.478 4.478 0 0 1-3.978 2.438C2.26 17.18.26 15.135.26 12.636V4.898a.75.75 0 0 1 .75-.75Zm.75 8.488c0 1.692 1.348 3.044 2.988 3.044s2.989-1.352 2.989-3.044c0-1.691-1.349-3.043-2.989-3.043S1.76 10.945 1.76 12.636Zm10.944-3.043c-1.64 0-2.988 1.352-2.988 3.043 0 1.692 1.348 3.044 2.988 3.044s2.988-1.352 2.988-3.044c0-1.69-1.348-3.043-2.988-3.043Zm4.328-1.23a.75.75 0 0 1 1.052.128l2.333 2.983 2.333-2.983a.75.75 0 0 1 1.181.924l-2.562 3.277 2.562 3.276a.75.75 0 1 1-1.181.924l-2.333-2.983-2.333 2.983a.75.75 0 1 1-1.181-.924l2.562-3.276-2.562-3.277a.75.75 0 0 1 .129-1.052Z";--icon-onedrive: "M13.616 4.147a7.689 7.689 0 0 0-7.642 3.285A6.299 6.299 0 0 0 1.455 17.3c.684.894 2.473 2.658 5.17 2.658h12.141c.95 0 1.882-.256 2.697-.743.815-.486 1.514-1.247 1.964-2.083a5.26 5.26 0 0 0-3.713-7.612 7.69 7.69 0 0 0-6.098-5.373ZM3.34 17.15c.674.63 1.761 1.308 3.284 1.308h12.142a3.76 3.76 0 0 0 2.915-1.383l-7.494-4.489L3.34 17.15Zm10.875-6.25 2.47-1.038a5.239 5.239 0 0 1 1.427-.389 6.19 6.19 0 0 0-10.3-1.952 6.338 6.338 0 0 1 2.118.813l4.285 2.567Zm4.55.033c-.512 0-1.019.104-1.489.307l-.006.003-1.414.594 6.521 3.906a3.76 3.76 0 0 0-3.357-4.8l-.254-.01ZM4.097 9.617A4.799 4.799 0 0 1 6.558 8.9c.9 0 1.84.25 2.587.713l3.4 2.037-10.17 4.28a4.799 4.799 0 0 1 1.721-6.312Z";--icon-huddle: "M6.204 2.002c-.252.23-.357.486-.357.67V21.07c0 .15.084.505.313.812.208.28.499.477.929.477.519 0 .796-.174.956-.365.178-.212.286-.535.286-.924v-.013l.117-6.58c.004-1.725 1.419-3.883 3.867-3.883 1.33 0 2.332.581 2.987 1.364.637.762.95 1.717.95 2.526v6.47c0 .392.11.751.305.995.175.22.468.41 1.008.41.52 0 .816-.198 1.002-.437.207-.266.31-.633.31-.969V14.04c0-2.81-1.943-5.108-4.136-5.422a5.971 5.971 0 0 0-3.183.41c-.912.393-1.538.96-1.81 1.489a.75.75 0 0 1-1.417-.344v-7.5c0-.587-.47-1.031-1.242-1.031-.315 0-.638.136-.885.36ZM5.194.892A2.844 2.844 0 0 1 7.09.142c1.328 0 2.742.867 2.742 2.53v5.607a6.358 6.358 0 0 1 1.133-.629 7.47 7.47 0 0 1 3.989-.516c3.056.436 5.425 3.482 5.425 6.906v6.914c0 .602-.177 1.313-.627 1.89-.47.605-1.204 1.016-2.186 1.016-.96 0-1.698-.37-2.179-.973-.46-.575-.633-1.294-.633-1.933v-6.469c0-.456-.19-1.071-.602-1.563-.394-.471-.986-.827-1.836-.827-1.447 0-2.367 1.304-2.367 2.39v.014l-.117 6.58c-.001.64-.177 1.333-.637 1.881-.48.57-1.2.9-2.105.9-.995 0-1.7-.5-2.132-1.081-.41-.552-.61-1.217-.61-1.708V2.672c0-.707.366-1.341.847-1.78Z"}:where(.lr-wgt-l10n_en-US,.lr-wgt-common),:host{--l10n-locale-name: "en-US";--l10n-upload-file: "Upload file";--l10n-upload-files: "Upload files";--l10n-choose-file: "Choose file";--l10n-choose-files: "Choose files";--l10n-drop-files-here: "Drop files here";--l10n-select-file-source: "Select file source";--l10n-selected: "Selected";--l10n-upload: "Upload";--l10n-add-more: "Add more";--l10n-cancel: "Cancel";--l10n-start-from-cancel: var(--l10n-cancel);--l10n-clear: "Clear";--l10n-camera-shot: "Shot";--l10n-upload-url: "Import";--l10n-upload-url-placeholder: "Paste link here";--l10n-edit-image: "Edit image";--l10n-edit-detail: "Details";--l10n-back: "Back";--l10n-done: "Done";--l10n-ok: "Ok";--l10n-remove-from-list: "Remove";--l10n-no: "No";--l10n-yes: "Yes";--l10n-confirm-your-action: "Confirm your action";--l10n-are-you-sure: "Are you sure?";--l10n-selected-count: "Selected:";--l10n-upload-error: "Upload error";--l10n-validation-error: "Validation error";--l10n-no-files: "No files selected";--l10n-browse: "Browse";--l10n-not-uploaded-yet: "Not uploaded yet...";--l10n-file__one: "file";--l10n-file__other: "files";--l10n-error__one: "error";--l10n-error__other: "errors";--l10n-header-uploading: "Uploading {{count}} {{plural:file(count)}}";--l10n-header-failed: "{{count}} {{plural:error(count)}}";--l10n-header-succeed: "{{count}} {{plural:file(count)}} uploaded";--l10n-header-total: "{{count}} {{plural:file(count)}} selected";--l10n-src-type-local: "From device";--l10n-src-type-from-url: "From link";--l10n-src-type-camera: "Camera";--l10n-src-type-draw: "Draw";--l10n-src-type-facebook: "Facebook";--l10n-src-type-dropbox: "Dropbox";--l10n-src-type-gdrive: "Google Drive";--l10n-src-type-gphotos: "Google Photos";--l10n-src-type-instagram: "Instagram";--l10n-src-type-flickr: "Flickr";--l10n-src-type-vk: "VK";--l10n-src-type-evernote: "Evernote";--l10n-src-type-box: "Box";--l10n-src-type-onedrive: "Onedrive";--l10n-src-type-huddle: "Huddle";--l10n-src-type-other: "Other";--l10n-src-type: var(--l10n-src-type-local);--l10n-caption-from-url: "Import from link";--l10n-caption-camera: "Camera";--l10n-caption-draw: "Draw";--l10n-caption-edit-file: "Edit file";--l10n-file-no-name: "No name...";--l10n-toggle-fullscreen: "Toggle fullscreen";--l10n-toggle-guides: "Toggle guides";--l10n-rotate: "Rotate";--l10n-flip-vertical: "Flip vertical";--l10n-flip-horizontal: "Flip horizontal";--l10n-brightness: "Brightness";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-resize: "Resize image";--l10n-crop: "Crop";--l10n-select-color: "Select color";--l10n-text: "Text";--l10n-draw: "Draw";--l10n-cancel-edit: "Cancel edit";--l10n-tab-view: "Preview";--l10n-tab-details: "Details";--l10n-file-name: "Name";--l10n-file-size: "Size";--l10n-cdn-url: "CDN URL";--l10n-file-size-unknown: "Unknown";--l10n-camera-permissions-denied: "Camera access denied";--l10n-camera-permissions-prompt: "Please allow access to the camera";--l10n-camera-permissions-request: "Request access";--l10n-files-count-limit-error-title: "Files count limit overflow";--l10n-files-count-limit-error-too-few: "You\2019ve chosen {{total}} {{plural:file(total)}}. At least {{min}} {{plural:file(min)}} required.";--l10n-files-count-limit-error-too-many: "You\2019ve chosen too many files. {{max}} {{plural:file(max)}} is maximum.";--l10n-files-max-size-limit-error: "File is too big. Max file size is {{maxFileSize}}.";--l10n-has-validation-errors: "File validation error ocurred. Please, check your files before upload.";--l10n-images-only-accepted: "Only image files are accepted.";--l10n-file-type-not-allowed: "Uploading of these file types is not allowed.";--l10n-some-files-were-not-uploaded: "Some files were not uploaded."}:where(.lr-wgt-theme,.lr-wgt-common),:host{--darkmode: 0;--h-foreground: 208;--s-foreground: 4%;--l-foreground: calc(10% + 78% * var(--darkmode));--h-background: 208;--s-background: 4%;--l-background: calc(97% - 85% * var(--darkmode));--h-accent: 211;--s-accent: 100%;--l-accent: calc(50% - 5% * var(--darkmode));--h-confirm: 137;--s-confirm: 85%;--l-confirm: 53%;--h-error: 358;--s-error: 100%;--l-error: 66%;--shadows: 1;--h-shadow: 0;--s-shadow: 0%;--l-shadow: 0%;--opacity-normal: .6;--opacity-hover: .9;--opacity-active: 1;--ui-size: 32px;--gap-min: 2px;--gap-small: 4px;--gap-mid: 10px;--gap-max: 20px;--gap-table: 0px;--borders: 1;--border-radius-element: 8px;--border-radius-frame: 12px;--border-radius-thumb: 6px;--transition-duration: .2s;--modal-max-w: 800px;--modal-max-h: 600px;--modal-normal-w: 430px;--darkmode-minus: calc(1 + var(--darkmode) * -2);--clr-background: hsl(var(--h-background), var(--s-background), var(--l-background));--clr-background-dark: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-background-light: hsl( var(--h-background), var(--s-background), calc(var(--l-background) + 3% * var(--darkmode-minus)) );--clr-accent: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 15% * var(--darkmode)));--clr-accent-light: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 30%);--clr-accent-lightest: hsla(var(--h-accent), var(--s-accent), var(--l-accent), 10%);--clr-accent-light-opaque: hsl(var(--h-accent), var(--s-accent), calc(var(--l-accent) + 45% * var(--darkmode-minus)));--clr-accent-lightest-opaque: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) + 47% * var(--darkmode-minus)) );--clr-confirm: hsl(var(--h-confirm), var(--s-confirm), var(--l-confirm));--clr-error: hsl(var(--h-error), var(--s-error), var(--l-error));--clr-error-light: hsla(var(--h-error), var(--s-error), var(--l-error), 15%);--clr-error-lightest: hsla(var(--h-error), var(--s-error), var(--l-error), 5%);--clr-error-message-bgr: hsl(var(--h-error), var(--s-error), calc(var(--l-error) + 31% * var(--darkmode-minus)));--clr-txt: hsl(var(--h-foreground), var(--s-foreground), var(--l-foreground));--clr-txt-mid: hsl(var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 20% * var(--darkmode-minus)));--clr-txt-light: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 30% * var(--darkmode-minus)) );--clr-txt-lightest: hsl( var(--h-foreground), var(--s-foreground), calc(var(--l-foreground) + 50% * var(--darkmode-minus)) );--clr-shade-lv1: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 5%);--clr-shade-lv2: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 8%);--clr-shade-lv3: hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), 12%);--clr-generic-file-icon: var(--clr-txt-lightest);--border-light: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.1 - .05 * var(--darkmode)) * var(--borders)) );--border-mid: 1px solid hsla( var(--h-foreground), var(--s-foreground), var(--l-foreground), calc((.2 - .1 * var(--darkmode)) * var(--borders)) );--border-accent: 1px solid hsla(var(--h-accent), var(--s-accent), var(--l-accent), 1 * var(--borders));--border-dashed: 1px dashed hsla(var(--h-foreground), var(--s-foreground), var(--l-foreground), calc(.2 * var(--borders)));--clr-curtain: hsla(var(--h-background), var(--s-background), calc(var(--l-background)), 60%);--hsl-shadow: var(--h-shadow), var(--s-shadow), var(--l-shadow);--modal-shadow: 0px 0px 1px hsla(var(--hsl-shadow), calc((.3 + .65 * var(--darkmode)) * var(--shadows))), 0px 6px 20px hsla(var(--hsl-shadow), calc((.1 + .4 * var(--darkmode)) * var(--shadows)));--clr-btn-bgr-primary: var(--clr-accent);--clr-btn-bgr-primary-hover: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 4% * var(--darkmode-minus)) );--clr-btn-bgr-primary-active: hsl( var(--h-accent), var(--s-accent), calc(var(--l-accent) - 8% * var(--darkmode-minus)) );--clr-btn-txt-primary: hsl(var(--h-accent), var(--s-accent), 98%);--shadow-btn-primary: none;--clr-btn-bgr-secondary: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 3% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-hover: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 7% * var(--darkmode-minus)) );--clr-btn-bgr-secondary-active: hsl( var(--h-background), var(--s-background), calc(var(--l-background) - 12% * var(--darkmode-minus)) );--clr-btn-txt-secondary: var(--clr-txt-mid);--shadow-btn-secondary: none;--clr-btn-bgr-disabled: var(--clr-background);--clr-btn-txt-disabled: var(--clr-txt-lightest);--shadow-btn-disabled: none}@media only screen and (max-height: 600px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-h: 100%}}@media only screen and (max-width: 430px){:where(.lr-wgt-theme,.lr-wgt-common),:host{--modal-max-w: 100vw;--modal-max-h: var(--uploadcare-blocks-window-height)}}:where(.lr-wgt-theme,.lr-wgt-common),:host{color:var(--clr-txt);font-size:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}:where(.lr-wgt-theme,.lr-wgt-common) *,:host *{box-sizing:border-box}:where(.lr-wgt-theme,.lr-wgt-common) [hidden],:host [hidden]{display:none!important}:where(.lr-wgt-theme,.lr-wgt-common) [activity]:not([active]),:host [activity]:not([active]){display:none}:where(.lr-wgt-theme,.lr-wgt-common) dialog:not([open]) [activity],:host dialog:not([open]) [activity]{display:none}:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{display:flex;align-items:center;justify-content:center;height:var(--ui-size);padding-right:1.4em;padding-left:1.4em;font-size:1em;font-family:inherit;white-space:nowrap;border:none;border-radius:var(--border-radius-element);cursor:pointer;user-select:none}@media only screen and (max-width: 800px){:where(.lr-wgt-theme,.lr-wgt-common) button,:host button{padding-right:1em;padding-left:1em}}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn,:host button.primary-btn{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary);box-shadow:var(--shadow-btn-primary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:hover,:host button.primary-btn:hover{background-color:var(--clr-btn-bgr-primary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.primary-btn:active,:host button.primary-btn:active{background-color:var(--clr-btn-bgr-primary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn,:host button.secondary-btn{color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary);transition:background-color var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:hover,:host button.secondary-btn:hover{background-color:var(--clr-btn-bgr-secondary-hover)}:where(.lr-wgt-theme,.lr-wgt-common) button.secondary-btn:active,:host button.secondary-btn:active{background-color:var(--clr-btn-bgr-secondary-active)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn,:host button.mini-btn{width:var(--ui-size);height:var(--ui-size);padding:0;background-color:transparent;border:none;cursor:pointer;transition:var(--transition-duration) ease;color:var(--clr-txt)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:hover,:host button.mini-btn:hover{background-color:var(--clr-shade-lv1)}:where(.lr-wgt-theme,.lr-wgt-common) button.mini-btn:active,:host button.mini-btn:active{background-color:var(--clr-shade-lv2)}:where(.lr-wgt-theme,.lr-wgt-common) :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]),:host :is(button[disabled],button.primary-btn[disabled],button.secondary-btn[disabled]){color:var(--clr-btn-txt-disabled);background-color:var(--clr-btn-bgr-disabled);box-shadow:var(--shadow-btn-disabled);pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) a,:host a{color:var(--clr-accent);text-decoration:none}:where(.lr-wgt-theme,.lr-wgt-common) a[disabled],:host a[disabled]{pointer-events:none}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]{display:flex;width:100%;height:var(--ui-size);padding-right:.6em;padding-left:.6em;color:var(--clr-txt);font-size:1em;font-family:inherit;background-color:var(--clr-background-light);border:var(--border-light);border-radius:var(--border-radius-element);transition:var(--transition-duration)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text],:host input[type=text]::placeholder{color:var(--clr-txt-lightest)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:hover,:host input[type=text]:hover{border-color:var(--clr-accent-light)}:where(.lr-wgt-theme,.lr-wgt-common) input[type=text]:focus,:host input[type=text]:focus{border-color:var(--clr-accent);outline:none}:where(.lr-wgt-theme,.lr-wgt-common) input[disabled],:host input[disabled]{opacity:.6;pointer-events:none}lr-icon{display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size)}lr-icon svg{width:calc(var(--ui-size) / 2);height:calc(var(--ui-size) / 2)}lr-icon:not([raw]) path{fill:currentColor}lr-tabs{display:grid;grid-template-rows:min-content minmax(var(--ui-size),auto);height:100%;overflow:hidden;color:var(--clr-txt-lightest)}lr-tabs>.tabs-row{display:flex;grid-template-columns:minmax();background-color:var(--clr-background-light)}lr-tabs>.tabs-context{overflow-y:auto}lr-tabs .tabs-row>.tab{display:flex;flex-grow:1;align-items:center;justify-content:center;height:var(--ui-size);border-bottom:var(--border-light);cursor:pointer;transition:var(--transition-duration)}lr-tabs .tabs-row>.tab[current]{color:var(--clr-txt);border-color:var(--clr-txt)}lr-range{position:relative;display:inline-flex;align-items:center;justify-content:center;height:var(--ui-size)}lr-range datalist{display:none}lr-range input{width:100%;height:100%;opacity:0}lr-range .track-wrapper{position:absolute;right:10px;left:10px;display:flex;align-items:center;justify-content:center;height:2px;user-select:none;pointer-events:none}lr-range .track{position:absolute;right:0;left:0;display:flex;align-items:center;justify-content:center;height:2px;background-color:currentColor;border-radius:2px;opacity:.5}lr-range .slider{position:absolute;width:16px;height:16px;background-color:currentColor;border-radius:100%;transform:translate(-50%)}lr-range .bar{position:absolute;left:0;height:100%;background-color:currentColor;border-radius:2px}lr-range .caption{position:absolute;display:inline-flex;justify-content:center}lr-color{position:relative;display:inline-flex;align-items:center;justify-content:center;width:var(--ui-size);height:var(--ui-size);overflow:hidden;background-color:var(--clr-background);cursor:pointer}lr-color[current]{background-color:var(--clr-txt)}lr-color input[type=color]{position:absolute;display:block;width:100%;height:100%;opacity:0}lr-color .current-color{position:absolute;width:50%;height:50%;border:2px solid #fff;border-radius:100%;pointer-events:none}lr-config{display:none}lr-simple-btn{position:relative;display:inline-flex}lr-simple-btn button{padding-left:.2em!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-simple-btn button lr-icon svg{transform:scale(.8)}lr-simple-btn button:hover{background-color:var(--clr-btn-bgr-secondary-hover)}lr-simple-btn button:active{background-color:var(--clr-btn-bgr-secondary-active)}lr-simple-btn>lr-drop-area{display:contents}lr-simple-btn .visual-drop-area{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;padding:var(--gap-min);border:var(--border-dashed);border-radius:inherit;opacity:0;transition:border-color var(--transition-duration) ease,background-color var(--transition-duration) ease,opacity var(--transition-duration) ease}lr-simple-btn .visual-drop-area:before{position:absolute;top:0;left:0;display:flex;align-items:center;justify-content:center;width:100%;height:100%;color:var(--clr-txt-light);background-color:var(--clr-background);border-radius:inherit;content:var(--l10n-drop-files-here)}lr-simple-btn>lr-drop-area[drag-state=active] .visual-drop-area{background-color:var(--clr-accent-lightest);opacity:1}lr-simple-btn>lr-drop-area[drag-state=inactive] .visual-drop-area{background-color:var(--clr-shade-lv1);opacity:0}lr-simple-btn>lr-drop-area[drag-state=near] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent-light);opacity:1}lr-simple-btn>lr-drop-area[drag-state=over] .visual-drop-area{background-color:var(--clr-accent-lightest);border-color:var(--clr-accent);opacity:1}lr-simple-btn>:where(lr-drop-area[drag-state=active],lr-drop-area[drag-state=near],lr-drop-area[drag-state=over]) button{box-shadow:none}lr-simple-btn>lr-drop-area:after{content:""}lr-source-btn{display:flex;align-items:center;margin-bottom:var(--gap-min);padding:var(--gap-min) var(--gap-mid);color:var(--clr-txt-mid);border-radius:var(--border-radius-element);cursor:pointer;transition-duration:var(--transition-duration);transition-property:background-color,color;user-select:none}lr-source-btn:hover{color:var(--clr-accent);background-color:var(--clr-accent-lightest)}lr-source-btn:active{color:var(--clr-accent);background-color:var(--clr-accent-light)}lr-source-btn lr-icon{display:inline-flex;flex-grow:1;justify-content:center;min-width:var(--ui-size);margin-right:var(--gap-mid);opacity:.8}lr-source-btn[type=local]>.txt:after{content:var(--l10n-local-files)}lr-source-btn[type=camera]>.txt:after{content:var(--l10n-camera)}lr-source-btn[type=url]>.txt:after{content:var(--l10n-from-url)}lr-source-btn[type=other]>.txt:after{content:var(--l10n-other)}lr-source-btn .txt{display:flex;align-items:center;box-sizing:border-box;width:100%;height:var(--ui-size);padding:0;white-space:nowrap;border:none}lr-drop-area{padding:var(--gap-min);overflow:hidden;border:var(--border-dashed);border-radius:var(--border-radius-frame);transition:var(--transition-duration) ease}lr-drop-area,lr-drop-area .content-wrapper{display:flex;align-items:center;justify-content:center;width:100%;height:100%}lr-drop-area .text{position:relative;margin:var(--gap-mid);color:var(--clr-txt-light);transition:var(--transition-duration) ease}lr-drop-area[ghost][drag-state=inactive]{display:none;opacity:0}lr-drop-area[ghost]:not([fullscreen]):is([drag-state=active],[drag-state=near],[drag-state=over]){background:var(--clr-background)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) :is(.text,.icon-container){color:var(--clr-accent)}lr-drop-area:is([drag-state=active],[drag-state=near],[drag-state=over],:hover){color:var(--clr-accent);background:var(--clr-accent-lightest);border-color:var(--clr-accent-light)}lr-drop-area:is([drag-state=active],[drag-state=near]){opacity:1}lr-drop-area[drag-state=over]{border-color:var(--clr-accent);opacity:1}lr-drop-area[with-icon]{min-height:calc(var(--ui-size) * 6)}lr-drop-area[with-icon] .content-wrapper{display:flex;flex-direction:column}lr-drop-area[with-icon] .text{color:var(--clr-txt);font-weight:500;font-size:1.1em}lr-drop-area[with-icon] .icon-container{position:relative;width:calc(var(--ui-size) * 2);height:calc(var(--ui-size) * 2);margin:var(--gap-mid);overflow:hidden;color:var(--clr-txt);background-color:var(--clr-background);border-radius:50%;transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon{position:absolute;top:calc(50% - var(--ui-size) / 2);left:calc(50% - var(--ui-size) / 2);transition:var(--transition-duration) ease}lr-drop-area[with-icon] lr-icon:last-child{transform:translateY(calc(var(--ui-size) * 1.5))}lr-drop-area[with-icon]:hover .icon-container,lr-drop-area[with-icon]:hover .text{color:var(--clr-accent)}lr-drop-area[with-icon]:hover .icon-container{background-color:var(--clr-accent-lightest)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .icon-container{color:#fff;background-color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) .text{color:var(--clr-accent)}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[with-icon]>.content-wrapper:is([drag-state=active],[drag-state=near],[drag-state=over]) lr-icon:last-child{transform:translateY(0)}lr-drop-area[with-icon]>.content-wrapper[drag-state=near] lr-icon:last-child{transform:scale(1.3)}lr-drop-area[with-icon]>.content-wrapper[drag-state=over] lr-icon:last-child{transform:scale(1.5)}lr-drop-area[fullscreen]{position:fixed;inset:0;z-index:2147483647;display:flex;align-items:center;justify-content:center;width:calc(100vw - var(--gap-mid) * 2);height:calc(100vh - var(--gap-mid) * 2);margin:var(--gap-mid)}lr-drop-area[fullscreen] .content-wrapper{width:100%;max-width:calc(var(--modal-normal-w) * .8);height:calc(var(--ui-size) * 6);color:var(--clr-txt);background-color:var(--clr-background-light);border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:var(--transition-duration) ease}lr-drop-area[with-icon][fullscreen][drag-state=active]>.content-wrapper,lr-drop-area[with-icon][fullscreen][drag-state=near]>.content-wrapper{transform:translateY(var(--gap-mid));opacity:0}lr-drop-area[with-icon][fullscreen][drag-state=over]>.content-wrapper{transform:translateY(0);opacity:1}:is(lr-drop-area[with-icon][fullscreen])>.content-wrapper lr-icon:first-child{transform:translateY(calc(var(--ui-size) * -1.5))}lr-drop-area[clickable]{cursor:pointer}lr-modal{--modal-max-content-height: calc(var(--uploadcare-blocks-window-height, 100vh) - 4 * var(--gap-mid) - var(--ui-size));--modal-content-height-fill: var(--uploadcare-blocks-window-height, 100vh)}lr-modal[dialog-fallback]{--lr-z-max: 2147483647;position:fixed;z-index:var(--lr-z-max);display:flex;align-items:center;justify-content:center;width:100vw;height:100vh;pointer-events:none;inset:0}lr-modal[dialog-fallback] dialog[open]{z-index:var(--lr-z-max);pointer-events:auto}lr-modal[dialog-fallback] dialog[open]+.backdrop{position:fixed;top:0;left:0;z-index:calc(var(--lr-z-max) - 1);align-items:center;justify-content:center;width:100vw;height:100vh;background-color:var(--clr-curtain);pointer-events:auto}lr-modal[strokes][dialog-fallback] dialog[open]+.backdrop{background-image:var(--modal-backdrop-background-image)}@supports selector(dialog::backdrop){lr-modal>dialog::backdrop{background-color:#0000001a}lr-modal[strokes]>dialog::backdrop{background-image:var(--modal-backdrop-background-image)}}lr-modal>dialog[open]{transform:translateY(0);visibility:visible;opacity:1}lr-modal>dialog:not([open]){transform:translateY(20px);visibility:hidden;opacity:0}lr-modal>dialog{display:flex;flex-direction:column;width:max-content;max-width:min(calc(100% - var(--gap-mid) * 2),calc(var(--modal-max-w) - var(--gap-mid) * 2));min-height:var(--ui-size);max-height:calc(var(--modal-max-h) - var(--gap-mid) * 2);margin:auto;padding:0;overflow:hidden;background-color:var(--clr-background-light);border:0;border-radius:var(--border-radius-frame);box-shadow:var(--modal-shadow);transition:transform calc(var(--transition-duration) * 2)}@media only screen and (max-width: 430px),only screen and (max-height: 600px){lr-modal>dialog>.content{height:var(--modal-max-content-height)}}lr-url-source{display:block;background-color:var(--clr-background-light)}lr-modal lr-url-source{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-url-source>.content{display:grid;grid-gap:var(--gap-small);grid-template-columns:1fr min-content;padding:var(--gap-mid);padding-top:0}lr-url-source .url-input{display:flex}lr-url-source .url-upload-btn:after{content:var(--l10n-upload-url)}lr-camera-source{position:relative;display:flex;flex-direction:column;width:100%;height:100%;max-height:100%;overflow:hidden;background-color:var(--clr-background-light);border-radius:var(--border-radius-element)}lr-modal lr-camera-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:100vh;max-height:var(--modal-max-content-height)}lr-camera-source.initialized{height:max-content}@media only screen and (max-width: 430px){lr-camera-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-camera-source video{display:block;width:100%;max-height:100%;object-fit:contain;object-position:center center;background-color:var(--clr-background-dark);border-radius:var(--border-radius-element)}lr-camera-source .toolbar{position:absolute;bottom:0;display:flex;justify-content:space-between;width:100%;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-camera-source .content{display:flex;flex:1;justify-content:center;width:100%;padding:var(--gap-mid);padding-top:0;overflow:hidden}lr-camera-source .message-box{--padding: calc(var(--gap-max) * 2);display:flex;flex-direction:column;grid-gap:var(--gap-max);align-items:center;justify-content:center;padding:var(--padding) var(--padding) 0 var(--padding);color:var(--clr-txt)}lr-camera-source .message-box button{color:var(--clr-btn-txt-primary);background-color:var(--clr-btn-bgr-primary)}lr-camera-source .shot-btn{position:absolute;bottom:var(--gap-max);width:calc(var(--ui-size) * 1.8);height:calc(var(--ui-size) * 1.8);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;opacity:.85;transition:var(--transition-duration) ease}lr-camera-source .shot-btn:hover{transform:scale(1.05);opacity:1}lr-camera-source .shot-btn:active{background-color:var(--clr-txt-mid);opacity:1}lr-camera-source .shot-btn[disabled]{bottom:calc(var(--gap-max) * -1 - var(--gap-mid) - var(--ui-size) * 2)}lr-camera-source .shot-btn lr-icon svg{width:calc(var(--ui-size) / 1.5);height:calc(var(--ui-size) / 1.5)}lr-external-source{display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--clr-background-light);overflow:hidden}lr-modal lr-external-source{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height)}lr-external-source>.content{position:relative;display:grid;flex:1;grid-template-rows:1fr min-content}@media only screen and (max-width: 430px){lr-external-source{width:calc(100vw - var(--gap-mid) * 2);height:var(--modal-content-height-fill, 100%)}}lr-external-source iframe{display:block;width:100%;height:100%;border:none}lr-external-source .iframe-wrapper{overflow:hidden}lr-external-source .toolbar{display:grid;grid-gap:var(--gap-mid);grid-template-columns:max-content 1fr max-content max-content;align-items:center;width:100%;padding:var(--gap-mid);border-top:var(--border-light)}lr-external-source .back-btn{padding-left:0}lr-external-source .back-btn:after{content:var(--l10n-back)}lr-external-source .selected-counter{display:flex;grid-gap:var(--gap-mid);align-items:center;justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt-light)}lr-upload-list{display:flex;flex-direction:column;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light);transition:opacity var(--transition-duration)}lr-modal lr-upload-list{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:max-content;max-height:var(--modal-max-content-height)}lr-upload-list .no-files{height:var(--ui-size);padding:var(--gap-max)}lr-upload-list .files{display:block;flex:1;min-height:var(--ui-size);padding:0 var(--gap-mid);overflow:auto}lr-upload-list .toolbar{display:flex;gap:var(--gap-small);justify-content:space-between;padding:var(--gap-mid);background-color:var(--clr-background-light)}lr-upload-list .toolbar .add-more-btn{padding-left:.2em}lr-upload-list .toolbar-spacer{flex:1}lr-upload-list lr-drop-area{position:absolute;top:0;left:0;width:calc(100% - var(--gap-mid) * 2);height:calc(100% - var(--gap-mid) * 2);margin:var(--gap-mid);border-radius:var(--border-radius-element)}lr-upload-list lr-activity-header>.header-text{padding:0 var(--gap-mid)}lr-upload-list .common-error{border-radius:var(--border-radius-element);color:var(--clr-error);background-color:var(--clr-error-message-bgr);display:flex;align-items:center;justify-content:center;padding:var(--gap-mid);margin:var(--gap-small) var(--gap-mid) 0 var(--gap-mid);font-size:.95em}lr-start-from{display:block;overflow-y:auto}lr-start-from .content{display:grid;grid-auto-flow:row;gap:var(--gap-max);width:100%;height:100%;padding:var(--gap-max);background-color:var(--clr-background-light)}lr-modal lr-start-from{width:min(calc(var(--modal-normal-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2))}lr-file-item{display:block}lr-file-item>.inner{position:relative;display:grid;grid-template-columns:32px 1fr max-content;gap:var(--gap-min);align-items:center;margin-bottom:var(--gap-small);padding:var(--gap-mid);overflow:hidden;font-size:.95em;background-color:var(--clr-background);border-radius:var(--border-radius-element);transition:var(--transition-duration)}lr-file-item:last-of-type>.inner{margin-bottom:0}lr-file-item>.inner[focused]{background-color:transparent}lr-file-item>.inner[uploading] .edit-btn{display:none}lr-file-item>:where(.inner[failed],.inner[limit-overflow]){background-color:var(--clr-error-lightest)}lr-file-item .thumb{position:relative;display:inline-flex;width:var(--ui-size);height:var(--ui-size);background-color:var(--clr-shade-lv1);background-position:center center;background-size:cover;border-radius:var(--border-radius-thumb)}lr-file-item .file-name-wrapper{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;max-width:100%;padding-right:var(--gap-mid);padding-left:var(--gap-mid);overflow:hidden;color:var(--clr-txt-light);transition:color var(--transition-duration)}lr-file-item .file-name{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}lr-file-item .file-error{display:none;color:var(--clr-error);font-size:.85em;line-height:130%}lr-file-item button.remove-btn,lr-file-item button.edit-btn{color:var(--clr-txt-lightest)!important}lr-file-item button.upload-btn{display:none}lr-file-item button:hover{color:var(--clr-txt-light)}lr-file-item .badge{position:absolute;top:calc(var(--ui-size) * -.13);right:calc(var(--ui-size) * -.13);width:calc(var(--ui-size) * .44);height:calc(var(--ui-size) * .44);color:var(--clr-background-light);background-color:var(--clr-txt);border-radius:50%;transform:scale(.3);opacity:0;transition:var(--transition-duration) ease;display:flex;justify-content:center;align-items:center}lr-file-item>.inner:where([failed],[limit-overflow],[finished]) .badge{transform:scale(1);opacity:1}lr-file-item>.inner[finished] .badge{background-color:var(--clr-confirm)}lr-file-item>.inner:where([failed],[limit-overflow]) .badge{background-color:var(--clr-error)}lr-file-item>.inner:where([failed],[limit-overflow]) .file-error{display:block}lr-file-item .badge lr-icon,lr-file-item .badge lr-icon svg{width:100%;height:100%}lr-file-item .progress-bar{top:calc(100% - 2px);height:2px}lr-file-item .file-actions{display:flex;gap:var(--gap-min);align-items:center;justify-content:center}lr-upload-details{display:flex;flex-direction:column;width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%);max-height:var(--modal-max-content-height);overflow:hidden;background-color:var(--clr-background-light)}lr-upload-details>.content{position:relative;display:grid;flex:1;grid-template-rows:auto min-content}lr-upload-details lr-tabs .tabs-context{position:relative}lr-upload-details .toolbar{display:grid;grid-template-columns:min-content min-content 1fr min-content;gap:var(--gap-mid);padding:var(--gap-mid);border-top:var(--border-light)}lr-upload-details .toolbar[edit-disabled]{display:flex;justify-content:space-between}lr-upload-details .remove-btn{padding-left:.5em}lr-upload-details .detail-btn{padding-left:0;color:var(--clr-txt);background-color:var(--clr-background)}lr-upload-details .edit-btn{padding-left:.5em}lr-upload-details .details{padding:var(--gap-max)}lr-upload-details .info-block{padding-top:var(--gap-max);padding-bottom:calc(var(--gap-max) + var(--gap-table));color:var(--clr-txt);border-bottom:var(--border-light)}lr-upload-details .info-block:first-of-type{padding-top:0}lr-upload-details .info-block:last-of-type{border-bottom:none}lr-upload-details .info-block>.info-block_name{margin-bottom:.4em;color:var(--clr-txt-light);font-size:.8em}lr-upload-details .cdn-link[disabled]{pointer-events:none}lr-upload-details .cdn-link[disabled]:before{filter:grayscale(1);content:var(--l10n-not-uploaded-yet)}lr-file-preview{position:absolute;inset:0;display:flex;align-items:center;justify-content:center}lr-file-preview>lr-img{display:contents}lr-file-preview>lr-img>.img-view{position:absolute;inset:0;width:100%;max-width:100%;height:100%;max-height:100%;object-fit:scale-down}lr-confirmation-dialog{display:block;padding:var(--gap-mid);padding-top:var(--gap-max)}lr-confirmation-dialog .message{display:flex;justify-content:center;padding:var(--gap-mid);padding-bottom:var(--gap-max);font-weight:500;font-size:1.1em}lr-confirmation-dialog .toolbar{display:grid;grid-template-columns:1fr 1fr;gap:var(--gap-mid);margin-top:var(--gap-mid)}lr-progress-bar-common{position:fixed;right:0;bottom:0;left:0;z-index:10000;display:block;height:var(--gap-mid);background-color:var(--clr-background);transition:opacity .3s}lr-progress-bar-common:not([active]){opacity:0;pointer-events:none}lr-progress-bar{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;overflow:hidden;pointer-events:none}lr-progress-bar .progress{width:calc(var(--l-width) * 1%);height:100%;background-color:var(--clr-accent-light);transform:translate(0);opacity:1;transition:width .6s,opacity .3s}lr-progress-bar .progress--hidden{opacity:0}lr-activity-header{display:flex;gap:var(--gap-mid);justify-content:space-between;padding:var(--gap-mid);color:var(--clr-txt);font-weight:500;font-size:1em;line-height:var(--ui-size)}lr-activity-header lr-icon{height:var(--ui-size)}lr-activity-header>*{display:flex;align-items:center}lr-activity-header button{display:inline-flex;align-items:center;justify-content:center;color:var(--clr-txt-mid)}lr-activity-header button:hover{background-color:var(--clr-background)}lr-activity-header button:active{background-color:var(--clr-background-dark)}lr-copyright{display:flex;align-items:flex-end}lr-copyright .credits{padding:0 var(--gap-mid) var(--gap-mid) calc(var(--gap-mid) * 1.5);color:var(--clr-txt-lightest);font-weight:400;font-size:.85em;opacity:.7;transition:var(--transition-duration) ease}lr-copyright .credits:hover{opacity:1}:host(.lr-cloud-image-editor) lr-icon,.lr-cloud-image-editor lr-icon{display:flex;align-items:center;justify-content:center;width:100%;height:100%}:host(.lr-cloud-image-editor) lr-icon svg,.lr-cloud-image-editor lr-icon svg{width:unset;height:unset}:host(.lr-cloud-image-editor) lr-icon:not([raw]) path,.lr-cloud-image-editor lr-icon:not([raw]) path{stroke-linejoin:round;fill:none;stroke:currentColor;stroke-width:1.2}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--icon-rotate: "M13.5.399902L12 1.9999l1.5 1.6M12.0234 2H14.4C16.3882 2 18 3.61178 18 5.6V8M4 17h9c.5523 0 1-.4477 1-1V7c0-.55228-.4477-1-1-1H4c-.55228 0-1 .44771-1 1v9c0 .5523.44771 1 1 1z";--icon-mirror: "M5.00042.399902l-1.5 1.599998 1.5 1.6M15.0004.399902l1.5 1.599998-1.5 1.6M3.51995 2H16.477M8.50042 16.7V6.04604c0-.30141-.39466-.41459-.5544-.159L1.28729 16.541c-.12488.1998.01877.459.2544.459h6.65873c.16568 0 .3-.1343.3-.3zm2.99998 0V6.04604c0-.30141.3947-.41459.5544-.159L18.7135 16.541c.1249.1998-.0187.459-.2544.459h-6.6587c-.1657 0-.3-.1343-.3-.3z";--icon-flip: "M19.6001 4.99993l-1.6-1.5-1.6 1.5m3.2 9.99997l-1.6 1.5-1.6-1.5M18 3.52337V16.4765M3.3 8.49993h10.654c.3014 0 .4146-.39466.159-.5544L3.459 1.2868C3.25919 1.16192 3 1.30557 3 1.5412v6.65873c0 .16568.13432.3.3.3zm0 2.99997h10.654c.3014 0 .4146.3947.159.5544L3.459 18.7131c-.19981.1248-.459-.0188-.459-.2544v-6.6588c0-.1657.13432-.3.3-.3z";--icon-sad: "M2 17c4.41828-4 11.5817-4 16 0M16.5 5c0 .55228-.4477 1-1 1s-1-.44772-1-1 .4477-1 1-1 1 .44772 1 1zm-11 0c0 .55228-.44772 1-1 1s-1-.44772-1-1 .44772-1 1-1 1 .44772 1 1z";--icon-closeMax: "M3 3l14 14m0-14L3 17";--icon-crop: "M20 14H7.00513C6.45001 14 6 13.55 6 12.9949V0M0 6h13.0667c.5154 0 .9333.41787.9333.93333V20M14.5.399902L13 1.9999l1.5 1.6M13 2h2c1.6569 0 3 1.34315 3 3v2M5.5 19.5999l1.5-1.6-1.5-1.6M7 18H5c-1.65685 0-3-1.3431-3-3v-2";--icon-tuning: "M8 10h11M1 10h4M1 4.5h11m3 0h4m-18 11h11m3 0h4M12 4.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M5 10a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0M12 15.5a1.5 1.5 0 103 0 1.5 1.5 0 10-3 0";--icon-filters: "M4.5 6.5a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m-3.5 6a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0m7 0a5.5 5.5 0 1011 0 5.5 5.5 0 10-11 0";--icon-done: "M1 10.6316l5.68421 5.6842L19 4";--icon-original: "M0 40L40-.00000133";--icon-slider: "M0 10h11m0 0c0 1.1046.8954 2 2 2s2-.8954 2-2m-4 0c0-1.10457.8954-2 2-2s2 .89543 2 2m0 0h5";--icon-exposure: "M10 20v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M5 10a5 5 0 1010 0 5 5 0 10-10 0";--icon-contrast: "M2 10a8 8 0 1016 0 8 8 0 10-16 0m8-8v16m8-8h-8m7.5977 2.5H10m6.24 2.5H10m7.6-7.5H10M16.2422 5H10";--icon-brightness: "M15 10c0 2.7614-2.2386 5-5 5m5-5c0-2.76142-2.2386-5-5-5m5 5h-5m0 5c-2.76142 0-5-2.2386-5-5 0-2.76142 2.23858-5 5-5m0 10V5m0 15v-3M2.92946 2.92897l2.12132 2.12132M0 10h3m-.07054 7.071l2.12132-2.1213M10 0v3m7.0705 14.071l-2.1213-2.1213M20 10h-3m.0705-7.07103l-2.1213 2.12132M14.3242 7.5H10m4.3242 5H10";--icon-gamma: "M17 3C9 6 2.5 11.5 2.5 17.5m0 0h1m-1 0v-1m14 1h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3 0h1m-3-14v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1m0 3v-1";--icon-enhance: "M19 13h-2m0 0c-2.2091 0-4-1.7909-4-4m4 4c-2.2091 0-4 1.7909-4 4m0-8V7m0 2c0 2.2091-1.7909 4-4 4m-2 0h2m0 0c2.2091 0 4 1.7909 4 4m0 0v2M8 8.5H6.5m0 0c-1.10457 0-2-.89543-2-2m2 2c-1.10457 0-2 .89543-2 2m0-4V5m0 1.5c0 1.10457-.89543 2-2 2M1 8.5h1.5m0 0c1.10457 0 2 .89543 2 2m0 0V12M12 3h-1m0 0c-.5523 0-1-.44772-1-1m1 1c-.5523 0-1 .44772-1 1m0-2V1m0 1c0 .55228-.44772 1-1 1M8 3h1m0 0c.55228 0 1 .44772 1 1m0 0v1";--icon-saturation: '    <circle cx="10.0006" cy="10.0001" r="9" transform="rotate(90 10.0006 10.0001)" fill="url(#paint0_linear)"/>     <defs>       <linearGradient id="paint0_linear" x1="10.0006" y1="1.00009" x2="10.0006" y2="19.0001" gradientUnits="userSpaceOnUse">         <stop stop-color="#DE15FF"/>         <stop offset=".203125" stop-color="#0029FF"/>         <stop offset=".479167" stop-color="#2AE4F0"/>         <stop offset=".604167" stop-color="#15EF11"/>         <stop offset=".75" stop-color="#FAE528"/>         <stop offset="1" stop-color="#EB2A2A"/>       </linearGradient>     </defs>  ';--icon-warmth: '    <path d="M7.5 13.0505l.42854.4199.17146-.1749v-.245h-.6zm5 0h-.6v.245l.1715.1749.4285-.4199zM8.1 3.5c0-1.04934.85066-1.9 1.9-1.9V.4C8.28792.4 6.9 1.78792 6.9 3.5h1.2zm0 9.5505V3.5H6.9v9.5505h1.2zM7.1 15.5c0-.7904.31539-1.5059.82854-2.0296l-.85708-.8398C6.34742 13.3694 5.9 14.3831 5.9 15.5h1.2zm2.9 2.9c-1.60163 0-2.9-1.2984-2.9-2.9H5.9c0 2.2644 1.83563 4.1 4.1 4.1v-1.2zm2.9-2.9c0 1.6016-1.2984 2.9-2.9 2.9v1.2c2.2644 0 4.1-1.8356 4.1-4.1h-1.2zm-.8285-2.0296c.5131.5237.8285 1.2392.8285 2.0296h1.2c0-1.1169-.4474-2.1306-1.1715-2.8694l-.857.8398zM11.9 3.5v9.5505h1.2V3.5h-1.2zM10 1.6c1.0493 0 1.9.85066 1.9 1.9h1.2c0-1.71208-1.3879-3.1-3.1-3.1v1.2z" fill="currentColor"/>    <path d="M10 14V8" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/>    <path d="M14 3h3m-3 3h3m-3 3h3m-8 6.5a1 1 0 102 0 1 1 0 10-2 0" stroke="currentColor" stroke-width="1.2"/>  ';--icon-vibrance: '  <path d="M2.125 5.6407c-.71643 1.29152-1.12439 2.77782-1.12439 4.3594 0 1.5816.40796 3.0679 1.12439 4.3594V5.6407z" fill="url(#paint0_linear)"/>  <path d="M2.875 15.4986V4.5016c.50222-.64987 1.09136-1.22915 1.75-1.72041V17.219c-.65864-.4912-1.24778-1.0705-1.75-1.7204z" fill="url(#paint1_linear)"/>  <path d="M5.375 17.722c.54811.3291 1.13415.6014 1.75.8089V1.46929c-.61585.20751-1.20189.47984-1.75.80888V17.722z" fill="url(#paint2_linear)"/>  <path d="M7.875 1.25258V18.7476c.56442.1367 1.14962.2202 1.75.2448V1.0078c-.60038.02465-1.18558.10811-1.75.24478z" fill="url(#paint3_linear)"/>  <path d="M10.375 1.00775V18.9925c.6004-.0246 1.1856-.108 1.75-.2446V1.25228c-.5644-.13658-1.1496-.21996-1.75-.24453z" fill="url(#paint4_linear)"/>  <path d="M12.875 1.46887V18.5313c.6158-.2074 1.2019-.4796 1.75-.8085V2.27744c-.5481-.32893-1.1342-.60115-1.75-.80857z" fill="url(#paint5_linear)"/>  <path d="M15.375 2.78028V17.2199c.6586-.491 1.2477-1.0701 1.75-1.7197V4.50002c-.5023-.64963-1.0914-1.22868-1.75-1.71974z" fill="url(#paint6_linear)"/>  <path d="M17.875 5.6385v8.7232c.7172-1.292 1.1256-2.7791 1.1256-4.3616 0-1.58248-.4084-3.06956-1.1256-4.3616z" fill="url(#paint7_linear)"/>  <defs>    <linearGradient id="paint0_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint1_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint2_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint3_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint4_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint5_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint6_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>    <linearGradient id="paint7_linear" x1="19.0006" y1="10.0001" x2="1.00061" y2="10.0001" gradientUnits="userSpaceOnUse">      <stop stop-color="#DE15FF"/>      <stop offset=".203125" stop-color="#0029FF"/>      <stop offset=".479167" stop-color="#2AE4F0"/>      <stop offset=".604167" stop-color="#15EF11"/>      <stop offset=".75" stop-color="#FAE528"/>      <stop offset="1" stop-color="#EB2A2A"/>    </linearGradient>  </defs>  '}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--l10n-cancel: "Cancel";--l10n-apply: "Apply";--l10n-brightness: "Brightness";--l10n-exposure: "Exposure";--l10n-gamma: "Gamma";--l10n-contrast: "Contrast";--l10n-saturation: "Saturation";--l10n-vibrance: "Vibrance";--l10n-warmth: "Warmth";--l10n-enhance: "Enhance";--l10n-original: "Original"}:host(.lr-cloud-image-editor),.lr-cloud-image-editor{--rgb-primary-accent: 6, 2, 196;--rgb-text-base: 0, 0, 0;--rgb-text-accent-contrast: 255, 255, 255;--rgb-fill-contrast: 255, 255, 255;--rgb-fill-shaded: 245, 245, 245;--rgb-shadow: 0, 0, 0;--rgb-error: 209, 81, 81;--opacity-shade-mid: .2;--color-primary-accent: rgb(var(--rgb-primary-accent));--color-text-base: rgb(var(--rgb-text-base));--color-text-accent-contrast: rgb(var(--rgb-text-accent-contrast));--color-text-soft: rgb(var(--rgb-fill-contrast));--color-text-error: rgb(var(--rgb-error));--color-fill-contrast: rgb(var(--rgb-fill-contrast));--color-modal-backdrop: rgba(var(--rgb-fill-shaded), .95);--color-image-background: rgba(var(--rgb-fill-shaded));--color-outline: rgba(var(--rgb-text-base), var(--opacity-shade-mid));--color-underline: rgba(var(--rgb-text-base), .08);--color-shade: rgba(var(--rgb-text-base), .02);--color-focus-ring: var(--color-primary-accent);--color-input-placeholder: rgba(var(--rgb-text-base), .32);--color-error: rgb(var(--rgb-error));--font-size-ui: 16px;--font-size-title: 18px;--font-weight-title: 500;--font-size-soft: 14px;--size-touch-area: 40px;--size-panel-heading: 66px;--size-ui-min-width: 130px;--size-line-width: 1px;--size-modal-width: 650px;--border-radius-connect: 2px;--border-radius-editor: 3px;--border-radius-thumb: 4px;--border-radius-ui: 5px;--border-radius-base: 6px;--cldtr-gap-min: 5px;--cldtr-gap-mid-1: 10px;--cldtr-gap-mid-2: 15px;--cldtr-gap-max: 20px;--opacity-min: var(--opacity-shade-mid);--opacity-mid: .1;--opacity-max: .05;--transition-duration-2: var(--transition-duration-all, .2s);--transition-duration-3: var(--transition-duration-all, .3s);--transition-duration-4: var(--transition-duration-all, .4s);--transition-duration-5: var(--transition-duration-all, .5s);--shadow-base: 0px 5px 15px rgba(var(--rgb-shadow), .1), 0px 1px 4px rgba(var(--rgb-shadow), .15);--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading);--transparent-pixel: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=);display:block;width:100%;height:100%;max-height:100%}:host(.lr-cloud-image-editor) :is([can-handle-paste]:hover,[can-handle-paste]:focus),.lr-cloud-image-editor :is([can-handle-paste]:hover,[can-handle-paste]:focus){--can-handle-paste: "true"}:host(.lr-cloud-image-editor) :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover),.lr-cloud-image-editor :is([tabindex][focus-visible],[tabindex]:hover,[with-effects][focus-visible],[with-effects]:hover){--filter-effect: var(--hover-filter) !important;--opacity-effect: var(--hover-opacity) !important;--color-effect: var(--hover-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex]:active,[with-effects]:active),.lr-cloud-image-editor :is([tabindex]:active,[with-effects]:active){--filter-effect: var(--down-filter) !important;--opacity-effect: var(--down-opacity) !important;--color-effect: var(--down-color-rgb) !important}:host(.lr-cloud-image-editor) :is([tabindex][active],[with-effects][active]),.lr-cloud-image-editor :is([tabindex][active],[with-effects][active]){--filter-effect: var(--active-filter) !important;--opacity-effect: var(--active-opacity) !important;--color-effect: var(--active-color-rgb) !important}:host(.lr-cloud-image-editor) [hidden-scrollbar]::-webkit-scrollbar,.lr-cloud-image-editor [hidden-scrollbar]::-webkit-scrollbar{display:none}:host(.lr-cloud-image-editor) [hidden-scrollbar],.lr-cloud-image-editor [hidden-scrollbar]{-ms-overflow-style:none;scrollbar-width:none}:host(.lr-cloud-image-editor.editor_ON),.lr-cloud-image-editor.editor_ON{--modal-header-opacity: 0;--modal-header-height: 0px;--modal-toolbar-height: calc(var(--size-panel-heading) * 2)}:host(.lr-cloud-image-editor.editor_OFF),.lr-cloud-image-editor.editor_OFF{--modal-header-opacity: 1;--modal-header-height: var(--size-panel-heading);--modal-toolbar-height: var(--size-panel-heading)}:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-min-img-height: var(--modal-toolbar-height);--l-max-img-height: 100%;--l-edit-button-width: 120px;--l-toolbar-horizontal-padding: var(--cldtr-gap-mid-1);position:relative;display:grid;grid-template-rows:minmax(var(--l-min-img-height),var(--l-max-img-height)) minmax(var(--modal-toolbar-height),auto);height:100%;overflow:hidden;overflow-y:auto}@media only screen and (max-width: 800px){:host(.lr-cloud-image-editor)>.wrapper,.lr-cloud-image-editor>.wrapper{--l-edit-button-width: 70px;--l-toolbar-horizontal-padding: var(--cldtr-gap-min)}}:host(.lr-cloud-image-editor)>.wrapper>.viewport,.lr-cloud-image-editor>.wrapper>.viewport{display:flex;align-items:center;justify-content:center;overflow:hidden}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image{--viewer-image-opacity: 1;position:absolute;top:0;left:0;z-index:10;display:block;box-sizing:border-box;width:100%;height:100%;object-fit:scale-down;background-color:var(--color-image-background);transform:scale(1);opacity:var(--viewer-image-opacity);user-select:none;pointer-events:auto}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_visible_viewer,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_visible_viewer{transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-4)}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_to_cropper{--viewer-image-opacity: 0;background-image:var(--transparent-pixel);transform:scale(1);transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container>.image.image_hidden_effects,.lr-cloud-image-editor>.wrapper>.viewport>.image_container>.image.image_hidden_effects{--viewer-image-opacity: 0;transform:scale(1);transition:opacity var(--transition-duration-3) cubic-bezier(.5,0,1,1),transform var(--transition-duration-4);pointer-events:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.image_container,.lr-cloud-image-editor>.wrapper>.viewport>.image_container{position:relative;display:block;width:100%;height:100%;background-color:var(--color-image-background);transition:var(--transition-duration-3)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar,.lr-cloud-image-editor>.wrapper>.toolbar{position:relative;transition:.3s}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content{position:absolute;bottom:0;left:0;box-sizing:border-box;width:100%;height:var(--modal-toolbar-height);min-height:var(--size-panel-heading);background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__viewer{display:flex;align-items:center;justify-content:space-between;height:var(--size-panel-heading);padding-right:var(--l-toolbar-horizontal-padding);padding-left:var(--l-toolbar-horizontal-padding)}:host(.lr-cloud-image-editor)>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor,.lr-cloud-image-editor>.wrapper>.toolbar>.toolbar_content.toolbar_content__editor{display:flex}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.info_pan,.lr-cloud-image-editor>.wrapper>.viewport>.info_pan{position:absolute;user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer{position:absolute;z-index:2;display:flex;max-width:120px;transform:translate(-40px);user-select:none}:host(.lr-cloud-image-editor)>.wrapper>.viewport>.file_type_outer>.file_type,.lr-cloud-image-editor>.wrapper>.viewport>.file_type_outer>.file_type{padding:4px .8em}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash,.lr-cloud-image-editor>.wrapper>.network_problems_splash{position:absolute;z-index:4;display:flex;flex-direction:column;width:100%;height:100%;background-color:var(--color-fill-contrast)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content{display:flex;flex:1;flex-direction:column;align-items:center;justify-content:center}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_icon{display:flex;align-items:center;justify-content:center;width:40px;height:40px;color:rgba(var(--rgb-text-base),.6);background-color:rgba(var(--rgb-fill-shaded));border-radius:50%}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_content>.network_problems_text{margin-top:var(--cldtr-gap-max);font-size:var(--font-size-ui)}:host(.lr-cloud-image-editor)>.wrapper>.network_problems_splash>.network_problems_footer,.lr-cloud-image-editor>.wrapper>.network_problems_splash>.network_problems_footer{display:flex;align-items:center;justify-content:center;height:var(--size-panel-heading)}lr-crop-frame>.svg{position:absolute;top:0;left:0;z-index:2;width:100%;height:100%;border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);opacity:inherit;transition:var(--transition-duration-3)}lr-crop-frame>.thumb{--idle-color-rgb: var(--color-text-base);--hover-color-rgb: var(--color-primary-accent);--focus-color-rgb: var(--color-primary-accent);--down-color-rgb: var(--color-primary-accent);--color-effect: var(--idle-color-rgb);color:var(--color-effect);transition:color var(--transition-duration-3),opacity var(--transition-duration-3)}lr-crop-frame>.thumb--visible{opacity:1;pointer-events:auto}lr-crop-frame>.thumb--hidden{opacity:0;pointer-events:none}lr-crop-frame>.guides{transition:var(--transition-duration-3)}lr-crop-frame>.guides--hidden{opacity:0}lr-crop-frame>.guides--semi-hidden{opacity:.2}lr-crop-frame>.guides--visible{opacity:1}lr-editor-button-control,lr-editor-crop-button-control,lr-editor-filter-control,lr-editor-operation-control{--l-base-min-width: 40px;--l-base-height: var(--l-base-min-width);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--filter-effect: var(--idle-filter);--idle-color-rgb: var(--rgb-text-base);--idle-opacity: .05;--idle-filter: 1;--hover-color-rgb: var(--idle-color-rgb);--hover-opacity: .08;--hover-filter: .8;--down-color-rgb: var(--hover-color-rgb);--down-opacity: .12;--down-filter: .6;position:relative;display:grid;grid-template-columns:var(--l-base-min-width) auto;align-items:center;height:var(--l-base-height);color:rgba(var(--idle-color-rgb));outline:none;cursor:pointer;transition:var(--l-width-transition)}lr-editor-button-control.active,lr-editor-operation-control.active,lr-editor-crop-button-control.active,lr-editor-filter-control.active{--idle-color-rgb: var(--rgb-primary-accent)}lr-editor-filter-control.not_active .preview[loaded]{opacity:1}lr-editor-filter-control.active .preview{opacity:0}lr-editor-button-control.not_active,lr-editor-operation-control.not_active,lr-editor-crop-button-control.not_active,lr-editor-filter-control.not_active{--idle-color-rgb: var(--rgb-text-base)}lr-editor-button-control>.before,lr-editor-operation-control>.before,lr-editor-crop-button-control>.before,lr-editor-filter-control>.before{position:absolute;right:0;left:0;z-index:-1;width:100%;height:100%;background-color:rgba(var(--color-effect),var(--opacity-effect));border-radius:var(--border-radius-editor);transition:var(--transition-duration-3)}lr-editor-button-control>.title,lr-editor-operation-control>.title,lr-editor-crop-button-control>.title,lr-editor-filter-control>.title{padding-right:var(--cldtr-gap-mid-1);font-size:.7em;letter-spacing:1.004px;text-transform:uppercase}lr-editor-filter-control>.preview{position:absolute;right:0;left:0;z-index:1;width:100%;height:var(--l-base-height);background-repeat:no-repeat;background-size:contain;border-radius:var(--border-radius-editor);opacity:0;filter:brightness(var(--filter-effect));transition:var(--transition-duration-3)}lr-editor-filter-control>.original-icon{color:var(--color-text-base);opacity:.3}lr-editor-image-cropper{position:absolute;top:0;left:0;z-index:10;display:block;width:100%;height:100%;opacity:0;pointer-events:none;touch-action:none}lr-editor-image-cropper.active_from_editor{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.active_from_viewer{transform:scale(1) translate(0);opacity:1;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1) .4s,opacity var(--transition-duration-3);pointer-events:auto}lr-editor-image-cropper.inactive_to_editor{opacity:0;transition:transform var(--transition-duration-4) cubic-bezier(.37,0,.63,1),opacity var(--transition-duration-3) calc(var(--transition-duration-3) + .05s);pointer-events:none}lr-editor-image-cropper>.canvas{position:absolute;top:0;left:0;z-index:1;display:block;width:100%;height:100%}lr-editor-image-fader{position:absolute;top:0;left:0;display:block;width:100%;height:100%}lr-editor-image-fader.active_from_viewer{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-start);pointer-events:auto}lr-editor-image-fader.active_from_cropper{z-index:3;transform:scale(1);opacity:1;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:auto}lr-editor-image-fader.inactive_to_cropper{z-index:3;transform:scale(1);opacity:0;transition:transform var(--transition-duration-4),opacity var(--transition-duration-3) steps(1,jump-end);pointer-events:none}lr-editor-image-fader .fader-image{position:absolute;top:0;left:0;display:block;width:100%;height:100%;object-fit:scale-down;transform:scale(1);user-select:none;content-visibility:auto}lr-editor-image-fader .fader-image--preview{background-color:var(--color-image-background);border-top-left-radius:var(--border-radius-base);border-top-right-radius:var(--border-radius-base);transform:scale(1);opacity:0;transition:var(--transition-duration-3)}lr-editor-scroller{display:flex;align-items:center;width:100%;height:100%;overflow-x:scroll}lr-editor-slider{display:flex;align-items:center;justify-content:center;width:100%;height:66px}lr-editor-toolbar{position:relative;width:100%;height:100%}@media only screen and (max-width: 600px){lr-editor-toolbar{--l-tab-gap: var(--cldtr-gap-mid-1);--l-slider-padding: var(--cldtr-gap-min);--l-controls-padding: var(--cldtr-gap-min)}}@media only screen and (min-width: 601px){lr-editor-toolbar{--l-tab-gap: calc(var(--cldtr-gap-mid-1) + var(--cldtr-gap-max));--l-slider-padding: var(--cldtr-gap-mid-1);--l-controls-padding: var(--cldtr-gap-mid-1)}}lr-editor-toolbar>.toolbar-container{position:relative;width:100%;height:100%;overflow:hidden}lr-editor-toolbar>.toolbar-container>.sub-toolbar{position:absolute;display:grid;grid-template-rows:1fr 1fr;width:100%;height:100%;background-color:var(--color-fill-contrast);transition:opacity var(--transition-duration-3) ease-in-out,transform var(--transition-duration-3) ease-in-out,visibility var(--transition-duration-3) ease-in-out}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--visible{transform:translateY(0);opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--top-hidden{transform:translateY(100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar.sub-toolbar--bottom-hidden{transform:translateY(-100%);opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row{display:flex;align-items:center;justify-content:space-between;padding-right:var(--l-controls-padding);padding-left:var(--l-controls-padding)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles{position:relative;display:grid;grid-auto-flow:column;grid-gap:0px var(--l-tab-gap);align-items:center;height:100%}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggles_indicator{position:absolute;bottom:0;left:0;width:var(--size-touch-area);height:2px;background-color:var(--color-primary-accent);transform:translate(0);transition:transform var(--transition-duration-3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row{position:relative}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content{position:absolute;top:0;left:0;display:flex;width:100%;height:100%;overflow:hidden;opacity:0;content-visibility:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--visible{opacity:1;pointer-events:auto}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content.tab-content--hidden{opacity:0;pointer-events:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--visible{display:contents}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles>.tab-toggle.tab-toggle--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.controls-row>.tab-toggles.tab-toggles--hidden{display:none}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_align{display:grid;grid-template-areas:". inner .";grid-template-columns:1fr auto 1fr;box-sizing:border-box;min-width:100%;padding-left:var(--cldtr-gap-max)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner{display:grid;grid-area:inner;grid-auto-flow:column;grid-gap:calc((var(--cldtr-gap-min) - 1px) * 3)}lr-editor-toolbar>.toolbar-container>.sub-toolbar>.tab-content-row>.tab-content .controls-list_inner:last-child{padding-right:var(--cldtr-gap-max)}lr-editor-toolbar .controls-list_last-item{margin-right:var(--cldtr-gap-max)}lr-editor-toolbar .info-tooltip_container{position:absolute;display:flex;align-items:flex-start;justify-content:center;width:100%;height:100%}lr-editor-toolbar .info-tooltip_wrapper{position:absolute;top:calc(-100% - var(--cldtr-gap-mid-2));display:flex;flex-direction:column;justify-content:flex-end;height:100%;pointer-events:none}lr-editor-toolbar .info-tooltip{z-index:3;padding-top:calc(var(--cldtr-gap-min) / 2);padding-right:var(--cldtr-gap-min);padding-bottom:calc(var(--cldtr-gap-min) / 2);padding-left:var(--cldtr-gap-min);color:var(--color-text-base);font-size:.7em;letter-spacing:1px;text-transform:uppercase;background-color:var(--color-text-accent-contrast);border-radius:var(--border-radius-editor);transform:translateY(100%);opacity:0;transition:var(--transition-duration-3)}lr-editor-toolbar .info-tooltip_visible{transform:translateY(0);opacity:1}lr-editor-toolbar .slider{padding-right:var(--l-slider-padding);padding-left:var(--l-slider-padding)}lr-btn-ui{--filter-effect: var(--idle-brightness);--opacity-effect: var(--idle-opacity);--color-effect: var(--idle-color-rgb);--l-transition-effect: var(--css-transition, color var(--transition-duration-2), filter var(--transition-duration-2));display:inline-flex;align-items:center;box-sizing:var(--css-box-sizing, border-box);height:var(--css-height, var(--size-touch-area));padding-right:var(--css-padding-right, var(--cldtr-gap-mid-1));padding-left:var(--css-padding-left, var(--cldtr-gap-mid-1));color:rgba(var(--color-effect),var(--opacity-effect));outline:none;cursor:pointer;filter:brightness(var(--filter-effect));transition:var(--l-transition-effect);user-select:none}lr-btn-ui .text{white-space:nowrap}lr-btn-ui .icon{display:flex;align-items:center;justify-content:center;color:rgba(var(--color-effect),var(--opacity-effect));filter:brightness(var(--filter-effect));transition:var(--l-transition-effect)}lr-btn-ui .icon_left{margin-right:var(--cldtr-gap-mid-1);margin-left:0}lr-btn-ui .icon_right{margin-right:0;margin-left:var(--cldtr-gap-mid-1)}lr-btn-ui .icon_single{margin-right:0;margin-left:0}lr-btn-ui .icon_hidden{display:none;margin:0}lr-btn-ui.primary{--idle-color-rgb: var(--rgb-primary-accent);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--idle-color-rgb);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.boring{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-text-base);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: 1;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-btn-ui.default{--idle-color-rgb: var(--rgb-text-base);--idle-brightness: 1;--idle-opacity: .6;--hover-color-rgb: var(--rgb-primary-accent);--hover-brightness: 1;--hover-opacity: 1;--down-color-rgb: var(--hover-color-rgb);--down-brightness: .75;--down-opacity: 1;--active-color-rgb: var(--rgb-primary-accent);--active-brightness: 1;--active-opacity: 1}lr-line-loader-ui{position:absolute;top:0;left:0;z-index:9999;width:100%;height:2px;opacity:.5}lr-line-loader-ui .inner{width:25%;max-width:200px;height:100%}lr-line-loader-ui .line{width:100%;height:100%;background-color:var(--color-primary-accent);transform:translate(-101%);transition:transform 1s}lr-slider-ui{--l-thumb-size: 24px;--l-zero-dot-size: 5px;--l-zero-dot-offset: 2px;--idle-color-rgb: var(--rgb-text-base);--hover-color-rgb: var(--rgb-primary-accent);--down-color-rgb: var(--rgb-primary-accent);--color-effect: var(--idle-color-rgb);--l-color: rgb(var(--color-effect));position:relative;display:flex;align-items:center;justify-content:center;width:100%;height:calc(var(--l-thumb-size) + (var(--l-zero-dot-size) + var(--l-zero-dot-offset)) * 2)}lr-slider-ui .thumb{position:absolute;left:0;width:var(--l-thumb-size);height:var(--l-thumb-size);background-color:var(--l-color);border-radius:50%;transform:translate(0);opacity:1;transition:opacity var(--transition-duration-2)}lr-slider-ui .steps{position:absolute;display:flex;align-items:center;justify-content:space-between;box-sizing:border-box;width:100%;height:100%;padding-right:calc(var(--l-thumb-size) / 2);padding-left:calc(var(--l-thumb-size) / 2)}lr-slider-ui .border-step{width:0px;height:10px;border-right:1px solid var(--l-color);opacity:.6;transition:var(--transition-duration-2)}lr-slider-ui .minor-step{width:0px;height:4px;border-right:1px solid var(--l-color);opacity:.2;transition:var(--transition-duration-2)}lr-slider-ui .zero-dot{position:absolute;top:calc(100% - var(--l-zero-dot-offset) * 2);left:calc(var(--l-thumb-size) / 2 - var(--l-zero-dot-size) / 2);width:var(--l-zero-dot-size);height:var(--l-zero-dot-size);background-color:var(--color-primary-accent);border-radius:50%;opacity:0;transition:var(--transition-duration-3)}lr-slider-ui .input{position:absolute;width:calc(100% - 10px);height:100%;margin:0;cursor:pointer;opacity:0}lr-presence-toggle.transition{transition:opacity var(--transition-duration-3),visibility var(--transition-duration-3)}lr-presence-toggle.visible{opacity:1;pointer-events:inherit}lr-presence-toggle.hidden{opacity:0;pointer-events:none}ctx-provider{--color-text-base: black;--color-primary-accent: blue;display:flex;align-items:center;justify-content:center;width:190px;height:40px;padding-right:10px;padding-left:10px;background-color:#f5f5f5;border-radius:3px}lr-cloud-image-editor-activity{position:relative;display:flex;width:100%;height:100%;overflow:hidden;background-color:var(--clr-background-light)}lr-modal lr-cloud-image-editor-activity{width:min(calc(var(--modal-max-w) - var(--gap-mid) * 2),calc(100vw - var(--gap-mid) * 2));height:var(--modal-content-height-fill, 100%)}lr-select{display:inline-flex}lr-select>button{position:relative;display:inline-flex;align-items:center;padding-right:0!important;color:var(--clr-btn-txt-secondary);background-color:var(--clr-btn-bgr-secondary);box-shadow:var(--shadow-btn-secondary)}lr-select>button>select{position:absolute;display:block;width:100%;height:100%;opacity:0}
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/static/uploadcare/uploadcare.min.js` & `pyuploadcare-5.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/subclassing.py` & `pyuploadcare-5.1.0/pyuploadcare/dj/subclassing.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/dj/templates/uploadcare/forms/widgets/file.html` & `pyuploadcare-5.1.0/pyuploadcare/dj/templates/uploadcare/forms/widgets/file.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% if value %}
     <script>
         window.addEventListener('DOMContentLoaded', (e) => {
             const uploaderCtx = document.querySelector('#uploaderctx_{{ name }}');
             {% if options.multiple == "true" %}
                 {# FileGroup #}
                 {% for file in value %}
-                    uploaderCtx.addFileFromUuid("{{ file.uuid }}")
+                    uploaderCtx.addFileFromCdnUrl("{{ file.cdn_url }}")
                 {% endfor %}
             {% else %}
                 {# File #}
-                uploaderCtx.addFileFromUuid("{{ value.uuid }}")
+                uploaderCtx.addFileFromCdnUrl("{{ value.cdn_url }}")
             {% endif %}
         });
     </script>
 {% endif %}
 
 <div style="position: relative; display: flex;">
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/exceptions.py` & `pyuploadcare-5.1.0/pyuploadcare/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/helpers.py` & `pyuploadcare-5.1.0/pyuploadcare/helpers.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/base.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/base.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/file.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import dataclasses
 import logging
 import re
 import time
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 from uuid import UUID
 
 from pyuploadcare.api.entities import (
     DocumentConvertFormatInfo,
     DocumentConvertInfo,
+    Face,
     VideoConvertInfo,
 )
 from pyuploadcare.exceptions import (
     InvalidParamError,
     InvalidRequestError,
     TimeoutError,
     UploadError,
@@ -495,14 +496,18 @@
     ) -> FileGroup:
         response: DocumentConvertFormatInfo = (
             self._client.document_convert_api.retrieve(self.uuid)
         )
         group_id = response.format.converted_groups[format]
         return self._client.file_group(group_id)
 
+    def detect_faces(self) -> List[Face]:
+        response = self._client.url_api.detect_faces(self.uuid)
+        return response.faces
+
 
 class FileFromUrl:
     """Contains the logic around an upload from url.
 
     It expects uploading token, for instance::
 
         >>> ffu = FileFromUrl(token='a6a2db73-2aaf-4124-b2e7-039aec022e18')
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/file_group.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/file_group.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/file_list.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/file_list.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/group_list.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/group_list.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/resources/utils.py` & `pyuploadcare-5.1.0/pyuploadcare/resources/utils.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/secure_url.py` & `pyuploadcare-5.1.0/pyuploadcare/secure_url.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/transformations/base.py` & `pyuploadcare-5.1.0/pyuploadcare/transformations/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from typing import List, Optional, Union
+from urllib.parse import quote
 
 from typing_extensions import Self
 
 
 class StrEnum(str, Enum):
     def __str__(self):
         return self.value
@@ -24,14 +25,22 @@
     def set(self, transformation_name: str, parameters: List[str]) -> Self:
         effect = transformation_name
         if parameters:
             effect += "/" + "/".join(parameters)
         self._effects.append(effect)
         return self
 
+    def _escape_percent(self, value: Union[str, int]) -> str:
+        return str(value).replace("%", "p")
+
+    def _escape_text(self, value: str) -> str:
+        return quote(
+            value.replace("~", "~~").replace("/", "~s").replace("\n", "~n")
+        )
+
     def _prefix(self, file_id: str) -> str:
         return f"{file_id}/"
 
     def __str__(self):
         return self.effects
 
     @property
```

### Comparing `pyuploadcare-5.0.1/pyuploadcare/transformations/document.py` & `pyuploadcare-5.1.0/pyuploadcare/transformations/document.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/transformations/video.py` & `pyuploadcare-5.1.0/pyuploadcare/transformations/video.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/convert_document.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/convert_document.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/convert_video.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/convert_video.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/create_group.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/create_group.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/create_webhook.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/delete_files.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/delete_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/helpers.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/list_files.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/list_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/list_groups.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/list_groups.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/store_files.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/store_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/sync.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/update_webhook.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/update_webhook.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/upload.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/commands/upload_from_url.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/commands/upload_from_url.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/main.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/main.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/pyuploadcare/ucare_cli/settings.py` & `pyuploadcare-5.1.0/pyuploadcare/ucare_cli/settings.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-5.0.1/PKG-INFO` & `pyuploadcare-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuploadcare
-Version: 5.0.1
+Version: 5.1.0
 Summary: Python library for Uploadcare.com
 Home-page: https://uploadcare.com
 Author: Uploadcare Inc
 Author-email: hello@uploadcare.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyuploadcare Version: 5.0.1 Summary: Python library
+Metadata-Version: 2.1 Name: pyuploadcare Version: 5.1.0 Summary: Python library
 for Uploadcare.com Home-page: https://uploadcare.com Author: Uploadcare Inc
 Author-email: hello@uploadcare.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

