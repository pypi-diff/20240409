# Comparing `tmp/openctm-0.0.4-py3-none-win_amd64.whl.zip` & `tmp/openctm-0.0.5-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 229919 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       57 b- defN 24-Mar-08 05:11 openctm/__init__.py
--rw-rw-rw-  2.0 fat     5389 b- defN 24-Mar-08 05:11 openctm/binding.py
--rw-rw-rw-  2.0 fat     1101 b- defN 24-Mar-08 05:12 openctm-0.0.4.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     3438 b- defN 24-Mar-08 05:12 openctm-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-08 05:12 openctm-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-08 05:12 openctm-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      537 b- defN 24-Mar-08 05:12 openctm-0.0.4.dist-info/RECORD
-?rw-------  2.0 fat   224256 b- stor 24-Mar-08 05:12 openctm/openctm.dll
-8 files, 234878 bytes uncompressed, 228853 bytes compressed:  2.6%
+Zip file size: 229931 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       57 b- defN 24-Apr-09 19:38 openctm/__init__.py
+-rw-rw-rw-  2.0 fat     5389 b- defN 24-Apr-09 19:38 openctm/binding.py
+-rw-rw-rw-  2.0 fat     1101 b- defN 24-Apr-09 19:39 openctm-0.0.5.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     3460 b- defN 24-Apr-09 19:39 openctm-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 19:39 openctm-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-09 19:39 openctm-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      537 b- defN 24-Apr-09 19:39 openctm-0.0.5.dist-info/RECORD
+?rw-------  2.0 fat   224256 b- stor 24-Apr-09 19:39 openctm/openctm.dll
+8 files, 234900 bytes uncompressed, 228865 bytes compressed:  2.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: openctm/__init__.py
 Comment: 
 
 Filename: openctm/binding.py
 Comment: 
 
-Filename: openctm-0.0.4.dist-info/LICENSE.md
+Filename: openctm-0.0.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: openctm-0.0.4.dist-info/METADATA
+Filename: openctm-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: openctm-0.0.4.dist-info/WHEEL
+Filename: openctm-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: openctm-0.0.4.dist-info/top_level.txt
+Filename: openctm-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: openctm-0.0.4.dist-info/RECORD
+Filename: openctm-0.0.5.dist-info/RECORD
 Comment: 
 
 Filename: openctm/openctm.dll
 Comment: 
 
 Zip file comment:
```

## openctm/openctm.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180012a78
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Mar  8 05:12:16 2024
+Time/Date		Tue Apr  9 19:39:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	38
 SizeOfCode		0000000000025c00
 SizeOfInitializedData	0000000000011e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000012a78
@@ -63538,17 +63538,17 @@
    18003035e:	add    %al,(%rax)
    180030360:	movabs 0xa800000001800272,%al
    180030369:	jb     0x18003036d
    18003036b:	addb   $0x0,(%rcx)
    18003036e:	add    %al,(%rax)
    180030370:	add    %al,(%rax)
    180030372:	add    %al,(%rax)
-   180030374:	xor    %bl,0x65ea(%rsi)
-   18003037a:	add    %al,(%rax)
-   18003037c:	or     $0x18000000,%eax
+   180030374:	jb     0x18003030f
+   180030376:	adc    $0x66,%eax
+   18003037b:	add    %cl,0x18000000(%rip)        # 0x198030381
    180030381:	add    (%rax),%eax
    180030383:	add    %bl,%ah
    180030385:	or     %eax,(%rbx)
    180030387:	add    %bl,%ah
    180030389:	stc
    18003038a:	add    (%rax),%al
    18003038c:	add    %al,(%rax)
```

## Comparing `openctm-0.0.4.dist-info/LICENSE.md` & `openctm-0.0.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openctm-0.0.4.dist-info/METADATA` & `openctm-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openctm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provide a loader for OpenCTM files
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: MIT License
         
         Copyright (c) 2024 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
 Provides-Extra: tests
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: trimesh ; extra == 'tests'
 
 # openctm
 [![Build And Release Wheels](https://github.com/trimesh/openctm/actions/workflows/wheels.yml/badge.svg)](https://github.com/trimesh/openctm/actions/workflows/wheels.yml) [![PyPI version](https://badge.fury.io/py/openctm.svg)](https://badge.fury.io/py/openctm)
```

