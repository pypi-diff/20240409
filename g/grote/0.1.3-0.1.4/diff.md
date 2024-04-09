# Comparing `tmp/grote-0.1.3.tar.gz` & `tmp/grote-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grote-0.1.3.tar", max compression
+gzip compressed data, was "grote-0.1.4.tar", max compression
```

## Comparing `grote-0.1.3.tar` & `grote-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.3/LICENSE
--rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.3/README.md
--rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.3/grote/__init__.py
--rw-r--r--   0        0        0      994 2024-02-14 09:45:46.262120 grote-0.1.3/grote/app.py
--rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.3/grote/collections/__init__.py
--rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.3/grote/collections/base.py
--rw-r--r--   0        0        0     1247 2024-02-14 16:49:31.321680 grote-0.1.3/grote/collections/config.yaml
--rw-r--r--   0        0        0     4033 2024-02-14 09:56:03.919866 grote-0.1.3/grote/collections/load.py
--rw-r--r--   0        0        0     7878 2024-02-14 16:47:24.260880 grote-0.1.3/grote/collections/translate.py
--rw-r--r--   0        0        0     1855 2024-02-13 15:36:18.636884 grote-0.1.3/grote/config.py
--rw-r--r--   0        0        0      231 2024-02-14 16:45:55.348690 grote-0.1.3/grote/config.yaml
--rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.3/grote/event_logging.py
--rw-r--r--   0        0        0      565 2024-02-13 15:46:02.979763 grote-0.1.3/grote/functions/__init__.py
--rw-r--r--   0        0        0     5314 2024-02-14 09:55:54.594248 grote-0.1.3/grote/functions/load.py
--rw-r--r--   0        0        0     2777 2024-02-03 12:47:59.873196 grote-0.1.3/grote/functions/translate.py
--rw-r--r--   0        0        0      412 2024-02-14 09:45:37.035928 grote-0.1.3/grote/style.py
--rw-r--r--   0        0        0     3659 2024-02-14 16:50:04.377076 grote-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.4/README.md
+-rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.4/grote/__init__.py
+-rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.4/grote/app.py
+-rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.4/grote/collections/__init__.py
+-rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.4/grote/collections/base.py
+-rw-r--r--   0        0        0     1338 2024-04-09 15:45:56.211676 grote-0.1.4/grote/collections/config.yaml
+-rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.4/grote/collections/load.py
+-rw-r--r--   0        0        0     8448 2024-04-09 15:48:52.382493 grote-0.1.4/grote/collections/translate.py
+-rw-r--r--   0        0        0     1855 2024-02-13 15:36:18.636884 grote-0.1.4/grote/config.py
+-rw-r--r--   0        0        0      231 2024-02-14 16:45:55.348690 grote-0.1.4/grote/config.yaml
+-rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.4/grote/event_logging.py
+-rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.4/grote/functions/__init__.py
+-rw-r--r--   0        0        0     5543 2024-04-09 15:48:39.327509 grote-0.1.4/grote/functions/load.py
+-rw-r--r--   0        0        0     3360 2024-04-09 15:48:39.327563 grote-0.1.4/grote/functions/translate.py
+-rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.4/grote/style.py
+-rw-r--r--   0        0        0     3659 2024-04-09 15:47:46.434940 grote-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.4/PKG-INFO
```

### Comparing `grote-0.1.3/LICENSE` & `grote-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `grote-0.1.3/README.md` & `grote-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `grote-0.1.3/grote/collections/base.py` & `grote-0.1.4/grote/collections/base.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.3/grote/collections/config.yaml` & `grote-0.1.4/grote/collections/config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 load:
     login_code_description: "<h3>1. 🔑 Login code: Insert the login code you received:</h3>"
     login_code_label: "Login code"
     login_code_placeholder: "Insert login code..."
     login_code_info: "If you didn't receive a login code, please contact us."
-    input_description: "<h3>2. 📝 Input sentences: Upload a file containing source sentences and translations OR insert source sentences manually:</h3>"
+    input_description: "<h3>2. 📝 Input sentences: Upload a file containing source sentences and translations in SOURCE ||| TRANSLATION format</h3>"
     file_label: "Input file"
     sentences_label: "Input sentences"
     sentences_placeholder: "Insert one sentence with format SOURCE ||| TARGET per line..."
     start_button_label: "📝 Start"
 translate:
-    source_side_label: "<h3>Source sentences</h3>"
+    source_side_label: "<h3>Source sentences</h3><p>These are the original sentences you need to translate.</p>"
     target_side_label: "<h3>Translations with&nbsp;<span style='background-color: #fee2e2; color: black;'>potential issues</span></h3><p>Use the green checkmark to remove remaining highlights after editing.</p>"
     reload_button_label: "⬅️ Back to data loading"
-    clear_button_label: "🗑️ Clear current changes"
     done_button_label: "✅ Done"
+    download_button_label: "📥 Download translations"
     source_textbox_label: "Source text"
     target_textbox_label: "Translation"
+    legend_label: "Potential issue severity"
     highlight_labels:
-        - "Minor Error"
-        - "Major Error"
+        - "Minor"
+        - "Major"
     highlight_colors:
-        - "#ccfbf1"
         - "#ffedd5"
+        - "#fcd29a"
```

### Comparing `grote-0.1.3/grote/collections/load.py` & `grote-0.1.4/grote/collections/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,23 +49,22 @@
 
     @classmethod
     def get_file_in(cls, value: str | list[str] | Callable | None = None, visible: bool = True) -> gr.File:
         return gr.File(
             label=LOAD_CFG["file_label"],
             interactive=True,
             elem_id="file_in",
-            height=200,
             file_count="single",
             file_types=["txt"],
             value=value,
             visible=visible,
         )
 
     @classmethod
