# Comparing `tmp/colcon-core-0.8.3.tar.gz` & `tmp/colcon-core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colcon-core-0.8.3.tar", last modified: Wed May  4 02:31:22 2022, max compression
+gzip compressed data, was "colcon-core-0.9.0.tar", last modified: Thu Jun 23 21:30:57 2022, max compression
```

## Comparing `colcon-core-0.8.3.tar` & `colcon-core-0.9.0.tar`

### file list

```diff
@@ -1,161 +1,164 @@
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/test/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1734 2022-04-25 17:51:53.000000 colcon-core-0.8.3/test/test_environment_pythonscriptspath.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2795 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_discovery_path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7165 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_identification.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      842 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_handler_log_command.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1004 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_argument_default.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7249 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_augmentation.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1785 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_decorator.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5575 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_verb.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5908 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_plugin_system.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1576 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_environment_path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4231 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_prefix_path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2319 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_topological_order.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1893 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_spell_check.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3377 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_shell_template_prefix_util.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1938 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_command.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19638 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_shell.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5431 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_entry_point.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3412 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_build_python.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4377 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_environment.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3478 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_shell_bat.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1085 2022-04-25 17:51:53.000000 colcon-core-0.8.3/test/test_environment_pythonpath.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4206 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_handler.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      737 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_dependency_descriptor.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9209 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_task.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8891 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_location.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4054 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_descriptor.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1823 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_logging.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5950 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_identification_python.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4635 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_argument_parser.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1752 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_flake8.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1393 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_copyright_license.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1353 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_handler_console_direct.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8536 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_executor.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3028 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_subprocess.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4154 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_reactor.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1642 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_task_python_test_pytest.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9298 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_discovery.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3520 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_shell_sh.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4405 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_executor_sequential.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2092 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_event_handler_console_start_end.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7722 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_selection.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3380 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_type_collector.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      818 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_package_identification_ignore.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1322 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_destination_collector.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2124 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_shell_template.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4753 2022-04-12 00:39:53.000000 colcon-core-0.8.3/test/test_command.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      262 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon/__main__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        0 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2245 2022-04-12 00:39:53.000000 colcon-core-0.8.3/setup.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1415 2022-05-04 02:31:22.000000 colcon-core-0.8.3/PKG-INFO
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5906 2022-05-04 02:31:22.000000 colcon-core-0.8.3/setup.cfg
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      364 2022-04-12 00:39:53.000000 colcon-core-0.8.3/README.rst
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4683 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/SOURCES.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2022-05-03 17:25:29.000000 colcon-core-0.8.3/colcon_core.egg-info/not-zip-safe
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3734 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/entry_points.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1415 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/PKG-INFO
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      348 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/requires.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       19 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/top_level.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core.egg-info/dependency_links.txt
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/prefix_path/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1306 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/prefix_path/colcon.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2996 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/prefix_path/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1771 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_decorator.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/event_handler/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1501 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event_handler/console_direct.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1011 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event_handler/log_command.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2260 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event_handler/console_start_end.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5395 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event_handler/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6453 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/entry_point.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/pytest/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      773 2022-05-04 02:31:10.000000 colcon-core-0.8.3/colcon_core/pytest/hooks.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        0 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/pytest/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1421 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/dependency_descriptor.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      207 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/environment_variable.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/package_discovery/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2449 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_discovery/path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9675 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_discovery/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      824 2022-05-04 02:31:10.000000 colcon-core-0.8.3/colcon_core/python_install_path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4289 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/logging.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/verb/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9063 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/verb/build.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8570 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/verb/test.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6479 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/verb/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6532 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/plugin_system.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4643 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event_reactor.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/package_identification/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      939 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_identification/ignore.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5363 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_identification/python.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6389 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_identification/__init__.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/shell/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/shell/template/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      757 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/package.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3897 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       21 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_set_value.dsv.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      247 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/command_prefix.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       26 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_append_value.dsv.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4377 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    15137 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix_util.py.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      264 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/command_prefix.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      102 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_set_value.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       26 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_prepend_value.dsv.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2011 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix_chain.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       92 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_set_value.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2833 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/package.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4746 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix_util.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1279 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_prepend_value.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      877 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/prefix_chain.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       68 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/package.dsv.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      291 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_prepend_value.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3077 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1584 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_append_value.bat.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1872 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/template/hook_append_value.sh.em
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6144 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/bat.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2172 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/installed_packages.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6269 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/sh.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2907 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/dsv.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    24044 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/shell/__init__.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/argument_parser/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3018 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/argument_parser/type_collector.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1871 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/argument_parser/destination_collector.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9044 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/argument_parser/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10254 2022-05-03 17:22:09.000000 colcon-core-0.8.3/colcon_core/subprocess.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/package_selection/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8428 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_selection/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2046 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/argument_default.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/environment/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1964 2022-04-25 17:51:53.000000 colcon-core-0.8.3/colcon_core/environment/path.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1158 2022-04-25 17:51:53.000000 colcon-core-0.8.3/colcon_core/environment/pythonpath.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6553 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/environment/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3062 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/topological_order.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/package_augmentation/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6044 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_augmentation/python.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8166 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_augmentation/__init__.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/executor/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4017 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/executor/sequential.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    12986 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/executor/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5418 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/package_descriptor.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/event/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      396 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/test.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2251 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/job.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      181 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/timer.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      335 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3723 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/command.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      747 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/event/output.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/task/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/task/python/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-05-04 02:31:22.000000 colcon-core-0.8.3/colcon_core/task/python/test/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7395 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/task/python/test/pytest.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1946 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/task/python/test/setuppy_test.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8123 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/task/python/test/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    13258 2022-05-04 02:31:10.000000 colcon-core-0.8.3/colcon_core/task/python/build.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1535 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/task/python/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10112 2022-05-03 17:22:09.000000 colcon-core-0.8.3/colcon_core/task/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      106 2022-05-04 02:31:10.000000 colcon-core-0.8.3/colcon_core/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19593 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/command.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7603 2022-04-12 00:39:53.000000 colcon-core-0.8.3/colcon_core/location.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.111437 colcon-core-0.9.0/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1415 2022-06-23 21:30:57.111437 colcon-core-0.9.0/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      364 2022-06-23 21:24:45.000000 colcon-core-0.9.0/README.rst
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.099437 colcon-core-0.9.0/colcon/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      262 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon/__main__.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.099437 colcon-core-0.9.0/colcon_core/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      106 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2046 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/argument_default.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/argument_parser/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9044 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/argument_parser/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1871 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/argument_parser/destination_collector.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3018 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/argument_parser/type_collector.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19593 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1421 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/dependency_descriptor.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6453 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/entry_point.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/environment/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6553 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/environment/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1964 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/environment/path.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1158 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/environment/pythonpath.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      207 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/environment_variable.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/event/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      335 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3723 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2251 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/job.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      747 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/output.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      396 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/test.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      181 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event/timer.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/event_handler/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5395 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event_handler/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1501 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event_handler/console_direct.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2260 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event_handler/console_start_end.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1011 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event_handler/log_command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4643 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/event_reactor.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/executor/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    12986 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/executor/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4017 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/executor/sequential.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7603 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/location.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4289 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/logging.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/package_augmentation/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8166 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_augmentation/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6044 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_augmentation/python.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1771 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_decorator.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5418 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_descriptor.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/package_discovery/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9675 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_discovery/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2449 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_discovery/path.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/package_identification/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6389 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_identification/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      939 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_identification/ignore.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5363 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_identification/python.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/package_selection/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8428 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/package_selection/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6532 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/plugin_system.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/prefix_path/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2996 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/prefix_path/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1306 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/prefix_path/colcon.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/pytest/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/pytest/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      773 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/pytest/hooks.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1232 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/python_install_path.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core/shell/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    24044 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6144 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/bat.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2907 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/dsv.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2172 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/installed_packages.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6269 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/sh.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/shell/template/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3077 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      264 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/command_prefix.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      247 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/command_prefix.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1584 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_append_value.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       26 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_append_value.dsv.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1872 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_append_value.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1279 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_prepend_value.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       26 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_prepend_value.dsv.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      291 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_prepend_value.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      102 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_set_value.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       21 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_set_value.dsv.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       92 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/hook_set_value.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      757 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/package.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       68 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/package.dsv.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2833 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/package.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3897 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4377 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      877 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix_chain.bat.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2011 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix_chain.sh.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4746 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix_util.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    15137 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/shell/template/prefix_util.py.em
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10254 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/subprocess.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/task/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10112 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/__init__.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/task/python/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1535 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    13563 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/build.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/task/python/template/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      174 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/template/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       90 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/template/sitecustomize.py.em
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/task/python/test/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8123 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/test/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7395 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/test/pytest.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1946 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/task/python/test/setuppy_test.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3062 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/topological_order.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.107437 colcon-core-0.9.0/colcon_core/verb/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6479 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/verb/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9063 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/verb/build.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8570 2022-06-23 21:24:45.000000 colcon-core-0.9.0/colcon_core/verb/test.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.103437 colcon-core-0.9.0/colcon_core.egg-info/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1415 2022-06-23 21:30:56.000000 colcon-core-0.9.0/colcon_core.egg-info/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4781 2022-06-23 21:30:57.000000 colcon-core-0.9.0/colcon_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2022-06-23 21:30:56.000000 colcon-core-0.9.0/colcon_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3734 2022-06-23 21:30:56.000000 colcon-core-0.9.0/colcon_core.egg-info/entry_points.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2022-06-23 21:30:31.000000 colcon-core-0.9.0/colcon_core.egg-info/not-zip-safe
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      348 2022-06-23 21:30:56.000000 colcon-core-0.9.0/colcon_core.egg-info/requires.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       19 2022-06-23 21:30:56.000000 colcon-core-0.9.0/colcon_core.egg-info/top_level.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5946 2022-06-23 21:30:57.115437 colcon-core-0.9.0/setup.cfg
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2245 2022-06-23 21:24:45.000000 colcon-core-0.9.0/setup.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2022-06-23 21:30:57.111437 colcon-core-0.9.0/test/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1004 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_argument_default.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4635 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_argument_parser.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3412 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_build_python.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4753 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1393 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_copyright_license.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      737 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_dependency_descriptor.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1322 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_destination_collector.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5431 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_entry_point.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4377 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_environment.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1576 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_environment_path.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1085 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_environment_pythonpath.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1734 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_environment_pythonscriptspath.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1938 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4206 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_handler.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1353 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_handler_console_direct.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2092 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_handler_console_start_end.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      842 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_handler_log_command.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4154 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_event_reactor.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8536 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_executor.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4405 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_executor_sequential.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1752 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_flake8.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8891 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_location.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1823 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_logging.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7249 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_augmentation.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1785 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_decorator.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4054 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_descriptor.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9298 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_discovery.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2795 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_discovery_path.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7165 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_identification.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      818 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_identification_ignore.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5950 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_identification_python.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7722 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_package_selection.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5908 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_plugin_system.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     4231 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_prefix_path.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19638 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_shell.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3478 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_shell_bat.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3520 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_shell_sh.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2124 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_shell_template.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3377 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_shell_template_prefix_util.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1893 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_spell_check.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3028 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_subprocess.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9209 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_task.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     1642 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_task_python_test_pytest.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2319 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_topological_order.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     3380 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_type_collector.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5575 2022-06-23 21:24:45.000000 colcon-core-0.9.0/test/test_verb.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `colcon-core-0.8.3/test/test_environment_pythonscriptspath.py` & `colcon-core-0.9.0/test/test_environment_pythonscriptspath.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_discovery_path.py` & `colcon-core-0.9.0/test/test_package_discovery_path.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_identification.py` & `colcon-core-0.9.0/test/test_package_identification.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_handler_log_command.py` & `colcon-core-0.9.0/test/test_event_handler_log_command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_argument_default.py` & `colcon-core-0.9.0/test/test_argument_default.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_augmentation.py` & `colcon-core-0.9.0/test/test_package_augmentation.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_decorator.py` & `colcon-core-0.9.0/test/test_package_decorator.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_verb.py` & `colcon-core-0.9.0/test/test_verb.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_plugin_system.py` & `colcon-core-0.9.0/test/test_plugin_system.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_environment_path.py` & `colcon-core-0.9.0/test/test_environment_path.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_prefix_path.py` & `colcon-core-0.9.0/test/test_prefix_path.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_topological_order.py` & `colcon-core-0.9.0/test/test_topological_order.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_spell_check.py` & `colcon-core-0.9.0/test/test_spell_check.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_shell_template_prefix_util.py` & `colcon-core-0.9.0/test/test_shell_template_prefix_util.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_command.py` & `colcon-core-0.9.0/test/test_event_command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_shell.py` & `colcon-core-0.9.0/test/test_shell.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_entry_point.py` & `colcon-core-0.9.0/test/test_entry_point.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_build_python.py` & `colcon-core-0.9.0/test/test_build_python.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_environment.py` & `colcon-core-0.9.0/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_shell_bat.py` & `colcon-core-0.9.0/test/test_shell_bat.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_environment_pythonpath.py` & `colcon-core-0.9.0/test/test_environment_pythonpath.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_handler.py` & `colcon-core-0.9.0/test/test_event_handler.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_dependency_descriptor.py` & `colcon-core-0.9.0/test/test_dependency_descriptor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_task.py` & `colcon-core-0.9.0/test/test_task.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_location.py` & `colcon-core-0.9.0/test/test_location.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_descriptor.py` & `colcon-core-0.9.0/test/test_package_descriptor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_logging.py` & `colcon-core-0.9.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_identification_python.py` & `colcon-core-0.9.0/test/test_package_identification_python.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_argument_parser.py` & `colcon-core-0.9.0/test/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_flake8.py` & `colcon-core-0.9.0/test/test_flake8.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_copyright_license.py` & `colcon-core-0.9.0/test/test_copyright_license.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_handler_console_direct.py` & `colcon-core-0.9.0/test/test_event_handler_console_direct.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_executor.py` & `colcon-core-0.9.0/test/test_executor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_subprocess.py` & `colcon-core-0.9.0/test/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_reactor.py` & `colcon-core-0.9.0/test/test_event_reactor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_task_python_test_pytest.py` & `colcon-core-0.9.0/test/test_task_python_test_pytest.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_discovery.py` & `colcon-core-0.9.0/test/test_package_discovery.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_shell_sh.py` & `colcon-core-0.9.0/test/test_shell_sh.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_executor_sequential.py` & `colcon-core-0.9.0/test/test_executor_sequential.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_event_handler_console_start_end.py` & `colcon-core-0.9.0/test/test_event_handler_console_start_end.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_selection.py` & `colcon-core-0.9.0/test/test_package_selection.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_type_collector.py` & `colcon-core-0.9.0/test/test_type_collector.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_package_identification_ignore.py` & `colcon-core-0.9.0/test/test_package_identification_ignore.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_destination_collector.py` & `colcon-core-0.9.0/test/test_destination_collector.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_shell_template.py` & `colcon-core-0.9.0/test/test_shell_template.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/test/test_command.py` & `colcon-core-0.9.0/test/test_command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/setup.py` & `colcon-core-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/PKG-INFO` & `colcon-core-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-core
-Version: 0.8.3
+Version: 0.9.0
 Summary: Command line tool to build sets of software packages.
 Home-page: https://colcon.readthedocs.io
 Author: Dirk Thomas
 Author-email: web@dirk-thomas.net
 Maintainer: Dirk Thomas
 Maintainer-email: web@dirk-thomas.net
 License: Apache License, Version 2.0
```

