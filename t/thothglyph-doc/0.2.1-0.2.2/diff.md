# Comparing `tmp/thothglyph_doc-0.2.1.tar.gz` & `tmp/thothglyph_doc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thothglyph_doc-0.2.1.tar", max compression
+gzip compressed data, was "thothglyph_doc-0.2.2.tar", max compression
```

## Comparing `thothglyph_doc-0.2.1.tar` & `thothglyph_doc-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.1/LICENSE
--rw-r--r--   0        0        0      813 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/README.md
--rw-r--r--   0        0        0      697 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/thothglyph/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/app/__init__.py
--rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/app/converter.py
--rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph.svg
--rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph_256.png
--rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph_64.png
--rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/error.py
--rw-r--r--   0        0        0     3064 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/blockdiag.py
--rw-r--r--   0        0        0     1164 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/graphviz.py
--rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/math.py
--rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/mermaid.py
--rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/plantuml.py
--rw-r--r--   0        0        0     1277 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/wavedrom.py
--rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/node/logging.py
--rw-r--r--   0        0        0    17076 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/node/nd.py
--rw-r--r--   0        0        0      311 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/__init__.py
--rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/md.py
--rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/reader.py
--rw-r--r--   0        0        0    45290 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/reader/tglyph.py
--rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.pdf
--rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.svg
--rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_en.pdf
--rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_en.svg
--rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_im.pdf
--rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_im.svg
--rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/docx/default/style.docx
--rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/template/html/default/index.html
--rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/template/html/preview/index.html
--rw-r--r--   0        0        0     6793 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/latex/default/document-ja.tex
--rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/__init__.py
--rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/docx.py
--rw-r--r--   0        0        0    16304 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/html.py
--rw-r--r--   0        0        0    18211 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/latex.py
--rw-r--r--   0        0        0     4530 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/pdf.py
--rw-r--r--   0        0        0     5363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/writer.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.2/LICENSE
+-rw-r--r--   0        0        0      813 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.2/README.md
+-rw-r--r--   0        0        0      697 2024-04-08 23:53:27.001795 thothglyph_doc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/app/__init__.py
+-rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/app/converter.py
+-rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph.svg
+-rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph_256.png
+-rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph_64.png
+-rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/error.py
+-rw-r--r--   0        0        0     3064 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/blockdiag.py
+-rw-r--r--   0        0        0     1164 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/graphviz.py
+-rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/math.py
+-rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/mermaid.py
+-rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/plantuml.py
+-rw-r--r--   0        0        0     1277 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/wavedrom.py
+-rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/node/logging.py
+-rw-r--r--   0        0        0    17162 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/node/nd.py
+-rw-r--r--   0        0        0      485 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/reader/__init__.py
+-rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/reader/md.py
+-rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/reader/reader.py
+-rw-r--r--   0        0        0    47815 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/reader/tglyph.py
+-rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.pdf
+-rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.svg
+-rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_en.pdf
+-rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_en.svg
+-rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_im.pdf
+-rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_im.svg
+-rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/docx/default/style.docx
+-rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.2/thothglyph/template/html/default/index.html
+-rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.2/thothglyph/template/html/preview/index.html
+-rw-r--r--   0        0        0     6793 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/latex/default/document-ja.tex
+-rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/__init__.py
+-rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/docx.py
+-rw-r--r--   0        0        0    16577 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/html.py
+-rw-r--r--   0        0        0    18375 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/latex.py
+-rw-r--r--   0        0        0     4530 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/pdf.py
+-rw-r--r--   0        0        0     5474 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/writer.py
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.2/PKG-INFO
```

### Comparing `thothglyph_doc-0.2.1/LICENSE` & `thothglyph_doc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/README.md` & `thothglyph_doc-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/pyproject.toml` & `thothglyph_doc-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thothglyph-doc"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Documentation converter and language for Engineers"
 authors = ["nakandev <nakandev.s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "thothglyph" },
 ]
