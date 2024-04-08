# Comparing `tmp/sdwi2iextender-0.0.9.tar.gz` & `tmp/sdwi2iextender-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdwi2iextender-0.0.9.tar", last modified: Thu Jan 18 01:59:10 2024, max compression
+gzip compressed data, was "sdwi2iextender-0.1.0.tar", last modified: Mon Apr  8 22:50:58 2024, max compression
```

## Comparing `sdwi2iextender-0.0.9.tar` & `sdwi2iextender-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 01:59:10.227615 sdwi2iextender-0.0.9/
--rw-rw-rw-   0        0        0     3627 2024-01-18 01:59:10.226616 sdwi2iextender-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3281 2024-01-17 19:19:58.000000 sdwi2iextender-0.0.9/README.md
--rw-rw-rw-   0        0        0      358 2024-01-18 01:58:52.000000 sdwi2iextender-0.0.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-18 01:59:10.211615 sdwi2iextender-0.0.9/sdwi2iextender/
--rw-rw-rw-   0        0        0      110 2024-01-18 01:58:20.000000 sdwi2iextender-0.0.9/sdwi2iextender/__init__.py
--rw-rw-rw-   0        0        0      744 2024-01-18 01:51:49.000000 sdwi2iextender-0.0.9/sdwi2iextender/gradio_helpers.py
-drwxrwxrwx   0        0        0        0 2024-01-18 01:59:10.224617 sdwi2iextender-0.0.9/sdwi2iextender/lib/
--rw-rw-rw-   0        0        0     4743 2024-01-18 01:58:20.000000 sdwi2iextender-0.0.9/sdwi2iextender/lib/img2img_tab_extender.py
--rw-rw-rw-   0        0        0      224 2023-11-04 03:21:41.000000 sdwi2iextender-0.0.9/sdwi2iextender/lib/one_time_callable.py
--rw-rw-rw-   0        0        0      356 2024-01-17 19:41:23.000000 sdwi2iextender-0.0.9/sdwi2iextender/lib/operation_mode.py
-drwxrwxrwx   0        0        0        0 2024-01-18 01:59:10.225616 sdwi2iextender-0.0.9/sdwi2iextender.egg-info/
--rw-rw-rw-   0        0        0     3627 2024-01-18 01:59:10.000000 sdwi2iextender-0.0.9/sdwi2iextender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-01-18 01:59:10.000000 sdwi2iextender-0.0.9/sdwi2iextender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 01:59:10.000000 sdwi2iextender-0.0.9/sdwi2iextender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-01-18 01:59:10.000000 sdwi2iextender-0.0.9/sdwi2iextender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-18 01:59:10.228617 sdwi2iextender-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 22:50:58.206138 sdwi2iextender-0.1.0/
+-rw-rw-rw-   0        0        0     1083 2024-01-20 11:18:02.000000 sdwi2iextender-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6191 2024-04-08 22:50:58.204139 sdwi2iextender-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5822 2024-04-08 21:29:24.000000 sdwi2iextender-0.1.0/README.md
+-rw-rw-rw-   0        0        0      358 2024-04-08 22:48:21.000000 sdwi2iextender-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-08 22:50:58.187138 sdwi2iextender-0.1.0/sdwi2iextender/
+-rw-rw-rw-   0        0        0      110 2024-01-18 01:58:20.000000 sdwi2iextender-0.1.0/sdwi2iextender/__init__.py
+-rw-rw-rw-   0        0        0     1507 2024-04-06 14:57:11.000000 sdwi2iextender-0.1.0/sdwi2iextender/gradio_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:50:58.202137 sdwi2iextender-0.1.0/sdwi2iextender/lib/
+-rw-rw-rw-   0        0        0     5303 2024-04-07 00:18:16.000000 sdwi2iextender-0.1.0/sdwi2iextender/lib/img2img_component_injector.py
+-rw-rw-rw-   0        0        0     5912 2024-04-08 21:32:58.000000 sdwi2iextender-0.1.0/sdwi2iextender/lib/img2img_tab_extender.py
+-rw-rw-rw-   0        0        0      224 2023-11-04 03:21:41.000000 sdwi2iextender-0.1.0/sdwi2iextender/lib/one_time_callable.py
+-rw-rw-rw-   0        0        0      443 2024-04-08 16:38:50.000000 sdwi2iextender-0.1.0/sdwi2iextender/lib/operation_mode.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:50:58.203136 sdwi2iextender-0.1.0/sdwi2iextender.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-04-08 22:50:58.000000 sdwi2iextender-0.1.0/sdwi2iextender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-08 22:50:58.000000 sdwi2iextender-0.1.0/sdwi2iextender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 22:50:58.000000 sdwi2iextender-0.1.0/sdwi2iextender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 22:50:58.000000 sdwi2iextender-0.1.0/sdwi2iextender.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 22:50:58.206138 sdwi2iextender-0.1.0/setup.cfg
```

### Comparing `sdwi2iextender-0.0.9/sdwi2iextender/lib/img2img_tab_extender.py` & `sdwi2iextender-0.1.0/sdwi2iextender/lib/img2img_tab_extender.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from dataclasses import dataclass
 import functools
 import gradio as gr
 
 from modules.scripts import script_callbacks
 from modules import ui_loadsave
 
