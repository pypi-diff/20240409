# Comparing `tmp/giant-events-0.2.9.tar.gz` & `tmp/giant_events-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant-events-0.2.9.tar", max compression
+gzip compressed data, was "giant_events-0.3.0.1.tar", max compression
```

## Comparing `giant-events-0.2.9.tar` & `giant_events-0.3.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2022-09-12 12:29:23.637350 giant-events-0.2.9/LICENSE
--rw-r--r--   0        0        0     2778 2022-11-24 06:07:25.847541 giant-events-0.2.9/README.md
--rw-r--r--   0        0        0       22 2022-09-12 12:29:23.637350 giant-events-0.2.9/giant_events/__init__.py
--rw-r--r--   0        0        0     2642 2023-02-05 13:22:48.149531 giant-events-0.2.9/giant_events/admin.py
--rw-r--r--   0        0        0       93 2023-02-05 16:19:22.457240 giant-events-0.2.9/giant_events/apps.py
--rw-r--r--   0        0        0      390 2023-02-06 08:25:32.157147 giant-events-0.2.9/giant_events/cms_apps.py
--rw-r--r--   0        0        0     5508 2022-09-12 12:29:23.637350 giant-events-0.2.9/giant_events/migrations/0001_initial.py
--rw-r--r--   0        0        0     1065 2022-09-12 12:29:23.637350 giant-events-0.2.9/giant_events/migrations/0002_add_climatecare_fields.py
--rw-r--r--   0        0        0      704 2022-09-12 12:29:23.637350 giant-events-0.2.9/giant_events/migrations/0003_make_fields_optional.py
--rw-r--r--   0        0        0      860 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/migrations/0004_auto_20220509_0816.py
--rw-r--r--   0        0        0        0 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/migrations/__init__.py
--rw-r--r--   0        0        0     3413 2023-02-05 13:00:44.232067 giant-events-0.2.9/giant_events/models.py
--rw-r--r--   0        0        0      324 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/sitemaps.py
--rw-r--r--   0        0        0        0 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/templates/base.html
--rw-r--r--   0        0        0      285 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/templates/events/detail.html
--rw-r--r--   0        0        0     1182 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/templates/events/index.html
--rw-r--r--   0        0        0        0 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/tests/__init__.py
--rw-r--r--   0        0        0      705 2023-02-05 16:23:30.940014 giant-events-0.2.9/giant_events/tests/conftest.py
--rw-r--r--   0        0        0      285 2023-02-05 16:23:30.928014 giant-events-0.2.9/giant_events/tests/test_cms_apps.py
--rw-r--r--   0        0        0     2607 2023-02-05 16:23:08.268126 giant-events-0.2.9/giant_events/tests/test_models.py
--rw-r--r--   0        0        0     1857 2023-02-05 16:19:22.453240 giant-events-0.2.9/giant_events/tests/test_views.py
--rw-r--r--   0        0        0      150 2022-09-12 12:29:23.641350 giant-events-0.2.9/giant_events/tests/urls.py
--rw-r--r--   0        0        0      233 2023-02-05 16:21:57.400475 giant-events-0.2.9/giant_events/urls.py
--rw-r--r--   0        0        0     1364 2023-02-05 16:22:36.900280 giant-events-0.2.9/giant_events/views.py
--rw-r--r--   0        0        0     1092 2023-02-06 08:26:00.792646 giant-events-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3674 2023-02-06 08:26:08.188600 giant-events-0.2.9/setup.py
--rw-r--r--   0        0        0     3799 2023-02-06 08:26:08.188830 giant-events-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/LICENSE
+-rw-r--r--   0        0        0     3023 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/__init__.py
+-rw-r--r--   0        0        0     2774 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/admin.py
+-rw-r--r--   0        0        0       87 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/apps.py
+-rw-r--r--   0        0        0      378 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/cms_apps.py
+-rw-r--r--   0        0        0     5508 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1065 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0002_add_climatecare_fields.py
+-rw-r--r--   0        0        0      704 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0003_make_fields_optional.py
+-rw-r--r--   0        0        0     1034 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/migrations/0004_auto_20220509_0816.py
+-rw-r--r--   0        0        0      861 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/migrations/0005_event_hero_image.py
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/__init__.py
+-rw-r--r--   0        0        0     3871 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/models.py
+-rw-r--r--   0        0        0      324 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/sitemaps.py
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/templates/base.html
+-rw-r--r--   0        0        0      285 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/templates/events/detail.html
+-rw-r--r--   0        0        0     1183 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/templates/events/index.html
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/tests/__init__.py
+-rw-r--r--   0        0        0      699 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/conftest.py
+-rw-r--r--   0        0        0      279 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/test_cms_apps.py
+-rw-r--r--   0        0        0     2601 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/test_models.py
+-rw-r--r--   0        0        0     3222 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/tests/test_views.py
+-rw-r--r--   0        0        0      150 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/urls.py
+-rw-r--r--   0        0        0      227 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/urls.py
+-rw-r--r--   0        0        0     2038 2024-04-09 08:53:51.255891 giant_events-0.3.0.1/events/views.py
+-rw-r--r--   0        0        0     1069 2024-04-09 12:53:13.974602 giant_events-0.3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 giant_events-0.3.0.1/PKG-INFO
```

### Comparing `giant-events-0.2.9/LICENSE` & `giant_events-0.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giant-events-0.2.9/README.md` & `giant_events-0.3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 This application exposes the following settings:
 
 - `EVENT_ADMIN_LIST_DISPLAY` is the field list for the admin index. This must be a list
 - `EVENT_ADMIN_FIELDSETS` allows the user to define the admin fieldset. This must be a list of two-tuples
 - `EVENT_ADMIN_READONLY_FIELDS` allows the user to configure readonly fields in the admin. This must be a list
 - `EVENT_ADMIN_SEARCH_FIELDS` allows the user to configure search fields in the admin. This must be a list
 - `EVENT_ADMIN_FILTER_FIELDS` allows the user to configure filter fields in the admin. This must be a list
