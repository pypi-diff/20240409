# Comparing `tmp/fractal_database-0.0.8.tar.gz` & `tmp/fractal_database-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_database-0.0.8.tar", max compression
+gzip compressed data, was "fractal_database-0.0.9.tar", max compression
```

## Comparing `fractal_database-0.0.8.tar` & `fractal_database-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       71 2024-02-14 19:15:43.854789 fractal_database-0.0.8/README.md
--rw-r--r--   0        0        0      401 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/__init__.py
--rw-r--r--   0        0        0       63 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/admin.py
--rw-r--r--   0        0        0     3172 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/apps.py
--rw-r--r--   0        0        0    35485 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/controllers/fractal_database_controller.py
--rw-r--r--   0        0        0      206 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/exceptions.py
--rw-r--r--   0        0        0     1067 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/fields.py
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/management/commands/__init__.py
--rw-r--r--   0        0        0     5019 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/management/commands/replicate.py
--rw-r--r--   0        0        0    10657 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/migrations/__init__.py
--rw-r--r--   0        0        0    23208 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/models.py
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/replication/__init__.py
--rw-r--r--   0        0        0     1385 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/replication/tasks.py
--rw-r--r--   0        0        0     1445 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/representations.py
--rw-r--r--   0        0        0    21547 2024-02-14 19:15:43.854789 fractal_database-0.0.8/fractal_database/signals.py
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/__init__.py-tpl
--rw-r--r--   0        0        0       63 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/admin.py-tpl
--rw-r--r--   0        0        0      363 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/apps.py-tpl
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/migrations/__init__.py-tpl
--rw-r--r--   0        0        0      109 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/models.py-tpl
--rw-r--r--   0        0        0       60 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/tests.py-tpl
--rw-r--r--   0        0        0       63 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/app_template/views.py-tpl
--rwxr-xr-x   0        0        0      674 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/manage.py-tpl
--rw-r--r--   0        0        0        0 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      428 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/project_name/asgi.py-tpl
--rw-r--r--   0        0        0     3655 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/project_name/settings.py-tpl
--rw-r--r--   0        0        0      789 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0      428 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/templates/project_template/project_name/wsgi.py-tpl
--rw-r--r--   0        0        0     3149 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/utils.py
--rw-r--r--   0        0        0       63 2024-02-14 19:15:43.858789 fractal_database-0.0.8/fractal_database/views.py
--rw-r--r--   0        0        0      464 2024-02-14 19:15:43.858789 fractal_database-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 fractal_database-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-03-04 17:41:09.189615 fractal_database-0.0.9/README.md
+-rw-r--r--   0        0        0      401 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/__init__.py
+-rw-r--r--   0        0        0       63 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/admin.py
+-rw-r--r--   0        0        0     3856 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/apps.py
+-rw-r--r--   0        0        0    35485 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/controllers/fractal_database_controller.py
+-rw-r--r--   0        0        0      206 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/exceptions.py
+-rw-r--r--   0        0        0     1067 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/fields.py
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/management/commands/__init__.py
+-rw-r--r--   0        0        0     5021 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/management/commands/replicate.py
+-rw-r--r--   0        0        0    10717 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/migrations/__init__.py
+-rw-r--r--   0        0        0    23148 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/models.py
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/replication/__init__.py
+-rw-r--r--   0        0        0     1385 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/replication/tasks.py
+-rw-r--r--   0        0        0     1498 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/representations.py
+-rw-r--r--   0        0        0    22750 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/signals.py
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0       63 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/admin.py-tpl
+-rw-r--r--   0        0        0      363 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/apps.py-tpl
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/migrations/__init__.py-tpl
+-rw-r--r--   0        0        0      109 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/models.py-tpl
+-rw-r--r--   0        0        0       60 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/tests.py-tpl
+-rw-r--r--   0        0        0       63 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/app_template/views.py-tpl
+-rwxr-xr-x   0        0        0      674 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/manage.py-tpl
+-rw-r--r--   0        0        0        0 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      428 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/project_name/asgi.py-tpl
+-rw-r--r--   0        0        0     3655 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/project_name/settings.py-tpl
+-rw-r--r--   0        0        0      789 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0      428 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/templates/project_template/project_name/wsgi.py-tpl
+-rw-r--r--   0        0        0     3149 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/utils.py
+-rw-r--r--   0        0        0       63 2024-03-04 17:41:09.189615 fractal_database-0.0.9/fractal_database/views.py
+-rw-r--r--   0        0        0      900 2024-03-04 17:41:09.193615 fractal_database-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 fractal_database-0.0.9/PKG-INFO
```

### Comparing `fractal_database-0.0.8/fractal_database/apps.py` & `fractal_database-0.0.9/fractal_database/apps.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     default_auto_field = "django.db.models.BigAutoField"
     name = "fractal_database"
 
     def ready(self):
         from fractal_database.models import Database, Device, ReplicatedModel
         from fractal_database.signals import (
             create_database_and_matrix_replication_target,
+            initialize_fractal_app_catalog,
             join_device_to_database,
             register_device_account,
             schedule_replication_on_m2m_change,
             upload_exported_apps,
         )
 
         #   Assert that fractal_database is last in INSTALLED_APPS
