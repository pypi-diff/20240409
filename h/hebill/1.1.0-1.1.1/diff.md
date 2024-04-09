# Comparing `tmp/hebill-1.1.0.tar.gz` & `tmp/hebill-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.1.0.tar", last modified: Sat Apr  6 00:42:49 2024, max compression
+gzip compressed data, was "hebill-1.1.1.tar", last modified: Tue Apr  9 00:11:09 2024, max compression
```

## Comparing `hebill-1.1.0.tar` & `hebill-1.1.1.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.562644 hebill-1.1.0/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.0/LICENSE.rst
--rw-rw-rw-   0        0        0      485 2024-04-06 00:42:49.562644 hebill-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.256548 hebill-1.1.0/hebill/
--rw-rw-rw-   0        0        0      402 2024-04-06 00:41:42.000000 hebill-1.1.0/hebill/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.270102 hebill-1.1.0/hebill/dir/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:51:33.000000 hebill-1.1.0/hebill/dir/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.273098 hebill-1.1.0/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.0/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1344 2024-04-05 08:18:44.000000 hebill-1.1.0/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.277620 hebill-1.1.0/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.278619 hebill-1.1.0/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.283633 hebill-1.1.0/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.0/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.287138 hebill-1.1.0/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.0/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.0/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.0/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.289139 hebill-1.1.0/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.0/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.0/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.292139 hebill-1.1.0/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.0/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.294143 hebill-1.1.0/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.0/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.0/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.299587 hebill-1.1.0/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.0/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.0/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.303092 hebill-1.1.0/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.0/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.0/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.306102 hebill-1.1.0/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.0/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.308431 hebill-1.1.0/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.0/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.310626 hebill-1.1.0/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.0/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.0/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.312608 hebill-1.1.0/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.0/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.315610 hebill-1.1.0/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.0/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.0/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.316608 hebill-1.1.0/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.318610 hebill-1.1.0/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.0/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.0/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.322133 hebill-1.1.0/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.0/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.0/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.324350 hebill-1.1.0/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.0/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.0/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.329209 hebill-1.1.0/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.0/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.0/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.333780 hebill-1.1.0/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.337295 hebill-1.1.0/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.0/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.0/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.0/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.339307 hebill-1.1.0/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.0/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.0/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.342618 hebill-1.1.0/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.0/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.0/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.345138 hebill-1.1.0/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.0/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.0/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.348137 hebill-1.1.0/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.0/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.351138 hebill-1.1.0/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.353139 hebill-1.1.0/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.356664 hebill-1.1.0/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.0/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.0/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.360188 hebill-1.1.0/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.363186 hebill-1.1.0/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.0/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.366184 hebill-1.1.0/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.0/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.368184 hebill-1.1.0/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.0/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.371703 hebill-1.1.0/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.374042 hebill-1.1.0/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.379912 hebill-1.1.0/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.384922 hebill-1.1.0/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.386954 hebill-1.1.0/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.393463 hebill-1.1.0/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.0/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.396462 hebill-1.1.0/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.0/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.399462 hebill-1.1.0/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.0/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.401465 hebill-1.1.0/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.0/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.403916 hebill-1.1.0/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.0/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.406108 hebill-1.1.0/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.0/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.408121 hebill-1.1.0/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.0/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.411120 hebill-1.1.0/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.0/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.413122 hebill-1.1.0/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.0/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.415121 hebill-1.1.0/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.0/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.417120 hebill-1.1.0/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.0/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.419121 hebill-1.1.0/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.0/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.423482 hebill-1.1.0/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.0/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.426494 hebill-1.1.0/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.0/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.0/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.430494 hebill-1.1.0/hebill/image/
--rw-rw-rw-   0        0        0      578 2024-04-05 04:11:13.000000 hebill-1.1.0/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.438408 hebill-1.1.0/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.0/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    67930 2024-04-05 04:08:42.000000 hebill-1.1.0/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5597 2024-04-05 01:52:47.000000 hebill-1.1.0/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.443928 hebill-1.1.0/hebill/mysql/
--rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.0/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.0/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.0/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.453129 hebill-1.1.0/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.457120 hebill-1.1.0/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.460498 hebill-1.1.0/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.0/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.0/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.462511 hebill-1.1.0/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.0/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.0/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.465509 hebill-1.1.0/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.0/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.0/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.474002 hebill-1.1.0/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.0/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.0/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.0/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.0/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.477526 hebill-1.1.0/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.479825 hebill-1.1.0/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.0/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.491634 hebill-1.1.0/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.0/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.0/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.0/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.0/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.0/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.0/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.496367 hebill-1.1.0/hebill/pdf/
--rw-rw-rw-   0        0        0      168 2024-03-19 09:06:22.000000 hebill-1.1.0/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.499367 hebill-1.1.0/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.0/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2484 2024-03-20 08:24:51.000000 hebill-1.1.0/hebill/pdf/component/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.506369 hebill-1.1.0/hebill/pdf/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:17:30.000000 hebill-1.1.0/hebill/pdf/configs/__init__.py
--rw-rw-rw-   0        0        0     1422 2024-03-20 08:42:29.000000 hebill-1.1.0/hebill/pdf/configs/document_configs.py
--rw-rw-rw-   0        0        0     1385 2024-03-20 08:21:22.000000 hebill-1.1.0/hebill/pdf/configs/page_configs.py
--rw-rw-rw-   0        0        0     4894 2024-03-20 08:22:49.000000 hebill-1.1.0/hebill/pdf/configs/styles.py
--rw-rw-rw-   0        0        0      456 2024-03-20 08:21:22.000000 hebill-1.1.0/hebill/pdf/configs/template.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.0/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8076 2024-04-05 02:02:15.000000 hebill-1.1.0/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.513223 hebill-1.1.0/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.0/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.0/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.0/hebill/pdf/library/configs_selector_font.py
--rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.0/hebill/pdf/library/get_display_width.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.542059 hebill-1.1.0/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.0/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      885 2024-03-20 08:21:22.000000 hebill-1.1.0/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.0/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.0/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.0/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3002 2024-03-20 08:34:38.000000 hebill-1.1.0/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.0/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.0/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.0/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.0/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.0/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.0/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.0/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.552121 hebill-1.1.0/hebill/pypi/
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.0/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     5946 2024-04-06 00:41:04.000000 hebill-1.1.0/hebill/pypi/core.py
--rw-rw-rw-   0        0        0       39 2024-04-05 16:19:43.000000 hebill-1.1.0/hebill/pypi/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.556116 hebill-1.1.0/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.0/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.0/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.560119 hebill-1.1.0/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.0/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.0/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-06 00:42:49.561630 hebill-1.1.0/hebill.egg-info/
--rw-rw-rw-   0        0        0      485 2024-04-06 00:42:49.000000 hebill-1.1.0/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6041 2024-04-06 00:42:49.000000 hebill-1.1.0/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 00:42:49.000000 hebill-1.1.0/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-06 00:42:49.000000 hebill-1.1.0/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 00:42:49.000000 hebill-1.1.0/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2024-04-06 00:42:49.564715 hebill-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      524 2024-04-06 00:41:58.000000 hebill-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.334321 hebill-1.1.1/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      485 2024-04-09 00:11:09.334321 hebill-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.179550 hebill-1.1.1/hebill/
+-rw-rw-rw-   0        0        0      458 2024-04-08 02:02:48.000000 hebill-1.1.1/hebill/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.188740 hebill-1.1.1/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.1/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2008 2024-04-08 01:58:16.000000 hebill-1.1.1/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.189993 hebill-1.1.1/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.1/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.1/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.191398 hebill-1.1.1/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.192473 hebill-1.1.1/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.194034 hebill-1.1.1/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.1/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.195034 hebill-1.1.1/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.1/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.1/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.1/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.196355 hebill-1.1.1/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.1/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.1/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.198366 hebill-1.1.1/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.1/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.199367 hebill-1.1.1/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.1/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.1/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.201367 hebill-1.1.1/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.1/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.1/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.202304 hebill-1.1.1/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.1/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.1/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.203828 hebill-1.1.1/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.1/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.204827 hebill-1.1.1/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.1/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.206826 hebill-1.1.1/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.1/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.1/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.208404 hebill-1.1.1/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.1/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.209911 hebill-1.1.1/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.1/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.1/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.209911 hebill-1.1.1/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.213237 hebill-1.1.1/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.1/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.1/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.215231 hebill-1.1.1/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.1/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.1/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.217748 hebill-1.1.1/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.1/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.1/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.220761 hebill-1.1.1/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.1/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.1/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.224636 hebill-1.1.1/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.226286 hebill-1.1.1/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.1/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.1/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.1/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.227886 hebill-1.1.1/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.1/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.1/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.229011 hebill-1.1.1/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.1/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.1/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.230092 hebill-1.1.1/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.1/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.1/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.231443 hebill-1.1.1/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.1/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.232695 hebill-1.1.1/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.234037 hebill-1.1.1/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.235298 hebill-1.1.1/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.1/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.1/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.236715 hebill-1.1.1/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.240236 hebill-1.1.1/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.1/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.242234 hebill-1.1.1/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.1/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.243234 hebill-1.1.1/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.1/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.244745 hebill-1.1.1/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.246756 hebill-1.1.1/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.248769 hebill-1.1.1/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.249770 hebill-1.1.1/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.251763 hebill-1.1.1/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.252764 hebill-1.1.1/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.1/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.255767 hebill-1.1.1/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.1/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.257765 hebill-1.1.1/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.1/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.261764 hebill-1.1.1/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.1/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.264796 hebill-1.1.1/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.1/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.266805 hebill-1.1.1/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.1/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.267814 hebill-1.1.1/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.1/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.270420 hebill-1.1.1/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.1/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.272381 hebill-1.1.1/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.1/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.273797 hebill-1.1.1/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.1/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.275812 hebill-1.1.1/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.1/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.276813 hebill-1.1.1/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.1/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.277813 hebill-1.1.1/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.1/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.279320 hebill-1.1.1/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.1/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.1/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.280329 hebill-1.1.1/hebill/image/
+-rw-rw-rw-   0        0        0      578 2024-04-05 04:11:13.000000 hebill-1.1.1/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.283337 hebill-1.1.1/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.1/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    67932 2024-04-06 01:07:24.000000 hebill-1.1.1/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.1/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.286011 hebill-1.1.1/hebill/mysql/
+-rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.1/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.1/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.1/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.289983 hebill-1.1.1/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.289983 hebill-1.1.1/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.292446 hebill-1.1.1/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.1/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.1/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.293444 hebill-1.1.1/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.1/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.1/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.294677 hebill-1.1.1/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.1/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.1/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.297209 hebill-1.1.1/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.1/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.1/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.1/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.1/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.298632 hebill-1.1.1/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.300643 hebill-1.1.1/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.1/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.304601 hebill-1.1.1/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.1/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.1/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.1/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.1/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.1/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.1/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.307092 hebill-1.1.1/hebill/pdf/
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:06:22.000000 hebill-1.1.1/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.308426 hebill-1.1.1/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.1/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-03-20 08:24:51.000000 hebill-1.1.1/hebill/pdf/component/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.312409 hebill-1.1.1/hebill/pdf/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:17:30.000000 hebill-1.1.1/hebill/pdf/configs/__init__.py
+-rw-rw-rw-   0        0        0     1422 2024-03-20 08:42:29.000000 hebill-1.1.1/hebill/pdf/configs/document_configs.py
+-rw-rw-rw-   0        0        0     1385 2024-03-20 08:21:22.000000 hebill-1.1.1/hebill/pdf/configs/page_configs.py
+-rw-rw-rw-   0        0        0     4894 2024-03-20 08:22:49.000000 hebill-1.1.1/hebill/pdf/configs/styles.py
+-rw-rw-rw-   0        0        0      456 2024-03-20 08:21:22.000000 hebill-1.1.1/hebill/pdf/configs/template.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.1/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8076 2024-04-05 02:02:15.000000 hebill-1.1.1/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.315920 hebill-1.1.1/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.1/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.1/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.1/hebill/pdf/library/configs_selector_font.py
+-rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.1/hebill/pdf/library/get_display_width.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.326495 hebill-1.1.1/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.1/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      885 2024-03-20 08:21:22.000000 hebill-1.1.1/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.1/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.1/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.1/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3002 2024-03-20 08:34:38.000000 hebill-1.1.1/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.1/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.1/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.1/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.1/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.1/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.1/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.1/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.327856 hebill-1.1.1/hebill/pypi/
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.1/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     7219 2024-04-09 00:11:07.000000 hebill-1.1.1/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.328865 hebill-1.1.1/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.1/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.1/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.330794 hebill-1.1.1/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.1/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.1/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:11:09.332310 hebill-1.1.1/hebill.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-04-09 00:11:09.000000 hebill-1.1.1/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6049 2024-04-09 00:11:09.000000 hebill-1.1.1/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 00:11:09.000000 hebill-1.1.1/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-09 00:11:09.000000 hebill-1.1.1/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 00:11:09.000000 hebill-1.1.1/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2024-04-09 00:11:09.335504 hebill-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      524 2024-04-09 00:11:08.000000 hebill-1.1.1/setup_by_hebill.py
```

### Comparing `hebill-1.1.0/hebill/file/core.py` & `hebill-1.1.1/hebill/file/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 import os
-import psutil
+from ..dir.core import Dir
 
 
-class File:
-    def __init__(self, file: str):
-        self._file = file
+class File(str):
+    def __init__(self, path: str):
+        self._input = path
 
     @property
