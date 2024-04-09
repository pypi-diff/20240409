# Comparing `tmp/sectxt-0.9.2.tar.gz` & `tmp/sectxt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectxt-0.9.2.tar", last modified: Thu Mar  7 10:00:25 2024, max compression
+gzip compressed data, was "sectxt-0.9.3.tar", last modified: Tue Apr  9 12:27:12 2024, max compression
```

## Comparing `sectxt-0.9.2.tar` & `sectxt-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 10:00:25.609032 sectxt-0.9.2/
--rw-rw-rw-   0        0        0    14114 2024-03-06 12:09:38.000000 sectxt-0.9.2/LICENCE
--rw-rw-rw-   0        0        0    12662 2024-03-07 10:00:25.608025 sectxt-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    11613 2024-03-07 09:54:23.000000 sectxt-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-07 10:00:25.601701 sectxt-0.9.2/sectxt/
--rw-rw-rw-   0        0        0    20176 2024-03-07 09:54:23.000000 sectxt-0.9.2/sectxt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-07 10:00:25.608025 sectxt-0.9.2/sectxt.egg-info/
--rw-rw-rw-   0        0        0    12662 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-03-07 10:00:25.000000 sectxt-0.9.2/sectxt.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1028 2024-03-07 10:00:25.609780 sectxt-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0       64 2024-03-06 12:09:38.000000 sectxt-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 10:00:25.606719 sectxt-0.9.2/test/
--rw-rw-rw-   0        0        0    13258 2024-03-07 09:54:23.000000 sectxt-0.9.2/test/test_sectxt.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:27:12.193256 sectxt-0.9.3/
+-rw-rw-rw-   0        0        0    14114 2024-03-06 12:09:38.000000 sectxt-0.9.3/LICENCE
+-rw-rw-rw-   0        0        0    12662 2024-04-09 12:27:12.193256 sectxt-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11613 2024-03-07 09:54:23.000000 sectxt-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 12:27:12.175256 sectxt-0.9.3/sectxt/
+-rw-rw-rw-   0        0        0    20249 2024-04-09 12:13:51.000000 sectxt-0.9.3/sectxt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:27:12.192263 sectxt-0.9.3/sectxt.egg-info/
+-rw-rw-rw-   0        0        0    12662 2024-04-09 12:27:12.000000 sectxt-0.9.3/sectxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-09 12:27:12.000000 sectxt-0.9.3/sectxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 12:27:12.000000 sectxt-0.9.3/sectxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-09 12:27:12.000000 sectxt-0.9.3/sectxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 12:27:12.000000 sectxt-0.9.3/sectxt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-03-07 10:00:25.000000 sectxt-0.9.3/sectxt.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1028 2024-04-09 12:27:12.194257 sectxt-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0       64 2024-03-06 12:09:38.000000 sectxt-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:27:12.191267 sectxt-0.9.3/test/
+-rw-rw-rw-   0        0        0    13958 2024-04-09 12:13:51.000000 sectxt-0.9.3/test/test_sectxt.py
```

### Comparing `sectxt-0.9.2/LICENCE` & `sectxt-0.9.3/LICENCE`

 * *Files identical despite different names*

### Comparing `sectxt-0.9.2/PKG-INFO` & `sectxt-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.9.2
+Version: 0.9.3
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sectxt-0.9.2/README.md` & `sectxt-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sectxt-0.9.2/sectxt/__init__.py` & `sectxt-0.9.3/sectxt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 import dateutil.parser
 import requests
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 s = requests.Session()
 
 
 class ErrorDict(TypedDict):
     code: str
     message: str
@@ -65,15 +65,15 @@
         "csaf",
     ]
 
     known_fields = uri_fields + [PREFERRED_LANGUAGES, "expires"]
 
     def __init__(
         self,
-        content: str,
+        content: bytes,
         urls: Optional[str] = None,
         recommend_unknown_fields: bool = True,
         is_local: bool = False
     ):
         self._urls = strlist_from_arg(urls)
         self._line_info: List[LineDict] = []
         self._errors: List[ErrorDict] = []
@@ -81,21 +81,23 @@
         self._notifications: List[ErrorDict] = []
         self._values: DefaultDict[str, List[str]] = defaultdict(list)
         self._langs: Optional[List[str]] = None
         self._signed = False
         self._reading_sig = False
         self._finished_sig = False
         self._content = content
+        self._content_str = None
         self.recommend_unknown_fields = recommend_unknown_fields
         self.is_local = is_local
         self._line_no: Optional[int] = None
         self._process()
 
     def _process(self) -> None:
-        lines = self._content.split("\n")
+        self._content_str = self._get_str(self._content)
+        lines = self._content_str.split("\n")
         self._line_no = 1
         for line in lines:
             self._line_info.append(self._parse_line(line))
             self._line_no += 1
         self._line_no = None
         self.validate_contents()
 
