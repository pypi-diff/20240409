# Comparing `tmp/hebill-1.1.2.tar.gz` & `tmp/hebill-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.1.2.tar", last modified: Tue Apr  9 00:42:13 2024, max compression
+gzip compressed data, was "hebill-1.1.3.tar", last modified: Tue Apr  9 01:17:06 2024, max compression
```

## Comparing `hebill-1.1.2.tar` & `hebill-1.1.3.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.516431 hebill-1.1.2/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0      485 2024-04-09 00:42:13.515429 hebill-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.383860 hebill-1.1.2/hebill/
--rw-rw-rw-   0        0        0      458 2024-04-09 00:42:12.000000 hebill-1.1.2/hebill/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.389400 hebill-1.1.2/hebill/dir/
--rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.2/hebill/dir/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.2/hebill/dir/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.390615 hebill-1.1.2/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.2/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.2/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.392622 hebill-1.1.2/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.393368 hebill-1.1.2/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.394373 hebill-1.1.2/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.2/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.395630 hebill-1.1.2/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.2/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.2/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.2/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.397433 hebill-1.1.2/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.2/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.2/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.398440 hebill-1.1.2/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.2/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.398440 hebill-1.1.2/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.2/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.2/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.400852 hebill-1.1.2/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.2/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.2/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.401861 hebill-1.1.2/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.2/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.2/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.402859 hebill-1.1.2/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.2/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.403859 hebill-1.1.2/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.2/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.404859 hebill-1.1.2/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.2/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.2/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.406860 hebill-1.1.2/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.2/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.408219 hebill-1.1.2/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.2/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.2/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.409409 hebill-1.1.2/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.410474 hebill-1.1.2/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.2/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.2/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.412106 hebill-1.1.2/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.2/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.2/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.413209 hebill-1.1.2/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.2/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.2/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.414305 hebill-1.1.2/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.2/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.2/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.415898 hebill-1.1.2/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.417021 hebill-1.1.2/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.2/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.2/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.2/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.418124 hebill-1.1.2/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.2/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.2/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.419163 hebill-1.1.2/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.2/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.2/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.420169 hebill-1.1.2/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.2/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.2/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.422584 hebill-1.1.2/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.2/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.423579 hebill-1.1.2/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.427619 hebill-1.1.2/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.430974 hebill-1.1.2/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.2/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.2/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.431986 hebill-1.1.2/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.432984 hebill-1.1.2/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.2/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.434331 hebill-1.1.2/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.2/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.435330 hebill-1.1.2/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.2/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.436336 hebill-1.1.2/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.438197 hebill-1.1.2/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.440206 hebill-1.1.2/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.441206 hebill-1.1.2/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.442207 hebill-1.1.2/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.443336 hebill-1.1.2/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.2/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.444345 hebill-1.1.2/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.2/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.445652 hebill-1.1.2/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.2/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.446799 hebill-1.1.2/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.2/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.448117 hebill-1.1.2/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.2/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.449240 hebill-1.1.2/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.2/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.450247 hebill-1.1.2/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.2/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.451539 hebill-1.1.2/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.2/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.453400 hebill-1.1.2/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.2/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.454409 hebill-1.1.2/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.2/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.455566 hebill-1.1.2/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.2/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.456573 hebill-1.1.2/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.2/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.459773 hebill-1.1.2/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.2/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.460785 hebill-1.1.2/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.2/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.2/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.460785 hebill-1.1.2/hebill/image/
--rw-rw-rw-   0        0        0      578 2024-04-05 04:11:13.000000 hebill-1.1.2/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.463878 hebill-1.1.2/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.2/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    67932 2024-04-06 01:07:24.000000 hebill-1.1.2/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.2/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.465267 hebill-1.1.2/hebill/mysql/
--rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.2/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.2/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.2/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.469533 hebill-1.1.2/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.471529 hebill-1.1.2/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.473162 hebill-1.1.2/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.2/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.2/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.474050 hebill-1.1.2/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.2/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.2/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.477050 hebill-1.1.2/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.2/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.2/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.481050 hebill-1.1.2/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.2/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.2/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.2/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.2/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.482048 hebill-1.1.2/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.485080 hebill-1.1.2/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.2/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.489296 hebill-1.1.2/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.2/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.2/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.2/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.2/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.2/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.2/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.491296 hebill-1.1.2/hebill/pdf/
--rw-rw-rw-   0        0        0      168 2024-03-19 09:06:22.000000 hebill-1.1.2/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.492722 hebill-1.1.2/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.2/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2484 2024-03-20 08:24:51.000000 hebill-1.1.2/hebill/pdf/component/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.496668 hebill-1.1.2/hebill/pdf/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:17:30.000000 hebill-1.1.2/hebill/pdf/configs/__init__.py
--rw-rw-rw-   0        0        0     1422 2024-03-20 08:42:29.000000 hebill-1.1.2/hebill/pdf/configs/document_configs.py
--rw-rw-rw-   0        0        0     1385 2024-03-20 08:21:22.000000 hebill-1.1.2/hebill/pdf/configs/page_configs.py
--rw-rw-rw-   0        0        0     4894 2024-03-20 08:22:49.000000 hebill-1.1.2/hebill/pdf/configs/styles.py
--rw-rw-rw-   0        0        0      456 2024-03-20 08:21:22.000000 hebill-1.1.2/hebill/pdf/configs/template.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.2/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8076 2024-04-05 02:02:15.000000 hebill-1.1.2/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.499675 hebill-1.1.2/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.2/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.2/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.2/hebill/pdf/library/configs_selector_font.py
--rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.2/hebill/pdf/library/get_display_width.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.509914 hebill-1.1.2/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.2/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      885 2024-03-20 08:21:22.000000 hebill-1.1.2/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.2/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.2/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.2/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3002 2024-03-20 08:34:38.000000 hebill-1.1.2/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.2/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.2/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.2/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.2/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.2/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.2/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.2/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.510421 hebill-1.1.2/hebill/pypi/
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.2/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     7860 2024-04-09 00:42:12.000000 hebill-1.1.2/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.512429 hebill-1.1.2/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.2/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.2/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.513430 hebill-1.1.2/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.2/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.2/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 00:42:13.514429 hebill-1.1.2/hebill.egg-info/
--rw-rw-rw-   0        0        0      485 2024-04-09 00:42:13.000000 hebill-1.1.2/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6049 2024-04-09 00:42:13.000000 hebill-1.1.2/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 00:42:13.000000 hebill-1.1.2/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-09 00:42:13.000000 hebill-1.1.2/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 00:42:13.000000 hebill-1.1.2/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2024-04-09 00:42:13.517432 hebill-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      524 2024-04-09 00:42:12.000000 hebill-1.1.2/setup_by_hebill.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.163570 hebill-1.1.3/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.1.3/LICENSE.rst
+-rw-rw-rw-   0        0        0      485 2024-04-09 01:17:06.163062 hebill-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.962823 hebill-1.1.3/hebill/
+-rw-rw-rw-   0        0        0      458 2024-04-09 01:17:04.000000 hebill-1.1.3/hebill/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.969336 hebill-1.1.3/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.1.3/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.1.3/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.971335 hebill-1.1.3/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.1.3/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.1.3/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.973596 hebill-1.1.3/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.974595 hebill-1.1.3/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.975595 hebill-1.1.3/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.1.3/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.977595 hebill-1.1.3/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.1.3/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.1.3/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.1.3/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.978596 hebill-1.1.3/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.1.3/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.1.3/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.980598 hebill-1.1.3/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.1.3/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.982104 hebill-1.1.3/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.1.3/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.1.3/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.983113 hebill-1.1.3/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.1.3/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.1.3/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.985492 hebill-1.1.3/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.1.3/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.1.3/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.987116 hebill-1.1.3/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.3/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.989337 hebill-1.1.3/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.3/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.990345 hebill-1.1.3/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.1.3/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.1.3/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.991853 hebill-1.1.3/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.1.3/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.993862 hebill-1.1.3/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.1.3/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.1.3/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.994866 hebill-1.1.3/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.996863 hebill-1.1.3/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.1.3/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.1.3/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:05.999210 hebill-1.1.3/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.1.3/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.1.3/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.001207 hebill-1.1.3/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.1.3/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.1.3/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.003476 hebill-1.1.3/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.1.3/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.1.3/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.005482 hebill-1.1.3/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.007744 hebill-1.1.3/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.1.3/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.1.3/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.1.3/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.009753 hebill-1.1.3/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.1.3/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.1.3/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.010751 hebill-1.1.3/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.1.3/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.1.3/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.012862 hebill-1.1.3/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.1.3/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.1.3/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.015379 hebill-1.1.3/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.1.3/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.017380 hebill-1.1.3/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.019392 hebill-1.1.3/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.021402 hebill-1.1.3/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.1.3/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.1.3/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.022910 hebill-1.1.3/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.024922 hebill-1.1.3/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.1.3/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.026921 hebill-1.1.3/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.1.3/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.028919 hebill-1.1.3/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.1.3/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.030918 hebill-1.1.3/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.031919 hebill-1.1.3/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.033918 hebill-1.1.3/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.035427 hebill-1.1.3/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.036435 hebill-1.1.3/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.038435 hebill-1.1.3/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.1.3/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.039436 hebill-1.1.3/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.1.3/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.041437 hebill-1.1.3/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.1.3/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.043434 hebill-1.1.3/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.1.3/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.044436 hebill-1.1.3/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.1.3/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.046438 hebill-1.1.3/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.1.3/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.047436 hebill-1.1.3/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.1.3/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.049436 hebill-1.1.3/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.1.3/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.052457 hebill-1.1.3/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.1.3/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.053985 hebill-1.1.3/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.1.3/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.054994 hebill-1.1.3/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.1.3/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.058229 hebill-1.1.3/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.1.3/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.060130 hebill-1.1.3/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.1.3/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.063140 hebill-1.1.3/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.1.3/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.1.3/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.063140 hebill-1.1.3/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.1.3/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.067667 hebill-1.1.3/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.1.3/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    67932 2024-04-06 01:07:24.000000 hebill-1.1.3/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.1.3/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.072881 hebill-1.1.3/hebill/mysql/
+-rw-rw-rw-   0        0        0       53 2024-04-05 02:36:51.000000 hebill-1.1.3/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.1.3/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.1.3/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.078941 hebill-1.1.3/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.080963 hebill-1.1.3/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.082471 hebill-1.1.3/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.1.3/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.1.3/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.084480 hebill-1.1.3/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.1.3/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.1.3/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.086045 hebill-1.1.3/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.1.3/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.1.3/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.090742 hebill-1.1.3/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.1.3/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.1.3/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.1.3/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.1.3/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.092751 hebill-1.1.3/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.094752 hebill-1.1.3/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.1.3/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.102271 hebill-1.1.3/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.1.3/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.1.3/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.1.3/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.1.3/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.1.3/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.1.3/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.106416 hebill-1.1.3/hebill/pdf/
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:06:22.000000 hebill-1.1.3/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.108108 hebill-1.1.3/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.1.3/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-03-20 08:24:51.000000 hebill-1.1.3/hebill/pdf/component/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.114344 hebill-1.1.3/hebill/pdf/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:17:30.000000 hebill-1.1.3/hebill/pdf/configs/__init__.py
+-rw-rw-rw-   0        0        0     1422 2024-03-20 08:42:29.000000 hebill-1.1.3/hebill/pdf/configs/document_configs.py
+-rw-rw-rw-   0        0        0     1385 2024-03-20 08:21:22.000000 hebill-1.1.3/hebill/pdf/configs/page_configs.py
+-rw-rw-rw-   0        0        0     4894 2024-03-20 08:22:49.000000 hebill-1.1.3/hebill/pdf/configs/styles.py
+-rw-rw-rw-   0        0        0      456 2024-03-20 08:21:22.000000 hebill-1.1.3/hebill/pdf/configs/template.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.1.3/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8076 2024-04-05 02:02:15.000000 hebill-1.1.3/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.119340 hebill-1.1.3/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.1.3/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.1.3/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.1.3/hebill/pdf/library/configs_selector_font.py
+-rw-rw-rw-   0        0        0      682 2024-03-19 11:34:35.000000 hebill-1.1.3/hebill/pdf/library/get_display_width.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.146971 hebill-1.1.3/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.1.3/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      885 2024-03-20 08:21:22.000000 hebill-1.1.3/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.1.3/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.1.3/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.1.3/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3002 2024-03-20 08:34:38.000000 hebill-1.1.3/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.1.3/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.1.3/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.1.3/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.1.3/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.1.3/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.1.3/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.1.3/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.150975 hebill-1.1.3/hebill/pypi/
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.1.3/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     7860 2024-04-09 00:42:12.000000 hebill-1.1.3/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.156917 hebill-1.1.3/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.3/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      404 2024-04-05 01:35:34.000000 hebill-1.1.3/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.159722 hebill-1.1.3/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.1.3/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.1.3/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:17:06.160872 hebill-1.1.3/hebill.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-04-09 01:17:05.000000 hebill-1.1.3/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6049 2024-04-09 01:17:05.000000 hebill-1.1.3/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 01:17:05.000000 hebill-1.1.3/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-09 01:17:05.000000 hebill-1.1.3/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 01:17:05.000000 hebill-1.1.3/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2024-04-09 01:17:06.164579 hebill-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      524 2024-04-09 01:17:05.000000 hebill-1.1.3/setup_by_hebill.py
```

### Comparing `hebill-1.1.2/hebill/dir/core.py` & `hebill-1.1.3/hebill/dir/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/file/core.py` & `hebill-1.1.3/hebill/file/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/html/head/core.py` & `hebill-1.1.3/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/table/core.py` & `hebill-1.1.3/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/table/tbody/core.py` & `hebill-1.1.3/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.1.3/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/table/thead/core.py` & `hebill-1.1.3/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/components/table/thead/tr/core.py` & `hebill-1.1.3/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/core.py` & `hebill-1.1.3/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/comment/core.py` & `hebill-1.1.3/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/group/core.py` & `hebill-1.1.3/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/group/create/core.py` & `hebill-1.1.3/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.1.3/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.1.3/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/node/core.py` & `hebill-1.1.3/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.1.3/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.1.3/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.1.3/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/nodes/tag/core.py` & `hebill-1.1.3/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/html/tags/__init__.py` & `hebill-1.1.3/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/image/__init__.py` & `hebill-1.1.3/hebill/image/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,7 +10,10 @@
 from .png.core import PNGIconMaximize
 from .png.core import PNGIconMinimize
 from .png.core import PNGIconMore
 from .png.core import PNGIconNormalize
 from .png.core import PNGIconQuite
 from .png.core import PNGIconSetting
 from .png.core import PNGIconUser
