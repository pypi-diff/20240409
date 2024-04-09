# Comparing `tmp/pgworkload-0.1.7.tar.gz` & `tmp/pgworkload-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgworkload-0.1.7.tar", max compression
+gzip compressed data, was "pgworkload-0.1.8.tar", max compression
```

## Comparing `pgworkload-0.1.7.tar` & `pgworkload-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.7/LICENSE
--rw-r--r--   0        0        0     9028 2023-08-09 14:49:03.166934 pgworkload-0.1.7/README.md
--rw-r--r--   0        0        0      495 2024-04-05 23:08:50.306315 pgworkload-0.1.7/pgworkload/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-07 22:27:57.373962 pgworkload-0.1.7/pgworkload/cli/dep.py
--rw-r--r--   0        0        0     6915 2024-04-07 22:27:57.444521 pgworkload-0.1.7/pgworkload/cli/main.py
--rw-r--r--   0        0        0     3863 2024-04-07 22:29:46.279410 pgworkload-0.1.7/pgworkload/cli/util.py
--rw-r--r--   0        0        0    10746 2024-04-07 22:27:57.469736 pgworkload-0.1.7/pgworkload/models/init.py
--rw-r--r--   0        0        0    10448 2024-04-07 22:20:28.798413 pgworkload-0.1.7/pgworkload/models/run.py
--rw-r--r--   0        0        0     7610 2024-04-07 22:20:28.798521 pgworkload-0.1.7/pgworkload/models/util.py
--rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.7/pgworkload/utils/builtin_workloads.py
--rw-r--r--   0        0        0    17469 2024-03-15 16:58:47.985432 pgworkload-0.1.7/pgworkload/utils/common.py
--rw-r--r--   0        0        0    21871 2024-04-05 19:40:38.128860 pgworkload-0.1.7/pgworkload/utils/simplefaker.py
--rw-r--r--   0        0        0      867 2024-04-07 22:30:31.092928 pgworkload-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    10186 1970-01-01 00:00:00.000000 pgworkload-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.8/LICENSE
+-rw-r--r--   0        0        0    10356 2024-04-09 18:26:42.210700 pgworkload-0.1.8/README.md
+-rw-r--r--   0        0        0      510 2024-04-09 13:52:42.542259 pgworkload-0.1.8/pgworkload/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-08 20:27:05.487329 pgworkload-0.1.8/pgworkload/cli/dep.py
+-rw-r--r--   0        0        0     6857 2024-04-09 15:08:48.393900 pgworkload-0.1.8/pgworkload/cli/main.py
+-rw-r--r--   0        0        0     3863 2024-04-07 22:29:46.279410 pgworkload-0.1.8/pgworkload/cli/util.py
+-rw-r--r--   0        0        0    10746 2024-04-07 22:27:57.469736 pgworkload-0.1.8/pgworkload/models/init.py
+-rw-r--r--   0        0        0    10814 2024-04-09 16:23:08.486672 pgworkload-0.1.8/pgworkload/models/run.py
+-rw-r--r--   0        0        0     7614 2024-04-08 20:36:44.283029 pgworkload-0.1.8/pgworkload/models/util.py
+-rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.8/pgworkload/utils/builtin_workloads.py
+-rw-r--r--   0        0        0    19696 2024-04-09 15:58:45.107198 pgworkload-0.1.8/pgworkload/utils/common.py
+-rw-r--r--   0        0        0    21875 2024-04-08 20:36:56.464511 pgworkload-0.1.8/pgworkload/utils/simplefaker.py
+-rw-r--r--   0        0        0      867 2024-04-09 18:28:44.359293 pgworkload-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    11514 1970-01-01 00:00:00.000000 pgworkload-0.1.8/PKG-INFO
```

### Comparing `pgworkload-0.1.7/LICENSE` & `pgworkload-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.7/README.md` & `pgworkload-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -27,80 +27,94 @@
 
 File `bank.yaml` is the data generation definition file.
 For each column of table `ref_data`, we deterministically generate random data.
 This file is meant as a guide to show what type of data can be generated, and what args are required.
 
 File `bank.py` defines the workload.
 The workload is defined as a class object.