-    def file(self) -> str: return self._file
+    def path(self) -> str:
+        return os.path.abspath(self._input)
+
+    @property
+    def name(self) -> str:
+        return os.path.basename(self._input)
+
+    @property
+    def parent(self):
+        return Dir(self.parent_path)
+
+    @property
+    def parent_path(self) -> str:
+        return os.path.abspath(os.path.dirname(self.path))
+
+    @property
+    def parent_name(self) -> str:
+        return os.path.basename(os.path.dirname(self.path))
+
+    def exists(self): return os.path.isfile(self.path)
 
     def _read_file(self):
         try:
             with open(self.absolute_path, 'r') as file:
                 result = []
                 lines = file.readlines()
                 for line in lines:
@@ -24,22 +43,27 @@
     def read_content(self):
         return '\n'.join(self._read_file())
 
     def read_lines(self):
         return self._read_file()
 
     @property
-    def absolute_path(self) -> str: return os.path.abspath(self._file)
+    def absolute_path(self) -> str: return os.path.abspath(self.path)
 
     @property
-    def basename(self) -> str: return os.path.basename(self._file)
+    def basename(self) -> str: return os.path.basename(self.path)
 
     def is_occupied(self):
+        import psutil
         for proc in psutil.process_iter():
             try:
                 files = proc.open_files()  # 获取进程打开的文件列表
                 for f in files:  # 检查文件路径是否匹配
                     if f.path == self.absolute_path:  # 文件被锁定
                         return True
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 pass
         return False