@@ -34,21 +35,29 @@
 
         # create the instance database for the project
         if not os.environ.get("MATRIX_ROOM_ID"):
             # create the matrix replication target for the project database
             models.signals.post_migrate.connect(
                 create_database_and_matrix_replication_target, sender=self
             )
+            models.signals.post_migrate.connect(initialize_fractal_app_catalog, sender=self)
         else:
             logger.warning(
                 "MATRIX_ROOM_ID is set, not creating database and matrix replication target."
             )
 
         models.signals.post_migrate.connect(upload_exported_apps, sender=self)
+
+        # connect the signal to register the device account for the Device model and its subclasses
         models.signals.post_save.connect(register_device_account, sender=Device)
+        for model in Device.get_subclasses():
+            logger.debug(
+                f"Connecting register_device_account signal for Device subclass: {model}"
+            )
+            models.signals.post_save.connect(register_device_account, sender=model)
 
         # automatically connect schedule replication signal for replicated models that have
         # many to many fields on them.
         for model in ReplicatedModel.models:
             for field in model._meta.get_fields():
                 # skip fields that aren't many to many
                 if not isinstance(field, ManyToManyField) and not isinstance(
@@ -60,14 +69,18 @@
                     field_name = field.name
                 elif isinstance(field, ManyToManyRel):
                     if field.related_name:
                         field_name = field.related_name
                     else:
                         field_name = f"{field.name}_set"
 
+                    # verify that this field is a ReplicatedModel subclass
+                    if not issubclass(field.related_model, ReplicatedModel):
+                        continue
+
                 through = getattr(model, field_name).through
                 if through is not None:
                     models.signals.m2m_changed.connect(
                         schedule_replication_on_m2m_change, sender=through
                     )
 
     @staticmethod
```

### Comparing `fractal_database-0.0.8/fractal_database/controllers/fractal_database_controller.py` & `fractal_database-0.0.9/fractal_database/controllers/fractal_database_controller.py`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/fields.py` & `fractal_database-0.0.9/fractal_database/fields.py`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/management/commands/replicate.py` & `fractal_database-0.0.9/fractal_database/management/commands/replicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import socket
 import json
 import os
+import socket
 import sys
 
-from django.core.exceptions import ObjectDoesNotExist
-from fractal.matrix.async_client import MatrixClient
 from asgiref.sync import async_to_sync
+from django.core.exceptions import ObjectDoesNotExist
 from django.core.management.base import BaseCommand, CommandError
-from fractal_database.models import Database, Device, DatabaseConfig
-from fractal_database_matrix.models import MatrixReplicationTarget, MatrixCredentials
+from fractal.matrix.async_client import MatrixClient
+from fractal_database.models import Database, DatabaseConfig, Device
+from fractal_database_matrix.models import MatrixCredentials, MatrixReplicationTarget
 from nio import RoomGetStateEventError
 
 
 class Command(BaseCommand):
     help = "Starts a replication process for the configured database."
 
     def add_arguments(self, parser):
@@ -38,21 +38,23 @@
             target_state_res = await client.room_get_state_event(room_id, "f.database")
             if isinstance(target_state_res, RoomGetStateEventError):
                 raise CommandError(
                     f"Failed to get database configuration from room state: {target_state_res.message}"
                 )
             # FIXME: Put into own function
             from fractal_database_matrix.broker import broker
+
             broker._init_queues()
             broker.replication_queue.checkpoint.since_token = None
             from fractal_database.replication.tasks import replicate_fixture
-            fixture_str = db_state_res.content['fixture']
+
+            fixture_str = db_state_res.content["fixture"]
             fixture = json.loads(fixture_str)
             await replicate_fixture(fixture)
-            fixture_str = target_state_res.content['fixture']
+            fixture_str = target_state_res.content["fixture"]
             fixture = json.loads(fixture_str)
             await replicate_fixture(fixture)
 
         database = await Database.objects.aget(pk=fixture["pk"])
         target = await database.aprimary_target()
 
         await DatabaseConfig.objects.acreate(current_db=database)
```

### Comparing `fractal_database-0.0.8/fractal_database/migrations/0001_initial.py` & `fractal_database-0.0.9/fractal_database/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 5.0.2 on 2024-02-12 22:52
+# Generated by Django 5.0.2 on 2024-02-22 21:00
 
 import django.core.serializers.json
 import django.db.models.deletion
 import fractal_database.fields
 from django.db import migrations, models
 
 
@@ -101,14 +101,15 @@
             name='App',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('date_created', models.DateTimeField(auto_now_add=True)),
                 ('date_modified', models.DateTimeField(auto_now=True)),
                 ('deleted', models.BooleanField(default=False)),
                 ('object_version', models.PositiveIntegerField(default=0)),
+                ('name', models.CharField(max_length=255)),
                 ('app_instance_id', models.CharField(max_length=255, unique=True)),
                 ('metadata', models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, to='fractal_database.appcatalog')),
                 ('devices', models.ManyToManyField(to='fractal_database.device')),
             ],
             options={
                 'abstract': False,
             },
