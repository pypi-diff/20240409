# Comparing `tmp/nuon-0.19.92.tar.gz` & `tmp/nuon-0.19.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuon-0.19.92.tar", last modified: Tue Apr  9 00:08:19 2024, max compression
+gzip compressed data, was "nuon-0.19.93.tar", last modified: Tue Apr  9 00:28:16 2024, max compression
```

## Comparing `nuon-0.19.92.tar` & `nuon-0.19.93.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.694736 nuon-0.19.92/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 00:08:19.694736 nuon-0.19.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 00:08:09.000000 nuon-0.19.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.654736 nuon-0.19.92/nuon/
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.658736 nuon-0.19.92/nuon/api/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   208357 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/apps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   230057 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/components_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   100599 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/installers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   263222 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/installs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    74180 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/orgs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55061 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/releases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54514 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api/vcs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.674736 nuon-0.19.92/nuon/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_config_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_config_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_input_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_installer_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_runner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_app_sandbox_config_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_awsecr_image_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_component_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_component_config_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_component_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_component_release_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_connected_github_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_docker_build_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_external_image_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_helm_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_install_sandbox_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_job_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_org_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_org_health_check_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_public_git_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_sandbox_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_sandbox_run_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_terraform_module_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_token_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_user_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_vcs_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/app_vcs_connection_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/metrics_decr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/metrics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/metrics_incr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/metrics_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/planv1_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_app_config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_app_config_template_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_app_input_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_aws_ecr_image_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_connected_github_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_connected_github_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_input_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_runner_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_app_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_component_build_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_component_release_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_component_release_request_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_connection_callback_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_docker_build_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_external_image_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_helm_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_install_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_install_inputs_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_install_request_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_install_request_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_job_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_org_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_create_terraform_module_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_installer_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_public_git_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_public_git_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_publish_metric_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_rendered_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_rendered_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/service_update_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/statsd_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/statsd_event_alert_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/statsd_event_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/models/stderr_err_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-09 00:08:09.000000 nuon-0.19.92/nuon/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.694736 nuon-0.19.92/nuon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 00:08:19.000000 nuon-0.19.92/nuon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-09 00:08:19.000000 nuon-0.19.92/nuon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:08:19.000000 nuon-0.19.92/nuon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 00:08:19.000000 nuon-0.19.92/nuon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 00:08:19.000000 nuon-0.19.92/nuon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 00:08:09.000000 nuon-0.19.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 00:08:19.694736 nuon-0.19.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-09 00:08:09.000000 nuon-0.19.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:08:19.694736 nuon-0.19.92/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_config_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_config_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_input_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_installer_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_runner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_runner_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_app_sandbox_config_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_awsecr_image_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_component_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_component_config_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_component_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_component_release_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_connected_github_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_docker_build_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_external_image_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_helm_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_install_sandbox_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_job_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_org_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_org_health_check_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_public_git_vcs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_sandbox_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_sandbox_run_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_terraform_module_component_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_token_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_user_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_vcs_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_app_vcs_connection_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_apps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_components_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_installers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_installs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_metrics_decr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_metrics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_metrics_incr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_metrics_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_orgs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_planv1_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_releases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_app_config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_app_config_template_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_app_input_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_app_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_aws_ecr_image_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_connected_github_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_connected_github_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_input_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_runner_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_app_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_component_build_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_component_release_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_component_release_request_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_connection_callback_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_docker_build_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_external_image_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_helm_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_install_deploy_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_install_inputs_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_install_request_aws_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_install_request_azure_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_job_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_org_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_create_terraform_module_component_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_installer_create_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_public_git_vcs_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_public_git_vcs_sandbox_config_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_publish_metric_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_rendered_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_rendered_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_app_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_app_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_app_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_component_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_install_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_installer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_installer_request_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_service_update_org_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_statsd_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_statsd_event_alert_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_statsd_event_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_stderr_err_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-09 00:08:09.000000 nuon-0.19.92/test/test_vcs_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.662820 nuon-0.19.93/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 00:28:16.662820 nuon-0.19.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 00:27:59.000000 nuon-0.19.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.618820 nuon-0.19.93/nuon/
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.622820 nuon-0.19.93/nuon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208357 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230057 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/components_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31790 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100599 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/installers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   263222 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/installs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74180 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/orgs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55061 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54514 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api/vcs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.642820 nuon-0.19.93/nuon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_config_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_input_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_installer_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_runner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_app_sandbox_config_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_awsecr_image_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_component_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_component_config_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_component_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_component_release_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_connected_github_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_docker_build_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_external_image_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_helm_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_install_sandbox_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_job_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_org_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_org_health_check_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_public_git_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_sandbox_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_sandbox_run_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_terraform_module_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_user_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_vcs_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/app_vcs_connection_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/metrics_decr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/metrics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/metrics_incr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/metrics_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/planv1_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_app_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_app_config_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_app_input_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_aws_ecr_image_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_connected_github_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_connected_github_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_input_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_runner_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_app_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_component_build_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_component_release_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_component_release_request_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_connection_callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_docker_build_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_external_image_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_helm_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_install_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_install_inputs_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_install_request_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_install_request_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_job_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_org_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_create_terraform_module_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_installer_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_public_git_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_public_git_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_publish_metric_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_rendered_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_rendered_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/service_update_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/statsd_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/statsd_event_alert_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/statsd_event_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/models/stderr_err_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-09 00:27:59.000000 nuon-0.19.93/nuon/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.662820 nuon-0.19.93/nuon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 00:28:16.000000 nuon-0.19.93/nuon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-09 00:28:16.000000 nuon-0.19.93/nuon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:28:16.000000 nuon-0.19.93/nuon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 00:28:16.000000 nuon-0.19.93/nuon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 00:28:16.000000 nuon-0.19.93/nuon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 00:27:59.000000 nuon-0.19.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 00:28:16.662820 nuon-0.19.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-09 00:27:59.000000 nuon-0.19.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:28:16.662820 nuon-0.19.93/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_config_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_input_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_installer_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_runner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_runner_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_app_sandbox_config_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_awsecr_image_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_component_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_component_config_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_component_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_component_release_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_connected_github_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_docker_build_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_external_image_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_helm_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_install_sandbox_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_job_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_org_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_org_health_check_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_public_git_vcs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_sandbox_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_sandbox_run_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_terraform_module_component_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_user_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_vcs_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_app_vcs_connection_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_components_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_installers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_installs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_metrics_decr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_metrics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_metrics_incr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_metrics_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_orgs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_planv1_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_releases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_app_config_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_app_config_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_app_input_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_app_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_aws_ecr_image_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_connected_github_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_connected_github_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_input_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_runner_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_app_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_component_build_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_component_release_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_component_release_request_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_connection_callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_docker_build_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_external_image_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_helm_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_install_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_install_inputs_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_install_request_aws_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_install_request_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_job_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_org_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_create_terraform_module_component_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_installer_create_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_public_git_vcs_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_public_git_vcs_sandbox_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_publish_metric_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_rendered_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_rendered_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_app_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_app_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_component_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_install_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_installer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_installer_request_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_service_update_org_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_statsd_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_statsd_event_alert_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_statsd_event_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_stderr_err_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-09 00:27:59.000000 nuon-0.19.93/test/test_vcs_api.py
```

### Comparing `nuon-0.19.92/nuon/__init__.py` & `nuon-0.19.93/nuon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.19.92"
+__version__ = "0.19.93"
 
 # import apis into sdk package
 from nuon.api.apps_api import AppsApi
 from nuon.api.components_api import ComponentsApi
 from nuon.api.general_api import GeneralApi
 from nuon.api.installers_api import InstallersApi
 from nuon.api.installs_api import InstallsApi
