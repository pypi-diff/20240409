# Comparing `tmp/genericsuite-0.1.2.tar.gz` & `tmp/genericsuite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericsuite-0.1.2.tar", max compression
+gzip compressed data, was "genericsuite-0.1.3.tar", max compression
```

## Comparing `genericsuite-0.1.2.tar` & `genericsuite-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      747 2024-03-31 23:36:29.408323 genericsuite-0.1.2/LICENSE
--rw-r--r--   0        0        0    12258 2024-03-31 23:43:26.985724 genericsuite-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-03 23:49:07.732831 genericsuite-0.1.2/genericsuite/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:14.702977 genericsuite-0.1.2/genericsuite/chalicelib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 11:10:05.850616 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/__init__.py
--rw-r--r--   0        0        0     1096 2024-02-24 02:22:20.582188 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/menu_options.py
--rw-r--r--   0        0        0     2125 2024-02-24 02:14:13.742858 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/users.py
--rw-r--r--   0        0        0     1482 2024-02-24 13:33:20.978316 genericsuite-0.1.2/genericsuite/chalicelib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:25.905045 genericsuite-0.1.2/genericsuite/chalicelib/util/__init__.py
--rw-r--r--   0        0        0     2751 2024-02-26 13:41:07.446923 genericsuite-0.1.2/genericsuite/chalicelib/util/create_app.py
--rw-r--r--   0        0        0     4647 2024-02-25 17:57:02.422438 genericsuite-0.1.2/genericsuite/chalicelib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.378538 genericsuite-0.1.2/genericsuite/config/__init__.py
--rw-r--r--   0        0        0     4443 2024-03-01 12:22:13.763424 genericsuite-0.1.2/genericsuite/config/config.py
--rw-r--r--   0        0        0     4683 2024-03-01 00:12:35.189298 genericsuite-0.1.2/genericsuite/config/config_from_db.py
--rw-r--r--   0        0        0      609 2024-02-18 20:15:35.895205 genericsuite-0.1.2/genericsuite/config/logging.conf.yml
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.895273 genericsuite-0.1.2/genericsuite/constants/__init__.py
--rw-r--r--   0        0        0     1443 2024-02-23 00:45:12.985504 genericsuite-0.1.2/genericsuite/constants/const_tables.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:32.204369 genericsuite-0.1.2/genericsuite/fastapilib/__init__.py
--rw-r--r--   0        0        0     1455 2024-02-24 13:33:13.552960 genericsuite-0.1.2/genericsuite/fastapilib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:35.347602 genericsuite-0.1.2/genericsuite/fastapilib/util/__init__.py
--rw-r--r--   0        0        0     1307 2024-02-18 20:15:35.911504 genericsuite-0.1.2/genericsuite/fastapilib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:50.817726 genericsuite-0.1.2/genericsuite/flasklib/__init__.py
--rw-r--r--   0        0        0     1708 2024-02-24 13:34:01.565559 genericsuite-0.1.2/genericsuite/flasklib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:42.207235 genericsuite-0.1.2/genericsuite/flasklib/util/__init__.py
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.903766 genericsuite-0.1.2/genericsuite/models/billing/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 02:47:22.334682 genericsuite-0.1.2/genericsuite/models/billing/billing_utilities.py
--rw-r--r--   0        0        0        0 2023-07-17 02:15:00.638430 genericsuite-0.1.2/genericsuite/models/menu_options/__init__.py
--rw-r--r--   0        0        0     2840 2024-02-24 02:14:13.741348 genericsuite-0.1.2/genericsuite/models/menu_options/menu_options.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.379886 genericsuite-0.1.2/genericsuite/models/users/__init__.py
--rw-r--r--   0        0        0     8650 2024-02-25 16:04:51.338589 genericsuite-0.1.2/genericsuite/models/users/users.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.380476 genericsuite-0.1.2/genericsuite/util/__init__.py
--rw-r--r--   0        0        0     5898 2024-02-29 11:32:04.042270 genericsuite-0.1.2/genericsuite/util/app_context.py
--rw-r--r--   0        0        0     1608 2024-02-23 01:37:50.489847 genericsuite-0.1.2/genericsuite/util/app_logger.py
--rw-r--r--   0        0        0     7160 2024-02-23 00:45:13.028977 genericsuite-0.1.2/genericsuite/util/aws.py
--rw-r--r--   0        0        0     4319 2024-02-23 00:45:12.989787 genericsuite-0.1.2/genericsuite/util/blueprint_one.py
--rw-r--r--   0        0        0     1797 2024-02-23 10:56:31.242663 genericsuite-0.1.2/genericsuite/util/config_dbdef_helpers.py
--rw-r--r--   0        0        0     1387 2024-02-27 16:04:59.642735 genericsuite-0.1.2/genericsuite/util/current_user_data.py
--rw-r--r--   0        0        0     4972 2024-03-02 04:46:29.973118 genericsuite-0.1.2/genericsuite/util/datetime_utilities.py
--rw-r--r--   0        0        0    35651 2024-02-25 15:25:41.529780 genericsuite-0.1.2/genericsuite/util/db_abstractor.py
--rw-r--r--   0        0        0      807 2024-02-21 16:28:35.421102 genericsuite-0.1.2/genericsuite/util/exceptions.py
--rw-r--r--   0        0        0     2287 2024-02-24 13:40:02.416560 genericsuite-0.1.2/genericsuite/util/framework_abs_layer.py
--rw-r--r--   0        0        0    47797 2024-02-25 17:57:22.042814 genericsuite-0.1.2/genericsuite/util/generic_db_helpers.py
--rw-r--r--   0        0        0     5889 2024-02-25 12:47:46.514099 genericsuite-0.1.2/genericsuite/util/generic_db_middleware.py
--rw-r--r--   0        0        0    10325 2024-02-27 16:04:16.316160 genericsuite-0.1.2/genericsuite/util/generic_endpoint_helpers.py
--rw-r--r--   0        0        0     5372 2024-02-26 14:01:45.304576 genericsuite-0.1.2/genericsuite/util/jwt.py
--rw-r--r--   0        0        0     3216 2024-02-23 00:45:13.032873 genericsuite-0.1.2/genericsuite/util/nav_helpers.py
--rw-r--r--   0        0        0     4421 2024-02-23 00:45:13.039348 genericsuite-0.1.2/genericsuite/util/parse_multipart.py
--rw-r--r--   0        0        0     1818 2024-02-23 01:37:50.488701 genericsuite-0.1.2/genericsuite/util/passwords.py
--rw-r--r--   0        0        0      585 2024-02-18 20:15:35.910549 genericsuite-0.1.2/genericsuite/util/request_handler.py
--rw-r--r--   0        0        0     6568 2024-02-23 00:45:13.032854 genericsuite-0.1.2/genericsuite/util/security.py
--rw-r--r--   0        0        0     3318 2024-02-25 11:52:22.059881 genericsuite-0.1.2/genericsuite/util/send_email.py
--rw-r--r--   0        0        0    16009 2024-03-02 15:00:06.343708 genericsuite-0.1.2/genericsuite/util/utilities.py
--rw-r--r--   0        0        0     1429 2024-04-02 13:49:21.876653 genericsuite-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    13455 1970-01-01 00:00:00.000000 genericsuite-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-03-31 23:36:29.408323 genericsuite-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12258 2024-04-09 13:09:49.814521 genericsuite-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 23:49:07.732831 genericsuite-0.1.3/genericsuite/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:14.702977 genericsuite-0.1.3/genericsuite/chalicelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 11:10:05.850616 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/__init__.py
+-rw-r--r--   0        0        0     1096 2024-02-24 02:22:20.582188 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/menu_options.py
+-rw-r--r--   0        0        0     2125 2024-02-24 02:14:13.742858 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/users.py
+-rw-r--r--   0        0        0     1482 2024-02-24 13:33:20.978316 genericsuite-0.1.3/genericsuite/chalicelib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:25.905045 genericsuite-0.1.3/genericsuite/chalicelib/util/__init__.py
+-rw-r--r--   0        0        0     2751 2024-02-26 13:41:07.446923 genericsuite-0.1.3/genericsuite/chalicelib/util/create_app.py
+-rw-r--r--   0        0        0     4647 2024-02-25 17:57:02.422438 genericsuite-0.1.3/genericsuite/chalicelib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.378538 genericsuite-0.1.3/genericsuite/config/__init__.py
+-rw-r--r--   0        0        0     4304 2024-04-09 13:08:35.964005 genericsuite-0.1.3/genericsuite/config/config.py
+-rw-r--r--   0        0        0     4646 2024-04-09 13:08:13.620684 genericsuite-0.1.3/genericsuite/config/config_from_db.py
+-rw-r--r--   0        0        0      609 2024-02-18 20:15:35.895205 genericsuite-0.1.3/genericsuite/config/logging.conf.yml
+-rw-r--r--   0        0        0        0 2024-02-18 20:15:35.895273 genericsuite-0.1.3/genericsuite/constants/__init__.py
+-rw-r--r--   0        0        0     1443 2024-02-23 00:45:12.985504 genericsuite-0.1.3/genericsuite/constants/const_tables.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:32.204369 genericsuite-0.1.3/genericsuite/fastapilib/__init__.py
+-rw-r--r--   0        0        0     1455 2024-02-24 13:33:13.552960 genericsuite-0.1.3/genericsuite/fastapilib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:35.347602 genericsuite-0.1.3/genericsuite/fastapilib/util/__init__.py
+-rw-r--r--   0        0        0     1307 2024-02-18 20:15:35.911504 genericsuite-0.1.3/genericsuite/fastapilib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:50.817726 genericsuite-0.1.3/genericsuite/flasklib/__init__.py
+-rw-r--r--   0        0        0     1708 2024-02-24 13:34:01.565559 genericsuite-0.1.3/genericsuite/flasklib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:42.207235 genericsuite-0.1.3/genericsuite/flasklib/util/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-18 20:15:35.903766 genericsuite-0.1.3/genericsuite/models/billing/__init__.py
+-rw-r--r--   0        0        0     1419 2024-03-03 02:47:22.334682 genericsuite-0.1.3/genericsuite/models/billing/billing_utilities.py
+-rw-r--r--   0        0        0        0 2023-07-17 02:15:00.638430 genericsuite-0.1.3/genericsuite/models/menu_options/__init__.py
+-rw-r--r--   0        0        0     2840 2024-02-24 02:14:13.741348 genericsuite-0.1.3/genericsuite/models/menu_options/menu_options.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.379886 genericsuite-0.1.3/genericsuite/models/users/__init__.py
+-rw-r--r--   0        0        0     8650 2024-02-25 16:04:51.338589 genericsuite-0.1.3/genericsuite/models/users/users.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.380476 genericsuite-0.1.3/genericsuite/util/__init__.py
+-rw-r--r--   0        0        0     5898 2024-02-29 11:32:04.042270 genericsuite-0.1.3/genericsuite/util/app_context.py
+-rw-r--r--   0        0        0     1608 2024-02-23 01:37:50.489847 genericsuite-0.1.3/genericsuite/util/app_logger.py
+-rw-r--r--   0        0        0     7160 2024-02-23 00:45:13.028977 genericsuite-0.1.3/genericsuite/util/aws.py
+-rw-r--r--   0        0        0     4456 2024-04-09 12:56:04.586894 genericsuite-0.1.3/genericsuite/util/blueprint_one.py
+-rw-r--r--   0        0        0     1797 2024-02-23 10:56:31.242663 genericsuite-0.1.3/genericsuite/util/config_dbdef_helpers.py
+-rw-r--r--   0        0        0     1387 2024-02-27 16:04:59.642735 genericsuite-0.1.3/genericsuite/util/current_user_data.py
+-rw-r--r--   0        0        0     4972 2024-03-02 04:46:29.973118 genericsuite-0.1.3/genericsuite/util/datetime_utilities.py
+-rw-r--r--   0        0        0    35651 2024-02-25 15:25:41.529780 genericsuite-0.1.3/genericsuite/util/db_abstractor.py
+-rw-r--r--   0        0        0      807 2024-02-21 16:28:35.421102 genericsuite-0.1.3/genericsuite/util/exceptions.py
+-rw-r--r--   0        0        0     2287 2024-02-24 13:40:02.416560 genericsuite-0.1.3/genericsuite/util/framework_abs_layer.py
+-rw-r--r--   0        0        0    47797 2024-02-25 17:57:22.042814 genericsuite-0.1.3/genericsuite/util/generic_db_helpers.py
+-rw-r--r--   0        0        0     5889 2024-02-25 12:47:46.514099 genericsuite-0.1.3/genericsuite/util/generic_db_middleware.py
+-rw-r--r--   0        0        0    10325 2024-02-27 16:04:16.316160 genericsuite-0.1.3/genericsuite/util/generic_endpoint_helpers.py
+-rw-r--r--   0        0        0     4472 2024-04-09 12:10:28.048429 genericsuite-0.1.3/genericsuite/util/jwt.py
+-rw-r--r--   0        0        0     3216 2024-02-23 00:45:13.032873 genericsuite-0.1.3/genericsuite/util/nav_helpers.py
+-rw-r--r--   0        0        0     4421 2024-02-23 00:45:13.039348 genericsuite-0.1.3/genericsuite/util/parse_multipart.py
+-rw-r--r--   0        0        0     1818 2024-02-23 01:37:50.488701 genericsuite-0.1.3/genericsuite/util/passwords.py
+-rw-r--r--   0        0        0      585 2024-02-18 20:15:35.910549 genericsuite-0.1.3/genericsuite/util/request_handler.py
+-rw-r--r--   0        0        0     6568 2024-02-23 00:45:13.032854 genericsuite-0.1.3/genericsuite/util/security.py
+-rw-r--r--   0        0        0     3318 2024-02-25 11:52:22.059881 genericsuite-0.1.3/genericsuite/util/send_email.py
+-rw-r--r--   0        0        0    16009 2024-03-02 15:00:06.343708 genericsuite-0.1.3/genericsuite/util/utilities.py
+-rw-r--r--   0        0        0     1429 2024-04-09 13:15:41.911453 genericsuite-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    13455 1970-01-01 00:00:00.000000 genericsuite-0.1.3/PKG-INFO
```

### Comparing `genericsuite-0.1.2/LICENSE` & `genericsuite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/README.md` & `genericsuite-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # The GenericSuite for Python (backend version)
 
 ![GenericSuite Logo](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/lib/images/gs_logo_circle.png)
 