```

### Comparing `fractal_database-0.0.8/fractal_database/models.py` & `fractal_database-0.0.9/fractal_database/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from fractal_database.exceptions import StaleObjectException
 from fractal_database.representations import Representation
 
 from .fields import SingletonField
 from .signals import defer_replication
 
 if TYPE_CHECKING:
+    from fractal_database.models import ReplicatedModel
     from fractal_database_matrix.models import (
         MatrixCredentials,
         MatrixReplicationTarget,
     )
 
 logger = logging.getLogger(__name__)
 # to get console output from logger:
@@ -72,14 +73,53 @@
                 fields=["singleton"],
                 condition=models.Q(singleton=True),
                 name="unique_database_singleton",
             )
         ]
 
 
+class RepresentationLog(BaseModel):
+    target = GenericForeignKey("target_type", "target_id")
+    target_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.CASCADE,
+        related_name="%(app_label)s_%(class)s_target_type",
+    )
+    target_id = models.CharField(max_length=255)
+    method = models.CharField(max_length=255)
+    instance: "ReplicatedModel" = GenericForeignKey()  # type: ignore
+    object_id = models.CharField(max_length=255)
+    content_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.CASCADE,
+        related_name="%(app_label)s_%(class)s_content_type",
+    )
+    metadata = models.JSONField(default=dict, encoder=DjangoJSONEncoder)
+
+    @classmethod
+    def _get_repr_instance(cls, module: str) -> Representation:
+        """
+        Imports and returns the provided method.
+        """
+        repr_module, repr_class = module.rsplit(".", 1)
+        repr_module = import_module(repr_module)
+        repr_class = getattr(repr_module, repr_class)
+        return repr_class()
+
+    async def apply(self) -> None:
+        model: models.Model = self.content_type.model_class()  # type: ignore
+        instance = await model.objects.aget(pk=self.object_id)
+        repr_instance = self._get_repr_instance(self.method)
+        logger.info("Calling create_representation method on: ", repr_instance)
+        metadata = await repr_instance.create_representation(self, self.target_id)  # type: ignore
+        if metadata:
+            await instance.store_metadata(metadata)  # type: ignore
+        await self.aupdate(deleted=True)
+
+
 class ReplicatedModel(BaseModel):
     object_version = models.PositiveIntegerField(default=0)
     reprlog_set = GenericRelation("fractal_database.RepresentationLog")
     replication_configs = GenericRelation("fractal_database.ReplicatedInstanceConfig")
     models = []
 
     class Meta:
@@ -113,14 +153,18 @@
     @classmethod
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         # keep track of subclasses so we can register signals for them in App.ready
         ReplicatedModel.models.append(cls)
 
     @classmethod
