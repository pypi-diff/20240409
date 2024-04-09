# Comparing `tmp/python_docs_theme-2024.3.tar.gz` & `tmp/python_docs_theme-2024.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_docs_theme-2024.3.tar", last modified: Fri Mar 22 11:27:23 2024, max compression
+gzip compressed data, was "python_docs_theme-2024.4.tar", last modified: Tue Apr  9 09:19:50 2024, max compression
```

## Comparing `python_docs_theme-2024.3.tar` & `python_docs_theme-2024.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2460 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/LICENSE
--rw-r--r--   0        0        0      991 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/README.rst
--rw-r--r--   0        0        0     1560 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/pyproject.toml
--rw-r--r--   0        0        0     1814 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/__init__.py
--rw-r--r--   0        0        0      184 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/footerdonate.html
--rw-r--r--   0        0        0     7775 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/layout.html
--rw-r--r--   0        0        0     3508 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/copybutton.js
--rw-r--r--   0        0        0     2137 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/menu.js
--rw-r--r--   0        0        0      695 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/py.png
--rw-r--r--   0        0        0     2041 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/py.svg
--rw-r--r--   0        0        0    12163 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/pydoctheme.css
--rw-r--r--   0        0        0     2214 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/pydoctheme_dark.css
--rw-r--r--   0        0        0      559 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/search-focus.js
--rw-r--r--   0        0        0     3350 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/sidebar.js_t
--rw-r--r--   0        0        0      779 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/static/themetoggle.js
--rw-r--r--   0        0        0     1040 2024-03-22 11:27:23.000000 python_docs_theme-2024.3/python_docs_theme/theme.conf
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 python_docs_theme-2024.3/PKG-INFO
+-rw-r--r--   0        0        0     2460 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/LICENSE
+-rw-r--r--   0        0        0     1066 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/README.md
+-rw-r--r--   0        0        0     1559 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/pyproject.toml
+-rw-r--r--   0        0        0     1814 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/footerdonate.html
+-rw-r--r--   0        0        0     7891 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/layout.html
+-rw-r--r--   0        0        0     3508 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/copybutton.js
+-rw-r--r--   0        0        0     2137 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/menu.js
+-rw-r--r--   0        0        0      695 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/py.png
+-rw-r--r--   0        0        0     2041 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/py.svg
+-rw-r--r--   0        0        0    13101 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/pydoctheme.css
+-rw-r--r--   0        0        0     2371 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/pydoctheme_dark.css
+-rw-r--r--   0        0        0      559 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/search-focus.js
+-rw-r--r--   0        0        0     3350 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/sidebar.js_t
+-rw-r--r--   0        0        0      779 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/static/themetoggle.js
+-rw-r--r--   0        0        0     1040 2024-04-09 09:19:50.000000 python_docs_theme-2024.4/python_docs_theme/theme.conf
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 python_docs_theme-2024.4/PKG-INFO
```

### Comparing `python_docs_theme-2024.3/LICENSE` & `python_docs_theme-2024.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/pyproject.toml` & `python_docs_theme-2024.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 build-backend = "flit_core.buildapi"
 requires = [
   "flit_core>=3.7",
 ]
 
 [project]
 name = "python-docs-theme"
-version = "2024.3"
+version = "2024.4"
 description = "The Sphinx theme for the CPython docs and related projects"
-readme = "README.rst"
+readme = "README.md"
 license.file = "LICENSE"
 authors = [{name = "PyPA", email = "distutils-sig@python.org"}]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Sphinx :: Theme",
   "Intended Audience :: Developers",
```

### Comparing `python_docs_theme-2024.3/python_docs_theme/__init__.py` & `python_docs_theme-2024.4/python_docs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/layout.html` & `python_docs_theme-2024.4/python_docs_theme/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -132,27 +132,41 @@
     </div>
 </div>
 {% endif -%}
 {% endblock %}
 
 {% block footer %}
     <div class="footer">
-    &copy; {% if theme_copyright_url or hasdoc('copyright') %}<a href="{% if theme_copyright_url %}{{ theme_copyright_url }}{% else %}{{ pathto('copyright') }}{% endif %}">{% endif %}{% trans %}Copyright{% endtrans %}{% if theme_copyright_url or hasdoc('copyright') %}</a>{% endif %} {{ copyright|e }}.
+    &copy; {% if theme_copyright_url or hasdoc('copyright') %}
+      <a href="{% if theme_copyright_url %}{{ theme_copyright_url }}{% else %}{{ pathto('copyright') }}{% endif %}">
+    {% endif %}
+    {% trans %}Copyright{% endtrans %}
+    {% if theme_copyright_url or hasdoc('copyright') %}
+      </a>
+    {% endif %} {{ copyright|e }}.
     <br />
     {% trans %}This page is licensed under the Python Software Foundation License Version 2.{% endtrans %}
     <br />
     {% trans %}Examples, recipes, and other code in the documentation are additionally licensed under the Zero Clause BSD License.{% endtrans %}
     <br />