+
+    def delete(self):
+        if self.exists():
+            os.remove(self.absolute_path)
```

### Comparing `hebill-1.1.0/hebill/html/components/html/head/core.py` & `hebill-1.1.1/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/components/table/core.py` & `hebill-1.1.1/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/components/table/tbody/core.py` & `hebill-1.1.1/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.1.1/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/components/table/thead/core.py` & `hebill-1.1.1/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/components/table/thead/tr/core.py` & `hebill-1.1.1/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/core.py` & `hebill-1.1.1/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/comment/core.py` & `hebill-1.1.1/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/group/core.py` & `hebill-1.1.1/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/group/create/core.py` & `hebill-1.1.1/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.1.1/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.1.1/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/node/core.py` & `hebill-1.1.1/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.1.1/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.1.1/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.1.1/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/nodes/tag/core.py` & `hebill-1.1.1/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/html/tags/__init__.py` & `hebill-1.1.1/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/image/__init__.py` & `hebill-1.1.1/hebill/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/image/png/constants.py` & `hebill-1.1.1/hebill/image/png/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 ICO_MAXIMIZE = 'iVBORw0KGgoAAAANSUhEUgAAAB4AAAAeCAYAAAA7MK6iAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAS0lEQVR4nO3WQQoAIAhE0bn/sZLOZSeQBBOi/gN3woDMQgk/mpL88Fgm2JtmK72YRHCIU1dRrhDlqqJcIcpVRbnue32sIXRkgvGWBcTLnnJ2JY0JAAAAAElFTkSuQmCC'
 ICO_MINIMIZE = 'iVBORw0KGgoAAAANSUhEUgAAAB4AAAAeCAYAAAA7MK6iAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAQElEQVR4nO3RQQoAEAAF0Tke7r+m5B6sbGVBKfPqr2fxQZKkTQkoQD+8AsRVuF6IzrUnwxHIF6IZCLt/S5I+NwDHN1vXMmzw6wAAAABJRU5ErkJggg=='
 ICO_MORE = 'iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAzUlEQVR4nO3TQQqCQBgF4O5RLszKwhKDblyRiaRRgYi3KU1Th/QCfwy4CZ1oFQO9b//e4p95vR4AAAAAAAAAtKyCUrEi5lohq82grI1z4S38XJctJyxbRqy0QkZmUNL8UpBxymnqZ0zzboosOaHmEm9ls+OD9ENGYzd1ZMkJNc/YKpu4KWlOUsmSE+J/sKts5NxpuIufsuSE+IA6y+yE1E28lyUnxNfPB9Qq28ZFf30dyJL7iK+fD4j/QdWOK36Jb8p+nQMAAAAAAAD4Ry/WvNE3Me+8hgAAAABJRU5ErkJggg=='
 ICO_NORMALIZE = 'iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAqElEQVR4nO3ZQQrDMAxFwXf/S6sn6CqObdoZ0D4ISR+cAgCAVeaSOmYuKQ04ZS6paxqwiwZkArICuQE5gr10fOeSOpYCc0lpwBcmoM0rsMu1K7CLBmQCsgK5ATmCSYHEYM/j8vU8Xk0MJgYTg4nBxGBiMDHY86ez1/N4tdVvh8s+ZBcNyAR0YvKuXYFjRgMyAWMFcgPm0p+j24/gaEAmYP5pBQAA6Id8AMBkDR6uWW+2AAAAAElFTkSuQmCC'
 ICO_QUITE = 'iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAACXBIWXMAAAsTAAALEwEAmpwYAAAB7ElEQVR4nO2Z3UrDMBTH81Amft01012oCOKt+BAqKA4miCJ44Y0PIIj4id6IdzrfwyFDbzargjYbrZVFWtexuXY2TZN0kD+cu5X9fzkn56QNAFpaWlqZVh2jWWKge8tAhGBEZYTl/ZcBS3VjaIbLvIXRjizTJAoGw63kK6/YPGkHnGYG8MomQwB37AAYWhkC+EwAoNo06goNQKJWJz9GSW54QDOQH6ffN9fUPT1ihrALK36oA2iZp+a7HywQ9voSpVWT0tortTfW1AC4Z8dt80F8HR78C9E2HzxXiweROkBjYY42H8o9EP0y0WPebAEUV9XsARYIHvNEZBuNA8FrnoieA/0g7MIyt3kiY5BFQdCXN27zRNYkjoTgNE9kHiV8iMpTaCbsYryeT1QC+Bu29qfmgz1xwj6xiUyA0G6TEgQQDRDVKpuV51QggEiAfn0+ssUyQgBRAHGGVBoQQAQAy4TlhQBpAyQ5HjQW52mz/Bh+isWSAdyri24jVTPWC0pYJpz9PQUlNDFC3cvzRBO2E8KJYV7cJp4c9TPB8mrYWU7O7nbs34sBkBhAA+CBywDMzqdFA36wAxiwpNw4DgLeMgN4lwvqjaPfyKEpkETe5YJq85aBNgGPvMsF7/u83D0BLa9sEq+8lpaWFpClH85QF54vuUIVAAAAAElFTkSuQmCC'
 ICO_SETTING = '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'
 ICO_USER = 'iVBORw0KGgoAAAANSUhEUgAAACgAAAAoCAYAAACM/rhtAAAACXBIWXMAAAsTAAALEwEAmpwYAAAFA0lEQVR4nN3W609TZxwH8GZvtmT/wa5vd4l/wZb4Ziq9g8bEIRMWYzaopVx64TKDomMTI8LUltPSgy3ltAwiCChCewr2dkoYQ4FtsnHTIVTuSK9c+lueE8Zgg1HktCx7km/65Lnk+eR5znlOWaz/c9Glxh2sFvNVhEQ4bBDzX+hSOauGs/wFU4bQpfuSnVhQUPDKvsCqvoj7gMgQ9NRJjy72YrLV6cYrELDchLBdQ/8+MRVCU17iojFd6NZnH3o9pjidiHukWizwDtzKD4ftFQCOrYP6HFdSA0aJsCVmuFtpRz5EuMmG4m1hsCGrNjXUSo8G9Wm8oFEi7NSlcj+JKtAoEfb/pj8XjgQHG+K33IAR4jzUZCZ4q8S8rKjg9CL2odvy44v/dqywQ3xt14GQCHy4iH2AcWC1RHCrX6PY1e5N1hfD3N2STW19avkKIeHrGQcSkvins81XI8Yt3LsGtbJjUJOdAMPV59fb5++WAJEuGGccaBDzfUFSGRFuBD1v2QkwRF6E+cc3oFZxDJ6aCum+5Q4M9CJuiHGgTsRZQW/l3zFBUglzzSUwXlcEvWop3PnqBDQVnoSp3lKA2So6031lNBiNDbWrwHCWF2AcaDjLe4EuYYR6fvsytF5KAWNmPHwvPwZ3Cj6F1uLPocuQDZ7uq+uwjaHwdOhRZsFM01UwZsQ/YRxozBT2e25/S+8UQg1ZL8Ly88otMVtl8uE1qM89DqPEBQS0Mg6sEvPLHpVLV5vPJcKo/euIYbCWpQkcDOk8oEpEQb2II2UcWH+Bfakx/0TYIObB0kTkOwcbokvjQK3saLi+KI55YJuas0BkCOhFXgYHa8AaWTyYKzgLjAPNWs6c5bukPQM7sGQwa9lzjAMtOJegTJ8t7xVImZJWSJxbxTiQrOC8a8HZs2YNG8Iz+l3jwjN6QHPNOHv2Pn74bVY0SpuG874F5y6HJtS7BoYmNGDW8pbvY4ffY0WzWHUCarK/aNfA531F0K7jO1nRLm0V7DM/NCQv7hbY1ZDsbdVyTkcd2F558DUS53qmfr4c+Vfkp2/AgvMm7pXFvcqKRTFjcR+TlXzfwtBffwi2y/xgKZCVfG+rhv1RTHDryAoOl8R5MEQpYGXqn18W1DbkkgMaY9Gy2az9KG2aOOhqOAlkJQ/6zWkQeFZOB9VRW1dDEqAx+4L7E+jpz4dnPQp4eC8FOvRCOqiO2lBfTIEKzP6OXOlMz9NQrhwNNY4Wn+jLpyFbBfWhMWgsmiMtd4izbj5g/pKWl7nfUmAUkYNR/tK7A76aH6ehZTAAZJ0EHrWe2RbY23oGrHUZ9Fg0p7R5wKfAKH+OmqrOVLneZAQnVdkTZJjTpyZHl6y/r4DNA+t5MDoDJHEK3A0pMExlwHhvLh1Ud9cng4U4RY/ZOId8ugyYZTSkKHd5s5QOwZ5wMqUzO1/b6W18vLhpkU3IMT9YbQYgTafBjPPpoHq7vRpsY/5t5zX+sgh52k6vAnNlvvTO5VW4vfeHg9suYttj2kZCgNaQqhzCXT9zcpXT1zzgixrOtpamAS/IMadXdt3xRsTAHLXLiFlGg9HG2daiMo+E0IsT8VWiwFxB69jmFyKasY6tAFoTndzOx6t0ppc1/+qLFc62FnQFoXtyR2Cuxu2q6Z6OKc7mATB1T0Ouxm2P5PnztAwFYg5sGQxAjpp6tiNQpnL4pUoH7EdkKod/R+B/rfwBBuK/i4zrKkUAAAAASUVORK5CYII='