+    def get_subclasses(cls, **kwargs):
+        return cls.__subclasses__()
+
+    @classmethod
     def connect_signals(cls, **kwargs):
         from fractal_database.signals import object_post_save, update_target_state
 
         for model_class in cls.models:
             logger.info(
                 'Registering replication signals for model "{}"'.format(model_class.__name__)
             )
@@ -132,49 +176,49 @@
 
     def schedule_replication(self, created: bool = False, database: Optional["Database"] = None):
         # must be in a txn for defer_replication to work properly
         if not transaction.get_connection().in_atomic_block:
             with transaction.atomic():
                 return self.schedule_replication(created=created)
 
-        print("Inside ReplicatedModel.schedule_replication()")
+        logger.debug(f"Inside ReplicatedModel.schedule_replication() for {self}")
         if not database:
             try:
                 database = Database.current_db()
             except Database.DoesNotExist as e:
                 logger.error("Unable to get current database from schedule_replication")
                 return
 
         # TODO replication targets to implement their own serialization strategy
         targets = database.get_all_replication_targets()  # type: ignore
         targets.extend(self.replication_targets())
+        if isinstance(self, ReplicationTarget) and self not in targets:
+            targets.append(self)
 
         repr_logs = None
         for target in targets:
-            # pass this replicated model instance to the target's replication method
-            if created or not target.metadata:
+            if created and not target.metadata:
                 # only allow targets to create representations for themselves,
                 # targets should not create representations for other targets
-                # targets always use their own credentials
                 if isinstance(self, ReplicationTarget) and self == target:
                     repr_logs = target.create_representation_logs(self)
             else:
-                print("Not creating repr for object: ", self)
+                logger.info("Not creating repr for object: ", self)
 
-            print(f"Creating replication log for target {target}")
+            logger.info(f"Creating replication log for target {target}")
             repl_log = ReplicationLog.objects.create(
                 payload=self.to_fixture(),
                 target=target,
                 instance=self,
                 txn_id=transaction.savepoint().split("_")[0],
             )
 
             # dummy targets return none
             if repr_logs:
-                print("Adding repr logs to repl log")
+                logger.info("Adding repr logs to repl log")
                 repl_log.repr_logs.add(*repr_logs)
 
             defer_replication(target)
 
     def to_fixture(self, json: bool = False) -> Union[str, List[Dict[str, Any]]]:
         if json:
             return serialize("json", [self])
@@ -343,21 +387,21 @@
             async for log in queryset:
                 async for repr_log in (
                     log.repr_logs.select_related("content_type", "target_type")
                     .filter(deleted=False)
                     .order_by("date_created")
                 ):
                     try:
-                        print("Calling apply for repr log: ", repr_log)
+                        logger.info("Calling apply for repr log: ", repr_log)
                         await repr_log.apply()
                         # after applying a representation for this target,
                         # we need to refresh ourself to get any latest metadata
-                        if repr_log.content_type.model_class() == self.__class__:
-                            logger.info(f"Refreshing {self} after applying representation")
-                            await self.arefresh_from_db()
+                        # if repr_log.content_type.model_class() == self.__class__:
+                        logger.info(f"Refreshing {self} after applying representation")
+                        await self.arefresh_from_db()
                         # call replicate again since apply will create new
                         # replication logs
                         return await self.replicate()
                     except Exception as e:
                         logger.error(f"Error applying representation log: {e}")
                         continue
                 fixture.append(log.payload[0])
@@ -367,30 +411,30 @@
                 # bulk update all of the logs in the queryset to deleted
                 await queryset.aupdate(deleted=True)
             except Exception as e:
                 logger.error(f"Error pushing replication log: {e}")
 
     async def store_metadata(self, metadata: dict) -> None:
         """
-        Store the Matrix room_id on target
+        Store the metadata on target.
         """
-        self.metadata["room_id"] = metadata["room_id"]
+        self.metadata.update(metadata)
         await self.asave()
 
     def create_representation_logs(self, instance: "ReplicatedModel"):
         """
         Create the representation logs (tasks) for creating a Matrix space
         """
         repr_logs = []
         repr_module = instance.get_representation_module()
         if not repr_module:
             return []
         repr_type = RepresentationLog._get_repr_instance(repr_module)
 
