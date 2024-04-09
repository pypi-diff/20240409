# Comparing `tmp/nxsconfigserver-db-1.10.4.tar.gz` & `tmp/nxsconfigserver-db-1.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsconfigserver-db-1.10.4.tar", last modified: Mon Jun 19 06:38:21 2023, max compression
+gzip compressed data, was "nxsconfigserver-db-1.10.5.tar", last modified: Tue Apr  9 06:45:44 2024, max compression
```

## Comparing `nxsconfigserver-db-1.10.4.tar` & `nxsconfigserver-db-1.10.5.tar`

### file list

```diff
@@ -1,9 +1,15 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.4/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)     5864 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     3630 2023-02-01 13:28:18.120510 nxsconfigserver-db-1.10.4/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-19 06:38:21.057699 nxsconfigserver-db-1.10.4/conf/
--rw-r--r--   0 jkotan   (15949) irc         (39)    21056 2014-07-29 06:43:42.000000 nxsconfigserver-db-1.10.4/conf/my.cnf
--rw-r--r--   0 jkotan   (15949) irc         (39)     1197 2015-02-16 13:04:15.000000 nxsconfigserver-db-1.10.4/conf/mysql_create.sql
--rw-r--r--   0 jkotan   (15949) irc         (39)      158 2016-07-04 14:03:04.000000 nxsconfigserver-db-1.10.4/setup.cfg
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     3092 2023-06-19 06:38:02.321855 nxsconfigserver-db-1.10.4/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-04-09 06:45:44.920199 nxsconfigserver-db-1.10.5/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2024-04-08 08:01:39.000000 nxsconfigserver-db-1.10.5/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       87 2024-04-08 08:01:39.000000 nxsconfigserver-db-1.10.5/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5904 2024-04-09 06:45:44.920199 nxsconfigserver-db-1.10.5/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3670 2024-04-08 08:01:39.000000 nxsconfigserver-db-1.10.5/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-04-09 06:45:44.920199 nxsconfigserver-db-1.10.5/conf/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    21056 2024-04-08 08:01:39.000000 nxsconfigserver-db-1.10.5/conf/my.cnf
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1197 2024-04-08 08:01:39.000000 nxsconfigserver-db-1.10.5/conf/mysql_create.sql
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-04-09 06:45:44.920199 nxsconfigserver-db-1.10.5/nxsconfigserver_db.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5904 2024-04-09 06:45:44.000000 nxsconfigserver-db-1.10.5/nxsconfigserver_db.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      253 2024-04-09 06:45:44.000000 nxsconfigserver-db-1.10.5/nxsconfigserver_db.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-04-09 06:45:44.000000 nxsconfigserver-db-1.10.5/nxsconfigserver_db.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-04-09 06:45:44.000000 nxsconfigserver-db-1.10.5/nxsconfigserver_db.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      196 2024-04-09 06:45:44.924199 nxsconfigserver-db-1.10.5/setup.cfg
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     3088 2024-04-09 06:44:40.000000 nxsconfigserver-db-1.10.5/setup.py
```

### Comparing `nxsconfigserver-db-1.10.4/COPYRIGHT` & `nxsconfigserver-db-1.10.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.4/PKG-INFO` & `nxsconfigserver-db-1.10.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsconfigserver-db
-Version: 1.10.4
+Version: 1.10.5
 Summary: Configuration Server  DataBase
 Home-page: https://github.com/jkotan/nexdatas/nxsconfigserver-db
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ===============================================================
         Welcome to NeXuS Configuration Server Database's documentation!
@@ -73,29 +73,29 @@
         	  $ mysql < conf/mysql_create.sql
         
         with proper privileges.
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian Jessie (and Wheezy) packages can be found in the HDRI repository.
+        Debian Bookworm, Bullseye, Buster as well as Lunar, Jammy, Focal packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/jessie-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         Finally,
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install python-nxsconfigserver nxsconfigserver-db
```

### Comparing `nxsconfigserver-db-1.10.4/README.rst` & `nxsconfigserver-db-1.10.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,29 @@
 	  $ mysql < conf/mysql_create.sql
 
 with proper privileges.
 
 Debian packages
 ^^^^^^^^^^^^^^^
 
-Debian Jessie (and Wheezy) packages can be found in the HDRI repository.
+Debian Bookworm, Bullseye, Buster as well as Lunar, Jammy, Focal packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
 	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
 
 and then download the corresponding source list
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/jessie-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
 
 Finally,
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install python-nxsconfigserver nxsconfigserver-db
```

### Comparing `nxsconfigserver-db-1.10.4/conf/my.cnf` & `nxsconfigserver-db-1.10.5/conf/my.cnf`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.4/conf/mysql_create.sql` & `nxsconfigserver-db-1.10.5/conf/mysql_create.sql`

 * *Files identical despite different names*

### Comparing `nxsconfigserver-db-1.10.4/setup.py` & `nxsconfigserver-db-1.10.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """ setup.py for NXS configuration server """
 
 import os
 
-from distutils.core import setup
+from setuptools import setup
 
 try:
     from sphinx.setup_command import BuildDoc
 except Exception:
     BuildDoc = None
 
 
@@ -34,15 +34,15 @@
 
     :param fname: readme file name
     """
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 #: (:obj:`str`) full release number
-release = '1.10.4'
+release = '1.10.5'
 #: (:obj:`str`) release verion number
 version = ".".join(release.split(".")[:2])
 #: (:obj:`str`) program name
 name = "NXSConfigServer-db"
 
 #: (:obj:`dict` <:obj:`str` , any >`) metadata for distutils
 SETUPDATA = dict(
```

