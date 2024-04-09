# Comparing `tmp/avtomat_aws-0.1.4.tar.gz` & `tmp/avtomat_aws-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.1.4.tar", max compression
+gzip compressed data, was "avtomat_aws-0.2.0.tar", max compression
```

## Comparing `avtomat_aws-0.1.4.tar` & `avtomat_aws-0.2.0.tar`

### file list

```diff
@@ -1,120 +1,125 @@
--rw-r--r--   0        0        0     1002 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/LICENSE
--rw-r--r--   0        0        0     3838 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/README.md
--rw-r--r--   0        0        0       69 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      864 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      928 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1156 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1145 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1300 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      711 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/create_snapshots.py
--rw-r--r--   0        0        0      855 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0      718 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      688 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      834 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      513 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      522 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1244 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1410 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      675 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1442 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1203 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      522 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1389 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      960 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      884 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1251 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1131 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      824 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      887 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      791 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      781 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      509 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      732 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      763 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      766 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      746 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1262 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1364 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      583 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     4829 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1242 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      895 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1225 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1365 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      462 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      789 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      615 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/__init__.py
--rw-r--r--   0        0        0      203 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/set_output.py
--rw-r--r--   0        0        0     2083 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/cli/table.py
--rw-r--r--   0        0        0      288 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2636 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      728 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-08 10:24:55.399010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3420 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3289 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1099 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2625 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     1988 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/create_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0     1532 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     3012 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3662 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3330 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5192 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     3322 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4818 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3514 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      497 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1743 2024-04-08 10:24:55.403010 avtomat_aws-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1285 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/README.md
+-rw-r--r--   0        0        0       69 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.499914 avtomat_aws-0.2.0/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      864 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      928 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1156 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1145 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1300 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      874 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_images.py
+-rw-r--r--   0        0        0      711 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      855 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0     1020 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_instances.py
+-rw-r--r--   0        0        0      718 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      688 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      834 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      513 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      522 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1244 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1410 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      675 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1442 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1203 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      522 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1389 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      960 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      884 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1251 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1131 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      824 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      887 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      791 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      781 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      509 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      732 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      763 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      766 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      746 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1262 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1364 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      583 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     4829 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1242 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      895 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1225 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1418 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      462 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/set_output.py
+-rw-r--r--   0        0        0     2083 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/cli/table.py
+-rw-r--r--   0        0        0      858 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/format_tags.py
+-rw-r--r--   0        0        0      288 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2821 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3420 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3289 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1187 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     2512 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_images.py
+-rw-r--r--   0        0        0     1988 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0    11038 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_instances.py
+-rw-r--r--   0        0        0     1532 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     3012 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3599 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3330 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5204 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4403 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-09 20:01:33.503914 avtomat_aws-0.2.0/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3514 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-09 20:01:33.507914 avtomat_aws-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.2.0/PKG-INFO
```

### Comparing `avtomat_aws-0.1.4/LICENSE` & `avtomat_aws-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/README.md` & `avtomat_aws-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/create_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_active_regions.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/main.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/services.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,18 @@
     "cloudtrail": [
         "discover_user_events",
         "discover_resource_events",
         "discover_events",
     ],
     "ec2": [
         "copy_snapshots",
+        "create_images",
         "create_snapshots",
         "delete_images",
+        "delete_instances",
         "delete_security_groups",
         "delete_snapshots",
         "delete_volumes",
         "discover_active_regions",
         "discover_default_ebs_encryption",
         "discover_images",
         "discover_instances",
```

### Comparing `avtomat_aws-0.1.4/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.2.0/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.2.0/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.2.0/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.2.0/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/helpers/cli/table.py` & `avtomat_aws-0.2.0/avtomat_aws/helpers/cli/table.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.2.0/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.2.0/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.2.0/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.2.0/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.2.0/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .copy_snapshots import copy_snapshots
+from .create_images import create_images
 from .create_snapshots import create_snapshots
 from .delete_images import delete_images
+from .delete_instances import delete_instances
 from .delete_security_groups import delete_security_groups
 from .delete_snapshots import delete_snapshots
 from .delete_volumes import delete_volumes
 from .discover_active_regions import discover_active_regions
 from .discover_default_ebs_encryption import discover_default_ebs_encryption
 from .discover_images import discover_images
 from .discover_instances import discover_instances
```

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/create_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/create_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_instances.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from avtomat_aws.decorators.authenticate import authenticate
 from avtomat_aws.decorators.set_logger import set_logger
 from avtomat_aws.decorators.validate import validate
+from avtomat_aws.helpers.format_tags import format_tags
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "states": ["running", "stopped", "pending", "stopping"],
     "tags": [],
@@ -74,22 +75,20 @@
     instance_ids = kwargs.get("instance_ids")
 
     filters = []
     filters.append({"Name": "instance-state-name", "Values": states})
 
     if tags:
         logger.debug(f"Filtering for tags: {tags}")
-        for tag in tags:
-            parsed_tag = parse_tag(tag)
-            if parsed_tag[1]:
-                filters.append(
-                    {"Name": f"tag:{parsed_tag[0]}", "Values": [parsed_tag[1]]}
-                )
+        formatted_tags = format_tags(tags)
+        for tag in formatted_tags:
+            if tag.get("Key") and tag.get("Value"):
+                filters.append({"Name": f"tag:{tag['Key']}", "Values": [tag["Value"]]})
             else:
-                filters.append({"Name": "tag-key", "Values": [parsed_tag[0]]})
+                filters.append({"Name": "tag-key", "Values": [tag["Key"]]})
 
     if public:
         logger.debug("Filtering for public instances")
         filters.append({"Name": "ip-address", "Values": ["*"]})
 
     if instance_ids:
         logger.debug(f"Filtering for instances: {instance_ids}")
@@ -114,14 +113,7 @@
         response = session_objects["ec2_resource"].instances.filter(
             Filters=windows_filters, InstanceIds=kwargs["instance_ids"]
         )
         windows_instances = [instance.id for instance in response]
         instances = [id for id in instances if id not in windows_instances]
 
     return instances
-
-
-def parse_tag(tag):
-    if "=" in tag:
-        return tag.split("=", 1)
-    else:
-        return tag, None
```

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from avtomat_aws.decorators.authenticate import authenticate
 from avtomat_aws.decorators.set_logger import set_logger
 from avtomat_aws.decorators.validate import validate
+from avtomat_aws.helpers.format_tags import format_tags
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "existing": False,
     "missing": False,
@@ -46,66 +47,58 @@
 def discover_tags(**kwargs):
     """Discover specific tags that exist on EC2 resources"""
 
     # Required parameters
     resource_types = kwargs.pop("resource_types")
     tags = kwargs.pop("tags")
 
-    # Convert 'tags' from ['Key=Value', 'Key', ...] format to a list of tuples [(Key, Value), (Key, None), ...]
-    tag_tuples = []
-    for tag in tags:
-        if "=" in tag:
-            key, value = tag.split("=", 1)
-            tag_tuples.append((key, value))
-        else:
-            tag_tuples.append((tag, None))
-
     session_objects = set_session_objects(
         kwargs["session"], resources=["ec2"], region=kwargs["region"]
     )
 
     if kwargs.get("existing"):
         logger.info(f"Discovering resources with tags: {tags}")
     elif kwargs.get("missing"):
         logger.info(f"Discovering resources without tags: {tags}")
 
+    formatted_tags = format_tags(tags)
     resources = []
     if "image" in resource_types:
         response = session_objects["ec2_resource"].images.filter(Owners=["self"])
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "instance" in resource_types:
         response = session_objects["ec2_resource"].instances.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "internet_gateway" in resource_types:
         response = session_objects["ec2_resource"].internet_gateways.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "key_pair" in resource_types:
         response = session_objects["ec2_resource"].key_pairs.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "network_acl" in resource_types:
         response = session_objects["ec2_resource"].network_acls.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "route_table" in resource_types:
         response = session_objects["ec2_resource"].route_tables.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "security_group" in resource_types:
         response = session_objects["ec2_resource"].security_groups.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "snapshot" in resource_types:
         response = session_objects["ec2_resource"].snapshots.filter(OwnerIds=["self"])
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "subnet" in resource_types:
         response = session_objects["ec2_resource"].subnets.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "volume" in resource_types:
         response = session_objects["ec2_resource"].volumes.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
     if "vpc" in resource_types:
         response = session_objects["ec2_resource"].vpcs.all()
-        resources.extend(search_collections(response, tag_tuples, **kwargs))
+        resources.extend(search_collections(response, formatted_tags, **kwargs))
 
     logger.info(f"{len(resources)} resources found")
     logger.debug(resources)
 
     return resources
 
 
@@ -122,24 +115,31 @@
             for tag in getattr(resource, "tags") or []
         }
         match = False
 
         if missing:
             match = any(
                 (
-                    key not in resource_tags
-                    or (value is not None and resource_tags[key] != value)
+                    tag["Key"] not in resource_tags
+                    or (
+                        tag.get("Value") is not None
+                        and resource_tags[tag["Key"]] != tag["Value"]
+                    )
                 )
-                for key, value in tags
+                for tag in tags
             )
 
         elif existing:
             match = all(
-                key in resource_tags and (value is None or resource_tags[key] == value)
-                for key, value in tags
+                tag["Key"] in resource_tags
+                and (
+                    tag.get("Value") is None
+                    or resource_tags[tag["Key"]] == tag["Value"]
+                )
+                for tag in tags
             )
 
         if match:
             try:
                 resources.append(resource.id)
             except AttributeError:
                 resources.append(resource.name)
