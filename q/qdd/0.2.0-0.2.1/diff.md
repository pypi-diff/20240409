# Comparing `tmp/qdd-0.2.0-cp39-cp39-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.zip` & `tmp/qdd-0.2.1-cp39-cp39-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 158444 bytes, number of entries: 18
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 05:03 qdd.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 05:03 qdd/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 05:03 qdd-0.2.0.dist-info/
--rw-r--r--  2.0 unx    25485 b- defN 24-Mar-26 05:03 qdd/qdd_estimator.py
--rw-r--r--  2.0 unx      792 b- defN 24-Mar-26 05:03 qdd/circuit_property.py
--rw-r--r--  2.0 unx      768 b- defN 24-Mar-26 05:03 qdd/qdd_job.py
--rw-r--r--  2.0 unx      197 b- defN 24-Mar-26 05:03 qdd/__init__.py
--rwxr-xr-x  2.0 unx   316040 b- defN 24-Mar-26 05:03 qdd/pyQDD.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    27872 b- defN 24-Mar-26 05:03 qdd/qdd_backend.py
--rw-r--r--  2.0 unx     7686 b- defN 24-Mar-26 05:03 qdd/qdd_sampler.py
--rw-r--r--  2.0 unx      863 b- defN 24-Mar-26 05:03 qdd/qdd_provider.py
--rw-r--r--  2.0 unx      627 b- defN 24-Mar-26 05:03 qdd/qdd_failed_job.py
--rw-r--r--  2.0 unx      640 b- defN 24-Mar-26 05:03 qdd/qdd_sv_backend.py
--rw-rw-r--  2.0 unx     1163 b- defN 24-Mar-26 05:03 qdd-0.2.0.dist-info/RECORD
--rw-r--r--  2.0 unx     4631 b- defN 24-Mar-26 05:03 qdd-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      149 b- defN 24-Mar-26 05:03 qdd-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Mar-26 05:03 qdd-0.2.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1650 b- defN 24-Mar-26 05:03 qdd-0.2.0.dist-info/LICENSE.txt
-18 files, 388630 bytes uncompressed, 156284 bytes compressed:  59.8%
+Zip file size: 159341 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 07:52 qdd/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 07:52 qdd.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 07:52 qdd-0.2.1.dist-info/
+-rw-r--r--  2.0 unx      863 b- defN 24-Apr-09 07:52 qdd/qdd_provider.py
+-rw-r--r--  2.0 unx    25485 b- defN 24-Apr-09 07:52 qdd/qdd_estimator.py
+-rw-r--r--  2.0 unx     7686 b- defN 24-Apr-09 07:52 qdd/qdd_sampler.py
+-rw-r--r--  2.0 unx      768 b- defN 24-Apr-09 07:52 qdd/qdd_job.py
+-rw-r--r--  2.0 unx      197 b- defN 24-Apr-09 07:52 qdd/__init__.py
+-rw-r--r--  2.0 unx      640 b- defN 24-Apr-09 07:52 qdd/qdd_sv_backend.py
+-rw-r--r--  2.0 unx    27872 b- defN 24-Apr-09 07:52 qdd/qdd_backend.py
+-rwxr-xr-x  2.0 unx   316040 b- defN 24-Apr-09 07:52 qdd/pyQDD.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      792 b- defN 24-Apr-09 07:52 qdd/circuit_property.py
+-rw-r--r--  2.0 unx      627 b- defN 24-Apr-09 07:52 qdd/qdd_failed_job.py
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-09 07:52 qdd-0.2.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     7244 b- defN 24-Apr-09 07:52 qdd-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-09 07:52 qdd-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1650 b- defN 24-Apr-09 07:52 qdd-0.2.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1163 b- defN 24-Apr-09 07:52 qdd-0.2.1.dist-info/RECORD
+18 files, 391243 bytes uncompressed, 157181 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,55 +1,55 @@
+Filename: qdd/
+Comment: 
+
 Filename: qdd.libs/
 Comment: 
 
-Filename: qdd/
+Filename: qdd-0.2.1.dist-info/
 Comment: 
 
-Filename: qdd-0.2.0.dist-info/
+Filename: qdd/qdd_provider.py
 Comment: 
 
 Filename: qdd/qdd_estimator.py
 Comment: 
 
-Filename: qdd/circuit_property.py
+Filename: qdd/qdd_sampler.py
 Comment: 
 
 Filename: qdd/qdd_job.py
 Comment: 
 
 Filename: qdd/__init__.py
 Comment: 
 
-Filename: qdd/pyQDD.cpython-39-x86_64-linux-gnu.so
+Filename: qdd/qdd_sv_backend.py
 Comment: 
 
 Filename: qdd/qdd_backend.py
 Comment: 
 
