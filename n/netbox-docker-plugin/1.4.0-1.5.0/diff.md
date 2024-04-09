# Comparing `tmp/netbox-docker-plugin-1.4.0.tar.gz` & `tmp/netbox-docker-plugin-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-docker-plugin-1.4.0.tar", last modified: Wed Mar 27 10:38:27 2024, max compression
+gzip compressed data, was "netbox-docker-plugin-1.5.0.tar", last modified: Tue Apr  9 12:39:58 2024, max compression
```

## Comparing `netbox-docker-plugin-1.4.0.tar` & `netbox-docker-plugin-1.5.0.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.917262 netbox-docker-plugin-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-27 10:38:27.917262 netbox-docker-plugin-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.901262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.901262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.905262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.909262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.909262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.901262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.909262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.909262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.909262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.913262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.917262 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:38:27.917262 netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-27 10:38:27.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-27 10:38:27.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:38:27.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 10:38:27.000000 netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-27 10:38:24.000000 netbox-docker-plugin-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:38:27.917262 netbox-docker-plugin-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.282664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.282664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.282664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.286664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.278664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.290664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-09 12:39:58.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-09 12:39:58.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:39:58.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 12:39:58.000000 netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 12:39:54.000000 netbox-docker-plugin-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:39:58.294664 netbox-docker-plugin-1.5.0/setup.cfg
```

### Comparing `netbox-docker-plugin-1.4.0/LICENSE` & `netbox-docker-plugin-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/PKG-INFO` & `netbox-docker-plugin-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.4.0
+Version: 1.5.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox-docker-plugin-1.4.0/README.md` & `netbox-docker-plugin-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/__init__.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.4.0"
+    version = "1.5.0"
     base_url = "docker"
     author= "Vincent Simonin"
     author_email= "vincent@saashup.com"
 
     def ready(self):
         post_migrate.connect(create_webhook)
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/serializers.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,24 +497,26 @@
 
 class RegistrySerializer(NetBoxModelSerializer):
     """Registry Serializer class"""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_docker_plugin-api:registry-detail"
     )
+    host = NestedHostSerializer()
     images = NestedImageSerializer(many=True, read_only=True)
 
     class Meta:
         """Registry Serializer Meta class"""
 
         model = Registry
         fields = (
             "id",
             "name",
             "url",
+            "host",
             "display",
             "serveraddress",
             "username",
             "password",
             "email",
             "images",
         )
@@ -526,14 +528,15 @@
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_docker_plugin-api:host-detail"
     )
     images = NestedImageSerializer(many=True, read_only=True)
     volumes = NestedVolumeSerializer(many=True, read_only=True)
     networks = NestedNetworkSerializer(many=True, read_only=True)
     containers = NestedContainerSerializer(many=True, read_only=True)
+    registries = NestedRegistrySerializer(many=True, read_only=True)
     token = NestedTokenSerializer(read_only=True)
 
     class Meta:
         """Host Serializer Meta class"""
 
         model = Host
         fields = (
@@ -551,8 +554,9 @@
             "created",
             "last_updated",
             "tags",
             "images",
             "volumes",
             "networks",
             "containers",
+            "registries",
         )
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/api/views.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/api/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from ..models.container import Container
 from ..models.registry import Registry
 
 
 class HostViewSet(NetBoxModelViewSet):
     """Host view set class"""
 
-    queryset = Host.objects.prefetch_related("images", "volumes", "tags")
+    queryset = Host.objects.prefetch_related(
+        "images", "volumes", "networks", "containers", "registries", "tags"
+    )
     filterset_class = filtersets.HostFilterSet
     serializer_class = HostSerializer
     http_method_names = ["get", "post", "patch", "delete", "options"]
 
     def perform_create(self, serializer):
         if isinstance(serializer.validated_data, Sequence):
             for obj in serializer.validated_data:
@@ -93,11 +95,11 @@
     serializer_class = ContainerSerializer
     http_method_names = ["get", "post", "patch", "delete", "options"]
 
 
 class RegistryViewSet(NetBoxModelViewSet):
     """Registry view set class"""
 
-    queryset = Registry.objects.prefetch_related("images", "tags")
+    queryset = Registry.objects.prefetch_related("host", "images", "tags")
     filterset_class = filtersets.RegistryFilterSet
     serializer_class = RegistrySerializer
     http_method_names = ["get", "post", "patch", "delete", "options"]
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/filtersets.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/filtersets.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,19 @@
         return queryset.filter(Q(name__icontains=value))
 
 
 class RegistryFilterSet(NetBoxModelFilterSet):
     """Registry filterset definition class"""
 
     name = filters.CharFilter(lookup_expr="icontains")