-from ..gradio_helpers import GradioContextSwitch
+from ..gradio_helpers import GradioContextSwitch, hijack_gradio_encode_pil_to_base64
 from .one_time_callable import one_time_callable
+from .img2img_component_injector import activate_injector
 
 
 new_tab_classes = []
 
 
 def register_operation_mode(tab_class):
+    hijack_gradio_encode_pil_to_base64()
     enable_tab_extender()
     new_tab_classes.append(tab_class)
 
 
 @dataclass
 class TabData:
     tab_index: int
     tab_class: type
     tab_object: object
+    selected: gr.Checkbox
 
 
 class Img2imgTabExtender:
     img2img_tabs_block = None
     inpaint_params_block = None
     amount_of_default_tabs = None
     tab_data_list = []
@@ -52,94 +55,113 @@
 
     @classmethod
     def register_requested_elem_ids(cls, component, elem_id):
         if elem_id is None:
             return
 
         for tab_class in new_tab_classes:
-            if not hasattr(tab_class, 'requested_elem_ids'):
-                continue
-
             if not hasattr(tab_class, '_registered_elem_ids'):
                 tab_class._registered_elem_ids = dict()
 
+            if not hasattr(tab_class, 'requested_elem_ids'):
+                continue
+
             if elem_id in tab_class.requested_elem_ids:
                 tab_class._registered_elem_ids[elem_id] = component
 
     @classmethod
-    def create_custom_tabs(cls):
-        cls.register_default_amount_of_tabs()
+    def create_custom_tab_objects(cls, selected_tab_index_component):
+        cls.selected_tab_index_component = selected_tab_index_component
+        
         cls.tab_data_list = []
-
         for tab_class in new_tab_classes:
-            tab_index = cls._find_new_tab_index()
-            custom_tab_object = tab_class(tab_index)
-            registered_components = getattr(tab_class, "_registered_elem_ids", None)
+            custom_tab_object = tab_class()
+            cls.register_custom_tab_data(-1, tab_class, custom_tab_object, gr.Checkbox())
 
+    @classmethod
+    def instantiate_custom_tabs(cls):
+        cls.register_default_amount_of_tabs()
+        for custom_tab in cls.tab_data_list:
+            tab_class = custom_tab.tab_class
+            custom_tab_object = custom_tab.tab_object
+            tab_index = cls._get_current_amount_of_tabs()
+            custom_tab.tab_index = tab_index
+            
             with GradioContextSwitch(cls.img2img_tabs_block):
                 custom_tab_object.tab()
             with GradioContextSwitch(cls.inpaint_params_block):
-                custom_tab_object.section(registered_components)
+                custom_tab_object.section(tab_class._registered_elem_ids)
 