```

### Comparing `thothglyph_doc-0.2.1/thothglyph/app/converter.py` & `thothglyph_doc-0.2.2/thothglyph/app/converter.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/data/tglyph.svg` & `thothglyph_doc-0.2.2/thothglyph/data/tglyph.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/data/tglyph_256.png` & `thothglyph_doc-0.2.2/thothglyph/data/tglyph_256.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/data/tglyph_64.png` & `thothglyph_doc-0.2.2/thothglyph/data/tglyph_64.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/ext/blockdiag.py` & `thothglyph_doc-0.2.2/thothglyph/ext/blockdiag.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/ext/graphviz.py` & `thothglyph_doc-0.2.2/thothglyph/ext/graphviz.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/ext/math.py` & `thothglyph_doc-0.2.2/thothglyph/ext/math.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/ext/wavedrom.py` & `thothglyph_doc-0.2.2/thothglyph/ext/wavedrom.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/node/logging.py` & `thothglyph_doc-0.2.2/thothglyph/node/logging.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/node/nd.py` & `thothglyph_doc-0.2.2/thothglyph/node/nd.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,19 @@
     attrkey = ('text',)
 
     def __init__(self, text: Optional[str] = None):
         super().__init__()
         self.text: str = str() if text is None else text
 
 
+class LinebreakNode(InlineNode):
+    def __init__(self):
+        super().__init__()
+
+
 class RoleNode(InlineNode):
     attrkey = ('role', 'args', 'opts', 'value')
 
     def __init__(self, role=None, args=None, opts=None, value=None):
         super().__init__()
         self.role: str = str() if role is None else role
         self.args: Any = list() if args is None else args
