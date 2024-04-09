# Comparing `tmp/scs-analysis-3.7.2.tar.gz` & `tmp/scs-analysis-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-3.7.2.tar", last modified: Mon Apr  8 08:21:21 2024, max compression
+gzip compressed data, was "scs-analysis-3.8.0.tar", last modified: Tue Apr  9 15:14:44 2024, max compression
```

## Comparing `scs-analysis-3.7.2.tar` & `scs-analysis-3.8.0.tar`

### file list

```diff
@@ -1,168 +1,170 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.682293 scs-analysis-3.7.2/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs-analysis-3.7.2/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-08 08:21:21.682102 scs-analysis-3.7.2/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-08 08:21:13.000000 scs-analysis-3.7.2/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-08 08:21:21.682329 scs-analysis-3.7.2/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     5533 2024-03-11 10:25:23.000000 scs-analysis-3.7.2/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.653980 scs-analysis-3.7.2/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.667789 scs-analysis-3.7.2/src/scs_analysis/
--rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-08 08:21:13.000000 scs-analysis-3.7.2/src/scs_analysis/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs-analysis-3.7.2/src/scs_analysis/alert.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs-analysis-3.7.2/src/scs_analysis/alert_status.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5970 2024-03-26 13:54:32.000000 scs-analysis-3.7.2/src/scs_analysis/aws_byline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs-analysis-3.7.2/src/scs_analysis/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/aws_mqtt_client.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7121 2024-03-04 12:00:45.000000 scs-analysis-3.7.2/src/scs_analysis/aws_topic_history.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/aws_topic_publisher.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/aws_upload_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    14781 2024-04-03 10:23:16.000000 scs-analysis-3.7.2/src/scs_analysis/baseline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs-analysis-3.7.2/src/scs_analysis/baseline_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.669142 scs-analysis-3.7.2/src/scs_analysis/chart/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/chart/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/chart/chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/chart/histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/chart/multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/chart/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6514 2024-03-13 09:22:10.000000 scs-analysis-3.7.2/src/scs_analysis/client_traffic.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.680314 scs-analysis-3.7.2/src/scs_analysis/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_alert_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4868 2024-03-13 09:22:10.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     4739 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-r--r--   0 bruno      (502) admin       (80)     4798 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     4518 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     2372 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_controller.py
--rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3123 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisations.py
--rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
--rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_gas_density.py
--rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_localize.py
--rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_median.py
--rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_single_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_uds.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5450 2024-04-03 10:23:16.000000 scs-analysis-3.7.2/src/scs_analysis/cognito_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6576 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/cognito_email.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs-analysis-3.7.2/src/scs_analysis/cognito_user_credentials.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8085 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/cognito_user_identity.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/cognito_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7663 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/configuration_csv.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3558 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/configuration_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3947 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/configuration_monitor_check.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4001 2023-12-01 15:39:55.000000 scs-analysis-3.7.2/src/scs_analysis/configuration_report.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/csv_collation_summary.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/csv_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/csv_join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/csv_reader.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/csv_segmentor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs-analysis-3.7.2/src/scs_analysis/csv_writer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs-analysis-3.7.2/src/scs_analysis/device_controller.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs-analysis-3.7.2/src/scs_analysis/device_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs-analysis-3.7.2/src/scs_analysis/device_monitor_status.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.681586 scs-analysis-3.7.2/src/scs_analysis/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/batch_download_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/configuration_csv_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5893 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/mqtt_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/sample_midpoint.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/handler/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/histo_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2127 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/localised_datetime.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/monitor_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/multi_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs-analysis-3.7.2/src/scs_analysis/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/organisation_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/organisation_path_roots.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/organisation_user_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/organisation_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs-analysis-3.7.2/src/scs_analysis/organisations.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs-analysis-3.7.2/src/scs_analysis/sample_aggregate.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_average.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_distance.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_duplicates.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_error.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_gas_concentration.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3561 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_gas_density.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/sample_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs-analysis-3.7.2/src/scs_analysis/sample_iso_8601.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_localize.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_low_pass.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_max.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_median.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_midpoint.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_min.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/sample_noise.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_nullify.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/sample_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs-analysis-3.7.2/src/scs_analysis/sample_slope.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_sort.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_stats.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs-analysis-3.7.2/src/scs_analysis/sample_subset.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/sample_time_shift.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs-analysis-3.7.2/src/scs_analysis/socket_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs-analysis-3.7.2/src/scs_analysis/timer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs-analysis-3.7.2/src/scs_analysis/uds_receiver.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-08 08:21:21.681775 scs-analysis-3.7.2/src/scs_analysis.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-08 08:21:21.000000 scs-analysis-3.7.2/src/scs_analysis.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     6152 2024-04-08 08:21:21.000000 scs-analysis-3.7.2/src/scs_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-08 08:21:21.000000 scs-analysis-3.7.2/src/scs_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-08 08:21:21.000000 scs-analysis-3.7.2/src/scs_analysis.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-08 08:21:21.000000 scs-analysis-3.7.2/src/scs_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.492346 scs-analysis-3.8.0/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs-analysis-3.8.0/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-09 15:14:44.492161 scs-analysis-3.8.0/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-09 15:14:44.492383 scs-analysis-3.8.0/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5533 2024-03-11 10:25:23.000000 scs-analysis-3.8.0/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.466216 scs-analysis-3.8.0/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.479472 scs-analysis-3.8.0/src/scs_analysis/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs-analysis-3.8.0/src/scs_analysis/alert.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs-analysis-3.8.0/src/scs_analysis/alert_status.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6000 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/aws_byline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs-analysis-3.8.0/src/scs_analysis/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/aws_mqtt_client.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7094 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/aws_topic_history.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3339 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/aws_topic_origin.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/aws_topic_publisher.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/aws_upload_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    14774 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/baseline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs-analysis-3.8.0/src/scs_analysis/baseline_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.480764 scs-analysis-3.8.0/src/scs_analysis/chart/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/chart/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/chart/chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/chart/histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/chart/multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/chart/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6514 2024-03-13 09:22:10.000000 scs-analysis-3.8.0/src/scs_analysis/client_traffic.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.490428 scs-analysis-3.8.0/src/scs_analysis/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2478 2024-04-09 15:14:30.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_topic_origin.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4868 2024-03-13 09:22:10.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4739 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4798 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4518 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2372 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3123 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisations.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_localize.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_uds.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5450 2024-04-03 10:23:16.000000 scs-analysis-3.8.0/src/scs_analysis/cognito_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6576 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/cognito_email.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs-analysis-3.8.0/src/scs_analysis/cognito_user_credentials.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8085 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/cognito_user_identity.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/cognito_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7663 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/configuration_csv.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3558 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/configuration_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3947 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/configuration_monitor_check.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4001 2023-12-01 15:39:55.000000 scs-analysis-3.8.0/src/scs_analysis/configuration_report.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/csv_collation_summary.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/csv_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/csv_join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/csv_reader.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/csv_segmentor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs-analysis-3.8.0/src/scs_analysis/csv_writer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs-analysis-3.8.0/src/scs_analysis/device_controller.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs-analysis-3.8.0/src/scs_analysis/device_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs-analysis-3.8.0/src/scs_analysis/device_monitor_status.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.491685 scs-analysis-3.8.0/src/scs_analysis/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/batch_download_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5893 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/mqtt_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/sample_midpoint.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/handler/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/histo_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2127 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/localised_datetime.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/monitor_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/multi_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs-analysis-3.8.0/src/scs_analysis/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/organisation_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/organisation_path_roots.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/organisation_user_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/organisation_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs-analysis-3.8.0/src/scs_analysis/organisations.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs-analysis-3.8.0/src/scs_analysis/sample_aggregate.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_average.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_distance.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_duplicates.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_error.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_gas_concentration.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3561 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_gas_density.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/sample_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs-analysis-3.8.0/src/scs_analysis/sample_iso_8601.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_localize.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_low_pass.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_max.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_median.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_midpoint.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_min.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/sample_noise.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_nullify.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/sample_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs-analysis-3.8.0/src/scs_analysis/sample_slope.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_sort.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_stats.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs-analysis-3.8.0/src/scs_analysis/sample_subset.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/sample_time_shift.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs-analysis-3.8.0/src/scs_analysis/socket_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs-analysis-3.8.0/src/scs_analysis/timer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs-analysis-3.8.0/src/scs_analysis/uds_receiver.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:14:44.491871 scs-analysis-3.8.0/src/scs_analysis.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-09 15:14:44.000000 scs-analysis-3.8.0/src/scs_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-09 15:14:44.000000 scs-analysis-3.8.0/src/scs_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-09 15:14:44.000000 scs-analysis-3.8.0/src/scs_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-09 15:14:44.000000 scs-analysis-3.8.0/src/scs_analysis.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-09 15:14:44.000000 scs-analysis-3.8.0/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-3.7.2/LICENSE` & `scs-analysis-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/PKG-INFO` & `scs-analysis-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.7.2
+Version: 3.8.0
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.11.4
+Requires-Dist: scs-core~=3.12.0
 Requires-Dist: scs-host-posix~=3.3.0
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
```

### Comparing `scs-analysis-3.7.2/README.md` & `scs-analysis-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/setup.py` & `scs-analysis-3.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/alert.py` & `scs-analysis-3.8.0/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/alert_status.py` & `scs-analysis-3.8.0/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_byline.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_byline.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 {"device": "scs-bgx-401", "topic": "south-coast-science-demo/brighton/loc/1/climate",
 "lastSeenTime": "2020-10-23T08:52:20Z", "last_write": "2020-10-23T08:52:20Z",
 "message": "{\"val\": {\"hmd\": 68.4, \"tmp\": 19.8, \"bar\": null}, \"rec\": \"2020-10-23T08:52:20Z\",
 \"tag\": \"scs-bgx-401\"}"}
 
 SEE ALSO
 scs_analysis/aws_topic_history