```

### Comparing `nuon-0.19.92/nuon/api/apps_api.py` & `nuon-0.19.93/nuon/api/apps_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/components_api.py` & `nuon-0.19.93/nuon/api/components_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/general_api.py` & `nuon-0.19.93/nuon/api/general_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/installers_api.py` & `nuon-0.19.93/nuon/api/installers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/installs_api.py` & `nuon-0.19.93/nuon/api/installs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/orgs_api.py` & `nuon-0.19.93/nuon/api/orgs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/releases_api.py` & `nuon-0.19.93/nuon/api/releases_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/sandboxes_api.py` & `nuon-0.19.93/nuon/api/sandboxes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api/vcs_api.py` & `nuon-0.19.93/nuon/api/vcs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/api_client.py` & `nuon-0.19.93/nuon/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.19.92/python'
+        self.user_agent = 'OpenAPI-Generator/0.19.93/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `nuon-0.19.92/nuon/api_response.py` & `nuon-0.19.93/nuon/api_response.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/nuon/configuration.py` & `nuon-0.19.93/nuon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -402,16 +402,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.19.92\n"\
-               "SDK Package Version: 0.19.92".\
+               "Version of the API: 0.19.93\n"\
+               "SDK Package Version: 0.19.93".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `nuon-0.19.92/nuon/exceptions.py` & `nuon-0.19.93/nuon/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `nuon-0.19.92/nuon/models/__init__.py` & `nuon-0.19.93/nuon/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app.py` & `nuon-0.19.93/nuon/models/app_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_config.py` & `nuon-0.19.93/nuon/models/app_app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_config_fmt.py` & `nuon-0.19.93/nuon/models/app_app_config_fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_config_status.py` & `nuon-0.19.93/nuon/models/app_app_config_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_input.py` & `nuon-0.19.93/nuon/models/app_app_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_input_config.py` & `nuon-0.19.93/nuon/models/app_app_input_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_installer.py` & `nuon-0.19.93/nuon/models/app_app_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_installer_metadata.py` & `nuon-0.19.93/nuon/models/app_app_installer_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_runner_config.py` & `nuon-0.19.93/nuon/models/app_app_runner_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_runner_type.py` & `nuon-0.19.93/nuon/models/app_install_deploy_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -23,26 +23,25 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class AppAppRunnerType(str, Enum):
+class AppInstallDeployType(str, Enum):
     """
-    AppAppRunnerType
+    AppInstallDeployType
     """
 
     """
     allowed enum values
     """
