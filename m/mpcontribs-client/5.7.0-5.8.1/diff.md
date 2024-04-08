# Comparing `tmp/mpcontribs-client-5.7.0.tar.gz` & `tmp/mpcontribs-client-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.7.0.tar", last modified: Fri Feb  2 21:26:44 2024, max compression
+gzip compressed data, was "mpcontribs-client-5.8.1.tar", last modified: Mon Apr  8 22:10:06 2024, max compression
```

## Comparing `mpcontribs-client-5.7.0.tar` & `mpcontribs-client-5.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.952535 mpcontribs-client-5.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-02 21:26:44.952535 mpcontribs-client-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.948535 mpcontribs-client-5.7.0/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.948535 mpcontribs-client-5.7.0/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    92632 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.952535 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-02 21:26:44.000000 mpcontribs-client-5.7.0/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.948535 mpcontribs-client-5.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 21:26:44.952535 mpcontribs-client-5.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 21:26:44.952535 mpcontribs-client-5.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-02 21:26:35.000000 mpcontribs-client-5.7.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.079616 mpcontribs-client-5.8.1/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.079616 mpcontribs-client-5.8.1/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    96520 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 22:10:06.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 22:10:05.000000 mpcontribs-client-5.8.1/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:10:06.083616 mpcontribs-client-5.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-08 22:09:59.000000 mpcontribs-client-5.8.1/tests/test_client.py
```

### Comparing `mpcontribs-client-5.7.0/LICENSE` & `mpcontribs-client-5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.7.0/PKG-INFO` & `mpcontribs-client-5.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.7.0
+Version: 5.8.1
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.7.0/README.md` & `mpcontribs-client-5.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.7.0/mpcontribs/client/__init__.py` & `mpcontribs-client-5.8.1/mpcontribs/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,23 +70,24 @@
 MAX_BYTES = 2.4 * MEGABYTES
 MAX_PAYLOAD = 15 * MEGABYTES
 MAX_COLUMNS = 160
 DEFAULT_HOST = "contribs-api.materialsproject.org"
 BULMA = "is-narrow is-fullwidth has-background-light"
 PROVIDERS = {"github", "google", "facebook", "microsoft", "amazon"}
 COMPONENTS = ["structures", "tables", "attachments"]  # using list to maintain order
-SUBDOMAINS = ["contribs", "lightsources", "ml", "micro"]
+SUBDOMAINS = ["contribs", "ml", "micro"]
 PORTS = [5000, 5002, 5003, 5005, 10000, 10002, 10003, 10005, 20000]
 HOSTS = ["localhost", "contribs-apis"]
 HOSTS += [f"192.168.0.{i}" for i in range(36, 47)]  # PrivateSubnetOne
 HOSTS += [f"192.168.0.{i}" for i in range(52, 63)]  # PrivateSubnetTwo
 VALID_URLS = {f"http://{h}:{p}" for p in PORTS for h in HOSTS}
 VALID_URLS |= {
     f"https://{n}-api{m}.materialsproject.org"
-    for n in SUBDOMAINS for m in ["", "-preview"]
+    for n in SUBDOMAINS
+    for m in ["", "-preview"]
 }
 VALID_URLS |= {f"http://localhost.{n}-api.materialsproject.org" for n in SUBDOMAINS}
 SUPPORTED_FILETYPES = (Gz, Jpeg, Png, Gif, Tiff)
 SUPPORTED_MIMES = [t().mime for t in SUPPORTED_FILETYPES]
 DEFAULT_DOWNLOAD_DIR = Path.home() / "mpcontribs-downloads"
 
 j2h = Json2Html()
@@ -109,44 +110,44 @@
 ureg.define("atom = 1")
 ureg.define("bohr_magneton = e * hbar / (2 * m_e) = µᵇ = µ_B = mu_B")
 ureg.define("electron_mass = 9.1093837015e-31 kg = mₑ = m_e")
 
 LOG_LEVEL = os.environ.get("MPCONTRIBS_CLIENT_LOG_LEVEL", "INFO")
 log_level = getattr(logging, LOG_LEVEL.upper())
 _session = requests.Session()
-_ipython = sys.modules['IPython'].get_ipython()
+_ipython = sys.modules["IPython"].get_ipython()
 
 
 class LogFilter(logging.Filter):
     def __init__(self, level, *args, **kwargs):
         self.level = level
         super(LogFilter, self).__init__(*args, **kwargs)
 
     def filter(self, record):
         return record.levelno < self.level
 
 
 class CustomLoggerAdapter(logging.LoggerAdapter):
     def process(self, msg, kwargs):
-        prefix = self.extra.get('prefix')
+        prefix = self.extra.get("prefix")
         return f"[{prefix}] {msg}" if prefix else msg, kwargs
 
 
 class TqdmToLogger(io.StringIO):
     logger = None
     level = None
-    buf = ''
+    buf = ""
 
     def __init__(self, logger, level=None):
         super(TqdmToLogger, self).__init__()
         self.logger = logger
         self.level = level or logging.INFO
 
     def write(self, buf):
-        self.buf = buf.strip('\r\n\t ')
+        self.buf = buf.strip("\r\n\t ")
 
     def flush(self):
         self.logger.log(self.level, self.buf)
 
 
 def get_logger(name):
     logger = logging.getLogger(name)
@@ -173,15 +174,17 @@
 def get_md5(d):
     s = ujson.dumps(d, sort_keys=True).encode("utf-8")
     return md5(s).hexdigest()
 
 
 def validate_email(email_string):
     if email_string.count(":") != 1:
-        raise SwaggerValidationError(f"{email_string} not of format <provider>:<email>.")
+        raise SwaggerValidationError(
+            f"{email_string} not of format <provider>:<email>."
+        )
 
     provider, email = email_string.split(":", 1)
     if provider not in PROVIDERS:
         raise SwaggerValidationError(f"{provider} is not a valid provider.")
 
     d = is_email(email, diagnose=True)
     if d > BaseDiagnosis.CATEGORIES["VALID"]:
@@ -200,15 +203,19 @@
 def validate_url(url_string, qualifying=("scheme", "netloc")):
     tokens = urlparse(url_string)
     if not all([getattr(tokens, qual_attr) for qual_attr in qualifying]):
         raise SwaggerValidationError(f"{url_string} invalid")
 
 
 url_format = SwaggerFormat(
-    format="url", to_wire=str, to_python=str, validate=validate_url, description="URL",
+    format="url",
+    to_wire=str,
+    to_python=str,
+    validate=validate_url,
+    description="URL",
 )
 bravado_config_dict = {
     "validate_responses": False,
     "use_models": False,
     "include_missing_properties": False,
     "formats": [email_format, url_format],
 }
@@ -231,31 +238,34 @@
 def _compress(data):
     data_json = ujson.dumps(data, indent=4).encode("utf-8")
     content = gzip.compress(data_json)
     return len(content), content
 
 
 def get_session(session=None):
-    adapter_kwargs = dict(max_retries=Retry(
-        total=RETRIES,
-        read=RETRIES,
-        connect=RETRIES,
-        respect_retry_after_header=True,
-        status_forcelist=[429, 502],  # rate limit
-        allowed_methods={'DELETE', 'GET', 'PUT', 'POST'},
-        backoff_factor=2
-    ))
+    adapter_kwargs = dict(
+        max_retries=Retry(
+            total=RETRIES,
+            read=RETRIES,
+            connect=RETRIES,
+            respect_retry_after_header=True,
+            status_forcelist=[429, 502],  # rate limit
+            allowed_methods={"DELETE", "GET", "PUT", "POST"},
+            backoff_factor=2,
+        )
+    )
     return FuturesSession(
         session=session if session else _session,
-        max_workers=MAX_WORKERS, adapter_kwargs=adapter_kwargs
+        max_workers=MAX_WORKERS,
+        adapter_kwargs=adapter_kwargs,
     )
 
 
 def _response_hook(resp, *args, **kwargs):
-    content_type = resp.headers['content-type']
+    content_type = resp.headers["content-type"]
     if content_type == "application/json":
         result = resp.json()
 
         if isinstance(result, dict):
             if "data" in result and isinstance(result["data"], list):
                 resp.result = result
                 resp.count = len(result["data"])
@@ -274,15 +284,15 @@
         resp.result = resp.content
         resp.count = 1
     else:
         logger.error(f"request failed with status {resp.status_code}!")
         resp.count = 0
 
 
-def _chunk_by_size(items, max_size=0.95*MAX_BYTES):
+def _chunk_by_size(items, max_size=0.95 * MAX_BYTES):
     buffer, buffer_size = [], 0
 
     for idx, item in enumerate(items):
         item_size = _compress(item)[0]
 
         if buffer_size + item_size <= max_size:
             buffer.append(item)
@@ -299,38 +309,45 @@
 def visit(path, key, value):
     if isinstance(value, dict) and "display" in value:
         return key, value["display"]
     return True
 
 
 def _in_ipython():
-    return _ipython is not None and 'IPKernelApp' in _ipython.config
+    return _ipython is not None and "IPKernelApp" in _ipython.config
 
 
 if _in_ipython():
+
     def _hide_traceback(
-        exc_tuple=None, filename=None, tb_offset=None,
-        exception_only=False, running_compiled_code=False
+        exc_tuple=None,
+        filename=None,
+        tb_offset=None,
+        exception_only=False,
+        running_compiled_code=False,
     ):
         etype, value, tb = sys.exc_info()
 
-        if issubclass(etype, (MPContribsClientError, SwaggerValidationError, ValidationError)):
+        if issubclass(
+            etype, (MPContribsClientError, SwaggerValidationError, ValidationError)
+        ):
             return _ipython._showtraceback(
                 etype, value, _ipython.InteractiveTB.get_exception_only(etype, value)
             )
 
         return _ipython._showtraceback(
             etype, value, _ipython.InteractiveTB(etype, value, tb)
         )
 
     _ipython.showtraceback = _hide_traceback
 
 
 class Dict(dict):
     """Custom dictionary to display itself as HTML table with Bulma CSS"""