-The class defines 3 methods: `init()`, `run()` and the constructor, `__init__()`.
+The class defines 2 methods: `run()` and the constructor, `__init__()`.
 All other methods are part of the application logic of the workload.
 Read the comments along the code for more information.
 
 Let's run the sample **Bank** workload.
 
-### Step 0 - Create Python env
+### Step 0 - env setup
 
 ```bash
 # upgrade pip - must have pip version 20.3+ 
 pip3 install --upgrade pip
 
-# we're now inside our virtual env
 pip3 install pgworkload
 
-# download the bank workload files
 mkdir workloads
+cd workloads
+
 # the workload class
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.py
-# the schema file
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.sql
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.py
+
+# the DDL file
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.sql
+
 # the data generation definition file
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.yaml
-# the arguments to pass at runtime, optional
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.args.yaml
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.yaml
 ```
 
-### Step 1 - Init the workload
+### Step 1 - init the workload
+
+Make sure your **CockroachDB** cluster or **PostgreSQL** server is up and running.
 
-We assume that your **CockroachDB** cluster or **PostgreSQL** server is up and running.
+Connect to the SQL prompt and load the `bank.sql` file.
+In CockroachDB, you can run
 
-Init the **Bank** workload.
+```sql
+sql> \i bank.sql
+```
+
+Next, generate some CSV data to seed the database:
 
 ```bash
-# CockroachDB
-pgworkload init -w workloads/bank.py --url 'postgres://root@localhost:26257/postgres?sslmode=disable'
+pgworkload util csv -i bank.yaml -x 1
+```
 
-# PostgreSQL
-pgworkload init --w workloads/bank.py --url 'postgres://root@localhost:5432/postgres?sslmode=disable'
+The CSV files will be located inside a `bank` directory.
+
+```bash
+$ ls -lh bank
+total 1032
+-rw-r--r--  1 fabio  staff   513K Apr  9 13:01 ref_data.0_0_0.csv
 ```
 
-You should see something like below
+Now you can import the CSV file.
+In CockroachDB, my favorite method is to use a webserver to serve the CSV file.
+Open a new terminal then start a simple python server
 
-```text
-2022-01-28 17:21:47,335 [INFO] (MainProcess 29422) URL: 'postgres://root@localhost:[5432|26257]/defaultdb?sslmode=disable&application_name=Bank'
-2022-01-28 17:21:47,480 [INFO] (MainProcess 29422) Database 'bank' created.
-2022-01-28 17:21:47,769 [INFO] (MainProcess 29422) Created workload schema
-2022-01-28 17:21:47,789 [INFO] (MainProcess 29422) Generating dataset for table 'ref_data'
-2022-01-28 17:22:07,088 [INFO] (MainProcess 29422) Importing data for table 'ref_data'
-2022-01-28 17:22:21,063 [INFO] (MainProcess 29422) Init completed. Please update your database connection url to 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank'
+```bash
+cd workloads
+cd bank
+python3 -m http.server 3000
 ```
 
-`pgworkload` has read file `bank.sql` and has created the database and its schema.
-It has then read file `bank.yaml` and has generated the CSV files for the table `ref_data`.
-Finally, it imports the CSV files into database `bank`.
+If you open your browser at <http://localhost:3000> you should see file `ref_data.0_0_0.csv` being served.
+
+At the SQL prompt, import the file
+
+```sql
+sql> IMPORT INTO ref_data CSV DATA ('http://localhost:3000/ref_data.0_0_0.csv') WITH delimiter = e'\t'; 
+```
 
 ### Step 2 - Run the workload
 
 Run the workload using 8 connections for 120 seconds or 100k cycles, whichever comes first.
 
 ```bash
 # CockroachDB
-pgworkload run -w workloads/bank.py -c 8 --url 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
+pgworkload run -w bank.py -c 8 --url 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
 
 # PostgreSQL
