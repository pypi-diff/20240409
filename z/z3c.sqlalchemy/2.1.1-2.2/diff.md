# Comparing `tmp/z3c.sqlalchemy-2.1.1.tar.gz` & `tmp/z3c.sqlalchemy-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.sqlalchemy-2.1.1.tar", last modified: Wed Sep  6 06:28:13 2023, max compression
+gzip compressed data, was "z3c.sqlalchemy-2.2.tar", last modified: Tue Apr  9 15:34:08 2024, max compression
```

## Comparing `z3c.sqlalchemy-2.1.1.tar` & `z3c.sqlalchemy-2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.744606 z3c.sqlalchemy-2.1.1/
--rw-r--r--   0 m.howitz   (502) staff       (20)    10717 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      196 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    18711 2023-09-06 06:28:13.744685 z3c.sqlalchemy-2.1.1/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     6708 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      103 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/buildout.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)      423 2023-09-06 06:28:13.744956 z3c.sqlalchemy-2.1.1/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     2581 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.739689 z3c.sqlalchemy-2.1.1/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.741536 z3c.sqlalchemy-2.1.1/src/z3c/
--rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.744052 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/
--rw-r--r--   0 m.howitz   (502) staff       (20)      600 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5230 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/base.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3534 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     8322 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/mapper.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4146 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/model.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2347 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/postgres.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.744432 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)      361 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7908 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4834 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/util.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-09-06 06:28:13.742830 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    18711 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      724 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      126 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1423 2023-09-06 06:28:13.000000 z3c.sqlalchemy-2.1.1/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.347361 z3c.sqlalchemy-2.2/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11014 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      196 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19312 2024-04-09 15:34:08.347217 z3c.sqlalchemy-2.2/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6708 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      389 2024-04-09 15:34:08.347612 z3c.sqlalchemy-2.2/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2631 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.341635 z3c.sqlalchemy-2.2/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.343856 z3c.sqlalchemy-2.2/src/z3c/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.346211 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      600 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5192 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/base.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3534 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8322 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/mapper.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4146 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/model.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2347 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/postgres.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.346566 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      361 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7908 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4834 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-09 15:34:08.346816 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19312 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      724 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      126 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2024-04-09 15:34:08.000000 z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1867 2024-04-09 15:34:07.000000 z3c.sqlalchemy-2.2/tox.ini
```

### Comparing `z3c.sqlalchemy-2.1.1/CHANGES.rst` & `z3c.sqlalchemy-2.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Change log
 ==========
 
+2.2 (2024-04-09)
+----------------
+
+- Add support for Python 3.12.
+
+- Partially revert commit fb7d533aae819dc7e1aef8322c2f2d60a9a1b5d0
+  which caused the sqlalchemy session instance to be persisted as an instance attribute.
+  (`#21 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/21>`_)
+
+
 2.1.1 (2023-09-06)
 ------------------
 
 - Fix transaction rollback with DBAPI cursor.execute.
   (`#17 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/17>`_)
```

### Comparing `z3c.sqlalchemy-2.1.1/CONTRIBUTING.md` & `z3c.sqlalchemy-2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/LICENSE.txt` & `z3c.sqlalchemy-2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/PKG-INFO` & `z3c.sqlalchemy-2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.sqlalchemy
-Version: 2.1.1
+Version: 2.2
 Summary: A SQLAlchemy wrapper for Zope
 Home-page: https://github.com/zopefoundation/z3c.sqlalchemy
 Author: Andreas Jung
 Author-email: info@zopyx.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zope-dev@zope.dev
 License: ZPL 2.1
@@ -22,17 +22,26 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: SQLAlchemy>=1.4
+Requires-Dist: zope.sqlalchemy>=1.2.0
+Requires-Dist: zope.component
+Requires-Dist: zope.interface
+Requires-Dist: zope.testing
+Requires-Dist: zope.schema
+Provides-Extra: test
+Requires-Dist: zope.testing; extra == "test"
 
 =====================================================
 z3c.sqlalchemy - A SQLAlchemy wrapper for Python/Zope
 =====================================================
 
 
 What is z3c.sqlalchemy?
@@ -212,14 +221,24 @@
 Martin Aspeli for giving valuable feedback.
 
 
 
 Change log
 ==========
 
