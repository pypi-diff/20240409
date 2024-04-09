# Comparing `tmp/houdini_package_manager-1.1.1.tar.gz` & `tmp/houdini_package_manager-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-1.1.1.tar", max compression
+gzip compressed data, was "houdini_package_manager-1.1.2.tar", max compression
```

## Comparing `houdini_package_manager-1.1.1.tar` & `houdini_package_manager-1.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    34523 2023-12-26 03:31:09.737911 houdini_package_manager-1.1.1/LICENSE
--rw-r--r--   0        0        0     7059 2023-12-26 03:31:09.737911 houdini_package_manager-1.1.1/README.md
--rw-r--r--   0        0        0       22 2023-12-26 03:31:09.857910 houdini_package_manager-1.1.1/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0     3840 2023-12-26 03:31:09.857910 houdini_package_manager-1.1.1/houdini_package_manager/dialogs.py
--rw-r--r--   0        0        0     1928 2023-12-26 03:31:09.857910 houdini_package_manager-1.1.1/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1975 2023-12-26 03:31:09.857910 houdini_package_manager-1.1.1/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0   614544 2023-12-26 03:31:09.861910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Black.ttf
--rw-r--r--   0        0        0   672480 2023-12-26 03:31:09.865910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
--rw-r--r--   0        0        0   657188 2023-12-26 03:31:09.869911 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   699008 2023-12-26 03:31:09.873911 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0        0        0   723544 2023-12-26 03:31:09.877910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf
--rw-r--r--   0        0        0   644556 2023-12-26 03:31:09.881910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Light.ttf
--rw-r--r--   0        0        0   658212 2023-12-26 03:31:09.881910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
--rw-r--r--   0        0        0   637068 2023-12-26 03:31:09.885910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf
--rw-r--r--   0        0        0   695588 2023-12-26 03:31:09.889910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
--rw-r--r--   0        0        0   657212 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0      332 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add.svg
--rw-r--r--   0        0        0      329 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_hover.svg
--rw-r--r--   0        0        0    10421 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages.svg
--rw-r--r--   0        0        0    10472 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_confirm.svg
--rw-r--r--   0        0        0    10475 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
--rw-r--r--   0        0        0    10424 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_hover.svg
--rw-r--r--   0        0        0     1991 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/bug.svg
--rw-r--r--   0        0        0     1988 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/bug_hover.svg
--rw-r--r--   0        0        0      803 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/delete.svg
--rw-r--r--   0        0        0      424 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/delete_hover.svg
--rw-r--r--   0        0        0      505 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/docs.svg
--rw-r--r--   0        0        0      502 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/docs_hover.svg
--rw-r--r--   0        0        0      455 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/file.svg
--rw-r--r--   0        0        0      452 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/folder.svg
--rw-r--r--   0        0        0      379 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/folder_hover.svg
--rw-r--r--   0        0        0     4286 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm.ico
--rw-r--r--   0        0        0      566 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm.svg
--rw-r--r--   0        0        0      598 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_ICO.svg
--rw-r--r--   0        0        0      591 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_grey.svg
--rw-r--r--   0        0        0      588 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_grey_hover.svg
--rw-r--r--   0        0        0      569 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_hover.svg
--rw-r--r--   0        0        0      571 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_icon.svg
--rw-r--r--   0        0        0      696 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/migrate.svg
--rw-r--r--   0        0        0      320 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2023-12-26 03:31:09.893910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_hover.svg
--rw-r--r--   0        0        0      484 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/remove.svg
--rw-r--r--   0        0        0      390 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      502 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/remove_hover.svg
--rw-r--r--   0        0        0      837 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/repo.svg
--rw-r--r--   0        0        0      834 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/repo_hover.svg
--rw-r--r--   0        0        0      224 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/warning.svg
--rw-r--r--   0        0        0      680 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/warning_hover.svg
--rw-r--r--   0        0        0      868 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/utils.py
--rw-r--r--   0        0        0      655 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0    22508 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     7350 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    21983 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12686 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    34452 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     1079 2023-12-26 03:31:09.897910 houdini_package_manager-1.1.1/houdini_package_manager/wrangle/package_templates.py
--rw-r--r--   0        0        0     2109 2023-12-26 03:31:27.517838 houdini_package_manager-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7740 1970-01-01 00:00:00.000000 houdini_package_manager-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-09 04:44:02.947486 houdini_package_manager-1.1.2/LICENSE
+-rw-r--r--   0        0        0     7059 2024-04-09 04:44:02.947486 houdini_package_manager-1.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0     1936 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2024-04-09 04:44:03.071484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2024-04-09 04:44:03.075484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2024-04-09 04:44:03.079484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2024-04-09 04:44:03.083484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2024-04-09 04:44:03.087484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2024-04-09 04:44:03.091484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2024-04-09 04:44:03.095484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2024-04-09 04:44:03.095484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2024-04-09 04:44:03.099484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      591 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey.svg
+-rw-r--r--   0        0        0      588 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey_hover.svg
+-rw-r--r--   0        0        0      569 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0      868 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22508 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     3840 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/dialogs.py
+-rw-r--r--   0        0        0     7350 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21983 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12686 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    34452 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1126 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2109 2024-04-09 04:44:23.039289 houdini_package_manager-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7740 1970-01-01 00:00:00.000000 houdini_package_manager-1.1.2/PKG-INFO
```

### Comparing `houdini_package_manager-1.1.1/LICENSE` & `houdini_package_manager-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/README.md` & `houdini_package_manager-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/dialogs.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/main.py` & `houdini_package_manager-1.1.2/houdini_package_manager/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # for processing cli args
 import logging
 import sys
 
 from PySide6.QtCore import QTimer
 from PySide6.QtWidgets import QApplication
 
-from houdini_package_manager.dialogs import ErrorDialog, Updater
+from houdini_package_manager.widgets.dialogs import ErrorDialog, Updater
 from houdini_package_manager.widgets.main_window import MainWindow
 from houdini_package_manager.wrangle.config_control import HoudiniManager
 
 
 def main(start: bool = True, headless: bool = False) -> QApplication:
     """Start the Houdini package manager app
```

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-1.1.2/houdini_package_manager/meta/meta_tools.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Black.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Bold.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Italic.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Light.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Medium.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/fonts/Lato-Regular.ttf` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_confirm.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/add_packages_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/bug.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/bug_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/clear_selection.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/clear_selection_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm.ico` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.ico`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_ICO.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_ICO.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_grey.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_grey_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/hpm_icon.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_icon.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/invert_selection.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/invert_selection_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_all.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_all_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/refresh_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/repo.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/repo_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/warning.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/resources/icons/warning_hover.svg` & `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/utils.py` & `houdini_package_manager-1.1.2/houdini_package_manager/utils.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/add_packages_layout.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/add_packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/main_window.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_table.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-1.1.2/houdini_package_manager/wrangle/config_control.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.1/pyproject.toml` & `houdini_package_manager-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "1.1.1"
+version = "1.1.2"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <ariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
```

### Comparing `houdini_package_manager-1.1.1/PKG-INFO` & `houdini_package_manager-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houdini_package_manager
-Version: 1.1.1
+Version: 1.1.2
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: ariffjeff@icloud.com
 Requires-Python: >=3.10.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

