# Comparing `tmp/django-db-queue-3.0.0.tar.gz` & `tmp/django-db-queue-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-queue-3.0.0.tar", last modified: Thu Jan  6 21:16:21 2022, max compression
+gzip compressed data, was "django-db-queue-3.1.0.tar", last modified: Tue Apr  9 09:33:12 2024, max compression
```

## Comparing `django-db-queue-3.0.0.tar` & `django-db-queue-3.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.535464 django-db-queue-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/django_db_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-01-06 21:16:21.000000 django-db-queue-3.0.0/django_db_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-01-06 21:16:21.000000 django-db-queue-3.0.0/django_db_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 21:16:21.000000 django-db-queue-3.0.0/django_db_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-06 21:16:21.000000 django-db-queue-3.0.0/django_db_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-01-06 21:16:21.000000 django-db-queue-3.0.0/django_db_queue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/django_dbq/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/django_dbq/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/django_dbq/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/management/commands/delete_old_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/management/commands/queue_depth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4541 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/management/commands/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:21.531464 django-db-queue-3.0.0/django_dbq/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0002_auto_20151016_1027.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0003_auto_20180713_1000.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0004_auto_20210818_0247.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0005_job_run_after.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/0006_alter_job_state.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5256 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13541 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/django_dbq/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-06 21:16:21.535464 django-db-queue-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-01-06 21:16:13.000000 django-db-queue-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.557471 django-db-queue-3.1.0/django_db_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 09:33:12.000000 django-db-queue-3.1.0/django_db_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 09:33:12.000000 django-db-queue-3.1.0/django_db_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:33:12.000000 django-db-queue-3.1.0/django_db_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 09:33:12.000000 django-db-queue-3.1.0/django_db_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 09:33:12.000000 django-db-queue-3.1.0/django_db_queue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.557471 django-db-queue-3.1.0/django_dbq/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/django_dbq/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/django_dbq/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/management/commands/delete_old_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/management/commands/queue_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/management/commands/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/django_dbq/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0002_auto_20151016_1027.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0003_auto_20180713_1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0004_auto_20210818_0247.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0005_job_run_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/0006_alter_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/django_dbq/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:33:12.561471 django-db-queue-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 09:32:56.000000 django-db-queue-3.1.0/setup.py
```

### Comparing `django-db-queue-3.0.0/LICENSE` & `django-db-queue-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/README.md` & `django-db-queue-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,37 +3,41 @@
 [![pypi release](https://img.shields.io/pypi/v/django-db-queue.svg)](https://pypi.python.org/pypi/django-db-queue)
 
 Simple database-backed job queue. Jobs are defined in your settings, and are processed by management commands.
 
 Asynchronous tasks are run via a *job queue*. This system is designed to support multi-step job workflows.
 
 Supported and tested against:
-- Django 3.2 and 4.0
-- Python 3.6, 3.7, 3.8, 3.9 and 3.10
+- Django 3.2, 4.0, 4.1, 4.2, 5.0
+- Python 3.8, 3.9, 3.10, 3.11, 3.12
 
 ## Getting Started
 
 ### Installation
 
 Install from PIP
 
-    pip install django-db-queue
+```
+pip install django-db-queue
+```
 
 Add `django_dbq` to your installed apps
 
 ```python
 INSTALLED_APPS = [
     ...,
     "django_dbq",
 ]
 ```
 
 Run migrations
 
-    manage.py migrate
+```
+manage.py migrate
+```
 
 ### Upgrading from 1.x to 2.x
 
 Note that version 2.x only supports Django 3.1 or newer. If you need support for Django 2.2, please stick with the latest 1.x release.
 
 ### Describe your job
 
@@ -108,15 +112,17 @@
 }
 ```
 
 ### Start the worker
 
 In another terminal:
 
-`python manage.py worker`
+```
+python manage.py worker
+```
 
 ### Create a job
 
 Using the name you configured for your job in your settings, create an instance of Job.
 
 ```python
 Job.objects.create(name="my_job")
@@ -182,19 +188,21 @@
 ```python
 def my_task(job):
     cats_import = CatsImport.objects.get(pk=job.workspace["cats_import_id"])
 ```
 
 Tasks within a single job can use the workspace to communicate with each other. A single task can edit the workspace, and the modified workspace will be passed on to the next task in the sequence. For example:
 
-    def my_first_task(job):
-        job.workspace['message'] = 'Hello, task 2!'
+```python
+def my_first_task(job):
+    job.workspace['message'] = 'Hello, task 2!'
 
-    def my_second_task(job):
-        logger.info("Task 1 says: %s" % job.workspace['message'])
+def my_second_task(job):
+    logger.info("Task 1 says: %s" % job.workspace['message'])
+```
 
 The workspace can be queried like any [JSONField](https://docs.djangoproject.com/en/3.2/topics/db/queries/#querying-jsonfield). For instance, if you wanted to display a list of jobs that a certain user had initiated, add `user_id` to the workspace when creating the job:
 
 ```python
 Job.objects.create(name="foo", workspace={"user_id": request.user.id})
 ```
 
@@ -208,17 +216,19 @@
 
 A *worker process* is a long-running process, implemented as a Django management command, which is responsible for executing the tasks associated with a job. There may be many worker processes running concurrently in the final system. Worker processes wait for a new job to be created in the database, and call the each associated task in the correct sequeunce.. A worker can be started using `python manage.py worker`, and a single worker instance is included in the development `procfile`.
 
 ### Configuration
 
 Jobs are configured in the Django `settings.py` file. The `JOBS` setting is a dictionary mapping a *job name* (eg `import_cats`) to a *list* of one or more task function paths. For example:
 
-    JOBS = {
-        'import_cats': ['apps.cat_importer.import_cats.step_one', 'apps.cat_importer.import_cats.step_two'],
-    }
+```python
+JOBS = {
+    'import_cats': ['apps.cat_importer.import_cats.step_one', 'apps.cat_importer.import_cats.step_two'],
+}
+```
 
 ### Job states
 
 Jobs have a `state` field which can have one of the following values:
 
 * `NEW` (has been created, waiting for a worker process to run the next task)
 * `READY` (has run a task before, awaiting a worker process to run the next task)
@@ -253,21 +263,22 @@
 in the dict returned by this method.
 
 #### Management commands
 
 ##### manage.py delete_old_jobs
 There is a management command, `manage.py delete_old_jobs`, which deletes any
 jobs from the database which are in state `COMPLETE` or `FAILED` and were
-created more than 24 hours ago. This could be run, for example, as a cron task,
-to ensure the jobs table remains at a reasonable size.
+created more than (by default) 24 hours ago. This could be run, for example, as a cron task, to ensure the jobs table remains at a reasonable size. Use the `--hours` argument to control the age of jobs that will be deleted.
 
 ##### manage.py worker
 To start a worker:
 
-    manage.py worker [queue_name] [--rate_limit]
+```
+manage.py worker [queue_name] [--rate_limit]
+```
 
 - `queue_name` is optional, and will default to `default`
 - The `--rate_limit` flag is optional, and will default to `1`. It is the minimum number of seconds that must have elapsed before a subsequent job can be run.
 
 ##### manage.py queue_depth
 If you'd like to check your queue depth from the command line, you can run `manage.py queue_depth [queue_name [queue_name ...]]` and any
 jobs in the "NEW" or "READY" states will be returned.
```

### Comparing `django-db-queue-3.0.0/django_db_queue.egg-info/SOURCES.txt` & `django-db-queue-3.1.0/django_db_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/management/commands/queue_depth.py` & `django-db-queue-3.1.0/django_dbq/management/commands/queue_depth.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/management/commands/worker.py` & `django-db-queue-3.1.0/django_dbq/management/commands/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         if len(args) != 1:
             raise CommandError("Please supply a single queue job name")
 
         queue_name = options["queue_name"]
         rate_limit_in_seconds = options["rate_limit"]
 
         self.stdout.write(
-            'Starting job worker for queue "%s" with rate limit %s/s'
+            'Starting job worker for queue "%s" with rate limit of one job per %s second(s)'
             % (queue_name, rate_limit_in_seconds)
         )
 
         worker = Worker(queue_name, rate_limit_in_seconds)
 
         if options["dry_run"]:
             return
```

### Comparing `django-db-queue-3.0.0/django_dbq/migrations/0001_initial.py` & `django-db-queue-3.1.0/django_dbq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/migrations/0003_auto_20180713_1000.py` & `django-db-queue-3.1.0/django_dbq/migrations/0003_auto_20180713_1000.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/migrations/0004_auto_20210818_0247.py` & `django-db-queue-3.1.0/django_dbq/migrations/0004_auto_20210818_0247.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/migrations/0006_alter_job_state.py` & `django-db-queue-3.1.0/django_dbq/migrations/0006_alter_job_state.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/models.py` & `django-db-queue-3.1.0/django_dbq/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import uuid
 
 
 logger = logging.getLogger(__name__)
 
 
-DELETE_JOBS_AFTER_HOURS = 24
+DEFAULT_DELETE_JOBS_AFTER_HOURS = 24
 
 
 class JobManager(models.Manager):
     def get_ready_or_none(self, queue_name, max_retries=3):
         """
         Get a job in state READY or NEW for a given queue. Supports retrying in case of database deadlock
 
@@ -45,25 +45,25 @@
                 retries_left -= 1
                 logger.warn(
                     "Caught %s when looking for a READY job, retrying %s more times",
                     str(e),
                     retries_left,
                 )
 
-    def delete_old(self):
+    def delete_old(self, hours=None):
         """
-        Delete all jobs older than DELETE_JOBS_AFTER_HOURS
+        Delete all jobs older than hours, or DEFAULT_DELETE_JOBS_AFTER_HOURS
         """
         delete_jobs_in_states = [
             Job.STATES.FAILED,
             Job.STATES.COMPLETE,
             Job.STATES.STOPPING,
         ]
         delete_jobs_created_before = timezone.now() - datetime.timedelta(
-            hours=DELETE_JOBS_AFTER_HOURS
+            hours=hours or DEFAULT_DELETE_JOBS_AFTER_HOURS
         )
         logger.info(
             "Deleting all job in states %s created before %s",
             ", ".join(delete_jobs_in_states),
             delete_jobs_created_before.isoformat(),
         )
         Job.objects.filter(
```

### Comparing `django-db-queue-3.0.0/django_dbq/tasks.py` & `django-db-queue-3.1.0/django_dbq/tasks.py`

 * *Files identical despite different names*

### Comparing `django-db-queue-3.0.0/django_dbq/tests.py` & `django-db-queue-3.1.0/django_dbq/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 
 from django_dbq.management.commands.worker import Worker
 from django_dbq.models import Job
 
 from io import StringIO
 
 
+try:
+    utc = timezone.utc
+except AttributeError:
+    from datetime import timezone as datetime_timezone
+
+    utc = datetime_timezone.utc
+
+
 def test_task(job=None):
     pass  # pragma: no cover
 
 
 def workspace_test_task(job):
     input = job.workspace["input"]
     job.workspace["output"] = input + "-output"
@@ -185,15 +193,15 @@
 
     def test_get_next_ready_job(self):
         self.assertTrue(Job.objects.get_ready_or_none("default") is None)
 
         Job.objects.create(name="testjob", state=Job.STATES.READY)
         Job.objects.create(name="testjob", state=Job.STATES.PROCESSING)
         expected = Job.objects.create(name="testjob", state=Job.STATES.READY)
-        expected.created = datetime.now() - timedelta(minutes=1)
+        expected.created = timezone.now() - timedelta(minutes=1)
         expected.save()
 
         self.assertEqual(Job.objects.get_ready_or_none("default"), expected)
 
     def test_gets_jobs_in_priority_order(self):
         job_1 = Job.objects.create(name="testjob")
         job_2 = Job.objects.create(name="testjob", state=Job.STATES.PROCESSING)
@@ -227,15 +235,17 @@
             {job for job in Job.objects.to_process("default")}, {job_1, job_3, job_4}
         )
         self.assertEqual(Job.objects.get_ready_or_none("default"), job_1)
         self.assertFalse(Job.objects.to_process("default").filter(id=job_2.id).exists())
 
     def test_ignores_jobs_until_run_after_is_in_the_past(self):
         job_1 = Job.objects.create(name="testjob")
-        job_2 = Job.objects.create(name="testjob", run_after=datetime(2021, 11, 4, 8))
+        job_2 = Job.objects.create(
+            name="testjob", run_after=datetime(2021, 11, 4, 8, tzinfo=utc)
+        )
 
         with freezegun.freeze_time(datetime(2021, 11, 4, 7)):
             self.assertEqual(
                 {job for job in Job.objects.to_process("default")}, {job_1}
             )
 
         with freezegun.freeze_time(datetime(2021, 11, 4, 9)):
@@ -252,15 +262,15 @@
         query picks the .first())
         """
         self.assertTrue(Job.objects.get_ready_or_none("default") is None)
 
         Job.objects.create(name="testjob", state=Job.STATES.NEW)
         Job.objects.create(name="testjob", state=Job.STATES.PROCESSING)
         expected = Job.objects.create(name="testjob", state=Job.STATES.NEW)
-        expected.created = datetime.now() - timedelta(minutes=1)
+        expected.created = timezone.now() - timedelta(minutes=1)
         expected.save()
 
         self.assertEqual(Job.objects.get_ready_or_none("default"), expected)
 
 
 @override_settings(JOBS={"testjob": {"tasks": ["a", "b", "c"]}})
 class JobTaskTestCase(TestCase):
@@ -332,15 +342,15 @@
         self.assertEqual(job.state, Job.STATES.FAILED)
         self.assertEqual(job.workspace["output"], "failure hook ran")
 
 
 @override_settings(JOBS={"testjob": {"tasks": ["a"]}})
 class DeleteOldJobsTestCase(TestCase):
     def test_delete_old_jobs(self):
-        two_days_ago = datetime.utcnow() - timedelta(days=2)
+        two_days_ago = timezone.now() - timedelta(days=2)
 
         j1 = Job.objects.create(name="testjob", state=Job.STATES.COMPLETE)
         j1.created = two_days_ago
         j1.save()
 
         j2 = Job.objects.create(name="testjob", state=Job.STATES.FAILED)
         j2.created = two_days_ago
@@ -357,7 +367,21 @@
         j5 = Job.objects.create(name="testjob", state=Job.STATES.COMPLETE)
 
         Job.objects.delete_old()
 
         self.assertEqual(Job.objects.count(), 2)
         self.assertTrue(j4 in Job.objects.all())
         self.assertTrue(j5 in Job.objects.all())
+
+    def test_delete_old_jobs_with_custom_hours_argument(self):
+        j1 = Job.objects.create(name="testjob", state=Job.STATES.COMPLETE)
+        j1.created = timezone.now() - timedelta(days=5)
+        j1.save()
+
+        j2 = Job.objects.create(name="testjob", state=Job.STATES.COMPLETE)
+        j2.created = timezone.now() - timedelta(days=3)
+        j2.save()
+
+        Job.objects.delete_old(hours=24 * 4)
+
+        self.assertEqual(Job.objects.count(), 1)
+        self.assertTrue(j2 in Job.objects.all())
```

### Comparing `django-db-queue-3.0.0/setup.py` & `django-db-queue-3.1.0/setup.py`

 * *Files identical despite different names*