-        print(f"Creating repr {repr_type} logs for instance {instance} on target {self}")
+        logger.info(f"Creating repr {repr_type} logs for instance {instance} on target {self}")
         repr_logs.extend(repr_type.create_representation_logs(instance, self))
         return repr_logs
 
     def save(self, *args, **kwargs):
         if not self.pk:  # If this is a new object (no primary key yet)
             # Set the content_type to the current model
             self.content_type = ContentType.objects.get_for_model(self.__class__)
@@ -411,54 +455,15 @@
                 target_id=self.pk,
                 target_type=self.get_content_type(),
             ).order_by("date_created")
             async for txn_id in txn_ids
         ]
 
     def __str__(self) -> str:
-        return f"{self.name}"
-
-
-class RepresentationLog(BaseModel):
-    target = GenericForeignKey("target_type", "target_id")
-    target_type = models.ForeignKey(
-        ContentType,
-        on_delete=models.CASCADE,
-        related_name="%(app_label)s_%(class)s_target_type",
-    )
-    target_id = models.CharField(max_length=255)
-    method = models.CharField(max_length=255)
-    instance: "ReplicatedModel" = GenericForeignKey()  # type: ignore
-    object_id = models.CharField(max_length=255)
-    content_type = models.ForeignKey(
-        ContentType,
-        on_delete=models.CASCADE,
-        related_name="%(app_label)s_%(class)s_content_type",
-    )
-    metadata = models.JSONField(default=dict, encoder=DjangoJSONEncoder)
-
-    @classmethod
-    def _get_repr_instance(cls, module: str) -> Representation:
-        """
-        Imports and returns the provided method.
-        """
-        repr_module, repr_class = module.rsplit(".", 1)
-        repr_module = import_module(repr_module)
-        repr_class = getattr(repr_module, repr_class)
-        return repr_class()
-
-    async def apply(self) -> None:
-        model: models.Model = self.content_type.model_class()  # type: ignore
-        instance = await model.objects.aget(pk=self.object_id)
-        repr_instance = self._get_repr_instance(self.method)
-        print("Calling create_representation method on: ", repr_instance)
-        metadata = await repr_instance.create_representation(self, self.target_id)  # type: ignore
-        if metadata:
-            await instance.store_metadata(metadata)  # type: ignore
-        await self.aupdate(deleted=True)
+        return f"{self.name} ({self.__class__.__name__})"
 
 
 class DummyReplicationTarget(ReplicationTarget):
     async def replicate(*args, **kwargs):
         pass
 
     def create_representation_logs(self, instance):
@@ -557,14 +562,15 @@
 
 
 class App(ReplicatedModel):
     """
     created when doing `fractal install`
     """
 
+    name = models.CharField(max_length=255)
     app_instance_id = models.CharField(max_length=255, unique=True)
     metadata = models.ForeignKey(AppCatalog, on_delete=models.DO_NOTHING)
     devices = models.ManyToManyField("fractal_database.Device")
 
 
 class Device(ReplicatedModel):
     # type hint for MatrixCredentials reverse relation
@@ -572,15 +578,14 @@
 
     name = models.CharField(max_length=255, unique=True)
     display_name = models.CharField(max_length=255, null=True, blank=True)
     owner_matrix_id = models.CharField(max_length=255, null=True, blank=True)
 
     def __str__(self) -> str:
         return self.name
-        # return str([cred.matrix_id for cred in self.matrixcredentials_set.all()])
 
     @classmethod
     def current_device(cls) -> "Device":
         """
         Returns the current device.
         """
         try:
@@ -597,19 +602,14 @@
     async def acurrent_device(cls) -> "Device":
         """
         Returns the current device.
         """
         return await sync_to_async(cls.current_device)()
 
 
-# class DeviceDatabaseConfig(ReplicatedModel):
-#     device = models.ForeignKey(Device, on_delete=models.CASCADE)
-#     database = models.ForeignKey(Database, on_delete=models.CASCADE)
-
-
 class Snapshot(ReplicatedModel):
     """
     Represents a snapshot of a database at a given point in time.
     Used to efficiently bootstrap a database on a new device.
     """
 
     url = models.URLField()
