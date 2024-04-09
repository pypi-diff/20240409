# Comparing `tmp/pyams_security-2.2.1.tar.gz` & `tmp/pyams_security-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security-2.2.1.tar", last modified: Mon Feb 26 22:29:56 2024, max compression
+gzip compressed data, was "dist/pyams_security-2.3.0.tar", last modified: Tue Apr  9 18:35:25 2024, max compression
```

## Comparing `pyams_security-2.2.1.tar` & `pyams_security-2.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 10:29:46.000000 pyams_security-2.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 10:29:46.000000 pyams_security-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6716 2024-02-26 22:29:56.000000 pyams_security-2.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4818 2024-02-26 22:23:14.000000 pyams_security-2.2.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-01-03 10:29:46.000000 pyams_security-2.2.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 22:29:56.000000 pyams_security-2.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3016 2024-02-26 22:23:14.000000 pyams_security-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/api/
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/credentials.rst
--rw-rw-rw-   0 root         (0) root         (0)     6424 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/manager.rst
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)     7314 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/passwords.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/plugins.rst
--rw-rw-rw-   0 root         (0) root         (0)     5925 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/policy.rst
--rw-rw-rw-   0 root         (0) root         (0)    15805 2024-02-03 01:44:13.000000 pyams_security-2.2.1/src/pyams_security/doctests/principals.rst
--rw-rw-rw-   0 root         (0) root         (0)     3690 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     5633 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/rest.rst
--rw-rw-rw-   0 root         (0) root         (0)     6801 2024-02-26 22:23:14.000000 pyams_security-2.2.1/src/pyams_security/doctests/roles.rst
--rw-rw-rw-   0 root         (0) root         (0)    21085 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/security.rst
--rw-rw-rw-   0 root         (0) root         (0)    18842 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/doctests/users.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/generations/
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-01-24 17:07:04.000000 pyams_security-2.2.1/src/pyams_security/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/include.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    11198 2024-02-12 16:09:26.000000 pyams_security-2.2.1/src/pyams_security/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3910 2024-02-26 22:23:14.000000 pyams_security-2.2.1/src/pyams_security/interfaces/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/interfaces/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4234 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/interfaces/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2024-02-12 16:09:26.000000 pyams_security-2.2.1/src/pyams_security/interfaces/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1771 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/interfaces/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1969 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/interfaces/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/interfaces/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17669 2024-02-26 22:23:14.000000 pyams_security-2.2.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
--rw-rw-rw-   0 root         (0) root         (0)    29946 2024-02-26 22:23:14.000000 pyams_security-2.2.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
--rw-rw-rw-   0 root         (0) root         (0)    16683 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/locales/pyams_security.pot
--rw-rw-rw-   0 root         (0) root         (0)     2433 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     2957 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/password.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8272 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/plugin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/templates/password-reset.pt
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/templates/register-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/templates/register-info.pt
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/templates/register-message.pt
--rw-rw-rw-   0 root         (0) root         (0)    17750 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-12 16:09:26.000000 pyams_security-2.2.1/src/pyams_security/principal.py
--rw-rw-rw-   0 root         (0) root         (0)     4658 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/property.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     6297 2024-02-26 22:23:14.000000 pyams_security-2.2.1/src/pyams_security/role.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12790 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/security.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     9326 2024-02-12 16:09:26.000000 pyams_security-2.2.1/src/pyams_security/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-03 10:29:46.000000 pyams_security-2.2.1/src/pyams_security/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6716 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2583 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 22:29:46.000000 pyams_security-2.2.1/src/pyams_security.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-26 22:29:56.000000 pyams_security-2.2.1/src/pyams_security.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 10:29:46.000000 pyams_security-2.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 10:29:46.000000 pyams_security-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6772 2024-04-09 18:35:25.000000 pyams_security-2.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4874 2024-04-09 18:28:27.000000 pyams_security-2.3.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-01-03 10:29:46.000000 pyams_security-2.3.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 18:35:25.000000 pyams_security-2.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3016 2024-04-09 18:28:27.000000 pyams_security-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/credentials.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6424 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/manager.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/passwords.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/plugins.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5925 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/policy.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15805 2024-02-03 01:44:13.000000 pyams_security-2.3.0/src/pyams_security/doctests/principals.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5633 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/rest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/doctests/roles.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/doctests/security.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19460 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/doctests/users.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-01-24 17:07:04.000000 pyams_security-2.3.0/src/pyams_security/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4961 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    11198 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/interfaces/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    16708 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/interfaces/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/interfaces/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17669 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo
+-rw-rw-rw-   0 root         (0) root         (0)    29946 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po
+-rw-rw-rw-   0 root         (0) root         (0)    16683 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/locales/pyams_security.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/password.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8272 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/password-reset.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-info.pt
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/plugin/templates/register-message.pt
+-rw-rw-rw-   0 root         (0) root         (0)    18335 2024-04-09 18:28:27.000000 pyams_security-2.3.0/src/pyams_security/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/principal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2024-02-26 22:23:14.000000 pyams_security-2.3.0/src/pyams_security/role.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12790 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9326 2024-02-12 16:09:26.000000 pyams_security-2.3.0/src/pyams_security/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-03 10:29:46.000000 pyams_security-2.3.0/src/pyams_security/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6772 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:35:15.000000 pyams_security-2.3.0/src/pyams_security.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-09 18:35:25.000000 pyams_security-2.3.0/src/pyams_security.egg-info/top_level.txt
```

### Comparing `pyams_security-2.2.1/LICENSE` & `pyams_security-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/PKG-INFO` & `pyams_security-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security
-Version: 2.2.1
+Version: 2.3.0
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.0
+-----
+ - allow case-insensitive local user login
+
 2.2.1
 -----
  - added support for custom attributes in roles
 
 2.2.0
 -----
  - added marker interface to handle unknown or missing principals
