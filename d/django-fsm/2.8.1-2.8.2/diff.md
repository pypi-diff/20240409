# Comparing `tmp/django-fsm-2.8.1.tar.gz` & `tmp/django-fsm-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-fsm-2.8.1.tar", last modified: Mon Aug 15 10:46:03 2022, max compression
+gzip compressed data, was "django-fsm-2.8.2.tar", last modified: Tue Apr  9 07:29:48 2024, max compression
```

## Comparing `django-fsm-2.8.1.tar` & `django-fsm-2.8.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2022-08-15 10:46:03.000000 django-fsm-2.8.1/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1883 2022-08-15 10:44:23.000000 django-fsm-2.8.1/setup.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2022-08-15 10:46:03.000000 django-fsm-2.8.1/django_fsm.egg-info/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       11 2022-08-15 10:46:02.000000 django-fsm-2.8.1/django_fsm.egg-info/top_level.txt
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2019-12-03 07:14:58.000000 django-fsm-2.8.1/django_fsm.egg-info/not-zip-safe
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      393 2022-08-15 10:46:02.000000 django-fsm-2.8.1/django_fsm.egg-info/SOURCES.txt
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1601 2022-08-15 10:46:02.000000 django-fsm-2.8.1/django_fsm.egg-info/PKG-INFO
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2022-08-15 10:46:02.000000 django-fsm-2.8.1/django_fsm.egg-info/dependency_links.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1601 2022-08-15 10:46:03.000000 django-fsm-2.8.1/PKG-INFO
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    12197 2022-08-15 10:45:08.000000 django-fsm-2.8.1/README.rst
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2022-08-15 10:46:03.000000 django-fsm-2.8.1/django_fsm/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      113 2020-10-13 11:09:05.000000 django-fsm-2.8.1/django_fsm/signals.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       88 2019-12-03 06:33:03.000000 django-fsm-2.8.1/django_fsm/models.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    23392 2022-08-15 10:15:22.000000 django-fsm-2.8.1/django_fsm/__init__.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2022-08-15 10:46:03.000000 django-fsm-2.8.1/django_fsm/management/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2022-08-15 10:46:03.000000 django-fsm-2.8.1/django_fsm/management/commands/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9065 2022-08-15 10:15:22.000000 django-fsm-2.8.1/django_fsm/management/commands/graph_transitions.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-12-03 06:33:03.000000 django-fsm-2.8.1/django_fsm/management/commands/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-12-03 06:33:03.000000 django-fsm-2.8.1/django_fsm/management/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      131 2022-08-15 10:46:03.000000 django-fsm-2.8.1/setup.cfg
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2024-04-09 07:29:48.896561 django-fsm-2.8.2/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1062 2019-12-03 06:33:03.000000 django-fsm-2.8.2/LICENSE
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1872 2024-04-09 07:29:48.896561 django-fsm-2.8.2/PKG-INFO
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    12349 2024-04-09 07:27:25.000000 django-fsm-2.8.2/README.rst
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2024-04-09 07:29:48.892562 django-fsm-2.8.2/django_fsm/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    24695 2023-12-21 09:18:02.000000 django-fsm-2.8.2/django_fsm/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2024-04-09 07:29:48.896561 django-fsm-2.8.2/django_fsm/management/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-12-03 06:33:03.000000 django-fsm-2.8.2/django_fsm/management/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2024-04-09 07:29:48.896561 django-fsm-2.8.2/django_fsm/management/commands/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-12-03 06:33:03.000000 django-fsm-2.8.2/django_fsm/management/commands/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9225 2024-04-09 07:28:01.000000 django-fsm-2.8.2/django_fsm/management/commands/graph_transitions.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       88 2019-12-03 06:33:03.000000 django-fsm-2.8.2/django_fsm/models.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      113 2020-10-13 11:09:05.000000 django-fsm-2.8.2/django_fsm/signals.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2024-04-09 07:29:48.896561 django-fsm-2.8.2/django_fsm.egg-info/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1872 2024-04-09 07:29:48.000000 django-fsm-2.8.2/django_fsm.egg-info/PKG-INFO
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      401 2024-04-09 07:29:48.000000 django-fsm-2.8.2/django_fsm.egg-info/SOURCES.txt
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2024-04-09 07:29:48.000000 django-fsm-2.8.2/django_fsm.egg-info/dependency_links.txt
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2019-12-03 07:14:58.000000 django-fsm-2.8.2/django_fsm.egg-info/not-zip-safe
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       11 2024-04-09 07:29:48.000000 django-fsm-2.8.2/django_fsm.egg-info/top_level.txt
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      131 2024-04-09 07:29:48.896561 django-fsm-2.8.2/setup.cfg
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2148 2024-04-09 07:26:32.000000 django-fsm-2.8.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-fsm-2.8.1/django_fsm.egg-info/PKG-INFO` & `django-fsm-2.8.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-fsm
-Version: 2.8.1
+Version: 2.8.2
 Summary: Django friendly finite state machine support.
 Home-page: http://github.com/kmmbvnr/django-fsm
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: MIT License
-Description: UNKNOWN
 Keywords: django
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,20 +20,27 @@
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `django-fsm-2.8.1/PKG-INFO` & `django-fsm-2.8.2/django_fsm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-fsm
-Version: 2.8.1
+Version: 2.8.2
 Summary: Django friendly finite state machine support.
 Home-page: http://github.com/kmmbvnr/django-fsm
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: MIT License
-Description: UNKNOWN
 Keywords: django
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,20 +20,27 @@
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Framework :: Django
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `django-fsm-2.8.1/README.rst` & `django-fsm-2.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 ``source`` state
 ~~~~~~~~~~~~~~~~
 
 ``source`` parameter accepts a list of states, or an individual state or ``django_fsm.State`` implementation.
 
 You can use ``*`` for ``source`` to allow switching to ``target`` from any state. 
 