-Filename: qdd/qdd_sampler.py
+Filename: qdd/pyQDD.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: qdd/qdd_provider.py
+Filename: qdd/circuit_property.py
 Comment: 
 
 Filename: qdd/qdd_failed_job.py
 Comment: 
 
-Filename: qdd/qdd_sv_backend.py
-Comment: 
-
-Filename: qdd-0.2.0.dist-info/RECORD
+Filename: qdd-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qdd-0.2.0.dist-info/METADATA
+Filename: qdd-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: qdd-0.2.0.dist-info/WHEEL
+Filename: qdd-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: qdd-0.2.0.dist-info/top_level.txt
+Filename: qdd-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: qdd-0.2.0.dist-info/LICENSE.txt
+Filename: qdd-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `qdd-0.2.0.dist-info/RECORD` & `qdd-0.2.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+qdd/qdd_provider.py,sha256=7kAVus1hjuRRNprXNiFtUirdh5-Q8v8zJUDNoCeKhQE,863
 qdd/qdd_estimator.py,sha256=jdj-bb1bEJti1IiIDx66gFs5P_AN6SWC7GBGCpT-S78,25485
-qdd/circuit_property.py,sha256=YQ-0fsGOmebPZZFbpmviteCa5My0j5PZV-DvJFQmWpg,792
+qdd/qdd_sampler.py,sha256=ku_6mq0afecPgSZ3gLevAljEJ-JCY9bJhE9s2vsxu-w,7686
 qdd/qdd_job.py,sha256=jgHJN6r0708EyYfL95CQZ0hPoAV4BcncRrCkDuc6Efo,768
 qdd/__init__.py,sha256=HvLpWZdFm8W748AaXJOVLeRl-gjqWzpkAELsMzS5RkM,197
-qdd/pyQDD.cpython-39-x86_64-linux-gnu.so,sha256=EvY_YfK68ZCfDyTOU4ZLykZgj4gC6wqugddRalJdIJM,316040
+qdd/qdd_sv_backend.py,sha256=0WQ96v0xcGSuMKXF8lbrXL4O2IGdZIjUW2tA8UEL4s0,640
 qdd/qdd_backend.py,sha256=DOfBx3viTR_BdXXCbkd-oktp2Ihc1JQ40XPgYwS1qPU,27872
-qdd/qdd_sampler.py,sha256=ku_6mq0afecPgSZ3gLevAljEJ-JCY9bJhE9s2vsxu-w,7686
-qdd/qdd_provider.py,sha256=7kAVus1hjuRRNprXNiFtUirdh5-Q8v8zJUDNoCeKhQE,863
+qdd/pyQDD.cpython-39-x86_64-linux-gnu.so,sha256=EvY_YfK68ZCfDyTOU4ZLykZgj4gC6wqugddRalJdIJM,316040
+qdd/circuit_property.py,sha256=YQ-0fsGOmebPZZFbpmviteCa5My0j5PZV-DvJFQmWpg,792
 qdd/qdd_failed_job.py,sha256=Qcu8xo10yhdzhdno7lZr0pwQ6Ih5Tk_k5tkng3tT94w,627
-qdd/qdd_sv_backend.py,sha256=0WQ96v0xcGSuMKXF8lbrXL4O2IGdZIjUW2tA8UEL4s0,640
-qdd-0.2.0.dist-info/RECORD,,
-qdd-0.2.0.dist-info/METADATA,sha256=qQIfF1qYKRkjsAIDbGvKA9Df5WDZEdMSrwQ0XPM2wiQ,4631
-qdd-0.2.0.dist-info/WHEEL,sha256=EH9o_--fHMPEJDclI8o9HjUumChQB_FhRplwpGS8fJk,149
-qdd-0.2.0.dist-info/top_level.txt,sha256=D9tZ6VwCpDGK9OaB_Q1aLmAL8MtFI7mNSy47JUEJAtc,67
-qdd-0.2.0.dist-info/LICENSE.txt,sha256=QiJ44oZZ9Cu0M_jKsGYWUJarn6eTEKGim5srwVdFGso,1650
+qdd-0.2.1.dist-info/top_level.txt,sha256=D9tZ6VwCpDGK9OaB_Q1aLmAL8MtFI7mNSy47JUEJAtc,67
+qdd-0.2.1.dist-info/METADATA,sha256=DL0eByVDibL_LWGRi9hKhkv0u87VsIAKBrViTbTyOi8,7244
+qdd-0.2.1.dist-info/WHEEL,sha256=EH9o_--fHMPEJDclI8o9HjUumChQB_FhRplwpGS8fJk,149
+qdd-0.2.1.dist-info/LICENSE.txt,sha256=QiJ44oZZ9Cu0M_jKsGYWUJarn6eTEKGim5srwVdFGso,1650
+qdd-0.2.1.dist-info/RECORD,,
```

## Comparing `qdd-0.2.0.dist-info/LICENSE.txt` & `qdd-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

