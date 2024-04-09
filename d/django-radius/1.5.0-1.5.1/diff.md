# Comparing `tmp/django-radius-1.5.0.tar.gz` & `tmp/django-radius-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-radius-1.5.0.tar", last modified: Mon Mar  2 16:11:11 2020, max compression
+gzip compressed data, was "django-radius-1.5.1.tar", last modified: Tue Apr  9 13:02:16 2024, max compression
```

## Comparing `django-radius-1.5.0.tar` & `django-radius-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 robgolding   (501) staff       (20)        0 2020-03-02 16:11:11.000000 django-radius-1.5.0/
--rw-r--r--   0 robgolding   (501) staff       (20)      483 2020-03-02 16:11:11.000000 django-radius-1.5.0/PKG-INFO
--rw-r--r--   0 robgolding   (501) staff       (20)     8249 2019-09-15 16:06:46.000000 django-radius-1.5.0/README.md
-drwxr-xr-x   0 robgolding   (501) staff       (20)        0 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/
--rw-r--r--   0 robgolding   (501) staff       (20)      483 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/PKG-INFO
--rw-r--r--   0 robgolding   (501) staff       (20)      323 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/SOURCES.txt
--rw-r--r--   0 robgolding   (501) staff       (20)        1 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/dependency_links.txt
--rw-r--r--   0 robgolding   (501) staff       (20)        1 2017-10-25 19:07:58.000000 django-radius-1.5.0/django_radius.egg-info/not-zip-safe
--rw-r--r--   0 robgolding   (501) staff       (20)       26 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/requires.txt
--rw-r--r--   0 robgolding   (501) staff       (20)       11 2020-03-02 16:11:11.000000 django-radius-1.5.0/django_radius.egg-info/top_level.txt
-drwxr-xr-x   0 robgolding   (501) staff       (20)        0 2020-03-02 16:11:11.000000 django-radius-1.5.0/radiusauth/
--rw-r--r--   0 robgolding   (501) staff       (20)       18 2020-03-02 16:10:53.000000 django-radius-1.5.0/radiusauth/__init__.py
-drwxr-xr-x   0 robgolding   (501) staff       (20)        0 2020-03-02 16:11:11.000000 django-radius-1.5.0/radiusauth/backends/
--rw-r--r--   0 robgolding   (501) staff       (20)       73 2017-10-25 18:55:36.000000 django-radius-1.5.0/radiusauth/backends/__init__.py
--rw-r--r--   0 robgolding   (501) staff       (20)    10515 2019-09-15 16:06:46.000000 django-radius-1.5.0/radiusauth/backends/radius.py
--rw-r--r--   0 robgolding   (501) staff       (20)       38 2020-03-02 16:11:11.000000 django-radius-1.5.0/setup.cfg
--rw-r--r--   0 robgolding   (501) staff       (20)      675 2019-09-15 16:06:46.000000 django-radius-1.5.0/setup.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-09 13:02:16.316852 django-radius-1.5.1/
+-rw-r--r--   0 rob        (501) staff       (20)     1512 2024-04-09 12:53:23.000000 django-radius-1.5.1/LICENSE
+-rw-r--r--   0 rob        (501) staff       (20)      466 2024-04-09 13:02:16.316746 django-radius-1.5.1/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     8508 2024-04-09 12:53:32.000000 django-radius-1.5.1/README.md
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-09 13:02:16.315988 django-radius-1.5.1/django_radius.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      466 2024-04-09 13:02:16.000000 django-radius-1.5.1/django_radius.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)      331 2024-04-09 13:02:16.000000 django-radius-1.5.1/django_radius.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2024-04-09 13:02:16.000000 django-radius-1.5.1/django_radius.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2024-04-09 12:58:46.000000 django-radius-1.5.1/django_radius.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       17 2024-04-09 13:02:16.000000 django-radius-1.5.1/django_radius.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)       11 2024-04-09 13:02:16.000000 django-radius-1.5.1/django_radius.egg-info/top_level.txt
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-09 13:02:16.316103 django-radius-1.5.1/radiusauth/
+-rw-r--r--   0 rob        (501) staff       (20)       18 2024-04-09 12:55:22.000000 django-radius-1.5.1/radiusauth/__init__.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-09 13:02:16.316525 django-radius-1.5.1/radiusauth/backends/
+-rw-r--r--   0 rob        (501) staff       (20)       73 2024-04-09 12:53:23.000000 django-radius-1.5.1/radiusauth/backends/__init__.py
+-rw-r--r--   0 rob        (501) staff       (20)    10645 2024-04-09 12:53:32.000000 django-radius-1.5.1/radiusauth/backends/radius.py
+-rw-r--r--   0 rob        (501) staff       (20)       38 2024-04-09 13:02:16.316891 django-radius-1.5.1/setup.cfg
+-rw-r--r--   0 rob        (501) staff       (20)      663 2024-04-09 12:53:32.000000 django-radius-1.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-radius-1.5.0/README.md` & `django-radius-1.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 
 ```python
 RADIUS_SERVER = 'localhost'
 RADIUS_PORT = 1812
 RADIUS_SECRET = 'S3kr3T'
 ```
 