+- `PAGINATE_EVENTS_BY` allows user to determine how many events to paginate by on the index page. Applies to time directed queryset. This must be an int
+- `DEFAULT_TIME_DIRECTION` chose from one of the following options - PAST, FUTURE & ANYTIME
 
 By default the app will use the templates that are defined inside the app directory itself. However if you wish to override which template is used you will need to create a directory in the projects template directory
 The structure should look something like this:
 
 ```
 templates/
     events/
```

### Comparing `giant-events-0.2.9/giant_events/admin.py` & `giant_events-0.3.0.1/events/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from django.contrib import admin
 from django.conf import settings
 
+from .models import Event, Tag, Location
 
+
+@admin.register(Tag)
 class TagAdmin(admin.ModelAdmin):
     """
     Admin config for EventTag model
     """
 
     list_display = ["name"]
 
     fields = ["name", "slug"]
     prepopulated_fields = {"slug": ["name"]}
 
 
+@admin.register(Event)
 class EventAdmin(admin.ModelAdmin):
     """
     Admin config for Event model
     """
 
     list_display = ["title", "start_at", "end_at", "is_published"]
-    search_fields = ["title", "location"]
+    search_fields = ["title", "location__name"]
     readonly_fields = ["created_at", "updated_at"]
     list_filter = ["is_published"]
     prepopulated_fields = {"slug": ["title"]}
 
     fieldsets = [
         (
             "Details",
@@ -36,15 +40,15 @@
                     "end_at",
                     "address",
                     "location",
                     "tags",
                 ]
             },
         ),
-        ("Image", {"fields": ["photo"]}),
+        ("Image", {"fields": ["photo", "hero_image"]}),
         ("Publishing", {"fields": ["is_published", "publish_at"]}),
         (
             "Metadata",
             {"classes": ("collapse",), "fields": ["created_at", "updated_at"]},
         ),
     ]
 