+
 ICO_HEBILL = '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'
 ICO_YANGS = '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'
```

### Comparing `hebill-1.1.0/hebill/image/png/core.py` & `hebill-1.1.1/hebill/image/png/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,58 +130,68 @@
 class PNGIconHelp(PNG):
     def __init__(self):
         super().__init__(ICO_HELP)
 
 
 class PNGIconHome(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_HOME)
 
 
 class PNGIconIcon(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_ICON)
 
 
 class PNGIconInfo(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_INFO)
 
 
 class PNGIconLangauge(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_LANGUAGE)
 
 
 class PNGIconMaximize(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_MAXIMIZE)
 
 
 class PNGIconMinimize(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_MINIMIZE)
 
 
 class PNGIconMore(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_MORE)
 
 
 class PNGIconNormalize(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_NORMALIZE)
 
 
 class PNGIconQuite(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_QUITE)
 
 
 class PNGIconSetting(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_SETTING)
 
 
 class PNGIconUser(PNG):
     def __init__(self):
-        super().__init__(ICO_DEMO)
+        super().__init__(ICO_USER)
+
+
+class PNGIconHebill(PNG):
+    def __init__(self):
+        super().__init__(ICO_HEBILL)
+
+
+class PNGIconYangs(PNG):
+    def __init__(self):
+        super().__init__(ICO_YANGS)
```

### Comparing `hebill-1.1.0/hebill/mysql/core.py` & `hebill-1.1.1/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/features/table_describe_data.py` & `hebill-1.1.1/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/features/table_index_data.py` & `hebill-1.1.1/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/features/table_status_data.py` & `hebill-1.1.1/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/plugins/columns/core.py` & `hebill-1.1.1/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/plugins/limits/core.py` & `hebill-1.1.1/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/plugins/orders/core.py` & `hebill-1.1.1/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.1.1/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.1.1/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/core.py` & `hebill-1.1.1/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/data/core.py` & `hebill-1.1.1/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/data/drop.py` & `hebill-1.1.1/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/data/insert.py` & `hebill-1.1.1/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/data/search.py` & `hebill-1.1.1/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/mysql/table/data/update.py` & `hebill-1.1.1/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/component/core.py` & `hebill-1.1.1/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/configs/document_configs.py` & `hebill-1.1.1/hebill/pdf/configs/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/configs/page_configs.py` & `hebill-1.1.1/hebill/pdf/configs/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/configs/styles.py` & `hebill-1.1.1/hebill/pdf/configs/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/constants.py` & `hebill-1.1.1/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/core.py` & `hebill-1.1.1/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/library/configs_selector_color.py` & `hebill-1.1.1/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/library/configs_selector_font.py` & `hebill-1.1.1/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/library/get_display_width.py` & `hebill-1.1.1/hebill/pdf/library/get_display_width.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/_draw_.py` & `hebill-1.1.1/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/core.py` & `hebill-1.1.1/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/draw_grids.py` & `hebill-1.1.1/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/draw_path.py` & `hebill-1.1.1/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/draw_rect.py` & `hebill-1.1.1/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pdf/page/draw_string.py` & `hebill-1.1.1/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.0/hebill/pypi/core.py` & `hebill-1.1.1/hebill/pypi/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os.path
+import subprocess
+import sys
 
 import hebill