+scs_analysis/aws_topic_origin
 scs_analysis/cognito_user_credentials
 
 scs_lambda/aws_message_delete
 """
 
 import sys
```

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_client_auth.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_topic_history.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_topic_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,25 @@
 {"device": "scs-bbe-401", "topic": "south-coast-science-demo/brighton/loc/1/climate", "upload": "2019-01-11T12:15:36Z",
 "payload": {"val": {"hmd": 68.4, "tmp": 12.3}, "rec": "2019-01-11T12:15:36Z", "tag": "scs-bgx-401"}}
 
 {"val": {"hmd": 68.4, "tmp": 12.3}, "rec": "2019-01-11T12:15:36Z", "tag": "scs-bgx-401"}
 
 SEE ALSO
 scs_analysis/aws_byline
+scs_analysis/aws_topic_origin
 scs_analysis/cognito_user_credentials
 """
 
 import sys
 
 from scs_analysis.cmd.cmd_aws_topic_history import CmdAWSTopicHistory
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
 from scs_core.aws.manager.byline.byline_finder import BylineFinder
-from scs_core.aws.manager.topic_history.topic_history_manager import TopicHistoryManager
+from scs_core.aws.manager.topic_history.topic_history_finder import TopicHistoryFinder
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
 
@@ -129,15 +130,15 @@
         # resources...
 
         # BylineFinder...
         byline_finder = BylineFinder()
 
         # MessageManager...
         reporter = BatchDownloadReporter()