@@ -70,14 +74,15 @@
 
     def get_list_filter(self, request):
         if hasattr(settings, "EVENT_ADMIN_FILTER_FIELDS"):
             return settings.EVENT_ADMIN_FILTER_FIELDS
         return super().get_list_filter(request)
 
 
+@admin.register(Location)
 class LocationAdmin(admin.ModelAdmin):
     """
     Admin class for the location model
     """
 
     list_display = ["name", "lat", "lng"]
     readonly_fields = ["created_at", "updated_at"]
```

### Comparing `giant-events-0.2.9/giant_events/migrations/0001_initial.py` & `giant_events-0.3.0.1/events/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-events-0.2.9/giant_events/migrations/0002_add_climatecare_fields.py` & `giant_events-0.3.0.1/events/migrations/0002_add_climatecare_fields.py`

 * *Files identical despite different names*

### Comparing `giant-events-0.2.9/giant_events/migrations/0003_make_fields_optional.py` & `giant_events-0.3.0.1/events/migrations/0003_make_fields_optional.py`

 * *Files identical despite different names*

### Comparing `giant-events-0.2.9/giant_events/migrations/0004_auto_20220509_0816.py` & `giant_events-0.3.0.1/events/migrations/0005_event_hero_image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-# Generated by Django 2.2 on 2022-05-09 08:16
+# Generated by Django 2.2 on 2023-01-30 07:43
 
+from django.conf import settings
 from django.db import migrations
 import django.db.models.deletion
-import filer.fields.file
+import filer.fields.image
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('filer', '0015_alter_file_owner_alter_file_polymorphic_ctype_and_more'),
-        ('events', '0003_make_fields_optional'),
+        migrations.swappable_dependency(settings.FILER_IMAGE_MODEL),
+        ("events", "0004_auto_20220509_0816"),
     ]
 
     operations = [
-        migrations.AlterModelOptions(
-            name='event',
-            options={'ordering': ['start_at__date', 'start_at__time'], 'verbose_name': 'Event', 'verbose_name_plural': 'Events'},
-        ),
         migrations.AddField(
-            model_name='event',
-            name='file',
-            field=filer.fields.file.FilerFileField(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='events_event_files', to='filer.File', verbose_name='File'),
+            model_name="event",
+            name="hero_image",
+            field=filer.fields.image.FilerImageField(
+                blank=True,
+                help_text="Select an image that will be displayed as the hero for the event detail page. ",
+                null=True,
+                on_delete=django.db.models.deletion.SET_NULL,
+                related_name="+",
+                to=settings.FILER_IMAGE_MODEL,
+            ),
         ),
     ]
```

### Comparing `giant-events-0.2.9/giant_events/models.py` & `giant_events-0.3.0.1/events/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
     class Meta:
         verbose_name = "Location"
         verbose_name_plural = "Locations"
         ordering = ["name"]
 
     def __str__(self):
+        """
+        String representation of the location object, in the Events app
+        """
         return self.name
 
 
 class EventQuerySet(PublishingQuerySetMixin):
     """
     Custom QuerySet model to override the base one
     """
@@ -68,15 +71,15 @@
     def past(self, user=None):
         """
         Return the published queryset for past events.
         """
         return self.published(user=user).filter(end_at__lt=timezone.now())
 
 
-class AbstractEvent(TimestampMixin, PublishingMixin, URLMixin):
+class Event(TimestampMixin, PublishingMixin, URLMixin):
     """
     Model for creating and storing and event object
     """
 
     title = models.CharField(max_length=255)
     slug = models.SlugField(max_length=255, unique=True)
     photo = FilerImageField(
@@ -84,14 +87,21 @@
         on_delete=models.SET_NULL,
         null=True,
     )
     start_at = models.DateTimeField()
     end_at = models.DateTimeField(blank=True, null=True)
     intro = models.CharField(max_length=255)
     content = PlaceholderField(slotname="event_content", related_name="event_content")
+    hero_image = FilerImageField(
+        related_name="+",
+        help_text="Select an image that will be displayed as the hero for the event detail page. ",
+        blank=True,
+        null=True,
+        on_delete=models.SET_NULL,
+    )
     tags = models.ManyToManyField(
         to=Tag,
         verbose_name="Tags",
         related_name="%(app_label)s_%(class)s_tags",
         blank=True,
     )
     address = models.CharField(max_length=255, blank=True)
