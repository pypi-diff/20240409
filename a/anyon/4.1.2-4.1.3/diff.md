# Comparing `tmp/anyon-4.1.2-cp312-none-macosx_10_9_universal2.whl.zip` & `tmp/anyon-4.1.3-cp312-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1056331 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-09 01:13 anyon-4.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2283 b- defN 24-Apr-09 01:13 anyon-4.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-09 01:13 anyon-4.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-09 01:13 anyon-4.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      376 b- defN 24-Apr-09 01:13 anyon-4.1.2.dist-info/RECORD
--rwxr-xr-x  2.0 unx   121664 b- defN 24-Apr-09 01:12 anyon/__init__.so
--rwxr-xr-x  2.0 unx   322350 b- defN 24-Apr-09 01:12 anyon/loader.so
--rwxr-xr-x  2.0 unx   393502 b- defN 24-Apr-09 01:12 anyon/remote.so
--rwxr-xr-x  2.0 unx   686014 b- defN 24-Apr-09 01:11 anyon/server.so
--rwxr-xr-x  2.0 unx   122000 b- defN 24-Apr-09 01:12 anyon/stage/__init__.so
--rwxr-xr-x  2.0 unx   744945 b- defN 24-Apr-09 01:13 anyon/stage/assembler.so
--rwxr-xr-x  2.0 unx   322802 b- defN 24-Apr-09 01:13 anyon/stage/calculator.so
--rwxr-xr-x  2.0 unx   458174 b- defN 24-Apr-09 01:12 anyon/stage/device.so
--rwxr-xr-x  2.0 unx   251473 b- defN 24-Apr-09 01:12 anyon/stage/processor.so
-14 files, 3426761 bytes uncompressed, 1054589 bytes compressed:  69.2%
+Zip file size: 468865 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-09 02:20 anyon-4.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2334 b- defN 24-Apr-09 02:20 anyon-4.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-09 02:20 anyon-4.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-09 02:20 anyon-4.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      376 b- defN 24-Apr-09 02:20 anyon-4.1.3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    20992 b- defN 24-Apr-09 02:20 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    96256 b- defN 24-Apr-09 02:20 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat   121344 b- defN 24-Apr-09 02:20 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   228352 b- defN 24-Apr-09 02:20 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    22016 b- defN 24-Apr-09 02:20 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat   251904 b- defN 24-Apr-09 02:20 anyon/stage/assembler.pyd
+-rw-rw-rw-  2.0 fat   100352 b- defN 24-Apr-09 02:20 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   140288 b- defN 24-Apr-09 02:20 anyon/stage/device.pyd
+-rw-rw-rw-  2.0 fat    67584 b- defN 24-Apr-09 02:20 anyon/stage/processor.pyd
+14 files, 1052984 bytes uncompressed, 467105 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-4.1.2.dist-info/LICENSE
+Filename: anyon-4.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-4.1.2.dist-info/METADATA
+Filename: anyon-4.1.3.dist-info/METADATA
 Comment: 
 
-Filename: anyon-4.1.2.dist-info/WHEEL
+Filename: anyon-4.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-4.1.2.dist-info/top_level.txt
+Filename: anyon-4.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-4.1.2.dist-info/RECORD
+Filename: anyon-4.1.3.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.so
+Filename: anyon/__init__.pyd
 Comment: 
 
-Filename: anyon/loader.so
+Filename: anyon/loader.pyd
 Comment: 
 
-Filename: anyon/remote.so
+Filename: anyon/remote.pyd
 Comment: 
 
-Filename: anyon/server.so
+Filename: anyon/server.pyd
 Comment: 
 
-Filename: anyon/stage/__init__.so
+Filename: anyon/stage/__init__.pyd
 Comment: 
 
-Filename: anyon/stage/assembler.so
+Filename: anyon/stage/assembler.pyd
 Comment: 
 
-Filename: anyon/stage/calculator.so
+Filename: anyon/stage/calculator.pyd
 Comment: 
 
-Filename: anyon/stage/device.so
+Filename: anyon/stage/device.pyd
 Comment: 
 
-Filename: anyon/stage/processor.so
+Filename: anyon/stage/processor.pyd
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-4.1.2.dist-info/LICENSE` & `anyon-4.1.3.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 YL Feng
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 YL Feng
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `anyon-4.1.2.dist-info/METADATA` & `anyon-4.1.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 4.1.2
-Summary: description
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL Feng
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy >=1.20.0
-Requires-Dist: axion >=3.4.5
-Requires-Dist: srpc >=4.2.8
-Requires-Dist: zee >=0.0.3
-Requires-Dist: requests >=2.28.0
-Requires-Dist: APScheduler
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 4.1.3
+Summary: description
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL Feng
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy >=1.20.0
+Requires-Dist: axion >=3.4.5
+Requires-Dist: srpc >=4.2.8
+Requires-Dist: zee >=0.0.3
+Requires-Dist: requests >=2.28.0
+Requires-Dist: APScheduler
+
```