@@ -155,15 +157,15 @@
                     "Signed security.txt must start with the header "
                     "'-----BEGIN PGP SIGNED MESSAGE-----'.",
                 )
             self._signed = True
 
             # Check pgp formatting if signed
             try:
-                pgpy.PGPMessage.from_blob(self._content)
+                pgpy.PGPMessage.from_blob(self._content_str)
             except ValueError:
                 self._add_error(
                     "pgp_data_error",
                     "Signed message did not contain a correct ASCII-armored PGP block."
                 )
             except PGPError as e:
                 self._add_error(
@@ -359,14 +361,29 @@
             self._add_recommendation(
                 "no_canonical", "'Canonical' field should be present in a signed file."
             )
 
     def is_valid(self) -> bool:
         return not self._errors
 
+    def _get_str(self, content: bytes) -> str:
+        try:
+            if content.startswith(codecs.BOM_UTF8):
+                content = content.replace(codecs.BOM_UTF8, b'', 1)
+                self._add_error(
+                    "bom_in_file",
+                    "The Byte-Order Mark was found at the start of the file. "
+                    "Security.txt must be encoded using UTF-8 in Net-Unicode form, "
+                    "the BOM signature must not appear at the beginning."
+                )
+            return content.decode('utf-8')
+        except UnicodeError:
+            self._add_error("utf8", "Content must be utf-8 encoded.")
+        return content.decode('utf-8', errors="replace")
+
     @property
     def errors(self) -> List[ErrorDict]:
         return self._errors
 
     @property
     def recommendations(self) -> List[ErrorDict]:
         return self._recommendations
@@ -413,35 +430,20 @@
                 raise ValueError("Invalid URL")
             loc = url_parts.netloc
         else:
             loc = url
         self._loc = loc
         self._path: Optional[str] = None
         self._url: Optional[str] = None
-        super().__init__("", recommend_unknown_fields=recommend_unknown_fields, is_local=is_local)
-
-    def _get_str(self, content: bytes) -> str:
-        try:
-            if content.startswith(codecs.BOM_UTF8):
-                content = content.replace(codecs.BOM_UTF8, b'', 1)
-                self._add_error(
-                    "bom_in_file",
-                    "The Byte-Order Mark was found at the start of the file. "
-                    "Security.txt must be encoded using UTF-8 in Net-Unicode form, "
-                    "the BOM signature must not appear at the beginning."
-                )
-            return content.decode('utf-8')
-        except UnicodeError:
-            self._add_error("utf8", "Content must be utf-8 encoded.")
-        return content.decode('utf-8', errors="replace")
+        super().__init__(b'', recommend_unknown_fields=recommend_unknown_fields, is_local=is_local)
 
     def _process(self) -> None:
         if self.is_local:
             security_txt_file = open(self._loc, mode="rb")
-            self._content = self._get_str(security_txt_file.read())
+            self._content = security_txt_file.read()
             security_txt_file.close()
             super()._process()
         else:
             security_txt_found = False
             for scheme in ["https", "http"]:
                 for path in [".well-known/security.txt", "security.txt"]:
                     url = urlunsplit((scheme, self._loc, path, None, None))
@@ -505,15 +507,15 @@
                             if charset != "utf-8" and charset != "csutf8":
                                 # According to RFC9116, charset default is utf-8
                                 self._add_error(
                                     "invalid_charset",
                                     "Charset parameter in Content-Type header must be "
                                     "'utf-8' if present.",
                                 )
-                        self._content = self._get_str(resp.content)
+                        self._content = resp.content
                         if resp.history:
                             self._urls = [resp.history[0].url, resp.url]
                         else:
                             self._urls = [url]
                         super()._process()
                         security_txt_found = True
                         break
```

### Comparing `sectxt-0.9.2/sectxt.egg-info/PKG-INFO` & `sectxt-0.9.3/sectxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.9.2
+Version: 0.9.3
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sectxt-0.9.2/setup.cfg` & `sectxt-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sectxt-0.9.2/test/test_sectxt.py` & `sectxt-0.9.3/test/test_sectxt.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,146 +42,146 @@
 -----END PGP SIGNATURE-----
 """
 
 
 class SecTxtTestCase(TestCase):
     def test_future_expires(self):
         content = f"Expires: {date.today().year + 3}-01-01T12:00:00Z\n"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._recommendations[0]["code"], "long_expiry")
 
     def test_invalid_expires(self):
         content = "Expires: Nonsense\n"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "invalid_expiry")
         content = "Expires: Thu, 15 Sep 2022 06:03:46 -0700\n"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "invalid_expiry")
 
     def test_expired(self):
         content = "Expires: 2020-01-01T12:00:00Z\n"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "expired")
 
     def test_long_expiry(self):
         content = "Expires: 2030-01-01T12:00:00Z\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         line_info = p._line_info[1]
         self.assertEqual(line_info["type"], "comment")
         self.assertEqual(line_info["value"], "# Wow")
 
     def test_preferred_languages(self):
         # Define content for a valid security.txt.
         static_content = (
             f"Expires: {(date.today() + timedelta(days=10)).isoformat()}"
             "T18:37:07z\n"
             "Contact: mailto:security@example.com\n"
         )
 
         # Single invalid value.
         content = static_content + "Preferred-Languages: English"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "invalid_lang")
 
         # Mix of valid and invalid value.
         content = static_content + "Preferred-Languages: nl, Invalid"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "invalid_lang")
 
         # Both ISO 639-1 (2 char) and ISO 639-2 (3 char) should be valid.
         # Case should be ignored.
         content = static_content + "Preferred-Languages: En, dUT"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertFalse(any(error["code"] == "invalid_lang" for error in p._errors))
 
     def test_prec_ws(self):
         content = "Contact : mailto:me@example.com\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "prec_ws")
 
     def test_empty_key(self):
         content = ": mailto:me@example.com\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "empty_key")
 
     def test_empty_key2(self):
         content = " : mailto:me@example.com\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[1]["code"], "empty_key")
 
     def test_missing_space(self):
         content = "Contact:mailto:me@example.com\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "no_space")
 
     def test_missing_value(self):
         content = "Contact: \n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "empty_value")
 
     def test_no_https(self):
         content = "Contact: http://example.com/contact\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "no_https")
 
     def test_no_uri(self):
         content = "Contact: me@example.com\n# Wow"
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._errors[0]["code"], "no_uri")
 
     def test_signed(self):
-        p = Parser(_signed_example)
+        p = Parser(_signed_example.encode())
         self.assertTrue(p.is_valid())
 
     def test_signed_invalid_pgp(self):
         # Remove required pgp signature header for pgp data error
         content = _signed_example.replace(
             "-----BEGIN PGP SIGNATURE-----", ""
         )
-        p1 = Parser(content)
+        p1 = Parser(content.encode())
         self.assertFalse(p1.is_valid())
         self.assertEqual(
             len([1 for r in p1._errors if r["code"] == "pgp_data_error"]), 1
         )
         # Add dash escaping within the pgp signature for pgp data error
         content = _signed_example.replace(
             "-----BEGIN PGP SIGNATURE-----", "-----BEGIN PGP SIGNATURE-----\n- \n"
         )
-        p2 = Parser(content)
+        p2 = Parser(content.encode())
         self.assertFalse(p2.is_valid())
         self.assertEqual(
             len([1 for r in p2._errors if r["code"] == "pgp_data_error"]), 1
         )
         # create an error in the pgp message by invalidating the base64 encoding of the signature
         content = _signed_example.replace(
             "wpwEAQEIABAFAmTHcawJEDs4gPMoG10dAACN5wP/UozhFqHcUWRNhg4KwfY4", "wpwEAQEIABAFAmTH"
         ).replace(
             "HHXU8bf222naeYJHgaHadLTJJ8YQIQ9N5fYF7K4BM0jPZc48aaUPaBdhNxw+", "HHXU8bf222naeYJHga"
         )
-        p3 = Parser(content)
+        p3 = Parser(content.encode())
         self.assertFalse(p3.is_valid())
         self.assertEqual(
             len([1 for r in p3._errors if r["code"] == "pgp_error"]), 1
         )
 
     def test_signed_no_canonical(self):
         content = _signed_example.replace(
             "Canonical: https://example.com/.well-known/security.txt", ""
         )
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertEqual(p._recommendations[0]["code"], "no_canonical")
 
     def test_signed_dash_escaped(self):
         content = _signed_example.replace("Expires", "- Expires")
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertTrue(p.is_valid())
 
     def test_pgp_signed_formatting(self):
         content = "\r\n" + _signed_example
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertFalse(p.is_valid())
         self.assertTrue(any(d["code"] == "signed_format_issue" for d in p.errors))
 
     def test_unknown_fields(self):
         # Define a security.txt that contains unknown fields (but is valid).
         # The fields Last-updated and Unknown, should be marked as unknown.
         content = (
@@ -190,78 +190,78 @@
             "Contact: mailto:security@example.com\n"
             "Last-updated: {date.today().isoformat()}T12:00:00z\n"
             "Unknown: value\n"
             "Encryption: https://example.com/pgp-key.txt\n"
         )
 
         # By default, recommend that there are unknown fields.
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertTrue(p.is_valid())
         self.assertEqual(
             len([1 for r in p._notifications if r["code"] == "unknown_field"]), 2
         )
 
         # When turned off, there should be no unknown_field recommendations.
-        p = Parser(content, recommend_unknown_fields=False)
+        p = Parser(content.encode(), recommend_unknown_fields=False)
         self.assertTrue(p.is_valid())
         self.assertEqual(
             len([1 for r in p._notifications if r["code"] == "unknown_field"]), 0
         )
 
     def test_no_line_separators(self):
         expire_date = (date.today() + timedelta(days=10)).isoformat()
         single_line_security_txt = (
             "Contact: mailto:security@example.com  Expires: "
             f"{expire_date}T18:37:07z  # All on a single line"
         )
-        p_line_separator = Parser(single_line_security_txt)
+        p_line_separator = Parser(single_line_security_txt.encode())
         self.assertFalse(p_line_separator.is_valid())
         self.assertEqual(
             len([1 for r in p_line_separator._errors if r["code"] == "no_line_separators"]), 1
         )
         line_length_4_no_carriage_feed = (
             "line 1\n"
             "line 2\n"
             "line 3\n"
             "Contact: mailto:security@example.com  Expires"
         )
-        p_length_4 = Parser(line_length_4_no_carriage_feed)
+        p_length_4 = Parser(line_length_4_no_carriage_feed.encode())
         self.assertFalse(p_length_4.is_valid())
         self.assertEqual(
             len([1 for r in p_length_4._errors if r["code"] == "no_line_separators"]), 1
         )
         self.assertEqual(
             [r["line"] for r in p_length_4._errors if r["code"] == "no_line_separators"], [4]
         )
 
     def test_csaf_https_uri(self):
         content = _signed_example.replace(
             "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
             "CSAF: http://example.com/.well-known/csaf/provider-metadata.json",
         )
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertFalse(p.is_valid())
         self.assertEqual(len([1 for r in p._errors if r["code"] == "no_https"]), 1)
 
     def test_csaf_provider_file(self):
         content = _signed_example.replace(
             "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
             "CSAF: https://example.com/.well-known/csaf/other_provider_name.json",
         )
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertFalse(p.is_valid())
         self.assertEqual(len([1 for r in p._errors if r["code"] == "no_csaf_file"]), 1)
 
     def test_multiple_csaf_notification(self):
         content = _signed_example.replace(
             "# CSAF link",
             "# CSAF link\n"
             "CSAF: https://example2.com/.well-known/csaf/provider-metadata.json",
         )
-        p = Parser(content)
+        p = Parser(content.encode())
         self.assertTrue(p.is_valid())
         self.assertEqual(
             len([1 for r in p._recommendations if r["code"] == "multiple_csaf_fields"]), 1
         )
 
     # noinspection PyMethodMayBeStatic
     def test_valid_security_txt(self):
@@ -300,27 +300,35 @@
                 "https://example.com/security.txt", exc=requests.exceptions.ConnectTimeout
             )
             m.get("http://example.com/.well-known/security.txt", text=_signed_example)
             s = SecurityTXT("example.com")
             if not any(d["code"] == "invalid_uri_scheme" for d in s.errors):
                 pytest.fail("invalid_uri_scheme error code should be given")
 
+    def test_byte_order_mark_parser(self):
+        expires = f"Expires: {(date.today() + timedelta(days=10)).isoformat()}T18:37:07z\n"
+        byte_content_with_bom = b'\xef\xbb\xbf\xef\xbb\xbfContact: mailto:me@example.com\n' \
+                                + expires.encode()
+        p = Parser(byte_content_with_bom)
+        self.assertFalse(p.is_valid())
+        self.assertTrue(any(d["code"] == "bom_in_file" for d in p.errors))
+
     # noinspection PyMethodMayBeStatic
     def test_byte_order_mark(self):
         with Mocker() as m:
             expires = f"Expires: {(date.today() + timedelta(days=10)).isoformat()}T18:37:07z\n"
             byte_content_with_bom = b'\xef\xbb\xbf\xef\xbb\xbfContact: mailto:me@example.com\n' \
-                                    + bytes(expires, "utf-8")
+                                    + expires.encode()
             m.get(
                 "https://example.com/.well-known/security.txt",
                 headers={"content-type": "text/plain"},
                 content=byte_content_with_bom,
             )
             s = SecurityTXT("example.com")
-            assert(not s.is_valid())
+            assert (not s.is_valid())
             if not any(d["code"] == "bom_in_file" for d in s.errors):
                 pytest.fail("bom_in_file error code should be given")
 
     # noinspection PyMethodMayBeStatic
     def test_local_file(self):
         # Create a text file to be used for the local test
         test_file_name = "test_security.txt"
```