@@ -101,17 +111,22 @@
     cta_text = models.CharField(max_length=255, blank=True)
 
     objects = EventQuerySet.as_manager()
 
     class Meta:
         # We need both orders to make sure that hours are respected. Purely using the start_at
         # would not correctly sort 2 items with the same date but different hours.
-        abstract = True
         ordering = ["start_at__date", "start_at__time"]
         verbose_name = "Event"
         verbose_name_plural = "Events"
 
     def __str__(self):
+        """
+        Returns the string representation of the event object
+        """
         return self.title
 
     def get_absolute_url(self):
+        """
+        Builds the url for the event object
+        """
         return reverse("events:detail", kwargs={"slug": self.slug})
```

### Comparing `giant-events-0.2.9/giant_events/templates/events/index.html` & `giant_events-0.3.0.1/events/templates/events/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,10 @@
                         </div>
                     </div>
                 </a>
             {% empty %}
                 <h3>No events currently listed</h3>
             {% endfor %}
         </div>
+
     </section>
 {% endblock body %}
```

### Comparing `giant-events-0.2.9/giant_events/tests/conftest.py` & `giant_events-0.3.0.1/events/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.utils import timezone
 
 import pytest
 
-from giant_events.models import Event
+from events.models import Event
 
 
 @pytest.fixture
 def unpublished_event():
     _date = timezone.now() - timezone.timedelta(days=1)
     return Event.objects.create(
         title="Event One",
```

### Comparing `giant-events-0.2.9/giant_events/tests/test_models.py` & `giant_events-0.3.0.1/events/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from giant_events.models import Event, Tag
+from events.models import Event, Tag
 
 from .conftest import *
 
 
 class TestTag:
     """
     Test case for the EventTag model
```

### Comparing `giant-events-0.2.9/giant_events/tests/test_views.py` & `giant_events-0.3.0.1/events/tests/test_views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,105 @@
 from django.test import Client
 from django.urls import reverse
-from django.utils import timezone
 
 import pytest
-from giant_events import models
+from events import models
+from events.views import EventIndex
 
 from .conftest import *
 
 
 @pytest.mark.django_db
 class TestEventView:
     """
     Test case for the Event app views
     """
 
     @pytest.fixture
-    def event_instance(self):
+    def future_event_instance(self):
         return models.Event.objects.create(
-            title="Event",
-            slug="event",
-            start_at=timezone.now(),
+            title="Future Event",
+            slug="future-event",
+            start_at=timezone.now() + timezone.timedelta(days=1),
             is_published=True,
             publish_at=timezone.now() - timezone.timedelta(hours=1),
         )
 
-    def test_event_detail(self, event_instance):
+    @pytest.fixture
+    def past_event_instance(self):
+        return models.Event.objects.create(
+            title="Past Event",
+            slug="past-event",
+            start_at=timezone.now() - timezone.timedelta(days=1),
+            is_published=True,
+            publish_at=timezone.now() - timezone.timedelta(hours=1),
+        )
+
+    def test_event_detail(self, future_event_instance):
         """
         Test the detail view returns the correct status code
         """
 
         client = Client()
-        event = event_instance
-        response = client.get(reverse("giant_events:detail", kwargs={"slug": event.slug}))
+        event = future_event_instance
+        response = client.get(reverse("events:detail", kwargs={"slug": event.slug}))
         assert response.status_code == 200
 
     def test_event_index(self):
         """
         Test the index view returns the correct status code
         """
         client = Client()
-        response = client.get(reverse("giant_events:index"))
+        response = client.get(reverse("events:index"))
         assert response.status_code == 200
 
     def test_unpublished_returns_404(self, unpublished_event):
         """
         Test to check that an unpublished event returns a 404
         """
         client = Client()
         response = client.get(
-            reverse("giant_events:detail", kwargs={"slug": unpublished_event.slug})
+            reverse("events:detail", kwargs={"slug": unpublished_event.slug})
         )
 
         assert response.status_code == 404
 
-    def test_update_context(self, event_instance):
+    def test_update_context(self, future_event_instance):
         """
         Test the context update returns published events queryset
         """
         client = Client()
-        event = event_instance
-        response = client.get(reverse("giant_events:index"))
+        event = future_event_instance
+        response = client.get(reverse("events:index"))
 
         assert event in response.context["object_list"]
         assert event in models.Event.objects.published()
+
+    def test_time_direction(self, client):
+        """
+        Test the context update returns published events queryset
+        """
+
+        url = f"{reverse('events:index')}?{EventIndex.TimeDirection.PAST}"
+        response = client.get(url)
+
+        event_index = EventIndex()
+        event_index.request = response.wsgi_request
+
+        assert event_index.time_direction == EventIndex.TimeDirection.PAST
+
+    def test_get_queryset(self, client, future_event_instance, past_event_instance):
+        """
+        Test the context update returns published events queryset
+        """
+
+        url = f"{reverse('events:index')}?{EventIndex.TimeDirection.FUTURE}"
+        response = client.get(url)
+
+        event_index = EventIndex()
+        event_index.request = response.wsgi_request
+
+        event_queryset = event_index.get_queryset()
+        assert (
+            future_event_instance in event_queryset
+            and past_event_instance not in event_queryset
+        )
```

### Comparing `giant-events-0.2.9/pyproject.toml` & `giant_events-0.3.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-events"
-version = "0.2.9"
+version = "0.3.0.1"
 description = "A small reusable package that adds an Events app to a project"
 authors = ["Will-Hoey <will.hoey@giantmade.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-events"
 repository = "https://github.com/giantmade/giant-events"
 keywords = ["events", "app"]
@@ -15,22 +15,21 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 include = [
     "LICENSE",
 ]
 packages = [
-    { include = "giant_events" }
+    { include = "events" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 giant-mixins = "*"
 django-filer = "*"
-swapper = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "~7"
 django = "~3"
 django-cms = "~3"
 black = "~22"
 pytest-django = "~3"
```

### Comparing `giant-events-0.2.9/PKG-INFO` & `giant_events-0.3.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: giant-events
-Version: 0.2.9
+Version: 0.3.0.1
 Summary: A small reusable package that adds an Events app to a project
 Home-page: https://github.com/giantmade/giant-events
 License: MIT
 Keywords: events,app
 Author: Will-Hoey
 Author-email: will.hoey@giantmade.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django-filer
 Requires-Dist: giant-mixins
-Requires-Dist: swapper (>=1.3.0,<2.0.0)
 Project-URL: Repository, https://github.com/giantmade/giant-events
 Description-Content-Type: text/markdown
 
 # Giant Events
 
 A re-usable package which can be used in any project that requires a generic `Events` app. 
 
@@ -44,14 +44,16 @@
 This application exposes the following settings:
 
 - `EVENT_ADMIN_LIST_DISPLAY` is the field list for the admin index. This must be a list
 - `EVENT_ADMIN_FIELDSETS` allows the user to define the admin fieldset. This must be a list of two-tuples
 - `EVENT_ADMIN_READONLY_FIELDS` allows the user to configure readonly fields in the admin. This must be a list
 - `EVENT_ADMIN_SEARCH_FIELDS` allows the user to configure search fields in the admin. This must be a list
 - `EVENT_ADMIN_FILTER_FIELDS` allows the user to configure filter fields in the admin. This must be a list
+- `PAGINATE_EVENTS_BY` allows user to determine how many events to paginate by on the index page. Applies to time directed queryset. This must be an int
+- `DEFAULT_TIME_DIRECTION` chose from one of the following options - PAST, FUTURE & ANYTIME
 
 By default the app will use the templates that are defined inside the app directory itself. However if you wish to override which template is used you will need to create a directory in the projects template directory
 The structure should look something like this:
 
 ```
 templates/
     events/
```

