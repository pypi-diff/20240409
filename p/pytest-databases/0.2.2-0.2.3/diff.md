# Comparing `tmp/pytest_databases-0.2.2.tar.gz` & `tmp/pytest_databases-0.2.3.tar.gz`

## Comparing `pytest_databases-0.2.2.tar` & `pytest_databases-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/CODEOWNERS
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/Makefile
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/sonar-project.properties
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/docker-compose.yml
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/__init__.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/LICENSE
--rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/README.md
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 pytest_databases-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/CODEOWNERS
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/Makefile
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/sonar-project.properties
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/docker-compose.yml
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/LICENSE
+-rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/README.md
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/PKG-INFO
```

### Comparing `pytest_databases-0.2.2/.pre-commit-config.yaml` & `pytest_databases-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/.sourcery.yaml` & `pytest_databases-0.2.3/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/CONTRIBUTING.rst` & `pytest_databases-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/Makefile` & `pytest_databases-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/.vscode/settings.json` & `pytest_databases-0.2.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/requirements/requirements-dev.txt` & `pytest_databases-0.2.3/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/requirements/requirements-docs.txt` & `pytest_databases-0.2.3/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/scripts/__init__.py` & `pytest_databases-0.2.3/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/scripts/build_docs.py` & `pytest_databases-0.2.3/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/__init__.py` & `pytest_databases-0.2.3/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/__metadata__.py` & `pytest_databases-0.2.3/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/helpers.py` & `pytest_databases-0.2.3/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/docker-compose.yml` & `pytest_databases-0.2.3/src/pytest_databases/docker/docker-compose.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,179 +1,179 @@
 services:
   postgres12:
     networks:
       - default
     image: postgres:12
     ports:
-      - "${POSTGRES12_PORT}:5432" # use a non-standard port here
+      - "${POSTGRES12_PORT:-5423}:5432" # use a non-standard port here
     environment:
-      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
+      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD:-super-secret}
   postgres13:
     networks:
       - default
     image: postgres:13
     ports:
-      - "${POSTGRES13_PORT}:5432" # use a non-standard port here
+      - "${POSTGRES13_PORT:-5424}:5432" # use a non-standard port here
     environment:
-      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
+      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD:-super-secret}
   postgres14:
     networks:
       - default
     image: postgres:14
     ports:
-      - "${POSTGRES14_PORT}:5432" # use a non-standard port here
+      - "${POSTGRES14_PORT:-5425}:5432" # use a non-standard port here
     environment:
-      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
+      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD:-super-secret}
   postgres15:
     networks:
       - default
     image: postgres:15
     ports:
-      - "${POSTGRES15_PORT}:5432" # use a non-standard port here
+      - "${POSTGRES15_PORT:-5426}:5432" # use a non-standard port here
     environment:
-      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
+      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD:-super-secret}
   postgres16:
     networks:
       - default
     image: postgres:16
     ports:
-      - "${POSTGRES16_PORT}:5432" # use a non-standard port here
+      - "${POSTGRES16_PORT:-5427}:5432" # use a non-standard port here
     environment:
-      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
+      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD:-super-secret}
   mariadb113:
     networks:
       - default
     image: mariadb:11.3
     ports:
-      - "${MARIADB113_PORT}:3306" # use a non-standard port here
+      - "${MARIADB113_PORT:-3359}:3306" # use a non-standard port here
     environment:
-      MARIADB_ROOT_PASSWORD: ${MARIADB_ROOT_PASSWORD}
-      MARIADB_PASSWORD: ${MARIADB_PASSWORD}
-      MARIADB_USER: ${MARIADB_USER}
-      MARIADB_DATABASE: ${MARIADB_DATABASE}
+      MARIADB_ROOT_PASSWORD: ${MARIADB_ROOT_PASSWORD:-super-secret}
+      MARIADB_PASSWORD: ${MARIADB_PASSWORD:-super-secret}
+      MARIADB_USER: ${MARIADB_USER:-app}
+      MARIADB_DATABASE: ${MARIADB_DATABASE:-db}
       MARIADB_ROOT_HOST: "%"
       LANG: C.UTF-8
   mysql8:
     networks:
       - default
     image: mysql:latest
     ports:
