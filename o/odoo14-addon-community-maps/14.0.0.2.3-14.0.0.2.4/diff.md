# Comparing `tmp/odoo14-addon-community_maps-14.0.0.2.3.tar.gz` & `tmp/odoo14-addon-community_maps-14.0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-community_maps-14.0.0.2.3.tar", last modified: Fri Mar  8 16:43:50 2024, max compression
+gzip compressed data, was "odoo14-addon-community_maps-14.0.0.2.4.tar", last modified: Tue Apr  9 14:26:16 2024, max compression
```

## Comparing `odoo14-addon-community_maps-14.0.0.2.3.tar` & `odoo14-addon-community_maps-14.0.0.2.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/PKG-INFO
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.611062 odoo14-addon-community_maps-14.0.0.2.3/odoo/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      116 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1336 2024-03-08 16:42:24.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/__manifest__.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/controllers/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       80 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/controllers/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      481 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/controllers/cm_map_controller.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1297 2024-03-07 17:07:22.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/data/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1960 2024-03-08 13:49:34.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/data/collect_place_submission_email_template.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      736 2024-03-05 11:29:58.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1055 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_button_color_config.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      357 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_crowdfunding_notification.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1056 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      466 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_external_id_mixin.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1728 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_filter.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1074 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_filter_group.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2913 2023-11-24 11:04:01.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_model.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6944 2024-03-07 17:00:46.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_submission.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      351 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_submission_metadata.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4426 2024-03-08 13:05:31.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    22162 2024-03-08 15:09:59.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1560 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map_colorschema.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5850 2024-01-30 10:24:48.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map_social_item.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      272 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_partner.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    36502 2024-03-08 14:57:54.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2918 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_category.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4141 2024-03-08 10:59:39.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_child.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      981 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_external_link.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      371 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_presenter_metadata.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      846 2024-01-23 16:39:43.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_presenter_model.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1831 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_slug_id_mixin.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      663 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_utils.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/security/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1610 2024-03-05 15:16:05.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/security/ir.model.access.csv
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3467 2024-03-08 09:11:49.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/security/rules.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       64 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5156 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/cm_map_forms_service.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6174 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/cm_map_service.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/static/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/static/src/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/static/src/img/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    21929 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2130 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_button_color_config_id.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2593 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_filter_group.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3062 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_model.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5900 2024-03-07 10:08:32.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_submission.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2374 2024-03-08 09:10:42.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     9856 2024-03-08 13:51:25.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_map.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2189 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_map_colorschema.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      171 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_menu_root.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      135 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_menu_root_config.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12868 2024-03-08 14:48:52.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2197 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place_category.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      770 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1933 2023-12-22 15:00:06.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_presenter_model.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      759 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      556 2024-03-05 09:54:25.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/ir_cron_views.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       43 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3307 2024-03-07 15:35:58.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1540 2024-03-05 09:27:15.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-03-08 16:43:50.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/PKG-INFO
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3311 2024-03-08 16:43:50.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/SOURCES.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-03-08 16:43:50.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/dependency_links.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2023-12-05 08:53:35.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/not-zip-safe
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      127 2024-03-08 16:43:50.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/requires.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-03-08 16:43:50.000000 odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/top_level.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-03-08 16:43:50.614395 odoo14-addon-community_maps-14.0.0.2.3/setup.cfg
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      256 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.3/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      116 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1336 2024-04-09 14:15:15.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       80 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/controllers/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      481 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/controllers/cm_map_controller.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1304 2024-04-09 14:18:10.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/data/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1960 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/data/collect_place_submission_email_template.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      736 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1055 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_button_color_config.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      357 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_crowdfunding_notification.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1056 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      466 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_external_id_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1728 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_filter.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1074 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_filter_group.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2913 2023-11-24 11:04:01.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_model.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6944 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_submission.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      351 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_submission_metadata.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4426 2024-04-09 14:16:53.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    22162 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1560 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map_colorschema.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5850 2024-01-30 10:24:48.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map_social_item.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      272 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_partner.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    36502 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2918 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_category.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4141 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_child.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      981 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_external_link.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      371 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_presenter_metadata.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      846 2024-01-23 16:39:43.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_presenter_model.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1831 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_slug_id_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      663 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_utils.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1610 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/security/ir.model.access.csv
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3467 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/security/rules.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       64 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5156 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/cm_map_forms_service.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6174 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/cm_map_service.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/static/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/static/src/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.793235 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/static/src/img/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    21929 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2130 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_button_color_config_id.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2593 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_filter_group.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3062 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_model.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5900 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_submission.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2374 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     9856 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_map.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2189 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_map_colorschema.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      171 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_menu_root.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      135 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_menu_root_config.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12868 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2197 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place_category.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      770 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1933 2023-12-22 15:00:06.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_presenter_model.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      759 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      556 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/ir_cron_views.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       43 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3307 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1540 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-04-09 14:26:16.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3311 2024-04-09 14:26:16.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-04-09 14:26:16.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2023-12-05 08:53:35.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      127 2024-04-09 14:26:16.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-04-09 14:26:16.000000 odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-04-09 14:26:16.796569 odoo14-addon-community_maps-14.0.0.2.4/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      256 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.4/setup.py
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/__manifest__.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'summary': """
     Module to create and manage your map visualizations into a  website""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "https://gitlab.com/coopdevs/community-maps-builder-backend",
 
     'category': 'community-maps',
-    'version': '14.0.0.2.3',
+    'version': '14.0.0.2.4',
 
     'depends': [
         'base',
         'base_rest',
         'base_rest_base_structure',
         'sale',
         'crm',
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             values = {'error': _('The url to perform this action is not correct.')}
             return request.render("community_maps.submission_transfer_page",values)
         request_id = request.env['cm.form.submission.transfer.request'].search([('cm_external_id','=',kwargs['request'])])
         if not request_id:
             values = {'error': _('The url to perform this action is not correct.')}
             return request.render("community_maps.submission_transfer_page",values)
         # mark rejection
-        request_id.with_delay().reject_request_transfer_reject()
+        request_id.sudo().with_delay().reject_request_transfer_reject()
         # return success
         values = {
             'success': _('The action has been successfully executed. Your submission will stay at {}').format(
                 request_id.origin_place_id.name
             )
         }
         return request.render("community_maps.submission_transfer_page",values)
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/data/collect_place_submission_email_template.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/data/collect_place_submission_email_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/__init__.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_button_color_config.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_button_color_config.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_filter.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_filter.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_filter_group.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_filter_group.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_model.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_model.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_submission.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_submission.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map_colorschema.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map_colorschema.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_map_social_item.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_map_social_item.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_category.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_category.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_child.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_child.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_place_external_link.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_place_external_link.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_presenter_model.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_presenter_model.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_slug_id_mixin.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_slug_id_mixin.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/models/cm_utils.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/models/cm_utils.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/security/ir.model.access.csv` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/security/rules.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/security/rules.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/cm_map_forms_service.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/cm_map_forms_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/services/cm_map_service.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/services/cm_map_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_button_color_config_id.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_button_color_config_id.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_filter_group.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_filter_group.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_model.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_model.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_submission.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_submission.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_map.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_map.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_map_colorschema.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_map_colorschema.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place_category.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place_category.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_presenter_model.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_presenter_model.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/views/ir_cron_views.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/views/ir_cron_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml` & `odoo14-addon-community_maps-14.0.0.2.4/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.3/odoo14_addon_community_maps.egg-info/SOURCES.txt` & `odoo14-addon-community_maps-14.0.0.2.4/odoo14_addon_community_maps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