-        message_manager = TopicHistoryManager(reporter=reporter)
+        finder = TopicHistoryFinder(reporter=reporter)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # check...
 
         if not Network.is_available():
             logger.info("waiting for network")
@@ -146,16 +147,16 @@
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         start_time = LocalizedDatetime.now()
 
         if cmd.latest_at:
-            message = message_manager.find_latest_for_topic(auth.id_token, cmd.topic, cmd.latest_at, None,
-                                                            cmd.include_wrapper, cmd.rec_only, None)
+            message = finder.find_latest_for_topic(auth.id_token, cmd.topic, cmd.latest_at, None,
+                                                   cmd.include_wrapper, cmd.rec_only, None)
 
             if message:
                 print(JSONify.dumps(message))
 
             exit(0)
 
         # start / end times...
@@ -176,17 +177,17 @@
             end = LocalizedDatetime.now() if cmd.end is None else cmd.end
             start = cmd.start
 
         logger.info("start: %s" % start)
         logger.info("end: %s" % end)
 
         # messages...
-        for message in message_manager.find_for_topic(auth.id_token, cmd.topic, start, end, None, cmd.fetch_last,
-                                                      cmd.checkpoint, cmd.include_wrapper, cmd.rec_only, cmd.min_max,
-                                                      cmd.exclude_remainder, False, None):
+        for message in finder.find_for_topic(auth.id_token, cmd.topic, start, end, None, cmd.fetch_last,
+                                             cmd.checkpoint, cmd.include_wrapper, cmd.rec_only, cmd.min_max,
+                                             cmd.exclude_remainder, False, None):
             print(JSONify.dumps(message))
             sys.stdout.flush()
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
```

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-3.8.0/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/baseline.py` & `scs-analysis-3.8.0/src/scs_analysis/baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from scs_analysis.cmd.cmd_baseline import CmdBaseline
 
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
 from scs_core.aws.client.device_control_client import DeviceControlClient
 
 from scs_core.aws.manager.byline.byline_finder import BylineFinder
-from scs_core.aws.manager.topic_history.topic_history_manager import TopicHistoryManager
+from scs_core.aws.manager.topic_history.topic_history_finder import TopicHistoryFinder
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.client.http_exception import HTTPGatewayTimeoutException
 
 from scs_core.data.datetime import LocalizedDatetime
@@ -143,15 +143,15 @@
         # resources...
 
         # BylineFinder...
         reporter = BatchDownloadReporter()
         byline_finder = BylineFinder(reporter=reporter)
 
         # MessageManager...
-        message_manager = TopicHistoryManager(reporter=reporter)
+        history_finder = TopicHistoryFinder(reporter=reporter)
 
         # DeviceControlClient...
         client = DeviceControlClient()
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
@@ -264,17 +264,17 @@
                 if end > now:
                     start -= Timedelta(days=1)
                     end -= Timedelta(days=1)
                     logger.error("WARNING: testing previous day...")
 
                 logger.info("start: %s end: %s" % (start.as_iso8601(), end.as_iso8601()))
 
-                data = list(message_manager.find_for_topic(auth.id_token, gases_topic, start, end,
-                                                           None, False, baseline_conf.checkpoint(),
-                                                           False, False, False, False, False, None))
+                data = list(history_finder.find_for_topic(auth.id_token, gases_topic, start, end,
+                                                          None, False, baseline_conf.checkpoint(),
+                                                          False, False, False, False, False, None))
 
                 if not data:
                     logger.error("no data found for %s." % gases_topic)
                     continue
 
                 logger.info("expected: %s retrieved: %s" % (baseline_conf.expected_data_points(start, end), len(data)))
                 logger.info("-")
```