+
     def display(self, attrs: str = f'class="table {BULMA}"'):
         """Nice table display of dictionary
 
         Args:
             attrs (str): table attributes to forward to Json2Html.convert
         """
         html = j2h.convert(json=remap(self, visit=visit), table_attributes=attrs)
@@ -338,14 +355,15 @@
             return display(HTML(html))
 
         return html
 
 
 class Table(pd.DataFrame):
     """Wrapper class around pandas.DataFrame to provide display() and info()"""
+
     def display(self):
         """Display a plotly graph for the table if in IPython/Jupyter"""
         if _in_ipython():
             try:
                 allowed_kwargs = getfullargspec(line_chart).args
                 attrs = {k: v for k, v in self.attrs.items() if k in allowed_kwargs}
                 return self.plot(**attrs)
@@ -382,15 +400,15 @@
         ret = cls(df)
         ret.attrs = {k: v for k, v in dct["attrs"].items()}
         return ret
 
     def _clean(self):
         """clean the dataframe"""
         self.replace([np.inf, -np.inf], np.nan, inplace=True)
-        self.fillna('', inplace=True)
+        self.fillna("", inplace=True)
         self.index = self.index.astype(str)
         for col in self.columns:
             self[col] = self[col].astype(str)
 
     def _attrs_as_dict(self):
         name = self.attrs.get("name", "table")
         title = self.attrs.get("title", name)
@@ -411,14 +429,15 @@
         dct = self.to_dict(orient="split")
         dct["name"], dct["attrs"] = self._attrs_as_dict()
         return dct
 
 
 class Structure(PmgStructure):
     """Wrapper class around pymatgen.Structure to provide display() and info()"""
+
     def display(self):
         return self  # TODO use static image from crystal toolkit?
 
     def info(self) -> Type[Dict]:
         """Show summary info for structure"""
         info = Dict((k, v) for k, v in self.attrs.items())
         info["formula"] = self.composition.formula
@@ -436,14 +455,15 @@
         ret = super().from_dict(dct)
         ret.attrs = {field: dct[field] for field in ["id", "name", "md5"]}
         return ret
 
 
 class Attachment(dict):
     """Wrapper class around dict to handle attachments"""
+
     def decode(self) -> str:
         """Decode base64-encoded content of attachment"""
         return b64decode(self["content"], validate=True)
 
     def unpack(self) -> str:
         unpacked = self.decode()
 
@@ -505,15 +525,15 @@
 
         if size > MAX_BYTES:
             raise MPContribsClientError(f"{name} too large ({size} > {MAX_BYTES})!")
 
         return cls(
             name=filename,
             mime="application/gzip",
-            content=b64encode(content).decode("utf-8")
+            content=b64encode(content).decode("utf-8"),
         )
 
     @classmethod
     def from_file(cls, path: Union[Path, str]):
         """Construct attachment from file
 
         Args:
@@ -541,15 +561,15 @@
 
         if size > MAX_BYTES:
             raise MPContribsClientError(f"{path} too large ({size} > {MAX_BYTES})!")
 
         return cls(
             name=path.name,
             mime=kind.mime if supported else "application/gzip",
-            content=b64encode(content).decode("utf-8")
+            content=b64encode(content).decode("utf-8"),
         )
 
     @classmethod
     def from_dict(cls, dct: dict):
         """Construct Attachment from dict
 
         Args:
@@ -557,14 +577,15 @@
         """
         keys = {"id", "name", "md5", "content", "mime"}
         return cls((k, v) for k, v in dct.items() if k in keys)
 
 
 class Attachments(list):
     """Wrapper class to handle attachments automatically"""
+
     # TODO implement "plural" versions for Attachment methods
 
     @classmethod
     def from_list(cls, elements: list):
         if not isinstance(elements, list):
             raise MPContribsClientError("use list to init Attachments")
 
@@ -659,15 +680,17 @@
     headers = ujson.loads(headers_json)
 
     if not spec_dict["paths"]:
         url = f"{protocol}://{host}"
         origin_url = f"{url}/apispec.json"
         http_client = RequestsClient()
         http_client.session.headers.update(headers)
-        swagger_spec = Spec.from_dict(spec_dict, origin_url, http_client, bravado_config_dict)
+        swagger_spec = Spec.from_dict(
+            spec_dict, origin_url, http_client, bravado_config_dict
+        )
         http_client.session.close()
         return swagger_spec
 
     # retrieve list of projects accessible to user
     query = {"name": project} if project else {}
     query["_fields"] = ["name"]
     url = f"{protocol}://{host}"
@@ -678,26 +701,28 @@
 
     if project and not resp["data"]:
         raise MPContribsClientError(f"{project} doesn't exist, or access denied!")
 
     projects = sorted(d["name"] for d in resp["data"])
     projects_json = ujson.dumps(projects)
     # expand regex-based query parameters for `data` columns
-    spec = _expand_params(protocol, host, version, projects_json, apikey=headers.get("x-api-key"))
+    spec = _expand_params(
+        protocol, host, version, projects_json, apikey=headers.get("x-api-key")
+    )
     spec.http_client.session.headers.update(headers)
     return spec
 
 
 @functools.lru_cache(maxsize=1)
 def _raw_specs(protocol, host, version):
     http_client = RequestsClient()
     url = f"{protocol}://{host}"
     origin_url = f"{url}/apispec.json"
-    url4fn = origin_url.replace("apispec", f"apispec-{version}").encode('utf-8')
-    fn = urlsafe_b64encode(url4fn).decode('utf-8')
+    url4fn = origin_url.replace("apispec", f"apispec-{version}").encode("utf-8")
+    fn = urlsafe_b64encode(url4fn).decode("utf-8")
     apispec = Path(gettempdir()) / fn
     spec_dict = None
 
     if apispec.exists():
         spec_dict = ujson.loads(apispec.read_bytes())
         logger.debug(f"Specs for {origin_url} and {version} re-loaded from {apispec}.")
     else:
@@ -706,27 +731,29 @@
 
         with apispec.open("w") as f:
             ujson.dump(spec_dict, f)
 
         logger.debug(f"Specs for {origin_url} and {version} saved as {apispec}.")
 
     if not spec_dict:
-        raise MPContribsClientError(f"Couldn't load specs from {url} for {version}!")  # not cached
+        raise MPContribsClientError(
+            f"Couldn't load specs from {url} for {version}!"
+        )  # not cached
 
     spec_dict["host"] = host
     spec_dict["schemes"] = [protocol]
     http_client.session.close()
     return spec_dict
 
 
 @cached(
     cache=LRUCache(maxsize=100),
     key=lambda protocol, host, version, projects_json, **kwargs: hashkey(
         protocol, host, version, projects_json
-    )
+    ),
 )
 def _expand_params(protocol, host, version, projects_json, apikey=None):
     columns = {"string": [], "number": []}
     projects = ujson.loads(projects_json)
     query = {"project__in": ",".join(projects)}
     query["_fields"] = ["columns"]
     url = f"{protocol}://{host}"
@@ -749,64 +776,67 @@
     spec_dict = _raw_specs(protocol, host, version)
     resource = spec_dict["paths"]["/contributions/"]["get"]
     raw_params = resource.pop("parameters")
     params = {}
 
     for param in raw_params:
         if param["name"].startswith("^data__"):
-            op = param["name"].rsplit('$__', 1)[-1]
+            op = param["name"].rsplit("$__", 1)[-1]
             typ = param["type"]
             key = "number" if typ == "number" else "string"
 
             for column in columns[key]:
                 param_name = f"{column}__{op}"
                 if param_name not in params:
                     param_spec = {
-                        k: v for k, v in param.items()
+                        k: v
+                        for k, v in param.items()
                         if k not in ["name", "description"]
                     }
                     param_spec["name"] = param_name
                     params[param_name] = param_spec
         else:
             params[param["name"]] = param
 
     resource["parameters"] = list(params.values())
 
     origin_url = f"{url}/apispec.json"
     spec = Spec(spec_dict, origin_url, http_client, bravado_config_dict)
     model_discovery(spec)
 
-    if spec.config['internally_dereference_refs']:
+    if spec.config["internally_dereference_refs"]:
         spec.deref = _identity
         spec._internal_spec_dict = spec.deref_flattened_spec
 
-    for user_defined_format in spec.config['formats']:
+    for user_defined_format in spec.config["formats"]:
         spec.register_format(user_defined_format)
 
     spec.resources = build_resources(spec)
     spec.api_url = build_api_serving_url(
         spec_dict=spec.spec_dict,
         origin_url=spec.origin_url,
-        use_spec_url_for_base_path=spec.config['use_spec_url_for_base_path'],
+        use_spec_url_for_base_path=spec.config["use_spec_url_for_base_path"],
     )
     http_client.session.close()
     return spec
 
 
 @functools.lru_cache(maxsize=1)
 def _version(url):
     retries, max_retries = 0, 3
     protocol = urlparse(url).scheme
-    is_mock_test = 'pytest' in sys.modules and protocol == "http"
+    is_mock_test = "pytest" in sys.modules and protocol == "http"
 
     if is_mock_test:
         now = datetime.datetime.now()
         return Version(
-            major=now.year, minor=now.month, patch=now.day,
-            prerelease=(str(now.hour), str(now.minute))
+            major=now.year,
+            minor=now.month,
+            patch=now.day,
+            prerelease=(str(now.hour), str(now.minute)),
         )
     else:
         while retries < max_retries:
             try:
                 r = requests.get(f"{url}/healthcheck", timeout=5)
                 if r.status_code in {200, 403}:
                     return r.json().get("version")
@@ -827,14 +857,15 @@
 
     Typical usage:
         - set environment variable MPCONTRIBS_API_KEY to the API key from your MP profile
         - import and init:
           >>> from mpcontribs.client import Client
           >>> client = Client()
     """