### Comparing `colcon-core-0.8.3/setup.cfg` & `colcon-core-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 console_scripts = 
 	colcon = colcon_core.command:main
 pytest11 = 
 	colcon_core_warnings_stderr = colcon_core.pytest.hooks
 
 [options.package_data]
 colcon_core.shell.template = *.em
+colcon_core.task.python.template = *.em
 
 [flake8]
 import-order-style = google
 
 [coverage:run]
 source = colcon_core
```

### Comparing `colcon-core-0.8.3/colcon_core.egg-info/SOURCES.txt` & `colcon-core-0.9.0/colcon_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 colcon_core/shell/template/prefix_chain.bat.em
 colcon_core/shell/template/prefix_chain.sh.em
 colcon_core/shell/template/prefix_util.py
 colcon_core/shell/template/prefix_util.py.em
 colcon_core/task/__init__.py
 colcon_core/task/python/__init__.py
 colcon_core/task/python/build.py
+colcon_core/task/python/template/__init__.py
+colcon_core/task/python/template/sitecustomize.py.em
 colcon_core/task/python/test/__init__.py
 colcon_core/task/python/test/pytest.py
 colcon_core/task/python/test/setuppy_test.py
 colcon_core/verb/__init__.py
 colcon_core/verb/build.py
 colcon_core/verb/test.py
 test/test_argument_default.py