+
+from .png.core import PNGIconHebill
+from .png.core import PNGIconYangs
```

### Comparing `hebill-1.1.2/hebill/image/png/constants.py` & `hebill-1.1.3/hebill/image/png/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/image/png/core.py` & `hebill-1.1.3/hebill/image/png/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/core.py` & `hebill-1.1.3/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/features/table_describe_data.py` & `hebill-1.1.3/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/features/table_index_data.py` & `hebill-1.1.3/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/features/table_status_data.py` & `hebill-1.1.3/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/plugins/columns/core.py` & `hebill-1.1.3/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/plugins/limits/core.py` & `hebill-1.1.3/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/plugins/orders/core.py` & `hebill-1.1.3/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.1.3/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.1.3/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/core.py` & `hebill-1.1.3/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/data/core.py` & `hebill-1.1.3/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/data/drop.py` & `hebill-1.1.3/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/data/insert.py` & `hebill-1.1.3/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/data/search.py` & `hebill-1.1.3/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/mysql/table/data/update.py` & `hebill-1.1.3/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/component/core.py` & `hebill-1.1.3/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/configs/document_configs.py` & `hebill-1.1.3/hebill/pdf/configs/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/configs/page_configs.py` & `hebill-1.1.3/hebill/pdf/configs/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/configs/styles.py` & `hebill-1.1.3/hebill/pdf/configs/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/constants.py` & `hebill-1.1.3/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/core.py` & `hebill-1.1.3/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/library/configs_selector_color.py` & `hebill-1.1.3/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/library/configs_selector_font.py` & `hebill-1.1.3/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/library/get_display_width.py` & `hebill-1.1.3/hebill/pdf/library/get_display_width.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/_draw_.py` & `hebill-1.1.3/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/core.py` & `hebill-1.1.3/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/draw_grids.py` & `hebill-1.1.3/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/draw_path.py` & `hebill-1.1.3/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/draw_rect.py` & `hebill-1.1.3/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pdf/page/draw_string.py` & `hebill-1.1.3/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill/pypi/core.py` & `hebill-1.1.3/hebill/pypi/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/hebill.egg-info/SOURCES.txt` & `hebill-1.1.3/hebill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hebill-1.1.2/setup_by_hebill.py` & `hebill-1.1.3/setup_by_hebill.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(
     name='hebill',
-    version='1.1.2',
+    version='1.1.3',
     description='Python Hebill',
     long_description=open(r'E:\PythonProjects\hebill\README.MD').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
```

