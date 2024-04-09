# Comparing `tmp/datasette-extract-0.1a3.tar.gz` & `tmp/datasette-extract-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-extract-0.1a3.tar", last modified: Wed Mar 13 15:34:44 2024, max compression
+gzip compressed data, was "datasette-extract-0.1a4.tar", last modified: Tue Apr  9 19:25:46 2024, max compression
```

## Comparing `datasette-extract-0.1a3.tar` & `datasette-extract-0.1a4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.675014 datasette-extract-0.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-13 15:34:44.671014 datasette-extract-0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.663014 datasette-extract-0.1a3/datasette_extract/
--rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.671014 datasette-extract-0.1a3/datasette_extract/static/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/static/extract.css
--rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/static/heic2any-0.0.4.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/static/pdf.worker.mjs
--rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/static/pdfjs-dist-4-0-379.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.671014 datasette-extract-0.1a3/datasette_extract/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/templates/_extract_drop_handler.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/templates/extract.html
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/templates/extract_create_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/templates/extract_progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/datasette_extract/templates/extract_to_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.671014 datasette-extract-0.1a3/datasette_extract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-13 15:34:44.000000 datasette-extract-0.1a3/datasette_extract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 15:34:44.675014 datasette-extract-0.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:34:44.671014 datasette-extract-0.1a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-13 15:34:38.000000 datasette-extract-0.1a3/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.783438 datasette-extract-0.1a4/datasette_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/extract.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/heic2any-0.0.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/pdf.worker.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/static/pdfjs-dist-4-0-379.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/_extract_drop_handler.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_create_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/datasette_extract/templates/extract_to_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/datasette_extract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 19:25:46.000000 datasette-extract-0.1a4/datasette_extract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:25:46.791438 datasette-extract-0.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:46.787438 datasette-extract-0.1a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-09 19:25:40.000000 datasette-extract-0.1a4/tests/test_web.py
```

### Comparing `datasette-extract-0.1a3/LICENSE` & `datasette-extract-0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/PKG-INFO` & `datasette-extract-0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a3
+Version: 0.1a4
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
```

### Comparing `datasette-extract-0.1a3/README.md` & `datasette-extract-0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/__init__.py` & `datasette-extract-0.1a4/datasette_extract/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,53 +277,40 @@
                 db = Database(conn)
                 db[table].insert(row)
 
         return _write
 
     error = None
 
-    async def ocr_image(image_bytes):
-        base64_image = base64.b64encode(image_bytes).decode("utf-8")
-        messages = [
-            {
-                "role": "system",
-                "content": "Run OCR and return all of the text in this image, with newlines where appropriate",
-            },
-            {
-                "role": "user",
-                "content": [
-                    {
-                        "type": "image_url",
-                        "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"},
-                    }
-                ],
-            },
-        ]
-        response = await async_client.chat.completions.create(
-            model="gpt-4-vision-preview", messages=messages, max_tokens=400
-        )
-        return response.choices[0].message.content
-
     try:
         messages = []
         if instructions:
             messages.append({"role": "system", "content": instructions})
+        if image_is_provided(image):
+            image_bytes = await image.read()
+            base64_image = base64.b64encode(image_bytes).decode("utf-8")
+            messages.append(
+                {
+                    "role": "user",
+                    "content": [
+                        {
+                            "type": "image_url",
+                            "image_url": {
+                                "url": f"data:image/jpeg;base64,{base64_image}"
+                            },
+                        }
+                    ],
+                }
+            )
         if content:
             messages.append({"role": "user", "content": content})