```

### Comparing `colcon-core-0.8.3/colcon_core.egg-info/entry_points.txt` & `colcon-core-0.9.0/colcon_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core.egg-info/PKG-INFO` & `colcon-core-0.9.0/colcon_core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-core
-Version: 0.8.3
+Version: 0.9.0
 Summary: Command line tool to build sets of software packages.
 Home-page: https://colcon.readthedocs.io
 Author: Dirk Thomas
 Author-email: web@dirk-thomas.net
 Maintainer: Dirk Thomas
 Maintainer-email: web@dirk-thomas.net
 License: Apache License, Version 2.0
```

### Comparing `colcon-core-0.8.3/colcon_core/prefix_path/colcon.py` & `colcon-core-0.9.0/colcon_core/prefix_path/colcon.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/prefix_path/__init__.py` & `colcon-core-0.9.0/colcon_core/prefix_path/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_decorator.py` & `colcon-core-0.9.0/colcon_core/package_decorator.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event_handler/console_direct.py` & `colcon-core-0.9.0/colcon_core/event_handler/console_direct.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event_handler/log_command.py` & `colcon-core-0.9.0/colcon_core/event_handler/log_command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event_handler/console_start_end.py` & `colcon-core-0.9.0/colcon_core/event_handler/console_start_end.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event_handler/__init__.py` & `colcon-core-0.9.0/colcon_core/event_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/entry_point.py` & `colcon-core-0.9.0/colcon_core/entry_point.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/pytest/hooks.py` & `colcon-core-0.9.0/colcon_core/pytest/hooks.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/dependency_descriptor.py` & `colcon-core-0.9.0/colcon_core/dependency_descriptor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_discovery/path.py` & `colcon-core-0.9.0/colcon_core/package_discovery/path.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_discovery/__init__.py` & `colcon-core-0.9.0/colcon_core/package_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/logging.py` & `colcon-core-0.9.0/colcon_core/logging.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/verb/build.py` & `colcon-core-0.9.0/colcon_core/verb/build.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/verb/test.py` & `colcon-core-0.9.0/colcon_core/verb/test.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/verb/__init__.py` & `colcon-core-0.9.0/colcon_core/verb/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/plugin_system.py` & `colcon-core-0.9.0/colcon_core/plugin_system.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event_reactor.py` & `colcon-core-0.9.0/colcon_core/event_reactor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_identification/ignore.py` & `colcon-core-0.9.0/colcon_core/package_identification/ignore.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_identification/python.py` & `colcon-core-0.9.0/colcon_core/package_identification/python.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_identification/__init__.py` & `colcon-core-0.9.0/colcon_core/package_identification/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/package.bat.em` & `colcon-core-0.9.0/colcon_core/shell/template/package.bat.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix.bat.em` & `colcon-core-0.9.0/colcon_core/shell/template/prefix.bat.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix.sh.em` & `colcon-core-0.9.0/colcon_core/shell/template/prefix.sh.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix_util.py.em` & `colcon-core-0.9.0/colcon_core/shell/template/prefix_util.py.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix_chain.sh.em` & `colcon-core-0.9.0/colcon_core/shell/template/prefix_chain.sh.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/package.sh.em` & `colcon-core-0.9.0/colcon_core/shell/template/package.sh.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix_util.py` & `colcon-core-0.9.0/colcon_core/shell/template/prefix_util.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/hook_prepend_value.bat.em` & `colcon-core-0.9.0/colcon_core/shell/template/hook_prepend_value.bat.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/prefix_chain.bat.em` & `colcon-core-0.9.0/colcon_core/shell/template/prefix_chain.bat.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/__init__.py` & `colcon-core-0.9.0/colcon_core/shell/template/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/hook_append_value.bat.em` & `colcon-core-0.9.0/colcon_core/shell/template/hook_append_value.bat.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/template/hook_append_value.sh.em` & `colcon-core-0.9.0/colcon_core/shell/template/hook_append_value.sh.em`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/bat.py` & `colcon-core-0.9.0/colcon_core/shell/bat.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/installed_packages.py` & `colcon-core-0.9.0/colcon_core/shell/installed_packages.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/sh.py` & `colcon-core-0.9.0/colcon_core/shell/sh.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/dsv.py` & `colcon-core-0.9.0/colcon_core/shell/dsv.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/shell/__init__.py` & `colcon-core-0.9.0/colcon_core/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/argument_parser/type_collector.py` & `colcon-core-0.9.0/colcon_core/argument_parser/type_collector.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/argument_parser/destination_collector.py` & `colcon-core-0.9.0/colcon_core/argument_parser/destination_collector.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/argument_parser/__init__.py` & `colcon-core-0.9.0/colcon_core/argument_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/subprocess.py` & `colcon-core-0.9.0/colcon_core/subprocess.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_selection/__init__.py` & `colcon-core-0.9.0/colcon_core/package_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/argument_default.py` & `colcon-core-0.9.0/colcon_core/argument_default.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/environment/path.py` & `colcon-core-0.9.0/colcon_core/environment/path.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/environment/pythonpath.py` & `colcon-core-0.9.0/colcon_core/environment/pythonpath.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/environment/__init__.py` & `colcon-core-0.9.0/colcon_core/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/topological_order.py` & `colcon-core-0.9.0/colcon_core/topological_order.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_augmentation/python.py` & `colcon-core-0.9.0/colcon_core/package_augmentation/python.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_augmentation/__init__.py` & `colcon-core-0.9.0/colcon_core/package_augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/executor/sequential.py` & `colcon-core-0.9.0/colcon_core/executor/sequential.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/executor/__init__.py` & `colcon-core-0.9.0/colcon_core/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/package_descriptor.py` & `colcon-core-0.9.0/colcon_core/package_descriptor.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event/job.py` & `colcon-core-0.9.0/colcon_core/event/job.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event/command.py` & `colcon-core-0.9.0/colcon_core/event/command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/event/output.py` & `colcon-core-0.9.0/colcon_core/event/output.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/task/python/test/pytest.py` & `colcon-core-0.9.0/colcon_core/task/python/test/pytest.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/task/python/test/setuppy_test.py` & `colcon-core-0.9.0/colcon_core/task/python/test/setuppy_test.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/task/python/test/__init__.py` & `colcon-core-0.9.0/colcon_core/task/python/test/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/task/python/build.py` & `colcon-core-0.9.0/colcon_core/task/python/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from colcon_core.shell import create_environment_hook
 from colcon_core.shell import get_command_environment
 from colcon_core.subprocess import check_output
 from colcon_core.task import run
 from colcon_core.task import TaskExtensionPoint
 from colcon_core.task.python import get_data_files_mapping
 from colcon_core.task.python import get_setup_data
+from colcon_core.task.python.template import expand_template
 
 logger = colcon_logger.getChild(__name__)
 
 
 class PythonBuildTask(TaskExtensionPoint):
     """Build Python packages."""
 
@@ -42,22 +43,31 @@
             env = await get_command_environment(
                 'setup_py', args.build_base, self.context.dependencies)
         except RuntimeError as e:
             logger.error(str(e))
             return 1
         setup_py_data = get_setup_data(self.context.pkg, env)
 
+        # override installation locations
+        prefix_override = Path(args.build_base) / 'prefix_override'
+        expand_template(
+            Path(__file__).parent / 'template' / 'sitecustomize.py.em',
+            prefix_override / 'sitecustomize.py',
+            {
+                'site_prefix': args.install_base,
+            })
+
         # `setup.py develop|install` requires the python lib path to exist
         python_lib = os.path.join(
             args.install_base, self._get_python_lib(args))
         os.makedirs(python_lib, exist_ok=True)
         # and being in the PYTHONPATH
         env = dict(env)
-        env['PYTHONPATH'] = python_lib + os.pathsep + \
-            env.get('PYTHONPATH', '')
+        env['PYTHONPATH'] = str(prefix_override) + os.pathsep + \
+            python_lib + os.pathsep + env.get('PYTHONPATH', '')
 
         # determine if setuptools specific commands are available
         available_commands = await self._get_available_commands(
             args.path, env)
 
         if not args.symlink_install or 'develop' not in available_commands:
             rc = await self._undo_develop(pkg, args, env)
@@ -75,15 +85,15 @@
                     'egg_info', '--egg-base',
                     os.path.relpath(
                         os.path.realpath(args.build_base),
                         os.path.realpath(args.path))]
             cmd += [
                 'build', '--build-base', os.path.join(
                     args.build_base, 'build'),
-                'install', '--prefix', args.install_base,
+                'install',
                 '--record', os.path.join(args.build_base, 'install.log')]
             if 'egg_info' in available_commands:
                 # prevent installation of dependencies specified in setup.py
                 cmd.append('--single-version-externally-managed')
             self._append_install_layout(args, cmd)
             completed = await run(
                 self.context, cmd, cwd=args.path, env=env)
@@ -98,22 +108,22 @@
             # to avoid placing any files in the source space
 
             try:
                 # --editable causes this to skip creating/editing the
                 # easy-install.pth file
                 cmd = [
                     executable, 'setup.py',
-                    'develop', '--prefix', args.install_base,
+                    'develop',
                     '--editable',
                     '--build-directory',
                     os.path.join(args.build_base, 'build'),
                     '--no-deps',
                 ]
                 if setup_py_data.get('data_files'):
-                    cmd += ['install_data', '--install-dir', args.install_base]
+                    cmd += ['install_data']
                 completed = await run(
                     self.context, cmd, cwd=args.build_base, env=env)
             finally:
                 # Remove symlinks that were only needed during build time
                 for symlink in temp_symlinks:
                     os.unlink(symlink)
 
@@ -159,15 +169,15 @@
         # undo previous develop if .egg-info is found and develop symlinks
         egg_info = os.path.join(
             args.build_base, '%s.egg-info' % pkg.name.replace('-', '_'))
         setup_py_build_space = os.path.join(args.build_base, 'setup.py')
         if os.path.exists(egg_info) and os.path.islink(setup_py_build_space):
             cmd = [
                 executable, 'setup.py',
-                'develop', '--prefix', args.install_base,
+                'develop',
                 '--uninstall', '--editable',
                 '--build-directory', os.path.join(args.build_base, 'build')
             ]
             completed = await run(
                 self.context, cmd, cwd=args.build_base, env=env)
             return completed.returncode
```

### Comparing `colcon-core-0.8.3/colcon_core/task/python/__init__.py` & `colcon-core-0.9.0/colcon_core/task/python/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/task/__init__.py` & `colcon-core-0.9.0/colcon_core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/command.py` & `colcon-core-0.9.0/colcon_core/command.py`

 * *Files identical despite different names*

### Comparing `colcon-core-0.8.3/colcon_core/location.py` & `colcon-core-0.9.0/colcon_core/location.py`

 * *Files identical despite different names*