+You may optionally accept whether the user is a staff or superuser from the
+remote radius server with the following option. If not set, it will default
+to `True`, as django-radius has functioned in earlier versions.
+
+```python
+RADIUS_REMOTE_ROLES = True
+```
+
 When a user is successfully authenticated via the RADIUS backend, a `User`
 object is created in Django's built-in auth application with the same username.
 This user's password is set to the password which they logged into the RADIUS
 server with, so that they will be able to login with their "cached"
 credentials, even if the RADIUS server is down. All activity within the Django
 project can then be linked to this `User` object via foreign keys etc.
```

### Comparing `django-radius-1.5.0/radiusauth/backends/radius.py` & `django-radius-1.5.1/radiusauth/backends/radius.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from future import standard_library
-standard_library.install_aliases()
-from past.builtins import basestring
 from builtins import object
 import logging
 from io import StringIO
 
 from pyrad.packet import AccessRequest, AccessAccept, AccessReject
 from pyrad.client import Client, Timeout
 from pyrad.dictionary import Dictionary
@@ -100,15 +97,15 @@
 
     def _get_server_from_settings(self):
         """
         Get the RADIUS server details from the settings file.
         """
         return (
             settings.RADIUS_SERVER,
-            settings.RADIUS_PORT,
+            int(settings.RADIUS_PORT),
             settings.RADIUS_SECRET.encode('utf-8'),
         )
 
     def _perform_radius_auth(self, client, packet):
         """
         Perform the actual radius authentication by passing the given packet
         to the server which `client` is bound to.
@@ -132,26 +129,26 @@
         elif reply.code != AccessAccept:
             logging.error("RADIUS access error for user '%s' (code %s)" % (
                 packet['User-Name'], reply.code))
             return None
 
         logging.info("RADIUS access granted for user '%s'" % (
             packet['User-Name']))
-        
+
         if not "Class" in reply.keys():
             return [], False, False
 
         groups = []
         is_staff = False
         is_superuser = False
-        
+
         app_class_prefix = getattr(settings, 'RADIUS_CLASS_APP_PREFIX', '')
         group_class_prefix = app_class_prefix + "group="
         role_class_prefix = app_class_prefix + "role="
-        
+
         for cl in reply['Class']:
             cl = cl.decode("utf-8")
             if cl.lower().find(group_class_prefix) == 0:
                 groups.append(cl[len(group_class_prefix):])
             elif cl.lower().find(role_class_prefix) == 0:
                 role = cl[len(role_class_prefix):]
                 if role == "staff":
@@ -178,19 +175,25 @@
         password to that (regardless of whether the user was created or not).
         """
         try:
             user = User.objects.get(username=username)
         except User.DoesNotExist:
             user = User(username=username)
 
-        user.is_staff = is_staff
-        user.is_superuser = is_superuser
+        # if RADIUS_REMOTE_ROLES is not set, configure it to the default value
+        # of versions <= 1.4.0
+        if not hasattr(settings, "RADIUS_REMOTE_ROLES"):
+            settings.RADIUS_REMOTE_ROLES = True
+
+        if settings.RADIUS_REMOTE_ROLES:
+            user.is_staff = is_staff
+            user.is_superuser = is_superuser
         if password is not None:
             user.set_password(password)
-        
+
         user.save()
         user.groups.set(groups)
         return user
 
     def get_user_groups(self, group_names):
         groups = Group.objects.filter(name__in=group_names)
         if len(groups) != len(group_names):
```

### Comparing `django-radius-1.5.0/setup.py` & `django-radius-1.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         'Programming Language :: Python :: 3',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
     ],
     zip_safe=False,
     packages=find_packages(),
-    install_requires=['pyrad >= 1.2', 'future==0.16.0'],
+    install_requires=['pyrad >= 1.2,!=2.2'],
 )
```

