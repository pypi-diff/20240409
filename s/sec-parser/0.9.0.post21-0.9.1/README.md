# Comparing `tmp/sec_parser-0.9.0.post21.tar.gz` & `tmp/sec_parser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sec_parser-0.9.0.post21.tar", max compression
+gzip compressed data, was "sec_parser-0.9.1.tar", max compression
```

## Comparing `sec_parser-0.9.0.post21.tar` & `sec_parser-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1069 2023-09-27 06:50:50.194832 sec_parser-0.9.0.post21/LICENSE
--rw-r--r--   0        0        0     4851 2023-09-27 06:50:50.194832 sec_parser-0.9.0.post21/README.md
--rw-r--r--   0        0        0     3409 2023-09-27 06:51:21.543385 sec_parser-0.9.0.post21/pyproject.toml
--rw-r--r--   0        0        0     1819 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/__init__.py
--rw-r--r--   0        0        0     1045 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/data_sources/__init__.py
--rw-r--r--   0        0        0     2567 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/data_sources/abstract_sec_data_retriever.py
--rw-r--r--   0        0        0     3153 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/data_sources/sec_edgar_enums.py
--rw-r--r--   0        0        0      838 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/data_sources/sec_edgar_utils.py
--rw-r--r--   0        0        0     6726 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/data_sources/secapio_data_retriever.py
--rw-r--r--   0        0        0      316 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/exceptions/__init__.py
--rw-r--r--   0        0        0      298 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/exceptions/core_exceptions.py
--rw-r--r--   0        0        0      671 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/__init__.py
--rw-r--r--   0        0        0      501 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/abstract_parser.py
--rw-r--r--   0        0        0        0 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/__init__.py
--rw-r--r--   0        0        0      335 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/abstract_html_tag_parser.py
--rw-r--r--   0        0        0     6358 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/html_tag.py
--rw-r--r--   0        0        0      926 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/root_tag_parser.py
--rw-r--r--   0        0        0     2577 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_engine/sec_parser.py
--rw-r--r--   0        0        0      963 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/__init__.py
--rw-r--r--   0        0        0     3252 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/abstract_elementwise_plugin.py
--rw-r--r--   0        0        0     2273 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/abstract_parsing_plugin.py
--rw-r--r--   0        0        0     2773 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/footnote_and_bulletpoint_plugin.py
--rw-r--r--   0        0        0     1518 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/highlighted_text_plugin.py
--rw-r--r--   0        0        0     1120 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/image_plugin.py
--rw-r--r--   0        0        0     2182 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/root_section_plugin.py
--rw-r--r--   0        0        0     1122 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/table_plugin.py
--rw-r--r--   0        0        0     1820 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/text_plugin.py
--rw-r--r--   0        0        0     2384 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/parsing_plugins/title_plugin.py
--rw-r--r--   0        0        0     1103 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/sec_parsing_entry.py
--rw-r--r--   0        0        0     1022 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_elements/__init__.py
--rw-r--r--   0        0        0     4465 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_elements/abstract_semantic_element.py
--rw-r--r--   0        0        0     2474 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_elements/highlighted_text_element.py
--rw-r--r--   0        0        0     2831 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_elements/semantic_elements.py
--rw-r--r--   0        0        0      762 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/__init__.py
--rw-r--r--   0        0        0      346 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/abstract_nesting_rule.py
--rw-r--r--   0        0        0     3711 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/nesting_rules.py
--rw-r--r--   0        0        0     2679 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/semantic_tree.py
--rw-r--r--   0        0        0     3383 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/tree_builder.py
--rw-r--r--   0        0        0     1954 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/semantic_tree/tree_node.py
--rw-r--r--   0        0        0      340 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/bs4_/__init__.py
--rw-r--r--   0        0        0      526 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/bs4_/contains_tag.py
--rw-r--r--   0        0        0     1046 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/bs4_/get_first_deepest_tag.py
--rw-r--r--   0        0        0     1026 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/bs4_/is_unary_tree.py
--rw-r--r--   0        0        0     2665 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/bs4_/text_styles_metrics.py
--rw-r--r--   0        0        0      575 2023-09-27 06:50:50.218832 sec_parser-0.9.0.post21/sec_parser/utils/env_var_helpers.py
--rw-r--r--   0        0        0     6489 1970-01-01 00:00:00.000000 sec_parser-0.9.0.post21/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-10-06 23:37:48.302062 sec_parser-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4851 2023-10-06 23:37:48.302062 sec_parser-0.9.1/README.md
+-rw-r--r--   0        0        0     3402 2023-10-06 23:37:48.322062 sec_parser-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1740 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/__init__.py
+-rw-r--r--   0        0        0     1045 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/data_sources/__init__.py
+-rw-r--r--   0        0        0     2567 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/data_sources/abstract_sec_data_retriever.py
+-rw-r--r--   0        0        0     3153 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/data_sources/sec_edgar_enums.py
+-rw-r--r--   0        0        0      813 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/data_sources/sec_edgar_utils.py
+-rw-r--r--   0        0        0     6726 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/data_sources/secapio_data_retriever.py
+-rw-r--r--   0        0        0      316 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/exceptions/__init__.py
+-rw-r--r--   0        0        0      297 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/exceptions/core_exceptions.py
+-rw-r--r--   0        0        0      730 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/__init__.py
+-rw-r--r--   0        0        0      501 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/abstract_parser.py
+-rw-r--r--   0        0        0        0 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/__init__.py
+-rw-r--r--   0        0        0      335 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/abstract_html_tag_parser.py
+-rw-r--r--   0        0        0     6358 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/html_tag.py
+-rw-r--r--   0        0        0      926 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/root_tag_parser.py
+-rw-r--r--   0        0        0     2577 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_engine/sec_parser.py
+-rw-r--r--   0        0        0      963 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/__init__.py
+-rw-r--r--   0        0        0     3252 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/abstract_elementwise_plugin.py
+-rw-r--r--   0        0        0     2273 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/abstract_parsing_plugin.py
+-rw-r--r--   0        0        0     2773 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/footnote_and_bulletpoint_plugin.py
+-rw-r--r--   0        0        0     1518 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/highlighted_text_plugin.py
+-rw-r--r--   0        0        0     1120 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/image_plugin.py
+-rw-r--r--   0        0        0     2182 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/root_section_plugin.py
+-rw-r--r--   0        0        0     1122 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/table_plugin.py
+-rw-r--r--   0        0        0     1820 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/text_plugin.py
+-rw-r--r--   0        0        0     2384 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/parsing_plugins/title_plugin.py
+-rw-r--r--   0        0        0     1103 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/sec_parsing_entry.py
+-rw-r--r--   0        0        0     1022 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/semantic_elements/__init__.py
+-rw-r--r--   0        0        0     4465 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/semantic_elements/abstract_semantic_element.py
+-rw-r--r--   0        0        0     2474 2023-10-06 23:37:48.322062 sec_parser-0.9.1/sec_parser/semantic_elements/highlighted_text_element.py
+-rw-r--r--   0        0        0     2831 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_elements/semantic_elements.py
+-rw-r--r--   0        0        0      762 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/__init__.py
+-rw-r--r--   0        0        0      346 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/abstract_nesting_rule.py
+-rw-r--r--   0        0        0     3711 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/nesting_rules.py
+-rw-r--r--   0        0        0     2679 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/semantic_tree.py
+-rw-r--r--   0        0        0     3383 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/tree_builder.py
+-rw-r--r--   0        0        0     1954 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/semantic_tree/tree_node.py
+-rw-r--r--   0        0        0      340 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/bs4_/__init__.py
+-rw-r--r--   0        0        0      526 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/bs4_/contains_tag.py
+-rw-r--r--   0        0        0     1046 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/bs4_/get_first_deepest_tag.py
+-rw-r--r--   0        0        0     1026 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/bs4_/is_unary_tree.py
+-rw-r--r--   0        0        0     2665 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/bs4_/text_styles_metrics.py
+-rw-r--r--   0        0        0      575 2023-10-06 23:37:48.326062 sec_parser-0.9.1/sec_parser/utils/env_var_helpers.py
+-rw-r--r--   0        0        0     6482 1970-01-01 00:00:00.000000 sec_parser-0.9.1/PKG-INFO
```

### Comparing `sec_parser-0.9.0.post21/LICENSE` & `sec_parser-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/README.md` & `sec_parser-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/pyproject.toml` & `sec_parser-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sec-parser"
-version = "0.9.0.post21"
+version = "0.9.1"
 description = "Parse SEC EDGAR HTML documents into a tree of elements that correspond to the visual structure of the document."
 authors = ["Alphanome.AI <info@alphanome.ai>"]
 readme = "README.md"
 repository = "https://github.com/alphanome-ai/sec-parser"
 license = "MIT"
 classifiers = [
     "Topic :: Text Processing :: Markup :: HTML",
```

### Comparing `sec_parser-0.9.0.post21/sec_parser/__init__.py` & `sec_parser-0.9.1/sec_parser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,23 +35,20 @@
     "TreeBuilder",
     # Common semantic elements
     "AbstractSemanticElement",
     "UndeterminedElement",
     "RootSectionElement",
     "TextElement",
     "TitleElement",
-    "InvalidTitleLevelError",
     "IrrelevantElement",
     "ImageElement",
     "TableElement",
     "RootSectionSeparatorElement",
-    "HighlightedElement",
     "EmptyElement",
     "BulletpointTextElement",
-    "FootnoteElement",
     # Common exceptions
     "SecParserError",
     "SecParserRuntimeError",
     "SecParserValueError",
     # Common types
     "AbstractNestingRule",
     "DocumentType",
```

### Comparing `sec_parser-0.9.0.post21/sec_parser/data_sources/__init__.py` & `sec_parser-0.9.1/sec_parser/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/data_sources/abstract_sec_data_retriever.py` & `sec_parser-0.9.1/sec_parser/data_sources/abstract_sec_data_retriever.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/data_sources/sec_edgar_enums.py` & `sec_parser-0.9.1/sec_parser/data_sources/sec_edgar_enums.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/data_sources/sec_edgar_utils.py` & `sec_parser-0.9.1/sec_parser/data_sources/sec_edgar_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
     InvalidDocumentTypeError,
     InvalidSectionTypeError,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
-    from sec_parser.data_sources.sec_edgar_enums import (
-        DocumentType,
-        SectionType,
-    )
+    from sec_parser.data_sources.sec_edgar_enums import DocumentType, SectionType
 
 
 def validate_sections(
     doc_type: DocumentType,
     sections: Iterable[SectionType] | None,
 ) -> None:
     if sections is None:
```

### Comparing `sec_parser-0.9.0.post21/sec_parser/data_sources/secapio_data_retriever.py` & `sec_parser-0.9.1/sec_parser/data_sources/secapio_data_retriever.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_engine/__init__.py` & `sec_parser-0.9.1/sec_parser/parsing_engine/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     AbstractSemanticElementParser,
 )
 from sec_parser.parsing_engine.html_parsers.html_tag import HtmlTag
 from sec_parser.parsing_engine.html_parsers.root_tag_parser import (
     AbstractHtmlTagParser,
     RootTagParser,
 )