```

### Comparing `pyams_security-2.2.1/docs/HISTORY.rst` & `pyams_security-2.3.0/docs/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.3.0
+-----
+ - allow case-insensitive local user login
+
 2.2.1
 -----
  - added support for custom attributes in roles
 
 2.2.0
 -----
  - added marker interface to handle unknown or missing principals
```

### Comparing `pyams_security-2.2.1/docs/README.rst` & `pyams_security-2.3.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/setup.py` & `pyams_security-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.2.1'
+version = '2.3.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_zmi'
 ]
```

### Comparing `pyams_security-2.2.1/src/pyams_security/__init__.py` & `pyams_security-2.3.0/src/pyams_security/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/api/__init__.py` & `pyams_security-2.3.0/src/pyams_security/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/credential.py` & `pyams_security-2.3.0/src/pyams_security/credential.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/README.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/credentials.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/credentials.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/manager.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/manager.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/notifications.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/notifications.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/passwords.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/passwords.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/plugins.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/plugins.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/policy.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/policy.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/principals.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/principals.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/profiles.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/profiles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/rest.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/rest.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/roles.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/roles.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/security.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/security.rst`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/doctests/users.rst` & `pyams_security-2.3.0/src/pyams_security/doctests/users.rst`

 * *Files 3% similar despite different names*

```diff
@@ -346,14 +346,45 @@
     >>> vocabulary = UsersFolderVocabulary()
     >>> len(vocabulary)
     1
     >>> pprint.pprint(vocabulary.by_value)
     {'users': <zope.schema.vocabulary.SimpleTerm object at 0x...>}
 
 
+Case insensitive login
+----------------------
+
+By default, local users folder login is case sensitive:
+
+    >>> folder.case_insensitive_login
+    False
+
+    >>> 'user1' in folder
+    True
+    >>> 'User1' in folder
+    False
+    >>> folder.get('User1') is None
+    True
+
+You can switch case sensitive property to False:
+
+    >>> folder.case_insensitive_login = True
+
+    >>> 'user1' in folder
+    True
+    >>> 'User1' in folder
+    True
+    >>> folder.get('User1') is user1
+    True
+
+    >>> folder['User4'] = LocalUser()
+    >>> sorted(folder.keys())
+    ['user1', 'user2@example.com', 'user3@example.com', 'user4']
+
+
 Principals groups
 -----------------
 
 Groups can be used to group principals together; permissions and roles can then be assigned to
 all group members in a single operation:
 
     >>> from pyams_security.interfaces.plugin import PrincipalsAddedToGroupEvent, \
```

### Comparing `pyams_security-2.2.1/src/pyams_security/generations/__init__.py` & `pyams_security-2.3.0/src/pyams_security/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/generations/evolve1.py` & `pyams_security-2.3.0/src/pyams_security/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/include.py` & `pyams_security-2.3.0/src/pyams_security/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/index.py` & `pyams_security-2.3.0/src/pyams_security/index.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/__init__.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/base.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/names.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/names.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/notification.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/plugin.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,19 @@
 
 
 class IUsersFolderPlugin(IAuthenticationPlugin, IDirectorySearchPlugin):
     """Local users folder interface"""
 
     contains('pyams_security.interfaces.ILocalUser')
 
+    case_insensitive_login = Bool(title=_("Use case insensitive login"),
+                                  description=_("If enabled, users login will not be case sensitive"),
+                                  required=True,
+                                  default=False)
+
     def check_login(self, login):
         """Check for existence of given login"""
 
 
 MAJS = range(ord('A'), ord('Z') + 1)
 MINS = range(ord('a'), ord('z') + 1)
 NUMS = range(ord('0'), ord('9') + 1)