-        if image_is_provided(image):
-            # Run a separate thing to OCR the image first, because gpt-4-vision can't handle tools yet
-            image_content = await ocr_image(await image.read())
-            if image_content:
-                messages.append({"role": "user", "content": image_content})
-            else:
-                raise ValueError("Could not extract text from image")
 
         async for chunk in await async_client.chat.completions.create(
             stream=True,
-            model="gpt-4-turbo-preview",
+            model="gpt-4-turbo",
             messages=messages,
             tools=[
                 {
                     "type": "function",
                     "function": {
                         "name": "extract_data",
                         "description": "Extract data matching this schema",
@@ -466,27 +453,29 @@
 def database_actions(datasette, actor, database):
     async def inner():
         if not await can_extract(datasette, actor, database):
             return []
         return [
             {
                 "href": datasette.urls.database(database) + "/-/extract",
-                "label": "Create table with extracted data",
+                "label": "Create table with AI extracted data",
+                "description": "Paste in text or an image to extract structured data",
             }
         ]
 
     return inner
 
 
 @hookimpl
 def table_actions(datasette, actor, database, table):
     async def inner():
         if not await can_extract(datasette, actor, database, table):
             return []
         return [
             {
                 "href": datasette.urls.table(database, table) + "/-/extract",
-                "label": "Extract data into this table",
+                "label": "Extract data into this table with AI",
+                "description": "Paste in text or an image to extract structured data",
             }
         ]
 
     return inner
```

### Comparing `datasette-extract-0.1a3/datasette_extract/static/heic2any-0.0.4.min.js` & `datasette-extract-0.1a4/datasette_extract/static/heic2any-0.0.4.min.js`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/static/pdf.worker.mjs` & `datasette-extract-0.1a4/datasette_extract/static/pdf.worker.mjs`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/static/pdfjs-dist-4-0-379.js` & `datasette-extract-0.1a4/datasette_extract/static/pdfjs-dist-4-0-379.js`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/templates/_extract_drop_handler.html` & `datasette-extract-0.1a4/datasette_extract/templates/_extract_drop_handler.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/templates/extract_create_table.html` & `datasette-extract-0.1a4/datasette_extract/templates/extract_create_table.html`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/datasette_extract/templates/extract_progress.html` & `datasette-extract-0.1a4/datasette_extract/templates/extract_progress.html`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,27 @@
 
 async function pollData() {
     const response = await fetch(pollUrl);
     const data = await response.json();
     if (data && data.items && data.items.length) {
         outputElement.textContent = JSON.stringify(data.items, null, 2);
     }
+    let finishMessage = 'Extraction complete!';
+    if (data && data.error) {
+        outputElement.textContent = `Error: ${data.error}`;
+        outputElement.style.color = "red";
+        finishMessage = 'Extraction failed';
+    }
     if (data.done) {
         clearInterval(pollInterval);
         const loadingSpinner = document.getElementById("loadingSpinner");
         loadingSpinner.parentNode.removeChild(loadingSpinner);
         const doneMessage = document.createElement("p");
         doneMessage.style.fontWeight = "bold";
-        doneMessage.textContent = "Extraction complete!";
+        doneMessage.textContent = finishMessage;
         outputElement.parentNode.appendChild(doneMessage);
     }
 }
 
 const pollInterval = setInterval(pollData, 1000);
 pollData();
 </script>
```

### Comparing `datasette-extract-0.1a3/datasette_extract/templates/extract_to_table.html` & `datasette-extract-0.1a4/datasette_extract/templates/extract_to_table.html`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
   </tr>
   {% for run in previous_runs %}
   <tr>
     <td>{{ run.id }}</td>
     <td>{{ run.created }}</td>
     <td>{{ run.completed or "" }}</td>
     <td>{{ run.properties }}</td>
-    <td>{{ run.instructions }}</td>
+    <td>{{ run.instructions or "" }}</td>
     <td>{{ run.error or "" }}</td>
     <td>{{ run.num_items }}</td>
   </tr>
   {% endfor %}
 </table>
 </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -14,9 +14,9 @@
 [Extract]
 {% include "_extract_drop_handler.html" %} {% if previous_runs %}
 ********** PPrreevviioouuss eexxttrraaccttiioonn ttaasskkss **********
 IIDD     ccrreeaatteedd     ccoommpplleetteedd     pprrooppeerrttiieess     iinnssttrruuccttiioonnss     eerrrroorr     nnuumm__iitteemmss
 {      {           {             {              {                {         {
 {      {           {             {              {                {         {
 run.id run.created run.completed run.properties run.instructions run.error run.num_items
-}}     }}          or "" }}      }}             }}               or "" }}  }}
+}}     }}          or "" }}      }}             or "" }}         or "" }}  }}
 {% endif %} {% endblock %}
```

### Comparing `datasette-extract-0.1a3/datasette_extract.egg-info/PKG-INFO` & `datasette-extract-0.1a4/datasette_extract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a3
+Version: 0.1a4
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
```

### Comparing `datasette-extract-0.1a3/datasette_extract.egg-info/SOURCES.txt` & `datasette-extract-0.1a4/datasette_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-extract-0.1a3/pyproject.toml` & `datasette-extract-0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-extract"
-version = "0.1a3"
+version = "0.1a4"
 description = "Import unstructured data (text and images) into structured tables"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette-extract-0.1a3/tests/test_web.py` & `datasette-extract-0.1a4/tests/test_web.py`

 * *Files identical despite different names*

