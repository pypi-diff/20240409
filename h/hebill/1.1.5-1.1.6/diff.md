# Comparing `tmp/hebill-1.1.5.tar.gz` & `tmp/hebill-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.1.5.tar", last modified: Tue Apr  9 02:09:59 2024, max compression
+gzip compressed data, was "hebill-1.1.6.tar", last modified: Tue Apr  9 02:35:07 2024, max compression
```

## Comparing `hebill-1.1.5.tar` & `hebill-1.1.6.tar`

### file list

```diff
@@ -1,259 +1,265 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.872401 hebill-1.1.5/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.5/LICENSE.rst
--rw-rw-rw-   0        0        0      487 2024-04-09 02:09:59.872401 hebill-1.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.732994 hebill-1.1.5/hebill/
--rw-rw-rw-   0        0        0      402 2024-04-09 02:09:58.000000 hebill-1.1.5/hebill/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.738503 hebill-1.1.5/hebill/dir/
--rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.5/hebill/dir/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.5/hebill/dir/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.739947 hebill-1.1.5/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.5/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.5/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.742331 hebill-1.1.5/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.742331 hebill-1.1.5/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.743327 hebill-1.1.5/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.5/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.744798 hebill-1.1.5/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.5/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.5/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.5/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.746142 hebill-1.1.5/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.5/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.5/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.747506 hebill-1.1.5/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.5/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.748516 hebill-1.1.5/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.5/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.5/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.750514 hebill-1.1.5/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.5/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.5/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.750514 hebill-1.1.5/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.5/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.5/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.753031 hebill-1.1.5/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.5/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.754031 hebill-1.1.5/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.5/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.755032 hebill-1.1.5/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.5/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.5/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.756031 hebill-1.1.5/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.5/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.758032 hebill-1.1.5/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.5/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.5/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.758032 hebill-1.1.5/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.759584 hebill-1.1.5/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.5/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.5/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.760592 hebill-1.1.5/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.5/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.5/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.761964 hebill-1.1.5/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.5/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.5/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.762974 hebill-1.1.5/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.5/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.5/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.763973 hebill-1.1.5/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.764973 hebill-1.1.5/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.5/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.5/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.5/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.766466 hebill-1.1.5/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.5/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.5/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.768483 hebill-1.1.5/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.5/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.5/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.769480 hebill-1.1.5/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.5/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.5/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.770995 hebill-1.1.5/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.5/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.771994 hebill-1.1.5/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.773325 hebill-1.1.5/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.774477 hebill-1.1.5/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.5/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.5/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.775487 hebill-1.1.5/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.776905 hebill-1.1.5/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.5/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.777912 hebill-1.1.5/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.5/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.780140 hebill-1.1.5/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.5/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.781148 hebill-1.1.5/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.782148 hebill-1.1.5/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.783149 hebill-1.1.5/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.784146 hebill-1.1.5/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.786333 hebill-1.1.5/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.788004 hebill-1.1.5/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.5/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.790017 hebill-1.1.5/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.5/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.793018 hebill-1.1.5/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.5/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.795538 hebill-1.1.5/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.5/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.796957 hebill-1.1.5/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.5/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.798965 hebill-1.1.5/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.5/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.800513 hebill-1.1.5/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.5/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.803588 hebill-1.1.5/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.5/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.805596 hebill-1.1.5/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.5/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.806840 hebill-1.1.5/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.5/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.808850 hebill-1.1.5/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.5/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.811370 hebill-1.1.5/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.5/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.812378 hebill-1.1.5/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.5/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.813894 hebill-1.1.5/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.5/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.5/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.814908 hebill-1.1.5/hebill/image/
--rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.1.5/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.816905 hebill-1.1.5/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.5/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    67932 2024-04-06 01:07:24.000000 hebill-1.1.5/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.5/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.820361 hebill-1.1.5/hebill/mysql/
--rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.5/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.5/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.5/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.822369 hebill-1.1.5/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.823876 hebill-1.1.5/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.824887 hebill-1.1.5/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.5/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.5/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.825883 hebill-1.1.5/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.5/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.5/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.827885 hebill-1.1.5/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.5/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.5/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.829885 hebill-1.1.5/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.5/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.5/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.5/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.5/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.831589 hebill-1.1.5/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.832967 hebill-1.1.5/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.5/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.841817 hebill-1.1.5/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.5/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.5/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.5/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.5/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.5/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.5/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.845771 hebill-1.1.5/hebill/numeric/
--rw-rw-rw-   0        0        0        0 2024-03-20 09:54:40.000000 hebill-1.1.5/hebill/numeric/__init__.py
--rw-rw-rw-   0        0        0      108 2024-03-20 12:33:50.000000 hebill-1.1.5/hebill/numeric/capitalize_numbers.py
--rw-rw-rw-   0        0        0     1077 2024-03-21 12:39:19.000000 hebill-1.1.5/hebill/numeric/constants.py
--rw-rw-rw-   0        0        0    13381 2024-03-21 15:31:11.000000 hebill-1.1.5/hebill/numeric/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.847314 hebill-1.1.5/hebill/pdf/
--rw-rw-rw-   0        0        0      309 2024-04-09 02:09:58.000000 hebill-1.1.5/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.848450 hebill-1.1.5/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.5/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/component/core.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.5/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8079 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.853820 hebill-1.1.5/hebill/pdf/features/
--rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.1.5/hebill/pdf/features/__init__.py
--rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/features/configs.py
--rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/features/document_configs.py
--rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/features/page_configs.py
--rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/features/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.855828 hebill-1.1.5/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.5/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.5/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.5/hebill/pdf/library/configs_selector_font.py
--rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.5/hebill/pdf/library/get_display_width.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.865436 hebill-1.1.5/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.5/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.5/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.5/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.5/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.1.5/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.5/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.5/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.5/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.5/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.5/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.5/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.5/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.867436 hebill-1.1.5/hebill/pypi/
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.5/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     7849 2024-04-09 01:50:41.000000 hebill-1.1.5/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.868435 hebill-1.1.5/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.5/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.5/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.869942 hebill-1.1.5/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.5/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.5/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 02:09:59.871389 hebill-1.1.5/hebill.egg-info/
--rw-rw-rw-   0        0        0      487 2024-04-09 02:09:59.000000 hebill-1.1.5/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6168 2024-04-09 02:09:59.000000 hebill-1.1.5/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 02:09:59.000000 hebill-1.1.5/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-09 02:09:59.000000 hebill-1.1.5/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 02:09:59.000000 hebill-1.1.5/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2024-04-09 02:09:59.873400 hebill-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      524 2024-04-09 02:09:59.000000 hebill-1.1.5/setup_by_hebill.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.169151 hebill-1.1.6/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.6/LICENSE.rst
+-rw-rw-rw-   0        0        0      487 2024-04-09 02:35:07.169151 hebill-1.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.969024 hebill-1.1.6/hebill/
+-rw-rw-rw-   0        0        0      402 2024-04-09 02:35:05.000000 hebill-1.1.6/hebill/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.976441 hebill-1.1.6/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.6/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.6/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.977449 hebill-1.1.6/hebill/excel/
+-rw-rw-rw-   0        0        0      116 2024-04-09 02:35:05.000000 hebill-1.1.6/hebill/excel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.979796 hebill-1.1.6/hebill/excel/methods/
+-rw-rw-rw-   0        0        0        0 2024-04-09 02:32:59.000000 hebill-1.1.6/hebill/excel/methods/__init__.py
+-rw-rw-rw-   0        0        0      161 2024-04-09 02:35:05.000000 hebill-1.1.6/hebill/excel/methods/letters_to_number.py
+-rw-rw-rw-   0        0        0      196 2024-04-09 02:35:05.000000 hebill-1.1.6/hebill/excel/methods/number_to_letters.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.981130 hebill-1.1.6/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.6/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.6/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.982303 hebill-1.1.6/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.983755 hebill-1.1.6/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.983755 hebill-1.1.6/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.6/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.986253 hebill-1.1.6/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.6/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.6/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.6/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:06.988227 hebill-1.1.6/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.6/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.6/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.003351 hebill-1.1.6/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.6/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.007738 hebill-1.1.6/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.6/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.6/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.009366 hebill-1.1.6/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.6/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.6/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.010379 hebill-1.1.6/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.6/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.6/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.013374 hebill-1.1.6/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.6/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.014887 hebill-1.1.6/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.6/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.016888 hebill-1.1.6/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.6/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.6/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.017888 hebill-1.1.6/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.6/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.023940 hebill-1.1.6/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.6/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.6/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.025957 hebill-1.1.6/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.033974 hebill-1.1.6/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.6/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.6/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.036968 hebill-1.1.6/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.6/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.6/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.038967 hebill-1.1.6/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.6/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.6/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.041478 hebill-1.1.6/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.6/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.6/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.043517 hebill-1.1.6/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.044488 hebill-1.1.6/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.6/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.6/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.6/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.046488 hebill-1.1.6/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.6/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.6/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.048489 hebill-1.1.6/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.6/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.6/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.049490 hebill-1.1.6/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.6/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.6/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.053016 hebill-1.1.6/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.6/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.055009 hebill-1.1.6/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.057008 hebill-1.1.6/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.058517 hebill-1.1.6/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.6/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.6/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.059527 hebill-1.1.6/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.061525 hebill-1.1.6/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.6/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.063042 hebill-1.1.6/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.6/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.065041 hebill-1.1.6/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.6/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.067765 hebill-1.1.6/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.069776 hebill-1.1.6/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.071778 hebill-1.1.6/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.073293 hebill-1.1.6/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.075804 hebill-1.1.6/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.076816 hebill-1.1.6/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.6/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.078819 hebill-1.1.6/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.6/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.080815 hebill-1.1.6/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.6/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.082324 hebill-1.1.6/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.6/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.084332 hebill-1.1.6/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.6/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.085332 hebill-1.1.6/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.6/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.087332 hebill-1.1.6/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.6/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.088387 hebill-1.1.6/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.6/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.090367 hebill-1.1.6/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.6/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.091337 hebill-1.1.6/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.6/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.092840 hebill-1.1.6/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.6/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.093848 hebill-1.1.6/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.6/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.095858 hebill-1.1.6/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.6/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.096858 hebill-1.1.6/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.6/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.6/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.097858 hebill-1.1.6/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.1.6/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.101086 hebill-1.1.6/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.6/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    67932 2024-04-06 01:07:24.000000 hebill-1.1.6/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.6/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.104345 hebill-1.1.6/hebill/mysql/
+-rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.6/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.6/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.6/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.108369 hebill-1.1.6/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.109880 hebill-1.1.6/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.110890 hebill-1.1.6/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.6/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.6/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.114174 hebill-1.1.6/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.6/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.6/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.115069 hebill-1.1.6/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.6/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.6/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.119069 hebill-1.1.6/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.6/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.6/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.6/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.6/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.121069 hebill-1.1.6/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.122069 hebill-1.1.6/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.6/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.129216 hebill-1.1.6/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.6/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.6/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.6/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.6/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.6/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.6/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.132029 hebill-1.1.6/hebill/numeric/
+-rw-rw-rw-   0        0        0        0 2024-03-20 09:54:40.000000 hebill-1.1.6/hebill/numeric/__init__.py
+-rw-rw-rw-   0        0        0      108 2024-03-20 12:33:50.000000 hebill-1.1.6/hebill/numeric/capitalize_numbers.py
+-rw-rw-rw-   0        0        0     1077 2024-03-21 12:39:19.000000 hebill-1.1.6/hebill/numeric/constants.py
+-rw-rw-rw-   0        0        0    13381 2024-03-21 15:31:11.000000 hebill-1.1.6/hebill/numeric/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.136028 hebill-1.1.6/hebill/pdf/
+-rw-rw-rw-   0        0        0      309 2024-04-09 02:09:58.000000 hebill-1.1.6/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.138028 hebill-1.1.6/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.6/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/component/core.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.6/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8079 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.142267 hebill-1.1.6/hebill/pdf/features/
+-rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.1.6/hebill/pdf/features/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/features/configs.py
+-rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/features/document_configs.py
+-rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/features/page_configs.py
+-rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/features/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.147555 hebill-1.1.6/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.6/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.6/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.6/hebill/pdf/library/configs_selector_font.py
+-rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.6/hebill/pdf/library/get_display_width.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.159989 hebill-1.1.6/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.6/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.6/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.6/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.6/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.1.6/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.6/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.6/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.6/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.6/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.6/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.6/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.6/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.163575 hebill-1.1.6/hebill/pypi/
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.6/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2024-04-09 01:50:41.000000 hebill-1.1.6/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.165568 hebill-1.1.6/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.6/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.6/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.167111 hebill-1.1.6/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.6/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.6/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:35:07.168151 hebill-1.1.6/hebill.egg-info/
+-rw-rw-rw-   0        0        0      487 2024-04-09 02:35:06.000000 hebill-1.1.6/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6310 2024-04-09 02:35:06.000000 hebill-1.1.6/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 02:35:06.000000 hebill-1.1.6/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-09 02:35:06.000000 hebill-1.1.6/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 02:35:06.000000 hebill-1.1.6/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2024-04-09 02:35:07.170153 hebill-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      524 2024-04-09 02:35:06.000000 hebill-1.1.6/setup_by_hebill.py
```

### Comparing `hebill-1.1.5/hebill/dir/core.py` & `hebill-1.1.6/hebill/dir/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/file/core.py` & `hebill-1.1.6/hebill/file/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/html/head/core.py` & `hebill-1.1.6/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/table/core.py` & `hebill-1.1.6/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/table/tbody/core.py` & `hebill-1.1.6/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.1.6/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/table/thead/core.py` & `hebill-1.1.6/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/components/table/thead/tr/core.py` & `hebill-1.1.6/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/core.py` & `hebill-1.1.6/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/comment/core.py` & `hebill-1.1.6/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/group/core.py` & `hebill-1.1.6/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/group/create/core.py` & `hebill-1.1.6/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.1.6/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.1.6/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/node/core.py` & `hebill-1.1.6/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.1.6/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.1.6/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.1.6/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/nodes/tag/core.py` & `hebill-1.1.6/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/html/tags/__init__.py` & `hebill-1.1.6/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/image/__init__.py` & `hebill-1.1.6/hebill/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/image/png/constants.py` & `hebill-1.1.6/hebill/image/png/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/image/png/core.py` & `hebill-1.1.6/hebill/image/png/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/core.py` & `hebill-1.1.6/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/features/table_describe_data.py` & `hebill-1.1.6/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/features/table_index_data.py` & `hebill-1.1.6/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/features/table_status_data.py` & `hebill-1.1.6/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/plugins/columns/core.py` & `hebill-1.1.6/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/plugins/limits/core.py` & `hebill-1.1.6/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/plugins/orders/core.py` & `hebill-1.1.6/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.1.6/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.1.6/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/core.py` & `hebill-1.1.6/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/data/core.py` & `hebill-1.1.6/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/data/drop.py` & `hebill-1.1.6/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/data/insert.py` & `hebill-1.1.6/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/data/search.py` & `hebill-1.1.6/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/mysql/table/data/update.py` & `hebill-1.1.6/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/numeric/constants.py` & `hebill-1.1.6/hebill/numeric/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/numeric/core.py` & `hebill-1.1.6/hebill/numeric/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/component/core.py` & `hebill-1.1.6/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/constants.py` & `hebill-1.1.6/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/core.py` & `hebill-1.1.6/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/features/document_configs.py` & `hebill-1.1.6/hebill/pdf/features/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/features/page_configs.py` & `hebill-1.1.6/hebill/pdf/features/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/features/styles.py` & `hebill-1.1.6/hebill/pdf/features/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/library/configs_selector_color.py` & `hebill-1.1.6/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/library/configs_selector_font.py` & `hebill-1.1.6/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/library/get_display_width.py` & `hebill-1.1.6/hebill/pdf/library/get_display_width.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/_draw_.py` & `hebill-1.1.6/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/core.py` & `hebill-1.1.6/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/draw_grids.py` & `hebill-1.1.6/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/draw_path.py` & `hebill-1.1.6/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/draw_rect.py` & `hebill-1.1.6/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pdf/page/draw_string.py` & `hebill-1.1.6/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill/pypi/core.py` & `hebill-1.1.6/hebill/pypi/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.5/hebill.egg-info/SOURCES.txt` & `hebill-1.1.6/hebill.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 hebill.egg-info/PKG-INFO
 hebill.egg-info/SOURCES.txt
 hebill.egg-info/dependency_links.txt
 hebill.egg-info/requires.txt
 hebill.egg-info/top_level.txt
 hebill/dir/__init__.py
 hebill/dir/core.py
+hebill/excel/__init__.py
+hebill/excel/methods/__init__.py
+hebill/excel/methods/letters_to_number.py
+hebill/excel/methods/number_to_letters.py
 hebill/file/__init__.py
 hebill/file/core.py
 hebill/html/__init__.py
 hebill/html/core.py
 hebill/html/components/__init__.py
 hebill/html/components/html/__init__.py
 hebill/html/components/html/core.py
```

### Comparing `hebill-1.1.5/setup_by_hebill.py` & `hebill-1.1.6/setup_by_hebill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(
     name='hebill',
-    version='1.1.5',
+    version='1.1.6',
     description='Python Hebill',
     long_description=open(r'E:\PythonProjects\hebill\README.MD').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
```

