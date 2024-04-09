# Comparing `tmp/smol_k8s_lab-4.0.0.tar.gz` & `tmp/smol_k8s_lab-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-4.0.0.tar", max compression
+gzip compressed data, was "smol_k8s_lab-4.0.1.tar", max compression
```

## Comparing `smol_k8s_lab-4.0.0.tar` & `smol_k8s_lab-4.0.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    34260 2024-04-08 12:51:25.226617 smol_k8s_lab-4.0.0/LICENSE
--rw-r--r--   0        0        0    27169 2024-04-08 12:51:25.226617 smol_k8s_lab-4.0.0/README.md
--rw-r--r--   0        0        0     2266 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/pyproject.toml
--rwxr-xr-x   0        0        0    15143 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/__init__.py
--rwxr-xr-x   0        0        0    12779 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    64187 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5675 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rwxr-xr-x   0        0        0     2318 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9486 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6716 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0    10293 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    14554 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20412 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3370 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1860 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1761 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    11178 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2543 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0      591 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/k8up_operater.py
--rw-r--r--   0        0        0      573 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/longhorn.py
--rw-r--r--   0        0        0    16270 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     4471 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0      520 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/prometheus.py
--rw-r--r--   0        0        0     4590 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2671 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3889 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     5089 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0     4974 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    15769 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1702 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    12253 2024-04-08 12:51:25.474617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    13293 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     4129 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     6497 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3751 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     7779 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4817 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     5548 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/argocd_util.py
--rwxr-xr-x   0        0        0     8032 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    10312 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0      219 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k9s.py
--rw-r--r--   0        0        0     1358 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    10866 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     7501 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0     6827 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     3533 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6904 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3763 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    10680 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    21507 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0     6151 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base_cluster_modal.py
--rwxr-xr-x   0        0        0     8373 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0      925 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     6076 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1561 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6386 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1116 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      867 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      855 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     1940 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1720 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1247 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3096 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2683 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10237 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    11500 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    13289 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4509 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4210 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     3733 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0     7714 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0    10049 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9388 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0     1184 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4624 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/help_text.py
--rwxr-xr-x   0        0        0     7215 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/subproc.py
--rw-r--r--   0        0        0      315 2024-04-08 12:51:25.478617 smol_k8s_lab-4.0.0/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    28815 1970-01-01 00:00:00.000000 smol_k8s_lab-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-04-08 14:11:19.785210 smol_k8s_lab-4.0.1/LICENSE
+-rw-r--r--   0        0        0    27169 2024-04-08 14:11:19.785210 smol_k8s_lab-4.0.1/README.md
+-rw-r--r--   0        0        0     2264 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0    15143 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/__init__.py
+-rwxr-xr-x   0        0        0    12779 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    64187 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5675 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rwxr-xr-x   0        0        0     2318 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9486 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6716 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0    10293 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    14554 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20412 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3370 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1860 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1761 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    11178 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2543 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/k8up_operater.py
+-rw-r--r--   0        0        0      573 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/longhorn.py
+-rw-r--r--   0        0        0    16270 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     4471 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0      520 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/prometheus.py
+-rw-r--r--   0        0        0     4590 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3889 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     5089 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0     4974 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    15769 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1702 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    12253 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    13293 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     4129 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     6497 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3751 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     7779 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4817 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     5548 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/argocd_util.py
+-rwxr-xr-x   0        0        0     8032 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    10312 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0      219 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/k9s.py
+-rw-r--r--   0        0        0     1358 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    10866 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     7501 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0     6827 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     3533 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6904 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3763 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    10680 2024-04-08 14:11:20.037213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    21507 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0     6151 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/base_cluster_modal.py
+-rwxr-xr-x   0        0        0     8373 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0      925 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     6076 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1561 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6386 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1116 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      867 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      855 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     1940 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1720 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1247 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3096 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2683 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10237 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    11500 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    13289 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4509 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4210 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     3733 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0     7714 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0    10049 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9388 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4624 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/rich_cli/help_text.py
+-rwxr-xr-x   0        0        0     7215 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/subproc.py
+-rw-r--r--   0        0        0      315 2024-04-08 14:11:20.041213 smol_k8s_lab-4.0.1/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    28815 1970-01-01 00:00:00.000000 smol_k8s_lab-4.0.1/PKG-INFO
```

### Comparing `smol_k8s_lab-4.0.0/LICENSE` & `smol_k8s_lab-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/README.md` & `smol_k8s_lab-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/pyproject.toml` & `smol_k8s_lab-4.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "4.0.0"
+version       = "4.0.1"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
@@ -35,23 +35,23 @@
 pyjwt              = "^2.8"
 python             = ">=3.11,<4.0"
 pyyaml             = "^6.0"
 requests           = "^2.28"
 rich               = "^13.0"
 ruamel-yaml        = "^0.18"
 ruamel-yaml-string = "^0.1"