```

### Comparing `thothglyph_doc-0.2.1/thothglyph/reader/md.py` & `thothglyph_doc-0.2.2/thothglyph/reader/md.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/reader/reader.py` & `thothglyph_doc-0.2.2/thothglyph/reader/reader.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/reader/tglyph.py` & `thothglyph_doc-0.2.2/thothglyph/reader/tglyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,27 @@
         'TOC_LINE': r' *¤toc(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'FIGURE_LINE': r' *¤figure(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'TABLE_LINE': r'^ *\|.+\| *$',
         'LISTTABLE_BEGIN_LINE': r'^ *\|=== *(?:⟦([^⟧]*)⟧)? *$',
         'LISTTABLE_END_LINE': r'^ *===\| *$',
         'FOOTNOTE_LIST_SYMBOL': r' *•\[\^(.+)\](?: +|$)',
         'REFERENCE_LIST_SYMBOL': r' *•\[\#(.+)\](?: +|$)',
+        # 'SCOPE_BEGIN_SYMBOL': r' *([•꓾]?)⦃',
+        'SCOPE_BEGIN_SYMBOL': r' *⦃',
+        'SCOPE_END_SYMBOL': r'⦄',
         'CHECK_LIST_SYMBOL': r' *(•+)(\[[ x-]\])(?: +|$)',
         'BULLET_LIST_SYMBOL': r' *(•+)(?: +|$)',
         'ORDERED_LIST_SYMBOL': r' *(꓾+)(?: +|$)',
         'DESC_LIST_SYMBOL': r' *(ᛝ+)([^ᛝ]+)ᛝ(?: +|$)',
         'LIST_TERMINATOR_SYMBOL': r' *(◃+) *$',
         'CUSTOM_LINE': r'( *)¤¤¤(.*)',
         'CODE_LINE': r'( *)⸌⸌⸌(.*)',
         'QUOTE_SYMBOL': r'^ *> ',
         'HR_LINE': r'^ *(?:(={4,})|(-{4,}))$',
-        'BREAK_LINE': r' *↲',
+        'BREAK_PARAGRAPH': r' *⊹',
         'STR_LINE': r'.+',
         'EMPTY_LINE': r'^$',
     }
     listblock_keys: Tuple[str, ...] = (
         'BULLET_LIST_SYMBOL',
         'ORDERED_LIST_SYMBOL',
         'DESC_LIST_SYMBOL',
@@ -83,14 +86,15 @@
     inline_tokens: Dict[str, str] = {
         'ATTR': r'⁅([A-Za-z0-9_\-]+)⁆',
         'ROLE': r'¤([A-Za-z]+)(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩',
         'LINK': r'(?:⟦([^⟧]*)⟧)?⸨([^⸩]+)⸩',
         'FOOTNOTE': r'\[\^([\w\-.]+)\]',
         'REFERENCE': r'\[\#([\w\-.]+)\]',
         'BRACKET': r'\[[^\]]+\]',
+        'LINEBREAK': r'↲',
     } | inline_deco_tokens
 
     def __init__(self):
         self._preproc_tokens: Dict[str, re.Pattern] = {
             k: re.compile(v) for k, v in self.preproc_tokens.items()
         }
         self._block_tokens: Dict[str, re.Pattern] = {
@@ -345,15 +349,15 @@
             msg = 'Nothing document or sections.'
             msg = f'{self.reader.path}: {msg}'
             raise ThothglyphError(msg)
         return self.nodes[idx]
 
     def p_blocks(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         while tokens:
-            if tokens[0].key == 'BREAK_LINE':
+            if tokens[0].key == 'BREAK_PARAGRAPH':
                 tokens.pop(0)
             elif tokens[0].key == 'BLOCKS_TERMINATOR':
                 tokens.pop(0)
                 break
             elif tokens[0].key == 'SECTION_TERMINATOR':
                 tokens.pop(0)
                 break
@@ -361,14 +365,16 @@
                 tokens = self.p_block(tokens)
             tokens = self.p_ignore_emptylines(tokens)
         return tokens
 
     def p_block(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         if tokens[0].key == 'SECTION_TITLE_LINE':
             tokens = self.p_section(tokens)
+        elif tokens[0].key == 'SCOPE_BEGIN_SYMBOL':
+            tokens = self.p_scoped_blocks(tokens)
         elif tokens[0].key == 'TOC_LINE':
             tokens = self.p_tocblock(tokens)
         elif tokens[0].key == 'FIGURE_LINE':
             tokens = self.p_figureblock(tokens)
         elif tokens[0].key == 'TABLE_LINE':
             tokens = self.p_basictableblock(tokens)
         elif tokens[0].key == 'LISTTABLE_BEGIN_LINE':
@@ -500,14 +506,63 @@
         text = self.replace_text_attrs(text)
         texttokens = self.lexer.lex_inline(text)
         self.nodes.append(item)
         self.p_inlinemarkup(texttokens)
         self.nodes.pop()
         return tokens
 
+    def p_scoped_blocks(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
+        begintoken = tokens[0]
+        tokens.pop(0)
+        nested = 1
+        subtokens = list()
+        while tokens:
+            if tokens[0].key == 'SCOPE_BEGIN_SYMBOL':
+                nested += 1
+            if tokens[0].key == 'SCOPE_END_SYMBOL':
+                nested -= 1
+                if nested == 0:
+                    break
+            subtokens.append(tokens.pop(0))
+        else:
+            lineno = begintoken.line + 1
+            msg = 'Scoped block is not closed.'
+            msg = f'{self.reader.path}:{lineno}: {msg}'
+            raise ThothglyphError(msg)
+        tokens.pop(0)
+
+        dummylistblock = nd.ListBlockNode()
+        self.nodes.append(dummylistblock)
+        while subtokens:
+            if subtokens[0].key == 'BREAK_PARAGRAPH':
+                subtokens.pop(0)
+            elif subtokens[0].key == 'BLOCKS_TERMINATOR':
+                subtokens.pop(0)
+                break
+            elif subtokens[0].key == 'SECTION_TERMINATOR':
+                subtokens.pop(0)
+                break
+            else:
+                subtokens = self.p_block(subtokens)
+            subtokens = self.p_ignore_emptylines(subtokens)
+        self.nodes.pop()
+
+        lastnode = self.nodes[-1]
+        if isinstance(lastnode, nd.ListBlockNode):
+            item = nd.ListItemNode()
+            item.level = len(self.nodes) - self.nodes[-2].parent.level - 1
+            item.indent = 0
+            for child in dummylistblock.children:
+                item.add(child)
+            lastnode.add(item)
+        else:
+            for child in dummylistblock.children:
+                self.nodes[-1].add(child)
+        return tokens
+
     def _get_listblock_by_token(self, token: Lexer.Token) -> List[nd.ListBlockNode]:
         table = {
             'BULLET_LIST_SYMBOL': nd.BulletListBlockNode,
             'ORDERED_LIST_SYMBOL': nd.OrderedListBlockNode,
             'DESC_LIST_SYMBOL': nd.DescriptionListBlockNode,
             'CHECK_LIST_SYMBOL': nd.CheckListBlockNode,
         }
@@ -946,14 +1001,16 @@
                 tokens = self.p_link(tokens)
             elif tokens[0].key == 'FOOTNOTE':
                 tokens = self.p_footnote(tokens)
             elif tokens[0].key == 'REFERENCE':
                 tokens = self.p_reference(tokens)
             elif tokens[0].key in Lexer.deco_keys:
                 tokens = self.p_deco(tokens)
+            elif tokens[0].key in 'LINEBREAK':
+                tokens = self.p_linebreak(tokens)
             else:
                 tokens = self.p_text(tokens)
         return tokens
 
     def p_role(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         m = re.match(Lexer.inline_tokens['ROLE'], tokens[0].value)
         assert m
@@ -1132,20 +1189,23 @@
 
         newtext = re.sub(
             Lexer.inline_tokens['ATTR'], attrvalue, text,
             flags=re.MULTILINE | re.DOTALL
         )
         return newtext
 
+    def p_linebreak(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
+        lb = nd.LinebreakNode()
+        self.nodes[-1].add(lb)
+        tokens.pop(0)
+        return tokens
+
     def p_text(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
-        if len(self.nodes[-1].children) == 0:
-            text = nd.TextNode()
-            self.nodes[-1].add(text)
-            text.text += tokens[0].value
-        elif not isinstance(self.nodes[-1].children[-1], nd.TextNode):
+        last_children = self.nodes[-1].children
+        if len(last_children) == 0 or not isinstance(last_children, nd.TextNode):
             text = nd.TextNode()
             self.nodes[-1].add(text)
             text.text += tokens[0].value
         else:
             text = self.nodes[-1].children[-1]
             text.text += '' + tokens[0].value
         tokens.pop(0)
@@ -1164,11 +1224,18 @@
     def __init__(self, parent: Optional[Reader] = None):
         super().__init__(parent=parent)
         self.parser: TglyphParser = TglyphParser(self)
 
     def read(self, path: str, encoding: Optional[str] = None) -> nd.ASTNode:
         try:
             return super().read(path, encoding)
-        except Exception as e:
-            _, errormsg = e.args
-            msg = 'File cannot found: {}'.format(e.filename)
+        except ThothglyphError as e:
+            msg = e.args[-1]
+            raise ThothglyphError(msg)
+        except OSError as e:
+            msg = '{}: {}'.format(e.strerror, e.filename)
+            raise ThothglyphError(msg)
+        except Exception:
+            exc_type, exc_msg, exc_tb = sys.exc_info()
+            tbinfo = 'file {}, line {}'.format(exc_tb.tb_frame.f_code.co_filename, exc_tb.tb_lineno)
+            msg = '{} ({})'.format(exc_msg, tbinfo)
             raise ThothglyphError(msg)
```

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.pdf` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.svg` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_en.pdf` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_en.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_en.svg` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_en.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_im.pdf` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_im.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/common/check_im.svg` & `thothglyph_doc-0.2.2/thothglyph/template/common/check_im.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/docx/default/style.docx` & `thothglyph_doc-0.2.2/thothglyph/template/docx/default/style.docx`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/html/default/index.html` & `thothglyph_doc-0.2.2/thothglyph/template/html/default/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/html/preview/index.html` & `thothglyph_doc-0.2.2/thothglyph/template/html/preview/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/template/latex/default/document-ja.tex` & `thothglyph_doc-0.2.2/thothglyph/template/latex/default/document-ja.tex`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/writer/docx.py` & `thothglyph_doc-0.2.2/thothglyph/writer/docx.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/writer/html.py` & `thothglyph_doc-0.2.2/thothglyph/writer/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                 f.write(self.data)
             os.makedirs(fdir, exist_ok=True)
             shutil.copytree(self.tmpdirname, fdir, dirs_exist_ok=True)
         self.tmpdirname = None
 
     def _copy_template(self, fpath: str) -> None:
         commondir = os.path.join(self.template_dir(), 'common')
+        if not os.path.exists(commondir):
+            commondir = os.path.join(self.pkg_template_dir(), 'common')
         newcommondir = os.path.join(self.tmpdirname, 'template', 'common')
         shutil.copytree(commondir, newcommondir, dirs_exist_ok=True)
 
     def _copy_resources(self, fpath: str) -> None:
         rscs: Dict[str, List[str]] = dict()
         typetable: Dict[str, Dict[str, str]] = {
             'img': {
@@ -430,14 +432,20 @@
         url = '#ref.{}'.format(node.ref_num)
         text = node.ref_num  # node.value
         self.data += '[<a href="{}">{}</a>]'.format(url, text)
 
     def leave_reference(self, node: nd.ASTNode) -> None:
         pass
 
+    def visit_linebreak(self, node: nd.ASTNode) -> None:
+        self.data += '<br />'
+
+    def leave_linebreak(self, node: nd.ASTNode) -> None:
+        pass
+
     def visit_text(self, node: nd.ASTNode) -> None:
         self.data += node.text
 
     def leave_text(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_other(self, node: nd.ASTNode) -> None:
```

### Comparing `thothglyph_doc-0.2.1/thothglyph/writer/latex.py` & `thothglyph_doc-0.2.2/thothglyph/writer/latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,20 @@
     def visit_reference(self, node: nd.ASTNode) -> None:
         url = 'ref.{}'.format(node.ref_num)
         self.data += '\\cite{{{}}}'.format(url)
 
     def leave_reference(self, node: nd.ASTNode) -> None:
         pass
 
+    def visit_linebreak(self, node: nd.ASTNode) -> None:
+        self.data += '{\\newline}'
+
+    def leave_linebreak(self, node: nd.ASTNode) -> None:
+        pass
+
     def visit_text(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent_block, nd.CodeBlockNode):
             text = node.text
             for key, delim in self.code_decoration_table.items():
                 text = text.replace(key, delim)
             self.data += text
         else:
```

### Comparing `thothglyph_doc-0.2.1/thothglyph/writer/pdf.py` & `thothglyph_doc-0.2.2/thothglyph/writer/pdf.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.1/thothglyph/writer/writer.py` & `thothglyph_doc-0.2.2/thothglyph/writer/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,22 +32,26 @@
 
     def __init__(self):
         self.encoding: str = 'utf-8'
         self.data: str = str()
         self.rootnode: Optional[nd.DocumentNode] = None
         self.__continue: bool = False
 
+    def pkg_template_dir(self) -> str:
+        libdir = os.path.join(os.path.dirname(__file__), '..')
+        template_dir = os.path.join(libdir, 'template')
+        return template_dir
+
     def template_dir(self) -> str:
         assert isinstance(self.rootnode, nd.DocumentNode)
         config = self.rootnode.config
         if hasattr(config, 'templatedir'):
             template_dir = config.templatedir
         else:
-            libdir = os.path.join(os.path.dirname(__file__), '..')
-            template_dir = os.path.join(libdir, 'template')
+            template_dir = self.pkg_template_dir()
         return template_dir
 
     def theme(self, target: Optional[str] = None) -> str:
         assert isinstance(self.rootnode, nd.DocumentNode)
         config = self.rootnode.config
         if hasattr(config, 'theme'):
             theme = config.theme
```

### Comparing `thothglyph_doc-0.2.1/PKG-INFO` & `thothglyph_doc-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothglyph-doc
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Documentation converter and language for Engineers
 License: MIT
 Author: nakandev
 Author-email: nakandev.s@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