-GenericSuite is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including Chalice, FastAPI, and Flask, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
+[GenericSuite](https://www.carlosjramirez.com/genericsuite) is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including FastAPI, Flask and Chalice, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
 
 ## Features
 
-- **Framework Agnostic**: Supports Chalice, FastAPI, and Flask frameworks.
+- **Framework Agnostic**: Supports FastAPI, Flask, and Chalice frameworks.
 - **Database Support**: Includes abstracted database operations for both MongoDB and DynamoDB, offering flexibility in choosing the database.
 - **Authentication**: Implements JWT-based authentication, providing secure access to endpoints.
 - **Dynamic Endpoint Creation**: Allows for defining endpoints dynamically through JSON configurations.
 - **Utilities**: A collection of utilities for tasks such as sending emails, parsing multipart data, handling passwords, and more.
 - **Billing Utilities**: Tools for managing billing plans and user subscriptions.
 - **Menu Options**: Functionality to manage and retrieve authorized menu options based on user roles.
 
@@ -28,15 +28,15 @@
 * AWS account, see [free tier](https://aws.amazon.com/free).
 * AWS Token, see [Access Keys](https://us-east-1.console.aws.amazon.com/iamv2/home?region=us-east-1#/security_credentials?section=IAM_credentials).
 * AWS Command-line interface, see [awscli](https://formulae.brew.sh/formula/awscli).
 * API Framework and Serverless Deployment, see [Chalice](https://github.com/aws/chalice).
 
 ## Getting Started
 
-To get started with GenericSuite, follow these steps:
+To get started with [GenericSuite](https://www.carlosjramirez.com/genericsuite), follow these steps:
 
 ### Initiate your project
 
 To create the project directory for the App's backend API. E.g. `exampleapp_backend`, instrctions will depend on the dependency management of your preference:
 
 ```bash
 # Pip
@@ -59,15 +59,15 @@
 # https://python-poetry.org/docs/basic-usage/
 poetry start exampleapp_backend
 cd exampleapp_backend
 ```
 
 ## Installation
 
-To use GenericSuite in your project, install it with the following command(s):
+To use [GenericSuite](https://www.carlosjramirez.com/genericsuite) in your project, install it with the following command(s):
 
 ### From Pypi
 
 #### Pip
 ```bash
 pip install genericsuite
 ```
@@ -234,37 +234,32 @@
 APP_DB_NAME_DEMO=xxxx
 APP_DB_URI_DEMO=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
 ```
 8. CORS origin
 ```
 # DEV
 APP_CORS_ORIGIN_DEV=*
-APP_FRONTEND_AUDIENCE_DEV=
 ```
 ```
 # QA
 APP_CORS_ORIGIN_QA=*
 APP_CORS_ORIGIN_QA_CLOUD=https://app-qa.exampleapp.com
 APP_CORS_ORIGIN_QA_LOCAL=http://localhost:3000
-APP_FRONTEND_AUDIENCE_QA=
 ```
 ```
 # Staging
 APP_CORS_ORIGIN_STAGING=https://app-qa.exampleapp.com
-APP_FRONTEND_AUDIENCE_STAGING=
 ```
 ```
 # PROD
 APP_CORS_ORIGIN_PROD=https://app.exampleapp.com
-APP_FRONTEND_AUDIENCE_PROD=
 ```
 ```
 # DEMO
 APP_CORS_ORIGIN_DEMO=https://app-demo.exampleapp.com
-APP_FRONTEND_AUDIENCE_DEMO=
 ```
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
```

### Comparing `genericsuite-0.1.2/genericsuite/chalicelib/endpoints/menu_options.py` & `genericsuite-0.1.3/genericsuite/chalicelib/endpoints/menu_options.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/chalicelib/endpoints/users.py` & `genericsuite-0.1.3/genericsuite/chalicelib/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/chalicelib/framework_abstraction.py` & `genericsuite-0.1.3/genericsuite/chalicelib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/chalicelib/util/create_app.py` & `genericsuite-0.1.3/genericsuite/chalicelib/util/create_app.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/chalicelib/util/generic_endpoint_builder.py` & `genericsuite-0.1.3/genericsuite/chalicelib/util/generic_endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/config/config.py` & `genericsuite-0.1.3/genericsuite/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         self.GIT_SUBMODULE_LOCAL_PATH = os.environ.get('GIT_SUBMODULE_LOCAL_PATH')
 
         # ............................
 
         # Auth parameters
 
         self.CORS_ORIGIN = self.get_env('APP_CORS_ORIGIN', '*')
-        self.FRONTEND_AUDIENCE = self.get_env('APP_FRONTEND_AUDIENCE', '')
         self.HEADER_TOKEN_ENTRY_NAME = self.get_env(
             'HEADER_TOKEN_ENTRY_NAME',
             'Authorization'  # 'x-access-tokens'
         )
 
         # Languages
 
@@ -128,12 +127,11 @@
             f'DEBUG = {self.DEBUG}\n' +
             f'SECRET_KEY = {self.SECRET_KEY}\n' +
             f'DB_CONFIG = {self.DB_CONFIG}\n' +
             f'DB_ENGINE = {self.DB_ENGINE}\n' +
             f'APP_SECRET_KEY = {self.APP_SECRET_KEY}\n' +
             f'APP_SUPERADMIN_EMAIL = {self.APP_SUPERADMIN_EMAIL}\n' +
             f'CORS_ORIGIN = {self.CORS_ORIGIN}\n' +
-            f'FRONTEND_AUDIENCE = {self.FRONTEND_AUDIENCE}\n' +
             f'HEADER_TOKEN_ENTRY_NAME = {self.HEADER_TOKEN_ENTRY_NAME}\n' +
             f'STAGE = {self.STAGE}\n' +
             '\n'
         )
```

### Comparing `genericsuite-0.1.2/genericsuite/config/config_from_db.py` & `genericsuite-0.1.3/genericsuite/config/config_from_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
                 "APP_VERSION",
                 "STAGE",
                 "SECRET_KEY",
                 "APP_SECRET_KEY",
                 "APP_SUPERADMIN_EMAIL",
                 "GIT_SUBMODULE_LOCAL_PATH",
                 "CORS_ORIGIN",
-                "FRONTEND_AUDIENCE",
                 "HEADER_TOKEN_ENTRY_NAME",
                 "USE_DB_PARAMS",
             ]
         }
     if DEBUG:
         log_debug('GGC-2) get_general_config |' +
                   f' resultset: {resultset}')
```

### Comparing `genericsuite-0.1.2/genericsuite/config/logging.conf.yml` & `genericsuite-0.1.3/genericsuite/config/logging.conf.yml`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/constants/const_tables.py` & `genericsuite-0.1.3/genericsuite/constants/const_tables.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/fastapilib/framework_abstraction.py` & `genericsuite-0.1.3/genericsuite/fastapilib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/fastapilib/util/generic_endpoint_builder.py` & `genericsuite-0.1.3/genericsuite/fastapilib/util/generic_endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/flasklib/framework_abstraction.py` & `genericsuite-0.1.3/genericsuite/flasklib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/models/billing/billing_utilities.py` & `genericsuite-0.1.3/genericsuite/models/billing/billing_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/models/menu_options/menu_options.py` & `genericsuite-0.1.3/genericsuite/models/menu_options/menu_options.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/models/users/users.py` & `genericsuite-0.1.3/genericsuite/models/users/users.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/app_context.py` & `genericsuite-0.1.3/genericsuite/util/app_context.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/app_logger.py` & `genericsuite-0.1.3/genericsuite/util/app_logger.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/aws.py` & `genericsuite-0.1.3/genericsuite/util/aws.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/config_dbdef_helpers.py` & `genericsuite-0.1.3/genericsuite/util/config_dbdef_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/current_user_data.py` & `genericsuite-0.1.3/genericsuite/util/current_user_data.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/datetime_utilities.py` & `genericsuite-0.1.3/genericsuite/util/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/db_abstractor.py` & `genericsuite-0.1.3/genericsuite/util/db_abstractor.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/exceptions.py` & `genericsuite-0.1.3/genericsuite/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/framework_abs_layer.py` & `genericsuite-0.1.3/genericsuite/util/framework_abs_layer.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/generic_db_helpers.py` & `genericsuite-0.1.3/genericsuite/util/generic_db_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/generic_db_middleware.py` & `genericsuite-0.1.3/genericsuite/util/generic_db_middleware.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/generic_endpoint_helpers.py` & `genericsuite-0.1.3/genericsuite/util/generic_endpoint_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/jwt.py` & `genericsuite-0.1.3/genericsuite/util/jwt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,99 @@
 """
 JWT Library
 """
-# from bson.json_util import dumps
 import base64
-from typing import Callable, List
+from typing import Callable
 import datetime
 
 import jwt
 
-# from chalice.app import Request
 from genericsuite.util.framework_abs_layer import Request
 
 from genericsuite.util.app_logger import log_debug, log_error
 from genericsuite.util.utilities import (
     standard_error_return,
     get_default_resultset,
     get_id_as_string,
 )
 from genericsuite.config.config import Config
 
 settings = Config()
 
-# import logging
-# logger = logging.getLogger(settings.APP_NAME)
-
 # ----------------------- JWT -----------------------
 
 EXPIRATION_MINUTES = 30
 DEBUG = False
 
 
-class TokenPayload:
+class AuthTokenPayload:
     """
     Represents the user's payload structure of the JWT token.
     """
     public_id: str
 
 
 class AuthorizedRequest(Request):
     """
     Represents the AuthorizedRequest payload structure of the JWT token,
     containing the authenticated user's data.
     """
-    user: TokenPayload
+    user: AuthTokenPayload
 
 
-def _request_authentication_with_audience(
-    audiences: List[str]
-) -> Callable[[Request], AuthorizedRequest]:
+def request_authentication() -> Callable[[Request], AuthorizedRequest]:
     """
     Returns a function that performs request authentication with the specified
     audience list.
 
     Args:
-        audiences (List[str]): The list of audiences to validate the token
-        against.
+        None
 
     Returns:
         Callable[[Request], AuthorizedRequest]: A function that performs
         request authentication.
     """
-    def _create_auth_request(request: Request) -> AuthorizedRequest:
+    def create_auth_request(request: Request) -> AuthorizedRequest:
         if settings.HEADER_TOKEN_ENTRY_NAME not in request.headers:
-            # raise UnauthorizedQuery('Missing Authorization Token')
             return standard_error_return('A valid token is missing')
         try:
             token_raw = request.headers[settings.HEADER_TOKEN_ENTRY_NAME]
-            token = token_raw.replace('Bearer ', '')
+            jwt_token = token_raw.replace('Bearer ', '')
             if DEBUG:
-                log_debug('||| _REQUEST_AUTHENTICATION_WITH_AUDIENCE' +
+                log_debug('||| REQUEST_AUTHENTICATION' +
                     '\n | HEADER_TOKEN_ENTRY_NAME: ' +
                     f'{settings.HEADER_TOKEN_ENTRY_NAME}' +
                     f'\n | token_raw: {token_raw}' +
-                    f'\n | token: {token}' +
+                    f'\n | jwt_token: {jwt_token}' +
                     # f'\n | settings.APP_SECRET_KEY: {settings.APP_SECRET_KEY}' +
-                    f'\n | audiences (Deprecated in PYJWT v3): {audiences}' )
-            token_payload = jwt.decode(
-                token,
+                    '\n')
+            jws_token_data = jwt.decode(
+                jwt_token,
                 settings.APP_SECRET_KEY,
                 algorithms="HS256",
-                # audiences=audiences,
             )
             if DEBUG:
-                log_debug('||| _REQUEST_AUTHENTICATION_WITH_AUDIENCE' +
-                    f' | token_payload = {token_payload}')
-            auth_request = AuthorizedRequest(
+                log_debug('||| REQUEST_AUTHENTICATION' +
+                    f' | jws_token_data = {jws_token_data}')
+            authorized_request = AuthorizedRequest(
                 # type: ignore[attr-defined]
                 request.to_original_event(),
                 # type: ignore[attr-defined]
                 lambda_context=request.lambda_context
             )
-            auth_request.user = token_payload
+            authorized_request.user = jws_token_data
             if DEBUG:
-                log_debug('||| _REQUEST_AUTHENTICATION_WITH_AUDIENCE' +
-                    f' | auth_request = {auth_request}')
+                log_debug('||| REQUEST_AUTHENTICATION' +
+                    f' | authorized_request = {authorized_request}')
         except Exception as err:
-            log_error('_REQUEST_AUTHENTICATION_WITH_AUDIENCE' +
+            log_error('REQUEST_AUTHENTICATION' +
                 f' | Exception = {str(err)}')
-            # raise e
             return standard_error_return('Token is invalid')
-        return auth_request
-    return _create_auth_request
-
-
-def request_authentication() -> Callable[[Request], AuthorizedRequest]:
-    """
-    Returns a function that performs request authentication with the specified
-    audience list.
-
-    Args:
-        None
-
-    Returns:
-        Callable[[Request], AuthorizedRequest]: A function that performs
-        request authentication.
-    """
-    audience_list = settings.FRONTEND_AUDIENCE.split(',')
-    return _request_authentication_with_audience(audience_list)
+        return authorized_request
+    return create_auth_request
 
 
 def token_encode(user):
     """
     Encode a JWT token for the given user.
 
     Args:
```

### Comparing `genericsuite-0.1.2/genericsuite/util/nav_helpers.py` & `genericsuite-0.1.3/genericsuite/util/nav_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/parse_multipart.py` & `genericsuite-0.1.3/genericsuite/util/parse_multipart.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/passwords.py` & `genericsuite-0.1.3/genericsuite/util/passwords.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/request_handler.py` & `genericsuite-0.1.3/genericsuite/util/request_handler.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/security.py` & `genericsuite-0.1.3/genericsuite/util/security.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/send_email.py` & `genericsuite-0.1.3/genericsuite/util/send_email.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/genericsuite/util/utilities.py` & `genericsuite-0.1.3/genericsuite/util/utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.2/pyproject.toml` & `genericsuite-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genericsuite"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Carlos J. Ramirez", email="<tomkat_cr@yahoo.com>" }
 ]
 description = "The GenericSuite for Python (backend version)"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 classifiers = [
@@ -15,15 +15,15 @@
 
 [project.urls]
 Homepage = "https://github.com/tomkat-cr/genericsuite-be"
 Issues = "https://github.com/tomkat-cr/genericsuite-be/issues"
 
 [tool.poetry]
 name = "genericsuite"
-version = "0.1.2"
+version = "0.1.3"
 description = "The GenericSuite for Python (backend version)"
 authors = ["Carlos J. Ramirez <tomkat_cr@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tomkat-cr/genericsuite-be.git"
 packages = [
     { include = "genericsuite" }
```

### Comparing `genericsuite-0.1.2/PKG-INFO` & `genericsuite-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genericsuite
-Version: 0.1.2
+Version: 0.1.3
 Summary: The GenericSuite for Python (backend version)
 Home-page: https://github.com/tomkat-cr/genericsuite-be.git
 License: MIT
 Author: Carlos J. Ramirez
 Author-email: tomkat_cr@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,19 +28,19 @@
 Project-URL: Repository, https://github.com/tomkat-cr/genericsuite-be.git
 Description-Content-Type: text/markdown
 
 # The GenericSuite for Python (backend version)
 
 ![GenericSuite Logo](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/lib/images/gs_logo_circle.png)
 
-GenericSuite is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including Chalice, FastAPI, and Flask, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
+[GenericSuite](https://www.carlosjramirez.com/genericsuite) is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including FastAPI, Flask and Chalice, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
 
 ## Features
 
-- **Framework Agnostic**: Supports Chalice, FastAPI, and Flask frameworks.
+- **Framework Agnostic**: Supports FastAPI, Flask, and Chalice frameworks.
 - **Database Support**: Includes abstracted database operations for both MongoDB and DynamoDB, offering flexibility in choosing the database.
 - **Authentication**: Implements JWT-based authentication, providing secure access to endpoints.
 - **Dynamic Endpoint Creation**: Allows for defining endpoints dynamically through JSON configurations.
 - **Utilities**: A collection of utilities for tasks such as sending emails, parsing multipart data, handling passwords, and more.
 - **Billing Utilities**: Tools for managing billing plans and user subscriptions.
 - **Menu Options**: Functionality to manage and retrieve authorized menu options based on user roles.
 
@@ -58,15 +58,15 @@
 * AWS account, see [free tier](https://aws.amazon.com/free).
 * AWS Token, see [Access Keys](https://us-east-1.console.aws.amazon.com/iamv2/home?region=us-east-1#/security_credentials?section=IAM_credentials).
 * AWS Command-line interface, see [awscli](https://formulae.brew.sh/formula/awscli).
 * API Framework and Serverless Deployment, see [Chalice](https://github.com/aws/chalice).
 
 ## Getting Started
 
-To get started with GenericSuite, follow these steps:
+To get started with [GenericSuite](https://www.carlosjramirez.com/genericsuite), follow these steps:
 
 ### Initiate your project
 
 To create the project directory for the App's backend API. E.g. `exampleapp_backend`, instrctions will depend on the dependency management of your preference:
 
 ```bash
 # Pip
@@ -89,15 +89,15 @@
 # https://python-poetry.org/docs/basic-usage/
 poetry start exampleapp_backend
 cd exampleapp_backend
 ```
 
 ## Installation
 
-To use GenericSuite in your project, install it with the following command(s):
+To use [GenericSuite](https://www.carlosjramirez.com/genericsuite) in your project, install it with the following command(s):
 
 ### From Pypi
 
 #### Pip
 ```bash
 pip install genericsuite
 ```
@@ -264,37 +264,32 @@
 APP_DB_NAME_DEMO=xxxx
 APP_DB_URI_DEMO=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
 ```
 8. CORS origin
 ```
 # DEV
 APP_CORS_ORIGIN_DEV=*
-APP_FRONTEND_AUDIENCE_DEV=
 ```
 ```
 # QA
 APP_CORS_ORIGIN_QA=*
 APP_CORS_ORIGIN_QA_CLOUD=https://app-qa.exampleapp.com
 APP_CORS_ORIGIN_QA_LOCAL=http://localhost:3000
-APP_FRONTEND_AUDIENCE_QA=
 ```
 ```
 # Staging
 APP_CORS_ORIGIN_STAGING=https://app-qa.exampleapp.com
-APP_FRONTEND_AUDIENCE_STAGING=
 ```
 ```
 # PROD
 APP_CORS_ORIGIN_PROD=https://app.exampleapp.com
-APP_FRONTEND_AUDIENCE_PROD=
 ```
 ```
 # DEMO
 APP_CORS_ORIGIN_DEMO=https://app-demo.exampleapp.com
-APP_FRONTEND_AUDIENCE_DEMO=
 ```
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
```