-textual            = "^0.54"
+textual            = "^0.56"
 xdg-base-dirs      = "^6.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5"
 mkdocs-video = "^1.5"
 
 [tool.poetry.group.dev.dependencies]
-deptry = "^0.15.0"
+deptry = "^0.16"
 textual-dev = "^1.1"
 pytest-textual-snapshot = "^0.4"
 
 [tool.poetry.plugins."smol-k8s-lab.application.plugin"]
 "smol-k8s-lab" = "smol_k8s_lab:main"
 
 [tool.poetry.scripts]
```

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/__init__.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-4.0.1/smol_k8s_lab/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-4.0.1/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/constants.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/env_config.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/k8up_operater.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/k8up_operater.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/longhorn.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/longhorn.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/prometheus.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/prometheus.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/home_assistant.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/apps_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/base.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/base_cluster_modal.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/base_cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/confirm_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/base.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/help_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/smol_k8s_lab/utils/subproc.py` & `smol_k8s_lab-4.0.1/smol_k8s_lab/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-4.0.0/PKG-INFO` & `smol_k8s_lab-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 4.0.0
+Version: 4.0.1
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -25,15 +25,15 @@
 Requires-Dist: pyfiglet (>=1.0,<2.0)
 Requires-Dist: pyjwt (>=2.8,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: ruamel-yaml (>=0.18,<0.19)
 Requires-Dist: ruamel-yaml-string (>=0.1,<0.2)
-Requires-Dist: textual (>=0.54,<0.55)
+Requires-Dist: textual (>=0.56,<0.57)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
 Project-URL: Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues
 Project-URL: Documentation, https://small-hack.github.io/smol-k8s-lab
 Project-URL: Repository, http://github.com/small-hack/smol-k8s-lab
 Description-Content-Type: text/markdown
 
 <h2 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 4.0.0 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 4.0.1 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
@@ -11,15 +11,15 @@
 Programming Language :: Python :: 3.12 Classifier: Topic :: System ::
 Installation/Setup Requires-Dist: bcrypt (>=4.0,<5.0) Requires-Dist: click
 (>=8.1,<9.0) Requires-Dist: cryptography (>=42.0,<43.0) Requires-Dist:
 kubernetes (>=29,<30) Requires-Dist: minio (>=7.2,<8.0) Requires-Dist: pyfiglet
 (>=1.0,<2.0) Requires-Dist: pyjwt (>=2.8,<3.0) Requires-Dist: pyyaml
 (>=6.0,<7.0) Requires-Dist: requests (>=2.28,<3.0) Requires-Dist: rich
 (>=13.0,<14.0) Requires-Dist: ruamel-yaml (>=0.18,<0.19) Requires-Dist: ruamel-
-yaml-string (>=0.1,<0.2) Requires-Dist: textual (>=0.54,<0.55) Requires-Dist:
+yaml-string (>=0.1,<0.2) Requires-Dist: textual (>=0.56,<0.57) Requires-Dist:
 xdg-base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/small-
 hack/smol-k8s-lab/issues Project-URL: Documentation, https://small-
 hack.github.io/smol-k8s-lab Project-URL: Repository, http://github.com/small-
 hack/smol-k8s-lab Description-Content-Type: text/markdown
   ********** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ccaattppppuucccciinn//ccaattppppuucccciinn//mmaaiinn//aasssseettss//
 mmiisscc//ttrraannssppaarreenntt..ppnngg]]?ð??§?¸ ssmmooll--kk88ss--llaabb_[[_hh_tt_tt_pp_ss_::_//_//_ii_mm_gg_.._ss_hh_ii_ee_ll_dd_ss_.._ii_oo_//_gg_ii_tt_hh_uu_bb_//_vv_//_rr_ee_ll_ee_aa_ss_ee_//
                              _ss_mm_aa_ll_ll_--_hh_aa_cc_kk_//_ss_mm_oo_ll_--_kk_88_ss_--
```

