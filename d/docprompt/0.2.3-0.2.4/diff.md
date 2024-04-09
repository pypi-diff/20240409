# Comparing `tmp/docprompt-0.2.3.tar.gz` & `tmp/docprompt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.3.tar", max compression
+gzip compressed data, was "docprompt-0.2.4.tar", max compression
```

## Comparing `docprompt-0.2.3.tar` & `docprompt-0.2.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.3/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.3/README.md
--rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.3/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.3/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.3/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.3/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.3/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.3/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.3/docprompt/provenance/util.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.3/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8389 2024-04-05 21:54:30.580449 docprompt-0.2.3/docprompt/schema/document.py
--rw-r--r--   0        0        0     6362 2024-04-05 21:39:49.476813 docprompt-0.2.3/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.3/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.3/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.3/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.3/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.3/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.3/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18333 2024-04-05 21:53:48.708070 docprompt-0.2.3/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.3/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.3/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.3/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.3/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.3/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.3/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.3/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.3/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.3/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.3/docprompt/utils/raster.py
--rw-r--r--   0        0        0     3655 2024-04-05 21:23:49.921077 docprompt-0.2.3/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.3/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-05 21:50:00.054079 docprompt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.3/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.3/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.3/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.3/tests/test_date_extraction.py
--rw-r--r--   0        0        0      971 2024-03-19 02:48:57.067976 docprompt-0.2.3/tests/test_document.py
--rw-r--r--   0        0        0      941 2024-03-19 01:25:52.547395 docprompt-0.2.3/tests/test_search.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.3/tests/util.py
--rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.4/README.md
+-rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.4/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.4/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.4/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.4/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.4/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.4/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.4/docprompt/provenance/util.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.4/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9472 2024-04-09 01:41:32.425414 docprompt-0.2.4/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6362 2024-04-05 21:39:49.476813 docprompt-0.2.4/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.4/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.4/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.4/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.4/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.4/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.4/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18333 2024-04-05 21:53:48.708070 docprompt-0.2.4/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.4/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.4/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.4/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.4/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.4/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.4/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.4/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.4/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.4/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.4/docprompt/utils/raster.py
+-rw-r--r--   0        0        0     3655 2024-04-05 21:23:49.921077 docprompt-0.2.4/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.4/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-09 01:47:50.624269 docprompt-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.4/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.4/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.4/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.4/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.4/tests/test_document.py
+-rw-r--r--   0        0        0     1240 2024-04-09 01:41:32.425414 docprompt-0.2.4/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.4/tests/test_search.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.4/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.4/PKG-INFO
```

### Comparing `docprompt-0.2.3/LICENSE` & `docprompt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/README.md` & `docprompt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/__init__.py` & `docprompt-0.2.4/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/_exec/ghostscript.py` & `docprompt-0.2.4/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/provenance/search.py` & `docprompt-0.2.4/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/provenance/source.py` & `docprompt-0.2.4/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/provenance/util.py` & `docprompt-0.2.4/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/schema/document.py` & `docprompt-0.2.4/docprompt/schema/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,48 @@
 
     width = int(base_width * dpi / 72)
     height = int(base_height * dpi / 72)
 
     return width, height
 
 
+def process_raster_image(
+    image_bytes: bytes,
+    *,
+    do_resize: bool = False,
+    resize_width: Optional[int] = None,
+    resize_height: Optional[int] = None,
+    do_convert: bool = True,
+    image_covert_mode: str = "L",
+    do_quantize: bool = True,
+    quantize_color_count: int = 8,
+):
+    if not do_resize and not do_quantize and not do_convert:
+        return image_bytes
+
+    image = Image.open(BytesIO(image_bytes))
+
+    if do_resize:
+        if resize_width is None or resize_height is None:
+            raise ValueError("Must specify both resize_width and resize_height")
+
+        image = image.resize((resize_width, resize_height))
+
+    if do_convert:
+        image = image.convert(image_covert_mode)
+
+    if do_quantize:
+        image = image.quantize(colors=quantize_color_count)
+
+    buffer = BytesIO()
+    image.save(buffer, format="PNG", optimize=True)
+
+    return buffer.getvalue()
+
+
 class PdfDocument(BaseModel):
     """
     Represents a PDF document
     """
 
     name: str = Field(description="The name of the document")
     file_bytes: bytes = Field(description="The bytes of the document", repr=False)