-    AWS_MINUS_ECS = 'aws-ecs'
-    AWS_MINUS_EKS = 'aws-eks'
-    AZURE_MINUS_AKS = 'azure-aks'
-    AZURE_MINUS_ACS = 'azure-acs'
+    RELEASE = 'release'
+    INSTALL = 'install'
+    TEARDOWN = 'teardown'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AppAppRunnerType from a JSON string"""
+        """Create an instance of AppInstallDeployType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `nuon-0.19.92/nuon/models/app_app_sandbox_config.py` & `nuon-0.19.93/nuon/models/app_app_sandbox_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_app_sandbox_config_artifacts.py` & `nuon-0.19.93/nuon/models/app_app_sandbox_config_artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_aws_account.py` & `nuon-0.19.93/nuon/models/app_aws_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_awsecr_image_config.py` & `nuon-0.19.93/nuon/models/app_awsecr_image_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_azure_account.py` & `nuon-0.19.93/nuon/models/app_azure_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_cloud_platform.py` & `nuon-0.19.93/nuon/models/app_cloud_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_component.py` & `nuon-0.19.93/nuon/models/app_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_component_build.py` & `nuon-0.19.93/nuon/models/app_component_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_component_config_connection.py` & `nuon-0.19.93/nuon/models/app_component_config_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_component_release.py` & `nuon-0.19.93/nuon/models/app_component_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_component_release_step.py` & `nuon-0.19.93/nuon/models/app_component_release_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_connected_github_vcs_config.py` & `nuon-0.19.93/nuon/models/app_connected_github_vcs_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_docker_build_component_config.py` & `nuon-0.19.93/nuon/models/app_docker_build_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_external_image_component_config.py` & `nuon-0.19.93/nuon/models/app_external_image_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_helm_component_config.py` & `nuon-0.19.93/nuon/models/app_helm_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install.py` & `nuon-0.19.93/nuon/models/app_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install_component.py` & `nuon-0.19.93/nuon/models/app_install_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install_deploy.py` & `nuon-0.19.93/nuon/models/app_install_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install_deploy_type.py` & `nuon-0.19.93/nuon/models/statsd_event_alert_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -23,25 +23,26 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class AppInstallDeployType(str, Enum):
+class StatsdEventAlertType(str, Enum):
     """
-    AppInstallDeployType
+    StatsdEventAlertType
     """
 
     """
     allowed enum values
     """
-    RELEASE = 'release'
-    INSTALL = 'install'
-    TEARDOWN = 'teardown'
+    INFO = 'info'
+    ERROR = 'error'
+    WARNING = 'warning'
+    SUCCESS = 'success'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AppInstallDeployType from a JSON string"""
+        """Create an instance of StatsdEventAlertType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `nuon-0.19.92/nuon/models/app_install_event.py` & `nuon-0.19.93/nuon/models/app_install_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install_inputs.py` & `nuon-0.19.93/nuon/models/app_install_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_install_sandbox_run.py` & `nuon-0.19.93/nuon/models/app_install_sandbox_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_job_component_config.py` & `nuon-0.19.93/nuon/models/app_job_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_operation_status.py` & `nuon-0.19.93/nuon/models/app_operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_org.py` & `nuon-0.19.93/nuon/models/app_org.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_org_health_check.py` & `nuon-0.19.93/nuon/models/app_org_health_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_org_health_check_status.py` & `nuon-0.19.93/nuon/models/app_org_health_check_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_public_git_vcs_config.py` & `nuon-0.19.93/nuon/models/app_public_git_vcs_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_sandbox.py` & `nuon-0.19.93/nuon/models/app_sandbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_sandbox_release.py` & `nuon-0.19.93/nuon/models/app_sandbox_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_sandbox_run_type.py` & `nuon-0.19.93/nuon/models/app_sandbox_run_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_terraform_module_component_config.py` & `nuon-0.19.93/nuon/models/app_terraform_module_component_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_token_type.py` & `nuon-0.19.93/nuon/models/app_token_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_user_org.py` & `nuon-0.19.93/nuon/models/app_user_org.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_user_token.py` & `nuon-0.19.93/nuon/models/app_user_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_vcs_connection.py` & `nuon-0.19.93/nuon/models/app_vcs_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/app_vcs_connection_commit.py` & `nuon-0.19.93/nuon/models/app_vcs_connection_commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py` & `nuon-0.19.93/nuon/models/github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/metrics_decr.py` & `nuon-0.19.93/nuon/models/metrics_incr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,17 +24,17 @@
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class MetricsDecr(BaseModel):
+class MetricsIncr(BaseModel):
     """
-    MetricsDecr
+    MetricsIncr
     """ # noqa: E501
     name: Optional[StrictStr] = None
     tags: Optional[List[StrictStr]] = None
     __properties: ClassVar[List[str]] = ["name", "tags"]
 
     model_config = {
         "populate_by_name": True,
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of MetricsDecr from a JSON string"""
+        """Create an instance of MetricsIncr from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,15 +73,15 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of MetricsDecr from a dict"""
+        """Create an instance of MetricsIncr from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `nuon-0.19.92/nuon/models/metrics_event.py` & `nuon-0.19.93/nuon/models/metrics_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/metrics_incr.py` & `nuon-0.19.93/nuon/models/service_create_component_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,21 +24,21 @@
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class MetricsIncr(BaseModel):
+class ServiceCreateComponentRequest(BaseModel):
     """
-    MetricsIncr
+    ServiceCreateComponentRequest
     """ # noqa: E501
-    name: Optional[StrictStr] = None
-    tags: Optional[List[StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["name", "tags"]
+    dependencies: Optional[List[StrictStr]] = None
+    name: StrictStr
+    __properties: ClassVar[List[str]] = ["dependencies", "name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of MetricsIncr from a JSON string"""
+        """Create an instance of ServiceCreateComponentRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,21 +73,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of MetricsIncr from a dict"""
+        """Create an instance of ServiceCreateComponentRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "tags": obj.get("tags")
+            "dependencies": obj.get("dependencies"),
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `nuon-0.19.92/nuon/models/metrics_timing.py` & `nuon-0.19.93/nuon/models/metrics_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/planv1_plan.py` & `nuon-0.19.93/nuon/models/planv1_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_app_config_template.py` & `nuon-0.19.93/nuon/models/service_app_config_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_app_config_template_type.py` & `nuon-0.19.93/nuon/models/service_app_config_template_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_app_input_request.py` & `nuon-0.19.93/nuon/models/service_app_input_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_app_installer.py` & `nuon-0.19.93/nuon/models/service_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/nuon/models/service_aws_ecr_image_config_request.py` & `nuon-0.19.93/nuon/models/service_aws_ecr_image_config_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_cli_config.py` & `nuon-0.19.93/nuon/models/service_cli_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_connected_github_vcs_config_request.py` & `nuon-0.19.93/nuon/models/service_connected_github_vcs_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_connected_github_vcs_sandbox_config_request.py` & `nuon-0.19.93/nuon/models/service_connected_github_vcs_sandbox_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_config_request.py` & `nuon-0.19.93/nuon/models/service_create_app_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_input_config_request.py` & `nuon-0.19.93/nuon/models/service_create_app_input_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_installer_request.py` & `nuon-0.19.93/nuon/models/service_create_app_installer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_installer_request_links.py` & `nuon-0.19.93/nuon/models/service_create_app_installer_request_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_request.py` & `nuon-0.19.93/nuon/models/service_create_app_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_runner_config_request.py` & `nuon-0.19.93/nuon/models/service_create_app_runner_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_app_sandbox_config_request.py` & `nuon-0.19.93/nuon/models/service_create_app_sandbox_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_component_build_request.py` & `nuon-0.19.93/nuon/models/service_create_component_build_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_component_release_request.py` & `nuon-0.19.93/nuon/models/service_create_component_release_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_component_release_request_strategy.py` & `nuon-0.19.93/nuon/models/service_create_component_release_request_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_component_request.py` & `nuon-0.19.93/nuon/models/service_update_component_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,17 +24,17 @@
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceCreateComponentRequest(BaseModel):
+class ServiceUpdateComponentRequest(BaseModel):
     """
-    ServiceCreateComponentRequest
+    ServiceUpdateComponentRequest
     """ # noqa: E501
     dependencies: Optional[List[StrictStr]] = None
     name: StrictStr
     __properties: ClassVar[List[str]] = ["dependencies", "name"]
 
     model_config = {
         "populate_by_name": True,
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceCreateComponentRequest from a JSON string"""
+        """Create an instance of ServiceUpdateComponentRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,15 +73,15 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceCreateComponentRequest from a dict"""
+        """Create an instance of ServiceUpdateComponentRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `nuon-0.19.92/nuon/models/service_create_connection_callback_request.py` & `nuon-0.19.93/nuon/models/service_create_connection_callback_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_connection_request.py` & `nuon-0.19.93/nuon/models/service_create_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_docker_build_component_config_request.py` & `nuon-0.19.93/nuon/models/service_create_docker_build_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_external_image_component_config_request.py` & `nuon-0.19.93/nuon/models/service_create_external_image_component_config_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_helm_component_config_request.py` & `nuon-0.19.93/nuon/models/service_create_helm_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_install_deploy_request.py` & `nuon-0.19.93/nuon/models/service_create_install_deploy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_install_inputs_request.py` & `nuon-0.19.93/nuon/models/service_create_install_inputs_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_install_request.py` & `nuon-0.19.93/nuon/models/service_create_install_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_install_request_aws_account.py` & `nuon-0.19.93/nuon/models/service_create_install_request_aws_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_install_request_azure_account.py` & `nuon-0.19.93/nuon/models/service_create_install_request_azure_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_job_component_config_request.py` & `nuon-0.19.93/nuon/models/service_create_job_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_org_request.py` & `nuon-0.19.93/nuon/models/service_create_org_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_org_user_request.py` & `nuon-0.19.93/nuon/models/service_create_org_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_create_terraform_module_component_config_request.py` & `nuon-0.19.93/nuon/models/service_create_terraform_module_component_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_installer_create_install_request.py` & `nuon-0.19.93/nuon/models/service_installer_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/nuon/models/service_public_git_vcs_config_request.py` & `nuon-0.19.93/nuon/models/service_public_git_vcs_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_public_git_vcs_sandbox_config_request.py` & `nuon-0.19.93/nuon/models/service_public_git_vcs_sandbox_config_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_publish_metric_input.py` & `nuon-0.19.93/nuon/models/service_publish_metric_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_rendered_install.py` & `nuon-0.19.93/nuon/models/service_rendered_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_rendered_installer.py` & `nuon-0.19.93/nuon/models/service_rendered_installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_repository.py` & `nuon-0.19.93/nuon/models/service_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_update_app_installer_request.py` & `nuon-0.19.93/nuon/models/service_update_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/nuon/models/service_update_app_installer_request_links.py` & `nuon-0.19.93/nuon/models/service_update_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/nuon/models/service_update_app_request.py` & `nuon-0.19.93/nuon/models/service_update_app_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_update_component_request.py` & `nuon-0.19.93/nuon/models/service_update_org_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,27 +18,26 @@
 import re  # noqa: F401
 import json
 
 
 
 
 from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceUpdateComponentRequest(BaseModel):
+class ServiceUpdateOrgRequest(BaseModel):
     """
-    ServiceUpdateComponentRequest
+    ServiceUpdateOrgRequest
     """ # noqa: E501
-    dependencies: Optional[List[StrictStr]] = None
     name: StrictStr
-    __properties: ClassVar[List[str]] = ["dependencies", "name"]
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceUpdateComponentRequest from a JSON string"""
+        """Create an instance of ServiceUpdateOrgRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,21 +72,20 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceUpdateComponentRequest from a dict"""
+        """Create an instance of ServiceUpdateOrgRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "dependencies": obj.get("dependencies"),
             "name": obj.get("name")
         })
         return _obj
```

### Comparing `nuon-0.19.92/nuon/models/service_update_install_request.py` & `nuon-0.19.93/nuon/models/service_update_install_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_update_installer_request.py` & `nuon-0.19.93/nuon/models/service_update_installer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_update_installer_request_links.py` & `nuon-0.19.93/nuon/models/service_update_installer_request_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/service_update_org_request.py` & `nuon-0.19.93/nuon/models/metrics_decr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,26 +18,27 @@
 import re  # noqa: F401
 import json
 
 
 
 
 from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ServiceUpdateOrgRequest(BaseModel):
+class MetricsDecr(BaseModel):
     """
-    ServiceUpdateOrgRequest
+    MetricsDecr
     """ # noqa: E501
-    name: StrictStr
-    __properties: ClassVar[List[str]] = ["name"]
+    name: Optional[StrictStr] = None
+    tags: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["name", "tags"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -49,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ServiceUpdateOrgRequest from a JSON string"""
+        """Create an instance of MetricsDecr from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,20 +73,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ServiceUpdateOrgRequest from a dict"""
+        """Create an instance of MetricsDecr from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `nuon-0.19.92/nuon/models/statsd_event.py` & `nuon-0.19.93/nuon/models/statsd_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/models/statsd_event_alert_type.py` & `nuon-0.19.93/nuon/models/statsd_event_priority.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -23,26 +23,24 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class StatsdEventAlertType(str, Enum):
+class StatsdEventPriority(str, Enum):
     """
-    StatsdEventAlertType
+    StatsdEventPriority
     """
 
     """
     allowed enum values
     """
-    INFO = 'info'
-    ERROR = 'error'
-    WARNING = 'warning'
-    SUCCESS = 'success'
+    NORMAL = 'normal'
+    LOW = 'low'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of StatsdEventAlertType from a JSON string"""
+        """Create an instance of StatsdEventPriority from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `nuon-0.19.92/nuon/models/stderr_err_response.py` & `nuon-0.19.93/nuon/models/stderr_err_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon/rest.py` & `nuon-0.19.93/nuon/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `nuon-0.19.92/nuon.egg-info/SOURCES.txt` & `nuon-0.19.93/nuon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/pyproject.toml` & `nuon-0.19.93/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuon"
-version = "0.19.92"
+version = "0.19.93"
 description = "Nuon"
 authors = ["Nuon Support <support@nuon.co>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Nuon"]
 include = ["nuon/py.typed"]
```

### Comparing `nuon-0.19.92/setup.py` & `nuon-0.19.93/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Nuon
 
     API for managing nuon apps, components, and installs.
 
-    The version of the OpenAPI document: 0.19.92
+    The version of the OpenAPI document: 0.19.93
     Contact: support@nuon.co
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "nuon"
-VERSION = "0.19.92"
+VERSION = "0.19.93"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `nuon-0.19.92/test/test_app_app.py` & `nuon-0.19.93/test/test_app_app.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_config.py` & `nuon-0.19.93/test/test_app_app_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_config_fmt.py` & `nuon-0.19.93/test/test_app_app_config_fmt.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_config_status.py` & `nuon-0.19.93/test/test_app_app_config_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_input.py` & `nuon-0.19.93/test/test_app_app_input.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_input_config.py` & `nuon-0.19.93/test/test_app_app_input_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_installer.py` & `nuon-0.19.93/test/test_app_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_installer_metadata.py` & `nuon-0.19.93/test/test_app_app_installer_metadata.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_runner_config.py` & `nuon-0.19.93/test/test_app_app_runner_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_runner_type.py` & `nuon-0.19.93/test/test_app_app_runner_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_sandbox_config.py` & `nuon-0.19.93/test/test_app_app_sandbox_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_app_sandbox_config_artifacts.py` & `nuon-0.19.93/test/test_app_app_sandbox_config_artifacts.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_aws_account.py` & `nuon-0.19.93/test/test_app_aws_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_awsecr_image_config.py` & `nuon-0.19.93/test/test_app_awsecr_image_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_azure_account.py` & `nuon-0.19.93/test/test_app_azure_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_cloud_platform.py` & `nuon-0.19.93/test/test_app_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_component.py` & `nuon-0.19.93/test/test_app_component.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_component_build.py` & `nuon-0.19.93/test/test_app_component_build.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_component_config_connection.py` & `nuon-0.19.93/test/test_app_component_config_connection.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_component_release.py` & `nuon-0.19.93/test/test_app_component_release.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_component_release_step.py` & `nuon-0.19.93/test/test_app_component_release_step.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_connected_github_vcs_config.py` & `nuon-0.19.93/test/test_app_connected_github_vcs_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_docker_build_component_config.py` & `nuon-0.19.93/test/test_app_docker_build_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_external_image_component_config.py` & `nuon-0.19.93/test/test_app_external_image_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_helm_component_config.py` & `nuon-0.19.93/test/test_app_helm_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install.py` & `nuon-0.19.93/test/test_app_install.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_component.py` & `nuon-0.19.93/test/test_app_install_component.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_deploy.py` & `nuon-0.19.93/test/test_app_install_deploy.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_deploy_type.py` & `nuon-0.19.93/test/test_app_install_deploy_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_event.py` & `nuon-0.19.93/test/test_app_install_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_inputs.py` & `nuon-0.19.93/test/test_app_install_inputs.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_install_sandbox_run.py` & `nuon-0.19.93/test/test_app_install_sandbox_run.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_job_component_config.py` & `nuon-0.19.93/test/test_app_job_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_operation_status.py` & `nuon-0.19.93/test/test_app_operation_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_org.py` & `nuon-0.19.93/test/test_app_org.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_org_health_check.py` & `nuon-0.19.93/test/test_app_org_health_check.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_org_health_check_status.py` & `nuon-0.19.93/test/test_app_org_health_check_status.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_public_git_vcs_config.py` & `nuon-0.19.93/test/test_app_public_git_vcs_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_sandbox.py` & `nuon-0.19.93/test/test_app_sandbox.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_sandbox_release.py` & `nuon-0.19.93/test/test_app_sandbox_release.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_sandbox_run_type.py` & `nuon-0.19.93/test/test_app_sandbox_run_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_terraform_module_component_config.py` & `nuon-0.19.93/test/test_app_terraform_module_component_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_token_type.py` & `nuon-0.19.93/test/test_app_token_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_user_org.py` & `nuon-0.19.93/test/test_app_user_org.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_user_token.py` & `nuon-0.19.93/test/test_app_user_token.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_vcs_connection.py` & `nuon-0.19.93/test/test_app_vcs_connection.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_app_vcs_connection_commit.py` & `nuon-0.19.93/test/test_app_vcs_connection_commit.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_apps_api.py` & `nuon-0.19.93/test/test_apps_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_components_api.py` & `nuon-0.19.93/test/test_components_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_general_api.py` & `nuon-0.19.93/test/test_general_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py` & `nuon-0.19.93/test/test_github_com_powertoolsdev_mono_services_ctl_api_internal_app_installs_worker_signals_operation.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_installers_api.py` & `nuon-0.19.93/test/test_installers_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_installs_api.py` & `nuon-0.19.93/test/test_installs_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_metrics_decr.py` & `nuon-0.19.93/test/test_metrics_decr.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_metrics_event.py` & `nuon-0.19.93/test/test_metrics_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_metrics_incr.py` & `nuon-0.19.93/test/test_metrics_incr.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_metrics_timing.py` & `nuon-0.19.93/test/test_metrics_timing.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_orgs_api.py` & `nuon-0.19.93/test/test_orgs_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_planv1_plan.py` & `nuon-0.19.93/test/test_planv1_plan.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_releases_api.py` & `nuon-0.19.93/test/test_releases_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_sandboxes_api.py` & `nuon-0.19.93/test/test_sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_app_config_template.py` & `nuon-0.19.93/test/test_service_app_config_template.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_app_config_template_type.py` & `nuon-0.19.93/test/test_service_app_config_template_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_app_input_request.py` & `nuon-0.19.93/test/test_service_app_input_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_app_installer.py` & `nuon-0.19.93/test/test_service_app_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_aws_ecr_image_config_request.py` & `nuon-0.19.93/test/test_service_aws_ecr_image_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_cli_config.py` & `nuon-0.19.93/test/test_service_cli_config.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_connected_github_vcs_config_request.py` & `nuon-0.19.93/test/test_service_connected_github_vcs_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_connected_github_vcs_sandbox_config_request.py` & `nuon-0.19.93/test/test_service_connected_github_vcs_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_config_request.py` & `nuon-0.19.93/test/test_service_create_app_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_input_config_request.py` & `nuon-0.19.93/test/test_service_create_app_input_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_installer_request.py` & `nuon-0.19.93/test/test_service_create_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_installer_request_links.py` & `nuon-0.19.93/test/test_service_create_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_request.py` & `nuon-0.19.93/test/test_service_create_app_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_runner_config_request.py` & `nuon-0.19.93/test/test_service_create_app_runner_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_app_sandbox_config_request.py` & `nuon-0.19.93/test/test_service_create_app_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_component_build_request.py` & `nuon-0.19.93/test/test_service_create_component_build_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_component_release_request.py` & `nuon-0.19.93/test/test_service_create_component_release_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_component_release_request_strategy.py` & `nuon-0.19.93/test/test_service_create_component_release_request_strategy.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_component_request.py` & `nuon-0.19.93/test/test_service_create_component_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_connection_callback_request.py` & `nuon-0.19.93/test/test_service_create_connection_callback_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_connection_request.py` & `nuon-0.19.93/test/test_service_create_connection_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_docker_build_component_config_request.py` & `nuon-0.19.93/test/test_service_create_docker_build_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_external_image_component_config_request.py` & `nuon-0.19.93/test/test_service_create_external_image_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_helm_component_config_request.py` & `nuon-0.19.93/test/test_service_create_helm_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_install_deploy_request.py` & `nuon-0.19.93/test/test_service_create_install_deploy_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_install_inputs_request.py` & `nuon-0.19.93/test/test_service_create_install_inputs_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_install_request.py` & `nuon-0.19.93/test/test_service_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_install_request_aws_account.py` & `nuon-0.19.93/test/test_service_create_install_request_aws_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_install_request_azure_account.py` & `nuon-0.19.93/test/test_service_create_install_request_azure_account.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_job_component_config_request.py` & `nuon-0.19.93/test/test_service_create_job_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_org_request.py` & `nuon-0.19.93/test/test_service_create_org_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_org_user_request.py` & `nuon-0.19.93/test/test_service_create_org_user_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_create_terraform_module_component_config_request.py` & `nuon-0.19.93/test/test_service_create_terraform_module_component_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_installer_create_install_request.py` & `nuon-0.19.93/test/test_service_installer_create_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_public_git_vcs_config_request.py` & `nuon-0.19.93/test/test_service_public_git_vcs_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_public_git_vcs_sandbox_config_request.py` & `nuon-0.19.93/test/test_service_public_git_vcs_sandbox_config_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_publish_metric_input.py` & `nuon-0.19.93/test/test_service_publish_metric_input.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_rendered_install.py` & `nuon-0.19.93/test/test_service_rendered_install.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_rendered_installer.py` & `nuon-0.19.93/test/test_service_rendered_installer.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_repository.py` & `nuon-0.19.93/test/test_service_repository.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_app_installer_request.py` & `nuon-0.19.93/test/test_service_update_app_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_app_installer_request_links.py` & `nuon-0.19.93/test/test_service_update_app_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_app_request.py` & `nuon-0.19.93/test/test_service_update_app_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_component_request.py` & `nuon-0.19.93/test/test_service_update_component_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_install_request.py` & `nuon-0.19.93/test/test_service_update_install_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_installer_request.py` & `nuon-0.19.93/test/test_service_update_installer_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_installer_request_links.py` & `nuon-0.19.93/test/test_service_update_installer_request_links.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_service_update_org_request.py` & `nuon-0.19.93/test/test_service_update_org_request.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_statsd_event.py` & `nuon-0.19.93/test/test_statsd_event.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_statsd_event_alert_type.py` & `nuon-0.19.93/test/test_statsd_event_alert_type.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_statsd_event_priority.py` & `nuon-0.19.93/test/test_statsd_event_priority.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_stderr_err_response.py` & `nuon-0.19.93/test/test_stderr_err_response.py`

 * *Files identical despite different names*

### Comparing `nuon-0.19.92/test/test_vcs_api.py` & `nuon-0.19.93/test/test_vcs_api.py`

 * *Files identical despite different names*