+from sec_parser.parsing_engine.sec_parser import SecParser
 
 __all__ = [
     "AbstractHtmlTagParser",
     "RootTagParser",
     "AbstractSemanticElementParser",
     "SecParser",
     "HtmlTag",
```

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/html_tag.py` & `sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/html_tag.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_engine/html_parsers/root_tag_parser.py` & `sec_parser-0.9.1/sec_parser/parsing_engine/html_parsers/root_tag_parser.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_engine/sec_parser.py` & `sec_parser-0.9.1/sec_parser/parsing_engine/sec_parser.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/__init__.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/abstract_elementwise_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/abstract_elementwise_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/abstract_parsing_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/abstract_parsing_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/footnote_and_bulletpoint_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/footnote_and_bulletpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/highlighted_text_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/highlighted_text_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/image_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/image_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/root_section_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/root_section_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/table_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/table_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/text_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/parsing_plugins/title_plugin.py` & `sec_parser-0.9.1/sec_parser/parsing_plugins/title_plugin.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/sec_parsing_entry.py` & `sec_parser-0.9.1/sec_parser/sec_parsing_entry.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_elements/__init__.py` & `sec_parser-0.9.1/sec_parser/semantic_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_elements/abstract_semantic_element.py` & `sec_parser-0.9.1/sec_parser/semantic_elements/abstract_semantic_element.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_elements/highlighted_text_element.py` & `sec_parser-0.9.1/sec_parser/semantic_elements/highlighted_text_element.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_elements/semantic_elements.py` & `sec_parser-0.9.1/sec_parser/semantic_elements/semantic_elements.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_tree/__init__.py` & `sec_parser-0.9.1/sec_parser/semantic_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_tree/nesting_rules.py` & `sec_parser-0.9.1/sec_parser/semantic_tree/nesting_rules.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_tree/semantic_tree.py` & `sec_parser-0.9.1/sec_parser/semantic_tree/semantic_tree.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_tree/tree_builder.py` & `sec_parser-0.9.1/sec_parser/semantic_tree/tree_builder.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/semantic_tree/tree_node.py` & `sec_parser-0.9.1/sec_parser/semantic_tree/tree_node.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/utils/bs4_/contains_tag.py` & `sec_parser-0.9.1/sec_parser/utils/bs4_/contains_tag.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/utils/bs4_/get_first_deepest_tag.py` & `sec_parser-0.9.1/sec_parser/utils/bs4_/get_first_deepest_tag.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/utils/bs4_/is_unary_tree.py` & `sec_parser-0.9.1/sec_parser/utils/bs4_/is_unary_tree.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/utils/bs4_/text_styles_metrics.py` & `sec_parser-0.9.1/sec_parser/utils/bs4_/text_styles_metrics.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/sec_parser/utils/env_var_helpers.py` & `sec_parser-0.9.1/sec_parser/utils/env_var_helpers.py`

 * *Files identical despite different names*

### Comparing `sec_parser-0.9.0.post21/PKG-INFO` & `sec_parser-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-parser
-Version: 0.9.0.post21
+Version: 0.9.1
 Summary: Parse SEC EDGAR HTML documents into a tree of elements that correspond to the visual structure of the document.
 Home-page: https://github.com/alphanome-ai/sec-parser
 License: MIT
 Author: Alphanome.AI
 Author-email: info@alphanome.ai
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: sec-parser Version: 0.9.0.post21 Summary: Parse SEC
-EDGAR HTML documents into a tree of elements that correspond to the visual
-structure of the document. Home-page: https://github.com/alphanome-ai/sec-
-parser License: MIT Author: Alphanome.AI Author-email: info@alphanome.ai
-Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*,
-!=3.5.*, !=3.6.*, !=3.7.*, !=3.8.* Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Financial and Insurance Industry Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
-Language :: English Classifier: Operating System :: OS Independent Classifier:
+Metadata-Version: 2.1 Name: sec-parser Version: 0.9.1 Summary: Parse SEC EDGAR
+HTML documents into a tree of elements that correspond to the visual structure
+of the document. Home-page: https://github.com/alphanome-ai/sec-parser License:
+MIT Author: Alphanome.AI Author-email: info@alphanome.ai Requires-Python:
+>=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*,
+!=3.7.*, !=3.8.* Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Financial and
+Insurance Industry Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Office/Business ::
 Financial Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Information
 Analysis Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Text Processing :: Markup :: HTML Requires-Dist:
```