-            cls.register_custom_tab_data(tab_index, tab_class, custom_tab_object)
-
-            with GradioContextSwitch(cls.inpaint_params_block):
-                img2img_tabs = cls._get_img2img_tabs()
-                cls.setup_navigation_events(img2img_tabs)
-                for tab_data in cls.tab_data_list:
-                    tab_data.tab_object.gradio_events(img2img_tabs)
+        with GradioContextSwitch(cls.inpaint_params_block):
+            img2img_tabs = cls._get_img2img_tabs()
+            cls.setup_navigation_events(img2img_tabs)
+            for tab_data in cls.tab_data_list:
+                tab_data.tab_object.gradio_events(tab_data.selected)
 
     @classmethod
     def register_default_amount_of_tabs(cls):
-        cls.amount_of_default_tabs = cls._find_new_tab_index()
+        cls.amount_of_default_tabs = cls._get_current_amount_of_tabs()
 
     @classmethod
-    def register_custom_tab_data(cls, tab_index, tab_class, tab_object):
-        cls.tab_data_list.append(TabData(tab_index, tab_class, tab_object))
+    def register_custom_tab_data(cls, tab_index, tab_class, tab_object, selected):
+        cls.tab_data_list.append(TabData(tab_index, tab_class, tab_object, selected))
 
     @classmethod
     def setup_navigation_events(cls, img2img_tabs):
-        block_data_iterator = zip(img2img_tabs[cls.amount_of_default_tabs:], cls.tab_data_list, strict=True)
-        for tab_block, custom_tab in block_data_iterator:
-            def update_func(custom_tab):
-                should_show_inpaint_params = getattr(custom_tab.tab_class, 'show_inpaint_params', True)
-                return gr.update(visible=should_show_inpaint_params)
+        padded_tab_data_list = [None] * cls.amount_of_default_tabs + cls.tab_data_list
+        block_data_iterator = zip(img2img_tabs, padded_tab_data_list, strict=True)
 
+        def update_func(custom_tab):
+            tab_class = getattr(custom_tab, 'tab_class', None)
+            should_show_inpaint_params = getattr(tab_class, 'show_inpaint_params', True)
+            update_inpaint_params = gr.update(visible=should_show_inpaint_params) if custom_tab is not None else gr.update()
+            offset = cls.amount_of_default_tabs
+            update_selected = [
+                gr.update(value=custom_tab is not None and (i + offset)==custom_tab.tab_index) 
+                for i in range(len(cls.tab_data_list))
+            ]
+            return update_inpaint_params, *update_selected
+        
+        for tab_block, custom_tab in block_data_iterator:
             func_dict = dict(
                 fn=functools.partial(update_func, custom_tab=custom_tab),
                 inputs=[],
                 outputs=[
-                    cls.inpaint_params_block
+                    cls.inpaint_params_block,
+                    *[tab_data.selected for tab_data in cls.tab_data_list],
                 ]
             )
 
             tab_block.select(**func_dict)
+            tab_block.select(
+                fn=None,
+                inputs=[],
+                outputs=[cls.selected_tab_index_component],
+                _js="(...args) => [get_tab_index('mode_img2img')]",
+            )
 
     @classmethod
-    def _find_new_tab_index(cls):
-        img2img_tabs = [
-            child
-            for child in cls.img2img_tabs_block.children
-            if isinstance(child, gr.TabItem)
-        ]
-        return len(img2img_tabs)
+    def _get_current_amount_of_tabs(cls):
+        return len(cls._get_img2img_tabs())
 
     @classmethod
     def _get_img2img_tabs(cls):
         return [
             child
             for child in cls.img2img_tabs_block.children
             if isinstance(child, gr.TabItem)
         ]
 
 
 @one_time_callable
 def enable_tab_extender():
+    activate_injector()
+
     script_callbacks.on_after_component(Img2imgTabExtender.on_after_component)
 
     original_ui_settings__init__ = ui_loadsave.UiLoadsave.__init__
 
     def hijack__init__(*args, **kwargs):
-        Img2imgTabExtender.create_custom_tabs()
+        Img2imgTabExtender.instantiate_custom_tabs()
         return original_ui_settings__init__(*args, **kwargs)
 
     ui_loadsave.UiLoadsave.__init__ = hijack__init__
```