-pgworkload run -w workloads/bank.py -c 8 --url 'postgres://root@localhost:5432/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
+pgworkload run -w bank.py -c 8 --url 'postgres://root@localhost:5432/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
 ```
 
 `pgworkload` uses exclusively the excellent [Psycopg 3](https://www.psycopg.org/psycopg3/docs/) to connect.
 No other ORMs or drivers/libraries are used.
 Psycopg has a very simple, neat way to [create connections and execute statements](https://www.psycopg.org/psycopg3/docs/basic/usage.html) and [transactions](https://www.psycopg.org/psycopg3/docs/basic/transactions.html).
 
 `pgworkload` will output something like below
@@ -130,36 +144,69 @@
 There are many built-in options.
 Check them out with
 
 ```bash
 pgworkload --help
 ```
 
+## How it works
+
+It’s helpful to understand first what `pgworkload` does:
+
+- At runtime, `pgworkload` first imports the class you pass, `bank.py`.
+- It spawns _n_ threads for concurrent execution (see next section on Concurrency).
+- By default, it sets the connection to `autocommit` mode.
+- **psycopg v3** will _PREPARE_ statements automatically after 5 executions.
+- Each thread creates a database connection - no need for a connection pool.
+- In a loop, `pgworkload` will:
+  - execute function `run()` which returns a list of functions.
+  - execute each function in the list sequentially. Each function, typically, executes a SQL statement/transaction.
+- Execution stats are funneled back to the _MainThread_, which aggregates and prints them to _stdout_.
+- If the connection drops, it will recreate it. You can also program how long you want the connection to last.
+- `pgworkload` stops once a limit has been reached (iteration/duration), or you Ctrl+C.
+
 ## Concurrency - processes and threads
 
-pgworkload uses both the `multiprocessing` and `threading` library to achieve high concurrency, that is, opening multiple connections to the DBMS.
+`pgworkload` uses both the `multiprocessing` and `threading` library to achieve high concurrency, that is, opening multiple connections to the DBMS.
 
 There are 2 parameters that can be used to configure how many processes you want to create, and for each process, how many threads:
 
 - `--procs`, or `-x`, to configure the count of processes (defaults to the CPU count)
 - `--concurrency`, or `-c`, to configure the total number of executing workloads to run (also referred to as _executing threads_)
 
-pgworkload will spread the load across the processes, so that each process has an even amount of threads.
+`pgworkload` will spread the load across the processes, so that each process has an even amount of threads.
 
 Example: if we set `--procs 4` and `--concurrency 10`, pgworkload will create as follows:
 
 - Process-1: MainThread + 2 extra threads. Total = 3
 - Process-2: MainThread + 2 extra threads. Total = 3
 - Process-3: MainThread + 1 extra thread.  Total = 2
 - Process-3: MainThread + 1 extra thread.  Total = 2
 
 Total workloads = 10
 
 This allows you to fine tune the count of Python processes and threads to fit your system.
 
+## Generating CSV files
+
+- You can seed a database quickly by letting pgworkload generate pseudo-random data and import it.
+- `pgworkload` takes the DDL as an input and creates an intermediate YAML file, with the definition of what data you want to create (a string, a number, a date, a bool..) based on the column data type.
+- You then refine the YAML file to suit your needs, for example, the size of the string, a range for a date, the precision for a decimal, a choice among a discrete list of values..
+- You can also specify what is the percentage of NULL for any column, or how many elements in an ARRAY type.
+- You then specify the total row count, how many rows per file, and in what order, if any, to sort by.
+- Then `pgworkload` will generate the data into CSV or TSV files, compress them if so requested.
+
+Write up: <https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4>
+
+Find out more on the `yaml` and `csv` commands by running
+
+```bash
+pgworkload util --help
+```
+
 ## Built-in Workloads
 
 `pgworkload` has the following workload already built-in and can be called without the need to pass a class file
 
 ### Querybench
 
 Querybench runs a list of SQL Statements sequentially and iteratively.
@@ -181,14 +228,10 @@
 
 Run **Querybench** like this:
 
 ```bash
 pgworkload run --builtin-workload Querybench --args mystmts.sql --url <conn-string>
 ```
 
-### Hovr
-
-Coming soon
-
 ## Acknowledgments
 
 Some methods and classes have been taken and modified from, or inspired by, <https://github.com/cockroachdb/movr>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pgworkload-0.1.7/pgworkload/cli/dep.py` & `pgworkload-0.1.8/pgworkload/cli/dep.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.7/pgworkload/cli/main.py` & `pgworkload-0.1.8/pgworkload/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import platform
 import re
 import sys
 import typer
 import yaml
 
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("pgworkload")
 
 app = typer.Typer(
     epilog=EPILOG,
     no_args_is_help=True,
     help=f"pgworkload v{__version__}: Workload utility for the PostgreSQL protocol.",
 )
 
@@ -121,15 +121,15 @@
         duration=duration,
         conn_duration=conn_duration,
         args=args,
         log_level=log_level.upper(),
     )
 
 
-@app.command(help="Init the workload.", epilog=EPILOG, no_args_is_help=True)
+#@app.command(help="Init the workload.", epilog=EPILOG, no_args_is_help=True)
 def init(
     workload_path: Optional[Path] = Param.WorkloadPath,
     procs: int = Param.Procs,
     dburl: str = Param.DBUrl,
     drop: bool = typer.Option(False, "--drop", help="Drop the database if it exists."),
     csv_max_rows: int = Param.CSVMaxRows,
     skip_schema: bool = typer.Option(
@@ -145,17 +145,15 @@
         None, show_default=False, help="Override the default DB name."
     ),
     http_server_hostname: str = Param.HTTPServerHostName,
     http_server_port: int = Param.HTTPServerPort,
     args: str = Param.Args,
     log_level: LogLevel = Param.LogLevel,
 ):
-    logging.getLogger(__package__).setLevel(log_level.upper())
-
-    logger.debug("Executing run()")
+    logger.debug("Executing init()")
 
     procs, dburl, args = __validate(procs, dburl, None, args, workload_path)
 
     pgworkload.models.init.init(
         db=db,
         workload_path=workload_path,
         dburl=dburl,
```

