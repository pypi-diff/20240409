# Comparing `tmp/gradio_pdf-0.0.5.tar.gz` & `tmp/gradio_pdf-0.0.6.tar.gz`

## Comparing `gradio_pdf-0.0.5.tar` & `gradio_pdf-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/__init__.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/pdf.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/pdf.pyi
--rw-r--r--   0        0        0   767453 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/Index-9e3f581a.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/index.js
--rw-r--r--   0        0        0    14825 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/style.css
--rw-r--r--   0        0        0    78006 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/wrapper-98f94c21-15fa1cb3.js
--rw-r--r--   0        0        0   560476 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/example/index.js
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/backend/gradio_pdf/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/_app.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/app.py
--rw-r--r--   0        0        0   127928 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/contract.pdf
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/css.css
--rw-r--r--   0        0        0   372153 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/invoice_2.pdf
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/requirements.txt
--rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/sample_invoice.pdf
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/demo/space.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/frontend/Example.svelte
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/frontend/Index.svelte
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/frontend/PdfUploadText.svelte
--rw-r--r--   0        0        0    64861 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/frontend/package-lock.json
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/frontend/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/LICENSE
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/README.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11575 2020-02-02 00:00:00.000000 gradio_pdf-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/pdf.py
+-rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/pdf.pyi
+-rw-r--r--   0        0        0   767472 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/Index-94e506c5.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/index.js
+-rw-r--r--   0        0        0    14825 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/style.css
+-rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/wrapper-98f94c21-d1a5537c.js
+-rw-r--r--   0        0        0   560467 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/example/index.js
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/backend/gradio_pdf/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/app.py
+-rw-r--r--   0        0        0   127928 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/contract.pdf
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/css.css
+-rw-r--r--   0        0        0   372153 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/invoice_2.pdf
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/requirements.txt
+-rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/sample_invoice.pdf
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/demo/space.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/frontend/Example.svelte
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/frontend/Index.svelte
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/frontend/PdfUploadText.svelte
+-rw-r--r--   0        0        0    64861 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/frontend/package-lock.json
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/frontend/package.json
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/.gitignore
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/README.md
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 gradio_pdf-0.0.6/PKG-INFO
```

### Comparing `gradio_pdf-0.0.5/backend/gradio_pdf/pdf.pyi` & `gradio_pdf-0.0.6/backend/gradio_pdf/pdf.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             queue: If True, will place the request on the queue, if the queue has been enabled. If False, will not put this event on the queue, even if the queue has been enabled. If None, will use the queue setting of the gradio app.
             batch: If True, then the function should process a batch of inputs, meaning that it should accept a list of input values for each parameter. The lists should be of equal length (and be up to length `max_batch_size`). The function is then *required* to return a tuple of lists (even if there is only 1 output component), with each list in the tuple corresponding to one output component.
             max_batch_size: Maximum number of inputs to batch together if this is called from the queue (only relevant if batch=True)
             preprocess: If False, will not run preprocessing of component data before running 'fn' (e.g. leaving it as a base64 string if this method is called with the `Image` component).
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
-            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` event) would allow a second submission after the pending event is complete.
+            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
             show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
@@ -119,14 +119,14 @@
             queue: If True, will place the request on the queue, if the queue has been enabled. If False, will not put this event on the queue, even if the queue has been enabled. If None, will use the queue setting of the gradio app.
             batch: If True, then the function should process a batch of inputs, meaning that it should accept a list of input values for each parameter. The lists should be of equal length (and be up to length `max_batch_size`). The function is then *required* to return a tuple of lists (even if there is only 1 output component), with each list in the tuple corresponding to one output component.
             max_batch_size: Maximum number of inputs to batch together if this is called from the queue (only relevant if batch=True)
             preprocess: If False, will not run preprocessing of component data before running 'fn' (e.g. leaving it as a base64 string if this method is called with the `Image` component).
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
-            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` event) would allow a second submission after the pending event is complete.
+            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
             show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
