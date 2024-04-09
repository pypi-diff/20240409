# Comparing `tmp/better_proxy-1.1.5.tar.gz` & `tmp/better_proxy-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_proxy-1.1.5.tar", max compression
+gzip compressed data, was "better_proxy-1.2.0b1.tar", max compression
```

## Comparing `better_proxy-1.1.5.tar` & `better_proxy-1.2.0b1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       60 2023-08-21 20:54:09.423000 better_proxy-1.1.5/better_proxy/__init__.py
--rw-r--r--   0        0        0     3199 2024-03-13 17:32:27.299863 better_proxy-1.1.5/better_proxy/proxy.py
--rw-r--r--   0        0        0      484 2024-03-13 17:34:38.000724 better_proxy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1888 2024-02-24 09:09:36.593943 better_proxy-1.1.5/README.md
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 better_proxy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-09 07:37:58.373466 better_proxy-1.2.0b1/better_proxy/__init__.py
+-rw-r--r--   0        0        0     3544 2024-04-09 07:36:49.254809 better_proxy-1.2.0b1/better_proxy/proxy.py
+-rw-r--r--   0        0        0      487 2024-04-09 07:38:59.657221 better_proxy-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1888 2024-02-24 09:09:36.593943 better_proxy-1.2.0b1/README.md
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 better_proxy-1.2.0b1/PKG-INFO
```

### Comparing `better_proxy-1.1.5/better_proxy/proxy.py` & `better_proxy-1.2.0b1/better_proxy/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,38 @@
 PROXY_FORMATS_REGEXP = [
     re.compile(r'^(?:(?P<protocol>.+)://)?(?P<login>[^:]+):(?P<password>[^@|:]+)[@|:](?P<host>[^:]+):(?P<port>\d+)$'),
     re.compile(r'^(?:(?P<protocol>.+)://)?(?P<host>[^:]+):(?P<port>\d+)[@|:](?P<login>[^:]+):(?P<password>[^:]+)$'),
     re.compile(r'^(?:(?P<protocol>.+)://)?(?P<host>[^:]+):(?P<port>\d+)$'),
 ]
 
 
+class ParsedProxy(TypedDict):
+    host: str
+    port: int
+    protocol: Protocol | None
+    login:    str | None
+    password: str | None
+
+
+def parse_proxy_str(proxy: str) -> ParsedProxy:
+    for pattern in PROXY_FORMATS_REGEXP:
+        match = pattern.match(proxy)
+        if match:
+            groups = match.groupdict()
+            return {
+                "host": groups["host"],
+                "port": int(groups["port"]),
+                "protocol": groups.get("protocol"),
+                "login": groups.get("login"),
+                "password": groups.get("password"),
+            }
+
+    raise ValueError(f'Unsupported proxy format: {proxy}')
+
+
 def _load_lines(filepath: Path | str) -> list[str]:
     with open(filepath, "r") as file:
         return [line.strip() for line in file.readlines() if line != "\n"]
 
 
 class PlaywrightProxySettings(TypedDict, total=False):
     server:   str
@@ -27,33 +51,24 @@
 
 class Proxy(BaseModel):
     host: str
     port: int
     protocol: Protocol = "http"
     login:    str | None = None
     password: str | None = None
+    refresh_url: str | None = None
 
     @classmethod
     def from_str(cls, proxy: str or "Proxy") -> "Proxy":
         if type(proxy) is cls or issubclass(type(proxy), cls):
             return proxy
 
-        for pattern in PROXY_FORMATS_REGEXP:
-            match = pattern.match(proxy)
-            if match:
-                groups = match.groupdict()
-                return cls(
-                    host=groups["host"],
-                    port=int(groups["port"]),
-                    protocol=groups.get("protocol") or "http",
-                    login=groups.get("login"),
-                    password=groups.get("password"),
-                )
-
-        raise ValueError(f'Unsupported proxy format: {proxy}')
+        parsed_proxy = parse_proxy_str(proxy)
+        parsed_proxy["protocol"] = parsed_proxy["protocol"] or "http"
+        return cls(**parsed_proxy)
 
     @classmethod
     def from_file(cls, filepath: Path | str) -> list["Proxy"]:
         return [cls.from_str(proxy) for proxy in _load_lines(filepath)]
 
     @property
     def as_url(self) -> str:
```

### Comparing `better_proxy-1.1.5/README.md` & `better_proxy-1.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `better_proxy-1.1.5/PKG-INFO` & `better_proxy-1.2.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-proxy
-Version: 1.1.5
+Version: 1.2.0b1
 Summary: Better proxy!
 Home-page: https://github.com/alenkimov/better_proxy
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