-    def get_sentences_txt(cls, value: str | Callable = "", visible: bool = True) -> gr.components.Textbox:
+    def get_sentences_txt(cls, value: str | Callable = "", visible: bool = False) -> gr.components.Textbox:
         return gr.Textbox(
             label=LOAD_CFG["sentences_label"],
             lines=6,
             elem_id="sentences_txt",
             placeholder=LOAD_CFG["sentences_placeholder"],
             value=value,
             visible=visible,
@@ -78,17 +77,16 @@
     @classmethod
     @buildmethod
     def build(cls: LoadComponents) -> LoadComponents:
         lc: LoadComponents = cls()
         lc.login_code_description_cap = lc.get_login_code_description_cap()
         lc.login_code_txt = lc.get_login_code_txt()
         lc.input_description_cap = lc.get_input_description_cap()
-        with gr.Row(equal_height=True):
-            lc.file_in = lc.get_file_in()
-            lc.sentences_txt = lc.get_sentences_txt()
+        lc.file_in = lc.get_file_in()
+        lc.sentences_txt = lc.get_sentences_txt()
         lc.start_btn = lc.get_start_btn()
         return lc
 
     def set_listeners(self, tc: TranslateComponents, out_state: gr.State) -> None:
         self.start_btn.click(
             check_and_parse_inputs_fn,
             inputs=[
```

### Comparing `grote-0.1.3/grote/collections/translate.py` & `grote-0.1.4/grote/collections/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 from grote.event_logging import EventLogger
 from grote.functions import (
     record_textbox_blur_fn,
     record_textbox_focus_fn,
     record_textbox_input_fn,
     record_textbox_remove_highlights_fn,
     record_trial_end_fn,
+    save_outputs_to_file,
 )
 
 TRANS_CFG = COMPONENT_CONFIGS["translate"]
 
 
 @dataclass
 class TranslateComponents(ComponentCollection):
     _id: str = "translate"
 
     source_side_label: gr.Markdown = None
     target_side_label: gr.Markdown = None
     target_side_legend: gr.Markdown = None
     reload_btn: gr.Button = None
     done_btn: gr.Button = None
+    download_btn: gr.DownloadButton = None
     textboxes_col: gr.Column = None
 
     @property
     def textboxes(self) -> list[gr.Textbox | HighlightedTextbox]:
         return [c for c in self.components if isinstance(c, (gr.Textbox, HighlightedTextbox))]
 
     @property
@@ -53,29 +55,39 @@
         if not value:
             value = TRANS_CFG["target_side_label"]
         return gr.Markdown(value, visible=visible, elem_id="target_side_label_cap")
 
     @classmethod
     def get_target_side_legend_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
         if not value and TRANS_CFG["highlight_labels"] and TRANS_CFG["highlight_colors"]:
-            value = "<b>Legend:</b>" + "".join(
+            value = f"<b>{TRANS_CFG['legend_label']}:</b>" + "".join(
                 f'<span style="background-color:{color}; margin-left: 0.5em; color: black; padding: 0px 5px;">{label}</span>'
                 for label, color in zip(TRANS_CFG["highlight_labels"], TRANS_CFG["highlight_colors"])
             )
         return gr.Markdown(value, visible=visible, elem_id="target_side_legend_cap")
 
     @classmethod
     def get_reload_btn(cls, visible: bool = False) -> gr.Button:
         return gr.Button(TRANS_CFG["reload_button_label"], variant="secondary", elem_id="reload_btn", visible=visible)
 
     @classmethod
     def get_done_btn(cls, visible: bool = False) -> gr.Button:
         return gr.Button(TRANS_CFG["done_button_label"], variant="primary", elem_id="done_btn", visible=visible)
 
     @classmethod
+    def get_download_btn(cls, visible: bool = False) -> gr.DownloadButton:
+        return gr.DownloadButton(
+            TRANS_CFG["download_button_label"],
+            variant="primary",
+            elem_id="download_btn",
+            visible=visible,
+            interactive=False,
+        )
+
+    @classmethod
     def get_textboxes_col(cls, visible: bool = False) -> gr.Column:
         return gr.Column(visible=visible, elem_id="textboxes_col")
 
     @classmethod
     def get_textbox_txt(
         cls,
         type: Literal["source", "target"],
@@ -136,14 +148,15 @@
             for idx, (src_sent, tgt_sent) in enumerate(zip(source_sentences, target_sentences)):
                 with gr.Row(equal_height=True, visible=False):
                     _ = tc.get_textbox_txt("source", idx, src_sent, lines=0)
                     _ = tc.get_textbox_txt("target", idx, tgt_sent, lines=0)
         with gr.Row(equal_height=True):
             tc.reload_btn = tc.get_reload_btn()
             tc.done_btn = tc.get_done_btn()
+        tc.download_btn = tc.get_download_btn()
         tc.textboxes_col = textboxes_col
         return tc
 
     def set_listeners(self, out_state: gr.State, lc_state: gr.State, logger: EventLogger) -> None:
         def save_logs_callback(state: dict[str, Any]) -> dict[str, Any]:
             if len(state["events"]) > cfg.event_logs_save_frequency:
                 logger.save(state["events"])
@@ -195,8 +208,12 @@
             record_trial_end_fn,
             inputs=[out_state, lc_state],
             outputs=[out_state],
         ).then(
             save_logs_callback_no_check,
             inputs=[out_state],
             outputs=[out_state],
-        ).then(None, js="window.location.reload()")
+        ).then(
+            save_outputs_to_file,
+            inputs=[lc_state] + self.target_textboxes,
+            outputs=[self.download_btn, self.done_btn],
+        )
```

### Comparing `grote-0.1.3/grote/config.py` & `grote-0.1.4/grote/config.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.3/grote/event_logging.py` & `grote-0.1.4/grote/event_logging.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.3/grote/functions/__init__.py` & `grote-0.1.4/grote/functions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from .translate import (
     record_textbox_blur_fn,
     record_textbox_focus_fn,
     record_textbox_input_fn,
     record_textbox_remove_highlights_fn,
     record_trial_end_fn,
     record_trial_start_fn,
+    save_outputs_to_file,
 )
 
 __all__ = [
     "check_and_parse_inputs_fn",
     "initialize_translate_interface_fn",
     "record_textbox_blur_fn",
     "record_textbox_focus_fn",
     "record_textbox_input_fn",
     "record_textbox_remove_highlights_fn",
     "record_trial_start_fn",
     "record_trial_end_fn",
+    "save_outputs_to_file",
 ]
```

### Comparing `grote-0.1.3/grote/functions/load.py` & `grote-0.1.4/grote/functions/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from pathlib import Path
 from typing import Any
 
 import gradio as gr
 
 from grote.config import CONFIG as cfg
 
 
@@ -39,15 +40,17 @@
         raise gr.Error("ERROR: No sentences were provided.")
     elif file_in and sentences_txt:
         raise gr.Error("ERROR: You can either upload a file or insert sentences manually, not both.")
 
     if file_in is not None:
         with open(file_in.name) as f:
             sentences_txt = f.read()
-    sentences_txt = sentences_txt.split("\n")
+            # remove empty lines
+            sentences_txt = re.sub(r"\n+", "\n", sentences_txt)
+    sentences_txt = sentences_txt.strip().split("\n")
 
     if not all(" ||| " in s for s in sentences_txt):
         raise gr.Error("ERROR: Sentences must match the format SOURCE ||| TARGET")
 
     source_sentences = [sent.split(" ||| ")[0] for sent in sentences_txt]
     target_sentences = [sent.split(" ||| ")[1] for sent in sentences_txt]
     # Check wellformedness of source and target sentences (highlights allowed in target sentences only)
@@ -67,14 +70,15 @@
                 ):
                     raise gr.Error(
                         f"ERROR: Target sentence {tgt_sent_idx} contains an invalid highlight ({curr_match_idx},"
                         f" {match[0]})."
                     )
     state["login_code_txt"] = login_code_txt
     state["file_in"] = None
+    state["_filename"] = Path(file_in.name).stem if file_in is not None else "grote_sentences.txt"
     state["sentences_txt"] = sentences_txt
     return state
 
 
 def initialize_translate_interface_fn(lc_state: dict[str, Any], tc_state: dict[str, Any]):
     """Initializes the translation tab."""
     from grote.collections import LoadComponents, TranslateComponents
```

### Comparing `grote-0.1.3/grote/functions/translate.py` & `grote-0.1.4/grote/functions/translate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from datetime import datetime
 from typing import Any
 
+import gradio as gr
+
 from grote.collections.base import COMPONENT_CONFIGS
 
 TRANS_CFG = COMPONENT_CONFIGS["translate"]
 
 
 def get_current_time() -> str:
     return datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
@@ -74,14 +76,28 @@
     }
     state[textbox_content["id"]] = current_text
     state["events"].append(out)
     return state
 
 
 def record_trial_end_fn(state: dict[str, Any], lc_state: dict[str, Any]) -> dict[str, Any]:
+    gr.Info("Saving trial information. Please wait...")
     out = {
         "time": get_current_time(),
         "login_code": lc_state["login_code_txt"],
         "event_type": "end",
     }
     state["events"].append(out)
     return state
+
+
+def save_outputs_to_file(lc_state, *txts) -> None:
+    fname = f"{lc_state['login_code_txt']}_{lc_state['_filename']}_output.txt"
+    with open(fname, "w") as f:
+        f.write("\n".join("".join(x[0] for x in txt["data"]) for txt in txts if txt["data"]))
+    gr.Info("Saving complete! Download the output file below")
+    return gr.DownloadButton(
+        label=TRANS_CFG["download_button_label"],
+        value=fname,
+        visible=True,
+        interactive=True,
+    ), gr.Button(interactive=False)
```

### Comparing `grote-0.1.3/pyproject.toml` & `grote-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "grote"
-version = "0.1.3"
+version = "0.1.4"
 description = "Groningen Translation Environment"
 readme = "README.md"
 authors = ["Gabriele Sarti"]
 maintainers = ["Gabriele Sarti <gabriele.sarti996@gmail.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/gsarti/grote"
 homepage = "https://github.com/gsarti/grote"
@@ -36,15 +36,15 @@
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "grote" = "grote.app:main"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 
-gradio = "^4.17.0"
+gradio = "^4.26.0"
 gradio_highlightedtextbox = "^0.0.11"
 toml = "^0.10.2"
 
 ipykernel = { version = "^6.19.2", optional = true }
 ipywidgets = { version = "^8.0.0rc2", optional = true }
 jupyterlab = { version = "^4.0.7", optional = true }
```

### Comparing `grote-0.1.3/PKG-INFO` & `grote-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grote
-Version: 0.1.3
+Version: 0.1.4
 Summary: Groningen Translation Environment
 Home-page: https://github.com/gsarti/grote
 License: Apache Software License 2.0
 Keywords: translation environment,gradio
 Author: Gabriele Sarti
 Maintainer: Gabriele Sarti
 Maintainer-email: gabriele.sarti996@gmail.com
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: notebook
-Requires-Dist: gradio (>=4.17.0,<5.0.0)
+Requires-Dist: gradio (>=4.26.0,<5.0.0)
 Requires-Dist: gradio_highlightedtextbox (>=0.0.11,<0.0.12)
 Requires-Dist: ipykernel (>=6.19.2,<7.0.0) ; extra == "notebook"
 Requires-Dist: ipywidgets (>=8.0.0rc2,<9.0.0) ; extra == "notebook"
 Requires-Dist: jupyterlab (>=4.0.7,<5.0.0) ; extra == "notebook"
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/gsarti/grote
 Description-Content-Type: text/markdown
```