-You can use ``+`` for ``source`` to allow switching to ``target`` from any state exluding ``target`` state.
+You can use ``+`` for ``source`` to allow switching to ``target`` from any state excluding ``target`` state.
 
 ``target`` state
 ~~~~~~~~~~~~~~~~
 
 ``target`` state parameter could point to a specific state or ``django_fsm.State`` implementation
 
 .. code:: python
@@ -401,15 +401,15 @@
 practically negating their effect.
 
 Drawing transitions
 -------------------
 
 Renders a graphical overview of your models states transitions
 
-You need ``pip install graphviz>=0.4`` library and add ``django_fsm`` to
+You need ``pip install "graphviz>=0.4"`` library and add ``django_fsm`` to
 your ``INSTALLED_APPS``:
 
 .. code:: python
 
     INSTALLED_APPS = (
         ...
         'django_fsm',
@@ -423,15 +423,17 @@
 
     # Create a PNG image file only for specific model
     $ ./manage.py graph_transitions -o blog_transitions.png myapp.Blog
 
 Changelog
 ---------
 
-
-django-fsm 2.8.1 2022-08-15
+django-fsm 2.8.2 2024-04-09
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-- Improve fix for get_available_FIELD_transition
+- Fix graph_transitions commnad for Django>=4.0
+- Preserve chosen "using" DB in ConcurentTransitionMixin
+- Fix error message in GET_STATE
+- Implement Transition __hash__ and __eq__ for 'in' operator
 
 .. |Build Status| image:: https://travis-ci.org/viewflow/django-fsm.svg?branch=master
    :target: https://travis-ci.org/viewflow/django-fsm
```

### Comparing `django-fsm-2.8.1/django_fsm/__init__.py` & `django-fsm-2.8.2/django_fsm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,25 @@
         elif user.has_perm(self.permission, instance):
             return True
         elif user.has_perm(self.permission):
             return True
         else:
             return False
 
+    def __hash__(self):
+        return hash(self.name)
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            return other == self.name
+        if isinstance(other, Transition):
+            return other.name == self.name
+
+        return False
+
 
 def get_available_FIELD_transitions(instance, field):
     """
     List of transitions available in current model state
     with all conditions met
     """
     curr_state = field.get_state(instance)
@@ -467,14 +478,40 @@
     def get_state(self, instance):
         return instance.__dict__[self.attname]
 
     def set_state(self, instance, state):
         instance.__dict__[self.attname] = self.to_python(state)
 
 
+class FSMModelMixin(object):
+    """
+    Mixin that allows refresh_from_db for models with fsm protected fields
+    """
+
+    def _get_protected_fsm_fields(self):
+        def is_fsm_and_protected(f):
+            return isinstance(f, FSMFieldMixin) and f.protected
+        protected_fields = filter(is_fsm_and_protected, self._meta.concrete_fields)
+        return {f.attname for f in protected_fields}
+
+    def refresh_from_db(self, *args, **kwargs):
+        fields = kwargs.pop("fields", None)
+
+        # Use provided fields, if not set then reload all non-deferred fields.0
+        if not fields:
+            deferred_fields = self.get_deferred_fields()
+            protected_fields = self._get_protected_fsm_fields()
+            skipped_fields = deferred_fields.union(protected_fields)
+
+            fields = [f.attname for f in self._meta.concrete_fields
+                      if f.attname not in skipped_fields]
+
+        kwargs['fields'] = fields
+        super(FSMModelMixin, self).refresh_from_db(*args, **kwargs)
+
 class ConcurrentTransitionMixin(object):
     """
     Protects a Model from undesirable effects caused by concurrently executed transitions,
     e.g. running the same transition multiple times at the same time, or running different
     transitions with the same SOURCE state at the same time.
 
     This behavior is achieved using an idea based on optimistic locking. No additional
@@ -526,15 +563,15 @@
 
         # It may happen that nothing was updated in the original _do_update method not because of unmatching state,
         # but because of missing PK. This codepath is possible when saving a new model instance with *preset PK*.
         # In this case Django does not know it has to do INSERT operation, so it tries UPDATE first and falls back to
         # INSERT if UPDATE fails.
         # Thus, we need to make sure we only catch the case when the object *is* in the DB, but with changed state; and
         # mimic standard _do_update behavior otherwise. Django will pick it up and execute _do_insert.
-        if not updated and base_qs.filter(pk=pk_val).exists():
+        if not updated and base_qs.filter(pk=pk_val).using(using).exists():
             raise ConcurrentTransition("Cannot save object! The state has been changed since fetched from the database!")
 
         return updated
 
     def _update_initial_state(self):
         self.__initial_states = dict((field.attname, field.value_from_object(self)) for field in self.state_fields)
 
@@ -638,9 +675,9 @@
         self.func = func
         self.allowed_states = states
 
     def get_state(self, model, transition, result, args=[], kwargs={}):
         result_state = self.func(model, *args, **kwargs)
         if self.allowed_states is not None:
             if result_state not in self.allowed_states:
-                raise InvalidResultState("{} is not in list of allowed states\n{}".format(result, self.allowed_states))
+                raise InvalidResultState("{} is not in list of allowed states\n{}".format(result_state, self.allowed_states))
         return result_state
```

### Comparing `django-fsm-2.8.1/django_fsm/management/commands/graph_transitions.py` & `django-fsm-2.8.2/django_fsm/management/commands/graph_transitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import graphviz
 from optparse import make_option
 from itertools import chain
 
 from django.core.management.base import BaseCommand
 try:
     from django.utils.encoding import force_text
+    _requires_system_checks = True
 except ImportError:  # Django >= 4.0
     from django.utils.encoding import force_str as force_text
+    from django.core.management.base import ALL_CHECKS
+    _requires_system_checks = ALL_CHECKS
 
 from django_fsm import FSMFieldMixin, GET_STATE, RETURN_VALUE
 
 try:
     from django.db.models import get_apps, get_app, get_models, get_model
 
     NEW_META_API = False
@@ -98,17 +101,17 @@
         subgraph = graphviz.Digraph(
             name="cluster_%s_%s_%s" % (opts.app_label, opts.object_name, field.name),
             graph_attr={"label": "%s.%s.%s" % (opts.app_label, opts.object_name, field.name)},
         )
 
         final_states = targets - sources
         for name, label in final_states:
-            subgraph.node(name, label=label, shape="doublecircle")
+            subgraph.node(name, label=str(label), shape="doublecircle")
         for name, label in (sources | targets) - final_states:
-            subgraph.node(name, label=label, shape="circle")
+            subgraph.node(name, label=str(label), shape="circle")
             if field.default:  # Adding initial state notation
                 if label == field.default:
                     initial_name = node_name(field, "_initial")
                     subgraph.node(name=initial_name, label="", shape="point")
                     subgraph.edge(initial_name, name)
         for source_name, target_name, attrs in edges:
             subgraph.edge(source_name, target_name, **dict(attrs))
@@ -131,15 +134,15 @@
 
         return graphviz.backend.ENGINES
     except Exception:
         return {"sfdp", "circo", "twopi", "dot", "neato", "fdp", "osage", "patchwork"}
 
 
 class Command(BaseCommand):
-    requires_system_checks = True
+    requires_system_checks = _requires_system_checks
 
     if not HAS_ARGPARSE:
         option_list = BaseCommand.option_list + (
             make_option(
                 "--output",
                 "-o",
                 action="store",
```