```

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from avtomat_aws.decorators.authenticate import authenticate
 from avtomat_aws.decorators.set_logger import set_logger
 from avtomat_aws.decorators.validate import validate
+from avtomat_aws.helpers.format_tags import format_tags
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "create": False,
     "delete": False,
@@ -23,54 +24,41 @@
 
 @validate(DEFAULTS, RULES)
 @set_logger()
 @authenticate()
 def modify_tags(**kwargs):
     """Create or delete tags for EC2 resources"""
 
-    if not kwargs.get("delete"):
-        for tag in kwargs["tags"]:
-            if "=" not in tag:
-                raise ValueError(
-                    f"Tag '{tag}' not in Key=Value format."
-                )  # Needs a validation rule
-
-    # Change tags into the correct format
-    # Needs better handling
-    formatted_tags = []
-    for tag in kwargs["tags"]:
-        if "=" in tag:
-            key, value = tag.split("=", 1)
-            formatted_tags.append({"Key": key, "Value": value})
-        else:
-            key = tag
-            formatted_tags.append({"Key": key})
-    kwargs["tags"] = formatted_tags
-
     # Required parameters
     resource_ids = kwargs.pop("resource_ids")
     tags = kwargs.pop("tags")
 
     if not resource_ids:
         logger.info("No resources to modify tags for")
         return []
 
     session_objects = set_session_objects(
         kwargs["session"], clients=["ec2"], region=kwargs["region"]
     )
 
     if kwargs.get("create"):
+        formatted_tags = format_tags(tags, creation=True)
         logger.info(f"Creating tags for resources")
-    elif kwargs.get("delete"):
+    else:
+        formatted_tags = format_tags(tags)
         logger.info(f"Deleting tags for resources")
 
     if kwargs.get("dynamic_tags"):
-        failed_resources = dynamic_tags(tags, resource_ids, session_objects, **kwargs)
+        failed_resources = dynamic_tags(
+            formatted_tags, resource_ids, session_objects, **kwargs
+        )
     else:
-        failed_resources = static_tags(tags, resource_ids, session_objects, **kwargs)
+        failed_resources = static_tags(
+            formatted_tags, resource_ids, session_objects, **kwargs
+        )
 
     if failed_resources:
         logger.info(f"{len(failed_resources)} resources failed tag modification")
     else:
         logger.info("Success")
     logger.debug(failed_resources)
```

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.2.0/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.2.0/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.2.0/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.2.0/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.2.0/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.2.0/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/avtomat_aws/validations/rules.py` & `avtomat_aws-0.2.0/avtomat_aws/validations/rules.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.1.4/pyproject.toml` & `avtomat_aws-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.1.4"
+version = "0.2.0"
 description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.1.4/PKG-INFO` & `avtomat_aws-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.1.4
+Version: 0.2.0
 Summary: A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.4 Summary: A collection of
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.2.0 Summary: A collection of
 reusable Amazon Web Services actions, bringing speed and certainty to cloud
 operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