-    {% if theme_license_url %}{% trans license_file=theme_license_url %}See <a href="{{ license_file }}">History and License</a> for more information.{% endtrans %}<br />{% endif %}
-    {% if theme_hosted_on %}{% trans hosted_on=theme_hosted_on %}Hosted on {{ hosted_on }}.{% endtrans %}<br />{% endif %}
+    {% if theme_license_url %}
+      {% trans license_file=theme_license_url %}See <a href="{{ license_file }}">History and License</a> for more information.{% endtrans %}<br />
+    {% endif %}
+    {% if theme_hosted_on %}
+      {% trans hosted_on=theme_hosted_on %}Hosted on {{ hosted_on }}.{% endtrans %}<br />
+    {% endif %}
     <br />
 
     {% include "footerdonate.html" %}
     <br />
 
-    {% trans last_updated=last_updated|e %}Last updated on {{ last_updated }}.{% endtrans %}
-    {% if theme_issues_url %}{% trans %}<a href="{{ theme_issues_url }}">Found a bug</a>?{% endtrans %}{% endif %}
+    {%- if last_updated %}
+      {% trans last_updated=last_updated|e %}Last updated on {{ last_updated }}.{% endtrans %}
+    {%- endif %}
+    {% if theme_issues_url %}
+      {% trans %}<a href="{{ theme_issues_url }}">Found a bug</a>?{% endtrans %}
+    {% endif %}
     <br />
 
     {% trans sphinx_version=sphinx_version|e %}Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> {{ sphinx_version }}.{% endtrans %}
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -37,26 +37,26 @@
 [Unknown INPUT type][{{ _('Go') }}]
 {%- endif %}
 {{ themeselector() }} {%- if logo %}
 _[_L_o_g_o_]
 {%- endif %} {%- for sidebartemplate in sidebars %} {%- include sidebartemplate
 %} {%- endfor %}
 {% endif -%} {% endblock %} {% block footer %}
-© {% if theme_copyright_url or hasdoc('copyright') %}_{_%_ _e_n_d_i_f_ _%_}_{_%_ _t_r_a_n_s
-_%_}_C_o_p_y_r_i_g_h_t_{_%_ _e_n_d_t_r_a_n_s_ _%_}_{_%_ _i_f_ _t_h_e_m_e___c_o_p_y_r_i_g_h_t___u_r_l_ _o_r_ _h_a_s_d_o_c_(_'_c_o_p_y_r_i_g_h_t_'_)_ _%_}{%
-endif %} {{ copyright|e }}.
+© {% if theme_copyright_url or hasdoc('copyright') %} _{_%_ _e_n_d_i_f_ _%_}_ _{_%_ _t_r_a_n_s
+_%_}_C_o_p_y_r_i_g_h_t_{_%_ _e_n_d_t_r_a_n_s_ _%_}_ _{_%_ _i_f_ _t_h_e_m_e___c_o_p_y_r_i_g_h_t___u_r_l_ _o_r_ _h_a_s_d_o_c_(_'_c_o_p_y_r_i_g_h_t_'_)_ _%_}_ 
+{% endif %} {{ copyright|e }}.
 {% trans %}This page is licensed under the Python Software Foundation License
 Version 2.{% endtrans %}
 {% trans %}Examples, recipes, and other code in the documentation are
 additionally licensed under the Zero Clause BSD License.{% endtrans %}
-{% if theme_license_url %}{% trans license_file=theme_license_url %}See _H_i_s_t_o_r_y
-_a_n_d_ _L_i_c_e_n_s_e for more information.{% endtrans %}
-{% endif %} {% if theme_hosted_on %}{% trans hosted_on=theme_hosted_on %}Hosted
-on {{ hosted_on }}.{% endtrans %}
+{% if theme_license_url %} {% trans license_file=theme_license_url %}See
+_H_i_s_t_o_r_y_ _a_n_d_ _L_i_c_e_n_s_e for more information.{% endtrans %}
+{% endif %} {% if theme_hosted_on %} {% trans hosted_on=theme_hosted_on
+%}Hosted on {{ hosted_on }}.{% endtrans %}
 {% endif %}
 {% include "footerdonate.html" %}
-{% trans last_updated=last_updated|e %}Last updated on {{ last_updated }}.{%
-endtrans %} {% if theme_issues_url %}{% trans %}_F_o_u_n_d_ _a_ _b_u_g?{% endtrans %}{%
-endif %}
+{%- if last_updated %} {% trans last_updated=last_updated|e %}Last updated on {
+{ last_updated }}.{% endtrans %} {%- endif %} {% if theme_issues_url %} {%
+trans %}_F_o_u_n_d_ _a_ _b_u_g?{% endtrans %} {% endif %}
 {% trans sphinx_version=sphinx_version|e %}Created using _S_p_h_i_n_x {
 { sphinx_version }}.{% endtrans %}
 {% endblock %}
