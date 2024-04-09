# Comparing `tmp/edx_event_bus_kafka-5.6.0.tar.gz` & `tmp/edx_event_bus_kafka-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_kafka-5.6.0.tar", last modified: Thu Jan 25 16:32:49 2024, max compression
+gzip compressed data, was "edx_event_bus_kafka-5.7.0.tar", last modified: Tue Apr  9 09:30:41 2024, max compression
```

## Comparing `edx_event_bus_kafka-5.6.0.tar` & `edx_event_bus_kafka-5.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20843 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.301500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32108 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    31455 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19282 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.301500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20843 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 16:32:49.000000 edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-25 16:32:49.309500 edx_event_bus_kafka-5.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5009 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:32:49.305500 edx_event_bus_kafka-5.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-25 16:32:46.000000 edx_event_bus_kafka-5.6.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.621473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.621473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32016 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31455 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19282 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.617473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 09:30:41.000000 edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5059 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:30:41.625473 edx_event_bus_kafka-5.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 09:30:36.000000 edx_event_bus_kafka-5.7.0/tests/test_models.py
```

### Comparing `edx_event_bus_kafka-5.6.0/CHANGELOG.rst` & `edx_event_bus_kafka-5.7.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.7.0] - 2024-03-22
+********************
+Changed
+=======
+* Dropped Support for Django 3.2, Django 4.0 and Django 4.1
+* Added Support for Python 3.12
+
 [5.6.0] - 2024-01-25
 ********************
 Changed
 =======
 * Added client.id to base configuration.
 
 [5.5.0] - 2023-09-21
```

### Comparing `edx_event_bus_kafka-5.6.0/LICENSE.txt` & `edx_event_bus_kafka-5.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/PKG-INFO` & `edx_event_bus_kafka-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 5.6.0
+Version: 5.7.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Django
 Requires-Dist: edx_django_utils
 Requires-Dist: edx_toggles
 Requires-Dist: openedx-events>=9.3.0
 
@@ -208,14 +209,21 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.7.0] - 2024-03-22
+********************
+Changed
+=======
+* Dropped Support for Django 3.2, Django 4.0 and Django 4.1
+* Added Support for Python 3.12
+
 [5.6.0] - 2024-01-25
 ********************
 Changed
 =======
 * Added client.id to base configuration.
 
 [5.5.0] - 2023-09-21
```

### Comparing `edx_event_bus_kafka-5.6.0/README.rst` & `edx_event_bus_kafka-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/config.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/consumer.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 
                             signal = self.determine_signal(msg)
                             msg.set_value(self._deserialize_message_value(msg, signal))
                             self.emit_signals_from_message(msg, signal)
                             consecutive_errors = 0
 
                     self._add_message_monitoring(run_context=run_context, message=msg)
-                except Exception as e:  # pylint: disable=broad-except
+                except Exception as e:
                     consecutive_errors += 1
                     self.record_event_consuming_error(run_context, e, msg)
                     # Kill the infinite loop if the error is fatal for the consumer
                     _, kafka_error = self._get_kafka_message_and_error(message=msg, error=e)
                     if kafka_error and kafka_error.fatal():
                         raise e
                     # Prevent fast error-looping when no event received from broker. Because
@@ -511,15 +511,15 @@
 
             # See ADR for details on why certain fields were included or omitted.
             logger.info(
                 f'Message received from Kafka: topic={msg.topic()}, partition={msg.partition()}, '
                 f'offset={msg.offset()}, message_id={message_id}, key={msg.key()}, '
                 f'event_timestamp_ms={timestamp_info}'
             )
-        except Exception as e:  # pragma: no cover  pylint: disable=broad-except
+        except Exception as e:  # pragma: no cover
             # Use this to fix any bugs in what should be benign logging code
             set_custom_attribute('kafka_logging_error', repr(e))
 
     def record_event_consuming_error(self, run_context, error, maybe_message):
         """
         Record an error caught while consuming an event, both to the logs and to telemetry.
 
@@ -599,15 +599,15 @@
                 # .. custom_attribute_name: kafka_error_fatal
                 # .. custom_attribute_description: Boolean describing if the error is fatal.
                 set_custom_attribute('kafka_error_fatal', kafka_error.fatal())
                 # .. custom_attribute_name: kafka_error_retriable
                 # .. custom_attribute_description: Boolean describing if the error is retriable.
                 set_custom_attribute('kafka_error_retriable', kafka_error.retriable())
 
-        except Exception as e:  # pragma: no cover  pylint: disable=broad-except
+        except Exception as e:  # pragma: no cover
             # Use this to fix any bugs in what should be benign monitoring code
             set_custom_attribute('kafka_monitoring_error', repr(e))
 
     def _get_kafka_message_and_error(self, message, error):
         """
         Returns tuple of (kafka_message, kafka_error), if they can be found.
```

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/producer.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             # Opportunistically ensure any pending callbacks from recent event-sends are triggered.
             # This ensures that we're polling at least as often as we're producing, which is a
             # reasonable balance. However, if events are infrequent, it doesn't ensure that
             # callbacks happen in a timely fashion, and the last event emitted before shutdown
             # would never get a delivery callback. That's why there's also a thread calling
             # poll(0) on a regular interval (see `poll_indefinitely`).
             self.producer.poll(0)
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:
             # Errors caused by the produce call should be handled by the on_delivery callback.
             # Here we might expect serialization errors, or any errors from preparing to produce.
             record_producing_error(e, context)
 
     def prepare_for_shutdown(self):
         """
         Prepare producer for a clean shutdown.
```

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_config.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_consumer.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_producer.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/tests/test_utils.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/internal/utils.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/management/commands/produce_event.py` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/management/commands/produce_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,9 +60,9 @@
                 signal=signal,
                 topic=options['topic'][0],
                 event_key_field=options['key_field'][0],
                 event_data=json.loads(options['data'][0]),
                 event_metadata=EventsMetadata(event_type=event_type),
             )
             producer.prepare_for_shutdown()  # otherwise command may exit before delivery is complete
-        except Exception:  # pylint: disable=broad-except
+        except Exception:
             logger.exception("Error producing Kafka event")
```

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/PKG-INFO` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 5.6.0
+Version: 5.7.0
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Django
 Requires-Dist: edx_django_utils
 Requires-Dist: edx_toggles
 Requires-Dist: openedx-events>=9.3.0
 
@@ -208,14 +209,21 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[5.7.0] - 2024-03-22
+********************
+Changed
+=======
+* Dropped Support for Django 3.2, Django 4.0 and Django 4.1
+* Added Support for Python 3.12
+
 [5.6.0] - 2024-01-25
 ********************
 Changed
 =======
 * Added client.id to base configuration.
 
 [5.5.0] - 2023-09-21
```

### Comparing `edx_event_bus_kafka-5.6.0/edx_event_bus_kafka.egg-info/SOURCES.txt` & `edx_event_bus_kafka-5.7.0/edx_event_bus_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-5.6.0/setup.py` & `edx_event_bus_kafka-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
     python_requires=">=3.8",
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Python edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