```

### Comparing `fractal_database-0.0.8/fractal_database/replication/tasks.py` & `fractal_database-0.0.9/fractal_database/replication/tasks.py`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/representations.py` & `fractal_database-0.0.9/fractal_database/representations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from typing import TYPE_CHECKING, Dict
+import logging
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from fractal_database.models import ReplicatedModel, ReplicationTarget
 
+logger = logging.getLogger(__name__)
+
 
 def get_nested_attr(obj, attr_path):
     """
     Recursively get nested attributes of an object.
 
     :param obj: The object from which attributes are fetched.
     :param attr_path: String path of nested attributes separated by dots.
@@ -30,15 +33,15 @@
         target: "ReplicationTarget",
     ):
         """
         Create representation logs (tasks) for creating a Representation
         """
         from fractal_database.models import RepresentationLog
 
-        print("Creating representation log for", cls)
+        logger.info("Creating representation log for", cls)
         return [
             RepresentationLog.objects.create(
                 instance=instance,
                 method=cls.representation_module,
                 target=target,
                 metadata=instance.repr_metadata_props(),
             )
```

### Comparing `fractal_database-0.0.8/fractal_database/signals.py` & `fractal_database-0.0.9/fractal_database/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from django.conf import settings
 from django.db import transaction
 from django.db.models import F
 from fractal.matrix import MatrixClient
 from fractal_database.utils import get_project_name, init_poetry_project
 from taskiq_matrix.lock import MatrixLock
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("django")
+# logger = logging.getLogger(__name__)
 
 _thread_locals = threading.local()
 
 if TYPE_CHECKING:
     from fractal_database.models import (
         Database,
         Device,
@@ -30,15 +31,15 @@
     from fractal_database_matrix.models import (
         MatrixCredentials,
         MatrixReplicationTarget,
     )
 
 try:
     FRACTAL_EXPORT_DIR = settings.FRACTAL_EXPORT_DIR
-except:
+except AttributeError:
     FRACTAL_EXPORT_DIR = settings.BASE_DIR / "export"
 
 
 def enter_signal_handler():
     """Increments the counter indicating we've entered a new signal handler."""
     if not hasattr(_thread_locals, "signal_nesting_count"):
         _thread_locals.signal_nesting_count = 0
@@ -62,15 +63,15 @@
 
     Intended to be called by the transaction.on_commit handler registered
     by defer_replication.
     """
     # this runs its own thread so once this completes, we need to clear the deferred replications
     # for this target
     try:
-        print("Inside signals: commit")
+        logger.debug("Inside signals: commit")
         try:
             async_to_sync(target.replicate)()
         except Exception as e:
             logger.error(f"Error replicating {target}: {e}")
     finally:
         clear_deferred_replications(target.name)
 
@@ -160,21 +161,23 @@
                 registration_token=registration_token,
                 device_name=instance.display_name or instance.name,
             )
             return access_token, matrix_id, password
 
     access_token, matrix_id, password = async_to_sync(_register_device_account)()
 
-    MatrixCredentials.objects.create(
+    target = Database.current_db().primary_target()
+
+    creds = MatrixCredentials.objects.create(
         matrix_id=matrix_id,
         password=password,
         access_token=access_token,
-        target=Database.current_db().primary_target(),
         device=instance,
     )
+    creds.targets.add(target)
 
 
 def increment_version(sender, instance, **kwargs) -> None:
     """
     Increments the object version and updates the last_updated_by field to the
     configured owner in settings.py
     """
@@ -197,14 +200,15 @@
 
     if not transaction.get_connection().in_atomic_block:
         with transaction.atomic():
             return object_post_save(sender, instance, created, raw, **kwargs)
 
     logger.debug("in atomic block")
 
+    # TODO: Make this a context manager so we dont ever have to worry about forgetting to exit
     enter_signal_handler()
 
     increment_version(sender, instance)
 
     try:
         if in_nested_signal_handler():
             logger.info(f"Back inside post_save for instance: {instance}")
@@ -230,45 +234,48 @@
     **kwargs,
 ) -> None:
     """
     Calls schedule replication on the instance (and its reverse relations) whenever a many to many field is changed.
 
     Connected via fractal_database.apps.FractalDatabaseConfig.ready
     """
+    # ensure that the signal is called in a transaction
+    if not transaction.get_connection().in_atomic_block:
+        with transaction.atomic():
+            return schedule_replication_on_m2m_change(
+                sender, instance, action, reverse, model, pk_set, **kwargs
+            )
+
     if action not in {"post_add", "post_remove"}:
         return None
 
-    print(f"Inside schedule_replication_on_m2m_change: {instance}")
+    logger.debug(f"Inside schedule_replication_on_m2m_change: {instance}")
     for id in pk_set:
         if reverse:
             related_instance = model.objects.get(pk=id)
             instance.schedule_replication(created=False)
             related_instance.schedule_replication(created=False)
         else:
             related_instance = instance
-            related_instance.save()
-            # related_instance.schedule_replication(created=False)
+            related_instance.schedule_replication(created=False)
 
 
 def create_database_and_matrix_replication_target(*args, **kwargs) -> None:
     """
     Runs on post_migrate signal to setup the MatrixReplicationTarget for the
     Django project.
     """
     from fractal.cli.controllers.auth import AuthenticatedController
     from fractal_database.models import (
         Database,
         DatabaseConfig,
         Device,
         DummyReplicationTarget,
     )
-    from fractal_database_matrix.models import (
-        MatrixCredentials,
-        MatrixReplicationTarget,
-    )
+    from fractal_database_matrix.models import MatrixReplicationTarget
 
     if not transaction.get_connection().in_atomic_block:
         with transaction.atomic():
             return create_database_and_matrix_replication_target(*args, **kwargs)
 
     project_name = get_project_name()
     logger.info('Creating Fractal Database for Django project "%s"' % project_name)
@@ -295,30 +302,30 @@
             name="dummy",
             database=database,
             primary=False,
         )
 
     creds = AuthenticatedController.get_creds()
     if creds:
-        access_token, homeserver_url, owner_matrix_id = creds
+        _, homeserver_url, owner_matrix_id = creds
     else:
         if (
             not os.environ.get("MATRIX_HOMESERVER_URL")
             or not os.environ.get("MATRIX_ACCESS_TOKEN")
             or not os.environ.get("MATRIX_OWNER_MATRIX_ID")
         ):
             logger.info(
                 "MATRIX_HOMESERVER_URL and/or MATRIX_ACCESS_TOKEN not set, skipping MatrixReplicationTarget creation"
             )
             return
         # make sure the appropriate matrix env vars are set
         homeserver_url = os.environ["MATRIX_HOMESERVER_URL"]
         owner_matrix_id = os.environ["MATRIX_OWNER_MATRIX_ID"]
         # TODO move access_token to a non-replicated model
-        access_token = os.environ["MATRIX_ACCESS_TOKEN"]
+        _ = os.environ["MATRIX_ACCESS_TOKEN"]
 
     logger.info("Creating MatrixReplicationTarget for database %s" % database)
     target, created = MatrixReplicationTarget.objects.get_or_create(
         name="matrix",
         database=database,
         defaults={
             "name": "matrix",
@@ -339,17 +346,16 @@
             "display_name": device_name,
         },
     )
     current_db_config.update(current_device=device)
     database.devices.add(device)
 
     # replicate the database now that we have a replication target
-    print(f"Replicating after adding device to database")
+    logger.debug("Replicating after adding device to database")
     database.save()
-    # database.schedule_replication()
 
 
 async def _accept_invite(
     device_creds: "MatrixCredentials", database_room_id: str, homeserver_url: str
 ):
     device_matrix_id = device_creds.matrix_id
     # accept invite on behalf of device
@@ -396,34 +402,46 @@
 
     current_device = Device.current_device()
 
     for device_id in pk_set:
         # dont send an invite if the device is the current device
         # since the current device is invited in create_representation
         if device_id == current_device.pk:
+            logger.debug("Not sending invite to current device in database...")
             continue
 
         device = Device.objects.get(pk=device_id)
         primary_target = instance.primary_target()
 
         device_creds = device.matrixcredentials_set.filter(
             target__homeserver=primary_target.homeserver  # type: ignore
         ).get()
 
         async_to_sync(_invite_device)(
             device_creds,
             primary_target.metadata["room_id"],  # type: ignore
             primary_target.homeserver,  # type: ignore
         )
+        async_to_sync(_invite_device)(
+            device_creds,
+            primary_target.metadata["devices_room_id"],  # type: ignore
+            primary_target.homeserver,  # type: ignore
+        )
+
+        # accept invite on behalf of device
         async_to_sync(_accept_invite)(
             device_creds,
             primary_target.metadata["room_id"],  # type: ignore
             primary_target.homeserver,  # type: ignore
         )
-        # accept invite on behalf of device
+        async_to_sync(_accept_invite)(
+            device_creds,
+            primary_target.metadata["devices_room_id"],  # type: ignore
+            primary_target.homeserver,  # type: ignore
+        )
 
 
 async def _lock_and_put_state(
     repr_instance: "Representation",
     room_id: str,
     target: "MatrixReplicationTarget",
     state_type: str,
@@ -454,19 +472,20 @@
     from fractal_database.models import Database, RepresentationLog
     from fractal_database_matrix.models import MatrixReplicationTarget
 
     # dont do anything if loading from fixture or a new object is created
     if not isinstance(instance, (Database, MatrixReplicationTarget)) or raw or created:
         return None
 
-    logger.info("Updating target state for %s" % instance)
     # only update the state if the object is the primary target
     if isinstance(instance, MatrixReplicationTarget) and not instance.primary:
         return None
-    elif isinstance(instance, Database):
+    logger.info("Updating target state for %s" % instance)
+
+    if isinstance(instance, Database):
         target = instance.primary_target()
         if not target or not isinstance(target, MatrixReplicationTarget):
             logger.warning(
                 "Cannot update target state, no primary target found for database %s" % instance
             )
             return None
     else:
@@ -475,15 +494,15 @@
     room_id = target.metadata.get("room_id")
     if not room_id:
         logger.warning("Cannot update target state, no room_id found for target %s" % target)
         return None
 
     instance_fixture = instance.to_fixture(json=True)
     representation_module = target.get_representation_module()
-    print(f"Got representation module: {representation_module}")
+    logger.info(f"Got representation module: {representation_module}")
     repr_instance = RepresentationLog._get_repr_instance(representation_module)
     state_type = "f.database" if isinstance(instance, Database) else "f.database.target"
     # put state needs the matrix credentials for the target so accessing the creds here
     # ensures that the creds are loaded into memory (avoiding lazy loading issues in async)
     # target.matrixcredentials_set
 
     async_to_sync(_lock_and_put_state)(
@@ -589,7 +608,20 @@
         if not app_name.endswith(".tar.gz"):
             continue
         logger.info(f"Uploading {app_name} to {primary_target.homeserver}")
         async_to_sync(_upload_app)(room_id, app_name)
 
         # remove the app after uploading (maybe we keep this?)
         # os.remove(f"{FRACTAL_EXPORT_DIR}/{app_name}")
+
+
+def initialize_fractal_app_catalog(*args, **kwargs):
+    from fractal_database.models import AppCatalog
+
+    logger.info("Initializing fractal app catalog")
+    AppCatalog.objects.get_or_create(
+        name="fractal",
+        defaults={
+            "name": "fractal",
+            "git_url": "https://github.com/fractalnetworksco/FIXME",
+        },
+    )
```

### Comparing `fractal_database-0.0.8/fractal_database/templates/project_template/manage.py-tpl` & `fractal_database-0.0.9/fractal_database/templates/project_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/templates/project_template/project_name/settings.py-tpl` & `fractal_database-0.0.9/fractal_database/templates/project_template/project_name/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/templates/project_template/project_name/urls.py-tpl` & `fractal_database-0.0.9/fractal_database/templates/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/fractal_database/utils.py` & `fractal_database-0.0.9/fractal_database/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_database-0.0.8/PKG-INFO` & `fractal_database-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: fractal-database
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Mo Balaa
 Author-email: balaa@fractalnetworks.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: dev
 Requires-Dist: django (>=5.0.0)
 Requires-Dist: fractal-cli (>=0.0.1)
 Requires-Dist: fractal-database-matrix (>=0.0.1)
+Requires-Dist: ipython (>=8.17.2,<9.0.0) ; extra == "dev"
+Requires-Dist: pytest (>=7.4.3,<8.0.0) ; extra == "dev"
+Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "dev"
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "dev"
+Requires-Dist: pytest-django (>=4.5.2,<5.0.0) ; extra == "dev"
+Requires-Dist: pytest-mock (>=3.11.1,<4.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # Fractal Database
 
 Self-hosted Serverless Databases powered by Django.
```