+
     def __init__(
         self,
         apikey: str = None,
         headers: dict = None,
         host: str = None,
         project: str = None,
         session: requests.Session = None,
@@ -863,50 +894,56 @@
 
         self.apikey = apikey
         self.headers = headers or {}
         self.headers = {"x-api-key": apikey} if apikey else self.headers
         self.headers["Content-Type"] = "application/json"
         self.headers_json = ujson.dumps(self.headers, sort_keys=True)
         self.host = host
-        ssl = host.endswith(".materialsproject.org") and not host.startswith("localhost.")
+        ssl = host.endswith(".materialsproject.org") and not host.startswith(
+            "localhost."
+        )
         self.protocol = "https" if ssl else "http"
         self.url = f"{self.protocol}://{self.host}"
         self.project = project
 
         if self.url not in VALID_URLS:
-            raise MPContribsClientError(f"{self.url} not a valid URL (one of {VALID_URLS})")
+            raise MPContribsClientError(
+                f"{self.url} not a valid URL (one of {VALID_URLS})"
+            )
 
         self.version = _version(self.url)  # includes healthcheck
         self.session = get_session(session=session)
         super().__init__(self.cached_swagger_spec)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         return None
 
     @property
     def cached_swagger_spec(self):
-        return _load(self.protocol, self.host, self.headers_json, self.project, self.version)
+        return _load(
+            self.protocol, self.host, self.headers_json, self.project, self.version
+        )
 
     def __dir__(self):
         members = set(self.swagger_spec.resources.keys())
         members |= set(k for k in self.__dict__.keys() if not k.startswith("_"))
         members |= set(k for k in dir(self.__class__) if not k.startswith("_"))
         return members
 
     def _reinit(self):
         _load.cache_clear()
         super().__init__(self.cached_swagger_spec)
 
     def _is_valid_payload(self, model: str, data: dict):
         model_spec = deepcopy(self.get_model(f"{model}sSchema")._model_spec)
         model_spec.pop("required")
-        model_spec['additionalProperties'] = False
+        model_spec["additionalProperties"] = False
 
         try:
             validate_object(self.swagger_spec, model_spec, data)
         except ValidationError as ex:
             return False, str(ex)
 
         return True, None
@@ -915,38 +952,44 @@
         for k, v in flatten(dct, reducer="dot").items():
             if v is not None and not isinstance(v, (str, int, float)):
                 error = f"Value {v} of {type(v)} for key {k} not supported."
                 return False, error
 
         return True, None
 
-    def _get_per_page_default_max(self, op: str = "query", resource: str = "contributions") -> int:
+    def _get_per_page_default_max(
+        self, op: str = "query", resource: str = "contributions"
+    ) -> int:
         attr = f"{op}{resource.capitalize()}"
         resource = self.swagger_spec.resources[resource]
         param_spec = getattr(resource, attr).params["per_page"].param_spec
         return param_spec["default"], param_spec["maximum"]
 
     def _get_per_page(
         self, per_page: int = -1, op: str = "query", resource: str = "contributions"
     ) -> int:
-        per_page_default, per_page_max = self._get_per_page_default_max(op=op, resource=resource)
+        per_page_default, per_page_max = self._get_per_page_default_max(
+            op=op, resource=resource
+        )
         if per_page < 0:
             per_page = per_page_default
         return min(per_page_max, per_page)
 
     def _split_query(
         self,
         query: dict,
         op: str = "query",
         resource: str = "contributions",
         pages: int = -1,
     ) -> List[dict]:
         """Avoid URI too long errors"""
         pp_default, pp_max = self._get_per_page_default_max(op=op, resource=resource)
-        per_page = pp_default if any(k.endswith("__in") for k in query.keys()) else pp_max
+        per_page = (
+            pp_default if any(k.endswith("__in") for k in query.keys()) else pp_max
+        )
         nr_params_to_split = sum(
             len(v) > per_page for v in query.values() if isinstance(v, list)
         )
         if nr_params_to_split > 1:
             raise MPContribsClientError(
                 f"More than one list in query with length > {per_page} not supported!"
             )
@@ -969,15 +1012,15 @@
         query["per_page"] = per_page
 
         if not queries:
             queries = [query]
 
         if len(queries) == 1 and pages and pages > 0:
             queries = []
-            for page in range(1, pages+1):
+            for page in range(1, pages + 1):
                 queries.append(deepcopy(query))
                 queries[-1]["page"] = page
 
         for q in queries:
             # copy over missing parameters
             for k, v in query.items():
                 if k not in q:
@@ -992,76 +1035,71 @@
 
     def _get_future(
         self,
         track_id,
         params: dict,
         rel_url: str = "contributions",
         op: str = "query",
-        data: dict = None
+        data: dict = None,
     ):
         rname = rel_url.split("/", 1)[0]
         resource = self.swagger_spec.resources[rname]
         attr = f"{op}{rname.capitalize()}"
         method = getattr(resource, attr).http_method
         kwargs = dict(
-            headers=self.headers, params=params, hooks={'response': _response_hook}
+            headers=self.headers, params=params, hooks={"response": _response_hook}
         )
 
         if method == "put" and data:
             kwargs["data"] = ujson.dumps(data).encode("utf-8")
 
-        future = getattr(self.session, method)(
-            f"{self.url}/{rel_url}/", **kwargs
-        )
+        future = getattr(self.session, method)(f"{self.url}/{rel_url}/", **kwargs)
         setattr(future, "track_id", track_id)
         return future
 
     def available_query_params(
-        self,
-        startswith: tuple = None,
-        resource: str = "contributions"
+        self, startswith: tuple = None, resource: str = "contributions"
     ) -> list:
         resources = self.swagger_spec.resources
         resource_obj = resources.get(resource)
         if not resource_obj:
             available_resources = list(resources.keys())
             raise MPContribsClientError(f"Choose one of {available_resources}!")
 
         op_key = f"query{resource.capitalize()}"
         operation = resource_obj.operations[op_key]
         params = [param.name for param in operation.params.values()]
         if not startswith:
             return params
 
-        return [
-            param for param in params
-            if param.startswith(startswith)
-        ]
+        return [param for param in params if param.startswith(startswith)]
 
     def get_project(self, name: str = None, fields: list = None) -> Type[Dict]:
         """Retrieve a project entry
 
         Args:
             name (str): name of the project
             fields (list): list of fields to include in response
         """
         name = self.project or name
         if not name:
-            raise MPContribsClientError("initialize client with project or set `name` argument!")
+            raise MPContribsClientError(
+                "initialize client with project or set `name` argument!"
+            )
 
         fields = fields or ["_all"]  # retrieve all fields by default
         return Dict(self.projects.getProjectByName(pk=name, _fields=fields).result())
 
     def query_projects(
         self,
         query: dict = None,
         term: str = None,
         fields: list = None,
         sort: str = None,
-        timeout: int = -1
+        timeout: int = -1,
     ) -> List[dict]:
         """Query projects by query and/or term (Atlas Search)
 
         See `client.available_query_params(resource="projects")` for keyword arguments used in
         query. Provide `term` to search for a term across all text fields in the project infos.
 
         Args:
@@ -1076,25 +1114,28 @@
         """
         query = query or {}
 
         if self.project or "name" in query:
             return [self.get_project(name=query.get("name"), fields=fields)]
 
         if term:
+
             def search_future(search_term):
                 future = self.session.get(
                     f"{self.url}/projects/search",
                     headers=self.headers,
-                    hooks={'response': _response_hook},
+                    hooks={"response": _response_hook},
                     params={"term": search_term},
                 )
                 setattr(future, "track_id", "search")
                 return future
 
-            responses = _run_futures([search_future(term)], timeout=timeout, disable=True)
+            responses = _run_futures(
+                [search_future(term)], timeout=timeout, disable=True
+            )
             query["name__in"] = responses["search"].get("result", [])
 
         if fields:
             query["_fields"] = fields
         if sort:
             query["_sort"] = sort
 
@@ -1106,27 +1147,31 @@
 
         for field in ["name__in", "_fields"]:
             if field in query:
                 query[field] = ",".join(query[field])
 
         queries = []
 
-        for page in range(2, total_pages+1):
+        for page in range(2, total_pages + 1):
             queries.append(deepcopy(query))
             queries[-1]["page"] = page
 
-        futures = [self._get_future(i, q, rel_url="projects") for i, q in enumerate(queries)]
+        futures = [
+            self._get_future(i, q, rel_url="projects") for i, q in enumerate(queries)
+        ]
         responses = _run_futures(futures, total=total_count, timeout=timeout)
 
         for resp in responses.values():
             ret["data"] += resp["result"]["data"]
 
         return ret["data"]
 
-    def create_project(self, name: str, title: str, authors: str, description: str, url: str):
+    def create_project(
+        self, name: str, title: str, authors: str, description: str, url: str
+    ):
         """Create a project
 
         Args:
             name (str): unique name matching `^[a-zA-Z0-9_]{3,31}$`
             title (str): unique title with 5-30 characters
             authors (str): comma-separated list of authors
             description (str): brief description (max 1500 characters)
@@ -1134,16 +1179,19 @@
         """
         queries = [{"name": name}, {"title": title}]
         for query in queries:
             if self.get_totals(query=query, resource="projects")[0]:
                 raise MPContribsClientError(f"Project with {query} already exists!")
 
         project = {
-            "name": name, "title": title, "authors": authors, "description": description,
-            "references": [{"label": "REF", "url": url}]
+            "name": name,
+            "title": title,
+            "authors": authors,
+            "description": description,
+            "references": [{"label": "REF", "url": url}],
         }
         resp = self.projects.createProject(project=project).result()
         owner = resp.get("owner")
         if owner:
             logger.info(f"Project `{name}` created with owner `{owner}`")
         elif "error" in resp:
             raise MPContribsClientError(resp["error"])
@@ -1159,25 +1207,31 @@
         """
         if not update:
             logger.warning("nothing to update")
             return
 
         name = self.project or name
         if not name:
-            raise MPContribsClientError("initialize client with project or set `name` argument!")
+            raise MPContribsClientError(
+                "initialize client with project or set `name` argument!"
+            )
 
         disallowed = ["is_approved", "stats", "columns", "is_public", "owner"]
         for k in list(update.keys()):
             if k in disallowed:
                 logger.warning(f"removing `{k}` from update - not allowed.")
                 update.pop(k)
                 if k == "columns":
-                    logger.info("use `client.init_columns()` to update project columns.")
+                    logger.info(
+                        "use `client.init_columns()` to update project columns."
+                    )
                 elif k == "is_public":
-                    logger.info("use `client.make_public/private()` to set `is_public`.")
+                    logger.info(
+                        "use `client.make_public/private()` to set `is_public`."
+                    )
             elif not isinstance(update[k], bool) and not update[k]:
                 logger.warning(f"removing `{k}` from update - no update requested.")
                 update.pop(k)
 
         if not update:
             logger.warning("nothing to update")
             return
@@ -1192,16 +1246,15 @@
         # allow name update only if no contributions in project
         if "name" in update and project["stats"]["contributions"] > 0:
             logger.warning("removing `name` from update - not allowed.")
             update.pop("name")
             logger.error("cannot change project name after contributions submitted.")
 
         payload = {
-            k: v for k, v in update.items()
-            if k in fields and project.get(k, None) != v
+            k: v for k, v in update.items() if k in fields and project.get(k, None) != v
         }
         if not payload:
             logger.warning("nothing to update")
             return
 
         valid, error = self._is_valid_payload("Project", payload)
         if valid:
@@ -1215,15 +1268,17 @@
         """Delete a project
 
         Args:
             name (str): name of the project
         """
         name = self.project or name
         if not name:
-            raise MPContribsClientError("initialize client with project or set `name` argument!")
+            raise MPContribsClientError(
+                "initialize client with project or set `name` argument!"
+            )
 
         if not self.get_totals(query={"name": name}, resource="projects")[0]:
             raise MPContribsClientError(f"Project `{name}` doesn't exist!")
 
         resp = self.projects.deleteProjectByName(pk=name).result()
         if resp and "error" in resp:
             raise MPContribsClientError(resp["error"])
@@ -1234,25 +1289,29 @@
         Args:
             cid (str): contribution ObjectID
             fields (list): list of fields to include in response
         """
         if not fields:
             fields = list(self.get_model("ContributionsSchema")._properties.keys())
             fields.remove("needs_build")  # internal field
-        return Dict(self.contributions.getContributionById(pk=cid, _fields=fields).result())
+        return Dict(
+            self.contributions.getContributionById(pk=cid, _fields=fields).result()
+        )
 
     def get_table(self, tid_or_md5: str) -> Type[Table]:
         """Retrieve full Pandas DataFrame for a table
 
         Args:
             tid_or_md5 (str): ObjectId or MD5 hash digest for table
         """
         str_len = len(tid_or_md5)
         if str_len not in {24, 32}:
-            raise MPContribsClientError(f"'{tid_or_md5}' is not a valid table id or md5 hash!")
+            raise MPContribsClientError(
+                f"'{tid_or_md5}' is not a valid table id or md5 hash!"
+            )
 
         if str_len == 32:
             tables = self.tables.queryTables(md5=tid_or_md5, _fields=["id"]).result()
             if not tables:
                 raise MPContribsClientError(f"table for md5 '{tid_or_md5}' not found!")
             tid = tables["data"][0]["id"]
         else:
@@ -1284,20 +1343,26 @@
         """Retrieve pymatgen structure
 
         Args:
             sid_or_md5 (str): ObjectId or MD5 hash digest for structure
         """
         str_len = len(sid_or_md5)
         if str_len not in {24, 32}:
-            raise MPContribsClientError(f"'{sid_or_md5}' is not a valid structure id or md5 hash!")
+            raise MPContribsClientError(
+                f"'{sid_or_md5}' is not a valid structure id or md5 hash!"
+            )
 
         if str_len == 32:
-            structures = self.structures.queryStructures(md5=sid_or_md5, _fields=["id"]).result()
+            structures = self.structures.queryStructures(
+                md5=sid_or_md5, _fields=["id"]
+            ).result()
             if not structures:
-                raise MPContribsClientError(f"structure for md5 '{sid_or_md5}' not found!")
+                raise MPContribsClientError(
+                    f"structure for md5 '{sid_or_md5}' not found!"
+                )
             sid = structures["data"][0]["id"]
         else:
             sid = sid_or_md5
 
         fields = list(self.get_model("StructuresSchema")._properties.keys())
         resp = self.structures.getStructureById(pk=sid, _fields=fields).result()
         return Structure.from_dict(resp)
@@ -1306,27 +1371,33 @@
         """Retrieve an attachment
 
         Args:
             aid_or_md5 (str): ObjectId or MD5 hash digest for attachment
         """
         str_len = len(aid_or_md5)
         if str_len not in {24, 32}:
-            raise MPContribsClientError(f"'{aid_or_md5}' is not a valid attachment id or md5 hash!")
+            raise MPContribsClientError(
+                f"'{aid_or_md5}' is not a valid attachment id or md5 hash!"
+            )
 
         if str_len == 32:
             attachments = self.attachments.queryAttachments(
                 md5=aid_or_md5, _fields=["id"]
             ).result()
             if not attachments:
-                raise MPContribsClientError(f"attachment for md5 '{aid_or_md5}' not found!")
+                raise MPContribsClientError(
+                    f"attachment for md5 '{aid_or_md5}' not found!"
+                )
             aid = attachments["data"][0]["id"]
         else:
             aid = aid_or_md5
 
-        return Attachment(self.attachments.getAttachmentById(pk=aid, _fields=["_all"]).result())
+        return Attachment(
+            self.attachments.getAttachmentById(pk=aid, _fields=["_all"]).result()
+        )
 
     def init_columns(self, columns: dict = None) -> dict:
         """initialize columns for a project to set their order and desired units
 
         The `columns` field of a project tracks the minima and maxima of each `data` field
         in its contributions. If columns are not initialized before submission using this
         function, `submit_contributions` will respect the order of columns as they are
@@ -1362,61 +1433,70 @@
 
         columns = flatten(columns or {}, reducer="dot")
 
         if len(columns) > MAX_COLUMNS:
             raise MPContribsClientError(f"Number of columns larger than {MAX_COLUMNS}!")
 
         if not all(isinstance(v, str) for v in columns.values() if v is not None):
-            raise MPContribsClientError("All values in `columns` need to be None or of type str!")
+            raise MPContribsClientError(
+                "All values in `columns` need to be None or of type str!"
+            )
 
         new_columns = []
 
         if columns:
             # check columns input
             scanned_columns = set()
 
             for k, v in columns.items():
                 if k in COMPONENTS:
                     scanned_columns.add(k)
                     continue
 
                 nesting = k.count(".")
                 if nesting > MAX_NESTING:
-                    raise MPContribsClientError(f"Nesting depth larger than {MAX_NESTING} for {k}!")
+                    raise MPContribsClientError(
+                        f"Nesting depth larger than {MAX_NESTING} for {k}!"
+                    )
 
                 for col in scanned_columns:
                     if nesting and col.startswith(k):
-                        raise MPContribsClientError(f"Duplicate definition of {k} in {col}!")
+                        raise MPContribsClientError(
+                            f"Duplicate definition of {k} in {col}!"
+                        )
 
-                    for n in range(1, nesting+1):
+                    for n in range(1, nesting + 1):
                         if k.rsplit(".", n)[0] == col:
                             raise MPContribsClientError(
                                 f"Ancestor of {k} already defined in {col}!"
                             )
 
                 is_valid_string = isinstance(v, str) and v.lower() != "nan"
                 if not is_valid_string and v is not None:
                     raise MPContribsClientError(
                         f"Unit '{v}' for {k} invalid (use `None` or a non-NaN string)!"
                     )
 
                 if v != "" and v is not None and v not in ureg:
-                    raise MPContribsClientError(f"Unit '{v}' for {k} invalid!")
+                    raise MPContribsClientError(f"Unit '{v}' for {k} not supported!")
 
                 scanned_columns.add(k)
 
             # sort to avoid "overlapping columns" error in handsontable's NestedHeaders
             sorted_columns = flatten(unflatten(columns, splitter="dot"), reducer="dot")
             # also sort by increasing nesting for better columns display
             sorted_columns = dict(
                 sorted(sorted_columns.items(), key=lambda item: item[0].count("."))
             )
 
+            # TODO catch unsupported column renaming or implement solution
             # reconcile with existing columns
-            resp = self.projects.getProjectByName(pk=self.project, _fields=["columns"]).result()
+            resp = self.projects.getProjectByName(
+                pk=self.project, _fields=["columns"]
+            ).result()
             existing_columns = {}
 
             for col in resp["columns"]:
                 path = col.pop("path")
                 existing_columns[path] = col
 
             for path, unit in sorted_columns.items():
@@ -1433,37 +1513,49 @@
 
                 if existing_column:
                     # NOTE if existing_unit == "NaN":
                     #   it was set by omitting "unit" in new_column
                     new_unit = new_column.get("unit", "NaN")
                     existing_unit = existing_column.get("unit")
                     if existing_unit != new_unit:
+                        conv_args = []
+                        for u in [existing_unit, new_unit]:
+                            try:
+                                conv_args.append(ureg.Unit(u))
+                            except ValueError:
+                                raise MPContribsClientError(
+                                    f"Can't convert {existing_unit} to {new_unit} for {path}"
+                                )
                         try:
-                            factor = ureg.convert(1, ureg.Unit(existing_unit), ureg.Unit(new_unit))
+                            factor = ureg.convert(1, *conv_args)
                         except DimensionalityError:
                             raise MPContribsClientError(
                                 f"Can't convert {existing_unit} to {new_unit} for {path}"
                             )
 
                         if not isclose(factor, 1):
-                            logger.info(f"Changing {existing_unit} to {new_unit} for {path} ...")
+                            logger.info(
+                                f"Changing {existing_unit} to {new_unit} for {path} ..."
+                            )
                             # TODO scale contributions to new unit
                             raise MPContribsClientError(
                                 "Changing units not supported yet. Please resubmit"
                                 " contributions or update accordingly."
                             )
 
                 new_columns.append(new_column)
 
         payload = {"columns": new_columns}
         valid, error = self._is_valid_payload("Project", payload)
         if not valid:
             raise MPContribsClientError(error)
 
-        return self.projects.updateProjectByName(pk=self.project, project=payload).result()
+        return self.projects.updateProjectByName(
+            pk=self.project, project=payload
+        ).result()
 
     def delete_contributions(self, query: dict = None, timeout: int = -1):
         """Remove all contributions for a query
 
         Args:
             query (dict): optional query to select contributions
             timeout (int): cancel remaining requests if timeout exceeded (in seconds)
@@ -1478,15 +1570,17 @@
 
         if self.project:
             query["project"] = self.project
 
         cids = list(self.get_all_ids(query).get(query["project"], {}).get("ids", set()))
 
         if not cids:
-            logger.info(f"There aren't any contributions to delete for {query['project']}")
+            logger.info(
+                f"There aren't any contributions to delete for {query['project']}"
+            )
             return
 
         total = len(cids)
         query = {"id__in": cids}
         _, total_pages = self.get_totals(query=query)
         queries = self._split_query(query, op="delete", pages=total_pages)
         futures = [self._get_future(i, q, op="delete") for i, q in enumerate(queries)]
@@ -1505,15 +1599,15 @@
             )
 
     def get_totals(
         self,
         query: dict = None,
         timeout: int = -1,
         resource: str = "contributions",
-        op: str = "query"
+        op: str = "query",
     ) -> tuple:
         """Retrieve total count and pages for resource entries matching query
 
         Args:
             query (dict): query to select resource entries
             timeout (int): cancel remaining requests if timeout exceeded (in seconds)
             resource (str): type of resource
@@ -1532,15 +1626,17 @@
             query["project"] = self.project
 
         skip_keys = {"per_page", "_fields", "format", "_sort"}
         query = {k: v for k, v in query.items() if k not in skip_keys}
         query["_fields"] = []  # only need totals -> explicitly request no fields
         queries = self._split_query(query, resource=resource, op=op)  # don't paginate
         result = {"total_count": 0, "total_pages": 0}
-        futures = [self._get_future(i, q, rel_url=resource) for i, q in enumerate(queries)]
+        futures = [
+            self._get_future(i, q, rel_url=resource) for i, q in enumerate(queries)
+        ]
         responses = _run_futures(futures, timeout=timeout, desc="Totals")
 
         for resp in responses.values():
             for k in result:
                 result[k] += resp.get("result", {}).get(k, 0)
 
         return result["total_count"], result["total_pages"]
@@ -1558,15 +1654,17 @@
             query (dict): query to select projects
 
         Returns:
             {"<project-name>": True|False, ...}
         """
         return {
             p["name"]: p["unique_identifiers"]
-            for p in self.query_projects(query=query, fields=["name", "unique_identifiers"])
+            for p in self.query_projects(
+                query=query, fields=["name", "unique_identifiers"]
+            )
         }
 
     def get_all_ids(
         self,
         query: dict = None,
         include: List[str] = None,
         timeout: int = -1,
@@ -1630,31 +1728,30 @@
             raise MPContribsClientError(f"`fmt` must be subset of {fmts}!")
 
         ops = {"query", "create", "update", "delete", "download"}
         if op not in ops:
             raise MPContribsClientError(f"`op` has to be one of {ops}")
 
         unique_identifiers = self.get_unique_identifiers_flags()
-        data_id_fields = {
-            k: v for k, v in data_id_fields.items()
-            if k in unique_identifiers and isinstance(v, str)
-        } if data_id_fields else {}
+        data_id_fields = data_id_fields or {}
+        for k, v in data_id_fields.items():
+            if k in unique_identifiers and isinstance(v, str):
+                data_id_fields[k] = v
 
         ret = {}
         query = query or {}
         if self.project and "project" not in query:
             query["project"] = self.project
 
         [query.pop(k, None) for k in ["page", "per_page", "_fields"]]
         id_fields = {"project", "id", "identifier"}
 
         if data_id_fields:
             id_fields.update(
-                f"data.{data_id_field}"
-                for data_id_field in data_id_fields.values()
+                f"data.{data_id_field}" for data_id_field in data_id_fields.values()
             )
 
         query["_fields"] = list(id_fields | components)
         _, total_pages = self.get_totals(query=query, timeout=timeout)
         queries = self._split_query(query, op=op, pages=total_pages)
         futures = [self._get_future(i, q) for i, q in enumerate(queries)]
         responses = _run_futures(futures, timeout=timeout, desc="Identifiers")
@@ -1711,28 +1808,30 @@
                     elif data_id_field and data_id_field_val:
                         ret[project][identifier] = {
                             data_id_field_val: {"id": contrib["id"]}
                         }
 
                         for component in components:
                             if component in contrib:
-                                ret[project][identifier][data_id_field_val][component] = {
+                                ret[project][identifier][data_id_field_val][
+                                    component
+                                ] = {
                                     d["name"]: {"id": d["id"], "md5": d["md5"]}
                                     for d in contrib[component]
                                 }
 
         return ret
 
     def query_contributions(
         self,
         query: dict = None,
         fields: list = None,
         sort: str = None,
         paginate: bool = False,
-        timeout: int = -1
+        timeout: int = -1,
     ) -> List[dict]:
         """Query contributions
 
         See `client.available_query_params()` for keyword arguments used in query.
 
         Args:
             query (dict): optional query to select contributions
@@ -1776,18 +1875,15 @@
             ret = self.contributions.queryContributions(
                 _fields=fields, _sort=sort, **query
             ).result()
 
         return ret
 
     def update_contributions(
-        self,
-        data: dict,
-        query: dict = None,
-        timeout: int = -1
+        self, data: dict, query: dict = None, timeout: int = -1
     ) -> dict:
         """Apply the same update to all contributions in a project (matching query)
 
         See `client.available_query_params()` for keyword arguments used in query.
 
         Args:
             data (dict): update to apply on every matching contribution
@@ -1823,60 +1919,58 @@
         cids = list(self.get_all_ids(query).get(self.project, {}).get("ids", set()))
 
         if not cids:
             logger.info(f"There aren't any contributions to update for {self.project}")
             return
 
         # get current list of data columns to decide if swagger reload is needed
-        resp = self.projects.getProjectByName(pk=self.project, _fields=["columns"]).result()
+        resp = self.projects.getProjectByName(
+            pk=self.project, _fields=["columns"]
+        ).result()
         old_paths = set(c["path"] for c in resp["columns"])
 
         total = len(cids)
         cids_query = {"id__in": cids}
         _, total_pages = self.get_totals(query=cids_query)
         queries = self._split_query(cids_query, op="update", pages=total_pages)
         futures = [
             self._get_future(i, q, op="update", data=data)
             for i, q in enumerate(queries)
         ]
         responses = _run_futures(futures, total=total, timeout=timeout)
         updated = sum(resp["count"] for _, resp in responses.items())
 
         if updated:
-            resp = self.projects.getProjectByName(pk=self.project, _fields=["columns"]).result()
+            resp = self.projects.getProjectByName(
+                pk=self.project, _fields=["columns"]
+            ).result()
             new_paths = set(c["path"] for c in resp["columns"])
 
             if new_paths != old_paths:
                 self.init_columns()
                 self._reinit()
 
         toc = time.perf_counter()
         return {"updated": updated, "total": total, "seconds_elapsed": toc - tic}
 
     def make_public(
-        self,
-        query: dict = None,
-        recursive: bool = False,
-        timeout: int = -1
+        self, query: dict = None, recursive: bool = False, timeout: int = -1
     ) -> dict:
         """Publish a project and optionally its contributions
 
         Args:
             query (dict): optional query to select contributions
             recursive (bool): also publish according contributions?
         """
         return self._set_is_public(
             True, query=query, recursive=recursive, timeout=timeout
         )
 
     def make_private(
-        self,
-        query: dict = None,
-        recursive: bool = False,
-        timeout: int = -1
+        self, query: dict = None, recursive: bool = False, timeout: int = -1
     ) -> dict:
         """Make a project and optionally its contributions private
 
         Args:
             query (dict): optional query to select contributions
             recursive (bool): also make according contributions private?
         """
@@ -1885,15 +1979,15 @@
         )
 
     def _set_is_public(
         self,
         is_public: bool,
         query: dict = None,
         recursive: bool = False,
-        timeout: int = -1
+        timeout: int = -1,
     ) -> dict:
         """Set the `is_public` flag for a project and optionally its contributions
 
         Args:
             is_public (bool): target value for `is_public` flag
             query (dict): optional query to select contributions
             recursive (bool): also set `is_public` for according contributions?
@@ -1910,24 +2004,30 @@
             query["project"] = self.project
 
         try:
             resp = self.projects.getProjectByName(
                 pk=query["project"], _fields=["is_public", "is_approved"]
             ).result()
         except HTTPNotFound:
-            raise MPContribsClientError(f"project `{query['project']}` not found or access denied!")
+            raise MPContribsClientError(
+                f"project `{query['project']}` not found or access denied!"
+            )
 
         if not recursive and resp["is_public"] == is_public:
-            return {"warning": f"`is_public` already set to {is_public} for `{query['project']}`."}
+            return {
+                "warning": f"`is_public` already set to {is_public} for `{query['project']}`."
+            }
 
         ret = {}
 
         if resp["is_public"] != is_public:
             if is_public and not resp["is_approved"]:
-                raise MPContribsClientError(f"project `{query['project']}` is not approved yet!")
+                raise MPContribsClientError(
+                    f"project `{query['project']}` is not approved yet!"
+                )
 
             resp = self.projects.updateProjectByName(
                 pk=query["project"], project={"is_public": is_public}
             ).result()
             ret["published"] = resp["count"] == 1
 
         if recursive:
@@ -1940,15 +2040,15 @@
         return ret
 
     def submit_contributions(
         self,
         contributions: List[dict],
         ignore_dupes: bool = False,
         timeout: int = -1,
-        skip_dupe_check: bool = False
+        skip_dupe_check: bool = False,
     ):
         """Submit a list of contributions
 
         Example for a single contribution dictionary:
 
         {
             "project": "sandbox",
@@ -1970,30 +2070,36 @@
         Args:
             contributions (list): list of contribution dicts to submit
             ignore_dupes (bool): force duplicate components to be submitted
             timeout (int): cancel remaining requests if timeout exceeded (in seconds)
             skip_dupe_check (bool): skip duplicate check for contribution identifiers
         """
         if not contributions or not isinstance(contributions, list):
-            raise MPContribsClientError("Please provide list of contributions to submit.")
+            raise MPContribsClientError(
+                "Please provide list of contributions to submit."
+            )
 
         # get existing contributions
         tic = time.perf_counter()
         project_names = set()
         collect_ids = []
         require_one_of = {"data"} | set(COMPONENTS)
 
         for idx, c in enumerate(contributions):
             has_keys = require_one_of & c.keys()
             if not has_keys:
-                raise MPContribsClientError(f"Nothing to submit for contribution #{idx}!")
+                raise MPContribsClientError(
+                    f"Nothing to submit for contribution #{idx}!"
+                )
             elif not all(c[k] for k in has_keys):
                 for k in has_keys:
                     if not c[k]:
-                        raise MPContribsClientError(f"Empty `{k}` for contribution #{idx}!")
+                        raise MPContribsClientError(
+                            f"Empty `{k}` for contribution #{idx}!"
+                        )
             elif "id" in c:
                 collect_ids.append(c["id"])
             elif "project" in c and "identifier" in c:
                 project_names.add(c["project"])
             elif self.project and "project" not in c and "identifier" in c:
                 project_names.add(self.project)
                 contributions[idx]["project"] = self.project
@@ -2013,20 +2119,26 @@
 
         existing = defaultdict(dict)
         unique_identifiers = defaultdict(dict)
         project_names = list(project_names)
 
         if not skip_dupe_check and len(collect_ids) != len(contributions):
             nproj = len(project_names)
-            query = {"name__in": project_names} if nproj > 1 else {"name": project_names[0]}
+            query = (
+                {"name__in": project_names} if nproj > 1 else {"name": project_names[0]}
+            )
             unique_identifiers = self.get_unique_identifiers_flags(query)
-            query = {"project__in": project_names} if nproj > 1 else {"project": project_names[0]}
-            existing = defaultdict(dict, self.get_all_ids(
-                query, include=COMPONENTS, timeout=timeout
-            ))
+            query = (
+                {"project__in": project_names}
+                if nproj > 1
+                else {"project": project_names[0]}
+            )
+            existing = defaultdict(
+                dict, self.get_all_ids(query, include=COMPONENTS, timeout=timeout)
+            )
 
         # prepare contributions
         contribs = defaultdict(list)
         digests = {project_name: defaultdict(set) for project_name in project_names}
         fields = [
             comp
             for comp in self.get_model("ContributionsSchema")._properties.keys()
@@ -2040,30 +2152,43 @@
                 serializable, error = self._is_serializable_dict(contrib["data"])
                 if not serializable:
                     raise MPContribsClientError(error)
 
             update = "id" in contrib
             project_name = id2project[contrib["id"]] if update else contrib["project"]
             if (
-                not update and unique_identifiers.get(project_name)
-                and contrib["identifier"] in existing.get(project_name, {}).get("identifiers", {})
+                not update
+                and unique_identifiers.get(project_name)
+                and contrib["identifier"]
+                in existing.get(project_name, {}).get("identifiers", {})
             ):
                 continue
 
-            contribs[project_name].append({
-                k: deepcopy(contrib[k])
-                for k in fields if k in contrib
-            })
+            contrib_copy = {}
+            for k in fields:
+                if k in contrib:
+                    flat = {}
+                    for kk, vv in flatten(contrib[k], reducer="dot").items():
+                        if isinstance(vv, bool):
+                            flat[kk] = "Yes" if vv else "No"
+                        elif isinstance(vv, str):
+                            flat[kk] = vv
+
+                    contrib_copy[k] = deepcopy(unflatten(flat, splitter="dot"))
+
+            contribs[project_name].append(contrib_copy)
 
             for component in COMPONENTS:
                 elements = contrib.get(component, [])
                 nelems = len(elements)
 
                 if nelems > MAX_ELEMS:
-                    raise MPContribsClientError(f"Too many {component} ({nelems} > {MAX_ELEMS})!")
+                    raise MPContribsClientError(
+                        f"Too many {component} ({nelems} > {MAX_ELEMS})!"
+                    )
 
                 if update and not nelems:
                     continue  # nothing to update for this component
 
                 contribs[project_name][-1][component] = []
 
                 for idx, element in enumerate(elements):
@@ -2071,15 +2196,17 @@
                         contribs[project_name][-1][component].append(None)
                         continue
 
                     is_structure = isinstance(element, PmgStructure)
                     is_table = isinstance(element, (pd.DataFrame, Table))
                     is_attachment = isinstance(element, (str, Path, Attachment))
                     if component == "structures" and not is_structure:
-                        raise MPContribsClientError(f"Use pymatgen Structure for {component}!")
+                        raise MPContribsClientError(
+                            f"Use pymatgen Structure for {component}!"
+                        )
                     elif component == "tables" and not is_table:
                         raise MPContribsClientError(
                             f"Use pandas DataFrame or mpontribs.client.Table for {component}!"
                         )
                     elif component == "attachments" and not is_attachment:
                         raise MPContribsClientError(
                             f"Use str, pathlib.Path or mpcontribs.client.Attachment for {component}"
@@ -2091,15 +2218,17 @@
                         del dct["@class"]
 
                         if not dct.get("charge"):
                             del dct["charge"]
 
                         if "properties" in dct:
                             if dct["properties"]:
-                                logger.warning("storing structure properties not supported, yet!")
+                                logger.warning(
+                                    "storing structure properties not supported, yet!"
+                                )
                             del dct["properties"]
                     elif is_table:
                         table = element
                         if not isinstance(table, Table):
                             table = Table(element)
                             table.attrs = element.attrs
 
@@ -2117,50 +2246,57 @@
                         dct["name"] = getattr(element, "name", "structure")
                     elif is_table:
                         dct["name"], dct["attrs"] = table._attrs_as_dict()
                     elif is_attachment:
                         dct["name"] = element.name
 
                     dupe = bool(
-                        digest in digests[project_name][component] or
-                        digest in existing.get(project_name, {}).get(component, {}).get("md5s", [])
+                        digest in digests[project_name][component]
+                        or digest
+                        in existing.get(project_name, {})
+                        .get(component, {})
+                        .get("md5s", [])
                     )
 
                     if not ignore_dupes and dupe:
                         # TODO add matching duplicate info to msg
                         msg = f"Duplicate in {project_name}: {contrib['identifier']} {dct['name']}"
                         raise MPContribsClientError(msg)
 
                     digests[project_name][component].add(digest)
                     contribs[project_name][-1][component].append(dct)
 
-                valid, error = self._is_valid_payload("Contribution", contribs[project_name][-1])
+                valid, error = self._is_valid_payload(
+                    "Contribution", contribs[project_name][-1]
+                )
                 if not valid:
-                    raise MPContribsClientError(f"{contrib['identifier']} invalid: {error}!")
+                    raise MPContribsClientError(
+                        f"{contrib['identifier']} invalid: {error}!"
+                    )
 
         # submit contributions
         if contribs:
             total, total_processed = 0, 0
             nmax = 1000  # TODO this should be set dynamically from `bulk_update_limit`
 
             def post_future(track_id, payload):
                 future = self.session.post(
                     f"{self.url}/contributions/",
                     headers=self.headers,
-                    hooks={'response': _response_hook},
+                    hooks={"response": _response_hook},
                     data=payload,
                 )
                 setattr(future, "track_id", track_id)
                 return future
 
             def put_future(pk, payload):
                 future = self.session.put(
                     f"{self.url}/contributions/{pk}/",
                     headers=self.headers,
-                    hooks={'response': _response_hook},
+                    hooks={"response": _response_hook},
                     data=payload,
                 )
                 setattr(future, "track_id", pk)
                 return future
 
             for project_name in project_names:
                 ncontribs = len(contribs[project_name])
@@ -2170,89 +2306,117 @@
                 while contribs[project_name]:
                     futures, post_chunk, idx = [], [], 0
 
                     for n, c in enumerate(contribs[project_name]):
                         if "id" in c:
                             pk = c.pop("id")
                             if not c:
-                                logger.error(f"SKIPPED: update of {project_name}/{pk} empty.")
+                                logger.error(
+                                    f"SKIPPED: update of {project_name}/{pk} empty."
+                                )
 
                             payload = ujson.dumps(c).encode("utf-8")
                             if len(payload) < MAX_PAYLOAD:
                                 futures.append(put_future(pk, payload))
                             else:
-                                logger.error(f"SKIPPED: update of {project_name}/{pk} too large.")
+                                logger.error(
+                                    f"SKIPPED: update of {project_name}/{pk} too large."
+                                )
                         else:
                             next_post_chunk = post_chunk + [c]
                             next_payload = ujson.dumps(next_post_chunk).encode("utf-8")
-                            if len(next_post_chunk) > nmax or len(next_payload) >= MAX_PAYLOAD:
+                            if (
+                                len(next_post_chunk) > nmax
+                                or len(next_payload) >= MAX_PAYLOAD
+                            ):
                                 if post_chunk:
                                     payload = ujson.dumps(post_chunk).encode("utf-8")
                                     futures.append(post_future(idx, payload))
                                     post_chunk = []
                                     idx += 1
                                 else:
-                                    logger.error(f"SKIPPED: contrib {project_name}/{n} too large.")
+                                    logger.error(
+                                        f"SKIPPED: contrib {project_name}/{n} too large."
+                                    )
                                     continue
 
                             post_chunk.append(c)
 
                     if post_chunk and len(futures) < ncontribs:
                         payload = ujson.dumps(post_chunk).encode("utf-8")
                         futures.append(post_future(idx, payload))
 
                     if not futures:
                         break  # nothing to do
 
                     responses = _run_futures(
-                        futures, total=ncontribs-total_processed, timeout=timeout, desc="Submit"
+                        futures,
+                        total=ncontribs - total_processed,
+                        timeout=timeout,
+                        desc="Submit",
                     )
                     processed = sum(r.get("count", 0) for r in responses.values())
                     total_processed += processed
 
-                    if total_processed != ncontribs and retries < RETRIES and \
-                            unique_identifiers.get(project_name):
-                        logger.info(f"{total_processed}/{ncontribs} processed -> retrying ...")
+                    if (
+                        total_processed != ncontribs
+                        and retries < RETRIES
+                        and unique_identifiers.get(project_name)
+                    ):
+                        logger.info(
+                            f"{total_processed}/{ncontribs} processed -> retrying ..."
+                        )
                         existing[project_name] = self.get_all_ids(
-                            dict(project=project_name), include=COMPONENTS, timeout=timeout
+                            dict(project=project_name),
+                            include=COMPONENTS,
+                            timeout=timeout,
                         ).get(project_name, {"identifiers": set()})
-                        unique_identifiers[project_name] = self.projects.getProjectByName(
-                            pk=project_name, _fields=["unique_identifiers"]
-                        ).result()["unique_identifiers"]
-                        existing_ids = existing.get(project_name, {}).get("identifiers", [])
+                        unique_identifiers[project_name] = (
+                            self.projects.getProjectByName(
+                                pk=project_name, _fields=["unique_identifiers"]
+                            ).result()["unique_identifiers"]
+                        )
+                        existing_ids = existing.get(project_name, {}).get(
+                            "identifiers", []
+                        )
                         contribs[project_name] = [
-                            c for c in contribs[project_name]
+                            c
+                            for c in contribs[project_name]
                             if c["identifier"] not in existing_ids
                         ]
                         retries += 1
                     else:
                         contribs[project_name] = []  # abort retrying
                         if total_processed != ncontribs:
                             if retries >= RETRIES:
-                                logger.error(f"{project_name}: Tried {RETRIES} times - abort.")
+                                logger.error(
+                                    f"{project_name}: Tried {RETRIES} times - abort."
+                                )
                             elif not unique_identifiers.get(project_name):
                                 logger.info(
                                     f"{project_name}: resubmit failed contributions manually"
                                 )
 
             toc = time.perf_counter()
             dt = (toc - tic) / 60
             self.init_columns()
             self._reinit()
-            logger.info(f"It took {dt:.1f}min to submit {total_processed}/{total} contributions.")
+            logger.info(
+                f"It took {dt:.1f}min to submit {total_processed}/{total} contributions."
+            )
         else:
             logger.info("Nothing to submit.")
 
     def download_contributions(
         self,
         query: dict = None,
         outdir: Union[str, Path] = DEFAULT_DOWNLOAD_DIR,
         overwrite: bool = False,
         include: List[str] = None,
-        timeout: int = -1
+        timeout: int = -1,
     ) -> int:
         """Download a list of contributions as .json.gz file(s)
 
         Args:
             query: query to select contributions
             outdir: optional output directory
             overwrite: force re-download
@@ -2292,16 +2456,20 @@
                     start = time.perf_counter()
 
                 ids = list(values[component]["ids"])
                 if not ids:
                     continue
 
                 paths = self._download_resource(
-                    resource=component, ids=ids, fmt=fmt,
-                    outdir=outdir, overwrite=overwrite, timeout=timeout
+                    resource=component,
+                    ids=ids,
+                    fmt=fmt,
+                    outdir=outdir,
+                    overwrite=overwrite,
+                    timeout=timeout,
                 )
                 logger.debug(
                     f"Downloaded {len(ids)} {component} for '{name}' in {len(paths)} file(s)."
                 )
 
                 cls = classes_map[component]
                 for path in paths:
@@ -2310,16 +2478,20 @@
                             components_loaded[component][c["id"]] = cls.from_dict(c)
 
             cids = list(values["ids"])
             if not cids:
                 continue
 
             paths = self._download_resource(
-                resource="contributions", ids=cids, fmt=fmt,
-                outdir=outdir, overwrite=overwrite, timeout=timeout
+                resource="contributions",
+                ids=cids,
+                fmt=fmt,
+                outdir=outdir,
+                overwrite=overwrite,
+                timeout=timeout,
             )
             logger.debug(
                 f"Downloaded {len(cids)} contributions for '{name}' in {len(paths)} file(s)."
             )
 
             for path in paths:
                 with gzip.open(path, "r") as f:
@@ -2337,91 +2509,103 @@
 
     def download_structures(
         self,
         ids: List[str],
         outdir: Union[str, Path] = DEFAULT_DOWNLOAD_DIR,
         overwrite: bool = False,
         timeout: int = -1,
-        fmt: str = "json"
+        fmt: str = "json",
     ) -> Path:
         """Download a list of structures as a .json.gz file
 
         Args:
             ids: list of structure ObjectIds
             outdir: optional output directory
             overwrite: force re-download
             timeout: cancel remaining requests if timeout exceeded (in seconds)
             fmt: download format - "json" or "csv"
 
         Returns:
             paths of output files
         """
         return self._download_resource(
-            resource="structures", ids=ids, fmt=fmt,
-            outdir=outdir, overwrite=overwrite, timeout=timeout
+            resource="structures",
+            ids=ids,
+            fmt=fmt,
+            outdir=outdir,
+            overwrite=overwrite,
+            timeout=timeout,
         )
 
     def download_tables(
         self,
         ids: List[str],
         outdir: Union[str, Path] = DEFAULT_DOWNLOAD_DIR,
         overwrite: bool = False,
         timeout: int = -1,
-        fmt: str = "json"
+        fmt: str = "json",
     ) -> Path:
         """Download a list of tables as a .json.gz file
 
         Args:
             ids: list of table ObjectIds
             outdir: optional output directory
             overwrite: force re-download
             timeout: cancel remaining requests if timeout exceeded (in seconds)
             fmt: download format - "json" or "csv"
 
         Returns:
             paths of output files
         """
         return self._download_resource(
-            resource="tables", ids=ids, fmt=fmt,
-            outdir=outdir, overwrite=overwrite, timeout=timeout
+            resource="tables",
+            ids=ids,
+            fmt=fmt,
+            outdir=outdir,
+            overwrite=overwrite,
+            timeout=timeout,
         )
 
     def download_attachments(
         self,
         ids: List[str],
         outdir: Union[str, Path] = DEFAULT_DOWNLOAD_DIR,
         overwrite: bool = False,
         timeout: int = -1,
-        fmt: str = "json"
+        fmt: str = "json",
     ) -> Path:
         """Download a list of attachments as a .json.gz file
 
         Args:
             ids: list of attachment ObjectIds
             outdir: optional output directory
             overwrite: force re-download
             timeout: cancel remaining requests if timeout exceeded (in seconds)
             fmt: download format - "json" or "csv"
 
         Returns:
             paths of output files
         """
         return self._download_resource(
-            resource="attachments", ids=ids, fmt=fmt,
-            outdir=outdir, overwrite=overwrite, timeout=timeout
+            resource="attachments",
+            ids=ids,
+            fmt=fmt,
+            outdir=outdir,
+            overwrite=overwrite,
+            timeout=timeout,
         )
 
     def _download_resource(
         self,
         resource: str,
         ids: List[str],
         outdir: Union[str, Path] = DEFAULT_DOWNLOAD_DIR,
         overwrite: bool = False,
         timeout: int = -1,
-        fmt: str = "json"
+        fmt: str = "json",
     ) -> Path:
         """Helper to download a list of resources as .json.gz file
 
         Args:
             resource: type of resource
             ids: list of resource ObjectIds
             outdir: optional output directory
@@ -2446,26 +2630,28 @@
         subdir.mkdir(parents=True, exist_ok=True)
         model = self.get_model(f"{resource.capitalize()}Schema")
         fields = list(model._properties.keys())
         query = {"format": fmt, "_fields": fields, "id__in": oids}
         _, total_pages = self.get_totals(
             query=query, resource=resource, op="download", timeout=timeout
         )
-        queries = self._split_query(query, resource=resource, op="download", pages=total_pages)
+        queries = self._split_query(
+            query, resource=resource, op="download", pages=total_pages
+        )
         paths, futures = [], []
 
         for query in queries:
             digest = get_md5({"ids": query["id__in"].split(",")})
             path = subdir / f"{digest}.{fmt}.gz"
             paths.append(path)
 
             if not path.exists() or overwrite:
-                futures.append(self._get_future(
-                    path, query, rel_url=f"{resource}/download/gz"
-                ))
+                futures.append(
+                    self._get_future(path, query, rel_url=f"{resource}/download/gz")
+                )
 
         if futures:
             responses = _run_futures(futures, timeout=timeout)
 
             for path, resp in responses.items():
                 path.write_bytes(resp["result"])
```

### Comparing `mpcontribs-client-5.7.0/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.8.1/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.7.0
+Version: 5.8.1
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.7.0/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.8.1/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.7.0/requirements/deployment.txt` & `mpcontribs-client-5.8.1/requirements/deployment.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,61 +8,61 @@
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 bravado==11.0.3
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
 exceptiongroup==1.2.0
     # via ipython
 executing==2.0.1
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-ipython==8.20.0
+ipython==8.23.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
@@ -70,63 +70,63 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via
     #   -r python/requirements.txt
     #   pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2024.1.26
+monty==2024.3.31
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   -r python/requirements.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==1.5.3
+pandas==2.2.1
     # via
     #   -r python/requirements.txt
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -134,38 +134,38 @@
     # via stack-data
 pybtex==0.24.0
     # via pymatgen
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymatgen==2024.1.27
+pymatgen==2024.3.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymongo==4.6.1
+pymongo==4.6.3
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
-pytz==2023.4
+pytz==2024.1
     # via
     #   bravado-core
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
@@ -173,23 +173,23 @@
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   -r python/requirements.txt
     #   pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 simplejson==3.19.2
     # via
@@ -197,51 +197,53 @@
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
+spglib==2.3.1
     # via pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
+    #   ipython
     #   swagger-spec-validator
+tzdata==2024.1
+    # via pandas
 ujson==5.9.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
 #
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-boltons==23.1.1
+backcall==0.2.0
+    # via ipython
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
-exceptiongroup==1.2.0
-    # via ipython
+emmet-core==0.68.0
+    # via mp-api
 executing==2.0.1
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-ipython==8.21.0
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+ipython==8.12.3
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
 joblib==1.3.2
     # via pymatgen
@@ -70,81 +77,100 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.8.2
+matplotlib==3.7.5
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2024.1.26
+monty==2023.9.25
+    # via
+    #   emmet-core
+    #   mp-api
+    #   pymatgen
+mp-api==0.35.1
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
-networkx==3.2.1
+    #   mp-api
+networkx==3.1
     # via pymatgen
-numpy==1.26.3
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.18.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
-    # via pymatgen
+    # via
+    #   emmet-core
+    #   pymatgen
+pydantic==1.10.15
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2024.1.27
-    # via mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymatgen==2023.8.10
+    # via
+    #   emmet-core
+    #   mp-api
+    #   mpcontribs-client (setup.py)
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -153,91 +179,102 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
+    #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.12.0
+scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.2
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
-    # via pymatgen
+spglib==2.3.1
+    # via
+    #   emmet-core
+    #   pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
+    #   emmet-core
+    #   ipython
+    #   mp-api
+    #   pydantic
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.18.1
+    # via importlib-resources
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,37 +8,35 @@
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage[toml]==7.4.1
-    # via
-    #   coverage
-    #   pytest-cov
+coverage[toml]==7.4.4
+    # via pytest-cov
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
 exceptiongroup==1.2.0
     # via
     #   ipython
     #   pytest
@@ -48,27 +46,27 @@
     # via mpcontribs-client (setup.py)
 flake8==7.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
     # via pytest
-ipython==8.21.0
+ipython==8.23.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
 joblib==1.3.2
     # via pymatgen
@@ -82,62 +80,62 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2024.1.26
+monty==2024.3.31
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
 networkx==3.2.1
     # via pymatgen
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.0
+pandas==2.2.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.4.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
@@ -157,33 +155,33 @@
     #   pytest-pycodestyle
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2024.1.27
+pymatgen==2024.3.1
     # via mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-pytest==8.0.0
+pytest==8.1.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -192,15 +190,15 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
@@ -208,41 +206,40 @@
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.2
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
+spglib==2.3.1
     # via pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (setup.py)
@@ -252,35 +249,36 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
+    #   ipython
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,64 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-backcall==0.2.0
-    # via ipython
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.68.0
-    # via mp-api
+exceptiongroup==1.2.0
+    # via ipython
 executing==2.0.1
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
-ipython==8.12.3
+importlib-resources==6.4.0
+    # via matplotlib
+ipython==8.18.1
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
 joblib==1.3.2
     # via pymatgen
@@ -77,100 +72,81 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.7.4
+matplotlib==3.8.4
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2023.9.25
-    # via
-    #   emmet-core
-    #   mp-api
-    #   pymatgen
-mp-api==0.35.1
+monty==2024.3.31
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
-    #   mp-api
-networkx==3.1
+networkx==3.2.1
     # via pymatgen
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.3
+pandas==2.2.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
-    # via
-    #   emmet-core
-    #   pymatgen
-pydantic==1.10.14
-    # via
-    #   emmet-core
-    #   pymatgen
+    # via pymatgen
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.8.10
-    # via
-    #   emmet-core
-    #   mp-api
-    #   mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymatgen==2024.3.1
+    # via mpcontribs-client (setup.py)
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -179,103 +155,93 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
-    #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.13.0
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.2
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
-    # via
-    #   emmet-core
-    #   pymatgen
+spglib==2.3.1
+    # via pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
-    #   emmet-core
     #   ipython
-    #   mp-api
-    #   pydantic
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-resources
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,37 +10,35 @@
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
 backcall==0.2.0
     # via ipython
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 contourpy==1.1.1
     # via matplotlib
-coverage[toml]==7.4.1
-    # via
-    #   coverage
-    #   pytest-cov
+coverage[toml]==7.4.4
+    # via pytest-cov
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
 emmet-core==0.68.0
     # via mp-api
 exceptiongroup==1.2.0
     # via pytest
@@ -50,25 +48,25 @@
     # via mpcontribs-client (setup.py)
 flake8==7.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.12.3
@@ -89,17 +87,17 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.7.4
+matplotlib==3.7.5
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
@@ -108,53 +106,53 @@
     #   emmet-core
     #   mp-api
     #   pymatgen
 mp-api==0.35.1
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
 numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.4.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
@@ -170,46 +168,46 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.11.1
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.14
+pydantic==1.10.15
     # via
     #   emmet-core
     #   pymatgen
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
 pymatgen==2023.8.10
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-pytest==8.0.0
+pytest==8.1.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -218,15 +216,15 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
@@ -235,19 +233,19 @@
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -257,19 +255,18 @@
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
+spglib==2.3.1
     # via
     #   emmet-core
     #   pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
@@ -281,44 +278,44 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.10.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
 exceptiongroup==1.2.0
     # via ipython
 executing==2.0.1
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-importlib-resources==6.1.1
-    # via matplotlib
-ipython==8.18.1
+ipython==8.23.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
 joblib==1.3.2
     # via pymatgen
@@ -72,59 +70,59 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
-monty==2024.1.26
+monty==2024.3.31
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
 networkx==3.2.1
     # via pymatgen
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.0
+pandas==2.2.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
@@ -132,21 +130,21 @@
     # via stack-data
 pybtex==0.24.0
     # via pymatgen
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2024.1.27
+pymatgen==2024.3.1
     # via mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -155,15 +153,15 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
@@ -171,78 +169,75 @@
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.2
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
+spglib==2.3.1
     # via pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.3
     # via plotly
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
     #   ipython
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.17.0
-    # via importlib-resources
```

### Comparing `mpcontribs-client-5.7.0/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.8.1/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,37 +8,35 @@
     # via isoduration
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-boltons==23.1.1
+boltons==24.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
 bravado-core==6.1.1
     # via bravado
-cachetools==5.3.2
+cachetools==5.3.3
     # via mpcontribs-client (setup.py)
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage[toml]==7.4.1
-    # via
-    #   coverage
-    #   pytest-cov
+coverage[toml]==7.4.4
+    # via pytest-cov
 cycler==0.12.1
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.5.0
+dnspython==2.6.1
     # via
     #   pyisemail
     #   pymongo
 exceptiongroup==1.2.0
     # via
     #   ipython
     #   pytest
@@ -48,25 +46,25 @@
     # via mpcontribs-client (setup.py)
 flake8==7.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.47.2
+fonttools==4.51.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via uncertainties
 idna==3.6
     # via
     #   jsonschema
     #   requests
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.18.1
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
@@ -84,62 +82,62 @@
     # via
     #   bravado-core
     #   swagger-spec-validator
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
-matplotlib==3.8.2
+matplotlib==3.8.4
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
-monty==2024.1.26
+monty==2024.3.31
     # via pymatgen
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
 networkx==3.2.1
     # via pymatgen
-numpy==1.26.3
+numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.2.0
+pandas==2.2.1
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.18.0
+plotly==5.20.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.4.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
@@ -159,33 +157,33 @@
     #   pytest-pycodestyle
 pyflakes==3.2.0
     # via flake8
 pygments==2.17.2
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2024.1.27
+pymatgen==2024.3.1
     # via mpcontribs-client (setup.py)
-pymongo==4.6.1
+pymongo==4.6.3
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-pytest==8.0.0
+pytest==8.1.1
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2024.1
@@ -194,15 +192,15 @@
     #   pandas
 pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-referencing==0.33.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
@@ -210,41 +208,40 @@
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3986-validator==0.1.1
     # via jsonschema
-rpds-py==0.17.1
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-ruamel-yaml==0.18.5
+ruamel-yaml==0.18.6
     # via pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-scipy==1.12.0
+scipy==1.13.0
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.2
     # via
     #   bravado
     #   bravado-core
 six==1.16.0
     # via
     #   asttokens
     #   bravado
     #   bravado-core
     #   flatten-dict
-    #   latexcodec
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
-spglib==2.3.0
+spglib==2.3.1
     # via pymatgen
 stack-data==0.6.3
     # via ipython
 swagger-spec-validator==3.0.3
     # via
     #   bravado-core
     #   mpcontribs-client (setup.py)
@@ -254,38 +251,38 @@
     # via pymatgen
 tenacity==8.2.3
     # via plotly
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.66.1
+tqdm==4.66.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-traitlets==5.14.1
+traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   bravado
     #   ipython
     #   swagger-spec-validator
-tzdata==2023.4
+tzdata==2024.1
     # via pandas
 ujson==5.9.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.7.0/setup.py` & `mpcontribs-client-5.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.7.0/tests/test_client.py` & `mpcontribs-client-5.8.1/tests/test_client.py`

 * *Files identical despite different names*