### Comparing `scs-analysis-3.7.2/src/scs_analysis/baseline_conf.py` & `scs-analysis-3.8.0/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/chart/chart.py` & `scs-analysis-3.8.0/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/chart/single_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/client_traffic.py` & `scs-analysis-3.8.0/src/scs_analysis/client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_client_traffic.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_configuration_report.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_controller.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_gas_concentration.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_gas_density.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_localize.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_single_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cmd/cmd_uds.py` & `scs-analysis-3.8.0/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cognito_devices.py` & `scs-analysis-3.8.0/src/scs_analysis/cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cognito_email.py` & `scs-analysis-3.8.0/src/scs_analysis/cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cognito_user_credentials.py` & `scs-analysis-3.8.0/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-3.8.0/src/scs_analysis/cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/cognito_users.py` & `scs-analysis-3.8.0/src/scs_analysis/cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/configuration_csv.py` & `scs-analysis-3.8.0/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/configuration_monitor.py` & `scs-analysis-3.8.0/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-3.8.0/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/configuration_report.py` & `scs-analysis-3.8.0/src/scs_analysis/configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_collator.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_join.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_reader.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_segmentor.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/csv_writer.py` & `scs-analysis-3.8.0/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/device_controller.py` & `scs-analysis-3.8.0/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/device_monitor.py` & `scs-analysis-3.8.0/src/scs_analysis/device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/device_monitor_status.py` & `scs-analysis-3.8.0/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/mqtt_reporter.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/handler/sample_regression.py` & `scs-analysis-3.8.0/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/histo_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/localised_datetime.py` & `scs-analysis-3.8.0/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/monitor_auth.py` & `scs-analysis-3.8.0/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/multi_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/node.py` & `scs-analysis-3.8.0/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/organisation_devices.py` & `scs-analysis-3.8.0/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-3.8.0/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-3.8.0/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/organisation_users.py` & `scs-analysis-3.8.0/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/organisations.py` & `scs-analysis-3.8.0/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_aggregate.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_average.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_collator.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_distance.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_duplicates.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_error.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_gas_concentration.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_gas_density.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_interval.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_localize.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_low_pass.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_max.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_median.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_midpoint.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_min.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_noise.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_nullify.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_paths.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_regression.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_slope.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_sort.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_stats.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_subset.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/sample_time_shift.py` & `scs-analysis-3.8.0/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/single_chart.py` & `scs-analysis-3.8.0/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/socket_receiver.py` & `scs-analysis-3.8.0/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/timer.py` & `scs-analysis-3.8.0/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis/uds_receiver.py` & `scs-analysis-3.8.0/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.7.2/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-3.8.0/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.7.2
+Version: 3.8.0
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.11.4
+Requires-Dist: scs-core~=3.12.0
 Requires-Dist: scs-host-posix~=3.3.0
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
```

### Comparing `scs-analysis-3.7.2/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-3.8.0/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/scs_analysis/__init__.py
 src/scs_analysis/alert.py
 src/scs_analysis/alert_status.py
 src/scs_analysis/aws_byline.py
 src/scs_analysis/aws_client_auth.py
 src/scs_analysis/aws_mqtt_client.py
 src/scs_analysis/aws_topic_history.py