```

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/copybutton.js` & `python_docs_theme-2024.4/python_docs_theme/static/copybutton.js`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/menu.js` & `python_docs_theme-2024.4/python_docs_theme/static/menu.js`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/py.png` & `python_docs_theme-2024.4/python_docs_theme/static/py.png`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/py.svg` & `python_docs_theme-2024.4/python_docs_theme/static/py.svg`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/pydoctheme.css` & `python_docs_theme-2024.4/python_docs_theme/static/pydoctheme.css`

 * *Files 10% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 
 .stableabi {
     color: #229;
 }
 
 dl > dt span ~ em,
 .sig {
-    font-family: ui-monospace, "Cascadia Mono", "Segoe UI Mono", "Liberation Mono", Menlo, Monaco, Consolas, monospace;
+    font-family: Menlo, Consolas, Monaco, Liberation Mono, Lucida Console, monospace;
 }
 
 .toctree-wrapper ul {
     padding-left: 20px;
 }
 
 .theme-selector {
@@ -618,7 +618,54 @@
 }
 
 @media (min-width: 1024px) {
     div.footer {
         margin-top: -2em;
     }
 }
+
+/* Version change directives */
+:root {
+    --versionadded: rgb(41 100 51);
+    --versionchanged: rgb(133 72 38);
+    --deprecated: rgb(159 49 51);
+
+    --versionadded-border: rgb(79 196 100);
+    --versionchanged-border: rgb(244, 227, 76);
+    --deprecated-border: rgb(244, 76, 78);
+}
+
+div.versionadded,
+div.versionchanged,
+div.deprecated,
+div.deprecated-removed {
+    border-left: 3px solid;
+    padding: 0 1rem;
+}
+
+div.versionadded {
+    border-left-color: var(--versionadded-border);
+}
+
+div.versionchanged {
+    border-left-color: var(--versionchanged-border);
+}
+
+div.deprecated,
+div.deprecated-removed,
+div.versionremoved {
+    border-left-color: var(--deprecated-border);
+}
+
+div.versionadded .versionmodified {
+    color: var(--versionadded);
+}
+
+div.versionchanged .versionmodified {
+    color: var(--versionchanged);
+}
+
+div.deprecated .versionmodified,
+div.deprecated-removed .versionmodified,
+div.versionremoved .versionmodified {
+    color: var(--deprecated);
+}
```

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/pydoctheme_dark.css` & `python_docs_theme-2024.4/python_docs_theme/static/pydoctheme_dark.css`

 * *Files 7% similar despite different names*

```diff
@@ -136,7 +136,14 @@
 /* C++ specific styling */
 
 /* Override Sphinx's basic.css to fix colour contrast */
 .sig.c   .k, .sig.c   .kt,
 .sig.cpp .k, .sig.cpp .kt {
     color: #5283ff;
 }
+
+/* Version change directives */
+:root {
+    --versionadded: rgb(79 196 100);
+    --versionchanged: rgb(244, 227, 76);
+    --deprecated: rgb(244, 76, 78);
+}
```

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/search-focus.js` & `python_docs_theme-2024.4/python_docs_theme/static/search-focus.js`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/sidebar.js_t` & `python_docs_theme-2024.4/python_docs_theme/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/static/themetoggle.js` & `python_docs_theme-2024.4/python_docs_theme/static/themetoggle.js`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/python_docs_theme/theme.conf` & `python_docs_theme-2024.4/python_docs_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `python_docs_theme-2024.3/PKG-INFO` & `python_docs_theme-2024.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-docs-theme
-Version: 2024.3
+Version: 2024.4
 Summary: The Sphinx theme for the CPython docs and related projects
 Author-email: PyPA <distutils-sig@python.org>
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,39 +21,40 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Project-URL: Code, https://github.com/python/python-docs-theme
 Project-URL: Download, https://pypi.org/project/python-docs-theme/
 Project-URL: Homepage, https://github.com/python/python-docs-theme/
 Project-URL: Issue tracker, https://github.com/python/python-docs-theme/issues
 
-Python Docs Sphinx Theme
-=========================
+# Python Docs Sphinx Theme
 
 This is the theme for the Python documentation.
 
 Note that when adopting this theme, you're also borrowing an element of the
 trust and credibility established by the CPython core developers over the
 years. That's fine, and you're welcome to do so for other Python community
 projects if you so choose, but please keep in mind that in doing so you're also
 choosing to accept some of the responsibility for maintaining that collective
 trust.
 
-To use the theme, install it into your docs build environment via ``pip``
+To use the theme, install it into your docs build environment via `pip`
 (preferably in a virtual environment).
 
 
-Configuration options
----------------------
+## Configuration options
 
-To use this theme, add the following to ``conf.py``:
+To use this theme, add the following to `conf.py`:
 
-- ``html_theme = 'python_docs_theme'``
+- `html_theme = 'python_docs_theme'`
 
-- ``html_sidebars``, defaults taken from https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_sidebars
+- `html_sidebars`, defaults taken from https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_sidebars
 
-Preview
--------
+## Preview
 
 See a demo of the CPython docs using this theme:
 
 - https://python-docs-theme-previews.readthedocs.io
 
+The kitchen sink is a showcase of every Sphinx feature:
+
+- https://sphinx-themes.org/sample-sites/python-docs-theme/kitchen-sink/
+
```