```

### Comparing `gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/Index-9e3f581a.js` & `gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/Index-94e506c5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3328,15 +3328,15 @@
             } = _, S = {
                 predict: N,
                 submit: D,
                 view_api: G,
                 component_server: X
             }, w = T ?? !0;
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
-                const I = await import("./wrapper-98f94c21-15fa1cb3.js");
+                const I = await import("./wrapper-98f94c21-d1a5537c.js");
                 NodeBlob = (await Promise.resolve().then(() => __viteBrowserExternal)).Blob, global.WebSocket = I.WebSocket;
             }
             const {
                 ws_protocol: C,
                 http_protocol: P,
                 host: b,
                 space_id: k
@@ -3427,16 +3427,16 @@
             }
 
             function D(I, B, ee) {
                 let Y, q;
                 if (typeof I == "number")
                     Y = I, q = M.unnamed_endpoints[Y];
                 else {
-                    const Q = I.replace(/^\//, "");
-                    Y = p[Q], q = M.named_endpoints[I.trim()];
+                    const Z = I.replace(/^\//, "");
+                    Y = p[Z], q = M.named_endpoints[I.trim()];
                 }
                 if (typeof Y != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
                 let le, pe, we = y.protocol ?? "sse";
                 const be = typeof I == "number" ? "/predict" : I;
@@ -3445,17 +3445,17 @@
                 const f = {};
                 let v = "";
                 typeof window < "u" && (v = new URLSearchParams(window.location.search).toString()), l(
                     `${P}//${resolve_root(b, y.path, !0)}`,
                     B,
                     q,
                     r
-                ).then((Q) => {
+                ).then((Z) => {
                     if (R = {
-                            data: Q || [],
+                            data: Z || [],
                             event_data: ee,
                             fn_index: Y
                         }, skip_queue(Y, y))
                         A({
                             type: "status",
                             endpoint: be,
                             stage: "pending",
@@ -3701,48 +3701,48 @@
                                 endpoint: be,
                                 fn_index: Y
                             }), pe.close()));
                         };
                     }
                 });
 
-                function A(Q) {
-                    const ue = f[Q.type] || [];
-                    ue == null || ue.forEach((me) => me(Q));
+                function A(Z) {
+                    const ue = f[Z.type] || [];
+                    ue == null || ue.forEach((me) => me(Z));
                 }
 
-                function O(Q, ce) {
+                function O(Z, ce) {
                     const ue = f,
-                        me = ue[Q] || [];
-                    return ue[Q] = me, me == null || me.push(ce), {
+                        me = ue[Z] || [];
+                    return ue[Z] = me, me == null || me.push(ce), {
                         on: O,
                         off: H,
                         cancel: z,
                         destroy: ae
                     };
                 }
 
-                function H(Q, ce) {
+                function H(Z, ce) {
                     const ue = f;
-                    let me = ue[Q] || [];
-                    return me = me == null ? void 0 : me.filter((fe) => fe !== ce), ue[Q] = me, {
+                    let me = ue[Z] || [];
+                    return me = me == null ? void 0 : me.filter((fe) => fe !== ce), ue[Z] = me, {
                         on: O,
                         off: H,
                         cancel: z,
                         destroy: ae
                     };
                 }
                 async function z() {
-                    const Q = {
+                    const Z = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
                     };
-                    g = Q, A({
-                        ...Q,
+                    g = Z, A({
+                        ...Z,
                         type: "status",
                         endpoint: be,
                         fn_index: Y
                     });
                     let ce = {};
                     we === "ws" ? (le && le.readyState === 0 ? le.addEventListener("open", () => {
                         le.close();
@@ -3770,17 +3770,17 @@
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
                 function ae() {
-                    for (const Q in f)
-                        f[Q].forEach((ce) => {
-                            H(Q, ce);
+                    for (const Z in f)
+                        f[Z].forEach((ce) => {
+                            H(Z, ce);
                         });
                 }
                 return {
                     on: O,
                     off: H,
                     cancel: z,
                     destroy: ae
@@ -8259,15 +8259,15 @@
             var __webpack_modules__ = [,
                     /* 1 */
                     /***/
                     (t, e) => {
                         var Ye;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
-                        }), e.VerbosityLevel = e.Util = e.UnknownErrorException = e.UnexpectedResponseException = e.TextRenderingMode = e.RenderingIntentFlag = e.PromiseCapability = e.PermissionFlag = e.PasswordResponses = e.PasswordException = e.PageActionEventType = e.OPS = e.MissingPDFException = e.MAX_IMAGE_SIZE_TO_CACHE = e.LINE_FACTOR = e.LINE_DESCENT_FACTOR = e.InvalidPDFException = e.ImageKind = e.IDENTITY_MATRIX = e.FormatError = e.FeatureTest = e.FONT_IDENTITY_MATRIX = e.DocumentActionEventType = e.CMapCompressionType = e.BaseException = e.BASELINE_FACTOR = e.AnnotationType = e.AnnotationReplyType = e.AnnotationPrefix = e.AnnotationMode = e.AnnotationFlag = e.AnnotationFieldFlag = e.AnnotationEditorType = e.AnnotationEditorPrefix = e.AnnotationEditorParamsType = e.AnnotationBorderStyleType = e.AnnotationActionEventType = e.AbortException = void 0, e.assert = le, e.bytesToString = z, e.createValidAbsoluteUrl = we, e.getModificationDate = xe, e.getUuid = Xe, e.getVerbosityLevel = B, e.info = ee, e.isArrayBuffer = ge, e.isArrayEqual = Ce, e.isNodeJS = void 0, e.normalizeUnicode = ze, e.objectFromMap = ue, e.objectSize = ce, e.setVerbosityLevel = I, e.shadow = be, e.string32 = Q, e.stringToBytes = ae, e.stringToPDFString = _e, e.stringToUTF8String = ie, e.unreachable = q, e.utf8StringToString = se, e.warn = Y;
+                        }), e.VerbosityLevel = e.Util = e.UnknownErrorException = e.UnexpectedResponseException = e.TextRenderingMode = e.RenderingIntentFlag = e.PromiseCapability = e.PermissionFlag = e.PasswordResponses = e.PasswordException = e.PageActionEventType = e.OPS = e.MissingPDFException = e.MAX_IMAGE_SIZE_TO_CACHE = e.LINE_FACTOR = e.LINE_DESCENT_FACTOR = e.InvalidPDFException = e.ImageKind = e.IDENTITY_MATRIX = e.FormatError = e.FeatureTest = e.FONT_IDENTITY_MATRIX = e.DocumentActionEventType = e.CMapCompressionType = e.BaseException = e.BASELINE_FACTOR = e.AnnotationType = e.AnnotationReplyType = e.AnnotationPrefix = e.AnnotationMode = e.AnnotationFlag = e.AnnotationFieldFlag = e.AnnotationEditorType = e.AnnotationEditorPrefix = e.AnnotationEditorParamsType = e.AnnotationBorderStyleType = e.AnnotationActionEventType = e.AbortException = void 0, e.assert = le, e.bytesToString = z, e.createValidAbsoluteUrl = we, e.getModificationDate = xe, e.getUuid = Xe, e.getVerbosityLevel = B, e.info = ee, e.isArrayBuffer = ge, e.isArrayEqual = Ce, e.isNodeJS = void 0, e.normalizeUnicode = ze, e.objectFromMap = ue, e.objectSize = ce, e.setVerbosityLevel = I, e.shadow = be, e.string32 = Z, e.stringToBytes = ae, e.stringToPDFString = _e, e.stringToUTF8String = ie, e.unreachable = q, e.utf8StringToString = se, e.warn = Y;
                         const i = typeof process == "object" && process + "" == "[object process]" && !process.versions.nw && !(process.versions.electron && process.type && process.type !== "browser");
                         e.isNodeJS = i;
                         const n = [1, 0, 0, 1, 0, 0];
                         e.IDENTITY_MATRIX = n;
                         const s = [1e-3, 0, 0, 1e-3, 0, 0];
                         e.FONT_IDENTITY_MATRIX = s;
                         const l = 1e7;
@@ -8699,15 +8699,15 @@
                             const ne = de.length,
                                 J = new Uint8Array(ne);
                             for (let ve = 0; ve < ne; ++ve)
                                 J[ve] = de.charCodeAt(ve) & 255;
                             return J;
                         }
 
-                        function Q(de) {
+                        function Z(de) {
                             return String.fromCharCode(de >> 24 & 255, de >> 16 & 255, de >> 8 & 255, de & 255);
                         }
 
                         function ce(de) {
                             return Object.keys(de).length;
                         }
 
@@ -8816,23 +8816,23 @@
                             }
                             static bezierBoundingBox(ne, J, ve, Se, tt, et, te, Te) {
                                 const Ne = [],
                                     ke = [
                                         [],
                                         []
                                     ];
-                                let $e, Be, Qe, Ae, Ke, Oe, U, u;
-                                for (let Z = 0; Z < 2; ++Z) {
-                                    if (Z === 0 ? (Be = 6 * ne - 12 * ve + 6 * tt, $e = -3 * ne + 9 * ve - 9 * tt + 3 * te, Qe = 3 * ve - 3 * ne) : (Be = 6 * J - 12 * Se + 6 * et, $e = -3 * J + 9 * Se - 9 * et + 3 * Te, Qe = 3 * Se - 3 * J), Math.abs($e) < 1e-12) {
+                                let $e, Be, Ze, Ae, Ke, Oe, U, u;
+                                for (let Q = 0; Q < 2; ++Q) {
+                                    if (Q === 0 ? (Be = 6 * ne - 12 * ve + 6 * tt, $e = -3 * ne + 9 * ve - 9 * tt + 3 * te, Ze = 3 * ve - 3 * ne) : (Be = 6 * J - 12 * Se + 6 * et, $e = -3 * J + 9 * Se - 9 * et + 3 * Te, Ze = 3 * Se - 3 * J), Math.abs($e) < 1e-12) {
                                         if (Math.abs(Be) < 1e-12)
                                             continue;
-                                        Ae = -Qe / Be, 0 < Ae && Ae < 1 && Ne.push(Ae);
+                                        Ae = -Ze / Be, 0 < Ae && Ae < 1 && Ne.push(Ae);
                                         continue;
                                     }
-                                    U = Be * Be - 4 * Qe * $e, u = Math.sqrt(U), !(U < 0) && (Ke = (-Be + u) / (2 * $e), 0 < Ke && Ke < 1 && Ne.push(Ke), Oe = (-Be - u) / (2 * $e), 0 < Oe && Oe < 1 && Ne.push(Oe));
+                                    U = Be * Be - 4 * Ze * $e, u = Math.sqrt(U), !(U < 0) && (Ke = (-Be + u) / (2 * $e), 0 < Ke && Ke < 1 && Ne.push(Ke), Oe = (-Be - u) / (2 * $e), 0 < Oe && Oe < 1 && Ne.push(Oe));
                                 }
                                 let L = Ne.length,
                                     j;
                                 const V = L;
                                 for (; L--;)
                                     Ae = Ne[L], j = 1 - Ae, ke[0][L] = j * j * j * ne + 3 * j * j * Ae * ve + 3 * j * Ae * Ae * tt + Ae * Ae * Ae * te, ke[1][L] = j * j * j * J + 3 * j * j * Ae * Se + 3 * j * Ae * Ae * et + Ae * Ae * Ae * Te;
                                 return ke[0][V] = ne, ke[1][V] = J, ke[0][V + 1] = te, ke[1][V + 1] = Te, ke[0].length = ke[1].length = V + 2, [Math.min(...ke[0]), Math.min(...ke[1]), Math.max(...ke[0]), Math.max(...ke[1])];
@@ -8883,30 +8883,30 @@
                                     return !1;
                             return !0;
                         }
 
                         function xe(de = /* @__PURE__ */ new Date()) {
                             return [de.getUTCFullYear().toString(), (de.getUTCMonth() + 1).toString().padStart(2, "0"), de.getUTCDate().toString().padStart(2, "0"), de.getUTCHours().toString().padStart(2, "0"), de.getUTCMinutes().toString().padStart(2, "0"), de.getUTCSeconds().toString().padStart(2, "0")].join("");
                         }
-                        class Ue {
+                        class He {
                             constructor() {
                                 W(this, Ye, !1);
                                 this.promise = new Promise((ne, J) => {
                                     this.resolve = (ve) => {
                                         oe(this, Ye, !0), ne(ve);
                                     }, this.reject = (ve) => {
                                         oe(this, Ye, !0), J(ve);
                                     };
                                 });
                             }
                             get settled() {
                                 return a(this, Ye);
                             }
                         }
-                        Ye = new WeakMap(), e.PromiseCapability = Ue;
+                        Ye = new WeakMap(), e.PromiseCapability = He;
                         let We = null,
                             je = null;
 
                         function ze(de) {
                             return We || (We = /([\u00a0\u00b5\u037e\u0eb3\u2000-\u200a\u202f\u2126\ufb00-\ufb04\ufb06\ufb20-\ufb36\ufb38-\ufb3c\ufb3e\ufb40-\ufb41\ufb43-\ufb44\ufb46-\ufba1\ufba4-\ufba9\ufbae-\ufbb1\ufbd3-\ufbdc\ufbde-\ufbe7\ufbea-\ufbf8\ufbfc-\ufbfd\ufc00-\ufc5d\ufc64-\ufcf1\ufcf5-\ufd3d\ufd88\ufdf4\ufdfa-\ufdfb\ufe71\ufe77\ufe79\ufe7b\ufe7d]+)|(\ufb05+)/gu, je = /* @__PURE__ */ new Map([
                                 ["ﬅ", "ſt"]
                             ])), de.replaceAll(We, (ne, J, ve) => J ? J.normalize("NFKC") : je.get(ve));
@@ -8997,15 +8997,15 @@
                                 f = M.stopAtErrors !== !0,
                                 v = Number.isInteger(M.maxImageSize) && M.maxImageSize > -1 ? M.maxImageSize : -1,
                                 A = M.isEvalSupported !== !1,
                                 O = typeof M.isOffscreenCanvasSupported == "boolean" ? M.isOffscreenCanvasSupported : !_util.isNodeJS,
                                 H = Number.isInteger(M.canvasMaxAreaInBytes) ? M.canvasMaxAreaInBytes : -1,
                                 z = typeof M.disableFontFace == "boolean" ? M.disableFontFace : _util.isNodeJS,
                                 ae = M.fontExtraProperties === !0,
-                                Q = M.enableXfa === !0,
+                                Z = M.enableXfa === !0,
                                 ce = M.ownerDocument || globalThis.document,
                                 ue = M.disableRange === !0,
                                 me = M.disableStream === !0,
                                 fe = M.disableAutoFetch === !0,
                                 Pe = M.pdfBug === !0,
                                 Fe = ee ? ee.length : M.length ?? NaN,
                                 Ee = typeof M.useSystemFonts == "boolean" ? M.useSystemFonts : !_util.isNodeJS && !z,
@@ -9025,30 +9025,30 @@
                             };
                             if (De || (ge.cMapReaderFactory = new R({
                                     baseUrl: we,
                                     isCompressed: be
                                 }), ge.standardFontDataFactory = new g({
                                     baseUrl: d
                                 })), !q) {
-                                const Ue = {
+                                const He = {
                                     verbosity: le,
                                     port: _worker_options.GlobalWorkerOptions.workerPort
                                 };
-                                q = Ue.port ? PDFWorker.fromPort(Ue) : new PDFWorker(Ue), m._worker = q;
+                                q = He.port ? PDFWorker.fromPort(He) : new PDFWorker(He), m._worker = q;
                             }
                             const Ce = {
                                     docId: N,
                                     apiVersion: "3.11.174",
                                     data: X,
                                     password: B,
                                     disableAutoFetch: fe,
                                     rangeChunkSize: Y,
                                     length: Fe,
                                     docBaseUrl: pe,
-                                    enableXfa: Q,
+                                    enableXfa: Z,
                                     evaluatorOptions: {
                                         maxImageSize: v,
                                         disableFontFace: z,
                                         ignoreErrors: f,
                                         isEvalSupported: A,
                                         isOffscreenCanvasSupported: O,
                                         canvasMaxAreaInBytes: H,
@@ -9059,24 +9059,24 @@
                                     }
                                 },
                                 xe = {
                                     ignoreErrors: f,
                                     isEvalSupported: A,
                                     disableFontFace: z,
                                     fontExtraProperties: ae,
-                                    enableXfa: Q,
+                                    enableXfa: Z,
                                     ownerDocument: ce,
                                     disableAutoFetch: fe,
                                     pdfBug: Pe,
                                     styleElement: se
                                 };
                             return q.promise.then(function() {
                                 if (m.destroyed)
                                     throw new Error("Loading aborted");
-                                const Ue = _fetchDocument(q, Ce),
+                                const He = _fetchDocument(q, Ce),
                                     We = new Promise(function(je) {
                                         let ze;
                                         ee ? ze = new _transport_stream.PDFDataTransportStream({
                                             length: Fe,
                                             initialData: ee.initialData,
                                             progressiveDone: ee.progressiveDone,
                                             contentDispositionFilename: ee.contentDispositionFilename,
@@ -9088,15 +9088,15 @@
                                             httpHeaders: G,
                                             withCredentials: I,
                                             rangeChunkSize: Y,
                                             disableRange: ue,
                                             disableStream: me
                                         })), je(ze);
                                     });
-                                return Promise.all([Ue, We]).then(function([je, ze]) {
+                                return Promise.all([He, We]).then(function([je, ze]) {
                                     if (m.destroyed)
                                         throw new Error("Loading aborted");
                                     const Xe = new _message_handler.MessageHandler(N, je, q.port),
                                         Ge = new WorkerTransport(Xe, m, ze, xe, ge);
                                     m._transport = Ge, Xe.send("Ready", null);
                                 });
                             }).catch(m._capability.reject), m;
@@ -10539,16 +10539,16 @@
                                         pageWidth: A,
                                         pageHeight: O,
                                         pageX: H,
                                         pageY: z
                                     }
                                 } = this.parent.viewport;
                                 this.rotation = v, this.pageRotation = (360 + v - this._uiManager.viewParameters.rotation) % 360, this.pageDimensions = [A, O], this.pageTranslation = [H, z];
-                                const [ae, Q] = this.parentDimensions;
-                                this.x = f.x / ae, this.y = f.y / Q, this.isAttachedToDOM = !1, this.deleted = !1;
+                                const [ae, Z] = this.parentDimensions;
+                                this.x = f.x / ae, this.y = f.y / Z, this.isAttachedToDOM = !1, this.deleted = !1;
                             }
                             get editorType() {
                                 return Object.getPrototypeOf(this).constructor._type;
                             }
                             static get _defaultLineColor() {
                                 return (0, s.shadow)(this, "_defaultLineColor", this._colorManager.getHexCode("CanvasText"));
                             }
@@ -10662,16 +10662,16 @@
                                     } = this.div.getBoundingClientRect();
                                     this.parent.findNewParent(this, ce, ue) && (this.x -= Math.floor(this.x), this.y -= Math.floor(this.y));
                                 }
                                 let {
                                     x: H,
                                     y: z
                                 } = this;
-                                const [ae, Q] = K(this, M, Ut).call(this);
-                                H += ae, z += Q, this.div.style.left = `${(100 * H).toFixed(2)}%`, this.div.style.top = `${(100 * z).toFixed(2)}%`, this.div.scrollIntoView({
+                                const [ae, Z] = K(this, M, Ut).call(this);
+                                H += ae, z += Z, this.div.style.left = `${(100 * H).toFixed(2)}%`, this.div.style.top = `${(100 * z).toFixed(2)}%`, this.div.scrollIntoView({
                                     block: "nearest"
                                 });
                             }
                             fixAndSetPosition() {
                                 const [f, v] = this.pageDimensions;
                                 let {
                                     x: A,
@@ -10690,16 +10690,16 @@
                                         A = Math.min(f, Math.max(H, A)), O = Math.min(v, Math.max(z, O));
                                         break;
                                     case 270:
                                         A = Math.min(f, Math.max(z, A)), O = Math.max(0, Math.min(v - H, O));
                                         break;
                                 }
                                 this.x = A /= f, this.y = O /= v;
-                                const [ae, Q] = K(this, M, Ut).call(this);
-                                A += ae, O += Q;
+                                const [ae, Z] = K(this, M, Ut).call(this);
+                                A += ae, O += Z;
                                 const {
                                     style: ce
                                 } = this.div;
                                 ce.left = `${(100 * A).toFixed(2)}%`, ce.top = `${(100 * O).toFixed(2)}%`, this.moveInDOM();
                             }
                             screenToPageTranslation(f, v) {
                                 var A;
@@ -10795,44 +10795,44 @@
                             _setParentAndPosition(f, v, A) {
                                 f.changeParent(this), this.x = v, this.y = A, this.fixAndSetPosition();
                             }
                             getRect(f, v) {
                                 const A = this.parentScale,
                                     [O, H] = this.pageDimensions,
                                     [z, ae] = this.pageTranslation,
-                                    Q = f / A,
+                                    Z = f / A,
                                     ce = v / A,
                                     ue = this.x * O,
                                     me = this.y * H,
                                     fe = this.width * O,
                                     Pe = this.height * H;
                                 switch (this.rotation) {
                                     case 0:
-                                        return [ue + Q + z, H - me - ce - Pe + ae, ue + Q + fe + z, H - me - ce + ae];
+                                        return [ue + Z + z, H - me - ce - Pe + ae, ue + Z + fe + z, H - me - ce + ae];
                                     case 90:
-                                        return [ue + ce + z, H - me + Q + ae, ue + ce + Pe + z, H - me + Q + fe + ae];
+                                        return [ue + ce + z, H - me + Z + ae, ue + ce + Pe + z, H - me + Z + fe + ae];
                                     case 180:
-                                        return [ue - Q - fe + z, H - me + ce + ae, ue - Q + z, H - me + ce + Pe + ae];
+                                        return [ue - Z - fe + z, H - me + ce + ae, ue - Z + z, H - me + ce + Pe + ae];
                                     case 270:
-                                        return [ue - ce - Pe + z, H - me - Q - fe + ae, ue - ce + z, H - me - Q + ae];
+                                        return [ue - ce - Pe + z, H - me - Z - fe + ae, ue - ce + z, H - me - Z + ae];
                                     default:
                                         throw new Error("Invalid rotation");
                                 }
                             }
                             getRectInCurrentCoords(f, v) {
-                                const [A, O, H, z] = f, ae = H - A, Q = z - O;
+                                const [A, O, H, z] = f, ae = H - A, Z = z - O;
                                 switch (this.rotation) {
                                     case 0:
-                                        return [A, v - z, ae, Q];
+                                        return [A, v - z, ae, Z];
                                     case 90:
-                                        return [A, v - O, Q, ae];
+                                        return [A, v - O, Z, ae];
                                     case 180:
-                                        return [H, v - O, ae, Q];
+                                        return [H, v - O, ae, Z];
                                     case 270:
-                                        return [H, v - z, Q, ae];
+                                        return [H, v - z, Z, ae];
                                     default:
                                         throw new Error("Invalid rotation");
                                 }
                             }
                             onceAdded() {}
                             isEmpty() {
                                 return !1;
@@ -10862,16 +10862,16 @@
                             static deserialize(f, v, A) {
                                 const O = new this.prototype.constructor({
                                     parent: v,
                                     id: v.getNextId(),
                                     uiManager: A
                                 });
                                 O.rotation = f.rotation;
-                                const [H, z] = O.pageDimensions, [ae, Q, ce, ue] = O.getRectInCurrentCoords(f.rect, z);
-                                return O.x = ae / H, O.y = Q / z, O.width = ce / H, O.height = ue / z, O;
+                                const [H, z] = O.pageDimensions, [ae, Z, ce, ue] = O.getRectInCurrentCoords(f.rect, z);
+                                return O.x = ae / H, O.y = Z / z, O.width = ce / H, O.height = ue / z, O;
                             }
                             remove() {
                                 var f;
                                 this.div.removeEventListener("focusin", a(this, P)), this.div.removeEventListener("focusout", a(this, b)), this.isEmpty() || this.commit(), this.parent ? this.parent.remove(this) : this._uiManager.removeEditor(this), (f = a(this, r)) == null || f.remove(), oe(this, r, null), oe(this, T, null);
                             }
                             get isResizable() {
                                 return !1;
@@ -10981,43 +10981,43 @@
                             this._isDraggable = !1;
                             const z = {
                                 passive: !0,
                                 capture: !0
                             };
                             window.addEventListener("pointermove", O, z);
                             const ae = this.x,
-                                Q = this.y,
+                                Z = this.y,
                                 ce = this.width,
                                 ue = this.height,
                                 me = this.parent.div.style.cursor,
                                 fe = this.div.style.cursor;
                             this.div.style.cursor = this.parent.div.style.cursor = window.getComputedStyle(v.target).cursor;
                             const Pe = () => {
                                 this._isDraggable = H, window.removeEventListener("pointerup", Pe), window.removeEventListener("blur", Pe), window.removeEventListener("pointermove", O, z), this.parent.div.style.cursor = me, this.div.style.cursor = fe;
                                 const Fe = this.x,
                                     Ee = this.y,
                                     De = this.width,
                                     _e = this.height;
-                                Fe === ae && Ee === Q && De === ce && _e === ue || this.addCommands({
+                                Fe === ae && Ee === Z && De === ce && _e === ue || this.addCommands({
                                     cmd: () => {
                                         this.width = De, this.height = _e, this.x = Fe, this.y = Ee;
                                         const [ie, se] = this.parentDimensions;
                                         this.setDims(ie * De, se * _e), this.fixAndSetPosition();
                                     },
                                     undo: () => {
-                                        this.width = ce, this.height = ue, this.x = ae, this.y = Q;
+                                        this.width = ce, this.height = ue, this.x = ae, this.y = Z;
                                         const [ie, se] = this.parentDimensions;
                                         this.setDims(ie * ce, se * ue), this.fixAndSetPosition();
                                     },
                                     mustExec: !0
                                 });
                             };
                             window.addEventListener("pointerup", Pe), window.addEventListener("blur", Pe);
                         }, q = new WeakSet(), Tn = function(f, v) {
-                            const [A, O] = this.parentDimensions, H = this.x, z = this.y, ae = this.width, Q = this.height, ce = d.MIN_SIZE / A, ue = d.MIN_SIZE / O, me = (ve) => Math.round(ve * 1e4) / 1e4, fe = K(this, X, Gt).call(this, this.rotation), Pe = (ve, Se) => [fe[0] * ve + fe[2] * Se, fe[1] * ve + fe[3] * Se], Fe = K(this, X, Gt).call(this, 360 - this.rotation), Ee = (ve, Se) => [Fe[0] * ve + Fe[2] * Se, Fe[1] * ve + Fe[3] * Se];
+                            const [A, O] = this.parentDimensions, H = this.x, z = this.y, ae = this.width, Z = this.height, ce = d.MIN_SIZE / A, ue = d.MIN_SIZE / O, me = (ve) => Math.round(ve * 1e4) / 1e4, fe = K(this, X, Gt).call(this, this.rotation), Pe = (ve, Se) => [fe[0] * ve + fe[2] * Se, fe[1] * ve + fe[3] * Se], Fe = K(this, X, Gt).call(this, 360 - this.rotation), Ee = (ve, Se) => [Fe[0] * ve + Fe[2] * Se, Fe[1] * ve + Fe[3] * Se];
                             let De, _e, ie = !1,
                                 se = !1;
                             switch (f) {
                                 case "topLeft":
                                     ie = !0, De = (ve, Se) => [0, 0], _e = (ve, Se) => [ve, Se];
                                     break;
                                 case "topMiddle":
@@ -11038,31 +11038,31 @@
                                 case "bottomLeft":
                                     ie = !0, De = (ve, Se) => [0, Se], _e = (ve, Se) => [ve, 0];
                                     break;
                                 case "middleLeft":
                                     se = !0, De = (ve, Se) => [0, Se / 2], _e = (ve, Se) => [ve, Se / 2];
                                     break;
                             }
-                            const ge = De(ae, Q),
-                                Ce = _e(ae, Q);
+                            const ge = De(ae, Z),
+                                Ce = _e(ae, Z);
                             let xe = Pe(...Ce);
-                            const Ue = me(H + xe[0]),
+                            const He = me(H + xe[0]),
                                 We = me(z + xe[1]);
                             let je = 1,
                                 ze = 1,
                                 [Xe, Ge] = this.screenToPageTranslation(v.movementX, v.movementY);
                             if ([Xe, Ge] = Ee(Xe / A, Ge / O), ie) {
-                                const ve = Math.hypot(ae, Q);
-                                je = ze = Math.max(Math.min(Math.hypot(Ce[0] - ge[0] - Xe, Ce[1] - ge[1] - Ge) / ve, 1 / ae, 1 / Q), ce / ae, ue / Q);
+                                const ve = Math.hypot(ae, Z);
+                                je = ze = Math.max(Math.min(Math.hypot(Ce[0] - ge[0] - Xe, Ce[1] - ge[1] - Ge) / ve, 1 / ae, 1 / Z), ce / ae, ue / Z);
                             } else
-                                se ? je = Math.max(ce, Math.min(1, Math.abs(Ce[0] - ge[0] - Xe))) / ae : ze = Math.max(ue, Math.min(1, Math.abs(Ce[1] - ge[1] - Ge))) / Q;
+                                se ? je = Math.max(ce, Math.min(1, Math.abs(Ce[0] - ge[0] - Xe))) / ae : ze = Math.max(ue, Math.min(1, Math.abs(Ce[1] - ge[1] - Ge))) / Z;
                             const Ye = me(ae * je),
-                                de = me(Q * ze);
+                                de = me(Z * ze);
                             xe = Pe(..._e(Ye, de));
-                            const ne = Ue - xe[0],
+                            const ne = He - xe[0],
                                 J = We - xe[1];
                             this.width = Ye, this.height = de, this.x = ne, this.y = J, this.setDims(A * Ye, O * de), this.fixAndSetPosition();
                         }, pe = new WeakSet(), Wt = async function() {
                             var A;
                             const f = a(this, r);
                             if (!f)
                                 return;
@@ -11104,16 +11104,16 @@
                             const v = this._uiManager.isSelected(this);
                             this._uiManager.setUpDragSession();
                             let A, O;
                             v && (A = {
                                 passive: !0,
                                 capture: !0
                             }, O = (z) => {
-                                const [ae, Q] = this.screenToPageTranslation(z.movementX, z.movementY);
-                                this._uiManager.dragSelectedEditors(ae, Q);
+                                const [ae, Z] = this.screenToPageTranslation(z.movementX, z.movementY);
+                                this._uiManager.dragSelectedEditors(ae, Z);
                             }, window.addEventListener("pointermove", O, A));
                             const H = () => {
                                 if (window.removeEventListener("pointerup", H), window.removeEventListener("blur", H), v && window.removeEventListener("pointermove", O, A), oe(this, k, !1), !this._uiManager.endDragSession()) {
                                     const {
                                         isMac: z
                                     } = s.FeatureTest.platform;
                                     f.ctrlKey && !z || f.shiftKey || f.metaKey && z ? this.parent.toggleSelected(this) : this.parent.setSelected(this);
@@ -11135,15 +11135,15 @@
                                 };
                             }
                         }
                     },
                     /* 5 */
                     /***/
                     (t, e, i) => {
-                        var w, C, P, b, k, qt, y, p, E, $, M, Pn, D, X, G, I, B, ee, Y, q, le, pe, we, be, R, d, g, f, v, A, O, H, z, ae, Q, ce, ue, me, fe, Pe, Fe, Ee, De, _e, ie, se, ge, xn, xe, zt, We, Xt, ze, Ct, Ge, Vt, de, Yt, J, at, Se, mt, et, kn, Te, Rn, ke, Kt, Be, bt, Ae, Jt;
+                        var w, C, P, b, k, qt, y, p, E, $, M, Pn, D, X, G, I, B, ee, Y, q, le, pe, we, be, R, d, g, f, v, A, O, H, z, ae, Z, ce, ue, me, fe, Pe, Fe, Ee, De, _e, ie, se, ge, xn, xe, zt, We, Xt, ze, Ct, Ge, Vt, de, Yt, J, at, Se, mt, et, kn, Te, Rn, ke, Kt, Be, bt, Ae, Jt;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.KeyboardManager = e.CommandManager = e.ColorManager = e.AnnotationEditorUIManager = void 0, e.bindEvents = l, e.opacityToHex = h;
                         var n = i(1),
                             s = i(6);
 
                         function l(U, u, L) {
@@ -11171,25 +11171,25 @@
                                 W(this, b, null);
                             }
                             static get _isSVGFittingCanvas() {
                                 const u = 'data:image/svg+xml;charset=UTF-8,<svg viewBox="0 0 1 1" width="1" height="1" xmlns="http://www.w3.org/2000/svg"><rect width="1" height="1" style="fill:red;"/></svg>',
                                     j = new OffscreenCanvas(1, 3).getContext("2d"),
                                     V = new Image();
                                 V.src = u;
-                                const Z = V.decode().then(() => (j.drawImage(V, 0, 0, 1, 1, 0, 0, 1, 3), new Uint32Array(j.getImageData(0, 0, 1, 1).data.buffer)[0] === 0));
-                                return (0, n.shadow)(this, "_isSVGFittingCanvas", Z);
+                                const Q = V.decode().then(() => (j.drawImage(V, 0, 0, 1, 1, 0, 0, 1, 3), new Uint32Array(j.getImageData(0, 0, 1, 1).data.buffer)[0] === 0));
+                                return (0, n.shadow)(this, "_isSVGFittingCanvas", Q);
                             }
                             async getFromFile(u) {
                                 const {
                                     lastModified: L,
                                     name: j,
                                     size: V,
-                                    type: Z
+                                    type: Q
                                 } = u;
-                                return K(this, k, qt).call(this, `${L}_${j}_${V}_${Z}`, u);
+                                return K(this, k, qt).call(this, `${L}_${j}_${V}_${Q}`, u);
                             }
                             async getFromUrl(u) {
                                 return K(this, k, qt).call(this, u, u);
                             }
                             async getFromId(u) {
                                 a(this, b) || oe(this, b, /* @__PURE__ */ new Map());
                                 const L = a(this, b).get(u);
@@ -11221,30 +11221,30 @@
                                     id: `image_${a(this, C)}_${_t(this, P)._++}`,
                                     refCounter: 0,
                                     isSvg: !1
                                 });
                                 let V;
                                 if (typeof L == "string") {
                                     j.url = L;
-                                    const Z = await fetch(L);
-                                    if (!Z.ok)
-                                        throw new Error(Z.statusText);
-                                    V = await Z.blob();
+                                    const Q = await fetch(L);
+                                    if (!Q.ok)
+                                        throw new Error(Q.statusText);
+                                    V = await Q.blob();
                                 } else
                                     V = j.file = L;
                                 if (V.type === "image/svg+xml") {
-                                    const Z = x._isSVGFittingCanvas,
+                                    const Q = x._isSVGFittingCanvas,
                                         he = new FileReader(),
                                         ye = new Image(),
                                         Me = new Promise((Re, qe) => {
                                             ye.onload = () => {
                                                 j.bitmap = ye, j.isSvg = !0, Re();
                                             }, he.onload = async () => {
                                                 const Ie = j.svgUrl = he.result;
-                                                ye.src = await Z ? `${Ie}#svgView(preserveAspectRatio(none))` : Ie;
+                                                ye.src = await Q ? `${Ie}#svgView(preserveAspectRatio(none))` : Ie;
                                             }, ye.onerror = he.onerror = qe;
                                         });
                                     he.readAsDataURL(V), await Me;
                                 } else
                                     j.bitmap = await createImageBitmap(V);
                                 j.refCounter = 1;
                             } catch (V) {
@@ -11262,29 +11262,29 @@
                                 oe(this, E, u);
                             }
                             add({
                                 cmd: u,
                                 undo: L,
                                 mustExec: j,
                                 type: V = NaN,
-                                overwriteIfSameType: Z = !1,
+                                overwriteIfSameType: Q = !1,
                                 keepUndo: he = !1
                             }) {
                                 if (j && u(), a(this, p))
                                     return;
                                 const ye = {
                                     cmd: u,
                                     undo: L,
                                     type: V
                                 };
                                 if (a(this, $) === -1) {
                                     a(this, y).length > 0 && (a(this, y).length = 0), oe(this, $, 0), a(this, y).push(ye);
                                     return;
                                 }
-                                if (Z && a(this, y)[a(this, $)].type === V) {
+                                if (Q && a(this, y)[a(this, $)].type === V) {
                                     he && (ye.undo = a(this, y)[a(this, $)].undo), a(this, y)[a(this, $)] = ye;
                                     return;
                                 }
                                 const Me = a(this, $) + 1;
                                 Me === a(this, E) ? a(this, y).splice(0, 1) : (oe(this, $, Me), Me < a(this, y).length && a(this, y).splice(Me)), a(this, y).push(ye);
                             }
                             undo() {
@@ -11307,41 +11307,41 @@
                         class r {
                             constructor(u) {
                                 W(this, M);
                                 this.buffer = [], this.callbacks = /* @__PURE__ */ new Map(), this.allKeys = /* @__PURE__ */ new Set();
                                 const {
                                     isMac: L
                                 } = n.FeatureTest.platform;
-                                for (const [j, V, Z = {}] of u)
+                                for (const [j, V, Q = {}] of u)
                                     for (const he of j) {
                                         const ye = he.startsWith("mac+");
                                         L && ye ? (this.callbacks.set(he.slice(4), {
                                             callback: V,
-                                            options: Z
+                                            options: Q
                                         }), this.allKeys.add(he.split("+").at(-1))) : !L && !ye && (this.callbacks.set(he, {
                                             callback: V,
-                                            options: Z
+                                            options: Q
                                         }), this.allKeys.add(he.split("+").at(-1)));
                                     }
                             }
                             exec(u, L) {
                                 if (!this.allKeys.has(L.key))
                                     return;
                                 const j = this.callbacks.get(K(this, M, Pn).call(this, L));
                                 if (!j)
                                     return;
                                 const {
                                     callback: V,
                                     options: {
-                                        bubbles: Z = !1,
+                                        bubbles: Q = !1,
                                         args: he = [],
                                         checker: ye = null
                                     }
                                 } = j;
-                                ye && !ye(u, L) || (V.bind(u, ...he)(), Z || (L.stopPropagation(), L.preventDefault()));
+                                ye && !ye(u, L) || (V.bind(u, ...he)(), Q || (L.stopPropagation(), L.preventDefault()));
                             }
                         }
                         M = new WeakSet(), Pn = function(u) {
                             u.altKey && this.buffer.push("alt"), u.ctrlKey && this.buffer.push("ctrl"), u.metaKey && this.buffer.push("meta"), u.shiftKey && this.buffer.push("shift"), this.buffer.push(u.key);
                             const L = this.buffer.join("+");
                             return this.buffer.length = 0, L;
                         }, e.KeyboardManager = r;
@@ -11354,15 +11354,15 @@
                                 return (0, s.getColorValues)(u), (0, n.shadow)(this, "_colors", u);
                             }
                             convert(u) {
                                 const L = (0, s.getRGB)(u);
                                 if (!window.matchMedia("(forced-colors: active)").matches)
                                     return L;
                                 for (const [j, V] of this._colors)
-                                    if (V.every((Z, he) => Z === L[he]))
+                                    if (V.every((Q, he) => Q === L[he]))
                                         return N._colorsMapping.get(j);
                                 return L;
                             }
                             getHexCode(u) {
                                 const L = this._colors.get(u);
                                 return L ? n.Util.makeHexColor(...L) : u;
                             }
@@ -11370,15 +11370,15 @@
                         nt(N, "_colorsMapping", /* @__PURE__ */ new Map([
                             ["CanvasText", [0, 0, 0]],
                             ["Canvas", [255, 255, 255]]
                         ]));
                         let T = N;
                         e.ColorManager = T;
                         const Oe = class Oe {
-                            constructor(u, L, j, V, Z, he) {
+                            constructor(u, L, j, V, Q, he) {
                                 W(this, ge);
                                 W(this, xe);
                                 W(this, We);
                                 W(this, ze);
                                 W(this, Ge);
                                 W(this, de);
                                 W(this, J);
@@ -11406,15 +11406,15 @@
                                 W(this, f, null);
                                 W(this, v, n.AnnotationEditorType.NONE);
                                 W(this, A, /* @__PURE__ */ new Set());
                                 W(this, O, null);
                                 W(this, H, this.blur.bind(this));
                                 W(this, z, this.focus.bind(this));
                                 W(this, ae, this.copy.bind(this));
-                                W(this, Q, this.cut.bind(this));
+                                W(this, Z, this.cut.bind(this));
                                 W(this, ce, this.paste.bind(this));
                                 W(this, ue, this.keydown.bind(this));
                                 W(this, me, this.onEditingAction.bind(this));
                                 W(this, fe, this.onPageChanging.bind(this));
                                 W(this, Pe, this.onScaleChanging.bind(this));
                                 W(this, Fe, this.onRotationChanging.bind(this));
                                 W(this, Ee, {
@@ -11424,26 +11424,26 @@
                                     hasSomethingToRedo: !1,
                                     hasSelectedEditor: !1
                                 });
                                 W(this, De, [0, 0]);
                                 W(this, _e, null);
                                 W(this, ie, null);
                                 W(this, se, null);
-                                oe(this, ie, u), oe(this, se, L), oe(this, I, j), this._eventBus = V, this._eventBus._on("editingaction", a(this, me)), this._eventBus._on("pagechanging", a(this, fe)), this._eventBus._on("scalechanging", a(this, Pe)), this._eventBus._on("rotationchanging", a(this, Fe)), oe(this, B, Z.annotationStorage), oe(this, be, Z.filterFactory), oe(this, O, he), this.viewParameters = {
+                                oe(this, ie, u), oe(this, se, L), oe(this, I, j), this._eventBus = V, this._eventBus._on("editingaction", a(this, me)), this._eventBus._on("pagechanging", a(this, fe)), this._eventBus._on("scalechanging", a(this, Pe)), this._eventBus._on("rotationchanging", a(this, Fe)), oe(this, B, Q.annotationStorage), oe(this, be, Q.filterFactory), oe(this, O, he), this.viewParameters = {
                                     realScale: s.PixelsPerInch.PDF_TO_CSS_UNITS,
                                     rotation: 0
                                 };
                             }
                             static get _keyboardManager() {
                                 const u = Oe.prototype,
-                                    L = (Z) => {
+                                    L = (Q) => {
                                         const {
                                             activeElement: he
                                         } = document;
-                                        return he && a(Z, ie).contains(he) && Z.hasSomethingToControl();
+                                        return he && a(Q, ie).contains(he) && Q.hasSomethingToControl();
                                     },
                                     j = this.TRANSLATE_SMALL,
                                     V = this.TRANSLATE_BIG;
                                 return (0, n.shadow)(this, "_keyboardManager", new r([
                                     [
                                         ["ctrl+a", "mac+meta+a"], u.selectAll
                                     ],
@@ -11533,19 +11533,19 @@
                             focusMainContainer() {
                                 a(this, ie).focus();
                             }
                             findParent(u, L) {
                                 for (const j of a(this, G).values()) {
                                     const {
                                         x: V,
-                                        y: Z,
+                                        y: Q,
                                         width: he,
                                         height: ye
                                     } = j.div.getBoundingClientRect();
-                                    if (u >= V && u <= V + he && L >= Z && L <= Z + ye)
+                                    if (u >= V && u <= V + he && L >= Q && L <= Q + ye)
                                         return j;
                                 }
                                 return null;
                             }
                             disableUserSelect(u = !1) {
                                 a(this, se).classList.toggle("noUserSelect", u);
                             }
@@ -11600,70 +11600,70 @@
                             }
                             copy(u) {
                                 var j;
                                 if (u.preventDefault(), (j = a(this, D)) == null || j.commitOrRemove(), !this.hasSelection)
                                     return;
                                 const L = [];
                                 for (const V of a(this, A)) {
-                                    const Z = V.serialize(!0);
-                                    Z && L.push(Z);
+                                    const Q = V.serialize(!0);
+                                    Q && L.push(Q);
                                 }
                                 L.length !== 0 && u.clipboardData.setData("application/pdfjs", JSON.stringify(L));
                             }
                             cut(u) {
                                 this.copy(u), this.delete();
                             }
                             paste(u) {
                                 u.preventDefault();
                                 const {
                                     clipboardData: L
                                 } = u;
-                                for (const Z of L.items)
+                                for (const Q of L.items)
                                     for (const he of a(this, pe))
-                                        if (he.isHandlingMimeForPasting(Z.type)) {
-                                            he.paste(Z, this.currentLayer);
+                                        if (he.isHandlingMimeForPasting(Q.type)) {
+                                            he.paste(Q, this.currentLayer);
                                             return;
                                         }
                                 let j = L.getData("application/pdfjs");
                                 if (!j)
                                     return;
                                 try {
                                     j = JSON.parse(j);
-                                } catch (Z) {
-                                    (0, n.warn)(`paste: "${Z.message}".`);
+                                } catch (Q) {
+                                    (0, n.warn)(`paste: "${Q.message}".`);
                                     return;
                                 }
                                 if (!Array.isArray(j))
                                     return;
                                 this.unselectAll();
                                 const V = this.currentLayer;
                                 try {
-                                    const Z = [];
+                                    const Q = [];
                                     for (const Me of j) {
                                         const Re = V.deserialize(Me);
                                         if (!Re)
                                             return;
-                                        Z.push(Re);
+                                        Q.push(Re);
                                     }
                                     const he = () => {
-                                            for (const Me of Z)
+                                            for (const Me of Q)
                                                 K(this, ke, Kt).call(this, Me);
-                                            K(this, Ae, Jt).call(this, Z);
+                                            K(this, Ae, Jt).call(this, Q);
                                         },
                                         ye = () => {
-                                            for (const Me of Z)
+                                            for (const Me of Q)
                                                 Me.remove();
                                         };
                                     this.addCommands({
                                         cmd: he,
                                         undo: ye,
                                         mustExec: !0
                                     });
-                                } catch (Z) {
-                                    (0, n.warn)(`paste: "${Z.message}".`);
+                                } catch (Q) {
+                                    (0, n.warn)(`paste: "${Q.message}".`);
                                 }
                             }
                             keydown(u) {
                                 var L;
                                 (L = this.getActive()) != null && L.shouldGetKeyboardEvents() || Oe._keyboardManager.exec(this, u);
                             }
                             onEditingAction(u) {
@@ -11869,24 +11869,24 @@
                                     });
                                 }
                             }
                             translateSelectedEditors(u, L, j = !1) {
                                 if (j || this.commitOrRemove(), !this.hasSelection)
                                     return;
                                 a(this, De)[0] += u, a(this, De)[1] += L;
-                                const [V, Z] = a(this, De), he = [...a(this, A)], ye = 1e3;
+                                const [V, Q] = a(this, De), he = [...a(this, A)], ye = 1e3;
                                 a(this, _e) && clearTimeout(a(this, _e)), oe(this, _e, setTimeout(() => {
                                     oe(this, _e, null), a(this, De)[0] = a(this, De)[1] = 0, this.addCommands({
                                         cmd: () => {
                                             for (const Me of he)
-                                                a(this, X).has(Me.id) && Me.translateInPage(V, Z);
+                                                a(this, X).has(Me.id) && Me.translateInPage(V, Q);
                                         },
                                         undo: () => {
                                             for (const Me of he)
-                                                a(this, X).has(Me.id) && Me.translateInPage(-V, -Z);
+                                                a(this, X).has(Me.id) && Me.translateInPage(-V, -Q);
                                         },
                                         mustExec: !1
                                     });
                                 }, ye));
                                 for (const Me of he)
                                     Me.translateInPage(u, L);
                             }
@@ -11909,42 +11909,42 @@
                                     return !1;
                                 this.disableUserSelect(!1);
                                 const u = a(this, le);
                                 oe(this, le, null);
                                 let L = !1;
                                 for (const [{
                                         x: V,
-                                        y: Z,
+                                        y: Q,
                                         pageIndex: he
                                     }, ye] of u)
-                                    ye.newX = V, ye.newY = Z, ye.newPageIndex = he, L || (L = V !== ye.savedX || Z !== ye.savedY || he !== ye.savedPageIndex);
+                                    ye.newX = V, ye.newY = Q, ye.newPageIndex = he, L || (L = V !== ye.savedX || Q !== ye.savedY || he !== ye.savedPageIndex);
                                 if (!L)
                                     return !1;
-                                const j = (V, Z, he, ye) => {
+                                const j = (V, Q, he, ye) => {
                                     if (a(this, X).has(V.id)) {
                                         const Me = a(this, G).get(ye);
-                                        Me ? V._setParentAndPosition(Me, Z, he) : (V.pageIndex = ye, V.x = Z, V.y = he);
+                                        Me ? V._setParentAndPosition(Me, Q, he) : (V.pageIndex = ye, V.x = Q, V.y = he);
                                     }
                                 };
                                 return this.addCommands({
                                     cmd: () => {
                                         for (const [V, {
-                                                newX: Z,
+                                                newX: Q,
                                                 newY: he,
                                                 newPageIndex: ye
                                             }] of u)
-                                            j(V, Z, he, ye);
+                                            j(V, Q, he, ye);
                                     },
                                     undo: () => {
                                         for (const [V, {
-                                                savedX: Z,
+                                                savedX: Q,
                                                 savedY: he,
                                                 savedPageIndex: ye
                                             }] of u)
-                                            j(V, Z, he, ye);
+                                            j(V, Q, he, ye);
                                     },
                                     mustExec: !0
                                 }), !0;
                             }
                             dragSelectedEditors(u, L) {
                                 if (a(this, le))
                                     for (const j of a(this, le).keys())
@@ -11966,30 +11966,30 @@
                             getMode() {
                                 return a(this, v);
                             }
                             get imageManager() {
                                 return (0, n.shadow)(this, "imageManager", new c());
                             }
                         };
-                        D = new WeakMap(), X = new WeakMap(), G = new WeakMap(), I = new WeakMap(), B = new WeakMap(), ee = new WeakMap(), Y = new WeakMap(), q = new WeakMap(), le = new WeakMap(), pe = new WeakMap(), we = new WeakMap(), be = new WeakMap(), R = new WeakMap(), d = new WeakMap(), g = new WeakMap(), f = new WeakMap(), v = new WeakMap(), A = new WeakMap(), O = new WeakMap(), H = new WeakMap(), z = new WeakMap(), ae = new WeakMap(), Q = new WeakMap(), ce = new WeakMap(), ue = new WeakMap(), me = new WeakMap(), fe = new WeakMap(), Pe = new WeakMap(), Fe = new WeakMap(), Ee = new WeakMap(), De = new WeakMap(), _e = new WeakMap(), ie = new WeakMap(), se = new WeakMap(), ge = new WeakSet(), xn = function() {
+                        D = new WeakMap(), X = new WeakMap(), G = new WeakMap(), I = new WeakMap(), B = new WeakMap(), ee = new WeakMap(), Y = new WeakMap(), q = new WeakMap(), le = new WeakMap(), pe = new WeakMap(), we = new WeakMap(), be = new WeakMap(), R = new WeakMap(), d = new WeakMap(), g = new WeakMap(), f = new WeakMap(), v = new WeakMap(), A = new WeakMap(), O = new WeakMap(), H = new WeakMap(), z = new WeakMap(), ae = new WeakMap(), Z = new WeakMap(), ce = new WeakMap(), ue = new WeakMap(), me = new WeakMap(), fe = new WeakMap(), Pe = new WeakMap(), Fe = new WeakMap(), Ee = new WeakMap(), De = new WeakMap(), _e = new WeakMap(), ie = new WeakMap(), se = new WeakMap(), ge = new WeakSet(), xn = function() {
                             window.addEventListener("focus", a(this, z)), window.addEventListener("blur", a(this, H));
                         }, xe = new WeakSet(), zt = function() {
                             window.removeEventListener("focus", a(this, z)), window.removeEventListener("blur", a(this, H));
                         }, We = new WeakSet(), Xt = function() {
                             window.addEventListener("keydown", a(this, ue), {
                                 capture: !0
                             });
                         }, ze = new WeakSet(), Ct = function() {
                             window.removeEventListener("keydown", a(this, ue), {
                                 capture: !0
                             });
                         }, Ge = new WeakSet(), Vt = function() {
-                            document.addEventListener("copy", a(this, ae)), document.addEventListener("cut", a(this, Q)), document.addEventListener("paste", a(this, ce));
+                            document.addEventListener("copy", a(this, ae)), document.addEventListener("cut", a(this, Z)), document.addEventListener("paste", a(this, ce));
                         }, de = new WeakSet(), Yt = function() {
-                            document.removeEventListener("copy", a(this, ae)), document.removeEventListener("cut", a(this, Q)), document.removeEventListener("paste", a(this, ce));
+                            document.removeEventListener("copy", a(this, ae)), document.removeEventListener("cut", a(this, Z)), document.removeEventListener("paste", a(this, ce));
                         }, J = new WeakSet(), at = function(u) {
                             Object.entries(u).some(([j, V]) => a(this, Ee)[j] !== V) && this._eventBus.dispatch("annotationeditorstateschanged", {
                                 source: this,
                                 details: Object.assign(a(this, Ee), u)
                             });
                         }, Se = new WeakSet(), mt = function(u) {
                             this._eventBus.dispatch("annotationeditorparamschanged", {
@@ -12028,15 +12028,15 @@
                         }, nt(Oe, "TRANSLATE_SMALL", 1), nt(Oe, "TRANSLATE_BIG", 10);
                         let S = Oe;
                         e.AnnotationEditorUIManager = S;
                     },
                     /* 6 */
                     /***/
                     (t, e, i) => {
-                        var Y, q, le, pe, we, be, R, d, g, f, v, A, dt, H, ft, ae, Qt, ce, Pt, me, xt, Pe, yt, Ee, vt;
+                        var Y, q, le, pe, we, be, R, d, g, f, v, A, dt, H, ft, ae, Zt, ce, Pt, me, xt, Pe, yt, Ee, vt;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.StatTimer = e.RenderingCancelledException = e.PixelsPerInch = e.PageViewport = e.PDFDateString = e.DOMStandardFontDataFactory = e.DOMSVGFactory = e.DOMFilterFactory = e.DOMCanvasFactory = e.DOMCMapReaderFactory = void 0, e.deprecated = $, e.getColorValues = X, e.getCurrentTransform = G, e.getCurrentTransformInverse = I, e.getFilenameFromUrl = k, e.getPdfFilenameFromUrl = F, e.getRGB = D, e.getXfaPageViewport = N, e.isDataScheme = P, e.isPdfFile = b, e.isValidFetchUrl = y, e.loadScript = E, e.noContextMenu = p, e.setLayerDimensions = B;
                         var n = i(7),
                             s = i(1);
                         const l = "http://www.w3.org/2000/svg",
                             ee = class ee {};
@@ -12071,98 +12071,98 @@
                             }
                             addFilter(se) {
                                 if (!se)
                                     return "none";
                                 let ge = a(this, A, dt).get(se);
                                 if (ge)
                                     return ge;
-                                let Ce, xe, Ue, We;
+                                let Ce, xe, He, We;
                                 if (se.length === 1) {
                                     const Ge = se[0],
                                         Ye = new Array(256);
                                     for (let de = 0; de < 256; de++)
                                         Ye[de] = Ge[de] / 255;
-                                    We = Ce = xe = Ue = Ye.join(",");
+                                    We = Ce = xe = He = Ye.join(",");
                                 } else {
                                     const [Ge, Ye, de] = se, ne = new Array(256), J = new Array(256), ve = new Array(256);
                                     for (let Se = 0; Se < 256; Se++)
                                         ne[Se] = Ge[Se] / 255, J[Se] = Ye[Se] / 255, ve[Se] = de[Se] / 255;
-                                    Ce = ne.join(","), xe = J.join(","), Ue = ve.join(","), We = `${Ce}${xe}${Ue}`;
+                                    Ce = ne.join(","), xe = J.join(","), He = ve.join(","), We = `${Ce}${xe}${He}`;
                                 }
                                 if (ge = a(this, A, dt).get(We), ge)
                                     return a(this, A, dt).set(se, ge), ge;
                                 const je = `g_${a(this, le)}_transfer_map_${_t(this, v)._++}`,
                                     ze = `url(#${je})`;
                                 a(this, A, dt).set(se, ze), a(this, A, dt).set(We, ze);
                                 const Xe = K(this, ce, Pt).call(this, je);
-                                return K(this, Pe, yt).call(this, Ce, xe, Ue, Xe), ze;
+                                return K(this, Pe, yt).call(this, Ce, xe, He, Xe), ze;
                             }
                             addHCMFilter(se, ge) {
                                 var Ye;
                                 const Ce = `${se}-${ge}`;
                                 if (a(this, be) === Ce)
                                     return a(this, R);
                                 if (oe(this, be, Ce), oe(this, R, "none"), (Ye = a(this, we)) == null || Ye.remove(), !se || !ge)
                                     return a(this, R);
                                 const xe = K(this, Ee, vt).call(this, se);
                                 se = s.Util.makeHexColor(...xe);
-                                const Ue = K(this, Ee, vt).call(this, ge);
-                                if (ge = s.Util.makeHexColor(...Ue), a(this, H, ft).style.color = "", se === "#000000" && ge === "#ffffff" || se === ge)
+                                const He = K(this, Ee, vt).call(this, ge);
+                                if (ge = s.Util.makeHexColor(...He), a(this, H, ft).style.color = "", se === "#000000" && ge === "#ffffff" || se === ge)
                                     return a(this, R);
                                 const We = new Array(256);
                                 for (let de = 0; de <= 255; de++) {
                                     const ne = de / 255;
                                     We[de] = ne <= 0.03928 ? ne / 12.92 : ((ne + 0.055) / 1.055) ** 2.4;
                                 }
                                 const je = We.join(","),
                                     ze = `g_${a(this, le)}_hcm_filter`,
                                     Xe = oe(this, d, K(this, ce, Pt).call(this, ze));
-                                K(this, Pe, yt).call(this, je, je, je, Xe), K(this, ae, Qt).call(this, Xe);
+                                K(this, Pe, yt).call(this, je, je, je, Xe), K(this, ae, Zt).call(this, Xe);
                                 const Ge = (de, ne) => {
                                     const J = xe[de] / 255,
-                                        ve = Ue[de] / 255,
+                                        ve = He[de] / 255,
                                         Se = new Array(ne + 1);
                                     for (let tt = 0; tt <= ne; tt++)
                                         Se[tt] = J + tt / ne * (ve - J);
                                     return Se.join(",");
                                 };
                                 return K(this, Pe, yt).call(this, Ge(0, 5), Ge(1, 5), Ge(2, 5), Xe), oe(this, R, `url(#${ze})`), a(this, R);
                             }
                             addHighlightHCMFilter(se, ge, Ce, xe) {
                                 var ve;
-                                const Ue = `${se}-${ge}-${Ce}-${xe}`;
-                                if (a(this, g) === Ue)
+                                const He = `${se}-${ge}-${Ce}-${xe}`;
+                                if (a(this, g) === He)
                                     return a(this, f);
-                                if (oe(this, g, Ue), oe(this, f, "none"), (ve = a(this, d)) == null || ve.remove(), !se || !ge)
+                                if (oe(this, g, He), oe(this, f, "none"), (ve = a(this, d)) == null || ve.remove(), !se || !ge)
                                     return a(this, f);
                                 const [We, je] = [se, ge].map(K(this, Ee, vt).bind(this));
                                 let ze = Math.round(0.2126 * We[0] + 0.7152 * We[1] + 0.0722 * We[2]),
                                     Xe = Math.round(0.2126 * je[0] + 0.7152 * je[1] + 0.0722 * je[2]),
                                     [Ge, Ye] = [Ce, xe].map(K(this, Ee, vt).bind(this));
                                 Xe < ze && ([ze, Xe, Ge, Ye] = [Xe, ze, Ye, Ge]), a(this, H, ft).style.color = "";
                                 const de = (Se, tt, et) => {
                                         const te = new Array(256),
                                             Te = (Xe - ze) / et,
                                             Ne = Se / 255,
                                             ke = (tt - Se) / (255 * et);
                                         let $e = 0;
                                         for (let Be = 0; Be <= et; Be++) {
-                                            const Qe = Math.round(ze + Be * Te),
+                                            const Ze = Math.round(ze + Be * Te),
                                                 Ae = Ne + Be * ke;
-                                            for (let Ke = $e; Ke <= Qe; Ke++)
+                                            for (let Ke = $e; Ke <= Ze; Ke++)
                                                 te[Ke] = Ae;
-                                            $e = Qe + 1;
+                                            $e = Ze + 1;
                                         }
                                         for (let Be = $e; Be < 256; Be++)
                                             te[Be] = te[$e - 1];
                                         return te.join(",");
                                     },
                                     ne = `g_${a(this, le)}_hcm_highlight_filter`,
                                     J = oe(this, d, K(this, ce, Pt).call(this, ne));
-                                return K(this, ae, Qt).call(this, J), K(this, Pe, yt).call(this, de(Ge[0], Ye[0], 5), de(Ge[1], Ye[1], 5), de(Ge[2], Ye[2], 5), J), oe(this, f, `url(#${ne})`), a(this, f);
+                                return K(this, ae, Zt).call(this, J), K(this, Pe, yt).call(this, de(Ge[0], Ye[0], 5), de(Ge[1], Ye[1], 5), de(Ge[2], Ye[2], 5), J), oe(this, f, `url(#${ne})`), a(this, f);
                             }
                             destroy(se = !1) {
                                 se && (a(this, R) || a(this, f)) || (a(this, q) && (a(this, q).parentNode.parentNode.remove(), oe(this, q, null)), a(this, Y) && (a(this, Y).clear(), oe(this, Y, null)), oe(this, v, 0));
                             }
                         }
                         Y = new WeakMap(), q = new WeakMap(), le = new WeakMap(), pe = new WeakMap(), we = new WeakMap(), be = new WeakMap(), R = new WeakMap(), d = new WeakMap(), g = new WeakMap(), f = new WeakMap(), v = new WeakMap(), A = new WeakSet(), dt = function() {
                             return a(this, Y) || oe(this, Y, /* @__PURE__ */ new Map());
@@ -12173,26 +12173,26 @@
                                         style: ge
                                     } = se;
                                 ge.visibility = "hidden", ge.contain = "strict", ge.width = ge.height = 0, ge.position = "absolute", ge.top = ge.left = 0, ge.zIndex = -1;
                                 const Ce = a(this, pe).createElementNS(l, "svg");
                                 Ce.setAttribute("width", 0), Ce.setAttribute("height", 0), oe(this, q, a(this, pe).createElementNS(l, "defs")), se.append(Ce), Ce.append(a(this, q)), a(this, pe).body.append(se);
                             }
                             return a(this, q);
-                        }, ae = new WeakSet(), Qt = function(se) {
+                        }, ae = new WeakSet(), Zt = function(se) {
                             const ge = a(this, pe).createElementNS(l, "feColorMatrix");
                             ge.setAttribute("type", "matrix"), ge.setAttribute("values", "0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0.2126 0.7152 0.0722 0 0 0 0 0 1 0"), se.append(ge);
                         }, ce = new WeakSet(), Pt = function(se) {
                             const ge = a(this, pe).createElementNS(l, "filter");
                             return ge.setAttribute("color-interpolation-filters", "sRGB"), ge.setAttribute("id", se), a(this, H, ft).append(ge), ge;
                         }, me = new WeakSet(), xt = function(se, ge, Ce) {
                             const xe = a(this, pe).createElementNS(l, ge);
                             xe.setAttribute("type", "discrete"), xe.setAttribute("tableValues", Ce), se.append(xe);
                         }, Pe = new WeakSet(), yt = function(se, ge, Ce, xe) {
-                            const Ue = a(this, pe).createElementNS(l, "feComponentTransfer");
-                            xe.append(Ue), K(this, me, xt).call(this, Ue, "feFuncR", se), K(this, me, xt).call(this, Ue, "feFuncG", ge), K(this, me, xt).call(this, Ue, "feFuncB", Ce);
+                            const He = a(this, pe).createElementNS(l, "feComponentTransfer");
+                            xe.append(He), K(this, me, xt).call(this, He, "feFuncR", se), K(this, me, xt).call(this, He, "feFuncG", ge), K(this, me, xt).call(this, He, "feFuncB", Ce);
                         }, Ee = new WeakSet(), vt = function(se) {
                             return a(this, H, ft).style.color = se, D(getComputedStyle(a(this, H, ft)).getPropertyValue("color"));
                         }, e.DOMFilterFactory = _;
                         class c extends n.BaseCanvasFactory {
                             constructor({
                                 ownerDocument: ie = globalThis.document
                             } = {}) {
@@ -12251,15 +12251,15 @@
                         class w {
                             constructor({
                                 viewBox: ie,
                                 scale: se,
                                 rotation: ge,
                                 offsetX: Ce = 0,
                                 offsetY: xe = 0,
-                                dontFlip: Ue = !1
+                                dontFlip: He = !1
                             }) {
                                 this.viewBox = ie, this.scale = se, this.rotation = ge, this.offsetX = Ce, this.offsetY = xe;
                                 const We = (ie[2] + ie[0]) / 2,
                                     je = (ie[3] + ie[1]) / 2;
                                 let ze, Xe, Ge, Ye;
                                 switch (ge %= 360, ge < 0 && (ge += 360), ge) {
                                     case 180:
@@ -12273,15 +12273,15 @@
                                         break;
                                     case 0:
                                         ze = 1, Xe = 0, Ge = 0, Ye = -1;
                                         break;
                                     default:
                                         throw new Error("PageViewport: Invalid rotation, must be a multiple of 90 degrees.");
                                 }
-                                Ue && (Ge = -Ge, Ye = -Ye);
+                                He && (Ge = -Ge, Ye = -Ye);
                                 let de, ne, J, ve;
                                 ze === 0 ? (de = Math.abs(je - ie[1]) * se + Ce, ne = Math.abs(We - ie[0]) * se + xe, J = (ie[3] - ie[1]) * se, ve = (ie[2] - ie[0]) * se) : (de = Math.abs(We - ie[0]) * se + Ce, ne = Math.abs(je - ie[1]) * se + xe, J = (ie[2] - ie[0]) * se, ve = (ie[3] - ie[1]) * se), this.transform = [ze * se, Xe * se, Ge * se, Ye * se, de - ze * se * We - Ge * se * je, ne - Xe * se * We - Ye * se * je], this.width = J, this.height = ve;
                             }
                             get rawDims() {
                                 const {
                                     viewBox: ie
                                 } = this;
@@ -12434,25 +12434,25 @@
                                 if (!se)
                                     return null;
                                 const ge = parseInt(se[1], 10);
                                 let Ce = parseInt(se[2], 10);
                                 Ce = Ce >= 1 && Ce <= 12 ? Ce - 1 : 0;
                                 let xe = parseInt(se[3], 10);
                                 xe = xe >= 1 && xe <= 31 ? xe : 1;
-                                let Ue = parseInt(se[4], 10);
-                                Ue = Ue >= 0 && Ue <= 23 ? Ue : 0;
+                                let He = parseInt(se[4], 10);
+                                He = He >= 0 && He <= 23 ? He : 0;
                                 let We = parseInt(se[5], 10);
                                 We = We >= 0 && We <= 59 ? We : 0;
                                 let je = parseInt(se[6], 10);
                                 je = je >= 0 && je <= 59 ? je : 0;
                                 const ze = se[7] || "Z";
                                 let Xe = parseInt(se[8], 10);
                                 Xe = Xe >= 0 && Xe <= 23 ? Xe : 0;
                                 let Ge = parseInt(se[9], 10) || 0;
-                                return Ge = Ge >= 0 && Ge <= 59 ? Ge : 0, ze === "-" ? (Ue += Xe, We += Ge) : ze === "+" && (Ue -= Xe, We -= Ge), new Date(Date.UTC(ge, Ce, xe, Ue, We, je));
+                                return Ge = Ge >= 0 && Ge <= 59 ? Ge : 0, ze === "-" ? (He += Xe, We += Ge) : ze === "+" && (He -= Xe, We -= Ge), new Date(Date.UTC(ge, Ce, xe, He, We, je));
                             }
                         }
                         e.PDFDateString = m;
 
                         function N(_e, {
                             scale: ie = 1,
                             rotation: se = 0
@@ -12490,40 +12490,40 @@
                         function G(_e) {
                             const {
                                 a: ie,
                                 b: se,
                                 c: ge,
                                 d: Ce,
                                 e: xe,
-                                f: Ue
+                                f: He
                             } = _e.getTransform();
-                            return [ie, se, ge, Ce, xe, Ue];
+                            return [ie, se, ge, Ce, xe, He];
                         }
 
                         function I(_e) {
                             const {
                                 a: ie,
                                 b: se,
                                 c: ge,
                                 d: Ce,
                                 e: xe,
-                                f: Ue
+                                f: He
                             } = _e.getTransform().invertSelf();
-                            return [ie, se, ge, Ce, xe, Ue];
+                            return [ie, se, ge, Ce, xe, He];
                         }
 
                         function B(_e, ie, se = !1, ge = !0) {
                             if (ie instanceof w) {
                                 const {
                                     pageWidth: Ce,
                                     pageHeight: xe
                                 } = ie.rawDims, {
-                                    style: Ue
+                                    style: He
                                 } = _e, We = s.FeatureTest.isCSSRoundSupported, je = `var(--scale-factor) * ${Ce}px`, ze = `var(--scale-factor) * ${xe}px`, Xe = We ? `round(${je}, 1px)` : `calc(${je})`, Ge = We ? `round(${ze}, 1px)` : `calc(${ze})`;
-                                !se || ie.rotation % 180 === 0 ? (Ue.width = Xe, Ue.height = Ge) : (Ue.width = Ge, Ue.height = Xe);
+                                !se || ie.rotation % 180 === 0 ? (He.width = Xe, He.height = Ge) : (He.width = Ge, He.height = Xe);
                             }
                             ge && _e.setAttribute("data-main-rotation", ie.rotation);
                         }
                     },
                     /* 7 */
                     /***/
                     (t, e, i) => {
@@ -12975,15 +12975,15 @@
                             }
                         }
                         e.NodeStandardFontDataFactory = c;
                     },
                     /* 11 */
                     /***/
                     (t, e, i) => {
-                        var q, Zt, pe, en;
+                        var q, Qt, pe, en;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.CanvasGraphics = void 0;
                         var n = i(1),
                             s = i(6),
                             l = i(12),
                             h = i(13);
@@ -13048,39 +13048,39 @@
                                     const g = this.cache[d];
                                     this.canvasFactory.destroy(g), delete this.cache[d];
                                 }
                             }
                         }
 
                         function b(R, d, g, f, v, A, O, H, z, ae) {
-                            const [Q, ce, ue, me, fe, Pe] = (0, s.getCurrentTransform)(R);
+                            const [Z, ce, ue, me, fe, Pe] = (0, s.getCurrentTransform)(R);
                             if (ce === 0 && ue === 0) {
-                                const De = O * Q + fe,
+                                const De = O * Z + fe,
                                     _e = Math.round(De),
                                     ie = H * me + Pe,
                                     se = Math.round(ie),
-                                    ge = (O + z) * Q + fe,
+                                    ge = (O + z) * Z + fe,
                                     Ce = Math.abs(Math.round(ge) - _e) || 1,
                                     xe = (H + ae) * me + Pe,
-                                    Ue = Math.abs(Math.round(xe) - se) || 1;
-                                return R.setTransform(Math.sign(Q), 0, 0, Math.sign(me), _e, se), R.drawImage(d, g, f, v, A, 0, 0, Ce, Ue), R.setTransform(Q, ce, ue, me, fe, Pe), [Ce, Ue];
+                                    He = Math.abs(Math.round(xe) - se) || 1;
+                                return R.setTransform(Math.sign(Z), 0, 0, Math.sign(me), _e, se), R.drawImage(d, g, f, v, A, 0, 0, Ce, He), R.setTransform(Z, ce, ue, me, fe, Pe), [Ce, He];
                             }
-                            if (Q === 0 && me === 0) {
+                            if (Z === 0 && me === 0) {
                                 const De = H * ue + fe,
                                     _e = Math.round(De),
                                     ie = O * ce + Pe,
                                     se = Math.round(ie),
                                     ge = (H + ae) * ue + fe,
                                     Ce = Math.abs(Math.round(ge) - _e) || 1,
                                     xe = (O + z) * ce + Pe,
-                                    Ue = Math.abs(Math.round(xe) - se) || 1;
-                                return R.setTransform(0, Math.sign(ce), Math.sign(ue), 0, _e, se), R.drawImage(d, g, f, v, A, 0, 0, Ue, Ce), R.setTransform(Q, ce, ue, me, fe, Pe), [Ue, Ce];
+                                    He = Math.abs(Math.round(xe) - se) || 1;
+                                return R.setTransform(0, Math.sign(ce), Math.sign(ue), 0, _e, se), R.drawImage(d, g, f, v, A, 0, 0, He, Ce), R.setTransform(Z, ce, ue, me, fe, Pe), [He, Ce];
                             }
                             R.drawImage(d, g, f, v, A, O, H, z, ae);
-                            const Fe = Math.hypot(Q, ce),
+                            const Fe = Math.hypot(Z, ce),
                                 Ee = Math.hypot(ue, me);
                             return [Fe * z, Ee * ae];
                         }
 
                         function k(R) {
                             const {
                                 width: d,
@@ -13089,34 +13089,34 @@
                             if (d > S || g > S)
                                 return null;
                             const f = 1e3,
                                 v = new Uint8Array([0, 2, 4, 0, 1, 0, 5, 4, 8, 10, 0, 8, 0, 2, 1, 0]),
                                 A = d + 1;
                             let O = new Uint8Array(A * (g + 1)),
                                 H, z, ae;
-                            const Q = d + 7 & -8;
-                            let ce = new Uint8Array(Q * g),
+                            const Z = d + 7 & -8;
+                            let ce = new Uint8Array(Z * g),
                                 ue = 0;
                             for (const Ee of R.data) {
                                 let De = 128;
                                 for (; De > 0;)
                                     ce[ue++] = Ee & De ? 0 : 255, De >>= 1;
                             }
                             let me = 0;
                             for (ue = 0, ce[ue] !== 0 && (O[0] = 1, ++me), z = 1; z < d; z++)
                                 ce[ue] !== ce[ue + 1] && (O[z] = ce[ue] ? 2 : 1, ++me), ue++;
                             for (ce[ue] !== 0 && (O[z] = 2, ++me), H = 1; H < g; H++) {
-                                ue = H * Q, ae = H * A, ce[ue - Q] !== ce[ue] && (O[ae] = ce[ue] ? 1 : 8, ++me);
-                                let Ee = (ce[ue] ? 4 : 0) + (ce[ue - Q] ? 8 : 0);
+                                ue = H * Z, ae = H * A, ce[ue - Z] !== ce[ue] && (O[ae] = ce[ue] ? 1 : 8, ++me);
+                                let Ee = (ce[ue] ? 4 : 0) + (ce[ue - Z] ? 8 : 0);
                                 for (z = 1; z < d; z++)
-                                    Ee = (Ee >> 2) + (ce[ue + 1] ? 4 : 0) + (ce[ue - Q + 1] ? 8 : 0), v[Ee] && (O[ae + z] = v[Ee], ++me), ue++;
-                                if (ce[ue - Q] !== ce[ue] && (O[ae + z] = ce[ue] ? 2 : 4, ++me), me > f)
+                                    Ee = (Ee >> 2) + (ce[ue + 1] ? 4 : 0) + (ce[ue - Z + 1] ? 8 : 0), v[Ee] && (O[ae + z] = v[Ee], ++me), ue++;
+                                if (ce[ue - Z] !== ce[ue] && (O[ae + z] = ce[ue] ? 2 : 4, ++me), me > f)
                                     return null;
                             }
-                            for (ue = Q * (g - 1), ae = H * A, ce[ue] !== 0 && (O[ae] = 8, ++me), z = 1; z < d; z++)
+                            for (ue = Z * (g - 1), ae = H * A, ce[ue] !== 0 && (O[ae] = 8, ++me), z = 1; z < d; z++)
                                 ce[ue] !== ce[ue + 1] && (O[ae + z] = ce[ue] ? 4 : 8, ++me), ue++;
                             if (ce[ue] !== 0 && (O[ae + z] = 4, ++me), me > f)
                                 return null;
                             const fe = new Int32Array([0, A, -1, 0, -A, 0, 0, 0, 1]),
                                 Pe = new Path2D();
                             for (H = 0; me && H <= g; H++) {
                                 let Ee = H * A;
@@ -13161,18 +13161,18 @@
                                 const f = n.Util.applyTransform(g, d),
                                     v = n.Util.applyTransform(g.slice(2), d);
                                 this.minX = Math.min(this.minX, f[0], v[0]), this.minY = Math.min(this.minY, f[1], v[1]), this.maxX = Math.max(this.maxX, f[0], v[0]), this.maxY = Math.max(this.maxY, f[1], v[1]);
                             }
                             updateScalingPathMinMax(d, g) {
                                 n.Util.scaleMinMax(d, g), this.minX = Math.min(this.minX, g[0]), this.maxX = Math.max(this.maxX, g[1]), this.minY = Math.min(this.minY, g[2]), this.maxY = Math.max(this.maxY, g[3]);
                             }
-                            updateCurvePathMinMax(d, g, f, v, A, O, H, z, ae, Q) {
+                            updateCurvePathMinMax(d, g, f, v, A, O, H, z, ae, Z) {
                                 const ce = n.Util.bezierBoundingBox(g, f, v, A, O, H, z, ae);
-                                if (Q) {
-                                    Q[0] = Math.min(Q[0], ce[0], ce[2]), Q[1] = Math.max(Q[1], ce[0], ce[2]), Q[2] = Math.min(Q[2], ce[1], ce[3]), Q[3] = Math.max(Q[3], ce[1], ce[3]);
+                                if (Z) {
+                                    Z[0] = Math.min(Z[0], ce[0], ce[2]), Z[1] = Math.max(Z[1], ce[0], ce[2]), Z[2] = Math.min(Z[2], ce[1], ce[3]), Z[3] = Math.max(Z[3], ce[1], ce[3]);
                                     return;
                                 }
                                 this.updateRectMinMax(d, ce);
                             }
                             getPathBoundingBox(d = l.PathType.FILL, g = null) {
                                 const f = [this.minX, this.minY, this.maxX, this.maxY];
                                 if (d === l.PathType.STROKE) {
@@ -13208,49 +13208,49 @@
                                 f = d.width,
                                 v = g % w,
                                 A = (g - v) / w,
                                 O = v === 0 ? A : A + 1,
                                 H = R.createImageData(f, w);
                             let z = 0,
                                 ae;
-                            const Q = d.data,
+                            const Z = d.data,
                                 ce = H.data;
                             let ue, me, fe, Pe;
                             if (d.kind === n.ImageKind.GRAYSCALE_1BPP) {
-                                const Fe = Q.byteLength,
+                                const Fe = Z.byteLength,
                                     Ee = new Uint32Array(ce.buffer, 0, ce.byteLength >> 2),
                                     De = Ee.length,
                                     _e = f + 7 >> 3,
                                     ie = 4294967295,
                                     se = n.FeatureTest.isLittleEndian ? 4278190080 : 255;
                                 for (ue = 0; ue < O; ue++) {
                                     for (fe = ue < A ? w : v, ae = 0, me = 0; me < fe; me++) {
                                         const ge = Fe - z;
                                         let Ce = 0;
                                         const xe = ge > _e ? f : ge * 8 - 7,
-                                            Ue = xe & -8;
+                                            He = xe & -8;
                                         let We = 0,
                                             je = 0;
-                                        for (; Ce < Ue; Ce += 8)
-                                            je = Q[z++], Ee[ae++] = je & 128 ? ie : se, Ee[ae++] = je & 64 ? ie : se, Ee[ae++] = je & 32 ? ie : se, Ee[ae++] = je & 16 ? ie : se, Ee[ae++] = je & 8 ? ie : se, Ee[ae++] = je & 4 ? ie : se, Ee[ae++] = je & 2 ? ie : se, Ee[ae++] = je & 1 ? ie : se;
+                                        for (; Ce < He; Ce += 8)
+                                            je = Z[z++], Ee[ae++] = je & 128 ? ie : se, Ee[ae++] = je & 64 ? ie : se, Ee[ae++] = je & 32 ? ie : se, Ee[ae++] = je & 16 ? ie : se, Ee[ae++] = je & 8 ? ie : se, Ee[ae++] = je & 4 ? ie : se, Ee[ae++] = je & 2 ? ie : se, Ee[ae++] = je & 1 ? ie : se;
                                         for (; Ce < xe; Ce++)
-                                            We === 0 && (je = Q[z++], We = 128), Ee[ae++] = je & We ? ie : se, We >>= 1;
+                                            We === 0 && (je = Z[z++], We = 128), Ee[ae++] = je & We ? ie : se, We >>= 1;
                                     }
                                     for (; ae < De;)
                                         Ee[ae++] = 0;
                                     R.putImageData(H, 0, ue * w);
                                 }
                             } else if (d.kind === n.ImageKind.RGBA_32BPP) {
                                 for (me = 0, Pe = f * w * 4, ue = 0; ue < A; ue++)
-                                    ce.set(Q.subarray(z, z + Pe)), z += Pe, R.putImageData(H, 0, me), me += w;
-                                ue < O && (Pe = f * v * 4, ce.set(Q.subarray(z, z + Pe)), R.putImageData(H, 0, me));
+                                    ce.set(Z.subarray(z, z + Pe)), z += Pe, R.putImageData(H, 0, me), me += w;
+                                ue < O && (Pe = f * v * 4, ce.set(Z.subarray(z, z + Pe)), R.putImageData(H, 0, me));
                             } else if (d.kind === n.ImageKind.RGB_24BPP)
                                 for (fe = w, Pe = f * fe, ue = 0; ue < O; ue++) {
                                     for (ue >= A && (fe = v, Pe = f * fe), ae = 0, me = Pe; me--;)
-                                        ce[ae++] = Q[z++], ce[ae++] = Q[z++], ce[ae++] = Q[z++], ce[ae++] = 255;
+                                        ce[ae++] = Z[z++], ce[ae++] = Z[z++], ce[ae++] = Z[z++], ce[ae++] = 255;
                                     R.putImageData(H, 0, ue * w);
                                 }
                             else
                                 throw new Error(`bad image kind: ${d.kind}`);
                         }
 
                         function y(R, d) {
@@ -13262,23 +13262,23 @@
                                 f = d.width,
                                 v = g % w,
                                 A = (g - v) / w,
                                 O = v === 0 ? A : A + 1,
                                 H = R.createImageData(f, w);
                             let z = 0;
                             const ae = d.data,
-                                Q = H.data;
+                                Z = H.data;
                             for (let ce = 0; ce < O; ce++) {
                                 const ue = ce < A ? w : v;
                                 ({
                                     srcPos: z
                                 } = (0, h.convertBlackAndWhiteToRGBA)({
                                     src: ae,
                                     srcPos: z,
-                                    dest: Q,
+                                    dest: Z,
                                     width: f,
                                     height: ue,
                                     nonBlackColor: 0
                                 })), R.putImageData(H, 0, ce * w);
                             }
                         }
 
@@ -13324,24 +13324,24 @@
                             const f = R.length;
                             for (let v = 3; v < f; v += 4) {
                                 const A = R[v - 3] * 77 + R[v - 2] * 152 + R[v - 1] * 28;
                                 d[v] = g ? d[v] * g[A >> 8] >> 8 : d[v] * A >> 16;
                             }
                         }
 
-                        function N(R, d, g, f, v, A, O, H, z, ae, Q) {
+                        function N(R, d, g, f, v, A, O, H, z, ae, Z) {
                             const ce = !!A,
                                 ue = ce ? A[0] : 0,
                                 me = ce ? A[1] : 0,
                                 fe = ce ? A[2] : 0,
                                 Pe = v === "Luminosity" ? m : M,
                                 Ee = Math.min(f, Math.ceil(1048576 / g));
                             for (let De = 0; De < f; De += Ee) {
                                 const _e = Math.min(Ee, f - De),
-                                    ie = R.getImageData(H - ae, De + (z - Q), g, _e),
+                                    ie = R.getImageData(H - ae, De + (z - Z), g, _e),
                                     se = d.getImageData(H, De + z, g, _e);
                                 ce && $(ie.data, ue, me, fe), Pe(ie.data, se.data, O), d.putImageData(se, H, De + z);
                             }
                         }
 
                         function D(R, d, g, f) {
                             const v = f[0],
@@ -13392,15 +13392,15 @@
                                     const A = d.argsArray,
                                         O = d.fnArray;
                                     let H = g || 0;
                                     const z = A.length;
                                     if (z === H)
                                         return H;
                                     const ae = z - H > T && typeof f == "function",
-                                        Q = ae ? Date.now() + r : 0;
+                                        Z = ae ? Date.now() + r : 0;
                                     let ce = 0;
                                     const ue = this.commonObjs,
                                         me = this.objs;
                                     let fe;
                                     for (;;) {
                                         if (v !== void 0 && H === v.nextBreakPoint)
                                             return v.breakIt(H, f), H;
@@ -13411,22 +13411,22 @@
                                                 const Fe = Pe.startsWith("g_") ? ue : me;
                                                 if (!Fe.has(Pe))
                                                     return Fe.get(Pe, f), H;
                                             }
                                         if (H++, H === z)
                                             return H;
                                         if (ae && ++ce > T) {
-                                            if (Date.now() > Q)
+                                            if (Date.now() > Z)
                                                 return f(), H;
                                             ce = 0;
                                         }
                                     }
                                 }
                                 endDrawing() {
-                                    K(this, q, Zt).call(this), this.cachedCanvases.clear(), this.cachedPatterns.clear();
+                                    K(this, q, Qt).call(this), this.cachedCanvases.clear(), this.cachedPatterns.clear();
                                     for (const d of this._cachedBitmapsMap.values()) {
                                         for (const g of d.values())
                                             typeof HTMLCanvasElement < "u" && g instanceof HTMLCanvasElement && (g.width = g.height = 0);
                                         d.clear();
                                     }
                                     this._cachedBitmapsMap.clear(), K(this, pe, en).call(this);
                                 }
@@ -13434,19 +13434,19 @@
                                     const f = d.width,
                                         v = d.height;
                                     let A = Math.max(Math.hypot(g[0], g[1]), 1),
                                         O = Math.max(Math.hypot(g[2], g[3]), 1),
                                         H = f,
                                         z = v,
                                         ae = "prescale1",
-                                        Q, ce;
+                                        Z, ce;
                                     for (; A > 2 && H > 1 || O > 2 && z > 1;) {
                                         let ue = H,
                                             me = z;
-                                        A > 2 && H > 1 && (ue = H >= 16384 ? Math.floor(H / 2) - 1 || 1 : Math.ceil(H / 2), A /= H / ue), O > 2 && z > 1 && (me = z >= 16384 ? Math.floor(z / 2) - 1 || 1 : Math.ceil(z) / 2, O /= z / me), Q = this.cachedCanvases.getCanvas(ae, ue, me), ce = Q.context, ce.clearRect(0, 0, ue, me), ce.drawImage(d, 0, 0, H, z, 0, 0, ue, me), d = Q.canvas, H = ue, z = me, ae = ae === "prescale1" ? "prescale2" : "prescale1";
+                                        A > 2 && H > 1 && (ue = H >= 16384 ? Math.floor(H / 2) - 1 || 1 : Math.ceil(H / 2), A /= H / ue), O > 2 && z > 1 && (me = z >= 16384 ? Math.floor(z / 2) - 1 || 1 : Math.ceil(z) / 2, O /= z / me), Z = this.cachedCanvases.getCanvas(ae, ue, me), ce = Z.context, ce.clearRect(0, 0, ue, me), ce.drawImage(d, 0, 0, H, z, 0, 0, ue, me), d = Z.canvas, H = ue, z = me, ae = ae === "prescale1" ? "prescale2" : "prescale1";
                                     }
                                     return {
                                         img: d,
                                         paintWidth: H,
                                         paintHeight: z
                                     };
                                 }
@@ -13455,43 +13455,43 @@
                                         {
                                             width: f,
                                             height: v
                                         } = d,
                                         A = this.current.fillColor,
                                         O = this.current.patternFill,
                                         H = (0, s.getCurrentTransform)(g);
-                                    let z, ae, Q, ce;
+                                    let z, ae, Z, ce;
                                     if ((d.bitmap || d.data) && d.count > 1) {
                                         const Ce = d.bitmap || d.data.buffer;
                                         ae = JSON.stringify(O ? H : [H.slice(0, 4), A]), z = this._cachedBitmapsMap.get(Ce), z || (z = /* @__PURE__ */ new Map(), this._cachedBitmapsMap.set(Ce, z));
                                         const xe = z.get(ae);
                                         if (xe && !O) {
-                                            const Ue = Math.round(Math.min(H[0], H[2]) + H[4]),
+                                            const He = Math.round(Math.min(H[0], H[2]) + H[4]),
                                                 We = Math.round(Math.min(H[1], H[3]) + H[5]);
                                             return {
                                                 canvas: xe,
-                                                offsetX: Ue,
+                                                offsetX: He,
                                                 offsetY: We
                                             };
                                         }
-                                        Q = xe;
+                                        Z = xe;
                                     }
-                                    Q || (ce = this.cachedCanvases.getCanvas("maskCanvas", f, v), y(ce.context, d));
+                                    Z || (ce = this.cachedCanvases.getCanvas("maskCanvas", f, v), y(ce.context, d));
                                     let ue = n.Util.transform(H, [1 / f, 0, 0, -1 / v, 0, 0]);
                                     ue = n.Util.transform(ue, [1, 0, 0, 1, 0, -v]);
                                     const me = n.Util.applyTransform([0, 0], ue),
                                         fe = n.Util.applyTransform([f, v], ue),
                                         Pe = n.Util.normalizeRect([me[0], me[1], fe[0], fe[1]]),
                                         Fe = Math.round(Pe[2] - Pe[0]) || 1,
                                         Ee = Math.round(Pe[3] - Pe[1]) || 1,
                                         De = this.cachedCanvases.getCanvas("fillCanvas", Fe, Ee),
                                         _e = De.context,
                                         ie = Math.min(me[0], fe[0]),
                                         se = Math.min(me[1], fe[1]);
-                                    _e.translate(-ie, -se), _e.transform(...ue), Q || (Q = this._scaleImage(ce.canvas, (0, s.getCurrentTransformInverse)(_e)), Q = Q.img, z && O && z.set(ae, Q)), _e.imageSmoothingEnabled = X((0, s.getCurrentTransform)(_e), d.interpolate), b(_e, Q, 0, 0, Q.width, Q.height, 0, 0, f, v), _e.globalCompositeOperation = "source-in";
+                                    _e.translate(-ie, -se), _e.transform(...ue), Z || (Z = this._scaleImage(ce.canvas, (0, s.getCurrentTransformInverse)(_e)), Z = Z.img, z && O && z.set(ae, Z)), _e.imageSmoothingEnabled = X((0, s.getCurrentTransform)(_e), d.interpolate), b(_e, Z, 0, 0, Z.width, Z.height, 0, 0, f, v), _e.globalCompositeOperation = "source-in";
                                     const ge = n.Util.transform((0, s.getCurrentTransformInverse)(_e), [1, 0, 0, 1, -ie, -se]);
                                     return _e.fillStyle = O ? A.getPattern(g, this, ge, l.PathType.FILL) : A, _e.fillRect(0, 0, f, v), z && !O && (this.cachedCanvases.delete("fillCanvas"), z.set(ae, De.canvas)), {
                                         canvas: De.canvas,
                                         offsetX: Math.round(ie),
                                         offsetY: Math.round(se)
                                     };
                                 }
@@ -13605,47 +13605,47 @@
                                 }
                                 constructPath(d, g, f) {
                                     const v = this.ctx,
                                         A = this.current;
                                     let O = A.x,
                                         H = A.y,
                                         z, ae;
-                                    const Q = (0, s.getCurrentTransform)(v),
-                                        ce = Q[0] === 0 && Q[3] === 0 || Q[1] === 0 && Q[2] === 0,
+                                    const Z = (0, s.getCurrentTransform)(v),
+                                        ce = Z[0] === 0 && Z[3] === 0 || Z[1] === 0 && Z[2] === 0,
                                         ue = ce ? f.slice(0) : null;
                                     for (let me = 0, fe = 0, Pe = d.length; me < Pe; me++)
                                         switch (d[me] | 0) {
                                             case n.OPS.rectangle:
                                                 O = g[fe++], H = g[fe++];
                                                 const Fe = g[fe++],
                                                     Ee = g[fe++],
                                                     De = O + Fe,
                                                     _e = H + Ee;
-                                                v.moveTo(O, H), Fe === 0 || Ee === 0 ? v.lineTo(De, _e) : (v.lineTo(De, H), v.lineTo(De, _e), v.lineTo(O, _e)), ce || A.updateRectMinMax(Q, [O, H, De, _e]), v.closePath();
+                                                v.moveTo(O, H), Fe === 0 || Ee === 0 ? v.lineTo(De, _e) : (v.lineTo(De, H), v.lineTo(De, _e), v.lineTo(O, _e)), ce || A.updateRectMinMax(Z, [O, H, De, _e]), v.closePath();
                                                 break;
                                             case n.OPS.moveTo:
-                                                O = g[fe++], H = g[fe++], v.moveTo(O, H), ce || A.updatePathMinMax(Q, O, H);
+                                                O = g[fe++], H = g[fe++], v.moveTo(O, H), ce || A.updatePathMinMax(Z, O, H);
                                                 break;
                                             case n.OPS.lineTo:
-                                                O = g[fe++], H = g[fe++], v.lineTo(O, H), ce || A.updatePathMinMax(Q, O, H);
+                                                O = g[fe++], H = g[fe++], v.lineTo(O, H), ce || A.updatePathMinMax(Z, O, H);
                                                 break;
                                             case n.OPS.curveTo:
-                                                z = O, ae = H, O = g[fe + 4], H = g[fe + 5], v.bezierCurveTo(g[fe], g[fe + 1], g[fe + 2], g[fe + 3], O, H), A.updateCurvePathMinMax(Q, z, ae, g[fe], g[fe + 1], g[fe + 2], g[fe + 3], O, H, ue), fe += 6;
+                                                z = O, ae = H, O = g[fe + 4], H = g[fe + 5], v.bezierCurveTo(g[fe], g[fe + 1], g[fe + 2], g[fe + 3], O, H), A.updateCurvePathMinMax(Z, z, ae, g[fe], g[fe + 1], g[fe + 2], g[fe + 3], O, H, ue), fe += 6;
                                                 break;
                                             case n.OPS.curveTo2:
-                                                z = O, ae = H, v.bezierCurveTo(O, H, g[fe], g[fe + 1], g[fe + 2], g[fe + 3]), A.updateCurvePathMinMax(Q, z, ae, O, H, g[fe], g[fe + 1], g[fe + 2], g[fe + 3], ue), O = g[fe + 2], H = g[fe + 3], fe += 4;
+                                                z = O, ae = H, v.bezierCurveTo(O, H, g[fe], g[fe + 1], g[fe + 2], g[fe + 3]), A.updateCurvePathMinMax(Z, z, ae, O, H, g[fe], g[fe + 1], g[fe + 2], g[fe + 3], ue), O = g[fe + 2], H = g[fe + 3], fe += 4;
                                                 break;
                                             case n.OPS.curveTo3:
-                                                z = O, ae = H, O = g[fe + 2], H = g[fe + 3], v.bezierCurveTo(g[fe], g[fe + 1], O, H, O, H), A.updateCurvePathMinMax(Q, z, ae, g[fe], g[fe + 1], O, H, O, H, ue), fe += 4;
+                                                z = O, ae = H, O = g[fe + 2], H = g[fe + 3], v.bezierCurveTo(g[fe], g[fe + 1], O, H, O, H), A.updateCurvePathMinMax(Z, z, ae, g[fe], g[fe + 1], O, H, O, H, ue), fe += 4;
                                                 break;
                                             case n.OPS.closePath:
                                                 v.closePath();
                                                 break;
                                         }
-                                    ce && A.updateScalingPathMinMax(Q, ue), A.setCurrentPoint(O, H);
+                                    ce && A.updateScalingPathMinMax(Z, ue), A.setCurrentPoint(O, H);
                                 }
                                 closePath() {
                                     this.ctx.closePath();
                                 }
                                 stroke(d = !0) {
                                     const g = this.ctx,
                                         f = this.current.strokeColor;
@@ -13711,23 +13711,23 @@
                                 setHScale(d) {
                                     this.current.textHScale = d / 100;
                                 }
                                 setLeading(d) {
                                     this.current.leading = -d;
                                 }
                                 setFont(d, g) {
-                                    var Q;
+                                    var Z;
                                     const f = this.commonObjs.get(d),
                                         v = this.current;
                                     if (!f)
                                         throw new Error(`Can't find font for ${d}`);
                                     if (v.fontMatrix = f.fontMatrix || n.FONT_IDENTITY_MATRIX, (v.fontMatrix[0] === 0 || v.fontMatrix[3] === 0) && (0, n.warn)("Invalid font matrix for font " + d), g < 0 ? (g = -g, v.fontDirection = -1) : v.fontDirection = 1, this.current.font = f, this.current.fontSize = g, f.isType3Font)
                                         return;
                                     const A = f.loadedName || "sans-serif",
-                                        O = ((Q = f.systemFontInfo) == null ? void 0 : Q.css) || `"${A}", ${f.fallbackName}`;
+                                        O = ((Z = f.systemFontInfo) == null ? void 0 : Z.css) || `"${A}", ${f.fallbackName}`;
                                     let H = "normal";
                                     f.black ? H = "900" : f.bold && (H = "bold");
                                     const z = f.italic ? "italic" : "normal";
                                     let ae = g;
                                     g < _ ? ae = _ : g > c && (ae = c), this.current.fontSizeScale = g / ae, this.ctx.font = `${z} ${H} ${ae}px ${O}`;
                                 }
                                 setTextRenderingMode(d) {
@@ -13750,19 +13750,19 @@
                                 }
                                 paintChar(d, g, f, v) {
                                     const A = this.ctx,
                                         O = this.current,
                                         H = O.font,
                                         z = O.textRenderingMode,
                                         ae = O.fontSize / O.fontSizeScale,
-                                        Q = z & n.TextRenderingMode.FILL_STROKE_MASK,
+                                        Z = z & n.TextRenderingMode.FILL_STROKE_MASK,
                                         ce = !!(z & n.TextRenderingMode.ADD_TO_PATH_FLAG),
                                         ue = O.patternFill && !H.missingFile;
                                     let me;
-                                    (H.disableFontFace || ce || ue) && (me = H.getPathGenerator(this.commonObjs, d)), H.disableFontFace || ue ? (A.save(), A.translate(g, f), A.beginPath(), me(A, ae), v && A.setTransform(...v), (Q === n.TextRenderingMode.FILL || Q === n.TextRenderingMode.FILL_STROKE) && A.fill(), (Q === n.TextRenderingMode.STROKE || Q === n.TextRenderingMode.FILL_STROKE) && A.stroke(), A.restore()) : ((Q === n.TextRenderingMode.FILL || Q === n.TextRenderingMode.FILL_STROKE) && A.fillText(d, g, f), (Q === n.TextRenderingMode.STROKE || Q === n.TextRenderingMode.FILL_STROKE) && A.strokeText(d, g, f)), ce && (this.pendingTextPaths || (this.pendingTextPaths = [])).push({
+                                    (H.disableFontFace || ce || ue) && (me = H.getPathGenerator(this.commonObjs, d)), H.disableFontFace || ue ? (A.save(), A.translate(g, f), A.beginPath(), me(A, ae), v && A.setTransform(...v), (Z === n.TextRenderingMode.FILL || Z === n.TextRenderingMode.FILL_STROKE) && A.fill(), (Z === n.TextRenderingMode.STROKE || Z === n.TextRenderingMode.FILL_STROKE) && A.stroke(), A.restore()) : ((Z === n.TextRenderingMode.FILL || Z === n.TextRenderingMode.FILL_STROKE) && A.fillText(d, g, f), (Z === n.TextRenderingMode.STROKE || Z === n.TextRenderingMode.FILL_STROKE) && A.strokeText(d, g, f)), ce && (this.pendingTextPaths || (this.pendingTextPaths = [])).push({
                                         transform: (0, s.getCurrentTransform)(A),
                                         x: g,
                                         y: f,
                                         fontSize: ae,
                                         addToPath: me
                                     });
                                 }
@@ -13789,22 +13789,22 @@
                                     if (v === 0)
                                         return;
                                     const A = this.ctx,
                                         O = g.fontSizeScale,
                                         H = g.charSpacing,
                                         z = g.wordSpacing,
                                         ae = g.fontDirection,
-                                        Q = g.textHScale * ae,
+                                        Z = g.textHScale * ae,
                                         ce = d.length,
                                         ue = f.vertical,
                                         me = ue ? 1 : -1,
                                         fe = f.defaultVMetrics,
                                         Pe = v * g.fontMatrix[0],
                                         Fe = g.textRenderingMode === n.TextRenderingMode.FILL && !f.disableFontFace && !g.patternFill;
-                                    A.save(), A.transform(...g.textMatrix), A.translate(g.x, g.y + g.textRise), ae > 0 ? A.scale(Q, -1) : A.scale(Q, 1);
+                                    A.save(), A.transform(...g.textMatrix), A.translate(g.x, g.y + g.textRise), ae > 0 ? A.scale(Z, -1) : A.scale(Z, 1);
                                     let Ee;
                                     if (g.patternFill) {
                                         A.save();
                                         const ge = g.fillColor.getPattern(A, this, (0, s.getCurrentTransformInverse)(A), l.PathType.FILL);
                                         Ee = (0, s.getCurrentTransform)(A), A.restore(), A.fillStyle = ge;
                                     }
                                     let De = g.lineWidth;
@@ -13815,86 +13815,86 @@
                                     } else
                                         De /= _e;
                                     if (O !== 1 && (A.scale(O, O), De /= O), A.lineWidth = De, f.isInvalidPDFjsFont) {
                                         const ge = [];
                                         let Ce = 0;
                                         for (const xe of d)
                                             ge.push(xe.unicode), Ce += xe.width;
-                                        A.fillText(ge.join(""), 0, 0), g.x += Ce * Pe * Q, A.restore(), this.compose();
+                                        A.fillText(ge.join(""), 0, 0), g.x += Ce * Pe * Z, A.restore(), this.compose();
                                         return;
                                     }
                                     let ie = 0,
                                         se;
                                     for (se = 0; se < ce; ++se) {
                                         const ge = d[se];
                                         if (typeof ge == "number") {
                                             ie += me * ge * v / 1e3;
                                             continue;
                                         }
                                         let Ce = !1;
                                         const xe = (ge.isSpace ? z : 0) + H,
-                                            Ue = ge.fontChar,
+                                            He = ge.fontChar,
                                             We = ge.accent;
                                         let je, ze, Xe = ge.width;
                                         if (ue) {
                                             const Ye = ge.vmetric || fe,
                                                 de = -(ge.vmetric ? Ye[1] : Xe * 0.5) * Pe,
                                                 ne = Ye[2] * Pe;
                                             Xe = Ye ? -Ye[0] : Xe, je = de / O, ze = (ie + ne) / O;
                                         } else
                                             je = ie / O, ze = 0;
                                         if (f.remeasure && Xe > 0) {
-                                            const Ye = A.measureText(Ue).width * 1e3 / v * O;
+                                            const Ye = A.measureText(He).width * 1e3 / v * O;
                                             if (Xe < Ye && this.isFontSubpixelAAEnabled) {
                                                 const de = Xe / Ye;
                                                 Ce = !0, A.save(), A.scale(de, 1), je /= de;
                                             } else
                                                 Xe !== Ye && (je += (Xe - Ye) / 2e3 * v / O);
                                         }
                                         if (this.contentVisible && (ge.isInFont || f.missingFile)) {
                                             if (Fe && !We)
-                                                A.fillText(Ue, je, ze);
-                                            else if (this.paintChar(Ue, je, ze, Ee), We) {
+                                                A.fillText(He, je, ze);
+                                            else if (this.paintChar(He, je, ze, Ee), We) {
                                                 const Ye = je + v * We.offset.x / O,
                                                     de = ze - v * We.offset.y / O;
                                                 this.paintChar(We.fontChar, Ye, de, Ee);
                                             }
                                         }
                                         const Ge = ue ? Xe * Pe - xe * ae : Xe * Pe + xe * ae;
                                         ie += Ge, Ce && A.restore();
                                     }
-                                    ue ? g.y -= ie : g.x += ie * Q, A.restore(), this.compose();
+                                    ue ? g.y -= ie : g.x += ie * Z, A.restore(), this.compose();
                                 }
                                 showType3Text(d) {
                                     const g = this.ctx,
                                         f = this.current,
                                         v = f.font,
                                         A = f.fontSize,
                                         O = f.fontDirection,
                                         H = v.vertical ? 1 : -1,
                                         z = f.charSpacing,
                                         ae = f.wordSpacing,
-                                        Q = f.textHScale * O,
+                                        Z = f.textHScale * O,
                                         ce = f.fontMatrix || n.FONT_IDENTITY_MATRIX,
                                         ue = d.length,
                                         me = f.textRenderingMode === n.TextRenderingMode.INVISIBLE;
                                     let fe, Pe, Fe, Ee;
                                     if (!(me || A === 0)) {
-                                        for (this._cachedScaleForStroking[0] = -1, this._cachedGetSinglePixelWidth = null, g.save(), g.transform(...f.textMatrix), g.translate(f.x, f.y), g.scale(Q, O), fe = 0; fe < ue; ++fe) {
+                                        for (this._cachedScaleForStroking[0] = -1, this._cachedGetSinglePixelWidth = null, g.save(), g.transform(...f.textMatrix), g.translate(f.x, f.y), g.scale(Z, O), fe = 0; fe < ue; ++fe) {
                                             if (Pe = d[fe], typeof Pe == "number") {
-                                                Ee = H * Pe * A / 1e3, this.ctx.translate(Ee, 0), f.x += Ee * Q;
+                                                Ee = H * Pe * A / 1e3, this.ctx.translate(Ee, 0), f.x += Ee * Z;
                                                 continue;
                                             }
                                             const De = (Pe.isSpace ? ae : 0) + z,
                                                 _e = v.charProcOperatorList[Pe.operatorListId];
                                             if (!_e) {
                                                 (0, n.warn)(`Type3 character "${Pe.operatorListId}" is not available.`);
                                                 continue;
                                             }
-                                            this.contentVisible && (this.processingType3 = Pe, this.save(), g.scale(A, A), g.transform(...ce), this.executeOperatorList(_e), this.restore()), Fe = n.Util.applyTransform([Pe.width, 0], ce)[0] * A + De, g.translate(Fe, 0), f.x += Fe * Q;
+                                            this.contentVisible && (this.processingType3 = Pe, this.save(), g.scale(A, A), g.transform(...ce), this.executeOperatorList(_e), this.restore()), Fe = n.Util.applyTransform([Pe.width, 0], ce)[0] * A + De, g.translate(Fe, 0), f.x += Fe * Z;
                                         }
                                         g.restore(), this.processingType3 = null;
                                     }
                                 }
                                 setCharWidth(d, g) {}
                                 setCharWidthAndBounds(d, g, f, v, A, O) {
                                     this.ctx.rect(f, v, A - f, O - v), this.ctx.clip(), this.endPath();
@@ -13941,16 +13941,16 @@
                                     const f = this._getPattern(d);
                                     g.fillStyle = f.getPattern(g, this, (0, s.getCurrentTransformInverse)(g), l.PathType.SHADING);
                                     const v = (0, s.getCurrentTransformInverse)(g);
                                     if (v) {
                                         const {
                                             width: A,
                                             height: O
-                                        } = g.canvas, [H, z, ae, Q] = n.Util.getAxialAlignedBoundingBox([0, 0, A, O], v);
-                                        this.ctx.fillRect(H, z, ae - H, Q - z);
+                                        } = g.canvas, [H, z, ae, Z] = n.Util.getAxialAlignedBoundingBox([0, 0, A, O], v);
+                                        this.ctx.fillRect(H, z, ae - H, Z - z);
                                     } else
                                         this.ctx.fillRect(-1e10, -1e10, 2e10, 2e10);
                                     this.compose(this.current.getClippedPathBoundingBox()), this.restore();
                                 }
                                 beginInlineImage() {
                                     (0, n.unreachable)("Should not call beginInlineImage");
                                 }
@@ -13979,33 +13979,33 @@
                                     let v = n.Util.getAxialAlignedBoundingBox(d.bbox, (0, s.getCurrentTransform)(g));
                                     const A = [0, 0, g.canvas.width, g.canvas.height];
                                     v = n.Util.intersect(v, A) || [0, 0, 0, 0];
                                     const O = Math.floor(v[0]),
                                         H = Math.floor(v[1]);
                                     let z = Math.max(Math.ceil(v[2]) - O, 1),
                                         ae = Math.max(Math.ceil(v[3]) - H, 1),
-                                        Q = 1,
+                                        Z = 1,
                                         ce = 1;
-                                    z > o && (Q = z / o, z = o), ae > o && (ce = ae / o, ae = o), this.current.startNewPathAndClipBox([0, 0, z, ae]);
+                                    z > o && (Z = z / o, z = o), ae > o && (ce = ae / o, ae = o), this.current.startNewPathAndClipBox([0, 0, z, ae]);
                                     let ue = "groupAt" + this.groupLevel;
                                     d.smask && (ue += "_smask_" + this.smaskCounter++ % 2);
                                     const me = this.cachedCanvases.getCanvas(ue, z, ae),
                                         fe = me.context;
-                                    fe.scale(1 / Q, 1 / ce), fe.translate(-O, -H), fe.transform(...f), d.smask ? this.smaskStack.push({
+                                    fe.scale(1 / Z, 1 / ce), fe.translate(-O, -H), fe.transform(...f), d.smask ? this.smaskStack.push({
                                         canvas: me.canvas,
                                         context: fe,
                                         offsetX: O,
                                         offsetY: H,
-                                        scaleX: Q,
+                                        scaleX: Z,
                                         scaleY: ce,
                                         subtype: d.smask.subtype,
                                         backdrop: d.smask.backdrop,
                                         transferMap: d.smask.transferMap || null,
                                         startTransformInverse: null
-                                    }) : (g.setTransform(1, 0, 0, 1, 0, 0), g.translate(O, H), g.scale(Q, ce), g.save()), p(g, fe), this.ctx = fe, this.setGState([
+                                    }) : (g.setTransform(1, 0, 0, 1, 0, 0), g.translate(O, H), g.scale(Z, ce), g.save()), p(g, fe), this.ctx = fe, this.setGState([
                                         ["BM", "source-over"],
                                         ["ca", 1],
                                         ["CA", 1]
                                     ]), this.groupStack.push(g), this.groupLevel++;
                                 }
                                 endGroup(d) {
                                     if (!this.contentVisible)
@@ -14020,22 +14020,22 @@
                                         const v = (0, s.getCurrentTransform)(this.ctx);
                                         this.restore(), this.ctx.save(), this.ctx.setTransform(...v);
                                         const A = n.Util.getAxialAlignedBoundingBox([0, 0, g.canvas.width, g.canvas.height], v);
                                         this.ctx.drawImage(g.canvas, 0, 0), this.ctx.restore(), this.compose(A);
                                     }
                                 }
                                 beginAnnotation(d, g, f, v, A) {
-                                    if (K(this, q, Zt).call(this), E(this.ctx), this.ctx.save(), this.save(), this.baseTransform && this.ctx.setTransform(...this.baseTransform), Array.isArray(g) && g.length === 4) {
+                                    if (K(this, q, Qt).call(this), E(this.ctx), this.ctx.save(), this.save(), this.baseTransform && this.ctx.setTransform(...this.baseTransform), Array.isArray(g) && g.length === 4) {
                                         const O = g[2] - g[0],
                                             H = g[3] - g[1];
                                         if (A && this.annotationCanvasMap) {
                                             f = f.slice(), f[4] -= g[0], f[5] -= g[1], g = g.slice(), g[0] = g[1] = 0, g[2] = O, g[3] = H;
                                             const [z, ae] = n.Util.singularValueDecompose2dScale((0, s.getCurrentTransform)(this.ctx)), {
-                                                viewportScale: Q
-                                            } = this, ce = Math.ceil(O * this.outputScaleX * Q), ue = Math.ceil(H * this.outputScaleY * Q);
+                                                viewportScale: Z
+                                            } = this, ce = Math.ceil(O * this.outputScaleX * Z), ue = Math.ceil(H * this.outputScaleY * Z);
                                             this.annotationCanvas = this.canvasFactory.create(ce, ue);
                                             const {
                                                 canvas: me,
                                                 context: fe
                                             } = this.annotationCanvas;
                                             this.annotationCanvasMap.set(d, me), this.annotationCanvas.savedCtx = this.ctx, this.ctx = fe, this.ctx.save(), this.ctx.setTransform(z, 0, 0, -ae, 0, H * ae), E(this.ctx);
                                         } else
@@ -14067,16 +14067,16 @@
                                     d = this.getObject(d.data, d);
                                     const H = this.ctx;
                                     H.save();
                                     const z = (0, s.getCurrentTransform)(H);
                                     H.transform(g, f, v, A, 0, 0);
                                     const ae = this._createMaskCanvas(d);
                                     H.setTransform(1, 0, 0, 1, ae.offsetX - z[4], ae.offsetY - z[5]);
-                                    for (let Q = 0, ce = O.length; Q < ce; Q += 2) {
-                                        const ue = n.Util.transform(z, [g, f, v, A, O[Q], O[Q + 1]]),
+                                    for (let Z = 0, ce = O.length; Z < ce; Z += 2) {
+                                        const ue = n.Util.transform(z, [g, f, v, A, O[Z], O[Z + 1]]),
                                             [me, fe] = n.Util.applyTransform([0, 0], ue);
                                         H.drawImage(ae.canvas, me, fe);
                                     }
                                     H.restore(), this.compose();
                                 }
                                 paintImageMaskXObjectGroup(d) {
                                     if (!this.contentVisible)
@@ -14086,18 +14086,18 @@
                                         v = this.current.patternFill;
                                     for (const A of d) {
                                         const {
                                             data: O,
                                             width: H,
                                             height: z,
                                             transform: ae
-                                        } = A, Q = this.cachedCanvases.getCanvas("maskCanvas", H, z), ce = Q.context;
+                                        } = A, Z = this.cachedCanvases.getCanvas("maskCanvas", H, z), ce = Z.context;
                                         ce.save();
                                         const ue = this.getObject(O, A);
-                                        y(ce, ue), ce.globalCompositeOperation = "source-in", ce.fillStyle = v ? f.getPattern(ce, this, (0, s.getCurrentTransformInverse)(g), l.PathType.FILL) : f, ce.fillRect(0, 0, H, z), ce.restore(), g.save(), g.transform(...ae), g.scale(1, -1), b(g, Q.canvas, 0, 0, H, z, 0, -1, 1, 1), g.restore();
+                                        y(ce, ue), ce.globalCompositeOperation = "source-in", ce.fillStyle = v ? f.getPattern(ce, this, (0, s.getCurrentTransformInverse)(g), l.PathType.FILL) : f, ce.fillRect(0, 0, H, z), ce.restore(), g.save(), g.transform(...ae), g.scale(1, -1), b(g, Z.canvas, 0, 0, H, z, 0, -1, 1, 1), g.restore();
                                     }
                                     this.compose();
                                 }
                                 paintImageXObject(d) {
                                     if (!this.contentVisible)
                                         return;
                                     const g = this.getObject(d);
@@ -14114,15 +14114,15 @@
                                     if (!A) {
                                         (0, n.warn)("Dependent image isn't ready yet");
                                         return;
                                     }
                                     const O = A.width,
                                         H = A.height,
                                         z = [];
-                                    for (let ae = 0, Q = v.length; ae < Q; ae += 2)
+                                    for (let ae = 0, Z = v.length; ae < Z; ae += 2)
                                         z.push({
                                             transform: [g, 0, 0, f, v[ae], v[ae + 1]],
                                             x: 0,
                                             y: 0,
                                             w: O,
                                             h: H
                                         });
@@ -14239,33 +14239,33 @@
                                         if (f === 0 && v === 0) {
                                             const z = Math.abs(g),
                                                 ae = Math.abs(A);
                                             if (z === ae)
                                                 if (d === 0)
                                                     O = H = 1 / z;
                                                 else {
-                                                    const Q = z * d;
-                                                    O = H = Q < 1 ? 1 / Q : 1;
+                                                    const Z = z * d;
+                                                    O = H = Z < 1 ? 1 / Z : 1;
                                                 }
                                             else if (d === 0)
                                                 O = 1 / z, H = 1 / ae;
                                             else {
-                                                const Q = z * d,
+                                                const Z = z * d,
                                                     ce = ae * d;
-                                                O = Q < 1 ? 1 / Q : 1, H = ce < 1 ? 1 / ce : 1;
+                                                O = Z < 1 ? 1 / Z : 1, H = ce < 1 ? 1 / ce : 1;
                                             }
                                         } else {
                                             const z = Math.abs(g * A - f * v),
                                                 ae = Math.hypot(g, f),
-                                                Q = Math.hypot(v, A);
+                                                Z = Math.hypot(v, A);
                                             if (d === 0)
-                                                O = Q / z, H = ae / z;
+                                                O = Z / z, H = ae / z;
                                             else {
                                                 const ce = d * z;
-                                                O = Q > ce ? Q / ce : 1, H = ae > ce ? ae / ce : 1;
+                                                O = Z > ce ? Z / ce : 1, H = ae > ce ? ae / ce : 1;
                                             }
                                         }
                                         this._cachedScaleForStroking[0] = O, this._cachedScaleForStroking[1] = H;
                                     }
                                     return this._cachedScaleForStroking;
                                 }
                                 rescaleAndStroke(d) {
@@ -14288,15 +14288,15 @@
                                 isContentVisible() {
                                     for (let d = this.markedContentStack.length - 1; d >= 0; d--)
                                         if (!this.markedContentStack[d].visible)
                                             return !1;
                                     return !0;
                                 }
                             };
-                        q = new WeakSet(), Zt = function() {
+                        q = new WeakSet(), Qt = function() {
                             for (; this.stateStack.length || this.inSMaskMode;)
                                 this.restore();
                             this.ctx.restore(), this.transparentCanvas && (this.ctx = this.compositeCtx, this.ctx.save(), this.ctx.setTransform(1, 0, 0, 1, 0, 0), this.ctx.drawImage(this.transparentCanvas, 0, 0), this.ctx.restore(), this.transparentCanvas = null);
                         }, pe = new WeakSet(), en = function() {
                             if (this.pageColors) {
                                 const d = this.filterFactory.addHCMFilter(this.pageColors.foreground, this.pageColors.background);
                                 if (d !== "none") {
@@ -14391,30 +14391,30 @@
                                 d = N[$ + 1],
                                 g = N[$ + 2],
                                 f = N[M],
                                 v = N[M + 1],
                                 A = N[M + 2],
                                 O = Math.round(B),
                                 H = Math.round(le);
-                            let z, ae, Q, ce, ue, me, fe, Pe;
+                            let z, ae, Z, ce, ue, me, fe, Pe;
                             for (let Fe = O; Fe <= H; Fe++) {
                                 if (Fe < Y) {
                                     const se = Fe < B ? 0 : (B - Fe) / (B - Y);
-                                    z = I - (I - ee) * se, ae = pe - (pe - R) * se, Q = we - (we - d) * se, ce = be - (be - g) * se;
+                                    z = I - (I - ee) * se, ae = pe - (pe - R) * se, Z = we - (we - d) * se, ce = be - (be - g) * se;
                                 } else {
                                     let se;
-                                    Fe > le ? se = 1 : Y === le ? se = 0 : se = (Y - Fe) / (Y - le), z = ee - (ee - q) * se, ae = R - (R - f) * se, Q = d - (d - v) * se, ce = g - (g - A) * se;
+                                    Fe > le ? se = 1 : Y === le ? se = 0 : se = (Y - Fe) / (Y - le), z = ee - (ee - q) * se, ae = R - (R - f) * se, Z = d - (d - v) * se, ce = g - (g - A) * se;
                                 }
                                 let Ee;
                                 Fe < B ? Ee = 0 : Fe > le ? Ee = 1 : Ee = (B - Fe) / (B - le), ue = I - (I - q) * Ee, me = pe - (pe - f) * Ee, fe = we - (we - v) * Ee, Pe = be - (be - A) * Ee;
                                 const De = Math.round(Math.min(z, ue)),
                                     _e = Math.round(Math.max(z, ue));
                                 let ie = X * Fe + De * 4;
                                 for (let se = De; se <= _e; se++)
-                                    Ee = (z - se) / (z - ue), Ee < 0 ? Ee = 0 : Ee > 1 && (Ee = 1), D[ie++] = ae - (ae - me) * Ee | 0, D[ie++] = Q - (Q - fe) * Ee | 0, D[ie++] = ce - (ce - Pe) * Ee | 0, D[ie++] = 255;
+                                    Ee = (z - se) / (z - ue), Ee < 0 ? Ee = 0 : Ee > 1 && (Ee = 1), D[ie++] = ae - (ae - me) * Ee | 0, D[ie++] = Z - (Z - fe) * Ee | 0, D[ie++] = ce - (ce - Pe) * Ee | 0, D[ie++] = 255;
                             }
                         }
 
                         function r(k, F, x) {
                             const y = F.coords,
                                 p = F.colors;
                             let E, $;
@@ -18158,15 +18158,15 @@
                         }, nt(B, "_freeTextDefaultContent", ""), nt(B, "_internalPadding", 0), nt(B, "_defaultColor", null), nt(B, "_defaultFontSize", 10), nt(B, "_type", "freetext");
                         let _ = B;
                         e.FreeTextEditor = _;
                     },
                     /* 29 */
                     /***/
                     (t, e, i) => {
-                        var g, v, ht, O, Nn, z, ae, Q, ce, ue, me, fe, Pe, Fe, Ee, De, _e, ie, se, ge, Ce, xe, Ue, $n, je, Mt, Xe, ln, Ye, cn, ne, J, ve, Se, tt, et, te, hn, Ne, ke, $e, Be, Bn, Ae, un;
+                        var g, v, ht, O, Nn, z, ae, Z, ce, ue, me, fe, Pe, Fe, Ee, De, _e, ie, se, ge, Ce, xe, He, $n, je, Mt, Xe, ln, Ye, cn, ne, J, ve, Se, tt, et, te, hn, Ne, ke, $e, Be, Bn, Ae, un;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.StampAnnotationElement = e.InkAnnotationElement = e.FreeTextAnnotationElement = e.AnnotationLayer = void 0;
                         var n = i(1),
                             s = i(6),
                             l = i(3),
                             h = i(30),
@@ -18261,39 +18261,39 @@
                                     parent: {
                                         page: L,
                                         viewport: j
                                     }
                                 } = this, V = document.createElement("section");
                                 V.setAttribute("data-annotation-id", u.id), this instanceof k || (V.tabIndex = o), V.style.zIndex = this.parent.zIndex++, this.data.popupRef && V.setAttribute("aria-haspopup", "dialog"), u.noRotate && V.classList.add("norotate");
                                 const {
-                                    pageWidth: Z,
+                                    pageWidth: Q,
                                     pageHeight: he,
                                     pageX: ye,
                                     pageY: Me
                                 } = j.rawDims;
                                 if (!u.rect || this instanceof M) {
                                     const {
-                                        rotation: He
+                                        rotation: Ue
                                     } = u;
-                                    return !u.hasOwnCanvas && He !== 0 && this.setRotation(He, V), V;
+                                    return !u.hasOwnCanvas && Ue !== 0 && this.setRotation(Ue, V), V;
                                 }
                                 const {
                                     width: Re,
                                     height: qe
                                 } = S(u.rect), Ie = n.Util.normalizeRect([u.rect[0], L.view[3] - u.rect[1] + L.view[1], u.rect[2], L.view[3] - u.rect[3] + L.view[1]]);
                                 if (!U && u.borderStyle.width > 0) {
                                     V.style.borderWidth = `${u.borderStyle.width}px`;
-                                    const He = u.borderStyle.horizontalCornerRadius,
+                                    const Ue = u.borderStyle.horizontalCornerRadius,
                                         Ve = u.borderStyle.verticalCornerRadius;
-                                    if (He > 0 || Ve > 0) {
-                                        const Ze = `calc(${He}px * var(--scale-factor)) / calc(${Ve}px * var(--scale-factor))`;
-                                        V.style.borderRadius = Ze;
+                                    if (Ue > 0 || Ve > 0) {
+                                        const Qe = `calc(${Ue}px * var(--scale-factor)) / calc(${Ve}px * var(--scale-factor))`;
+                                        V.style.borderRadius = Qe;
                                     } else if (this instanceof p) {
-                                        const Ze = `calc(${Re}px * var(--scale-factor)) / calc(${qe}px * var(--scale-factor))`;
-                                        V.style.borderRadius = Ze;
+                                        const Qe = `calc(${Re}px * var(--scale-factor)) / calc(${qe}px * var(--scale-factor))`;
+                                        V.style.borderRadius = Qe;
                                     }
                                     switch (u.borderStyle.style) {
                                         case n.AnnotationBorderStyleType.SOLID:
                                             V.style.borderStyle = "solid";
                                             break;
                                         case n.AnnotationBorderStyleType.DASHED:
                                             V.style.borderStyle = "dashed";
@@ -18307,40 +18307,40 @@
                                         case n.AnnotationBorderStyleType.UNDERLINE:
                                             V.style.borderBottomStyle = "solid";
                                             break;
                                     }
                                     const Je = u.borderColor || null;
                                     Je ? (oe(this, g, !0), V.style.borderColor = n.Util.makeHexColor(Je[0] | 0, Je[1] | 0, Je[2] | 0)) : V.style.borderWidth = 0;
                                 }
-                                V.style.left = `${100 * (Ie[0] - ye) / Z}%`, V.style.top = `${100 * (Ie[1] - Me) / he}%`;
+                                V.style.left = `${100 * (Ie[0] - ye) / Q}%`, V.style.top = `${100 * (Ie[1] - Me) / he}%`;
                                 const {
                                     rotation: Le
                                 } = u;
-                                return u.hasOwnCanvas || Le === 0 ? (V.style.width = `${100 * Re / Z}%`, V.style.height = `${100 * qe / he}%`) : this.setRotation(Le, V), V;
+                                return u.hasOwnCanvas || Le === 0 ? (V.style.width = `${100 * Re / Q}%`, V.style.height = `${100 * qe / he}%`) : this.setRotation(Le, V), V;
                             }
                             setRotation(U, u = this.container) {
                                 if (!this.data.rect)
                                     return;
                                 const {
                                     pageWidth: L,
                                     pageHeight: j
                                 } = this.parent.viewport.rawDims, {
                                     width: V,
-                                    height: Z
+                                    height: Q
                                 } = S(this.data.rect);
                                 let he, ye;
-                                U % 180 === 0 ? (he = 100 * V / L, ye = 100 * Z / j) : (he = 100 * Z / L, ye = 100 * V / j), u.style.width = `${he}%`, u.style.height = `${ye}%`, u.setAttribute("data-main-rotation", (360 - U) % 360);
+                                U % 180 === 0 ? (he = 100 * V / L, ye = 100 * Q / j) : (he = 100 * Q / L, ye = 100 * V / j), u.style.width = `${he}%`, u.style.height = `${ye}%`, u.setAttribute("data-main-rotation", (360 - U) % 360);
                             }
                             get _commonActions() {
                                 const U = (u, L, j) => {
                                     const V = j.detail[u],
-                                        Z = V[0],
+                                        Q = V[0],
                                         he = V.slice(1);
-                                    j.target.style[L] = h.ColorConverters[`${Z}_HTML`](he), this.annotationStorage.setValue(this.data.id, {
-                                        [L]: h.ColorConverters[`${Z}_rgb`](he)
+                                    j.target.style[L] = h.ColorConverters[`${Q}_HTML`](he), this.annotationStorage.setValue(this.data.id, {
+                                        [L]: h.ColorConverters[`${Q}_rgb`](he)
                                     });
                                 };
                                 return (0, n.shadow)(this, "_commonActions", {
                                     display: (u) => {
                                         const {
                                             display: L
                                         } = u.detail, j = L % 2 === 1;
@@ -18414,23 +18414,23 @@
                                 if (!this.enableScripting)
                                     return;
                                 const u = this.annotationStorage.getRawValue(this.data.id);
                                 if (!u)
                                     return;
                                 const L = this._commonActions;
                                 for (const [j, V] of Object.entries(u)) {
-                                    const Z = L[j];
-                                    if (Z) {
+                                    const Q = L[j];
+                                    if (Q) {
                                         const he = {
                                             detail: {
                                                 [j]: V
                                             },
                                             target: U
                                         };
-                                        Z(he), delete u[j];
+                                        Q(he), delete u[j];
                                     }
                                 }
                             }
                             _createQuadrilaterals() {
                                 if (!this.container)
                                     return;
                                 const {
@@ -18440,58 +18440,58 @@
                                     return;
                                 const [u, L, j, V] = this.data.rect;
                                 if (U.length === 1) {
                                     const [, {
                                         x: Ve,
                                         y: Je
                                     }, {
-                                        x: Ze,
+                                        x: Qe,
                                         y: st
                                     }] = U[0];
-                                    if (j === Ve && V === Je && u === Ze && L === st)
+                                    if (j === Ve && V === Je && u === Qe && L === st)
                                         return;
                                 }
                                 const {
-                                    style: Z
+                                    style: Q
                                 } = this.container;
                                 let he;
                                 if (a(this, g)) {
                                     const {
                                         borderColor: Ve,
                                         borderWidth: Je
-                                    } = Z;
-                                    Z.borderWidth = 0, he = ["url('data:image/svg+xml;utf8,", '<svg xmlns="http://www.w3.org/2000/svg"', ' preserveAspectRatio="none" viewBox="0 0 1 1">', `<g fill="transparent" stroke="${Ve}" stroke-width="${Je}">`], this.container.classList.add("hasBorder");
+                                    } = Q;
+                                    Q.borderWidth = 0, he = ["url('data:image/svg+xml;utf8,", '<svg xmlns="http://www.w3.org/2000/svg"', ' preserveAspectRatio="none" viewBox="0 0 1 1">', `<g fill="transparent" stroke="${Ve}" stroke-width="${Je}">`], this.container.classList.add("hasBorder");
                                 }
                                 const ye = j - u,
                                     Me = V - L,
                                     {
                                         svgFactory: Re
                                     } = this,
                                     qe = Re.createElement("svg");
                                 qe.classList.add("quadrilateralsContainer"), qe.setAttribute("width", 0), qe.setAttribute("height", 0);
                                 const Ie = Re.createElement("defs");
                                 qe.append(Ie);
                                 const Le = Re.createElement("clipPath"),
-                                    He = `clippath_${this.data.id}`;
-                                Le.setAttribute("id", He), Le.setAttribute("clipPathUnits", "objectBoundingBox"), Ie.append(Le);
+                                    Ue = `clippath_${this.data.id}`;
+                                Le.setAttribute("id", Ue), Le.setAttribute("clipPathUnits", "objectBoundingBox"), Ie.append(Le);
                                 for (const [, {
                                         x: Ve,
                                         y: Je
                                     }, {
-                                        x: Ze,
+                                        x: Qe,
                                         y: st
                                     }] of U) {
                                     const it = Re.createElement("rect"),
-                                        rt = (Ze - u) / ye,
+                                        rt = (Qe - u) / ye,
                                         lt = (V - Je) / Me,
-                                        ct = (Ve - Ze) / ye,
+                                        ct = (Ve - Qe) / ye,
                                         An = (Je - st) / Me;
                                     it.setAttribute("x", rt), it.setAttribute("y", lt), it.setAttribute("width", ct), it.setAttribute("height", An), Le.append(it), he == null || he.push(`<rect vector-effect="non-scaling-stroke" x="${rt}" y="${lt}" width="${ct}" height="${An}"/>`);
                                 }
-                                a(this, g) && (he.push("</g></svg>')"), Z.backgroundImage = he.join("")), this.container.append(qe), this.container.style.clipPath = `url(#${He})`;
+                                a(this, g) && (he.push("</g></svg>')"), Q.backgroundImage = he.join("")), this.container.append(qe), this.container.style.clipPath = `url(#${Ue})`;
                             }
                             _createPopup() {
                                 const {
                                     container: U,
                                     data: u
                                 } = this;
                                 U.setAttribute("aria-haspopup", "dialog");
@@ -18518,40 +18518,40 @@
                             _getElementsByName(U, u = null) {
                                 const L = [];
                                 if (this._fieldObjects) {
                                     const j = this._fieldObjects[U];
                                     if (j)
                                         for (const {
                                                 page: V,
-                                                id: Z,
+                                                id: Q,
                                                 exportValues: he
                                             }
                                             of j) {
-                                            if (V === -1 || Z === u)
+                                            if (V === -1 || Q === u)
                                                 continue;
                                             const ye = typeof he == "string" ? he : null,
-                                                Me = document.querySelector(`[data-element-id="${Z}"]`);
+                                                Me = document.querySelector(`[data-element-id="${Q}"]`);
                                             if (Me && !T.has(Me)) {
-                                                (0, n.warn)(`_getElementsByName - element not allowed: ${Z}`);
+                                                (0, n.warn)(`_getElementsByName - element not allowed: ${Q}`);
                                                 continue;
                                             }
                                             L.push({
-                                                id: Z,
+                                                id: Q,
                                                 exportValue: ye,
                                                 domElement: Me
                                             });
                                         }
                                     return L;
                                 }
                                 for (const j of document.getElementsByName(U)) {
                                     const {
                                         exportValue: V
-                                    } = j, Z = j.getAttribute("data-element-id");
-                                    Z !== u && T.has(j) && L.push({
-                                        id: Z,
+                                    } = j, Q = j.getAttribute("data-element-id");
+                                    Q !== u && T.has(j) && L.push({
+                                        id: Q,
                                         exportValue: V,
                                         domElement: j
                                     });
                                 }
                                 return L;
                             }
                             show() {
@@ -18628,16 +18628,16 @@
                                 u.href = this.linkService.getAnchorUrl("");
                                 const j = /* @__PURE__ */ new Map([
                                     ["Action", "onclick"],
                                     ["Mouse Up", "onmouseup"],
                                     ["Mouse Down", "onmousedown"]
                                 ]);
                                 for (const V of Object.keys(L.actions)) {
-                                    const Z = j.get(V);
-                                    Z && (u[Z] = () => {
+                                    const Q = j.get(V);
+                                    Q && (u[Q] = () => {
                                         var he;
                                         return (he = this.linkService.eventBus) == null || he.dispatch("dispatcheventinsandbox", {
                                             source: this,
                                             detail: {
                                                 id: L.id,
                                                 name: V
                                             }
@@ -18653,30 +18653,30 @@
                                     return;
                                 }
                                 u.onclick = () => {
                                     var qe;
                                     j == null || j();
                                     const {
                                         fields: V,
-                                        refs: Z,
+                                        refs: Q,
                                         include: he
                                     } = L, ye = [];
-                                    if (V.length !== 0 || Z.length !== 0) {
-                                        const Ie = new Set(Z);
+                                    if (V.length !== 0 || Q.length !== 0) {
+                                        const Ie = new Set(Q);
                                         for (const Le of V) {
-                                            const He = this._fieldObjects[Le] || [];
+                                            const Ue = this._fieldObjects[Le] || [];
                                             for (const {
                                                     id: Ve
                                                 }
-                                                of He)
+                                                of Ue)
                                                 Ie.add(Ve);
                                         }
                                         for (const Le of Object.values(this._fieldObjects))
-                                            for (const He of Le)
-                                                Ie.has(He.id) === he && ye.push(He);
+                                            for (const Ue of Le)
+                                                Ie.has(Ue.id) === he && ye.push(Ue);
                                     } else
                                         for (const Ie of Object.values(this._fieldObjects))
                                             ye.push(...Ie);
                                     const Me = this.annotationStorage,
                                         Re = [];
                                     for (const Ie of ye) {
                                         const {
@@ -18705,23 +18705,23 @@
                                                     value: Ve
                                                 });
                                                 break;
                                             }
                                             default:
                                                 continue;
                                         }
-                                        const He = document.querySelector(`[data-element-id="${Le}"]`);
-                                        if (He) {
-                                            if (!T.has(He)) {
+                                        const Ue = document.querySelector(`[data-element-id="${Le}"]`);
+                                        if (Ue) {
+                                            if (!T.has(Ue)) {
                                                 (0, n.warn)(`_bindResetFormAction - element not allowed: ${Le}`);
                                                 continue;
                                             }
                                         } else
                                             continue;
-                                        He.dispatchEvent(new Event("resetform"));
+                                        Ue.dispatchEvent(new Event("resetform"));
                                     }
                                     return this.enableScripting && ((qe = this.linkService.eventBus) == null || qe.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: "app",
                                             ids: Re,
                                             name: "ResetForm"
@@ -18761,113 +18761,113 @@
                                 const {
                                     isWin: u,
                                     isMac: L
                                 } = n.FeatureTest.platform;
                                 return u && U.ctrlKey || L && U.metaKey;
                             }
                             _setEventListener(U, u, L, j, V) {
-                                L.includes("mouse") ? U.addEventListener(L, (Z) => {
+                                L.includes("mouse") ? U.addEventListener(L, (Q) => {
                                     var he;
                                     (he = this.linkService.eventBus) == null || he.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: this.data.id,
                                             name: j,
-                                            value: V(Z),
-                                            shift: Z.shiftKey,
-                                            modifier: this._getKeyModifier(Z)
+                                            value: V(Q),
+                                            shift: Q.shiftKey,
+                                            modifier: this._getKeyModifier(Q)
                                         }
                                     });
-                                }) : U.addEventListener(L, (Z) => {
+                                }) : U.addEventListener(L, (Q) => {
                                     var he;
                                     if (L === "blur") {
-                                        if (!u.focused || !Z.relatedTarget)
+                                        if (!u.focused || !Q.relatedTarget)
                                             return;
                                         u.focused = !1;
                                     } else if (L === "focus") {
                                         if (u.focused)
                                             return;
                                         u.focused = !0;
                                     }
                                     V && ((he = this.linkService.eventBus) == null || he.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: this.data.id,
                                             name: j,
-                                            value: V(Z)
+                                            value: V(Q)
                                         }
                                     }));
                                 });
                             }
                             _setEventListeners(U, u, L, j) {
-                                var V, Z, he;
+                                var V, Q, he;
                                 for (const [ye, Me] of L)
                                     (Me === "Action" || (V = this.data.actions) != null && V[Me]) && ((Me === "Focus" || Me === "Blur") && (u || (u = {
                                         focused: !1
-                                    })), this._setEventListener(U, u, ye, Me, j), Me === "Focus" && !((Z = this.data.actions) != null && Z.Blur) ? this._setEventListener(U, u, "blur", "Blur", null) : Me === "Blur" && !((he = this.data.actions) != null && he.Focus) && this._setEventListener(U, u, "focus", "Focus", null));
+                                    })), this._setEventListener(U, u, ye, Me, j), Me === "Focus" && !((Q = this.data.actions) != null && Q.Blur) ? this._setEventListener(U, u, "blur", "Blur", null) : Me === "Blur" && !((he = this.data.actions) != null && he.Focus) && this._setEventListener(U, u, "focus", "Focus", null));
                             }
                             _setBackgroundColor(U) {
                                 const u = this.data.backgroundColor || null;
                                 U.style.backgroundColor = u === null ? "transparent" : n.Util.makeHexColor(u[0], u[1], u[2]);
                             }
                             _setTextStyle(U) {
                                 const u = ["left", "center", "right"],
                                     {
                                         fontColor: L
                                     } = this.data.defaultAppearanceData,
                                     j = this.data.defaultAppearanceData.fontSize || r,
                                     V = U.style;
-                                let Z;
+                                let Q;
                                 const he = 2,
                                     ye = (Me) => Math.round(10 * Me) / 10;
                                 if (this.data.multiLine) {
                                     const Me = Math.abs(this.data.rect[3] - this.data.rect[1] - he),
                                         Re = Math.round(Me / (n.LINE_FACTOR * j)) || 1,
                                         qe = Me / Re;
-                                    Z = Math.min(j, ye(qe / n.LINE_FACTOR));
+                                    Q = Math.min(j, ye(qe / n.LINE_FACTOR));
                                 } else {
                                     const Me = Math.abs(this.data.rect[3] - this.data.rect[1] - he);
-                                    Z = Math.min(j, ye(Me / n.LINE_FACTOR));
+                                    Q = Math.min(j, ye(Me / n.LINE_FACTOR));
                                 }
-                                V.fontSize = `calc(${Z}px * var(--scale-factor))`, V.color = n.Util.makeHexColor(L[0], L[1], L[2]), this.data.textAlignment !== null && (V.textAlign = u[this.data.textAlignment]);
+                                V.fontSize = `calc(${Q}px * var(--scale-factor))`, V.color = n.Util.makeHexColor(L[0], L[1], L[2]), this.data.textAlignment !== null && (V.textAlign = u[this.data.textAlignment]);
                             }
                             _setRequired(U, u) {
                                 u ? U.setAttribute("required", !0) : U.removeAttribute("required"), U.setAttribute("aria-required", u);
                             }
                         }
                         class F extends k {
                             constructor(U) {
                                 const u = U.renderForms || !U.data.hasAppearance && !!U.data.fieldValue;
                                 super(U, {
                                     isRenderable: u
                                 });
                             }
                             setPropertyOnSiblings(U, u, L, j) {
                                 const V = this.annotationStorage;
-                                for (const Z of this._getElementsByName(U.name, U.id))
-                                    Z.domElement && (Z.domElement[u] = L), V.setValue(Z.id, {
+                                for (const Q of this._getElementsByName(U.name, U.id))
+                                    Q.domElement && (Q.domElement[u] = L), V.setValue(Q.id, {
                                         [j]: L
                                     });
                             }
                             render() {
                                 var j, V;
                                 const U = this.annotationStorage,
                                     u = this.data.id;
                                 this.container.classList.add("textWidgetAnnotation");
                                 let L = null;
                                 if (this.renderForms) {
-                                    const Z = U.getValue(u, {
+                                    const Q = U.getValue(u, {
                                         value: this.data.fieldValue
                                     });
-                                    let he = Z.value || "";
+                                    let he = Q.value || "";
                                     const ye = U.getValue(u, {
                                         charLimit: this.data.maxLen
                                     }).charLimit;
                                     ye && he.length > ye && (he = he.slice(0, ye));
-                                    let Me = Z.formattedValue || ((j = this.data.textContent) == null ? void 0 : j.join(`
+                                    let Me = Q.formattedValue || ((j = this.data.textContent) == null ? void 0 : j.join(`
 `)) || null;
                                     Me && this.data.comb && (Me = Me.replaceAll(/\s+/g, ""));
                                     const Re = {
                                         userValue: he,
                                         formattedValue: Me,
                                         lastCommittedValue: null,
                                         commitKey: 1,
@@ -18888,20 +18888,20 @@
                                         Le != null && (Ie.target.value = Le), Ie.target.scrollLeft = 0;
                                     };
                                     if (this.enableScripting && this.hasJSActions) {
                                         L.addEventListener("focus", (Le) => {
                                             if (Re.focused)
                                                 return;
                                             const {
-                                                target: He
+                                                target: Ue
                                             } = Le;
-                                            Re.userValue && (He.value = Re.userValue), Re.lastCommittedValue = He.value, Re.commitKey = 1, Re.focused = !0;
+                                            Re.userValue && (Ue.value = Re.userValue), Re.lastCommittedValue = Ue.value, Re.commitKey = 1, Re.focused = !0;
                                         }), L.addEventListener("updatefromsandbox", (Le) => {
                                             this.showElementAndHideCanvas(Le.target);
-                                            const He = {
+                                            const Ue = {
                                                 value(Ve) {
                                                     Re.userValue = Ve.detail.value ?? "", U.setValue(u, {
                                                         value: Re.userValue.toString()
                                                     }), Ve.target.value = Re.userValue;
                                                 },
                                                 formattedValue(Ve) {
                                                     const {
@@ -18915,120 +18915,120 @@
                                                     Ve.target.setSelectionRange(...Ve.detail.selRange);
                                                 },
                                                 charLimit: (Ve) => {
                                                     var it;
                                                     const {
                                                         charLimit: Je
                                                     } = Ve.detail, {
-                                                        target: Ze
+                                                        target: Qe
                                                     } = Ve;
                                                     if (Je === 0) {
-                                                        Ze.removeAttribute("maxLength");
+                                                        Qe.removeAttribute("maxLength");
                                                         return;
                                                     }
-                                                    Ze.setAttribute("maxLength", Je);
+                                                    Qe.setAttribute("maxLength", Je);
                                                     let st = Re.userValue;
-                                                    !st || st.length <= Je || (st = st.slice(0, Je), Ze.value = Re.userValue = st, U.setValue(u, {
+                                                    !st || st.length <= Je || (st = st.slice(0, Je), Qe.value = Re.userValue = st, U.setValue(u, {
                                                         value: st
                                                     }), (it = this.linkService.eventBus) == null || it.dispatch("dispatcheventinsandbox", {
                                                         source: this,
                                                         detail: {
                                                             id: u,
                                                             name: "Keystroke",
                                                             value: st,
                                                             willCommit: !0,
                                                             commitKey: 1,
-                                                            selStart: Ze.selectionStart,
-                                                            selEnd: Ze.selectionEnd
+                                                            selStart: Qe.selectionStart,
+                                                            selEnd: Qe.selectionEnd
                                                         }
                                                     }));
                                                 }
                                             };
-                                            this._dispatchEventFromSandbox(He, Le);
+                                            this._dispatchEventFromSandbox(Ue, Le);
                                         }), L.addEventListener("keydown", (Le) => {
                                             var Je;
                                             Re.commitKey = 1;
-                                            let He = -1;
-                                            if (Le.key === "Escape" ? He = 0 : Le.key === "Enter" && !this.data.multiLine ? He = 2 : Le.key === "Tab" && (Re.commitKey = 3), He === -1)
+                                            let Ue = -1;
+                                            if (Le.key === "Escape" ? Ue = 0 : Le.key === "Enter" && !this.data.multiLine ? Ue = 2 : Le.key === "Tab" && (Re.commitKey = 3), Ue === -1)
                                                 return;
                                             const {
                                                 value: Ve
                                             } = Le.target;
                                             Re.lastCommittedValue !== Ve && (Re.lastCommittedValue = Ve, Re.userValue = Ve, (Je = this.linkService.eventBus) == null || Je.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: u,
                                                     name: "Keystroke",
                                                     value: Ve,
                                                     willCommit: !0,
-                                                    commitKey: He,
+                                                    commitKey: Ue,
                                                     selStart: Le.target.selectionStart,
                                                     selEnd: Le.target.selectionEnd
                                                 }
                                             }));
                                         });
                                         const Ie = qe;
                                         qe = null, L.addEventListener("blur", (Le) => {
                                             var Ve;
                                             if (!Re.focused || !Le.relatedTarget)
                                                 return;
                                             Re.focused = !1;
                                             const {
-                                                value: He
+                                                value: Ue
                                             } = Le.target;
-                                            Re.userValue = He, Re.lastCommittedValue !== He && ((Ve = this.linkService.eventBus) == null || Ve.dispatch("dispatcheventinsandbox", {
+                                            Re.userValue = Ue, Re.lastCommittedValue !== Ue && ((Ve = this.linkService.eventBus) == null || Ve.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: u,
                                                     name: "Keystroke",
-                                                    value: He,
+                                                    value: Ue,
                                                     willCommit: !0,
                                                     commitKey: Re.commitKey,
                                                     selStart: Le.target.selectionStart,
                                                     selEnd: Le.target.selectionEnd
                                                 }
                                             })), Ie(Le);
                                         }), (V = this.data.actions) != null && V.Keystroke && L.addEventListener("beforeinput", (Le) => {
                                             var lt;
                                             Re.lastCommittedValue = null;
                                             const {
-                                                data: He,
+                                                data: Ue,
                                                 target: Ve
                                             } = Le, {
                                                 value: Je,
-                                                selectionStart: Ze,
+                                                selectionStart: Qe,
                                                 selectionEnd: st
                                             } = Ve;
-                                            let it = Ze,
+                                            let it = Qe,
                                                 rt = st;
                                             switch (Le.inputType) {
                                                 case "deleteWordBackward": {
-                                                    const ct = Je.substring(0, Ze).match(/\w*[^\w]*$/);
+                                                    const ct = Je.substring(0, Qe).match(/\w*[^\w]*$/);
                                                     ct && (it -= ct[0].length);
                                                     break;
                                                 }
                                                 case "deleteWordForward": {
-                                                    const ct = Je.substring(Ze).match(/^[^\w]*\w*/);
+                                                    const ct = Je.substring(Qe).match(/^[^\w]*\w*/);
                                                     ct && (rt += ct[0].length);
                                                     break;
                                                 }
                                                 case "deleteContentBackward":
-                                                    Ze === st && (it -= 1);
+                                                    Qe === st && (it -= 1);
                                                     break;
                                                 case "deleteContentForward":
-                                                    Ze === st && (rt += 1);
+                                                    Qe === st && (rt += 1);
                                                     break;
                                             }
                                             Le.preventDefault(), (lt = this.linkService.eventBus) == null || lt.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: u,
                                                     name: "Keystroke",
                                                     value: Je,
-                                                    change: He || "",
+                                                    change: Ue || "",
                                                     willCommit: !1,
                                                     selStart: it,
                                                     selEnd: rt
                                                 }
                                             });
                                         }), this._setEventListeners(L, Re, [
                                             ["focus", "Focus"],
@@ -19068,50 +19068,50 @@
                                 let j = U.getValue(L, {
                                     value: u.exportValue === u.fieldValue
                                 }).value;
                                 typeof j == "string" && (j = j !== "Off", U.setValue(L, {
                                     value: j
                                 })), this.container.classList.add("buttonWidgetAnnotation", "checkBox");
                                 const V = document.createElement("input");
-                                return T.add(V), V.setAttribute("data-element-id", L), V.disabled = u.readOnly, this._setRequired(V, this.data.required), V.type = "checkbox", V.name = u.fieldName, j && V.setAttribute("checked", !0), V.setAttribute("exportValue", u.exportValue), V.tabIndex = o, V.addEventListener("change", (Z) => {
+                                return T.add(V), V.setAttribute("data-element-id", L), V.disabled = u.readOnly, this._setRequired(V, this.data.required), V.type = "checkbox", V.name = u.fieldName, j && V.setAttribute("checked", !0), V.setAttribute("exportValue", u.exportValue), V.tabIndex = o, V.addEventListener("change", (Q) => {
                                     const {
                                         name: he,
                                         checked: ye
-                                    } = Z.target;
+                                    } = Q.target;
                                     for (const Me of this._getElementsByName(he, L)) {
                                         const Re = ye && Me.exportValue === u.exportValue;
                                         Me.domElement && (Me.domElement.checked = Re), U.setValue(Me.id, {
                                             value: Re
                                         });
                                     }
                                     U.setValue(L, {
                                         value: ye
                                     });
-                                }), V.addEventListener("resetform", (Z) => {
+                                }), V.addEventListener("resetform", (Q) => {
                                     const he = u.defaultFieldValue || "Off";
-                                    Z.target.checked = he === u.exportValue;
-                                }), this.enableScripting && this.hasJSActions && (V.addEventListener("updatefromsandbox", (Z) => {
+                                    Q.target.checked = he === u.exportValue;
+                                }), this.enableScripting && this.hasJSActions && (V.addEventListener("updatefromsandbox", (Q) => {
                                     const he = {
                                         value(ye) {
                                             ye.target.checked = ye.detail.value !== "Off", U.setValue(L, {
                                                 value: ye.target.checked
                                             });
                                         }
                                     };
-                                    this._dispatchEventFromSandbox(he, Z);
+                                    this._dispatchEventFromSandbox(he, Q);
                                 }), this._setEventListeners(V, null, [
                                     ["change", "Validate"],
                                     ["change", "Action"],
                                     ["focus", "Focus"],
                                     ["blur", "Blur"],
                                     ["mousedown", "Mouse Down"],
                                     ["mouseenter", "Mouse Enter"],
                                     ["mouseleave", "Mouse Exit"],
                                     ["mouseup", "Mouse Up"]
-                                ], (Z) => Z.target.checked)), this._setBackgroundColor(V), this._setDefaultPropertiesFromJS(V), this.container.append(V), this.container;
+                                ], (Q) => Q.target.checked)), this._setBackgroundColor(V), this._setDefaultPropertiesFromJS(V), this.container.append(V), this.container;
                             }
                         }
                         class p extends k {
                             constructor(U) {
                                 super(U, {
                                     isRenderable: U.renderForms
                                 });
@@ -19124,35 +19124,35 @@
                                 let j = U.getValue(L, {
                                     value: u.fieldValue === u.buttonValue
                                 }).value;
                                 typeof j == "string" && (j = j !== u.buttonValue, U.setValue(L, {
                                     value: j
                                 }));
                                 const V = document.createElement("input");
-                                if (T.add(V), V.setAttribute("data-element-id", L), V.disabled = u.readOnly, this._setRequired(V, this.data.required), V.type = "radio", V.name = u.fieldName, j && V.setAttribute("checked", !0), V.tabIndex = o, V.addEventListener("change", (Z) => {
+                                if (T.add(V), V.setAttribute("data-element-id", L), V.disabled = u.readOnly, this._setRequired(V, this.data.required), V.type = "radio", V.name = u.fieldName, j && V.setAttribute("checked", !0), V.tabIndex = o, V.addEventListener("change", (Q) => {
                                         const {
                                             name: he,
                                             checked: ye
-                                        } = Z.target;
+                                        } = Q.target;
                                         for (const Me of this._getElementsByName(he, L))
                                             U.setValue(Me.id, {
                                                 value: !1
                                             });
                                         U.setValue(L, {
                                             value: ye
                                         });
-                                    }), V.addEventListener("resetform", (Z) => {
+                                    }), V.addEventListener("resetform", (Q) => {
                                         const he = u.defaultFieldValue;
-                                        Z.target.checked = he != null && he === u.buttonValue;
+                                        Q.target.checked = he != null && he === u.buttonValue;
                                     }), this.enableScripting && this.hasJSActions) {
-                                    const Z = u.buttonValue;
+                                    const Q = u.buttonValue;
                                     V.addEventListener("updatefromsandbox", (he) => {
                                         const ye = {
                                             value: (Me) => {
-                                                const Re = Z === Me.detail.value;
+                                                const Re = Q === Me.detail.value;
                                                 for (const qe of this._getElementsByName(Me.target.name)) {
                                                     const Ie = Re && qe.id === L;
                                                     qe.domElement && (qe.domElement.checked = Ie), U.setValue(qe.id, {
                                                         value: Ie
                                                     });
                                                 }
                                             }
@@ -19208,56 +19208,56 @@
                                     for (const Ie of j.options)
                                         Ie.selected = Ie.value === qe;
                                 });
                                 for (const Re of this.data.options) {
                                     const qe = document.createElement("option");
                                     qe.textContent = Re.displayValue, qe.value = Re.exportValue, L.value.includes(Re.exportValue) && (qe.setAttribute("selected", !0), V = !1), j.append(qe);
                                 }
-                                let Z = null;
+                                let Q = null;
                                 if (V) {
                                     const Re = document.createElement("option");
-                                    Re.value = " ", Re.setAttribute("hidden", !0), Re.setAttribute("selected", !0), j.prepend(Re), Z = () => {
-                                        Re.remove(), j.removeEventListener("input", Z), Z = null;
-                                    }, j.addEventListener("input", Z);
+                                    Re.value = " ", Re.setAttribute("hidden", !0), Re.setAttribute("selected", !0), j.prepend(Re), Q = () => {
+                                        Re.remove(), j.removeEventListener("input", Q), Q = null;
+                                    }, j.addEventListener("input", Q);
                                 }
                                 const he = (Re) => {
                                     const qe = Re ? "value" : "textContent",
                                         {
                                             options: Ie,
                                             multiple: Le
                                         } = j;
-                                    return Le ? Array.prototype.filter.call(Ie, (He) => He.selected).map((He) => He[qe]) : Ie.selectedIndex === -1 ? null : Ie[Ie.selectedIndex][qe];
+                                    return Le ? Array.prototype.filter.call(Ie, (Ue) => Ue.selected).map((Ue) => Ue[qe]) : Ie.selectedIndex === -1 ? null : Ie[Ie.selectedIndex][qe];
                                 };
                                 let ye = he(!1);
                                 const Me = (Re) => {
                                     const qe = Re.target.options;
                                     return Array.prototype.map.call(qe, (Ie) => ({
                                         displayValue: Ie.textContent,
                                         exportValue: Ie.value
                                     }));
                                 };
                                 return this.enableScripting && this.hasJSActions ? (j.addEventListener("updatefromsandbox", (Re) => {
                                     const qe = {
                                         value(Ie) {
-                                            Z == null || Z();
+                                            Q == null || Q();
                                             const Le = Ie.detail.value,
-                                                He = new Set(Array.isArray(Le) ? Le : [Le]);
+                                                Ue = new Set(Array.isArray(Le) ? Le : [Le]);
                                             for (const Ve of j.options)
-                                                Ve.selected = He.has(Ve.value);
+                                                Ve.selected = Ue.has(Ve.value);
                                             U.setValue(u, {
                                                 value: he(!0)
                                             }), ye = he(!1);
                                         },
                                         multipleSelection(Ie) {
                                             j.multiple = !0;
                                         },
                                         remove(Ie) {
                                             const Le = j.options,
-                                                He = Ie.detail.remove;
-                                            Le[He].selected = !1, j.remove(He), Le.length > 0 && Array.prototype.findIndex.call(Le, (Je) => Je.selected) === -1 && (Le[0].selected = !0), U.setValue(u, {
+                                                Ue = Ie.detail.remove;
+                                            Le[Ue].selected = !1, j.remove(Ue), Le.length > 0 && Array.prototype.findIndex.call(Le, (Je) => Je.selected) === -1 && (Le[0].selected = !0), U.setValue(u, {
                                                 value: he(!0),
                                                 items: Me(Ie)
                                             }), ye = he(!1);
                                         },
                                         clear(Ie) {
                                             for (; j.length !== 0;)
                                                 j.remove(0);
@@ -19265,44 +19265,44 @@
                                                 value: null,
                                                 items: []
                                             }), ye = he(!1);
                                         },
                                         insert(Ie) {
                                             const {
                                                 index: Le,
-                                                displayValue: He,
+                                                displayValue: Ue,
                                                 exportValue: Ve
-                                            } = Ie.detail.insert, Je = j.children[Le], Ze = document.createElement("option");
-                                            Ze.textContent = He, Ze.value = Ve, Je ? Je.before(Ze) : j.append(Ze), U.setValue(u, {
+                                            } = Ie.detail.insert, Je = j.children[Le], Qe = document.createElement("option");
+                                            Qe.textContent = Ue, Qe.value = Ve, Je ? Je.before(Qe) : j.append(Qe), U.setValue(u, {
                                                 value: he(!0),
                                                 items: Me(Ie)
                                             }), ye = he(!1);
                                         },
                                         items(Ie) {
                                             const {
                                                 items: Le
                                             } = Ie.detail;
                                             for (; j.length !== 0;)
                                                 j.remove(0);
-                                            for (const He of Le) {
+                                            for (const Ue of Le) {
                                                 const {
                                                     displayValue: Ve,
                                                     exportValue: Je
-                                                } = He, Ze = document.createElement("option");
-                                                Ze.textContent = Ve, Ze.value = Je, j.append(Ze);
+                                                } = Ue, Qe = document.createElement("option");
+                                                Qe.textContent = Ve, Qe.value = Je, j.append(Qe);
                                             }
                                             j.options.length > 0 && (j.options[0].selected = !0), U.setValue(u, {
                                                 value: he(!0),
                                                 items: Me(Ie)
                                             }), ye = he(!1);
                                         },
                                         indices(Ie) {
                                             const Le = new Set(Ie.detail.indices);
-                                            for (const He of Ie.target.options)
-                                                He.selected = Le.has(He.index);
+                                            for (const Ue of Ie.target.options)
+                                                Ue.selected = Le.has(Ue.index);
                                             U.setValue(u, {
                                                 value: he(!0)
                                             }), ye = he(!1);
                                         },
                                         editable(Ie) {
                                             Ie.target.disabled = !Ie.detail.editable;
                                         }
@@ -19375,28 +19375,28 @@
                         class m {
                             constructor({
                                 container: U,
                                 color: u,
                                 elements: L,
                                 titleObj: j,
                                 modificationDate: V,
-                                contentsObj: Z,
+                                contentsObj: Q,
                                 richText: he,
                                 parent: ye,
                                 rect: Me,
                                 parentRect: Re,
                                 open: qe
                             }) {
-                                W(this, Ue);
+                                W(this, He);
                                 W(this, je);
                                 W(this, Xe);
                                 W(this, Ye);
                                 W(this, z, null);
-                                W(this, ae, K(this, Ue, $n).bind(this));
-                                W(this, Q, K(this, Ye, cn).bind(this));
+                                W(this, ae, K(this, He, $n).bind(this));
+                                W(this, Z, K(this, Ye, cn).bind(this));
                                 W(this, ce, K(this, Xe, ln).bind(this));
                                 W(this, ue, K(this, je, Mt).bind(this));
                                 W(this, me, null);
                                 W(this, fe, null);
                                 W(this, Pe, null);
                                 W(this, Fe, null);
                                 W(this, Ee, null);
@@ -19404,24 +19404,24 @@
                                 W(this, _e, !1);
                                 W(this, ie, null);
                                 W(this, se, null);
                                 W(this, ge, null);
                                 W(this, Ce, null);
                                 W(this, xe, !1);
                                 var Le;
-                                oe(this, fe, U), oe(this, Ce, j), oe(this, Pe, Z), oe(this, ge, he), oe(this, Ee, ye), oe(this, me, u), oe(this, se, Me), oe(this, De, Re), oe(this, Fe, L);
+                                oe(this, fe, U), oe(this, Ce, j), oe(this, Pe, Q), oe(this, ge, he), oe(this, Ee, ye), oe(this, me, u), oe(this, se, Me), oe(this, De, Re), oe(this, Fe, L);
                                 const Ie = s.PDFDateString.toDateObject(V);
                                 Ie && oe(this, z, ye.l10n.get("annotation_date_string", {
                                     date: Ie.toLocaleDateString(),
                                     time: Ie.toLocaleTimeString()
-                                })), this.trigger = L.flatMap((He) => He.getElementsToTriggerPopup());
-                                for (const He of this.trigger)
-                                    He.addEventListener("click", a(this, ue)), He.addEventListener("mouseenter", a(this, ce)), He.addEventListener("mouseleave", a(this, Q)), He.classList.add("popupTriggerArea");
-                                for (const He of L)
-                                    (Le = He.container) == null || Le.addEventListener("keydown", a(this, ae));
+                                })), this.trigger = L.flatMap((Ue) => Ue.getElementsToTriggerPopup());
+                                for (const Ue of this.trigger)
+                                    Ue.addEventListener("click", a(this, ue)), Ue.addEventListener("mouseenter", a(this, ce)), Ue.addEventListener("mouseleave", a(this, Z)), Ue.classList.add("popupTriggerArea");
+                                for (const Ue of L)
+                                    (Le = Ue.container) == null || Le.addEventListener("keydown", a(this, ae));
                                 a(this, fe).hidden = !0, qe && K(this, je, Mt).call(this);
                             }
                             render() {
                                 if (a(this, ie))
                                     return;
                                 const {
                                     page: {
@@ -19431,84 +19431,83 @@
                                         rawDims: {
                                             pageWidth: u,
                                             pageHeight: L,
                                             pageX: j,
                                             pageY: V
                                         }
                                     }
-                                } = a(this, Ee), Z = oe(this, ie, document.createElement("div"));
-                                if (Z.className = "popup", a(this, me)) {
-                                    const it = Z.style.outlineColor = n.Util.makeHexColor(...a(this, me));
-                                    CSS.supports("background-color", "color-mix(in srgb, red 30%, white)") ? Z.style.backgroundColor = `color-mix(in srgb, ${it} 30%, white)` : Z.style.backgroundColor = n.Util.makeHexColor(...a(this, me).map((lt) => Math.floor(0.7 * (255 - lt) + lt)));
+                                } = a(this, Ee), Q = oe(this, ie, document.createElement("div"));
+                                if (Q.className = "popup", a(this, me)) {
+                                    const it = Q.style.outlineColor = n.Util.makeHexColor(...a(this, me));
+                                    CSS.supports("background-color", "color-mix(in srgb, red 30%, white)") ? Q.style.backgroundColor = `color-mix(in srgb, ${it} 30%, white)` : Q.style.backgroundColor = n.Util.makeHexColor(...a(this, me).map((lt) => Math.floor(0.7 * (255 - lt) + lt)));
                                 }
                                 const he = document.createElement("span");
                                 he.className = "header";
                                 const ye = document.createElement("h1");
                                 if (he.append(ye), {
                                         dir: ye.dir,
                                         str: ye.textContent
-                                    } = a(this, Ce), Z.append(he), a(this, z)) {
+                                    } = a(this, Ce), Q.append(he), a(this, z)) {
                                     const it = document.createElement("span");
                                     it.classList.add("popupDate"), a(this, z).then((rt) => {
                                         it.textContent = rt;
                                     }), he.append(it);
                                 }
                                 const Me = a(this, Pe),
                                     Re = a(this, ge);
                                 if (Re != null && Re.str && (!(Me != null && Me.str) || Me.str === Re.str))
                                     c.XfaLayer.render({
                                         xfaHtml: Re.html,
                                         intent: "richText",
-                                        div: Z
-                                    }), Z.lastChild.classList.add("richText", "popupContent");
+                                        div: Q
+                                    }), Q.lastChild.classList.add("richText", "popupContent");
                                 else {
                                     const it = this._formatContents(Me);
-                                    Z.append(it);
+                                    Q.append(it);
                                 }
                                 let qe = !!a(this, De),
                                     Ie = qe ? a(this, De) : a(this, se);
                                 for (const it of a(this, Fe))
                                     if (!Ie || n.Util.intersect(it.data.rect, Ie) !== null) {
                                         Ie = it.data.rect, qe = !0;
                                         break;
                                     }
                                 const Le = n.Util.normalizeRect([Ie[0], U[3] - Ie[1] + U[1], Ie[2], U[3] - Ie[3] + U[1]]),
-                                    He = 5,
-                                    Ve = qe ? Ie[2] - Ie[0] + He : 0,
+                                    Ve = qe ? Ie[2] - Ie[0] + 5 : 0,
                                     Je = Le[0] + Ve,
-                                    Ze = Le[1],
+                                    Qe = Le[1],
                                     {
                                         style: st
                                     } = a(this, fe);
-                                st.left = `${100 * (Je - j) / u}%`, st.top = `${100 * (Ze - V) / L}%`, a(this, fe).append(Z);
+                                st.left = `${100 * (Je - j) / u}%`, st.top = `${100 * (Qe - V) / L}%`, a(this, fe).append(Q);
                             }
                             _formatContents({
                                 str: U,
                                 dir: u
                             }) {
                                 const L = document.createElement("p");
                                 L.classList.add("popupContent"), L.dir = u;
                                 const j = U.split(/(?:\r\n?|\n)/);
-                                for (let V = 0, Z = j.length; V < Z; ++V) {
+                                for (let V = 0, Q = j.length; V < Q; ++V) {
                                     const he = j[V];
-                                    L.append(document.createTextNode(he)), V < Z - 1 && L.append(document.createElement("br"));
+                                    L.append(document.createTextNode(he)), V < Q - 1 && L.append(document.createElement("br"));
                                 }
                                 return L;
                             }
                             forceHide() {
                                 oe(this, xe, this.isVisible), a(this, xe) && (a(this, fe).hidden = !0);
                             }
                             maybeShow() {
                                 a(this, xe) && (oe(this, xe, !1), a(this, fe).hidden = !1);
                             }
                             get isVisible() {
                                 return a(this, fe).hidden === !1;
                             }
                         }
-                        z = new WeakMap(), ae = new WeakMap(), Q = new WeakMap(), ce = new WeakMap(), ue = new WeakMap(), me = new WeakMap(), fe = new WeakMap(), Pe = new WeakMap(), Fe = new WeakMap(), Ee = new WeakMap(), De = new WeakMap(), _e = new WeakMap(), ie = new WeakMap(), se = new WeakMap(), ge = new WeakMap(), Ce = new WeakMap(), xe = new WeakMap(), Ue = new WeakSet(), $n = function(U) {
+                        z = new WeakMap(), ae = new WeakMap(), Z = new WeakMap(), ce = new WeakMap(), ue = new WeakMap(), me = new WeakMap(), fe = new WeakMap(), Pe = new WeakMap(), Fe = new WeakMap(), Ee = new WeakMap(), De = new WeakMap(), _e = new WeakMap(), ie = new WeakMap(), se = new WeakMap(), ge = new WeakMap(), Ce = new WeakMap(), xe = new WeakMap(), He = new WeakSet(), $n = function(U) {
                             U.altKey || U.shiftKey || U.ctrlKey || U.metaKey || (U.key === "Enter" || U.key === "Escape" && a(this, _e)) && K(this, je, Mt).call(this);
                         }, je = new WeakSet(), Mt = function() {
                             oe(this, _e, !a(this, _e)), a(this, _e) ? (K(this, Xe, ln).call(this), a(this, fe).addEventListener("click", a(this, ue)), a(this, fe).addEventListener("keydown", a(this, ae))) : (K(this, Ye, cn).call(this), a(this, fe).removeEventListener("click", a(this, ue)), a(this, fe).removeEventListener("keydown", a(this, ae)));
                         }, Xe = new WeakSet(), ln = function() {
                             a(this, ie) || this.render(), this.isVisible ? a(this, _e) && a(this, fe).classList.add("focused") : (a(this, fe).hidden = !1, a(this, fe).style.zIndex = parseInt(a(this, fe).style.zIndex) + 1e3);
                         }, Ye = new WeakSet(), cn = function() {
                             a(this, fe).classList.remove("focused"), !(a(this, _e) || !this.isVisible) && (a(this, fe).hidden = !0, a(this, fe).style.zIndex = parseInt(a(this, fe).style.zIndex) - 1e3);
@@ -19546,16 +19545,16 @@
                                 this.container.classList.add("lineAnnotation");
                                 const u = this.data,
                                     {
                                         width: L,
                                         height: j
                                     } = S(u.rect),
                                     V = this.svgFactory.create(L, j, !0),
-                                    Z = oe(this, ne, this.svgFactory.createElement("svg:line"));
-                                return Z.setAttribute("x1", u.rect[2] - u.lineCoordinates[0]), Z.setAttribute("y1", u.rect[3] - u.lineCoordinates[1]), Z.setAttribute("x2", u.rect[2] - u.lineCoordinates[2]), Z.setAttribute("y2", u.rect[3] - u.lineCoordinates[3]), Z.setAttribute("stroke-width", u.borderStyle.width || 1), Z.setAttribute("stroke", "transparent"), Z.setAttribute("fill", "transparent"), V.append(Z), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                    Q = oe(this, ne, this.svgFactory.createElement("svg:line"));
+                                return Q.setAttribute("x1", u.rect[2] - u.lineCoordinates[0]), Q.setAttribute("y1", u.rect[3] - u.lineCoordinates[1]), Q.setAttribute("x2", u.rect[2] - u.lineCoordinates[2]), Q.setAttribute("y2", u.rect[3] - u.lineCoordinates[3]), Q.setAttribute("stroke-width", u.borderStyle.width || 1), Q.setAttribute("stroke", "transparent"), Q.setAttribute("fill", "transparent"), V.append(Q), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return a(this, ne);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -19573,17 +19572,17 @@
                                 this.container.classList.add("squareAnnotation");
                                 const u = this.data,
                                     {
                                         width: L,
                                         height: j
                                     } = S(u.rect),
                                     V = this.svgFactory.create(L, j, !0),
-                                    Z = u.borderStyle.width,
+                                    Q = u.borderStyle.width,
                                     he = oe(this, J, this.svgFactory.createElement("svg:rect"));
-                                return he.setAttribute("x", Z / 2), he.setAttribute("y", Z / 2), he.setAttribute("width", L - Z), he.setAttribute("height", j - Z), he.setAttribute("stroke-width", Z || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return he.setAttribute("x", Q / 2), he.setAttribute("y", Q / 2), he.setAttribute("width", L - Q), he.setAttribute("height", j - Q), he.setAttribute("stroke-width", Q || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return a(this, J);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -19601,17 +19600,17 @@
                                 this.container.classList.add("circleAnnotation");
                                 const u = this.data,
                                     {
                                         width: L,
                                         height: j
                                     } = S(u.rect),
                                     V = this.svgFactory.create(L, j, !0),
-                                    Z = u.borderStyle.width,
+                                    Q = u.borderStyle.width,
                                     he = oe(this, ve, this.svgFactory.createElement("svg:ellipse"));
-                                return he.setAttribute("cx", L / 2), he.setAttribute("cy", j / 2), he.setAttribute("rx", L / 2 - Z / 2), he.setAttribute("ry", j / 2 - Z / 2), he.setAttribute("stroke-width", Z || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return he.setAttribute("cx", L / 2), he.setAttribute("cy", j / 2), he.setAttribute("rx", L / 2 - Q / 2), he.setAttribute("ry", j / 2 - Q / 2), he.setAttribute("stroke-width", Q || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return a(this, ve);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -19630,23 +19629,23 @@
                                 this.container.classList.add(this.containerClassName);
                                 const u = this.data,
                                     {
                                         width: L,
                                         height: j
                                     } = S(u.rect),
                                     V = this.svgFactory.create(L, j, !0);
-                                let Z = [];
+                                let Q = [];
                                 for (const ye of u.vertices) {
                                     const Me = ye.x - u.rect[0],
                                         Re = u.rect[3] - ye.y;
-                                    Z.push(Me + "," + Re);
+                                    Q.push(Me + "," + Re);
                                 }
-                                Z = Z.join(" ");
+                                Q = Q.join(" ");
                                 const he = oe(this, Se, this.svgFactory.createElement(this.svgElementName));
-                                return he.setAttribute("points", Z), he.setAttribute("stroke-width", u.borderStyle.width || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
+                                return he.setAttribute("points", Q), he.setAttribute("stroke-width", u.borderStyle.width || 1), he.setAttribute("stroke", "transparent"), he.setAttribute("fill", "transparent"), V.append(he), this.container.append(V), !u.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
                             getElementsToTriggerPopup() {
                                 return a(this, Se);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
@@ -19681,17 +19680,17 @@
                                 this.container.classList.add(this.containerClassName);
                                 const u = this.data,
                                     {
                                         width: L,
                                         height: j
                                     } = S(u.rect),
                                     V = this.svgFactory.create(L, j, !0);
-                                for (const Z of u.inkLists) {
+                                for (const Q of u.inkLists) {
                                     let he = [];
-                                    for (const Me of Z) {
+                                    for (const Me of Q) {
                                         const Re = Me.x - u.rect[0],
                                             qe = u.rect[3] - Me.y;
                                         he.push(`${Re},${qe}`);
                                     }
                                     he = he.join(" ");
                                     const ye = this.svgFactory.createElement(this.svgElementName);
                                     a(this, tt).push(ye), ye.setAttribute("points", he), ye.setAttribute("stroke-width", u.borderStyle.width || 1), ye.setAttribute("stroke", "transparent"), ye.setAttribute("fill", "transparent"), !u.popupRef && this.hasPopupData && this._createPopup(), V.append(ye);
@@ -19791,16 +19790,16 @@
                                     data: L
                                 } = this;
                                 let j;
                                 L.hasAppearance || L.fillAlpha === 0 ? j = document.createElement("div") : (j = document.createElement("img"), j.src = `${this.imageResourcesPath}annotation-${/paperclip/i.test(L.name) ? "paperclip" : "pushpin"}.svg`, L.fillAlpha && L.fillAlpha < 1 && (j.style = `filter: opacity(${Math.round(L.fillAlpha * 100)}%);`)), j.addEventListener("dblclick", K(this, te, hn).bind(this)), oe(this, et, j);
                                 const {
                                     isMac: V
                                 } = n.FeatureTest.platform;
-                                return u.addEventListener("keydown", (Z) => {
-                                    Z.key === "Enter" && (V ? Z.metaKey : Z.ctrlKey) && K(this, te, hn).call(this);
+                                return u.addEventListener("keydown", (Q) => {
+                                    Q.key === "Enter" && (V ? Q.metaKey : Q.ctrlKey) && K(this, te, hn).call(this);
                                 }), !L.popupRef && this.hasPopupData ? this._createPopup() : j.classList.add("popupTriggerArea"), u.append(j), u;
                             }
                             getElementsToTriggerPopup() {
                                 return a(this, et);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
@@ -19813,22 +19812,22 @@
                         class d {
                             constructor({
                                 div: U,
                                 accessibilityManager: u,
                                 annotationCanvasMap: L,
                                 l10n: j,
                                 page: V,
-                                viewport: Z
+                                viewport: Q
                             }) {
                                 W(this, Be);
                                 W(this, Ae);
                                 W(this, Ne, null);
                                 W(this, ke, null);
                                 W(this, $e, /* @__PURE__ */ new Map());
-                                this.div = U, oe(this, Ne, u), oe(this, ke, L), this.l10n = j, this.page = V, this.viewport = Z, this.zIndex = 0, this.l10n || (this.l10n = _.NullL10n);
+                                this.div = U, oe(this, Ne, u), oe(this, ke, L), this.l10n = j, this.page = V, this.viewport = Q, this.zIndex = 0, this.l10n || (this.l10n = _.NullL10n);
                             }
                             async render(U) {
                                 const {
                                     annotations: u
                                 } = U, L = this.div;
                                 (0, s.setLayerDimensions)(L, this.viewport);
                                 const j = /* @__PURE__ */ new Map(),
@@ -19843,42 +19842,42 @@
                                         annotationStorage: U.annotationStorage || new l.AnnotationStorage(),
                                         enableScripting: U.enableScripting === !0,
                                         hasJSActions: U.hasJSActions,
                                         fieldObjects: U.fieldObjects,
                                         parent: this,
                                         elements: null
                                     };
-                                for (const Z of u) {
-                                    if (Z.noHTML)
+                                for (const Q of u) {
+                                    if (Q.noHTML)
                                         continue;
-                                    const he = Z.annotationType === n.AnnotationType.POPUP;
+                                    const he = Q.annotationType === n.AnnotationType.POPUP;
                                     if (he) {
-                                        const Re = j.get(Z.id);
+                                        const Re = j.get(Q.id);
                                         if (!Re)
                                             continue;
                                         V.elements = Re;
                                     } else {
                                         const {
                                             width: Re,
                                             height: qe
-                                        } = S(Z.rect);
+                                        } = S(Q.rect);
                                         if (Re <= 0 || qe <= 0)
                                             continue;
                                     }
-                                    V.data = Z;
+                                    V.data = Q;
                                     const ye = w.create(V);
                                     if (!ye.isRenderable)
                                         continue;
-                                    if (!he && Z.popupRef) {
-                                        const Re = j.get(Z.popupRef);
-                                        Re ? Re.push(ye) : j.set(Z.popupRef, [ye]);
+                                    if (!he && Q.popupRef) {
+                                        const Re = j.get(Q.popupRef);
+                                        Re ? Re.push(ye) : j.set(Q.popupRef, [ye]);
                                     }
                                     ye.annotationEditorType > 0 && a(this, $e).set(ye.data.id, ye);
                                     const Me = ye.render();
-                                    Z.hidden && (Me.style.visibility = "hidden"), K(this, Be, Bn).call(this, Me, Z.id);
+                                    Q.hidden && (Me.style.visibility = "hidden"), K(this, Be, Bn).call(this, Me, Q.id);
                                 }
                                 K(this, Ae, un).call(this), await this.l10n.translate(L);
                             }
                             update({
                                 viewport: U
                             }) {
                                 const u = this.div;
@@ -20223,15 +20222,15 @@
                             }
                         }
                         e.XfaLayer = s;
                     },
                     /* 33 */
                     /***/
                     (t, e, i) => {
-                        var o, r, T, S, w, C, P, b, k, F, x, y, p, E, $, Hn, m, Un, D, jn, G, Gn, B, dn, Y, Wn, le, pn, we, qn, R, zn, g, Xn, v, Vn, O, Yn, z, ot, Q, gn, ue, Ft, fe, It, Fe, pt, De, _n, ie, Lt, ge, Kn, xe, mn, We, Jn, ze, Qn, Ge, bn, de, Dt, J, gt;
+                        var o, r, T, S, w, C, P, b, k, F, x, y, p, E, $, Hn, m, Un, D, jn, G, Gn, B, dn, Y, Wn, le, pn, we, qn, R, zn, g, Xn, v, Vn, O, Yn, z, ot, Z, gn, ue, Ft, fe, It, Fe, pt, De, _n, ie, Lt, ge, Kn, xe, mn, We, Jn, ze, Zn, Ge, bn, de, Dt, J, gt;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.InkEditor = void 0;
                         var n = i(1),
                             s = i(4),
                             l = i(29),
                             h = i(6),
@@ -20251,15 +20250,15 @@
                                 W(this, le);
                                 W(this, we);
                                 W(this, R);
                                 W(this, g);
                                 W(this, v);
                                 W(this, O);
                                 W(this, z);
-                                W(this, Q);
+                                W(this, Z);
                                 W(this, ue);
                                 W(this, fe);
                                 W(this, Fe);
                                 W(this, De);
                                 W(this, ie);
                                 W(this, ze);
                                 W(this, Ge);
@@ -20362,100 +20361,100 @@
                             canvasPointerdown(te) {
                                 te.button !== 0 || !this.isInEditMode() || a(this, b) || (this.setInForeground(), te.preventDefault(), te.type !== "mouse" && this.div.focus(), K(this, Y, Wn).call(this, te.offsetX, te.offsetY));
                             }
                             canvasPointermove(te) {
                                 te.preventDefault(), K(this, le, pn).call(this, te.offsetX, te.offsetY);
                             }
                             canvasPointerup(te) {
-                                te.preventDefault(), K(this, Q, gn).call(this, te);
+                                te.preventDefault(), K(this, Z, gn).call(this, te);
                             }
                             canvasPointerleave(te) {
-                                K(this, Q, gn).call(this, te);
+                                K(this, Z, gn).call(this, te);
                             }
                             get isResizable() {
                                 return !this.isEmpty() && a(this, b);
                             }
                             render() {
                                 if (this.div)
                                     return this.div;
                                 let te, Te;
-                                this.width && (te = this.x, Te = this.y), super.render(), s.AnnotationEditor._l10nPromise.get("editor_ink2_aria_label").then((Qe) => {
+                                this.width && (te = this.x, Te = this.y), super.render(), s.AnnotationEditor._l10nPromise.get("editor_ink2_aria_label").then((Ze) => {
                                     var Ae;
-                                    return (Ae = this.div) == null ? void 0 : Ae.setAttribute("aria-label", Qe);
+                                    return (Ae = this.div) == null ? void 0 : Ae.setAttribute("aria-label", Ze);
                                 });
                                 const [Ne, ke, $e, Be] = K(this, G, Gn).call(this);
                                 if (this.setAt(Ne, ke, 0, 0), this.setDims($e, Be), K(this, ue, Ft).call(this), this.width) {
-                                    const [Qe, Ae] = this.parentDimensions;
-                                    this.setAspectRatio(this.width * Qe, this.height * Ae), this.setAt(te * Qe, Te * Ae, this.width * Qe, this.height * Ae), oe(this, F, !0), K(this, Fe, pt).call(this), this.setDims(this.width * Qe, this.height * Ae), K(this, z, ot).call(this), this.div.classList.add("disabled");
+                                    const [Ze, Ae] = this.parentDimensions;
+                                    this.setAspectRatio(this.width * Ze, this.height * Ae), this.setAt(te * Ze, Te * Ae, this.width * Ze, this.height * Ae), oe(this, F, !0), K(this, Fe, pt).call(this), this.setDims(this.width * Ze, this.height * Ae), K(this, z, ot).call(this), this.div.classList.add("disabled");
                                 } else
                                     this.div.classList.add("editing"), this.enableEditMode();
                                 return K(this, fe, It).call(this), this.div;
                             }
                             setDimensions(te, Te) {
                                 const Ne = Math.round(te),
                                     ke = Math.round(Te);
                                 if (a(this, y) === Ne && a(this, p) === ke)
                                     return;
                                 oe(this, y, Ne), oe(this, p, ke), this.canvas.style.visibility = "hidden";
                                 const [$e, Be] = this.parentDimensions;
                                 this.width = te / $e, this.height = Te / Be, this.fixAndSetPosition(), a(this, b) && K(this, De, _n).call(this, te, Te), K(this, Fe, pt).call(this), K(this, z, ot).call(this), this.canvas.style.visibility = "visible", this.fixDims();
                             }
                             static deserialize(te, Te, Ne) {
-                                var V, Z, he;
+                                var V, Q, he;
                                 if (te instanceof l.InkAnnotationElement)
                                     return null;
                                 const ke = super.deserialize(te, Te, Ne);
                                 ke.thickness = te.thickness, ke.color = n.Util.makeHexColor(...te.color), ke.opacity = te.opacity;
-                                const [$e, Be] = ke.pageDimensions, Qe = ke.width * $e, Ae = ke.height * Be, Ke = ke.parentScale, Oe = te.thickness / 2;
-                                oe(ke, b, !0), oe(ke, y, Math.round(Qe)), oe(ke, p, Math.round(Ae));
+                                const [$e, Be] = ke.pageDimensions, Ze = ke.width * $e, Ae = ke.height * Be, Ke = ke.parentScale, Oe = te.thickness / 2;
+                                oe(ke, b, !0), oe(ke, y, Math.round(Ze)), oe(ke, p, Math.round(Ae));
                                 const {
                                     paths: U,
                                     rect: u,
                                     rotation: L
                                 } = te;
                                 for (let {
                                         bezier: ye
                                     }
                                     of U) {
                                     ye = K(V = Se, We, Jn).call(V, ye, u, L);
                                     const Me = [];
                                     ke.paths.push(Me);
                                     let Re = Ke * (ye[0] - Oe),
                                         qe = Ke * (ye[1] - Oe);
-                                    for (let Le = 2, He = ye.length; Le < He; Le += 6) {
+                                    for (let Le = 2, Ue = ye.length; Le < Ue; Le += 6) {
                                         const Ve = Ke * (ye[Le] - Oe),
                                             Je = Ke * (ye[Le + 1] - Oe),
-                                            Ze = Ke * (ye[Le + 2] - Oe),
+                                            Qe = Ke * (ye[Le + 2] - Oe),
                                             st = Ke * (ye[Le + 3] - Oe),
                                             it = Ke * (ye[Le + 4] - Oe),
                                             rt = Ke * (ye[Le + 5] - Oe);
                                         Me.push([
                                             [Re, qe],
                                             [Ve, Je],
-                                            [Ze, st],
+                                            [Qe, st],
                                             [it, rt]
                                         ]), Re = it, qe = rt;
                                     }
                                     const Ie = K(this, ge, Kn).call(this, Me);
                                     ke.bezierPath2D.push(Ie);
                                 }
-                                const j = K(Z = ke, Ge, bn).call(Z);
-                                return oe(ke, r, Math.max(s.AnnotationEditor.MIN_SIZE, j[2] - j[0])), oe(ke, o, Math.max(s.AnnotationEditor.MIN_SIZE, j[3] - j[1])), K(he = ke, De, _n).call(he, Qe, Ae), ke;
+                                const j = K(Q = ke, Ge, bn).call(Q);
+                                return oe(ke, r, Math.max(s.AnnotationEditor.MIN_SIZE, j[2] - j[0])), oe(ke, o, Math.max(s.AnnotationEditor.MIN_SIZE, j[3] - j[1])), K(he = ke, De, _n).call(he, Ze, Ae), ke;
                             }
                             serialize() {
                                 if (this.isEmpty())
                                     return null;
                                 const te = this.getRect(0, 0),
                                     Te = s.AnnotationEditor._colorManager.convert(this.ctx.strokeStyle);
                                 return {
                                     annotationType: n.AnnotationEditorType.INK,
                                     color: Te,
                                     thickness: this.thickness,
                                     opacity: this.opacity,
-                                    paths: K(this, ze, Qn).call(this, this.scaleFactor / this.parentScale, this.translationX, this.translationY, te),
+                                    paths: K(this, ze, Zn).call(this, this.scaleFactor / this.parentScale, this.translationX, this.translationY, te),
                                     pageIndex: this.pageIndex,
                                     rect: te,
                                     rotation: this.rotation,
                                     structTreeParentId: this._structTreeParentId
                                 };
                             }
                         };
@@ -20560,20 +20559,20 @@
                             }
                             const ke = a(this, P),
                                 $e = this.currentPath;
                             this.currentPath = [], oe(this, P, new Path2D());
                             const Be = () => {
                                     this.allRawPaths.push($e), this.paths.push(Ne), this.bezierPath2D.push(ke), this.rebuild();
                                 },
-                                Qe = () => {
+                                Ze = () => {
                                     this.allRawPaths.pop(), this.paths.pop(), this.bezierPath2D.pop(), this.paths.length === 0 ? this.remove() : (this.canvas || (K(this, ue, Ft).call(this), K(this, fe, It).call(this)), K(this, J, gt).call(this));
                                 };
                             this.addCommands({
                                 cmd: Be,
-                                undo: Qe,
+                                undo: Ze,
                                 mustExec: !0
                             });
                         }, g = new WeakSet(), Xn = function() {
                             if (!a(this, k))
                                 return;
                             oe(this, k, !1);
                             const te = Math.ceil(this.thickness * this.parentScale),
@@ -20584,35 +20583,35 @@
                             const {
                                 ctx: $e
                             } = this;
                             $e.save(), $e.clearRect(0, 0, this.canvas.width, this.canvas.height);
                             for (const Be of this.bezierPath2D)
                                 $e.stroke(Be);
                             $e.stroke(a(this, P)), $e.restore();
-                        }, v = new WeakSet(), Vn = function(te, Te, Ne, ke, $e, Be, Qe) {
+                        }, v = new WeakSet(), Vn = function(te, Te, Ne, ke, $e, Be, Ze) {
                             const Ae = (Te + ke) / 2,
                                 Ke = (Ne + $e) / 2,
                                 Oe = (ke + Be) / 2,
-                                U = ($e + Qe) / 2;
+                                U = ($e + Ze) / 2;
                             te.bezierCurveTo(Ae + 2 * (ke - Ae) / 3, Ke + 2 * ($e - Ke) / 3, Oe + 2 * (ke - Oe) / 3, U + 2 * ($e - U) / 3, Oe, U);
                         }, O = new WeakSet(), Yn = function() {
                             const te = this.currentPath;
                             if (te.length <= 2)
                                 return [
                                     [te[0], te[0], te.at(-1), te.at(-1)]
                                 ];
                             const Te = [];
                             let Ne, [ke, $e] = te[0];
                             for (Ne = 1; Ne < te.length - 2; Ne++) {
-                                const [u, L] = te[Ne], [j, V] = te[Ne + 1], Z = (u + j) / 2, he = (L + V) / 2, ye = [ke + 2 * (u - ke) / 3, $e + 2 * (L - $e) / 3], Me = [Z + 2 * (u - Z) / 3, he + 2 * (L - he) / 3];
+                                const [u, L] = te[Ne], [j, V] = te[Ne + 1], Q = (u + j) / 2, he = (L + V) / 2, ye = [ke + 2 * (u - ke) / 3, $e + 2 * (L - $e) / 3], Me = [Q + 2 * (u - Q) / 3, he + 2 * (L - he) / 3];
                                 Te.push([
-                                    [ke, $e], ye, Me, [Z, he]
-                                ]), [ke, $e] = [Z, he];
+                                    [ke, $e], ye, Me, [Q, he]
+                                ]), [ke, $e] = [Q, he];
                             }
-                            const [Be, Qe] = te[Ne], [Ae, Ke] = te[Ne + 1], Oe = [ke + 2 * (Be - ke) / 3, $e + 2 * (Qe - $e) / 3], U = [Ae + 2 * (Be - Ae) / 3, Ke + 2 * (Qe - Ke) / 3];
+                            const [Be, Ze] = te[Ne], [Ae, Ke] = te[Ne + 1], Oe = [ke + 2 * (Be - ke) / 3, $e + 2 * (Ze - $e) / 3], U = [Ae + 2 * (Be - Ae) / 3, Ke + 2 * (Ze - Ke) / 3];
                             return Te.push([
                                 [ke, $e], Oe, U, [Ae, Ke]
                             ]), Te;
                         }, z = new WeakSet(), ot = function() {
                             if (this.isEmpty()) {
                                 K(this, ie, Lt).call(this);
                                 return;
@@ -20621,15 +20620,15 @@
                             const {
                                 canvas: te,
                                 ctx: Te
                             } = this;
                             Te.setTransform(1, 0, 0, 1, 0, 0), Te.clearRect(0, 0, te.width, te.height), K(this, ie, Lt).call(this);
                             for (const Ne of this.bezierPath2D)
                                 Te.stroke(Ne);
-                        }, Q = new WeakSet(), gn = function(te) {
+                        }, Z = new WeakSet(), gn = function(te) {
                             this.canvas.removeEventListener("pointerleave", a(this, S)), this.canvas.removeEventListener("pointermove", a(this, T)), this.canvas.removeEventListener("pointerup", a(this, w)), this.canvas.addEventListener("pointerdown", a(this, C)), setTimeout(() => {
                                 this.canvas.removeEventListener("contextmenu", h.noContextMenu);
                             }, 10), K(this, R, zn).call(this, te.offsetX, te.offsetY), this.addToAnnotationStorage(), this.setInBackground();
                         }, ue = new WeakSet(), Ft = function() {
                             this.canvas = document.createElement("canvas"), this.canvas.width = this.canvas.height = 0, this.canvas.className = "inkEditorCanvas", s.AnnotationEditor._l10nPromise.get("editor_ink_canvas_aria_label").then((te) => {
                                 var Te;
                                 return (Te = this.canvas) == null ? void 0 : Te.setAttribute("aria-label", te);
@@ -20651,99 +20650,99 @@
                             this.scaleFactor = Math.min(ke, $e);
                         }, ie = new WeakSet(), Lt = function() {
                             const te = K(this, de, Dt).call(this) / 2;
                             this.ctx.setTransform(this.scaleFactor, 0, 0, this.scaleFactor, this.translationX * this.scaleFactor + te, this.translationY * this.scaleFactor + te);
                         }, ge = new WeakSet(), Kn = function(te) {
                             const Te = new Path2D();
                             for (let Ne = 0, ke = te.length; Ne < ke; Ne++) {
-                                const [$e, Be, Qe, Ae] = te[Ne];
-                                Ne === 0 && Te.moveTo(...$e), Te.bezierCurveTo(Be[0], Be[1], Qe[0], Qe[1], Ae[0], Ae[1]);
+                                const [$e, Be, Ze, Ae] = te[Ne];
+                                Ne === 0 && Te.moveTo(...$e), Te.bezierCurveTo(Be[0], Be[1], Ze[0], Ze[1], Ae[0], Ae[1]);
                             }
                             return Te;
                         }, xe = new WeakSet(), mn = function(te, Te, Ne) {
-                            const [ke, $e, Be, Qe] = Te;
+                            const [ke, $e, Be, Ze] = Te;
                             switch (Ne) {
                                 case 0:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2)
-                                        te[Ae] += ke, te[Ae + 1] = Qe - te[Ae + 1];
+                                        te[Ae] += ke, te[Ae + 1] = Ze - te[Ae + 1];
                                     break;
                                 case 90:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2) {
                                         const Oe = te[Ae];
                                         te[Ae] = te[Ae + 1] + ke, te[Ae + 1] = Oe + $e;
                                     }
                                     break;
                                 case 180:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2)
                                         te[Ae] = Be - te[Ae], te[Ae + 1] += $e;
                                     break;
                                 case 270:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2) {
                                         const Oe = te[Ae];
-                                        te[Ae] = Be - te[Ae + 1], te[Ae + 1] = Qe - Oe;
+                                        te[Ae] = Be - te[Ae + 1], te[Ae + 1] = Ze - Oe;
                                     }
                                     break;
                                 default:
                                     throw new Error("Invalid rotation");
                             }
                             return te;
                         }, We = new WeakSet(), Jn = function(te, Te, Ne) {
-                            const [ke, $e, Be, Qe] = Te;
+                            const [ke, $e, Be, Ze] = Te;
                             switch (Ne) {
                                 case 0:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2)
-                                        te[Ae] -= ke, te[Ae + 1] = Qe - te[Ae + 1];
+                                        te[Ae] -= ke, te[Ae + 1] = Ze - te[Ae + 1];
                                     break;
                                 case 90:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2) {
                                         const Oe = te[Ae];
                                         te[Ae] = te[Ae + 1] - $e, te[Ae + 1] = Oe - ke;
                                     }
                                     break;
                                 case 180:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2)
                                         te[Ae] = Be - te[Ae], te[Ae + 1] -= $e;
                                     break;
                                 case 270:
                                     for (let Ae = 0, Ke = te.length; Ae < Ke; Ae += 2) {
                                         const Oe = te[Ae];
-                                        te[Ae] = Qe - te[Ae + 1], te[Ae + 1] = Be - Oe;
+                                        te[Ae] = Ze - te[Ae + 1], te[Ae + 1] = Be - Oe;
                                     }
                                     break;
                                 default:
                                     throw new Error("Invalid rotation");
                             }
                             return te;
-                        }, ze = new WeakSet(), Qn = function(te, Te, Ne, ke) {
+                        }, ze = new WeakSet(), Zn = function(te, Te, Ne, ke) {
                             var Ke, Oe;
                             const $e = [],
                                 Be = this.thickness / 2,
-                                Qe = te * Te + Be,
+                                Ze = te * Te + Be,
                                 Ae = te * Ne + Be;
                             for (const U of this.paths) {
                                 const u = [],
                                     L = [];
                                 for (let j = 0, V = U.length; j < V; j++) {
-                                    const [Z, he, ye, Me] = U[j], Re = te * Z[0] + Qe, qe = te * Z[1] + Ae, Ie = te * he[0] + Qe, Le = te * he[1] + Ae, He = te * ye[0] + Qe, Ve = te * ye[1] + Ae, Je = te * Me[0] + Qe, Ze = te * Me[1] + Ae;
-                                    j === 0 && (u.push(Re, qe), L.push(Re, qe)), u.push(Ie, Le, He, Ve, Je, Ze), L.push(Ie, Le), j === V - 1 && L.push(Je, Ze);
+                                    const [Q, he, ye, Me] = U[j], Re = te * Q[0] + Ze, qe = te * Q[1] + Ae, Ie = te * he[0] + Ze, Le = te * he[1] + Ae, Ue = te * ye[0] + Ze, Ve = te * ye[1] + Ae, Je = te * Me[0] + Ze, Qe = te * Me[1] + Ae;
+                                    j === 0 && (u.push(Re, qe), L.push(Re, qe)), u.push(Ie, Le, Ue, Ve, Je, Qe), L.push(Ie, Le), j === V - 1 && L.push(Je, Qe);
                                 }
                                 $e.push({
                                     bezier: K(Ke = Se, xe, mn).call(Ke, u, ke, this.rotation),
                                     points: K(Oe = Se, xe, mn).call(Oe, L, ke, this.rotation)
                                 });
                             }
                             return $e;
                         }, Ge = new WeakSet(), bn = function() {
                             let te = 1 / 0,
                                 Te = -1 / 0,
                                 Ne = 1 / 0,
                                 ke = -1 / 0;
                             for (const $e of this.paths)
-                                for (const [Be, Qe, Ae, Ke] of $e) {
-                                    const Oe = n.Util.bezierBoundingBox(...Be, ...Qe, ...Ae, ...Ke);
+                                for (const [Be, Ze, Ae, Ke] of $e) {
+                                    const Oe = n.Util.bezierBoundingBox(...Be, ...Ze, ...Ae, ...Ke);
                                     te = Math.min(te, Oe[0]), Ne = Math.min(Ne, Oe[1]), Te = Math.max(Te, Oe[2]), ke = Math.max(ke, Oe[3]);
                                 }
                             return [te, Ne, Te, ke];
                         }, de = new WeakSet(), Dt = function() {
                             return a(this, b) ? Math.ceil(this.thickness * this.parentScale) : 0;
                         }, J = new WeakSet(), gt = function(te = !1) {
                             if (this.isEmpty())
@@ -20753,29 +20752,29 @@
                                 return;
                             }
                             const Te = K(this, Ge, bn).call(this),
                                 Ne = K(this, de, Dt).call(this);
                             oe(this, r, Math.max(s.AnnotationEditor.MIN_SIZE, Te[2] - Te[0])), oe(this, o, Math.max(s.AnnotationEditor.MIN_SIZE, Te[3] - Te[1]));
                             const ke = Math.ceil(Ne + a(this, r) * this.scaleFactor),
                                 $e = Math.ceil(Ne + a(this, o) * this.scaleFactor),
-                                [Be, Qe] = this.parentDimensions;
-                            this.width = ke / Be, this.height = $e / Qe, this.setAspectRatio(ke, $e);
+                                [Be, Ze] = this.parentDimensions;
+                            this.width = ke / Be, this.height = $e / Ze, this.setAspectRatio(ke, $e);
                             const Ae = this.translationX,
                                 Ke = this.translationY;
                             this.translationX = -Te[0], this.translationY = -Te[1], K(this, Fe, pt).call(this), K(this, z, ot).call(this), oe(this, y, ke), oe(this, p, $e), this.setDims(ke, $e);
                             const Oe = te ? Ne / this.scaleFactor / 2 : 0;
                             this.translate(Ae - this.translationX - Oe, Ke - this.translationY - Oe);
                         }, W(Se, ge), W(Se, xe), W(Se, We), nt(Se, "_defaultColor", null), nt(Se, "_defaultOpacity", 1), nt(Se, "_defaultThickness", 1), nt(Se, "_type", "ink");
                         let c = Se;
                         e.InkEditor = c;
                     },
                     /* 34 */
                     /***/
                     (t, e, i) => {
-                        var c, o, r, T, S, w, C, P, b, k, F, Et, y, St, E, Ot, M, yn, N, Zn, X, ei, I, vn, ee, Nt, q, ti;
+                        var c, o, r, T, S, w, C, P, b, k, F, Et, y, St, E, Ot, M, yn, N, Qn, X, ei, I, vn, ee, Nt, q, ti;
                         Object.defineProperty(e, "__esModule", {
                             value: !0
                         }), e.StampEditor = void 0;
                         var n = i(1),
                             s = i(4),
                             l = i(6),
                             h = i(29);
@@ -20862,16 +20861,16 @@
                                         rect: v,
                                         bitmapUrl: A,
                                         bitmapId: O,
                                         isSvg: H,
                                         accessibilityData: z
                                     } = R;
                                 O && g.imageManager.isValidId(O) ? oe(f, o, O) : oe(f, T, A), oe(f, b, H);
-                                const [ae, Q] = f.pageDimensions;
-                                return f.width = (v[2] - v[0]) / ae, f.height = (v[3] - v[1]) / Q, z && (f.altTextData = z), f;
+                                const [ae, Z] = f.pageDimensions;
+                                return f.width = (v[2] - v[0]) / ae, f.height = (v[3] - v[1]) / Z, z && (f.altTextData = z), f;
                             }
                             serialize(R = !1, d = null) {
                                 if (this.isEmpty())
                                     return null;
                                 const g = {
                                     annotationType: n.AnnotationEditorType.STAMP,
                                     bitmapId: a(this, o),
@@ -20968,15 +20967,15 @@
                                     type: "editing",
                                     subtype: this.editorType,
                                     data: {
                                         action: "inserted_image"
                                     }
                                 }
                             }), this.addAltTextButton();
-                        }, N = new WeakSet(), Zn = function(R, d) {
+                        }, N = new WeakSet(), Qn = function(R, d) {
                             var A;
                             const [g, f] = this.parentDimensions;
                             this.width = R / g, this.height = d / f, this.setDims(R, d), (A = this._initialOptions) != null && A.isCentered ? this.center() : this.fixAndSetPosition(), this._initialOptions = null, a(this, P) !== null && clearTimeout(a(this, P)), oe(this, P, setTimeout(() => {
                                 oe(this, P, null), K(this, I, vn).call(this, R, d);
                             }, 200));
                         }, X = new WeakSet(), ei = function(R, d) {
                             const {
@@ -21020,15 +21019,15 @@
                                 const [d, g] = this.pageDimensions, f = Math.round(this.width * d * l.PixelsPerInch.PDF_TO_CSS_UNITS), v = Math.round(this.height * g * l.PixelsPerInch.PDF_TO_CSS_UNITS), A = new OffscreenCanvas(f, v);
                                 return A.getContext("2d").drawImage(a(this, c), 0, 0, a(this, c).width, a(this, c).height, 0, 0, f, v), A.transferToImageBitmap();
                             }
                             return structuredClone(a(this, c));
                         }, q = new WeakSet(), ti = function() {
                             oe(this, C, new ResizeObserver((R) => {
                                 const d = R[0].contentRect;
-                                d.width && d.height && K(this, N, Zn).call(this, d.width, d.height);
+                                d.width && d.height && K(this, N, Qn).call(this, d.width, d.height);
                             })), a(this, C).observe(this.div);
                         }, nt(pe, "_type", "stamp");
                         let _ = pe;
                         e.StampEditor = _;
                     }
                     /******/
                 ],
@@ -21765,20 +21764,20 @@
     pdfjsLib.GlobalWorkerOptions.workerSrc = "https://cdn.bootcss.com/pdf.js/3.11.174/pdf.worker.js";
     let b = h,
         k = b,
         F, x = 1,
         y = 1,
         p;
     async function E() {
-        i(12, b = null), await tick(), P.dispatch("change");
+        i(12, b = null), await tick(), P.dispatch("change"), i(14, y = 1);
     }
     async function $({
         detail: G
     }) {
-        i(0, h = G), await tick(), P.dispatch("change"), P.dispatch("upload");
+        i(0, h = G), await tick(), P.dispatch("change"), P.dispatch("upload"), i(14, y = 1);
     }
     async function M(G) {
         F = await pdfjsLib.getDocument(G.url).promise, i(13, x = F.numPages), m();
     }
 
     function m() {
         F.getPage(y).then((G) => {
```

### Comparing `gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/style.css` & `gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/backend/gradio_pdf/templates/component/wrapper-98f94c21-15fa1cb3.js` & `gradio_pdf-0.0.6/backend/gradio_pdf/templates/component/wrapper-98f94c21-d1a5537c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     r as S
-} from "./Index-9e3f581a.js";
+} from "./Index-94e506c5.js";
 
 function z(s) {
     return s && s.__esModule && Object.prototype.hasOwnProperty.call(s, "default") ? s.default : s;
 }
 
 function gt(s) {
     if (s.__esModule)
@@ -911,15 +911,15 @@
     getPayloadLength64() {
         if (this._bufferedBytes < 8) {
             this._loop = !1;
             return;
         }
         const e = this.consume(8),
             t = e.readUInt32BE(0);
-        return t > Math.pow(2, 53 - 32) - 1 ? (this._loop = !1, g(
+        return t > Math.pow(2, 21) - 1 ? (this._loop = !1, g(
             RangeError,
             "Unsupported WebSocket frame: payload length > 2^53 - 1",
             !1,
             1009,
             "WS_ERR_UNSUPPORTED_DATA_PAYLOAD_LENGTH"
         )) : (this._payloadLength = t * Math.pow(2, 32) + e.readUInt32BE(4), this.haveLength());
     }
@@ -1853,16 +1853,15 @@
      * @param {(String|Buffer)} [data] The reason why the connection is
      *     closing
      * @public
      */
     close(e, t) {
         if (this.readyState !== d.CLOSED) {
             if (this.readyState === d.CONNECTING) {
-                const r = "WebSocket was closed before the connection was established";
-                b(this, this._req, r);
+                b(this, this._req, "WebSocket was closed before the connection was established");
                 return;
             }
             if (this.readyState === d.CLOSING) {
                 this._closeFrameSent && (this._closeFrameReceived || this._receiver._writableState.errorEmitted) && this._socket.end();
                 return;
             }
             this._readyState = d.CLOSING, this._sender.close(e, t, !this._isServer, (r) => {
@@ -1958,16 +1957,15 @@
      * Forcibly close the connection.
      *
      * @public
      */
     terminate() {
         if (this.readyState !== d.CLOSED) {
             if (this.readyState === d.CONNECTING) {
-                const e = "WebSocket was closed before the connection was established";
-                b(this, this._req, e);
+                b(this, this._req, "WebSocket was closed before the connection was established");
                 return;
             }
             this._socket && (this._readyState = d.CLOSING, this._socket.destroy());
         }
     }
 };
 Object.defineProperty(m, "CONNECTING", {
```

### Comparing `gradio_pdf-0.0.5/backend/gradio_pdf/templates/example/index.js` & `gradio_pdf-0.0.6/backend/gradio_pdf/templates/example/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -708,30 +708,30 @@
                                     return !1;
                             return !0;
                         }
 
                         function Ct(ot = /* @__PURE__ */ new Date()) {
                             return [ot.getUTCFullYear().toString(), (ot.getUTCMonth() + 1).toString().padStart(2, "0"), ot.getUTCDate().toString().padStart(2, "0"), ot.getUTCHours().toString().padStart(2, "0"), ot.getUTCMinutes().toString().padStart(2, "0"), ot.getUTCSeconds().toString().padStart(2, "0")].join("");
                         }
-                        class jt {
+                        class Ut {
                             constructor() {
                                 L(this, $t, !1);
                                 this.promise = new Promise((Y, G) => {
                                     this.resolve = (bt) => {
                                         Z(this, $t, !0), Y(bt);
                                     }, this.reject = (bt) => {
                                         Z(this, $t, !0), G(bt);
                                     };
                                 });
                             }
                             get settled() {
                                 return t(this, $t);
                             }
                         }
-                        $t = new WeakMap(), d.PromiseCapability = jt;
+                        $t = new WeakMap(), d.PromiseCapability = Ut;
                         let Gt = null,
                             Ht = null;
 
                         function Xt(ot) {
                             return Gt || (Gt = /([\u00a0\u00b5\u037e\u0eb3\u2000-\u200a\u202f\u2126\ufb00-\ufb04\ufb06\ufb20-\ufb36\ufb38-\ufb3c\ufb3e\ufb40-\ufb41\ufb43-\ufb44\ufb46-\ufba1\ufba4-\ufba9\ufbae-\ufbb1\ufbd3-\ufbdc\ufbde-\ufbe7\ufbea-\ufbf8\ufbfc-\ufbfd\ufc00-\ufc5d\ufc64-\ufcf1\ufcf5-\ufd3d\ufd88\ufdf4\ufdfa-\ufdfb\ufe71\ufe77\ufe79\ufe7b\ufe7d]+)|(\ufb05+)/gu, Ht = /* @__PURE__ */ new Map([
                                 ["ﬅ", "ſt"]
                             ])), ot.replaceAll(Gt, (Y, G, bt) => G ? G.normalize("NFKC") : Ht.get(bt));
@@ -850,19 +850,19 @@
                             };
                             if (Dt || (ht.cMapReaderFactory = new S({
                                     baseUrl: wt,
                                     isCompressed: xt
                                 }), ht.standardFontDataFactory = new n({
                                     baseUrl: i
                                 })), !H) {
-                                const jt = {
+                                const Ut = {
                                     verbosity: lt,
                                     port: _worker_options.GlobalWorkerOptions.workerPort
                                 };
-                                H = jt.port ? PDFWorker.fromPort(jt) : new PDFWorker(jt), r._worker = H;
+                                H = Ut.port ? PDFWorker.fromPort(Ut) : new PDFWorker(Ut), r._worker = H;
                             }
                             const Et = {
                                     docId: T,
                                     apiVersion: "3.11.174",
                                     data: U,
                                     password: V,
                                     disableAutoFetch: ut,
@@ -893,15 +893,15 @@
                                     disableAutoFetch: ut,
                                     pdfBug: Ft,
                                     styleElement: J
                                 };
                             return H.promise.then(function() {
                                 if (r.destroyed)
                                     throw new Error("Loading aborted");
-                                const jt = _fetchDocument(H, Et),
+                                const Ut = _fetchDocument(H, Et),
                                     Gt = new Promise(function(Ht) {
                                         let Xt;
                                         st ? Xt = new _transport_stream.PDFDataTransportStream({
                                             length: Bt,
                                             initialData: st.initialData,
                                             progressiveDone: st.progressiveDone,
                                             contentDispositionFilename: st.contentDispositionFilename,
@@ -913,15 +913,15 @@
                                             httpHeaders: z,
                                             withCredentials: E,
                                             rangeChunkSize: at,
                                             disableRange: ct,
                                             disableStream: yt
                                         })), Ht(Xt);
                                     });
-                                return Promise.all([jt, Gt]).then(function([Ht, Xt]) {
+                                return Promise.all([Ut, Gt]).then(function([Ht, Xt]) {
                                     if (r.destroyed)
                                         throw new Error("Loading aborted");
                                     const Vt = new _message_handler.MessageHandler(T, Ht, H.port),
                                         Wt = new WorkerTransport(Vt, r, Xt, Ct, ht);
                                     r._transport = Wt, Vt.send("Ready", null);
                                 });
                             }).catch(r._capability.reject), r;
@@ -2866,28 +2866,28 @@
                                 case "middleLeft":
                                     J = !0, Dt = (bt, At) => [0, At / 2], ft = (bt, At) => [bt, At / 2];
                                     break;
                             }
                             const ht = Dt(tt, Q),
                                 Et = ft(tt, Q);
                             let Ct = Ft(...Et);
-                            const jt = yt(M + Ct[0]),
+                            const Ut = yt(M + Ct[0]),
                                 Gt = yt(N + Ct[1]);
                             let Ht = 1,
                                 Xt = 1,
                                 [Vt, Wt] = this.screenToPageTranslation(o.movementX, o.movementY);
                             if ([Vt, Wt] = St(Vt / h, Wt / b), K) {
                                 const bt = Math.hypot(tt, Q);
                                 Ht = Xt = Math.max(Math.min(Math.hypot(Et[0] - ht[0] - Vt, Et[1] - ht[1] - Wt) / bt, 1 / tt, 1 / Q), nt / tt, ct / Q);
                             } else
                                 J ? Ht = Math.max(nt, Math.min(1, Math.abs(Et[0] - ht[0] - Vt))) / tt : Xt = Math.max(ct, Math.min(1, Math.abs(Et[1] - ht[1] - Wt))) / Q;
                             const $t = yt(tt * Ht),
                                 ot = yt(Q * Xt);
                             Ct = Ft(...ft($t, ot));
-                            const Y = jt - Ct[0],
+                            const Y = Ut - Ct[0],
                                 G = Gt - Ct[1];
                             this.width = $t, this.height = ot, this.x = Y, this.y = G, this.setDims(h * $t, b * ot), this.fixAndSetPosition();
                         }, gt = new WeakSet(), Ge = async function() {
                             var h;
                             const s = t(this, g);
                             if (!s)
                                 return;
@@ -3896,72 +3896,72 @@
                             }
                             addFilter(J) {
                                 if (!J)
                                     return "none";
                                 let ht = t(this, h, de).get(J);
                                 if (ht)
                                     return ht;
-                                let Et, Ct, jt, Gt;
+                                let Et, Ct, Ut, Gt;
                                 if (J.length === 1) {
                                     const Wt = J[0],
                                         $t = new Array(256);
                                     for (let ot = 0; ot < 256; ot++)
                                         $t[ot] = Wt[ot] / 255;
-                                    Gt = Et = Ct = jt = $t.join(",");
+                                    Gt = Et = Ct = Ut = $t.join(",");
                                 } else {
                                     const [Wt, $t, ot] = J, Y = new Array(256), G = new Array(256), bt = new Array(256);
                                     for (let At = 0; At < 256; At++)
                                         Y[At] = Wt[At] / 255, G[At] = $t[At] / 255, bt[At] = ot[At] / 255;
-                                    Et = Y.join(","), Ct = G.join(","), jt = bt.join(","), Gt = `${Et}${Ct}${jt}`;
+                                    Et = Y.join(","), Ct = G.join(","), Ut = bt.join(","), Gt = `${Et}${Ct}${Ut}`;
                                 }
                                 if (ht = t(this, h, de).get(Gt), ht)
                                     return t(this, h, de).set(J, ht), ht;
                                 const Ht = `g_${t(this, lt)}_transfer_map_${ge(this, o)._++}`,
                                     Xt = `url(#${Ht})`;
                                 t(this, h, de).set(J, Xt), t(this, h, de).set(Gt, Xt);
                                 const Vt = W(this, nt, Te).call(this, Ht);
-                                return W(this, Ft, _e).call(this, Et, Ct, jt, Vt), Xt;
+                                return W(this, Ft, _e).call(this, Et, Ct, Ut, Vt), Xt;
                             }
                             addHCMFilter(J, ht) {
                                 var $t;
                                 const Et = `${J}-${ht}`;
                                 if (t(this, xt) === Et)
                                     return t(this, S);
                                 if (Z(this, xt, Et), Z(this, S, "none"), ($t = t(this, wt)) == null || $t.remove(), !J || !ht)
                                     return t(this, S);
                                 const Ct = W(this, St, Ae).call(this, J);
                                 J = P.Util.makeHexColor(...Ct);
-                                const jt = W(this, St, Ae).call(this, ht);
-                                if (ht = P.Util.makeHexColor(...jt), t(this, M, ue).style.color = "", J === "#000000" && ht === "#ffffff" || J === ht)
+                                const Ut = W(this, St, Ae).call(this, ht);
+                                if (ht = P.Util.makeHexColor(...Ut), t(this, M, ue).style.color = "", J === "#000000" && ht === "#ffffff" || J === ht)
                                     return t(this, S);
                                 const Gt = new Array(256);
                                 for (let ot = 0; ot <= 255; ot++) {
                                     const Y = ot / 255;
                                     Gt[ot] = Y <= 0.03928 ? Y / 12.92 : ((Y + 0.055) / 1.055) ** 2.4;
                                 }
                                 const Ht = Gt.join(","),
                                     Xt = `g_${t(this, lt)}_hcm_filter`,
                                     Vt = Z(this, i, W(this, nt, Te).call(this, Xt));
                                 W(this, Ft, _e).call(this, Ht, Ht, Ht, Vt), W(this, tt, Je).call(this, Vt);
                                 const Wt = (ot, Y) => {
                                     const G = Ct[ot] / 255,
-                                        bt = jt[ot] / 255,
+                                        bt = Ut[ot] / 255,
                                         At = new Array(Y + 1);
                                     for (let te = 0; te <= Y; te++)
                                         At[te] = G + te / Y * (bt - G);
                                     return At.join(",");
                                 };
                                 return W(this, Ft, _e).call(this, Wt(0, 5), Wt(1, 5), Wt(2, 5), Vt), Z(this, S, `url(#${Xt})`), t(this, S);
                             }
                             addHighlightHCMFilter(J, ht, Et, Ct) {
                                 var bt;
-                                const jt = `${J}-${ht}-${Et}-${Ct}`;
-                                if (t(this, n) === jt)
+                                const Ut = `${J}-${ht}-${Et}-${Ct}`;
+                                if (t(this, n) === Ut)
                                     return t(this, s);
-                                if (Z(this, n, jt), Z(this, s, "none"), (bt = t(this, i)) == null || bt.remove(), !J || !ht)
+                                if (Z(this, n, Ut), Z(this, s, "none"), (bt = t(this, i)) == null || bt.remove(), !J || !ht)
                                     return t(this, s);
                                 const [Gt, Ht] = [J, ht].map(W(this, St, Ae).bind(this));
                                 let Xt = Math.round(0.2126 * Gt[0] + 0.7152 * Gt[1] + 0.0722 * Gt[2]),
                                     Vt = Math.round(0.2126 * Ht[0] + 0.7152 * Ht[1] + 0.0722 * Ht[2]),
                                     [Wt, $t] = [Et, Ct].map(W(this, St, Ae).bind(this));
                                 Vt < Xt && ([Xt, Vt, Wt, $t] = [Vt, Xt, $t, Wt]), t(this, M, ue).style.color = "";
                                 const ot = (At, te, Zt) => {
@@ -4008,16 +4008,16 @@
                         }, nt = new WeakSet(), Te = function(J) {
                             const ht = t(this, gt).createElementNS(rt, "filter");
                             return ht.setAttribute("color-interpolation-filters", "sRGB"), ht.setAttribute("id", J), t(this, M, ue).append(ht), ht;
                         }, yt = new WeakSet(), Pe = function(J, ht, Et) {
                             const Ct = t(this, gt).createElementNS(rt, ht);
                             Ct.setAttribute("type", "discrete"), Ct.setAttribute("tableValues", Et), J.append(Ct);
                         }, Ft = new WeakSet(), _e = function(J, ht, Et, Ct) {
-                            const jt = t(this, gt).createElementNS(rt, "feComponentTransfer");
-                            Ct.append(jt), W(this, yt, Pe).call(this, jt, "feFuncR", J), W(this, yt, Pe).call(this, jt, "feFuncG", ht), W(this, yt, Pe).call(this, jt, "feFuncB", Et);
+                            const Ut = t(this, gt).createElementNS(rt, "feComponentTransfer");
+                            Ct.append(Ut), W(this, yt, Pe).call(this, Ut, "feFuncR", J), W(this, yt, Pe).call(this, Ut, "feFuncG", ht), W(this, yt, Pe).call(this, Ut, "feFuncB", Et);
                         }, St = new WeakSet(), Ae = function(J) {
                             return t(this, M, ue).style.color = J, m(getComputedStyle(t(this, M, ue)).getPropertyValue("color"));
                         }, d.DOMFilterFactory = pt;
                         class B extends l.BaseCanvasFactory {
                             constructor({
                                 ownerDocument: K = globalThis.document
                             } = {}) {
@@ -4076,15 +4076,15 @@
                         class x {
                             constructor({
                                 viewBox: K,
                                 scale: J,
                                 rotation: ht,
                                 offsetX: Et = 0,
                                 offsetY: Ct = 0,
-                                dontFlip: jt = !1
+                                dontFlip: Ut = !1
                             }) {
                                 this.viewBox = K, this.scale = J, this.rotation = ht, this.offsetX = Et, this.offsetY = Ct;
                                 const Gt = (K[2] + K[0]) / 2,
                                     Ht = (K[3] + K[1]) / 2;
                                 let Xt, Vt, Wt, $t;
                                 switch (ht %= 360, ht < 0 && (ht += 360), ht) {
                                     case 180:
@@ -4098,15 +4098,15 @@
                                         break;
                                     case 0:
                                         Xt = 1, Vt = 0, Wt = 0, $t = -1;
                                         break;
                                     default:
                                         throw new Error("PageViewport: Invalid rotation, must be a multiple of 90 degrees.");
                                 }
-                                jt && (Wt = -Wt, $t = -$t);
+                                Ut && (Wt = -Wt, $t = -$t);
                                 let ot, Y, G, bt;
                                 Xt === 0 ? (ot = Math.abs(Ht - K[1]) * J + Et, Y = Math.abs(Gt - K[0]) * J + Ct, G = (K[3] - K[1]) * J, bt = (K[2] - K[0]) * J) : (ot = Math.abs(Gt - K[0]) * J + Et, Y = Math.abs(Ht - K[1]) * J + Ct, G = (K[2] - K[0]) * J, bt = (K[3] - K[1]) * J), this.transform = [Xt * J, Vt * J, Wt * J, $t * J, ot - Xt * J * Gt - Wt * J * Ht, Y - Vt * J * Gt - $t * J * Ht], this.width = G, this.height = bt;
                             }
                             get rawDims() {
                                 const {
                                     viewBox: K
                                 } = this;
@@ -4259,25 +4259,25 @@
                                 if (!J)
                                     return null;
                                 const ht = parseInt(J[1], 10);
                                 let Et = parseInt(J[2], 10);
                                 Et = Et >= 1 && Et <= 12 ? Et - 1 : 0;
                                 let Ct = parseInt(J[3], 10);
                                 Ct = Ct >= 1 && Ct <= 31 ? Ct : 1;
-                                let jt = parseInt(J[4], 10);
-                                jt = jt >= 0 && jt <= 23 ? jt : 0;
+                                let Ut = parseInt(J[4], 10);
+                                Ut = Ut >= 0 && Ut <= 23 ? Ut : 0;
                                 let Gt = parseInt(J[5], 10);
                                 Gt = Gt >= 0 && Gt <= 59 ? Gt : 0;
                                 let Ht = parseInt(J[6], 10);
                                 Ht = Ht >= 0 && Ht <= 59 ? Ht : 0;
                                 const Xt = J[7] || "Z";
                                 let Vt = parseInt(J[8], 10);
                                 Vt = Vt >= 0 && Vt <= 23 ? Vt : 0;
                                 let Wt = parseInt(J[9], 10) || 0;
-                                return Wt = Wt >= 0 && Wt <= 59 ? Wt : 0, Xt === "-" ? (jt += Vt, Gt += Wt) : Xt === "+" && (jt -= Vt, Gt -= Wt), new Date(Date.UTC(ht, Et, Ct, jt, Gt, Ht));
+                                return Wt = Wt >= 0 && Wt <= 59 ? Wt : 0, Xt === "-" ? (Ut += Vt, Gt += Wt) : Xt === "+" && (Ut -= Vt, Gt -= Wt), new Date(Date.UTC(ht, Et, Ct, Ut, Gt, Ht));
                             }
                         }
                         d.PDFDateString = r;
 
                         function T(ft, {
                             scale: K = 1,
                             rotation: J = 0
@@ -4315,40 +4315,40 @@
                         function z(ft) {
                             const {
                                 a: K,
                                 b: J,
                                 c: ht,
                                 d: Et,
                                 e: Ct,
-                                f: jt
+                                f: Ut
                             } = ft.getTransform();
-                            return [K, J, ht, Et, Ct, jt];
+                            return [K, J, ht, Et, Ct, Ut];
                         }
 
                         function E(ft) {
                             const {
                                 a: K,
                                 b: J,
                                 c: ht,
                                 d: Et,
                                 e: Ct,
-                                f: jt
+                                f: Ut
                             } = ft.getTransform().invertSelf();
-                            return [K, J, ht, Et, Ct, jt];
+                            return [K, J, ht, Et, Ct, Ut];
                         }
 
                         function V(ft, K, J = !1, ht = !0) {
                             if (K instanceof x) {
                                 const {
                                     pageWidth: Et,
                                     pageHeight: Ct
                                 } = K.rawDims, {
-                                    style: jt
+                                    style: Ut
                                 } = ft, Gt = P.FeatureTest.isCSSRoundSupported, Ht = `var(--scale-factor) * ${Et}px`, Xt = `var(--scale-factor) * ${Ct}px`, Vt = Gt ? `round(${Ht}, 1px)` : `calc(${Ht})`, Wt = Gt ? `round(${Xt}, 1px)` : `calc(${Xt})`;
-                                !J || K.rotation % 180 === 0 ? (jt.width = Vt, jt.height = Wt) : (jt.width = Wt, jt.height = Vt);
+                                !J || K.rotation % 180 === 0 ? (Ut.width = Vt, Ut.height = Wt) : (Ut.width = Wt, Ut.height = Vt);
                             }
                             ht && ft.setAttribute("data-main-rotation", K.rotation);
                         }
                     },
                     /* 7 */
                     /***/
                     (dt, d, et) => {
@@ -4882,27 +4882,27 @@
                                 const Dt = b * Q + ut,
                                     ft = Math.round(Dt),
                                     K = M * yt + Ft,
                                     J = Math.round(K),
                                     ht = (b + N) * Q + ut,
                                     Et = Math.abs(Math.round(ht) - ft) || 1,
                                     Ct = (M + tt) * yt + Ft,
-                                    jt = Math.abs(Math.round(Ct) - J) || 1;
-                                return S.setTransform(Math.sign(Q), 0, 0, Math.sign(yt), ft, J), S.drawImage(i, n, s, o, h, 0, 0, Et, jt), S.setTransform(Q, nt, ct, yt, ut, Ft), [Et, jt];
+                                    Ut = Math.abs(Math.round(Ct) - J) || 1;
+                                return S.setTransform(Math.sign(Q), 0, 0, Math.sign(yt), ft, J), S.drawImage(i, n, s, o, h, 0, 0, Et, Ut), S.setTransform(Q, nt, ct, yt, ut, Ft), [Et, Ut];
                             }
                             if (Q === 0 && yt === 0) {
                                 const Dt = M * ct + ut,
                                     ft = Math.round(Dt),
                                     K = b * nt + Ft,
                                     J = Math.round(K),
                                     ht = (M + tt) * ct + ut,
                                     Et = Math.abs(Math.round(ht) - ft) || 1,
                                     Ct = (b + N) * nt + Ft,
-                                    jt = Math.abs(Math.round(Ct) - J) || 1;
-                                return S.setTransform(0, Math.sign(nt), Math.sign(ct), 0, ft, J), S.drawImage(i, n, s, o, h, 0, 0, jt, Et), S.setTransform(Q, nt, ct, yt, ut, Ft), [jt, Et];
+                                    Ut = Math.abs(Math.round(Ct) - J) || 1;
+                                return S.setTransform(0, Math.sign(nt), Math.sign(ct), 0, ft, J), S.drawImage(i, n, s, o, h, 0, 0, Ut, Et), S.setTransform(Q, nt, ct, yt, ut, Ft), [Ut, Et];
                             }
                             S.drawImage(i, n, s, o, h, b, M, N, tt);
                             const Bt = Math.hypot(Q, nt),
                                 St = Math.hypot(ct, yt);
                             return [Bt * N, St * tt];
                         }
 
@@ -5048,18 +5048,18 @@
                                     K = 4294967295,
                                     J = l.FeatureTest.isLittleEndian ? 4278190080 : 255;
                                 for (ct = 0; ct < b; ct++) {
                                     for (ut = ct < h ? x : o, tt = 0, yt = 0; yt < ut; yt++) {
                                         const ht = Bt - N;
                                         let Et = 0;
                                         const Ct = ht > ft ? s : ht * 8 - 7,
-                                            jt = Ct & -8;
+                                            Ut = Ct & -8;
                                         let Gt = 0,
                                             Ht = 0;
-                                        for (; Et < jt; Et += 8)
+                                        for (; Et < Ut; Et += 8)
                                             Ht = Q[N++], St[tt++] = Ht & 128 ? K : J, St[tt++] = Ht & 64 ? K : J, St[tt++] = Ht & 32 ? K : J, St[tt++] = Ht & 16 ? K : J, St[tt++] = Ht & 8 ? K : J, St[tt++] = Ht & 4 ? K : J, St[tt++] = Ht & 2 ? K : J, St[tt++] = Ht & 1 ? K : J;
                                         for (; Et < Ct; Et++)
                                             Gt === 0 && (Ht = Q[N++], Gt = 128), St[tt++] = Ht & Gt ? K : J, Gt >>= 1;
                                     }
                                     for (; tt < Dt;)
                                         St[tt++] = 0;
                                     S.putImageData(M, 0, ct * x);
@@ -5286,19 +5286,19 @@
                                         M = (0, P.getCurrentTransform)(n);
                                     let N, tt, Q, nt;
                                     if ((i.bitmap || i.data) && i.count > 1) {
                                         const Et = i.bitmap || i.data.buffer;
                                         tt = JSON.stringify(b ? M : [M.slice(0, 4), h]), N = this._cachedBitmapsMap.get(Et), N || (N = /* @__PURE__ */ new Map(), this._cachedBitmapsMap.set(Et, N));
                                         const Ct = N.get(tt);
                                         if (Ct && !b) {
-                                            const jt = Math.round(Math.min(M[0], M[2]) + M[4]),
+                                            const Ut = Math.round(Math.min(M[0], M[2]) + M[4]),
                                                 Gt = Math.round(Math.min(M[1], M[3]) + M[5]);
                                             return {
                                                 canvas: Ct,
-                                                offsetX: jt,
+                                                offsetX: Ut,
                                                 offsetY: Gt
                                             };
                                         }
                                         Q = Ct;
                                     }
                                     Q || (nt = this.cachedCanvases.getCanvas("maskCanvas", s, o), y(nt.context, i));
                                     let ct = l.Util.transform(M, [1 / s, 0, 0, -1 / o, 0, 0]);
@@ -5653,36 +5653,36 @@
                                         const ht = i[J];
                                         if (typeof ht == "number") {
                                             K += yt * ht * o / 1e3;
                                             continue;
                                         }
                                         let Et = !1;
                                         const Ct = (ht.isSpace ? N : 0) + M,
-                                            jt = ht.fontChar,
+                                            Ut = ht.fontChar,
                                             Gt = ht.accent;
                                         let Ht, Xt, Vt = ht.width;
                                         if (ct) {
                                             const $t = ht.vmetric || ut,
                                                 ot = -(ht.vmetric ? $t[1] : Vt * 0.5) * Ft,
                                                 Y = $t[2] * Ft;
                                             Vt = $t ? -$t[0] : Vt, Ht = ot / b, Xt = (K + Y) / b;
                                         } else
                                             Ht = K / b, Xt = 0;
                                         if (s.remeasure && Vt > 0) {
-                                            const $t = h.measureText(jt).width * 1e3 / o * b;
+                                            const $t = h.measureText(Ut).width * 1e3 / o * b;
                                             if (Vt < $t && this.isFontSubpixelAAEnabled) {
                                                 const ot = Vt / $t;
                                                 Et = !0, h.save(), h.scale(ot, 1), Ht /= ot;
                                             } else
                                                 Vt !== $t && (Ht += (Vt - $t) / 2e3 * o / b);
                                         }
                                         if (this.contentVisible && (ht.isInFont || s.missingFile)) {
                                             if (Bt && !Gt)
-                                                h.fillText(jt, Ht, Xt);
-                                            else if (this.paintChar(jt, Ht, Xt, St), Gt) {
+                                                h.fillText(Ut, Ht, Xt);
+                                            else if (this.paintChar(Ut, Ht, Xt, St), Gt) {
                                                 const $t = Ht + o * Gt.offset.x / b,
                                                     ot = Xt - o * Gt.offset.y / b;
                                                 this.paintChar(Gt.fontChar, $t, ot, St);
                                             }
                                         }
                                         const Wt = ct ? Vt * Ft - Ct * tt : Vt * Ft + Ct * tt;
                                         K += Wt, Et && h.restore();
@@ -9983,15 +9983,15 @@
                         }, ee(V, "_freeTextDefaultContent", ""), ee(V, "_internalPadding", 0), ee(V, "_defaultColor", null), ee(V, "_defaultFontSize", 10), ee(V, "_type", "freetext");
                         let pt = V;
                         d.FreeTextEditor = pt;
                     },
                     /* 29 */
                     /***/
                     (dt, d, et) => {
-                        var n, o, ce, b, Ii, N, tt, Q, nt, ct, yt, ut, Ft, Bt, St, Dt, ft, K, J, ht, Et, Ct, jt, Li, Ht, Fe, Vt, ai, $t, oi, Y, G, bt, At, te, Zt, $, li, Lt, Tt, Ot, Nt, Oi, _t, ci;
+                        var n, o, ce, b, Ii, N, tt, Q, nt, ct, yt, ut, Ft, Bt, St, Dt, ft, K, J, ht, Et, Ct, Ut, Li, Ht, Fe, Vt, ai, $t, oi, Y, G, bt, At, te, Zt, $, li, Lt, Tt, Ot, Nt, Oi, _t, ci;
                         Object.defineProperty(d, "__esModule", {
                             value: !0
                         }), d.StampAnnotationElement = d.InkAnnotationElement = d.FreeTextAnnotationElement = d.AnnotationLayer = void 0;
                         var l = et(1),
                             P = et(6),
                             rt = et(3),
                             X = et(30),
@@ -10093,28 +10093,28 @@
                                     pageWidth: q,
                                     pageHeight: it,
                                     pageX: mt,
                                     pageY: kt
                                 } = D.rawDims;
                                 if (!e.rect || this instanceof p) {
                                     const {
-                                        rotation: Ut
+                                        rotation: jt
                                     } = e;
-                                    return !e.hasOwnCanvas && Ut !== 0 && this.setRotation(Ut, j), j;
+                                    return !e.hasOwnCanvas && jt !== 0 && this.setRotation(jt, j), j;
                                 }
                                 const {
                                     width: Pt,
                                     height: zt
                                 } = I(e.rect), Mt = l.Util.normalizeRect([e.rect[0], f.view[3] - e.rect[1] + f.view[1], e.rect[2], f.view[3] - e.rect[3] + f.view[1]]);
                                 if (!R && e.borderStyle.width > 0) {
                                     j.style.borderWidth = `${e.borderStyle.width}px`;
-                                    const Ut = e.borderStyle.horizontalCornerRadius,
+                                    const jt = e.borderStyle.horizontalCornerRadius,
                                         qt = e.borderStyle.verticalCornerRadius;
-                                    if (Ut > 0 || qt > 0) {
-                                        const Qt = `calc(${Ut}px * var(--scale-factor)) / calc(${qt}px * var(--scale-factor))`;
+                                    if (jt > 0 || qt > 0) {
+                                        const Qt = `calc(${jt}px * var(--scale-factor)) / calc(${qt}px * var(--scale-factor))`;
                                         j.style.borderRadius = Qt;
                                     } else if (this instanceof a) {
                                         const Qt = `calc(${Pt}px * var(--scale-factor)) / calc(${zt}px * var(--scale-factor))`;
                                         j.style.borderRadius = Qt;
                                     }
                                     switch (e.borderStyle.style) {
                                         case l.AnnotationBorderStyleType.SOLID:
@@ -10292,31 +10292,31 @@
                                         svgFactory: Pt
                                     } = this,
                                     zt = Pt.createElement("svg");
                                 zt.classList.add("quadrilateralsContainer"), zt.setAttribute("width", 0), zt.setAttribute("height", 0);
                                 const Mt = Pt.createElement("defs");
                                 zt.append(Mt);
                                 const Rt = Pt.createElement("clipPath"),
-                                    Ut = `clippath_${this.data.id}`;
-                                Rt.setAttribute("id", Ut), Rt.setAttribute("clipPathUnits", "objectBoundingBox"), Mt.append(Rt);
+                                    jt = `clippath_${this.data.id}`;
+                                Rt.setAttribute("id", jt), Rt.setAttribute("clipPathUnits", "objectBoundingBox"), Mt.append(Rt);
                                 for (const [, {
                                         x: qt,
                                         y: Kt
                                     }, {
                                         x: Qt,
                                         y: se
                                     }] of R) {
                                     const ie = Pt.createElement("rect"),
                                         ne = (Qt - e) / mt,
                                         oe = (j - Kt) / kt,
                                         le = (qt - Qt) / mt,
                                         _i = (Kt - se) / kt;
                                     ie.setAttribute("x", ne), ie.setAttribute("y", oe), ie.setAttribute("width", le), ie.setAttribute("height", _i), Rt.append(ie), it == null || it.push(`<rect vector-effect="non-scaling-stroke" x="${ne}" y="${oe}" width="${le}" height="${_i}"/>`);
                                 }
-                                t(this, n) && (it.push("</g></svg>')"), q.backgroundImage = it.join("")), this.container.append(zt), this.container.style.clipPath = `url(#${Ut})`;
+                                t(this, n) && (it.push("</g></svg>')"), q.backgroundImage = it.join("")), this.container.append(zt), this.container.style.clipPath = `url(#${jt})`;
                             }
                             _createPopup() {
                                 const {
                                     container: R,
                                     data: e
                                 } = this;
                                 R.setAttribute("aria-haspopup", "dialog");
@@ -10484,24 +10484,24 @@
                                         fields: j,
                                         refs: q,
                                         include: it
                                     } = f, mt = [];
                                     if (j.length !== 0 || q.length !== 0) {
                                         const Mt = new Set(q);
                                         for (const Rt of j) {
-                                            const Ut = this._fieldObjects[Rt] || [];
+                                            const jt = this._fieldObjects[Rt] || [];
                                             for (const {
                                                     id: qt
                                                 }
-                                                of Ut)
+                                                of jt)
                                                 Mt.add(qt);
                                         }
                                         for (const Rt of Object.values(this._fieldObjects))
-                                            for (const Ut of Rt)
-                                                Mt.has(Ut.id) === it && mt.push(Ut);
+                                            for (const jt of Rt)
+                                                Mt.has(jt.id) === it && mt.push(jt);
                                     } else
                                         for (const Mt of Object.values(this._fieldObjects))
                                             mt.push(...Mt);
                                     const kt = this.annotationStorage,
                                         Pt = [];
                                     for (const Mt of mt) {
                                         const {
@@ -10530,23 +10530,23 @@
                                                     value: qt
                                                 });
                                                 break;
                                             }
                                             default:
                                                 continue;
                                         }
-                                        const Ut = document.querySelector(`[data-element-id="${Rt}"]`);
-                                        if (Ut) {
-                                            if (!O.has(Ut)) {
+                                        const jt = document.querySelector(`[data-element-id="${Rt}"]`);
+                                        if (jt) {
+                                            if (!O.has(jt)) {
                                                 (0, l.warn)(`_bindResetFormAction - element not allowed: ${Rt}`);
                                                 continue;
                                             }
                                         } else
                                             continue;
-                                        Ut.dispatchEvent(new Event("resetform"));
+                                        jt.dispatchEvent(new Event("resetform"));
                                     }
                                     return this.enableScripting && ((zt = this.linkService.eventBus) == null || zt.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: "app",
                                             ids: Pt,
                                             name: "ResetForm"
@@ -10713,20 +10713,20 @@
                                         Rt != null && (Mt.target.value = Rt), Mt.target.scrollLeft = 0;
                                     };
                                     if (this.enableScripting && this.hasJSActions) {
                                         f.addEventListener("focus", (Rt) => {
                                             if (Pt.focused)
                                                 return;
                                             const {
-                                                target: Ut
+                                                target: jt
                                             } = Rt;
-                                            Pt.userValue && (Ut.value = Pt.userValue), Pt.lastCommittedValue = Ut.value, Pt.commitKey = 1, Pt.focused = !0;
+                                            Pt.userValue && (jt.value = Pt.userValue), Pt.lastCommittedValue = jt.value, Pt.commitKey = 1, Pt.focused = !0;
                                         }), f.addEventListener("updatefromsandbox", (Rt) => {
                                             this.showElementAndHideCanvas(Rt.target);
-                                            const Ut = {
+                                            const jt = {
                                                 value(qt) {
                                                     Pt.userValue = qt.detail.value ?? "", R.setValue(e, {
                                                         value: Pt.userValue.toString()
                                                     }), qt.target.value = Pt.userValue;
                                                 },
                                                 formattedValue(qt) {
                                                     const {
@@ -10764,63 +10764,63 @@
                                                             commitKey: 1,
                                                             selStart: Qt.selectionStart,
                                                             selEnd: Qt.selectionEnd
                                                         }
                                                     }));
                                                 }
                                             };
-                                            this._dispatchEventFromSandbox(Ut, Rt);
+                                            this._dispatchEventFromSandbox(jt, Rt);
                                         }), f.addEventListener("keydown", (Rt) => {
                                             var Kt;
                                             Pt.commitKey = 1;
-                                            let Ut = -1;
-                                            if (Rt.key === "Escape" ? Ut = 0 : Rt.key === "Enter" && !this.data.multiLine ? Ut = 2 : Rt.key === "Tab" && (Pt.commitKey = 3), Ut === -1)
+                                            let jt = -1;
+                                            if (Rt.key === "Escape" ? jt = 0 : Rt.key === "Enter" && !this.data.multiLine ? jt = 2 : Rt.key === "Tab" && (Pt.commitKey = 3), jt === -1)
                                                 return;
                                             const {
                                                 value: qt
                                             } = Rt.target;
                                             Pt.lastCommittedValue !== qt && (Pt.lastCommittedValue = qt, Pt.userValue = qt, (Kt = this.linkService.eventBus) == null || Kt.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: e,
                                                     name: "Keystroke",
                                                     value: qt,
                                                     willCommit: !0,
-                                                    commitKey: Ut,
+                                                    commitKey: jt,
                                                     selStart: Rt.target.selectionStart,
                                                     selEnd: Rt.target.selectionEnd
                                                 }
                                             }));
                                         });
                                         const Mt = zt;
                                         zt = null, f.addEventListener("blur", (Rt) => {
                                             var qt;
                                             if (!Pt.focused || !Rt.relatedTarget)
                                                 return;
                                             Pt.focused = !1;
                                             const {
-                                                value: Ut
+                                                value: jt
                                             } = Rt.target;
-                                            Pt.userValue = Ut, Pt.lastCommittedValue !== Ut && ((qt = this.linkService.eventBus) == null || qt.dispatch("dispatcheventinsandbox", {
+                                            Pt.userValue = jt, Pt.lastCommittedValue !== jt && ((qt = this.linkService.eventBus) == null || qt.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: e,
                                                     name: "Keystroke",
-                                                    value: Ut,
+                                                    value: jt,
                                                     willCommit: !0,
                                                     commitKey: Pt.commitKey,
                                                     selStart: Rt.target.selectionStart,
                                                     selEnd: Rt.target.selectionEnd
                                                 }
                                             })), Mt(Rt);
                                         }), (j = this.data.actions) != null && j.Keystroke && f.addEventListener("beforeinput", (Rt) => {
                                             var oe;
                                             Pt.lastCommittedValue = null;
                                             const {
-                                                data: Ut,
+                                                data: jt,
                                                 target: qt
                                             } = Rt, {
                                                 value: Kt,
                                                 selectionStart: Qt,
                                                 selectionEnd: se
                                             } = qt;
                                             let ie = Qt,
@@ -10845,15 +10845,15 @@
                                             }
                                             Rt.preventDefault(), (oe = this.linkService.eventBus) == null || oe.dispatch("dispatcheventinsandbox", {
                                                 source: this,
                                                 detail: {
                                                     id: e,
                                                     name: "Keystroke",
                                                     value: Kt,
-                                                    change: Ut || "",
+                                                    change: jt || "",
                                                     willCommit: !1,
                                                     selStart: ie,
                                                     selEnd: ne
                                                 }
                                             });
                                         }), this._setEventListeners(f, Pt, [
                                             ["focus", "Focus"],
@@ -11046,43 +11046,43 @@
                                 }
                                 const it = (Pt) => {
                                     const zt = Pt ? "value" : "textContent",
                                         {
                                             options: Mt,
                                             multiple: Rt
                                         } = D;
-                                    return Rt ? Array.prototype.filter.call(Mt, (Ut) => Ut.selected).map((Ut) => Ut[zt]) : Mt.selectedIndex === -1 ? null : Mt[Mt.selectedIndex][zt];
+                                    return Rt ? Array.prototype.filter.call(Mt, (jt) => jt.selected).map((jt) => jt[zt]) : Mt.selectedIndex === -1 ? null : Mt[Mt.selectedIndex][zt];
                                 };
                                 let mt = it(!1);
                                 const kt = (Pt) => {
                                     const zt = Pt.target.options;
                                     return Array.prototype.map.call(zt, (Mt) => ({
                                         displayValue: Mt.textContent,
                                         exportValue: Mt.value
                                     }));
                                 };
                                 return this.enableScripting && this.hasJSActions ? (D.addEventListener("updatefromsandbox", (Pt) => {
                                     const zt = {
                                         value(Mt) {
                                             q == null || q();
                                             const Rt = Mt.detail.value,
-                                                Ut = new Set(Array.isArray(Rt) ? Rt : [Rt]);
+                                                jt = new Set(Array.isArray(Rt) ? Rt : [Rt]);
                                             for (const qt of D.options)
-                                                qt.selected = Ut.has(qt.value);
+                                                qt.selected = jt.has(qt.value);
                                             R.setValue(e, {
                                                 value: it(!0)
                                             }), mt = it(!1);
                                         },
                                         multipleSelection(Mt) {
                                             D.multiple = !0;
                                         },
                                         remove(Mt) {
                                             const Rt = D.options,
-                                                Ut = Mt.detail.remove;
-                                            Rt[Ut].selected = !1, D.remove(Ut), Rt.length > 0 && Array.prototype.findIndex.call(Rt, (Kt) => Kt.selected) === -1 && (Rt[0].selected = !0), R.setValue(e, {
+                                                jt = Mt.detail.remove;
+                                            Rt[jt].selected = !1, D.remove(jt), Rt.length > 0 && Array.prototype.findIndex.call(Rt, (Kt) => Kt.selected) === -1 && (Rt[0].selected = !0), R.setValue(e, {
                                                 value: it(!0),
                                                 items: kt(Mt)
                                             }), mt = it(!1);
                                         },
                                         clear(Mt) {
                                             for (; D.length !== 0;)
                                                 D.remove(0);
@@ -11090,44 +11090,44 @@
                                                 value: null,
                                                 items: []
                                             }), mt = it(!1);
                                         },
                                         insert(Mt) {
                                             const {
                                                 index: Rt,
-                                                displayValue: Ut,
+                                                displayValue: jt,
                                                 exportValue: qt
                                             } = Mt.detail.insert, Kt = D.children[Rt], Qt = document.createElement("option");
-                                            Qt.textContent = Ut, Qt.value = qt, Kt ? Kt.before(Qt) : D.append(Qt), R.setValue(e, {
+                                            Qt.textContent = jt, Qt.value = qt, Kt ? Kt.before(Qt) : D.append(Qt), R.setValue(e, {
                                                 value: it(!0),
                                                 items: kt(Mt)
                                             }), mt = it(!1);
                                         },
                                         items(Mt) {
                                             const {
                                                 items: Rt
                                             } = Mt.detail;
                                             for (; D.length !== 0;)
                                                 D.remove(0);
-                                            for (const Ut of Rt) {
+                                            for (const jt of Rt) {
                                                 const {
                                                     displayValue: qt,
                                                     exportValue: Kt
-                                                } = Ut, Qt = document.createElement("option");
+                                                } = jt, Qt = document.createElement("option");
                                                 Qt.textContent = qt, Qt.value = Kt, D.append(Qt);
                                             }
                                             D.options.length > 0 && (D.options[0].selected = !0), R.setValue(e, {
                                                 value: it(!0),
                                                 items: kt(Mt)
                                             }), mt = it(!1);
                                         },
                                         indices(Mt) {
                                             const Rt = new Set(Mt.detail.indices);
-                                            for (const Ut of Mt.target.options)
-                                                Ut.selected = Rt.has(Ut.index);
+                                            for (const jt of Mt.target.options)
+                                                jt.selected = Rt.has(jt.index);
                                             R.setValue(e, {
                                                 value: it(!0)
                                             }), mt = it(!1);
                                         },
                                         editable(Mt) {
                                             Mt.target.disabled = !Mt.detail.editable;
                                         }
@@ -11207,20 +11207,20 @@
                                 contentsObj: q,
                                 richText: it,
                                 parent: mt,
                                 rect: kt,
                                 parentRect: Pt,
                                 open: zt
                             }) {
-                                L(this, jt);
+                                L(this, Ut);
                                 L(this, Ht);
                                 L(this, Vt);
                                 L(this, $t);
                                 L(this, N, null);
-                                L(this, tt, W(this, jt, Li).bind(this));
+                                L(this, tt, W(this, Ut, Li).bind(this));
                                 L(this, Q, W(this, $t, oi).bind(this));
                                 L(this, nt, W(this, Vt, ai).bind(this));
                                 L(this, ct, W(this, Ht, Fe).bind(this));
                                 L(this, yt, null);
                                 L(this, ut, null);
                                 L(this, Ft, null);
                                 L(this, Bt, null);
@@ -11234,19 +11234,19 @@
                                 L(this, Ct, !1);
                                 var Rt;
                                 Z(this, ut, R), Z(this, Et, D), Z(this, Ft, q), Z(this, ht, it), Z(this, St, mt), Z(this, yt, e), Z(this, J, kt), Z(this, Dt, Pt), Z(this, Bt, f);
                                 const Mt = P.PDFDateString.toDateObject(j);
                                 Mt && Z(this, N, mt.l10n.get("annotation_date_string", {
                                     date: Mt.toLocaleDateString(),
                                     time: Mt.toLocaleTimeString()
-                                })), this.trigger = f.flatMap((Ut) => Ut.getElementsToTriggerPopup());
-                                for (const Ut of this.trigger)
-                                    Ut.addEventListener("click", t(this, ct)), Ut.addEventListener("mouseenter", t(this, nt)), Ut.addEventListener("mouseleave", t(this, Q)), Ut.classList.add("popupTriggerArea");
-                                for (const Ut of f)
-                                    (Rt = Ut.container) == null || Rt.addEventListener("keydown", t(this, tt));
+                                })), this.trigger = f.flatMap((jt) => jt.getElementsToTriggerPopup());
+                                for (const jt of this.trigger)
+                                    jt.addEventListener("click", t(this, ct)), jt.addEventListener("mouseenter", t(this, nt)), jt.addEventListener("mouseleave", t(this, Q)), jt.classList.add("popupTriggerArea");
+                                for (const jt of f)
+                                    (Rt = jt.container) == null || Rt.addEventListener("keydown", t(this, tt));
                                 t(this, ut).hidden = !0, zt && W(this, Ht, Fe).call(this);
                             }
                             render() {
                                 if (t(this, K))
                                     return;
                                 const {
                                     page: {
@@ -11293,16 +11293,15 @@
                                     Mt = zt ? t(this, Dt) : t(this, J);
                                 for (const ie of t(this, Bt))
                                     if (!Mt || l.Util.intersect(ie.data.rect, Mt) !== null) {
                                         Mt = ie.data.rect, zt = !0;
                                         break;
                                     }
                                 const Rt = l.Util.normalizeRect([Mt[0], R[3] - Mt[1] + R[1], Mt[2], R[3] - Mt[3] + R[1]]),
-                                    Ut = 5,
-                                    qt = zt ? Mt[2] - Mt[0] + Ut : 0,
+                                    qt = zt ? Mt[2] - Mt[0] + 5 : 0,
                                     Kt = Rt[0] + qt,
                                     Qt = Rt[1],
                                     {
                                         style: se
                                     } = t(this, ut);
                                 se.left = `${100 * (Kt - D) / e}%`, se.top = `${100 * (Qt - j) / f}%`, t(this, ut).append(q);
                             }
@@ -11325,15 +11324,15 @@
                             maybeShow() {
                                 t(this, Ct) && (Z(this, Ct, !1), t(this, ut).hidden = !1);
                             }
                             get isVisible() {
                                 return t(this, ut).hidden === !1;
                             }
                         }
-                        N = new WeakMap(), tt = new WeakMap(), Q = new WeakMap(), nt = new WeakMap(), ct = new WeakMap(), yt = new WeakMap(), ut = new WeakMap(), Ft = new WeakMap(), Bt = new WeakMap(), St = new WeakMap(), Dt = new WeakMap(), ft = new WeakMap(), K = new WeakMap(), J = new WeakMap(), ht = new WeakMap(), Et = new WeakMap(), Ct = new WeakMap(), jt = new WeakSet(), Li = function(R) {
+                        N = new WeakMap(), tt = new WeakMap(), Q = new WeakMap(), nt = new WeakMap(), ct = new WeakMap(), yt = new WeakMap(), ut = new WeakMap(), Ft = new WeakMap(), Bt = new WeakMap(), St = new WeakMap(), Dt = new WeakMap(), ft = new WeakMap(), K = new WeakMap(), J = new WeakMap(), ht = new WeakMap(), Et = new WeakMap(), Ct = new WeakMap(), Ut = new WeakSet(), Li = function(R) {
                             R.altKey || R.shiftKey || R.ctrlKey || R.metaKey || (R.key === "Enter" || R.key === "Escape" && t(this, ft)) && W(this, Ht, Fe).call(this);
                         }, Ht = new WeakSet(), Fe = function() {
                             Z(this, ft, !t(this, ft)), t(this, ft) ? (W(this, Vt, ai).call(this), t(this, ut).addEventListener("click", t(this, ct)), t(this, ut).addEventListener("keydown", t(this, tt))) : (W(this, $t, oi).call(this), t(this, ut).removeEventListener("click", t(this, ct)), t(this, ut).removeEventListener("keydown", t(this, tt)));
                         }, Vt = new WeakSet(), ai = function() {
                             t(this, K) || this.render(), this.isVisible ? t(this, ft) && t(this, ut).classList.add("focused") : (t(this, ut).hidden = !1, t(this, ut).style.zIndex = parseInt(t(this, ut).style.zIndex) + 1e3);
                         }, $t = new WeakSet(), oi = function() {
                             t(this, ut).classList.remove("focused"), !(t(this, ft) || !this.isVisible) && (t(this, ut).hidden = !0, t(this, ut).style.zIndex = parseInt(t(this, ut).style.zIndex) - 1e3);
@@ -12242,15 +12241,15 @@
                                     }
                                     of R) {
                                     mt = W(j = At, Gt, $i).call(j, mt, e, f);
                                     const kt = [];
                                     Tt.paths.push(kt);
                                     let Pt = Yt * (mt[0] - It),
                                         zt = Yt * (mt[1] - It);
-                                    for (let Rt = 2, Ut = mt.length; Rt < Ut; Rt += 6) {
+                                    for (let Rt = 2, jt = mt.length; Rt < jt; Rt += 6) {
                                         const qt = Yt * (mt[Rt] - It),
                                             Kt = Yt * (mt[Rt + 1] - It),
                                             Qt = Yt * (mt[Rt + 2] - It),
                                             se = Yt * (mt[Rt + 3] - It),
                                             ie = Yt * (mt[Rt + 4] - It),
                                             ne = Yt * (mt[Rt + 5] - It);
                                         kt.push([
@@ -12544,16 +12543,16 @@
                                 Nt = this.thickness / 2,
                                 Jt = $ * vt + Nt,
                                 _t = $ * Lt + Nt;
                             for (const R of this.paths) {
                                 const e = [],
                                     f = [];
                                 for (let D = 0, j = R.length; D < j; D++) {
-                                    const [q, it, mt, kt] = R[D], Pt = $ * q[0] + Jt, zt = $ * q[1] + _t, Mt = $ * it[0] + Jt, Rt = $ * it[1] + _t, Ut = $ * mt[0] + Jt, qt = $ * mt[1] + _t, Kt = $ * kt[0] + Jt, Qt = $ * kt[1] + _t;
-                                    D === 0 && (e.push(Pt, zt), f.push(Pt, zt)), e.push(Mt, Rt, Ut, qt, Kt, Qt), f.push(Mt, Rt), D === j - 1 && f.push(Kt, Qt);
+                                    const [q, it, mt, kt] = R[D], Pt = $ * q[0] + Jt, zt = $ * q[1] + _t, Mt = $ * it[0] + Jt, Rt = $ * it[1] + _t, jt = $ * mt[0] + Jt, qt = $ * mt[1] + _t, Kt = $ * kt[0] + Jt, Qt = $ * kt[1] + _t;
+                                    D === 0 && (e.push(Pt, zt), f.push(Pt, zt)), e.push(Mt, Rt, jt, qt, Kt, Qt), f.push(Mt, Rt), D === j - 1 && f.push(Kt, Qt);
                                 }
                                 Ot.push({
                                     bezier: W(Yt = At, Ct, pi).call(Yt, e, Tt, this.rotation),
                                     points: W(It = At, Ct, pi).call(It, f, Tt, this.rotation)
                                 });
                             }
                             return Ot;
```

### Comparing `gradio_pdf-0.0.5/demo/_app.py` & `gradio_pdf-0.0.6/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/demo/app.py` & `gradio_pdf-0.0.6/demo/space.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import gradio as gr
-from _app import demo as app
+from app import demo as app
 import os
 
-_docs = {'PDF': {'description': 'A base class for defining methods that all input/output components should have.', 'members': {'__init__': {'value': {'type': 'Any', 'default': 'None', 'description': None}, 'height': {'type': 'int | None', 'default': 'None', 'description': None}, 'label': {'type': 'str | None', 'default': 'None', 'description': None}, 'info': {'type': 'str | None', 'default': 'None', 'description': None}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': None}, 'container': {'type': 'bool', 'default': 'True', 'description': None}, 'scale': {'type': 'int | None', 'default': 'None', 'description': None}, 'min_width': {'type': 'int | None', 'default': 'None', 'description': None}, 'interactive': {'type': 'bool | None', 'default': 'None', 'description': None}, 'visible': {'type': 'bool', 'default': 'True', 'description': None}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': None}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': None}, 'render': {'type': 'bool', 'default': 'True', 'description': None}, 'load_fn': {'type': 'Callable[..., Any] | None', 'default': 'None', 'description': None}, 'every': {'type': 'float | None', 'default': 'None', 'description': None}}, 'postprocess': {'value': {'type': 'str | None', 'description': None}}, 'preprocess': {'return': {'type': 'str', 'description': None}, 'value': None}}, 'events': {'change': {'type': None, 'default': None, 'description': ''}, 'upload': {'type': None, 'default': None, 'description': ''}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'PDF': []}}}
-    
+_docs = {'PDF': {'description': 'A base class for defining methods that all input/output components should have.', 'members': {'__init__': {'value': {'type': 'typing.Any', 'default': 'None', 'description': None}, 'height': {'type': 'int | None', 'default': 'None', 'description': None}, 'label': {'type': 'str | None', 'default': 'None', 'description': None}, 'info': {'type': 'str | None', 'default': 'None', 'description': None}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': None}, 'container': {'type': 'bool', 'default': 'True', 'description': None}, 'scale': {'type': 'int | None', 'default': 'None', 'description': None}, 'min_width': {'type': 'int | None', 'default': 'None', 'description': None}, 'interactive': {'type': 'bool | None', 'default': 'None', 'description': None}, 'visible': {'type': 'bool', 'default': 'True', 'description': None}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': None}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': None}, 'render': {'type': 'bool', 'default': 'True', 'description': None}, 'load_fn': {'type': 'Callable[Ellipsis, typing.Any] | None', 'default': 'None', 'description': None}, 'every': {'type': 'float | None', 'default': 'None', 'description': None}}, 'postprocess': {'value': {'type': 'str | None', 'description': "The output data received by the component from the user's function in the backend."}}, 'preprocess': {'return': {'type': 'str', 'description': "The preprocessed input data sent to the user's function in the backend."}, 'value': None}}, 'events': {'change': {'type': None, 'default': None, 'description': ''}, 'upload': {'type': None, 'default': None, 'description': ''}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'PDF': []}}}
+
 abs_path = os.path.join(os.path.dirname(__file__), "css.css")
 
 with gr.Blocks(
     css=abs_path,
     theme=gr.themes.Default(
         font_mono=[
             gr.themes.GoogleFont("Inconsolata"),
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_pdf`
 
 <div style="display: flex; gap: 7px;">
-<a href="https://pypi.org/project/gradio_pdf/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_pdf"></a> <a href="https://github.com/freddyaboulton/gradio-pdf/issues" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/Issues-white?logo=github&logoColor=black"></a> <a href="https://huggingface.co/spaces/freddyaboulton/gradio_pdf/discussions" target="_blank"><img alt="Static Badge" src="https://img.shields.io/badge/%F0%9F%A4%97%20Discuss-%23097EFF?style=flat&logoColor=black"></a>
+<a href="https://pypi.org/project/gradio_pdf/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_pdf"></a>  
 </div>
 
 Easily display PDFs in Gradio
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
@@ -90,20 +90,21 @@
 
     gr.Markdown("""
 
 ### User function
 
 The impact on the users predict function varies depending on whether the component is used as an input or output for an event (or both).
 
-- When used as an Input, the component only impacts the input signature of the user function. 
-- When used as an output, the component only impacts the return signature of the user function. 
+- When used as an Input, the component only impacts the input signature of the user function.
+- When used as an output, the component only impacts the return signature of the user function.
 
 The code snippet below is accurate in cases where the component is used as both an input and an output.
 
-
+- **As input:** Is passed, the preprocessed input data sent to the user's function in the backend.
+- **As output:** Should return, the output data received by the component from the user's function in the backend.
 
  ```python
 def predict(
     value: str
 ) -> str | None:
     return value
 ```
@@ -126,15 +127,15 @@
                     el.innerHTML = el.innerHTML.replace(
                         new RegExp("\\b"+ref+"\\b", "g"),
                         `<a href="#h-${ref.toLowerCase()}">${ref}</a>`
                     );
                 })
             }
         })
-        
+
         Object.entries(refs).forEach(([key, refs]) => {
             if (refs.length > 0) {
                 const el = document.querySelector(`.${key}`);
                 if (!el) return;
                 refs.forEach(ref => {
                     el.innerHTML = el.innerHTML.replace(
                         new RegExp("\\b"+ref+"\\b", "g"),
```

### Comparing `gradio_pdf-0.0.5/demo/contract.pdf` & `gradio_pdf-0.0.6/demo/contract.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/demo/css.css` & `gradio_pdf-0.0.6/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/demo/invoice_2.pdf` & `gradio_pdf-0.0.6/demo/invoice_2.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/demo/sample_invoice.pdf` & `gradio_pdf-0.0.6/demo/sample_invoice.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/frontend/Example.svelte` & `gradio_pdf-0.0.6/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/frontend/Index.svelte` & `gradio_pdf-0.0.6/frontend/Index.svelte`

 * *Files 6% similar despite different names*

```diff
@@ -38,21 +38,23 @@
 		let currentPage = 1;
 		let canvasRef;
 
 		async function handle_clear() {
 			_value = null;
 			await tick();
 			gradio.dispatch("change");
+			currentPage = 1;
 		}
 
 		async function handle_upload({detail}: CustomEvent<FileData>): Promise<void> {
 			value = detail;
 			await tick();
 			gradio.dispatch("change");
 			gradio.dispatch("upload");
+			currentPage = 1;
 		}
 
 
 		async function get_doc(value: FileData) {
 			const loadingTask = pdfjsLib.getDocument(value.url);
 			pdfDoc = await loadingTask.promise;
 			numPages = pdfDoc.numPages;
```

### Comparing `gradio_pdf-0.0.5/frontend/PdfUploadText.svelte` & `gradio_pdf-0.0.6/frontend/PdfUploadText.svelte`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/frontend/package-lock.json` & `gradio_pdf-0.0.6/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/frontend/package.json` & `gradio_pdf-0.0.6/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.5/pyproject.toml` & `gradio_pdf-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_pdf"
-version = "0.0.5"
+version = "0.0.6"
 description = "Easily display PDFs in Gradio"
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" }]
 keywords = [
   "Documents",
@@ -38,16 +38,12 @@
   'Topic :: Scientific/Engineering :: Artificial Intelligence',
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
-[project.urls]
-repository = "https://github.com/freddyaboulton/gradio-pdf"
-space = "https://huggingface.co/spaces/freddyaboulton/gradio_pdf"
-
 [tool.hatch.build]
 artifacts = ["/backend/gradio_pdf/templates", "*.pyi", "backend/gradio_pdf/templates", "backend/gradio_pdf/templates", "backend/gradio_pdf/templates", "backend/gradio_pdf/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_pdf"]
```