+src/scs_analysis/aws_topic_origin.py
 src/scs_analysis/aws_topic_publisher.py
 src/scs_analysis/aws_upload_interval.py
 src/scs_analysis/baseline.py
 src/scs_analysis/baseline_conf.py
 src/scs_analysis/client_traffic.py
 src/scs_analysis/cognito_devices.py
 src/scs_analysis/cognito_email.py
@@ -85,14 +86,15 @@
 src/scs_analysis/chart/single_chart.py
 src/scs_analysis/cmd/__init__.py
 src/scs_analysis/cmd/cmd_alert.py
 src/scs_analysis/cmd/cmd_alert_status.py
 src/scs_analysis/cmd/cmd_aws_byline.py
 src/scs_analysis/cmd/cmd_aws_client_auth.py
 src/scs_analysis/cmd/cmd_aws_topic_history.py
+src/scs_analysis/cmd/cmd_aws_topic_origin.py
 src/scs_analysis/cmd/cmd_aws_topic_publisher.py
 src/scs_analysis/cmd/cmd_baseline.py
 src/scs_analysis/cmd/cmd_baseline_conf.py
 src/scs_analysis/cmd/cmd_client_traffic.py
 src/scs_analysis/cmd/cmd_cognito_devices.py
 src/scs_analysis/cmd/cmd_cognito_email.py
 src/scs_analysis/cmd/cmd_cognito_user_credentials.py
```

