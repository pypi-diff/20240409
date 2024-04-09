# Comparing `tmp/Doggel_Inc-1.3.2.tar.gz` & `tmp/Doggel-Inc-1.4.1.tar.gz`

## Comparing `Doggel_Inc-1.3.2.tar` & `Doggel-Inc-1.4.1.tar`

### file list

```diff
@@ -9,16 +9,16 @@
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1370 2024-04-08 20:28:29.000000 Doggel_Inc/DICord/user.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     3424 2024-04-09 08:50:19.000000 Doggel_Inc/DICord/__init__.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      398 2024-04-08 18:00:53.000000 Doggel_Inc/DICord/message.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      136 2024-04-08 16:12:02.000000 Doggel_Inc/DICord/transformer.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      502 2024-04-08 18:35:06.000000 Doggel_Inc/DICord/msg.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      619 2024-04-08 20:28:08.000000 Doggel_Inc/DICord/channel.py
 -rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      647 2024-04-07 17:11:43.000000 Doggel_Inc/AI/AI.py
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      734 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/PKG-INFO
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       41 2024-04-09 09:04:59.000000 Doggel_Inc-1.3.2/README.md
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       38 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/setup.cfg
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      734 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/Doggel_Inc.egg-info/PKG-INFO
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      187 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/Doggel_Inc.egg-info/SOURCES.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/Doggel_Inc.egg-info/dependency_links.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       19 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/Doggel_Inc.egg-info/requires.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-09 09:05:58.000000 Doggel_Inc-1.3.2/Doggel_Inc.egg-info/top_level.txt
--rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1011 2024-04-09 09:03:57.000000 Doggel_Inc-1.3.2/setup.py
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      459 2024-04-09 12:25:05.000000 Doggel-Inc-1.4.1/pyproject.toml
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      434 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/PKG-INFO
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       41 2024-04-09 09:04:59.000000 Doggel-Inc-1.4.1/README.md
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)       38 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/setup.cfg
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      434 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/Doggel_Inc.egg-info/PKG-INFO
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)      169 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/Doggel_Inc.egg-info/SOURCES.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/Doggel_Inc.egg-info/dependency_links.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)        1 2024-04-09 12:26:14.000000 Doggel-Inc-1.4.1/Doggel_Inc.egg-info/top_level.txt
+-rw-r--r--   0 pterodactyl   (997) pterodactyl   (996)     1011 2024-04-09 12:24:59.000000 Doggel-Inc-1.4.1/setup.py
```

### Comparing `Doggel_Inc-1.3.2/setup.py` & `Doggel-Inc-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Doggel_Inc', 
-    version='1.3.2', 
+    version='1.4.1', 
     description='Doggeł Inc packages',
     author='Lordpomind',
     author_email='lordpomind@gmail.com',
     url='',  
     package_data={
         'Doggel_Inc': ["src/*"]
     },
```