-      - "${MYSQL8_PORT}:3306" # use a non-standard port here
+      - "${MYSQL8_PORT:-3360}:3306" # use a non-standard port here
     environment:
-      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD}
-      MYSQL_PASSWORD: ${MYSQL_PASSWORD}
-      MYSQL_USER: ${MYSQL_USER}
-      MYSQL_DATABASE: ${MYSQL_DATABASE}
+      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD:-super-secret}
+      MYSQL_PASSWORD: ${MYSQL_PASSWORD:-super-secret}
+      MYSQL_USER: ${MYSQL_USER:-app}
+      MYSQL_DATABASE: ${MYSQL_DATABASE:-db}
       MYSQL_ROOT_HOST: "%"
       LANG: C.UTF-8
   mysql57:
     networks:
       - default
     image: mysql:5.7
     ports:
-      - "${MYSQL57_PORT}:3306" # use a non-standard port here
+      - "${MYSQL57_PORT:-3362}:3306" # use a non-standard port here
     environment:
-      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD}
-      MYSQL_PASSWORD: ${MYSQL_PASSWORD}
-      MYSQL_USER: ${MYSQL_USER}
-      MYSQL_DATABASE: ${MYSQL_DATABASE}
+      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD:-super-secret}
+      MYSQL_PASSWORD: ${MYSQL_PASSWORD:-super-secret}
+      MYSQL_USER: ${MYSQL_USER:-app}
+      MYSQL_DATABASE: ${MYSQL_DATABASE:-db}
       MYSQL_ROOT_HOST: "%"
       LANG: C.UTF-8
   mysql56:
     networks:
       - default
     image: mysql:5.6
     ports:
-      - "${MYSQL56_PORT}:3306" # use a non-standard port here
+      - "${MYSQL56_PORT:-3363}:3306" # use a non-standard port here
     environment:
-      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD}
-      MYSQL_PASSWORD: ${MYSQL_PASSWORD}
-      MYSQL_USER: ${MYSQL_USER}
-      MYSQL_DATABASE: ${MYSQL_DATABASE}
+      MYSQL_ROOT_PASSWORD: ${MYSQL_ROOT_PASSWORD:-super-secret}
+      MYSQL_PASSWORD: ${MYSQL_PASSWORD:-super-secret}
+      MYSQL_USER: ${MYSQL_USER:-app}
+      MYSQL_DATABASE: ${MYSQL_DATABASE:-db}
       MYSQL_ROOT_HOST: "%"
       LANG: C.UTF-8
   oracle18c:
     networks:
       - default
     image: gvenzl/oracle-xe:18-slim-faststart
     ports:
-      - "${ORACLE18C_PORT}:1521" # use a non-standard port here
+      - "${ORACLE18C_PORT:-1514}:1521" # use a non-standard port here
     environment:
-      ORACLE_PASSWORD: ${ORACLE_SYSTEM_PASSWORD}
-      APP_USER_PASSWORD: ${ORACLE_PASSWORD}
-      APP_USER: ${ORACLE_USER}
+      ORACLE_PASSWORD: ${ORACLE_SYSTEM_PASSWORD:-super-secret}
+      APP_USER_PASSWORD: ${ORACLE_PASSWORD:-super-secret}
+      APP_USER: ${ORACLE_USER:-app}
   oracle23c:
     networks:
       - default
     image: gvenzl/oracle-free:23-slim-faststart
     ports:
-      - "${ORACLE23C_PORT}:1521" # use a non-standard port here
+      - "${ORACLE23C_PORT:-1513}:1521" # use a non-standard port here
     environment:
-      ORACLE_PASSWORD: ${ORACLE_SYSTEM_PASSWORD}
-      APP_USER_PASSWORD: ${ORACLE_PASSWORD}
-      APP_USER: ${ORACLE_USER}
+      ORACLE_PASSWORD: ${ORACLE_SYSTEM_PASSWORD:-super-secret}
+      APP_USER_PASSWORD: ${ORACLE_PASSWORD:-super-secret}
+      APP_USER: ${ORACLE_USER:-app}
   mssql2022:
     networks:
       - default
     image: mcr.microsoft.com/mssql/server:2022-latest
     ports:
       - "${MSSQL2022_PORT:-4133}:1433" # use a non-standard port here
     environment:
       SA_PASSWORD: ${MSSQL_PASSWORD:-Super-secret1}
       MSSQL_PID: Developer
       ACCEPT_EULA: Accepted
       MSSQL_TCP_PORT: 1433
   spanner:
     image: gcr.io/cloud-spanner-emulator/emulator:latest
     ports:
-      - "${SPANNER_PORT}:9010"
+      - "${SPANNER_PORT:-9010}:9010"
   # Init (Create Instance)
   spanner_init:
     image: gcr.io/google.com/cloudsdktool/cloud-sdk:332.0.0-slim
     command: >
       bash -c 'gcloud config configurations create emulator &&
               gcloud config set auth/disable_credentials true &&
               gcloud config set project $${PROJECT_ID} &&
               gcloud config set auth/disable_credentials true &&
               gcloud spanner instances create $${INSTANCE_NAME} --config=emulator-config --description=Emulator --nodes=1'
     environment:
-      PROJECT_ID: ${GOOGLE_CLOUD_PROJECT}
-      INSTANCE_NAME: ${SPANNER_INSTANCE}
-      DATABASE_NAME: ${SPANNER_DATABASE}
+      PROJECT_ID: ${GOOGLE_CLOUD_PROJECT:-emulator-test-project}
+      INSTANCE_NAME: ${SPANNER_INSTANCE:-test-instance}
+      DATABASE_NAME: ${SPANNER_DATABASE:-test-database}
     depends_on:
       - spanner
   cockroachdb:
     image: cockroachdb/cockroach:latest-v23.1
     command: start-single-node --insecure
     restart: "no"
     expose:
       - "8080"
-      - "${COCKROACHDB_PORT}"
+      - "${COCKROACHDB_PORT:-26257}"
     ports:
-      - "${COCKROACHDB_PORT}:26257"
+      - "${COCKROACHDB_PORT:-26257}:26257"
       - "8880:8080"
     healthcheck:
       test: ["CMD", "curl", "-f", "http://localhost:8080/health?ready=1"]
       interval: 3s
       timeout: 3s
       retries: 5
   redis:
     image: redis
     ports:
-      - "${REDIS_PORT}:6379"
+      - "${REDIS_PORT:-6397}:6379"
   keydb:
     image: eqalpha/keydb
     ports:
-      - "${KEYDB_PORT}:6379"
+      - "${KEYDB_PORT:-6396}:6379"
   dragonfly:
     image: "docker.dragonflydb.io/dragonflydb/dragonfly"
     ulimits:
       memlock: -1
     ports:
-      - "${DRAGONFLY_PORT}:6379"
+      - "${DRAGONFLY_PORT:-6398}:6379"
     # For better performance, consider `host` mode instead `port` to avoid docker NAT.
     # `host` mode is NOT currently supported in Swarm Mode.
     # https://docs.docker.com/compose/compose-file/compose-file-v3/#network_mode
     # network_mode: "host"
     volumes:
       - dragonflydata:/data
 networks:
```

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/redis.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.2.3/src/pytest_databases/docker/spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/__init__.py` & `pytest_databases-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/conftest.py` & `pytest_databases-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/__init__.py` & `pytest_databases-0.2.3/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_cockroachdb.py` & `pytest_databases-0.2.3/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_dragonfly.py` & `pytest_databases-0.2.3/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_keydb.py` & `pytest_databases-0.2.3/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_mariadb.py` & `pytest_databases-0.2.3/tests/docker/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_mssql.py` & `pytest_databases-0.2.3/tests/docker/test_mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_mysql.py` & `pytest_databases-0.2.3/tests/docker/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_oracle.py` & `pytest_databases-0.2.3/tests/docker/test_oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_postgres.py` & `pytest_databases-0.2.3/tests/docker/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_redis.py` & `pytest_databases-0.2.3/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/tests/docker/test_spanner.py` & `pytest_databases-0.2.3/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/.gitignore` & `pytest_databases-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/LICENSE` & `pytest_databases-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/README.md` & `pytest_databases-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.2/pyproject.toml` & `pytest_databases-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.2"
+version = "0.2.3"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
```

### Comparing `pytest_databases-0.2.2/PKG-INFO` & `pytest_databases-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