-setup_data = None
+import glob
 
 
 class Pypi:
     def __init__(self):
         self._name = None
         self._version = None
         self._description = None
@@ -14,14 +16,15 @@
         self._packages = []
         self._install_requires = {}
         self._entry_point_console_scripts = {}
         self._python_requires = '3.12'
         self._output_build_base = ''
         self._output_dist_dir = ''
         self._output_egg_base = ''
+        self._setup_py = 'setup_by_hebill.py'
 
     @property
     def name(self): return self._name
 
     @name.setter
     def name(self, name: str): self._name = name
 
@@ -87,15 +90,25 @@
 
     @property
     def output_egg_base(self): return self._output_egg_base
 
     @output_egg_base.setter
     def output_egg_base(self, path: str): self._output_egg_base = path
 
-    def pack(self):
+    @property
+    def setup_py(self): return self._setup_py
+
+    @setup_py.setter
+    def setup_py(self, filename: str): self._setup_py = filename
+
+    def build(self):
+        from ..dir.core import Dir
+        Dir('build').delete()
+        Dir('dist').delete()
+        Dir('hebill.egg-info').delete()
         lines = [
             '# -*- coding: utf-8 -*-',
             'from setuptools import setup',
             'setup(',
             f'    name=\'{self.name if self.name else 'My Module'}\',',
             f'    version=\'{self.version if self.version else '1.0.0'}\',',
         ]
