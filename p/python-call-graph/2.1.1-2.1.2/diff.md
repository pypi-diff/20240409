# Comparing `tmp/python-call-graph-2.1.1.tar.gz` & `tmp/python-call-graph-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-call-graph-2.1.1.tar", last modified: Sun Mar 31 14:51:21 2024, max compression
+gzip compressed data, was "python-call-graph-2.1.2.tar", last modified: Tue Apr  9 07:35:41 2024, max compression
```

## Comparing `python-call-graph-2.1.1.tar` & `python-call-graph-2.1.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.267495 python-call-graph-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.267495 python-call-graph-2.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.267495 python-call-graph-2.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.267495 python-call-graph-2.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/globbing_filter.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/output.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/pycallgraph.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/api/tracer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.271494 python-call-graph-2.1.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    31702 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/basic.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/basic.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22218 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/basic_thumb.png
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/examples.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1635 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1449 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp.py
--rw-r--r--   0 runner    (1001) docker     (127)   158650 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_grouped.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_grouped_thumb.png
--rw-r--r--   0 runner    (1001) docker     (127)   142780 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_ungrouped.png
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_ungrouped.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18530 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/examples/regexp_ungrouped_thumb.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.271494 python-call-graph-2.1.1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/command_line_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/custom_outputs.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.271494 python-call-graph-2.1.1/docs/guide/filtering/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/banana.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/examples.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_exclude.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_max_depth.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      346 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_max_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_none.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/filter_none.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/filtering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/guide/outputs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.271494 python-call-graph-2.1.1/man/
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/man/pycallgraph.1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/pycallgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/color.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5396 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/globbing_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/grouper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/memory_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/pycallgraph/output/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/gephi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/output/ubigraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/pycallgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/pycallgraph/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/python_call_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22267 2024-03-31 14:51:21.000000 python-call-graph-2.1.1/python_call_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-31 14:51:21.000000 python-call-graph-2.1.1/python_call_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:51:21.000000 python-call-graph-2.1.1/python_call_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 14:51:21.000000 python-call-graph-2.1.1/python_call_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:51:21.000000 python-call-graph-2.1.1/python_call_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/scripts/pycallgraph
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2496 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:51:21.275495 python-call-graph-2.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_gephi.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_pycallgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_trace_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-31 14:51:15.000000 python-call-graph-2.1.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.667839 python-call-graph-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.667839 python-call-graph-2.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.667839 python-call-graph-2.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.667839 python-call-graph-2.1.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/globbing_filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/pycallgraph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/api/tracer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.671840 python-call-graph-2.1.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    31702 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/basic.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22218 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/basic_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/examples.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1635 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1449 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158650 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_grouped.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_grouped_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (127)   142780 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_ungrouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_ungrouped.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18530 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/examples/regexp_ungrouped_thumb.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.671840 python-call-graph-2.1.2/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/command_line_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/custom_outputs.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.675840 python-call-graph-2.1.2/docs/guide/filtering/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/banana.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_exclude.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_max_depth.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      346 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_max_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_none.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/filter_none.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/guide/outputs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.675840 python-call-graph-2.1.2/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/man/pycallgraph.1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.675840 python-call-graph-2.1.2/pycallgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/color.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5396 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/globbing_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/grouper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/memory_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.675840 python-call-graph-2.1.2/pycallgraph/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/gephi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/output/ubigraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/pycallgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/pycallgraph/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/python_call_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-04-09 07:35:41.000000 python-call-graph-2.1.2/python_call_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-09 07:35:41.000000 python-call-graph-2.1.2/python_call_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:35:41.000000 python-call-graph-2.1.2/python_call_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 07:35:41.000000 python-call-graph-2.1.2/python_call_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 07:35:41.000000 python-call-graph-2.1.2/python_call_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/scripts/pycallgraph
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2496 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:35:41.679839 python-call-graph-2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_gephi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_pycallgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_trace_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 07:35:31.000000 python-call-graph-2.1.2/test/test_util.py
```

### Comparing `python-call-graph-2.1.1/LICENSE` & `python-call-graph-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/Makefile` & `python-call-graph-2.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/PKG-INFO` & `python-call-graph-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-call-graph
-Version: 2.1.1
-Summary: Python Call Graph is a library and command line tool that visualises the flow of your Python application.  This is a fork of the original, updated to work with Python 3.5 - 3.11 and from 2.1.0 3.8 - 3.12  See https://pycallgraph.readthedocs.io/en/develop/ for more information.
+Version: 2.1.2
+Summary: Python Call Graph is a library and command line tool that visualises the flow of your Python application.  This is a fork of the original, updated to work with Python 3.5 - 3.11 and from 2.1.0 3.8 - 3.12  See https://lewiscowles1986.github.io/py-call-graph/ for more information.
 Home-page: http://pycallgraph.readthedocs.io/
 Author: Gerald Kaszuba
 Author-email: pycallgraph@gakman.com
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -306,29 +306,29 @@
 Provides-Extra: memory-psutil
 License-File: LICENSE
 
 # Python Call Graph
 
 Welcome! Python Call Graph is a [Python](http://www.python.org) module that creates [call graph](http://en.wikipedia.org/wiki/Call_graph) visualizations for Python applications.
 
-This repo used to be `pycallgraph` which is still hosted at pypi [link](https://pypi.org/project/pycallgraph/).
+This repo used to be `pycallgraph` which is still hosted at pypi [link](https://pypi.org/project/python-call-graph/).
 
 The uploader makes no representations of their contribution, and merely wanted this to work in python 3.5; with a goal to porting it to 3.11 and 3.12
 
 [![CI Status](https://github.com/Lewiscowles1986/py-call-graph/actions/workflows/ci.yml/badge.svg)](https://github.com/Lewiscowles1986/py-call-graph/actions/workflows/ci.yml)
 
 ## Screenshots
 
 Click on the images below to see a larger version and the source code that generated them.
 
-[![Basic Output thumbnail](http://pycallgraph.readthedocs.io/en/develop/_images/basic_thumb.png)](http://pycallgraph.readthedocs.io/en/develop/examples/basic.html)
+[![Basic Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/basic_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/basic.html)
 
-[![Regex grouped Output thumbnail](https://pycallgraph.readthedocs.io/en/develop/_images/regexp_grouped_thumb.png)](https://pycallgraph.readthedocs.io/en/develop/examples/regexp_grouped.html)
+[![Regex grouped Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/regexp_grouped_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/regexp_grouped)
 
-[![Regex ungrouped Output thumbnail](https://pycallgraph.readthedocs.io/en/develop/_images/regexp_ungrouped_thumb.png)](https://pycallgraph.readthedocs.io/en/develop/examples/regexp_ungrouped.html)
+[![Regex ungrouped Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/regexp_ungrouped_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/regexp_ungrouped.html)
 
 ## Project Status
 
 The latest version is **2.1.1** which was released on 2024-03-31.
 The latest version has been tested running on Python versions 3.8 - 3.12
 
 The [project lives on GitHub](https://github.com/lewiscowles1986/py-call-graph/#python-call-graph), where you can [report issues](https://github.com/lewiscowles1986/py-call-graph/issues), contribute to the project by [forking the project](https://help.github.com/articles/fork-a-repo) then creating a [pull request](https://help.github.com/articles/using-pull-requests), or just [browse the source code](https://github.com/lewiscowles1986/py-call-graph/).
@@ -349,15 +349,15 @@
 Installation is easy as
 
 ```shell
 pip install python-call-graph
 
 ```
 
-You can either use the [command-line interface](https://pycallgraph.readthedocs.io/en/develop/guide/command_line_usage.html) for a quick visualization of your Python script, or the [pycallgraph module](https://pycallgraph.readthedocs.io/en/develop/api/pycallgraph.html) for more fine-grained settings.
+You can either use the [command-line interface](https://lewiscowles1986.github.io/py-call-graph/guide/command_line_usage.html) for a quick visualization of your Python script, or the [pycallgraph module](https://lewiscowles1986.github.io/py-call-graph/api/pycallgraph.html) for more fine-grained settings.
 
 The following examples specify graphviz as the outputter, so it's required to be installed. They will generate a file called `pycallgraph.png`.
 
 ### The command-line method of running pycallgraph is
 
 ```shell
 pycallgraph graphviz -- ./mypythonscript.py
@@ -373,8 +373,8 @@
 with PyCallGraph(output=GraphvizOutput()):
     code_to_profile()
 
 ```
 
 ## Documentation
 
-Feel free to browse the [documentation of pycallgraph](https://pycallgraph.readthedocs.io/en/develop/) for the [usage guide](https://pycallgraph.readthedocs.io/en/develop/guide/index.html) and [API reference](https://pycallgraph.readthedocs.io/en/develop/api/api.html).
+Feel free to browse the [documentation of pycallgraph](https://lewiscowles1986.github.io/py-call-graph/) for the [usage guide](https://lewiscowles1986.github.io/py-call-graph/guide/index.html) and [API reference](https://lewiscowles1986.github.io/py-call-graph/api/api.html).
```

### Comparing `python-call-graph-2.1.1/docs/Makefile` & `python-call-graph-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/conf.py` & `python-call-graph-2.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,34 @@
 todo_include_todos = True
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.todo', 'sphinx.ext.coverage', 'sphinx.ext.viewcode']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.todo', 'sphinx.ext.coverage', 'sphinx.ext.viewcode', 'myst_parser']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.md': 'markdown',
+}
 
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'Python Call Graph'
-copyright = u'2007-2013 Gerald Kaszuba, et al.'
+copyright = u'2007-2024 Gerald Kaszuba, et al.'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = pycallgraph.__version__
```

### Comparing `python-call-graph-2.1.1/docs/examples/basic.png` & `python-call-graph-2.1.2/docs/examples/basic.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/basic.py` & `python-call-graph-2.1.2/docs/examples/basic.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/basic_thumb.png` & `python-call-graph-2.1.2/docs/examples/basic_thumb.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/examples.yml` & `python-call-graph-2.1.2/docs/examples/examples.yml`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/generate.py` & `python-call-graph-2.1.2/docs/examples/generate.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp.py` & `python-call-graph-2.1.2/docs/examples/regexp.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_grouped.png` & `python-call-graph-2.1.2/docs/examples/regexp_grouped.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_grouped.rst` & `python-call-graph-2.1.2/docs/examples/regexp_grouped.rst`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_grouped_thumb.png` & `python-call-graph-2.1.2/docs/examples/regexp_grouped_thumb.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_ungrouped.png` & `python-call-graph-2.1.2/docs/examples/regexp_ungrouped.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_ungrouped.rst` & `python-call-graph-2.1.2/docs/examples/regexp_ungrouped.rst`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/examples/regexp_ungrouped_thumb.png` & `python-call-graph-2.1.2/docs/examples/regexp_ungrouped_thumb.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/command_line_usage.rst` & `python-call-graph-2.1.2/docs/guide/command_line_usage.rst`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/filtering/filter_exclude.png` & `python-call-graph-2.1.2/docs/guide/filtering/filter_exclude.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/filtering/filter_max_depth.png` & `python-call-graph-2.1.2/docs/guide/filtering/filter_max_depth.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/filtering/filter_none.png` & `python-call-graph-2.1.2/docs/guide/filtering/filter_none.png`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/filtering/generate.py` & `python-call-graph-2.1.2/docs/guide/filtering/generate.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/filtering.rst` & `python-call-graph-2.1.2/docs/guide/filtering.rst`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/docs/guide/intro.rst` & `python-call-graph-2.1.2/docs/guide/intro.rst`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/man/pycallgraph.1` & `python-call-graph-2.1.2/man/pycallgraph.1`

 * *Files 0% similar despite different names*

```diff
@@ -145,10 +145,10 @@
 .UNINDENT
 .SH AUTHOR
 pycallgraph was written by Gerald Kaszuba <pycallgraph@slowchop.com>.
 
 This manual page was originally written by Jan Alonzo <jmalonzo@unpluggable.com>, for the Debian GNU/Linux system.
 
 .SH COPYRIGHT
-2007-2013 Gerald Kaszuba, et al.
+2007-2024 Gerald Kaszuba, et al.
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `python-call-graph-2.1.1/pycallgraph/__init__.py` & `python-call-graph-2.1.2/pycallgraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Python Call Graph is a library and command line tool that visualises the flow
 of your Python application.
 
 This is a fork of the original, updated to work with Python 3.5 - 3.11 and from 2.1.0 3.8 - 3.12
 
-See https://pycallgraph.readthedocs.io/en/develop/ for more information.
+See https://lewiscowles1986.github.io/py-call-graph/ for more information.
 '''
 from .metadata import __version__
 from .metadata import __copyright__
 from .metadata import __license__
 from .metadata import __author__
 from .metadata import __email__
 from .metadata import __url__
```

### Comparing `python-call-graph-2.1.1/pycallgraph/color.py` & `python-call-graph-2.1.2/pycallgraph/color.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/config.py` & `python-call-graph-2.1.2/pycallgraph/config.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/globbing_filter.py` & `python-call-graph-2.1.2/pycallgraph/globbing_filter.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/grouper.py` & `python-call-graph-2.1.2/pycallgraph/grouper.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/memory_profiler.py` & `python-call-graph-2.1.2/pycallgraph/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/output/gephi.py` & `python-call-graph-2.1.2/pycallgraph/output/gephi.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/output/graphviz.py` & `python-call-graph-2.1.2/pycallgraph/output/graphviz.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/output/output.py` & `python-call-graph-2.1.2/pycallgraph/output/output.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/output/pickle.py` & `python-call-graph-2.1.2/pycallgraph/output/pickle.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/output/ubigraph.py` & `python-call-graph-2.1.2/pycallgraph/output/ubigraph.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/pycallgraph.py` & `python-call-graph-2.1.2/pycallgraph/pycallgraph.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/pycallgraph/tracer.py` & `python-call-graph-2.1.2/pycallgraph/tracer.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/python_call_graph.egg-info/PKG-INFO` & `python-call-graph-2.1.2/python_call_graph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-call-graph
-Version: 2.1.1
-Summary: Python Call Graph is a library and command line tool that visualises the flow of your Python application.  This is a fork of the original, updated to work with Python 3.5 - 3.11 and from 2.1.0 3.8 - 3.12  See https://pycallgraph.readthedocs.io/en/develop/ for more information.
+Version: 2.1.2
+Summary: Python Call Graph is a library and command line tool that visualises the flow of your Python application.  This is a fork of the original, updated to work with Python 3.5 - 3.11 and from 2.1.0 3.8 - 3.12  See https://lewiscowles1986.github.io/py-call-graph/ for more information.
 Home-page: http://pycallgraph.readthedocs.io/
 Author: Gerald Kaszuba
 Author-email: pycallgraph@gakman.com
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -306,29 +306,29 @@
 Provides-Extra: memory-psutil
 License-File: LICENSE
 
 # Python Call Graph
 
 Welcome! Python Call Graph is a [Python](http://www.python.org) module that creates [call graph](http://en.wikipedia.org/wiki/Call_graph) visualizations for Python applications.
 
-This repo used to be `pycallgraph` which is still hosted at pypi [link](https://pypi.org/project/pycallgraph/).
+This repo used to be `pycallgraph` which is still hosted at pypi [link](https://pypi.org/project/python-call-graph/).
 
 The uploader makes no representations of their contribution, and merely wanted this to work in python 3.5; with a goal to porting it to 3.11 and 3.12
 
 [![CI Status](https://github.com/Lewiscowles1986/py-call-graph/actions/workflows/ci.yml/badge.svg)](https://github.com/Lewiscowles1986/py-call-graph/actions/workflows/ci.yml)
 
 ## Screenshots
 
 Click on the images below to see a larger version and the source code that generated them.
 
-[![Basic Output thumbnail](http://pycallgraph.readthedocs.io/en/develop/_images/basic_thumb.png)](http://pycallgraph.readthedocs.io/en/develop/examples/basic.html)
+[![Basic Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/basic_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/basic.html)
 
-[![Regex grouped Output thumbnail](https://pycallgraph.readthedocs.io/en/develop/_images/regexp_grouped_thumb.png)](https://pycallgraph.readthedocs.io/en/develop/examples/regexp_grouped.html)
+[![Regex grouped Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/regexp_grouped_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/regexp_grouped)
 
-[![Regex ungrouped Output thumbnail](https://pycallgraph.readthedocs.io/en/develop/_images/regexp_ungrouped_thumb.png)](https://pycallgraph.readthedocs.io/en/develop/examples/regexp_ungrouped.html)
+[![Regex ungrouped Output thumbnail](https://lewiscowles1986.github.io/py-call-graph/_images/regexp_ungrouped_thumb.png)](https://lewiscowles1986.github.io/py-call-graph/examples/regexp_ungrouped.html)
 
 ## Project Status
 
 The latest version is **2.1.1** which was released on 2024-03-31.
 The latest version has been tested running on Python versions 3.8 - 3.12
 
 The [project lives on GitHub](https://github.com/lewiscowles1986/py-call-graph/#python-call-graph), where you can [report issues](https://github.com/lewiscowles1986/py-call-graph/issues), contribute to the project by [forking the project](https://help.github.com/articles/fork-a-repo) then creating a [pull request](https://help.github.com/articles/using-pull-requests), or just [browse the source code](https://github.com/lewiscowles1986/py-call-graph/).
@@ -349,15 +349,15 @@
 Installation is easy as
 
 ```shell
 pip install python-call-graph
 
 ```
 
-You can either use the [command-line interface](https://pycallgraph.readthedocs.io/en/develop/guide/command_line_usage.html) for a quick visualization of your Python script, or the [pycallgraph module](https://pycallgraph.readthedocs.io/en/develop/api/pycallgraph.html) for more fine-grained settings.
+You can either use the [command-line interface](https://lewiscowles1986.github.io/py-call-graph/guide/command_line_usage.html) for a quick visualization of your Python script, or the [pycallgraph module](https://lewiscowles1986.github.io/py-call-graph/api/pycallgraph.html) for more fine-grained settings.
 
 The following examples specify graphviz as the outputter, so it's required to be installed. They will generate a file called `pycallgraph.png`.
 
 ### The command-line method of running pycallgraph is
 
 ```shell
 pycallgraph graphviz -- ./mypythonscript.py
@@ -373,8 +373,8 @@
 with PyCallGraph(output=GraphvizOutput()):
     code_to_profile()
 
 ```
 
 ## Documentation
 
-Feel free to browse the [documentation of pycallgraph](https://pycallgraph.readthedocs.io/en/develop/) for the [usage guide](https://pycallgraph.readthedocs.io/en/develop/guide/index.html) and [API reference](https://pycallgraph.readthedocs.io/en/develop/api/api.html).
+Feel free to browse the [documentation of pycallgraph](https://lewiscowles1986.github.io/py-call-graph/) for the [usage guide](https://lewiscowles1986.github.io/py-call-graph/guide/index.html) and [API reference](https://lewiscowles1986.github.io/py-call-graph/api/api.html).
```

### Comparing `python-call-graph-2.1.1/python_call_graph.egg-info/SOURCES.txt` & `python-call-graph-2.1.2/python_call_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/scripts/pycallgraph` & `python-call-graph-2.1.2/scripts/pycallgraph`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/setup.py` & `python-call-graph-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_color.py` & `python-call-graph-2.1.2/test/test_color.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_decorators.py` & `python-call-graph-2.1.2/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_gephi.py` & `python-call-graph-2.1.2/test/test_gephi.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_graphviz.py` & `python-call-graph-2.1.2/test/test_graphviz.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_pycallgraph.py` & `python-call-graph-2.1.2/test/test_pycallgraph.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_trace_processor.py` & `python-call-graph-2.1.2/test/test_trace_processor.py`

 * *Files identical despite different names*

### Comparing `python-call-graph-2.1.1/test/test_util.py` & `python-call-graph-2.1.2/test/test_util.py`

 * *Files identical despite different names*