### Comparing `pgworkload-0.1.7/pgworkload/cli/util.py` & `pgworkload-0.1.8/pgworkload/cli/util.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.7/pgworkload/models/init.py` & `pgworkload-0.1.8/pgworkload/models/init.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.7/pgworkload/models/run.py` & `pgworkload-0.1.8/pgworkload/models/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 import threading
 import time
 import traceback
 import logging.handlers
 import tabulate
 
 DEFAULT_SLEEP = 3
+MAX_RETRIES = 3
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("pgworkload")
 
 HEADERS: list = [
     "id",
     "elapsed",
     "tot_ops",
     "tot_ops/s",
     "period_ops",
@@ -324,18 +325,24 @@
                             "conn_duration reached, will reset the connection."
                         )
                         break
 
                     cycle_start = time.time()
                     for txn in w.run():
                         start = time.time()
-                        pgworkload.utils.common.run_transaction(
-                            conn, lambda conn: txn(conn)
+                        retries = pgworkload.utils.common.run_transaction(
+                            conn, lambda conn: txn(conn), max_retries=MAX_RETRIES
                         )
-                        if not q.full() and not disable_stats:
+
+                        # record how many retries there were, if any
+                        for _ in range(retries):
+                            q.put(("40001", 0))
+
+                        # if retries matches max_retries, then it's a total failure and we don't record the txn time
+                        if not q.full() and not disable_stats and retries < MAX_RETRIES:
                             q.put((txn.__name__, time.time() - start))
 
                     c += 1
                     if not q.full() and not disable_stats:
                         q.put(("__cycle__", time.time() - cycle_start))
 
         # catch any error, pass that error to the MainProcess
```

### Comparing `pgworkload-0.1.7/pgworkload/models/util.py` & `pgworkload-0.1.8/pgworkload/models/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os
 import pgworkload.utils.simplefaker
 import pgworkload.utils.common
 import sys
 import yaml
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("pgworkload")
 
 
 def util_csv(
     input: str,
     output: str,
     compression: str,
     procs: int,
```

### Comparing `pgworkload-0.1.7/pgworkload/utils/builtin_workloads.py` & `pgworkload-0.1.8/pgworkload/utils/builtin_workloads.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.7/pgworkload/utils/common.py` & `pgworkload-0.1.8/pgworkload/utils/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "bucket_count",
 ]
 
 DEFAULT_ARRAY_COUNT = 3
 SUPPORTED_DBMS = ["PostgreSQL", "CockroachDB"]
 
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("pgworkload")
 
 
 class QuietServerHandler(http.server.SimpleHTTPRequestHandler):
     """SimpleHTTPRequestHandler that doesn't output any log"""
 
     def log_message(self, format, *args):
         pass
@@ -81,15 +81,16 @@
     def add_latency_measurement(self, action: str, measurement: float) -> None:
         self.window_stats.setdefault(action, []).append(measurement)
         self.cumulative_counts.setdefault(action, 0)
         self.cumulative_counts[action] += 1
 
         if action not in self.prom_latency:
             self.prom_latency[action] = prometheus_client.Summary(
-                f"latency_{action}", f"Latency for transaction {action}"
+                f"latency_{action.replace(' ', '')}",
+                f"Latency for transaction {action}",
             )
         self.prom_latency[action].observe(measurement)
 
     # calculate the current stats this instance has collected.
     def calculate_stats(self) -> list:
         def get_stats_row(action: str):
             elapsed: float = time.time() - self.instantiation_time
@@ -177,26 +178,27 @@
     *max_retries* times before giving up (and propagate it).
     """
     for retry in range(1, max_retries + 1):
         try:
             op(conn)
             # If we reach this point, we were able to commit, so we break
             # from the retry loop.
-            return
+            return retry - 1
         except psycopg.errors.SerializationFailure as e:
             # This is a retry error, so we roll back the current
             # transaction and sleep for a bit before retrying. The
             # sleep time increases for each failed transaction.
             logger.debug(f"psycopg.SerializationFailure:: {e}")
             conn.rollback()
             time.sleep((2**retry) * 0.1 * (random.random() + 0.5))
         except psycopg.Error as e:
             raise e
 
-    raise ValueError(f"Transaction did not succeed after {max_retries} retries")
+    logger.debug(f"Transaction did not succeed after {max_retries} retries")
+    return retry
 
 
 def get_based_name_dir(filepath: str):
     """Return the directory name based on the filename
 
     Args:
         filepath (str): the filepath, eg: /path/to/myfile.txt
@@ -311,32 +313,44 @@
     Args:
         ddl (str): CREATE TABLE statements
 
     Returns:
         (str): the YAML data gen definition string
     """
 
-    def get_type_and_args(datatypes: list):
+    def get_type_and_args(col_type_and_args: list):
+        is_not_null = False
+        if "not" in col_type_and_args and "null" in col_type_and_args:
+            is_not_null = True
         # check if it is an array
         # string array
         # string []
         # string[]
         is_array = False
-        datatypes = [x.lower() for x in datatypes]
-        if "[]" in datatypes[0] or "array" in datatypes or "[]" in datatypes:
+        col_type_and_args = [x.lower() for x in col_type_and_args]
+        if (
+            "[]" in col_type_and_args[0]
+            or "array" in col_type_and_args
+            or "[]" in col_type_and_args
+        ):
             is_array = True
 
-        datatype: str = datatypes[0].replace("[]", "")
+        datatype: str = col_type_and_args[0].replace("[]", "")
+        arg = None
+        if len(col_type_and_args) > 1:
+            arg = col_type_and_args[1:]
 
         if datatype.lower() in ["bool", "boolean"]:
             return {
                 "type": "bool",
                 "args": {
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in [
             "int",
             "integer",
@@ -349,106 +363,143 @@
         ]:
             return {
                 "type": "integer",
                 "args": {
                     "min": 0,
                     "max": 1000000,
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["string", "char", "character", "varchar", "text"]:
+            _min = 10
+            _max = 30
+            if arg and arg[0].isdigit():
+                _min = int(arg[0]) // 3
+                _max = int(arg[0])
+
             return {
                 "type": "string",
                 "args": {
-                    "min": 10,
-                    "max": 30,
+                    "min": _min,
+                    "max": _max,
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in [
             "decimal",
             "float",
+            "float4",
+            "float8",
             "dec",
             "numeric",
             "real",
             "double",
         ]:
+            _max = 10000000
+            _round = 2
+            if arg:
+                if ":" in arg[0]:
+                    prec, scale = arg[0].split(":")
+                    if prec:
+                        _max = 10 ** int(prec)
+                    if scale:
+                        _round = int(scale)
+                elif arg[0].isdigit():
+                    _max = 10 ** int(arg[0])
+                    _round = 0
+
             return {
                 "type": "float",
                 "args": {
-                    "max": 10000,
-                    "round": 2,
+                    "max": _max,
+                    "round": _round,
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["time", "timetz"]:
             return {
                 "type": "time",
                 "args": {
                     "start": "07:30:00",
                     "end": "15:30:00",
                     "micros": False,
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["json", "jsonb"]:
             return {
                 "type": "jsonb",
                 "args": {
                     "min": 10,
                     "max": 50,
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                 },
             }
 
         elif datatype.lower() == "date":
             return {
                 "type": "date",
                 "args": {
                     "start": "2022-01-01",
                     "end": "2022-12-31",
                     "format": "%Y-%m-%d",
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["timestamp", "timestamptz"]:
             return {
                 "type": "timestamp",
                 "args": {
                     "start": "2022-01-01",
                     "end": "2022-12-31",
                     "format": "%Y-%m-%d %H:%M:%S.%f",
                     "seed": random.random(),
-                    "null_pct": 0.0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() == "uuid":
             return {
                 "type": "UUIDv4",
                 "args": {
                     "seed": random.random(),
-                    "null_pct": 0,
+                    "null_pct": 0.0
+                    if is_not_null
+                    else round(random.randint(20, 80) / 100, 2),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         else:
             raise ValueError(f"Data type not implemented: '{datatype}'")
 
@@ -470,33 +521,39 @@
         #   s string(30)
         col_def_raw = create_table_stmt[p1 + 1 : p2]
 
         # remove slices delimited by parenthesis
         # eg: from id 'sting(30)' to 'id string'
         # this is important as within parenthesis we might find commas
         # and we need to split on commas later
-        within_brackets = False
+        within_brackets = 0
         col_def = ""
         for i in col_def_raw:
             if i == "(":
-                within_brackets = True
+                within_brackets += 1
+                col_def += " "
                 continue
             if i == ")":
-                within_brackets = False
+                within_brackets -= 1
+                col_def += " "
                 continue
-            if not within_brackets:
+            if within_brackets == 0 or i.isdigit():
                 col_def += i
+            elif within_brackets > 0 and i == ",":
+                col_def += ":"
 
         col_def = [x.strip().lower() for x in col_def.split(",")]
 
         ll = []
         for x in col_def:
             # remove commented lines
             if not x.startswith("--"):
-                col_name_and_type = x.strip().split(" ")[:3]
+                # break it down to tokens
+                col_name_and_type = x.strip().split(" ")
+                col_name_and_type = [x for x in col_name_and_type if x]
                 # remove those lines that are not column definition,
                 # like CONSTRAINT, INDEX, FAMILY, etc..
                 if col_name_and_type[0].lower() not in RESERVED_WORDS:
                     ll.append(col_name_and_type)
 
         table_list = []
         table_list.append({"count": count})
@@ -527,14 +584,15 @@
         # keep only string that start with 'create' and
         # have word 'table' between beginning and the first open parenthesis
         create_table_stmts = []
         for i in stmts:
             p1 = i.find("(")
             if i.startswith("create"):
                 if "table" in i[:p1].lower():
+                    i = i[: i.find("with")]
                     create_table_stmts.append(i)
 
         return create_table_stmts
 
     stmts = get_create_table_stmts(ddl)
 
     d = {}
```

### Comparing `pgworkload-0.1.7/pgworkload/utils/simplefaker.py` & `pgworkload-0.1.8/pgworkload/utils/simplefaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import multiprocessing as mp
 import os
 import pandas as pd
 import uuid
 import random
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("pgworkload")
 
 
 class SimpleFaker:
     """Pseudo-random data generator based on
     the random.Random class.
     """
```

### Comparing `pgworkload-0.1.7/pyproject.toml` & `pgworkload-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgworkload"
-version = "0.1.7"
+version = "0.1.8"
 description = "Workload framework for the PostgreSQL protocol"
 authors = ["Fabio Ghirardello"]
 license = "GPLv3+"
 readme = "README.md"
 homepage = "https://github.com/fabiog1901/pgworkload"
 repository = "https://github.com/fabiog1901/pgworkload"
 classifiers = [
```

### Comparing `pgworkload-0.1.7/PKG-INFO` & `pgworkload-0.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgworkload
-Version: 0.1.7
+Version: 0.1.8
 Summary: Workload framework for the PostgreSQL protocol
 Home-page: https://github.com/fabiog1901/pgworkload
 License: GPLv3+
 Author: Fabio Ghirardello
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
@@ -55,80 +55,94 @@
 
 File `bank.yaml` is the data generation definition file.
 For each column of table `ref_data`, we deterministically generate random data.
 This file is meant as a guide to show what type of data can be generated, and what args are required.
 
 File `bank.py` defines the workload.
 The workload is defined as a class object.
-The class defines 3 methods: `init()`, `run()` and the constructor, `__init__()`.
+The class defines 2 methods: `run()` and the constructor, `__init__()`.
 All other methods are part of the application logic of the workload.
 Read the comments along the code for more information.
 
 Let's run the sample **Bank** workload.
 
-### Step 0 - Create Python env
+### Step 0 - env setup
 
 ```bash
 # upgrade pip - must have pip version 20.3+ 
 pip3 install --upgrade pip
 
-# we're now inside our virtual env
 pip3 install pgworkload
 
-# download the bank workload files
 mkdir workloads
+cd workloads
+
 # the workload class
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.py
-# the schema file
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.sql
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.py
+
+# the DDL file
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.sql
+
 # the data generation definition file
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.yaml
-# the arguments to pass at runtime, optional
-wget -P workloads https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.args.yaml
+wget https://raw.githubusercontent.com/fabiog1901/pgworkload/main/workloads/bank.yaml
 ```
 
-### Step 1 - Init the workload
+### Step 1 - init the workload
+
+Make sure your **CockroachDB** cluster or **PostgreSQL** server is up and running.
 
-We assume that your **CockroachDB** cluster or **PostgreSQL** server is up and running.
+Connect to the SQL prompt and load the `bank.sql` file.
+In CockroachDB, you can run
 
-Init the **Bank** workload.
+```sql
+sql> \i bank.sql
+```
+
+Next, generate some CSV data to seed the database:
 
 ```bash
-# CockroachDB
-pgworkload init -w workloads/bank.py --url 'postgres://root@localhost:26257/postgres?sslmode=disable'
+pgworkload util csv -i bank.yaml -x 1
+```
 
-# PostgreSQL
-pgworkload init --w workloads/bank.py --url 'postgres://root@localhost:5432/postgres?sslmode=disable'
+The CSV files will be located inside a `bank` directory.
+
+```bash
+$ ls -lh bank
+total 1032
+-rw-r--r--  1 fabio  staff   513K Apr  9 13:01 ref_data.0_0_0.csv
 ```
 
-You should see something like below
+Now you can import the CSV file.
+In CockroachDB, my favorite method is to use a webserver to serve the CSV file.
+Open a new terminal then start a simple python server
 
-```text
-2022-01-28 17:21:47,335 [INFO] (MainProcess 29422) URL: 'postgres://root@localhost:[5432|26257]/defaultdb?sslmode=disable&application_name=Bank'
-2022-01-28 17:21:47,480 [INFO] (MainProcess 29422) Database 'bank' created.
-2022-01-28 17:21:47,769 [INFO] (MainProcess 29422) Created workload schema
-2022-01-28 17:21:47,789 [INFO] (MainProcess 29422) Generating dataset for table 'ref_data'
-2022-01-28 17:22:07,088 [INFO] (MainProcess 29422) Importing data for table 'ref_data'
-2022-01-28 17:22:21,063 [INFO] (MainProcess 29422) Init completed. Please update your database connection url to 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank'
+```bash
+cd workloads
+cd bank
+python3 -m http.server 3000
 ```
 
-`pgworkload` has read file `bank.sql` and has created the database and its schema.
-It has then read file `bank.yaml` and has generated the CSV files for the table `ref_data`.
-Finally, it imports the CSV files into database `bank`.
+If you open your browser at <http://localhost:3000> you should see file `ref_data.0_0_0.csv` being served.
+
+At the SQL prompt, import the file
+
+```sql
+sql> IMPORT INTO ref_data CSV DATA ('http://localhost:3000/ref_data.0_0_0.csv') WITH delimiter = e'\t'; 
+```
 
 ### Step 2 - Run the workload
 
 Run the workload using 8 connections for 120 seconds or 100k cycles, whichever comes first.
 
 ```bash
 # CockroachDB
-pgworkload run -w workloads/bank.py -c 8 --url 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
+pgworkload run -w bank.py -c 8 --url 'postgres://root@localhost:26257/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
 
 # PostgreSQL
-pgworkload run -w workloads/bank.py -c 8 --url 'postgres://root@localhost:5432/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
+pgworkload run -w bank.py -c 8 --url 'postgres://root@localhost:5432/bank?sslmode=disable&application_name=Bank' -d 120 -i 100000
 ```
 
 `pgworkload` uses exclusively the excellent [Psycopg 3](https://www.psycopg.org/psycopg3/docs/) to connect.
 No other ORMs or drivers/libraries are used.
 Psycopg has a very simple, neat way to [create connections and execute statements](https://www.psycopg.org/psycopg3/docs/basic/usage.html) and [transactions](https://www.psycopg.org/psycopg3/docs/basic/transactions.html).
 
 `pgworkload` will output something like below
@@ -158,36 +172,69 @@
 There are many built-in options.
 Check them out with
 
 ```bash
 pgworkload --help
 ```
 
+## How it works
+
+It’s helpful to understand first what `pgworkload` does:
+
+- At runtime, `pgworkload` first imports the class you pass, `bank.py`.
+- It spawns _n_ threads for concurrent execution (see next section on Concurrency).
+- By default, it sets the connection to `autocommit` mode.
+- **psycopg v3** will _PREPARE_ statements automatically after 5 executions.
+- Each thread creates a database connection - no need for a connection pool.
+- In a loop, `pgworkload` will:
+  - execute function `run()` which returns a list of functions.
+  - execute each function in the list sequentially. Each function, typically, executes a SQL statement/transaction.
+- Execution stats are funneled back to the _MainThread_, which aggregates and prints them to _stdout_.
+- If the connection drops, it will recreate it. You can also program how long you want the connection to last.
+- `pgworkload` stops once a limit has been reached (iteration/duration), or you Ctrl+C.
+
 ## Concurrency - processes and threads
 
-pgworkload uses both the `multiprocessing` and `threading` library to achieve high concurrency, that is, opening multiple connections to the DBMS.
+`pgworkload` uses both the `multiprocessing` and `threading` library to achieve high concurrency, that is, opening multiple connections to the DBMS.
 
 There are 2 parameters that can be used to configure how many processes you want to create, and for each process, how many threads:
 
 - `--procs`, or `-x`, to configure the count of processes (defaults to the CPU count)
 - `--concurrency`, or `-c`, to configure the total number of executing workloads to run (also referred to as _executing threads_)
 
-pgworkload will spread the load across the processes, so that each process has an even amount of threads.
+`pgworkload` will spread the load across the processes, so that each process has an even amount of threads.
 
 Example: if we set `--procs 4` and `--concurrency 10`, pgworkload will create as follows:
 
 - Process-1: MainThread + 2 extra threads. Total = 3
 - Process-2: MainThread + 2 extra threads. Total = 3
 - Process-3: MainThread + 1 extra thread.  Total = 2
 - Process-3: MainThread + 1 extra thread.  Total = 2
 
 Total workloads = 10
 
 This allows you to fine tune the count of Python processes and threads to fit your system.
 
+## Generating CSV files
+
+- You can seed a database quickly by letting pgworkload generate pseudo-random data and import it.
+- `pgworkload` takes the DDL as an input and creates an intermediate YAML file, with the definition of what data you want to create (a string, a number, a date, a bool..) based on the column data type.
+- You then refine the YAML file to suit your needs, for example, the size of the string, a range for a date, the precision for a decimal, a choice among a discrete list of values..
+- You can also specify what is the percentage of NULL for any column, or how many elements in an ARRAY type.
+- You then specify the total row count, how many rows per file, and in what order, if any, to sort by.
+- Then `pgworkload` will generate the data into CSV or TSV files, compress them if so requested.
+
+Write up: <https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4>
+
+Find out more on the `yaml` and `csv` commands by running
+
+```bash
+pgworkload util --help
+```
+
 ## Built-in Workloads
 
 `pgworkload` has the following workload already built-in and can be called without the need to pass a class file
 
 ### Querybench
 
 Querybench runs a list of SQL Statements sequentially and iteratively.
@@ -209,15 +256,11 @@
 
 Run **Querybench** like this:
 
 ```bash
 pgworkload run --builtin-workload Querybench --args mystmts.sql --url <conn-string>
 ```
 
-### Hovr
-
-Coming soon
-
 ## Acknowledgments
 
 Some methods and classes have been taken and modified from, or inspired by, <https://github.com/cockroachdb/movr>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