@@ -136,18 +149,42 @@
                 lines.append(f'{' '*8}}},')
             if self.output_egg_base:
                 lines.append(f'{' '*8}\'bdist_egg\': {{')
                 lines.append(f'{' '*12}\'egg_base\': r\'{self.output_egg_base}\',')
                 lines.append(f'{' '*8}}},')
             lines.append(f'{' '*4}}},')"""
         lines.append(')\n')
-        with open('setup.py', 'w') as file:
-            file.write('\n'.join(lines))
-        command = ['python', 'setup.py', 'sdist', 'bdist_wheel']
-        """if self.output_build_base:
-            command.extend(["--build-base", self.output_build_base])"""
-        """if self.output_dist_dir:
-            command.extend(["--dist-dir", self.output_dist_dir])"""
-        """if self.output_egg_base:
-            command.extend(["--egg-base", self.output_egg_base])"""
+        try:
+            with open(self.setup_py, 'w') as file:
+                file.write('\n'.join(lines))
+            print(f'{self.setup_py} 文件已经生成：{self.setup_py}')
+        except (Exception, IOError) as e:
+            print(f'{self.setup_py} 文件生成失败[{e}]')
+            return
 
-        print(' '.join(command))
+    def pack(self):
+        self.build()
+        command = [r'E:\PythonEnvs\hebill\Scripts\python.exe', self.setup_py, 'sdist', 'bdist_wheel']
+        if self.output_build_base:
+            command.extend(["--build-base", self.output_build_base])
+        if self.output_dist_dir:
+            command.extend(["--dist-dir", self.output_dist_dir])
+        if self.output_egg_base:
+            command.extend(["--egg-base", self.output_egg_base])
+        print(f"执行命令：{' '.join(command)}")
+        result = subprocess.run(' '.join(command))
+
+        if result.returncode == 0:
+            print("打包处理执行完成，下面开始上传")
+        else:
+            print("打包处理执行失败！")
+            return
+
+        '''dist_files = glob.glob('dist/*')'''
+        command = ['twine', 'upload', 'dist/*']  #  + dist_files
+        print(f"执行命令：{' '.join(command)}")
+        result = subprocess.run(command)
+        if result.returncode == 0:
+            print("上传成功")
+        else:
+            print("上传失败！")
+            return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hebill-1.1.0/hebill.egg-info/SOURCES.txt` & `hebill-1.1.1/hebill.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE.rst
 setup.cfg
-setup.py
+setup_by_hebill.py
 hebill/__init__.py
 hebill.egg-info/PKG-INFO
 hebill.egg-info/SOURCES.txt
 hebill.egg-info/dependency_links.txt
 hebill.egg-info/requires.txt
 hebill.egg-info/top_level.txt
 hebill/dir/__init__.py
+hebill/dir/core.py
 hebill/file/__init__.py
 hebill/file/core.py
 hebill/html/__init__.py
 hebill/html/core.py
 hebill/html/components/__init__.py
 hebill/html/components/html/__init__.py
 hebill/html/components/html/core.py
@@ -166,12 +167,11 @@
 hebill/pdf/page/draw_grids.py
 hebill/pdf/page/draw_line.py
 hebill/pdf/page/draw_path.py
 hebill/pdf/page/draw_rect.py
 hebill/pdf/page/draw_string.py
 hebill/pypi/__init__.py
 hebill/pypi/core.py
-hebill/pypi/setup.py
 hebill/sys/__init__.py
 hebill/sys/core.py
 hebill/url/__init__.py
 hebill/url/core.py
```

### Comparing `hebill-1.1.0/setup.py` & `hebill-1.1.1/setup_by_hebill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(
     name='hebill',
-    version='1.1.0',
+    version='1.1.1',
     description='Python Hebill',
     long_description=open(r'E:\PythonProjects\hebill\README.MD').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
```