+2.2 (2024-04-09)
+----------------
+
+- Add support for Python 3.12.
+
+- Partially revert commit fb7d533aae819dc7e1aef8322c2f2d60a9a1b5d0
+  which caused the sqlalchemy session instance to be persisted as an instance attribute.
+  (`#21 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/21>`_)
+
+
 2.1.1 (2023-09-06)
 ------------------
 
 - Fix transaction rollback with DBAPI cursor.execute.
   (`#17 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/17>`_)
```

### Comparing `z3c.sqlalchemy-2.1.1/README.rst` & `z3c.sqlalchemy-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/setup.py` & `z3c.sqlalchemy-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def _read_file(filename):
     with open(os.path.join(HERE, filename)) as f:
         return f.read()
 
 
 README = _read_file('README.rst')
 CHANGES = _read_file('CHANGES.rst')
-version = '2.1.1'
+version = '2.2'
 
 
 setup(name='z3c.sqlalchemy',
       version=version,
       url='https://github.com/zopefoundation/z3c.sqlalchemy',
       project_urls={
           'Issue Tracker': ('https://github.com/zopefoundation/'
@@ -53,14 +53,15 @@
           'Topic :: Database :: Front-Ends',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12',
       ],
       packages=find_packages('src'),
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       namespace_packages=['z3c'],
       python_requires='>=3.7',
```

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/__init__.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/base.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if not hasattr(self, '_v_metadata'):
             self._v_metadata = MetaData()
         return self._v_metadata
 
     @property
     def session(self):
         """ Return thread-local session """
-        return self._session
+        return self._sessionmaker()
 
     @property
     def connection(self):
         """ Return underlying connection """
         session = self.session
         # Return the ConnectionFairy
         return session.connection().connection
@@ -136,8 +136,7 @@
         self._engine = create_engine(self.dsn, **self.engine_options)
         self._sessionmaker = scoped_session(sessionmaker(bind=self._engine,
                                             autocommit=not self.transactional,
                                             twophase=self.twophase,
                                             autoflush=True,
                                             **self.session_options))
         register(self._sessionmaker, **self.extension_options)
-        self._session = self._sessionmaker()
```

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/interfaces.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/mapper.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/mapper.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/model.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/postgres.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/postgres.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c/sqlalchemy/util.py` & `z3c.sqlalchemy-2.2/src/z3c/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/PKG-INFO` & `z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.sqlalchemy
-Version: 2.1.1
+Version: 2.2
 Summary: A SQLAlchemy wrapper for Zope
 Home-page: https://github.com/zopefoundation/z3c.sqlalchemy
 Author: Andreas Jung
 Author-email: info@zopyx.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zope-dev@zope.dev
 License: ZPL 2.1
@@ -22,17 +22,26 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: SQLAlchemy>=1.4
+Requires-Dist: zope.sqlalchemy>=1.2.0
+Requires-Dist: zope.component
+Requires-Dist: zope.interface
+Requires-Dist: zope.testing
+Requires-Dist: zope.schema
+Provides-Extra: test
+Requires-Dist: zope.testing; extra == "test"
 
 =====================================================
 z3c.sqlalchemy - A SQLAlchemy wrapper for Python/Zope
 =====================================================
 
 
 What is z3c.sqlalchemy?
@@ -212,14 +221,24 @@
 Martin Aspeli for giving valuable feedback.
 
 
 
 Change log
 ==========
 
+2.2 (2024-04-09)
+----------------
+
+- Add support for Python 3.12.
+
+- Partially revert commit fb7d533aae819dc7e1aef8322c2f2d60a9a1b5d0
+  which caused the sqlalchemy session instance to be persisted as an instance attribute.
+  (`#21 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/21>`_)
+
+
 2.1.1 (2023-09-06)
 ------------------
 
 - Fix transaction rollback with DBAPI cursor.execute.
   (`#17 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/17>`_)
```

### Comparing `z3c.sqlalchemy-2.1.1/src/z3c.sqlalchemy.egg-info/SOURCES.txt` & `z3c.sqlalchemy-2.2/src/z3c.sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.1.1/tox.ini` & `z3c.sqlalchemy-2.2/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
     py37
     py38
     py39
     py310
     py311
+    py312
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
 deps =
     zope.testrunner
+setenv =
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