+    host_id = ModelMultipleChoiceFilter(
+        field_name="host_id",
+        queryset=Host.objects.all(),
+        label="Host (ID)",
+    )
 
     class Meta:
         """Registry filterset definition meta class"""
 
         model = Registry
         fields = ("name",)
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/bind.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/bind.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/container.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/container.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/env.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/env.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/host.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/host.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/image.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 """Image Forms definitions"""
 
 from django import forms
-from utilities.forms.fields import TagFilterField, DynamicModelMultipleChoiceField
+from utilities.forms.fields import (
+    TagFilterField,
+    DynamicModelMultipleChoiceField,
+    DynamicModelChoiceField,
+)
 from netbox.forms import (
     NetBoxModelForm,
     NetBoxModelImportForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
 )
 from ..models.image import Image
 from ..models.host import Host
 from ..models.registry import Registry
 
 
 class ImageForm(NetBoxModelForm):
     """Image form definition class"""
 
+    host = DynamicModelChoiceField(
+        label="Host", queryset=Host.objects.all(), required=True
+    )
+    registry = DynamicModelChoiceField(
+        label="Registry",
+        queryset=Registry.objects.all(),
+        required=True,
+        query_params={"host_id": "$host"},
+    )
+
     class Meta:
         """Image form definition Meta class"""
 
         model = Image
         fields = (
             "host",
             "registry",
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/label.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/label.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/mount.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/mount.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/network.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/network.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/network_setting.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/port.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/port.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/registry.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Registry Forms definitions"""
 
 from django import forms
-from utilities.forms.fields import TagFilterField
+from utilities.forms.fields import TagFilterField, DynamicModelMultipleChoiceField
 from netbox.forms import (
     NetBoxModelForm,
     NetBoxModelFilterSetForm,
 )
 from ..models.registry import Registry
+from ..models.host import Host
 
 
 class RegistryForm(NetBoxModelForm):
     """Registry form definition class"""
 
     password = forms.CharField(
         label="Password",
@@ -20,14 +21,15 @@
     )
 
     class Meta:
         """Registry form definition Meta class"""
 
         model = Registry
         fields = (
+            "host",
             "name",
             "serveraddress",
             "username",
             "password",
             "email",
             "tags",
         )
@@ -35,9 +37,14 @@
         labels = {"name": "Name", "serveraddress": "Server Address"}
 
 
 class RegistryFilterForm(NetBoxModelFilterSetForm):
     """Registry filter form definition class"""
 
     model = Registry
+    host_id = DynamicModelMultipleChoiceField(
+        queryset=Host.objects.all(),
+        required=False,
+        label="Host",
+    )
     name = forms.CharField(label="Name", required=False)
     tag = TagFilterField(model)
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/forms/volume.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0001_initial.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0002_image.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0004_volume.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0005_network.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """Migration file"""
 
 import taggit.managers
 import utilities.json
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
-import netbox_docker_plugin.models.registry
 
 
 class Migration(migrations.Migration):
     """Migration file"""
 
     dependencies = [
         ("netbox_docker_plugin", "0020_container_hostname"),
@@ -56,15 +55,14 @@
                 "ordering": ("name",),
             },
         ),
         migrations.AddField(
             model_name="image",
             name="registry",
             field=models.ForeignKey(
-                default=netbox_docker_plugin.models.registry.Registry.get_default_registry,
                 on_delete=django.db.models.deletion.CASCADE,
                 related_name="images",
                 to="netbox_docker_plugin.registry",
             ),
         ),
         migrations.RemoveConstraint(
             model_name="image",
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/migrations/__init__.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/container.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/container.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/host.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/image.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 class Image(NetBoxModel):
     """Image definition class"""
 
     host = models.ForeignKey(Host, on_delete=models.CASCADE, related_name="images")
     registry = models.ForeignKey(
         Registry,
-        default=Registry.get_default_registry,  # type: ignore
         on_delete=models.CASCADE,
         related_name="images",
     )
     name = models.CharField(
         max_length=255,
         validators=[
             MinLengthValidator(limit_value=1),
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/network.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/network.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/registry.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 """Registry Model definition"""
 
 from django.db import models
+from django.db.models.signals import post_save
+from django.dispatch import receiver
 from django.core.validators import (
     MinLengthValidator,
     MaxLengthValidator,
 )
 from django.urls import reverse
 from netbox.models import NetBoxModel
+from .host import Host
+
+
+@receiver(post_save, sender=Host)
+def create_default_registry(sender, **kwargs): # pylint: disable=W0613
+    """Create default registry on Host creation"""
+
+    if kwargs.get("created") is True:
+        registry = Registry(
+            host=kwargs.get("instance"),
+            name="dockerhub",
+            serveraddress="https://registry.hub.docker.com/v2/",
+        )
+        registry.save()
 
 
 class Registry(NetBoxModel):
     """Registry definition class"""
 
+    host = models.ForeignKey(Host, on_delete=models.CASCADE, related_name="registries")
     name = models.CharField(
-        unique=True,
         max_length=255,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=255),
         ],
     )
     serveraddress = models.URLField()
     username = models.CharField(blank=True, null=True, max_length=512)
     password = models.CharField(blank=True, null=True, max_length=512)
     email = models.EmailField(blank=True, null=True, max_length=512)
 
-    @classmethod
-    def get_default_registry(cls):
-        """Return the default Registry"""
-        # pylint: disable=W0612
-        registry, created = cls.objects.get_or_create(
-            name="dockerhub",
-            serveraddress="https://registry.hub.docker.com/v2/",
-        )
-        return registry.pk
-
     class Meta:
         """Registry Model Meta Class"""
 
         ordering = ("name",)
+        constraints = (
+            models.UniqueConstraint(
+                fields=["host", "name"],
+                name="%(app_label)s_%(class)s_name_host",
+            ),
+        )
 
     def __str__(self):
         return f"{self.name}"
 
     def get_absolute_url(self):
         """override"""
         return reverse("plugins:netbox_docker_plugin:registry", args=[self.pk])
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/models/volume.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/navigation.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tables.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,31 @@
     {% include 'inc/panels/related_objects.html' with filter_name='host_id' %}
     {% plugin_right_page object %}
   </div>
 </div>
 <div class="row">
   <div class="col col-md-12">
     <div class="card">
+      <h5 class="card-header">Registry</h5>
+      <div class="card-body htmx-container table-responsive"
+        hx-get="{% url 'plugins:netbox_docker_plugin:registry_list' %}?host_id={{ object.pk }}"
+        hx-trigger="load"
+      ></div>
+      {% if perms.netbox_docker_plugin.add_container %}
+        <div class="card-footer text-end noprint">
+          <a href="{% url 'plugins:netbox_docker_plugin:registry_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+            <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Registry
+          </a>
+        </div>
+      {% endif %}
+    </div>
+    {% plugin_full_width_page object %}
+  </div>
+  <div class="col col-md-12">
+    <div class="card">
       <h5 class="card-header">Container</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:container_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_container %}
         <div class="card-footer text-end noprint">
```

#### html2text {}

```diff
@@ -6,14 +6,19 @@
 SSttaattee              {{ object.get_state_display }}
 AAggeenntt VVeerrssiioonn      {{ object.agent_version|placeholder }}
 DDoocckkeerr AAPPII VVeerrssiioonn {{ object.docker_api_version|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %} {% plugin_left_page object %}
 {% include 'inc/panels/related_objects.html' with filter_name='host_id' %} {%
 plugin_right_page object %}
+**** RReeggiissttrryy ****
+{% if perms.netbox_docker_plugin.add_container %}
+_A_d_d_ _a_ _R_e_g_i_s_t_r_y
+{% endif %}
+{% plugin_full_width_page object %}
 **** CCoonnttaaiinneerr ****
 {% if perms.netbox_docker_plugin.add_container %}
 _A_d_d_ _a_ _C_o_n_t_a_i_n_e_r
 {% endif %}
 {% plugin_full_width_page object %}
 **** IImmaaggeess ****
 {% if perms.netbox_docker_plugin.add_image %}
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 <div class="row mb-3">
   <div class="col col-md-6">
     <div class="card">
       <h5 class="card-header">REGISTRY</h5>
       <div class="card-body">
         <table class="table table-hover attr-table">
           <tr>
+            <th scope="row">Host</th>
+            <td><a href="{{ object.host.get_absolute_url }}">{{ object.host }}</a></td>
+          </tr>
+          <tr>
             <th scope="row">Name</th>
             <td>{{ object.name }}</td>
           </tr>
           <tr>
             <th scope="row">Server Address</th>
             <td>{{ object.serveraddress }}</td>
           </tr>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% load host %} {% block
 content %}
 **** RREEGGIISSTTRRYY ****
+HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
 NNaammee           {{ object.name }}
 SSeerrvveerr AAddddrreessss {{ object.serveraddress }}
 uusseerrnnaammee       {{ object.username|placeholder }}
 eemmaaiill          {{ object.email|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
 %} {% plugin_left_page object %}
 {% include 'inc/panels/related_objects.html' with filter_name='registry_id' %}
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/base.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.network import Network
 from netbox_docker_plugin.models.image import Image
 from netbox_docker_plugin.models.volume import Volume
+from netbox_docker_plugin.models.registry import Registry
 from netbox_docker_plugin.tests.base import BaseAPITestCase
 
 
 class ContainerApiTestCase(
     BaseAPITestCase,
     APIViewTestCases.GetObjectViewTestCase,
     APIViewTestCases.ListObjectsViewTestCase,
@@ -40,16 +41,23 @@
     ]
 
     @classmethod
     def setUpTestData(cls) -> None:
         host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
         host2 = Host.objects.create(endpoint="http://localhost:8080", name="host2")
 
-        image1 = Image.objects.create(host=host1, name="image1")
-        image2 = Image.objects.create(host=host2, name="image2")
+        registry1 = Registry.objects.create(
+            host=host1, name="registry1", serveraddress="http://localhost:8080"
+        )
+        registry2 = Registry.objects.create(
+            host=host2, name="registry2", serveraddress="http://localhost:8082"
+        )
+
+        image1 = Image.objects.create(host=host1, name="image1", registry=registry1)
+        image2 = Image.objects.create(host=host2, name="image2", registry=registry2)
 
         network1 = Network.objects.create(host=host1, name="network1")
         network2 = Network.objects.create(host=host2, name="network2")
 
         volume1 = Volume.objects.create(host=host1, name="volume1")
         volume2 = Volume.objects.create(host=host1, name="volume2")
         volume3 = Volume.objects.create(host=host2, name="volume3")
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from utilities.testing.utils import disable_warnings, post_data
 from users.models import ObjectPermission
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.image import Image
+from netbox_docker_plugin.models.registry import Registry
 from netbox_docker_plugin.tests.base import BaseModelViewTestCase
 
 
 class ContainerViewsTestCase(BaseModelViewTestCase, ModelViewTestCase):
     """Container operation Views Test Case Class"""
 
     model = Container
@@ -244,14 +245,21 @@
         )
 
     @classmethod
     def setUpTestData(cls):
         host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
         host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
 
-        image1 = Image.objects.create(host=host1, name="image1")
-        image2 = Image.objects.create(host=host2, name="image2")
+        registry1 = Registry.objects.create(
+            host=host1, name="registry1", serveraddress="http://localhost:8080"
+        )
+        registry2 = Registry.objects.create(
+            host=host2, name="registry2", serveraddress="http://localhost:8082"
+        )
+
+        image1 = Image.objects.create(host=host1, name="image1", registry=registry1)
+        image2 = Image.objects.create(host=host2, name="image2", registry=registry2)
 
         Container.objects.create(host=host1, image=image1, name="container1")
         Container.objects.create(host=host1, image=image1, name="container2")
         Container.objects.create(host=host2, image=image2, name="container3")
         Container.objects.create(host=host2, image=image2, name="container4")
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.test import TestCase
 from django.core.exceptions import ValidationError
 from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.image import Image
 from netbox_docker_plugin.models.volume import Volume
 from netbox_docker_plugin.models.network import Network
+from netbox_docker_plugin.models.registry import Registry
 from netbox_docker_plugin.models.container import Mount, NetworkSetting
 
 
 class ContainerValidationTestCase(TestCase):
     """Container Validation Case Class"""
 
     objects = {}
@@ -109,19 +110,30 @@
         cls.objects["host1"] = Host.objects.create(
             endpoint="http://localhost:8080", name="host1"
         )
         cls.objects["host2"] = Host.objects.create(
             endpoint="http://localhost:8081", name="host2"
         )
 
+        cls.objects["registry1"] = Registry.objects.create(
+            host=cls.objects["host1"],
+            name="registry1",
+            serveraddress="http://localhost:8080",
+        )
+        cls.objects["registry2"] = Registry.objects.create(
+            host=cls.objects["host2"],
+            name="registry2",
+            serveraddress="http://localhost:8082",
+        )
+
         cls.objects["image1"] = Image.objects.create(
-            host=cls.objects["host1"], name="image1"
+            host=cls.objects["host1"], name="image1", registry=cls.objects["registry1"]
         )
         cls.objects["image2"] = Image.objects.create(
-            host=cls.objects["host2"], name="image2"
+            host=cls.objects["host2"], name="image2", registry=cls.objects["registry2"]
         )
 
         cls.objects["volume1"] = Volume.objects.create(
             host=cls.objects["host1"], name="volume1"
         )
         cls.objects["volume2"] = Volume.objects.create(
             host=cls.objects["host2"], name="volume2"
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-"""Container Views Test Case"""
+"""Image Views Test Case"""
 
 from utilities.testing import ViewTestCases
 from netbox_docker_plugin.tests.base import BaseModelViewTestCase
 from netbox_docker_plugin.models.host import Host
-from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.image import Image
+from netbox_docker_plugin.models.registry import Registry
 
 
-class ContainerViewsTestCase(
+class ImageViewsTestCase(
     BaseModelViewTestCase, ViewTestCases.PrimaryObjectViewTestCase
 ):
-    """Container Views Test Case Class"""
+    """Image Views Test Case Class"""
 
-    model = Container
+    model = Image
 
     @classmethod
     def setUpTestData(cls):
         host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
         host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
+        host3 = Host.objects.create(endpoint="http://localhost:8081", name="host3")
 
-        image1 = Image.objects.create(host=host1, name="image1")
-        image2 = Image.objects.create(host=host2, name="image2")
+        registry = Registry.objects.filter(name="dockerhub")[0]
 
-        container1 = Container.objects.create(
-            host=host1, image=image1, name="container1"
-        )
-        container2 = Container.objects.create(
-            host=host1, image=image1, name="container2"
-        )
-        Container.objects.create(host=host2, image=image2, name="container3")
-        Container.objects.create(host=host2, image=image2, name="container4")
+        image1 = Image.objects.create(name="image1", host=host1, registry=registry)
+        image2 = Image.objects.create(name="image2", host=host2, registry=registry)
+        image3 = Image.objects.create(name="image3", host=host3, registry=registry)
 
         cls.form_data = {
-            "name": "container5",
+            "name": "image1",
+            "version": "v1.2.3",
+            "provider": "github",
             "host": host1.pk,
-            "image": image1.pk,
-            "state": "created",
+            "registry": registry.pk,
         }
 
         cls.csv_data = (
-            "name,host,image,hostname",
-            f"container6,{host1.pk},{image1.pk},",
-            f"container7,{host2.pk},{image2.pk},container7",
+            "name,version,registry,host",
+            f"image4,latest,{registry.pk},{host1.pk}",
+            f"image5,,{registry.pk},{host2.pk}",
+            f"image6,v1.2.3,{registry.pk},{host3.pk}",
         )
 
-        cls.bulk_edit_data = {"state": "running"}
+        cls.bulk_edit_data = {"version": "v1.0.0"}
 
         cls.csv_update_data = (
-            "id,name,host,image,state,hostname",
-            f"{container1.pk},container1,{host1.pk},{image1.pk},paused,",
-            f"{container2.pk},container2,{host1.pk},{image1.pk},running,container2",
+            "id,version,registry",
+            f"{image1.pk},latest,{registry.pk}",
+            f"{image2.pk},,{registry.pk}",
+            f"{image3.pk},v1.0.0,{registry.pk}",
         )
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,79 @@
-"""Host API Test Case"""
+"""Host Views Test Case"""
 
 from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ObjectDoesNotExist
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from users.models import ObjectPermission
-from rest_framework import status
-from utilities.testing import APIViewTestCases
+from utilities.testing import ViewTestCases, post_data
 from netbox_docker_plugin.models.host import Host
-from ..base import BaseAPITestCase
+from ..base import BaseModelViewTestCase
 
 
-class HostApiTestCase(
-    BaseAPITestCase,
-    APIViewTestCases.GetObjectViewTestCase,
-    APIViewTestCases.ListObjectsViewTestCase,
-    APIViewTestCases.CreateObjectViewTestCase,
-    APIViewTestCases.UpdateObjectViewTestCase,
-    APIViewTestCases.DeleteObjectViewTestCase,
-):
-    """Host API Test Case Class"""
+class HostViewsTestCase(BaseModelViewTestCase, ViewTestCases.PrimaryObjectViewTestCase):
+    """Host Views Test Case Class"""
 
     model = Host
-    brief_fields = [
-        "agent_version",
-        "display",
-        "docker_api_version",
-        "endpoint",
-        "id",
-        "name",
-        "state",
-        "url",
-    ]
-    create_data = [
-        {
-            "endpoint": "http://localhost:8083",
-            "name": "host4",
-        },
-        {
-            "endpoint": "http://localhost:8084",
-            "name": "host5",
-        },
-        {
-            "endpoint": "http://localhost:8085",
-            "name": "host6",
-        },
-    ]
+    form_data = {
+        "name": "host4",
+        "endpoint": "http://localhost:8084",
+    }
+    csv_data = (
+        "name,endpoint",
+        "host5,http://localhost:8084",
+        "host6,http://localhost:8084",
+        "host7,http://localhost:8084",
+    )
+    bulk_edit_data = {"endpoint": "http://localhost:8083"}
 
     def setUp(self):
         super().setUp()
-        self.header["HTTP_ORIGIN"] = "http://localhost:8080"
+        self.client.defaults = {"HTTP_ORIGIN": "http://localhost:8080"}
 
-    def test_delete_object(self):
-        """
-        DELETE a single object identified by its numeric ID.
-        """
+    def test_delete_object_with_permission(self):
         instance = self._get_queryset().first()
-        url = self._get_detail_url(instance)
 
-        # Add object-level permission
+        # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["delete"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
         obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
 
-        response = self.client.delete(url, **self.header)
-        self.assertHttpStatus(response, status.HTTP_204_NO_CONTENT)
-        self.assertFalse(self._get_queryset().filter(pk=instance.pk).exists())
+        # Try GET with model-level permission
+        self.assertHttpStatus(self.client.get(self._get_url("delete", instance)), 200)
+
+        # Try POST with model-level permission
+        request = {
+            "path": self._get_url("delete", instance),
+            "data": post_data({"confirm": True}),
+        }
+        self.assertHttpStatus(self.client.post(**request), 302)
+        with self.assertRaises(ObjectDoesNotExist):
+            self._get_queryset().get(pk=instance.pk)
 
         objectchanges = ObjectChange.objects.filter(
             changed_object_type=ContentType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 2)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_DELETE
         )
         self.assertEqual(
             objectchanges[1].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
     @classmethod
-    def setUpTestData(cls) -> None:
-        Host.objects.create(endpoint="http://localhost:8080", name="host1")
-        Host.objects.create(endpoint="http://localhost:8081", name="host2")
-        Host.objects.create(endpoint="http://localhost:8081", name="host3")
+    def setUpTestData(cls):
+        host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
+        host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
+        host3 = Host.objects.create(endpoint="http://localhost:8081", name="host3")
+
+        cls.csv_update_data = (
+            "id,endpoint",
+            f"{host1.pk},http://localhost:8085",
+            f"{host2.pk},http://localhost:8085",
+            f"{host3.pk},http://localhost:8085",
+        )
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,65 @@
-"""Image Views Test Case"""
+"""Registry API Test Case"""
 
-from utilities.testing import ViewTestCases
-from netbox_docker_plugin.tests.base import BaseModelViewTestCase
-from netbox_docker_plugin.models.host import Host
-from netbox_docker_plugin.models.image import Image
+from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.registry import Registry
+from netbox_docker_plugin.models.host import Host
+from ..base import BaseAPITestCase
 
 
-class ImageViewsTestCase(
-    BaseModelViewTestCase, ViewTestCases.PrimaryObjectViewTestCase
+class RegistryApiTestCase(
+    BaseAPITestCase,
+    APIViewTestCases.GetObjectViewTestCase,
+    APIViewTestCases.ListObjectsViewTestCase,
+    APIViewTestCases.CreateObjectViewTestCase,
+    APIViewTestCases.UpdateObjectViewTestCase,
+    APIViewTestCases.DeleteObjectViewTestCase,
 ):
-    """Image Views Test Case Class"""
+    """Registry API Test Case Class"""
 
-    model = Image
+    model = Registry
+    brief_fields = [
+        "display",
+        "email",
+        "id",
+        "name",
+        "password",
+        "serveraddress",
+        "url",
+        "username",
+    ]
 
     @classmethod
-    def setUpTestData(cls):
+    def setUpTestData(cls) -> None:
         host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
-        host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
-        host3 = Host.objects.create(endpoint="http://localhost:8081", name="host3")
-
-        registry = Registry.objects.filter(name="dockerhub")[0]
+        host2 = Host.objects.create(endpoint="http://localhost:8080", name="host2")
 
-        image1 = Image.objects.create(name="image1", host=host1, registry=registry)
-        image2 = Image.objects.create(name="image2", host=host2, registry=registry)
-        image3 = Image.objects.create(name="image3", host=host3, registry=registry)
-
-        cls.form_data = {
-            "name": "image1",
-            "version": "v1.2.3",
-            "provider": "github",
-            "host": host1.pk,
-            "registry": registry.pk,
-        }
-
-        cls.csv_data = (
-            "name,version,registry,host",
-            f"image4,latest,{registry.pk},{host1.pk}",
-            f"image5,,{registry.pk},{host2.pk}",
-            f"image6,v1.2.3,{registry.pk},{host3.pk}",
+        Registry.objects.create(
+            host=host1, serveraddress="http://localhost:8080", name="registry0"
         )
-
-        cls.bulk_edit_data = {"version": "v1.0.0"}
-
-        cls.csv_update_data = (
-            "id,version,registry",
-            f"{image1.pk},latest,{registry.pk}",
-            f"{image2.pk},,{registry.pk}",
-            f"{image3.pk},v1.0.0,{registry.pk}",
+        Registry.objects.create(
+            host=host1, serveraddress="http://localhost:8081", name="registry1"
+        )
+        Registry.objects.create(
+            host=host2, serveraddress="http://localhost:8082", name="registry2"
         )
+
+        cls.create_data = [
+        {
+            "host": host1.pk,
+            "name": "github",
+            "serveraddress": "https://ghcr.io",
+        },
+        {
+            "host": host2.pk,
+            "name": "gitlab",
+            "serveraddress": "http://registry.example.com",
+            "username": "test",
+            "password": "goodpassword",
+            "email": "test@example.com",
+        },
+        {
+            "host": host1.pk,
+            "name": "registry",
+            "serveraddress": "http://localhost:1010",
+        },
+    ]
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,39 @@
-"""Registry API Test Case"""
+"""Registry Views Test Case"""
 
-from utilities.testing import APIViewTestCases
+from utilities.testing import ViewTestCases
 from netbox_docker_plugin.models.registry import Registry
-from ..base import BaseAPITestCase
+from netbox_docker_plugin.models.host import Host
+from ..base import BaseModelViewTestCase
 
 
-class RegistryApiTestCase(
-    BaseAPITestCase,
-    APIViewTestCases.GetObjectViewTestCase,
-    APIViewTestCases.ListObjectsViewTestCase,
-    APIViewTestCases.CreateObjectViewTestCase,
-    APIViewTestCases.UpdateObjectViewTestCase,
-    APIViewTestCases.DeleteObjectViewTestCase,
+class RegistryTestCase(
+    BaseModelViewTestCase,
+    ViewTestCases.GetObjectViewTestCase,
+    ViewTestCases.GetObjectChangelogViewTestCase,
+    ViewTestCases.CreateObjectViewTestCase,
+    ViewTestCases.EditObjectViewTestCase,
+    ViewTestCases.DeleteObjectViewTestCase,
+    ViewTestCases.ListObjectsViewTestCase,
+    ViewTestCases.BulkDeleteObjectsViewTestCase,
 ):
-    """Registry API Test Case Class"""
+    """Registry Views Test Case Class"""
 
     model = Registry
-    brief_fields = [
-        "display",
-        "email",
-        "id",
-        "name",
-        "password",
-        "serveraddress",
-        "url",
-        "username",
-    ]
-    create_data = [
-        {
+
+    @classmethod
+    def setUpTestData(cls):
+        host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
+        host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
+
+        Registry.objects.create(host=host1, serveraddress="http://localhost:8080", name="registry0")
+        Registry.objects.create(host=host1, serveraddress="http://localhost:8081", name="registry1")
+        Registry.objects.create(host=host2, serveraddress="http://localhost:8082", name="registry2")
+
+        cls.form_data = {
+            "host": host1.pk,
             "name": "github",
             "serveraddress": "https://ghcr.io",
-        },
-        {
-            "name": "gitlab",
-            "serveraddress": "http://registry.example.com",
             "username": "test",
-            "password": "goodpassword",
+            "password": "thisisapassword",
             "email": "test@example.com",
-        },
-        {
-            "name": "registry",
-            "serveraddress": "http://localhost:1010",
-        },
-    ]
-
-    @classmethod
-    def setUpTestData(cls) -> None:
-        Registry.objects.create(serveraddress="http://localhost:8080", name="registry0")
-        Registry.objects.create(serveraddress="http://localhost:8081", name="registry1")
-        Registry.objects.create(serveraddress="http://localhost:8082", name="registry2")
+        }
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,48 @@
-"""Registry Views Test Case"""
+"""Volume Views Test Case"""
 
 from utilities.testing import ViewTestCases
-from netbox_docker_plugin.models.registry import Registry
-from ..base import BaseModelViewTestCase
+from netbox_docker_plugin.tests.base import BaseModelViewTestCase
+from netbox_docker_plugin.models.host import Host
+from netbox_docker_plugin.models.volume import Volume
 
 
-class RegistryTestCase(
+class VolumeViewsTestCase(
     BaseModelViewTestCase,
     ViewTestCases.GetObjectViewTestCase,
     ViewTestCases.GetObjectChangelogViewTestCase,
     ViewTestCases.CreateObjectViewTestCase,
     ViewTestCases.EditObjectViewTestCase,
     ViewTestCases.DeleteObjectViewTestCase,
     ViewTestCases.ListObjectsViewTestCase,
+    ViewTestCases.BulkImportObjectsViewTestCase,
     ViewTestCases.BulkDeleteObjectsViewTestCase,
 ):
-    """Registry Views Test Case Class"""
+    """Volume Views Test Case Class"""
 
-    model = Registry
-    form_data = {
-        "name": "github",
-        "serveraddress": "https://ghcr.io",
-        "username": "test",
-        "password": "thisisapassword",
-        "email": "test@example.com",
-    }
+    model = Volume
 
     @classmethod
     def setUpTestData(cls):
-        Registry.objects.create(serveraddress="http://localhost:8080", name="registry0")
-        Registry.objects.create(serveraddress="http://localhost:8081", name="registry1")
-        Registry.objects.create(serveraddress="http://localhost:8082", name="registry2")
+        host1 = Host.objects.create(endpoint="http://localhost:8080", name="host1")
+        host2 = Host.objects.create(endpoint="http://localhost:8081", name="host2")
+
+        volume1 = Volume.objects.create(name="volume1", host=host1)
+        volume2 = Volume.objects.create(name="volume2", host=host2)
+
+        cls.form_data = {
+            "name": "volume3",
+            "driver": "local",
+            "host": host1.pk,
+        }
+
+        cls.csv_data = (
+            "name,driver,host",
+            f"volume4,local,{host1.pk}",
+            f"volume5,,{host2.pk}",
+        )
+
+        cls.csv_update_data = (
+            "id,driver",
+            f"{volume1.pk},local",
+            f"{volume2.pk},",
+        )
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/test_init.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/urls.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/utilities/__init__.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/bind.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/container.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/container.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/env.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/host.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/host.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from .. import tables, filtersets
 from ..forms import host
 from ..models.host import Host
 from ..models.image import Image
 from ..models.volume import Volume
 from ..models.network import Network
 from ..models.container import Container
+from ..models.registry import Registry
 
 
 class HostView(generic.ObjectView):
     """Host view definition"""
 
     queryset = Host.objects.prefetch_related(
-        "images", "volumes", "networks", "containers"
+        "images", "volumes", "networks", "containers", "registries"
     )
 
     def get_extra_context(self, request, instance):
         related_models = (
             (
                 Image.objects.filter(host=instance),
                 "host_id",
@@ -33,14 +34,18 @@
                 Network.objects.filter(host=instance),
                 "host_id",
             ),
             (
                 Container.objects.filter(host=instance),
                 "host_id",
             ),
+            (
+                Registry.objects.filter(host=instance),
+                "host_id",
+            ),
         )
 
         return {
             "related_models": related_models,
         }
 
 
@@ -48,14 +53,15 @@
     """Host list view definition"""
 
     queryset = Host.objects.annotate(
         image_count=count_related(Image, "host"),
         volume_count=count_related(Volume, "host"),
         network_count=count_related(Network, "host"),
         container_count=count_related(Container, "host"),
+        registry_count=count_related(Registry, "host"),
     )
     table = tables.HostTable
     filterset = filtersets.HostFilterSet
     filterset_form = host.HostFilterForm
 
 
 class HostEditView(generic.ObjectEditView):
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/image.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/image.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/label.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/mount.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/network.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/network.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/network_setting.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/port.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/registry.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/registry.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin/views/volume.py` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin/views/volume.py`

 * *Files identical despite different names*

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.4.0
+Version: 1.5.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox-docker-plugin-1.4.0/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox-docker-plugin-1.5.0/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 netbox_docker_plugin/migrations/0016_alter_env_value.py
 netbox_docker_plugin/migrations/0017_network_state.py
 netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
 netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
 netbox_docker_plugin/migrations/0020_container_hostname.py
 netbox_docker_plugin/migrations/0021_registry_and_more.py
 netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+netbox_docker_plugin/migrations/0023_delete_hosts.py
+netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
 netbox_docker_plugin/migrations/__init__.py
 netbox_docker_plugin/models/__init__.py
 netbox_docker_plugin/models/container.py
 netbox_docker_plugin/models/host.py
 netbox_docker_plugin/models/image.py
 netbox_docker_plugin/models/network.py
 netbox_docker_plugin/models/registry.py
```

### Comparing `netbox-docker-plugin-1.4.0/pyproject.toml` & `netbox-docker-plugin-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-docker-plugin"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="Vincent Simonin", email="vincent@saashup.com" },
 ]
 description = "Manage Docker with Netbox & style."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

