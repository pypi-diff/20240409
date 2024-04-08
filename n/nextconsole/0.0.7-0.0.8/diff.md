# Comparing `tmp/nextconsole-0.0.7-py3-none-any.whl.zip` & `tmp/nextconsole-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2704 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 14:13 nextconsole/__init__.py
+Zip file size: 2714 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       60 b- defN 24-Apr-08 14:17 nextconsole/__init__.py
 -rw-rw-r--  2.0 unx     2029 b- defN 24-Apr-08 14:13 nextconsole/command.py
--rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 14:14 nextconsole-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 14:14 nextconsole-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-08 14:14 nextconsole-0.0.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 14:14 nextconsole-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 14:14 nextconsole-0.0.7.dist-info/RECORD
-7 files, 3311 bytes uncompressed, 1684 bytes compressed:  49.1%
+-rw-rw-r--  2.0 unx      507 b- defN 24-Apr-08 14:17 nextconsole-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-08 14:17 nextconsole-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       93 b- defN 24-Apr-08 14:17 nextconsole-0.0.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-08 14:17 nextconsole-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      569 b- defN 24-Apr-08 14:17 nextconsole-0.0.8.dist-info/RECORD
+7 files, 3362 bytes uncompressed, 1694 bytes compressed:  49.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: nextconsole/__init__.py
 Comment: 
 
 Filename: nextconsole/command.py
 Comment: 
 
-Filename: nextconsole-0.0.7.dist-info/METADATA
+Filename: nextconsole-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: nextconsole-0.0.7.dist-info/WHEEL
+Filename: nextconsole-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: nextconsole-0.0.7.dist-info/entry_points.txt
+Filename: nextconsole-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: nextconsole-0.0.7.dist-info/top_level.txt
+Filename: nextconsole-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: nextconsole-0.0.7.dist-info/RECORD
+Filename: nextconsole-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextconsole/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = __VERISON__ = "0.0.7"
+__version__ = __VERISON__ = "0.0.8"
 from .command import cmd
```