@@ -153,14 +187,18 @@
     def rasterize_page(
         self,
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
         use_cache: bool = True,
+        do_convert: bool = False,
+        image_covert_mode: str = "L",
+        do_quantize: bool = False,
+        quantize_color_count: int = 8,
     ) -> bytes:
         """
         Rasterizes a page of the document using Ghostscript
         """
         generated_image = False
 
         if page_number < 0 or page_number > self.num_pages:
@@ -182,35 +220,37 @@
 
             generated_image = True
 
         if use_cache and generated_image:
             self._raster_cache.setdefault(dpi, {})
             self._raster_cache[dpi][page_number] = rastered
 
-        if downscale_size:
-            with Image.open(BytesIO(rastered)) as img:
-                width, height = img.size
-                if not (width < downscale_size[0] or height < downscale_size[1]):
-                    img = img.resize(downscale_size)
-                    img_bytes = BytesIO()
-                    img.save(img_bytes, format="PNG")
-                    rastered = img_bytes.getvalue()
+        rastered = process_raster_image(
+            rastered,
+            do_resize=downscale_size is not None,
+            resize_width=downscale_size[0] if downscale_size else None,
+            resize_height=downscale_size[1] if downscale_size else None,
+            do_convert=do_convert,
+            image_covert_mode=image_covert_mode,
+            do_quantize=do_quantize,
+            quantize_color_count=quantize_color_count,
+        )
 
         return rastered
 
     def rasterize_page_to_data_uri(
         self,
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
         use_cache: bool = True,
     ) -> str:
         """
-        Rasterizes a page of the document using Ghostscript and returns a data URI, which can
+        Rasterizes a page of the document using Pdfium and returns a data URI, which can
         be embedded into HTML or passed to large language models
         """
         image_bytes = self.rasterize_page(
             page_number,
             dpi=dpi,
             downscale_size=downscale_size,
             use_cache=use_cache,
@@ -219,15 +259,15 @@
 
     def rasterize_pdf(
         self,
         dpi: int = DEFAULT_DPI,
         use_cache: bool = True,
     ) -> Dict[int, bytes]:
         """
-        Rasterizes the entire document using Ghostscript
+        Rasterizes the entire document using Pdfium
         """
         if (
             use_cache
             and self._raster_cache.get(dpi)
             and len(self._raster_cache[dpi]) == self.num_pages
         ):
             return self._raster_cache[dpi]
```

### Comparing `docprompt-0.2.3/docprompt/schema/layout.py` & `docprompt-0.2.4/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/schema/pipeline.py` & `docprompt-0.2.4/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/base.py` & `docprompt-0.2.4/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/message.py` & `docprompt-0.2.4/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/ocr/gcp.py` & `docprompt-0.2.4/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/ocr/result.py` & `docprompt-0.2.4/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/table_extraction/base.py` & `docprompt-0.2.4/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.2.4/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/tasks/table_extraction/result.py` & `docprompt-0.2.4/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/utils/date_extraction.py` & `docprompt-0.2.4/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/utils/splitter.py` & `docprompt-0.2.4/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/docprompt/utils/util.py` & `docprompt-0.2.4/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/pyproject.toml` & `docprompt-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.3"
+version = "0.2.4"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.3/tests/fixtures/1.pdf` & `docprompt-0.2.4/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/tests/fixtures/1_ocr.json` & `docprompt-0.2.4/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/tests/test_date_extraction.py` & `docprompt-0.2.4/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/tests/test_search.py` & `docprompt-0.2.4/tests/test_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,7 +29,19 @@
     result_all_pages = locator.search("and")
 
     assert len(result_all_pages) == 50
 
     result_page_1 = locator.search("rooted", page_number=1)
 
     assert len(result_page_1) == 1
+
+    result_multiple_words = locator.search("MMAX2 system", page_number=1)
+
+    assert len(result_multiple_words) == 1
+
+    n_best = locator.search_n_best("and", n=3)
+
+    assert len(n_best) == 3
+
+    raw_search = locator.search_raw('content:"rooted"')
+
+    assert len(raw_search) == 1
```

### Comparing `docprompt-0.2.3/tests/util.py` & `docprompt-0.2.4/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.3/PKG-INFO` & `docprompt-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.3
+Version: 0.2.4
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 Provides-Extra: search
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.3 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.2.4 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Provides-
-Extra: azure Provides-Extra: dev Provides-Extra: doc Provides-Extra: google
-Provides-Extra: search Provides-Extra: test Requires-Dist: azure-ai-
-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist: bump2version
-(>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8 (>=6.1.0,<7.0.0) ;
-extra == "test" Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra ==
-"test" Requires-Dist: fsspec (>=2022.11.0) Requires-Dist: google-cloud-
-documentai (>=2.20.0) ; extra == "google" Requires-Dist: isort
-(>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ;
-extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist:
-mkdocs-material-extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings
-(>=0.15.2,<0.16.0) ; extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ;
-extra == "test" Requires-Dist: networkx (>=2.8.8) ; extra == "search" Requires-
-Dist: numpy (>=1.20.3,<2.0.0) Requires-Dist: pillow (>=9.0.1) Requires-Dist:
-pip (>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-commit
-(>=2.12.0,<3.0.0) ; extra == "dev" Requires-Dist: pydantic (>=2.1.0) Requires-
-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-Dist: pytest (>=7.4.2,<8.0.0) ;
-extra == "test" Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "test"
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-magic
-(>=0.4.24) Requires-Dist: rapidfuzz (>=3.0.0) Requires-Dist: rtree
-(>=1.2.0,<2.0.0) ; extra == "search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ;
-extra == "test" Requires-Dist: tantivy (>=0.21.0,<0.22.0) ; extra == "search"
-Requires-Dist: tenacity (>=7.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ;
-extra == "dev" Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-
-Dist: tqdm (>=4.61.0) Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
-Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev" Description-
-Content-Type: text/markdown [![pypi](https://img.shields.io/pypi/v/
-docprompt.svg)](https://pypi.org/project/docprompt/) [![python](https://
-img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/
-docprompt/) [![Build Status](https://github.com/Page-Leaf/Docprompt/actions/
-workflows/dev.yml/badge.svg)](https://github.com/Page-Leaf/docprompt/actions/
-workflows/dev.yml) [![codecov](https://codecov.io/gh/Page-Leaf/Docprompt/
-branch/main/graphs/badge.svg)](https://codecov.io/github/Page-Leaf/Docprompt)
+Python :: 3.8 Provides-Extra: azure Provides-Extra: dev Provides-Extra: doc
+Provides-Extra: google Provides-Extra: search Provides-Extra: test Requires-
+Dist: azure-ai-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist:
+bump2version (>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8
+(>=6.1.0,<7.0.0) ; extra == "test" Requires-Dist: flake8-docstrings
+(>=1.7.0,<2.0.0) ; extra == "test" Requires-Dist: fsspec (>=2022.11.0)
+Requires-Dist: google-cloud-documentai (>=2.20.0) ; extra == "google" Requires-
+Dist: isort (>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs
+(>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-autorefs
+(>=0.2.1,<0.3.0) ; extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
+(>=1.0.0,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-material
+(>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-extensions
+(>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ; extra ==
+"doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ; extra == "test" Requires-Dist:
+networkx (>=2.8.8) ; extra == "search" Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pillow (>=9.0.1) Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra
+== "dev" Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev" Requires-
+Dist: pydantic (>=2.1.0) Requires-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-
+Dist: pytest (>=7.4.2,<8.0.0) ; extra == "test" Requires-Dist: pytest-cov
+(>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24) Requires-Dist:
+rapidfuzz (>=3.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0) ; extra == "search"
+Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test" Requires-Dist: tantivy
+(>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist: tenacity (>=7.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tox
+(>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm (>=4.61.0) Requires-
+Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
+(>=20.2.2,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown [!
+[pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/project/
+docprompt/) [![python](https://img.shields.io/pypi/pyversions/docprompt.svg)]
+(https://pypi.org/project/docprompt/) [![Build Status](https://github.com/Page-
+Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://github.com/Page-
+Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://codecov.io/gh/
+Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://codecov.io/github/
+Page-Leaf/Docprompt)
                                     _[_L_o_g_o_]
                               ******** DDooccpprroommpptt ********
                         Document AI, powered by LLM's
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                        Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # About Docprompt is a library for Document AI. It aims to make enterprise-
```