```

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/profile.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/rest.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/interfaces/site.py` & `pyams_security-2.3.0/src/pyams_security/interfaces/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo` & `pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.mo`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po` & `pyams_security-2.3.0/src/pyams_security/locales/fr/LC_MESSAGES/pyams_security.po`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/locales/pyams_security.pot` & `pyams_security-2.3.0/src/pyams_security/locales/pyams_security.pot`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/notification.py` & `pyams_security-2.3.0/src/pyams_security/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/password.py` & `pyams_security-2.3.0/src/pyams_security/password.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/permission.py` & `pyams_security-2.3.0/src/pyams_security/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/__init__.py` & `pyams_security-2.3.0/src/pyams_security/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/admin.py` & `pyams_security-2.3.0/src/pyams_security/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/group.py` & `pyams_security-2.3.0/src/pyams_security/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/templates/password-reset.pt` & `pyams_security-2.3.0/src/pyams_security/plugin/templates/password-reset.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/templates/register-body.pt` & `pyams_security-2.3.0/src/pyams_security/plugin/templates/register-body.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/templates/register-info.pt` & `pyams_security-2.3.0/src/pyams_security/plugin/templates/register-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/plugin/userfolder.py` & `pyams_security-2.3.0/src/pyams_security/plugin/userfolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,39 @@
 class UsersFolder(Folder):
     """Local users folder"""
 
     prefix = FieldProperty(IUsersFolderPlugin['prefix'])
     title = FieldProperty(IUsersFolderPlugin['title'])
     enabled = FieldProperty(IUsersFolderPlugin['enabled'])
 
+    case_insensitive_login = FieldProperty(IUsersFolderPlugin['case_insensitive_login'])
+
+    def get(self, key, default=None):
+        if self.case_insensitive_login:
+            key = key.lower()
+        return super().get(key, default)
+
+    def __contains__(self, item):
+        if self.case_insensitive_login:
+            item = item.lower()
+        return super().__contains__(item)
+
+    def __setitem__(self, key, value):
+        if self.case_insensitive_login:
+            key = key.lower()
+        super().__setitem__(key, value)
+
     def authenticate(self, credentials, request):  # pylint: disable=unused-argument
         """Try to authenticate given credentials"""
         if not self.enabled:
             return None
         attrs = credentials.attributes
         login = attrs.get('login')
+        if not login:
+            return None
         principal = self.get(login)
         if principal is not None:
             password = attrs.get('password')
             if principal.check_password(password):
                 return PRINCIPAL_ID_FORMATTER.format(prefix=self.prefix,
                                                      login=principal.login)
         return None
```

### Comparing `pyams_security-2.2.1/src/pyams_security/policy.py` & `pyams_security-2.3.0/src/pyams_security/policy.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/principal.py` & `pyams_security-2.3.0/src/pyams_security/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/profile.py` & `pyams_security-2.3.0/src/pyams_security/profile.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/property.py` & `pyams_security-2.3.0/src/pyams_security/property.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/rest.py` & `pyams_security-2.3.0/src/pyams_security/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/role.py` & `pyams_security-2.3.0/src/pyams_security/role.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/schema.py` & `pyams_security-2.3.0/src/pyams_security/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/security.py` & `pyams_security-2.3.0/src/pyams_security/security.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/site.py` & `pyams_security-2.3.0/src/pyams_security/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/tests/__init__.py` & `pyams_security-2.3.0/src/pyams_security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/tests/test_utilsdocs.py` & `pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/tests/test_utilsdocstrings.py` & `pyams_security-2.3.0/src/pyams_security/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/utility.py` & `pyams_security-2.3.0/src/pyams_security/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security/vocabulary.py` & `pyams_security-2.3.0/src/pyams_security/vocabulary.py`

 * *Files identical despite different names*

### Comparing `pyams_security-2.2.1/src/pyams_security.egg-info/PKG-INFO` & `pyams_security-2.3.0/src/pyams_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security
-Version: 2.2.1
+Version: 2.3.0
 Summary: PyAMS security management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -50,14 +50,18 @@
 Finally, PyAMS_security provides ACLs and roles management, as well as custom schema fields to
 store roles assigned to principals.
 
 
 Changelog
 =========
 
+2.3.0
+-----
+ - allow case-insensitive local user login
+
 2.2.1
 -----
  - added support for custom attributes in roles
 
 2.2.0
 -----
  - added marker interface to handle unknown or missing principals
```

### Comparing `pyams_security-2.2.1/src/pyams_security.egg-info/SOURCES.txt` & `pyams_security-2.3.0/src/pyams_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

