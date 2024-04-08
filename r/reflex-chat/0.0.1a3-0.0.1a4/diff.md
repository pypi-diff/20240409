# Comparing `tmp/reflex-chat-0.0.1a3.tar.gz` & `tmp/reflex-chat-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-chat-0.0.1a3.tar", last modified: Wed Mar 13 02:44:02 2024, max compression
+gzip compressed data, was "reflex-chat-0.0.1a4.tar", last modified: Mon Apr  8 22:00:09 2024, max compression
```

## Comparing `reflex-chat-0.0.1a3.tar` & `reflex-chat-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-03-13 02:44:02.132244 reflex-chat-0.0.1a3/
--rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-03-13 02:44:02.132012 reflex-chat-0.0.1a3/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)       93 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a3/README.md
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-03-13 02:44:02.129807 reflex-chat-0.0.1a3/custom_components/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-03-13 02:44:02.130552 reflex-chat-0.0.1a3/custom_components/reflex_chat/
--rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     4089 2024-03-13 02:36:04.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat/chat.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-03-13 02:44:02.131663 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-03-13 02:44:02.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      368 2024-03-13 02:44:02.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-03-13 02:44:02.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-03-13 02:44:02.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-03-13 02:44:02.000000 reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      668 2024-03-13 02:43:37.000000 reflex-chat-0.0.1a3/pyproject.toml
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-03-13 02:44:02.132282 reflex-chat-0.0.1a3/setup.cfg
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.216578 reflex-chat-0.0.1a4/
+-rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-04-08 22:00:09.216375 reflex-chat-0.0.1a4/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)       93 2024-03-07 21:28:46.000000 reflex-chat-0.0.1a4/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.214466 reflex-chat-0.0.1a4/custom_components/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.215119 reflex-chat-0.0.1a4/custom_components/reflex_chat/
+-rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     4771 2024-03-27 23:06:34.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat/chat.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-08 22:00:09.216060 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)      570 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      368 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-08 22:00:09.000000 reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      669 2024-04-08 18:52:03.000000 reflex-chat-0.0.1a4/pyproject.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-08 22:00:09.216624 reflex-chat-0.0.1a4/setup.cfg
```

### Comparing `reflex-chat-0.0.1a3/PKG-INFO` & `reflex-chat-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Reflex custom component chat
 Author-email: Your Name <YOUREMAIL@domain.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
```

### Comparing `reflex-chat-0.0.1a3/custom_components/reflex_chat/chat.py` & `reflex-chat-0.0.1a4/custom_components/reflex_chat/chat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,74 @@
 """A custom component for a chat interface."""
 
 from typing import ClassVar
 
 import reflex as rx
 
 
-class Chat(rx.Base):
-    """"""
+class Chat(rx.ComponentState):
+    """A chat component with state."""
 
     # The full chat history.
     messages: list[dict[str, str]] = [{
         "role": "system",
         "content": "You are a friendly chatbot named Reflex. Respond in markdown."
     }]
 
     # Whether we are processing the question.
     processing: bool = False
 
-    # Dynamic creation of per-component State classes
-    _instances: ClassVar[int] = 0
-
     @classmethod
-    def create(cls, process, **props) -> rx.Component:
-        cls._instances += 1
-        return type(
-            f"{cls.__name__}_n{cls._instances}", (cls, rx.State), {}
-        ).component(process, _id=cls._instances, **props)
+    def create(self, process, **props):
+        component = super().create(**props)
+        component.State.process = process
+        return component
 
     @classmethod
-    def component(cls, process, **props) -> rx.Component:
-        cls.process = process
+    def get_component(cls, **props) -> rx.Component:
         return rx.vstack(
-            rx.box(
-                rx.foreach(cls.messages, lambda message, i: chat_bubble(message, i)),
-                id=f"chatbox-{cls.__name__}",
-                overflow="auto",
+            rx.link(
+                rx.hstack(
+                    "Built with ",
+                    rx.image(src="/Reflex.svg"),
+                    align="center",
+                    background_color=rx.color("purple", 4),
+                    border_bottom=f"1px solid {rx.color('purple', 6)}",
+                    width="100%",
+                    padding="1em",
+                ),
                 width="100%",
-                padding_bottom="2em",
+                href="https://reflex.dev",
+                _hover={
+                    "text_decoration": "none",
+                },
+                color=rx.color("mauve", 12),
+                is_external=True,
             ),
             rx.spacer(),
-            action_bar(cls),
+            rx.vstack(
+                rx.box(
+                    rx.foreach(cls.messages, lambda message, i: chat_bubble(message, i)),
+                    id=f"chatbox-{cls.__name__}",
+                    overflow="auto",
+                    width="100%",
+                    padding_bottom="2em",
+                ),
+                rx.spacer(),
+                action_bar(cls),
+                padding=props.pop("padding", "1em"),
+                background_color=props.pop("background_color", rx.color("mauve", 1)),
+                border=props.pop("border", f"1px solid {rx.color('mauve', 4)}"),
+                height="100%",
+                width="100%",
+                **props,
+            ),
+            spacing="0",
             height="100%",
             width="100%",
-            padding=props.pop("padding", "1em"),
-            background_color=props.pop("background_color", rx.color("mauve", 1)),
-            border=props.pop("border", f"1px solid {rx.color('mauve', 4)}"),
-            **props
         )
 
     def scroll_to_bottom(self):
         return rx.call_script(
             f"""
     var element = document.getElementById('chatbox-{type(self).__name__}');
     element.scrollTop = element.scrollHeight;
@@ -92,16 +111,16 @@
     """
     return rx.cond(
         message["role"] == "system",
         rx.fragment(),
         rx.box(
             rx.markdown(
                 message["content"],
-                background_color=rx.cond(message["role"] == "user", rx.color("mauve", 4), rx.color("accent", 4)),
-                color=rx.cond(message["role"] == "user", rx.color("mauve", 12), rx.color("accent", 12)),
+                background_color=rx.cond(message["role"] == "user", rx.color("mauve", 4), rx.color("purple", 4)),
+                color=rx.cond(message["role"] == "user", rx.color("mauve", 12), rx.color("purple", 12)),
                 display="inline-block",
                 padding_x="1em",
                 border_radius="8px",
                 max_width=["30em", "30em", "50em", "50em", "50em", "50em"],
             ),
             id=f"message-{idx}",
             text_align=rx.cond(message["role"] == "user", "right", "left"),
```

### Comparing `reflex-chat-0.0.1a3/custom_components/reflex_chat.egg-info/PKG-INFO` & `reflex-chat-0.0.1a4/custom_components/reflex_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Reflex custom component chat
 Author-email: Your Name <YOUREMAIL@domain.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
```

### Comparing `reflex-chat-0.0.1a3/pyproject.toml` & `reflex-chat-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-chat"
-version = "0.0.1a3"
+version = "0.0.1a4"
 description = "Reflex custom component chat"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Your Name", email = "YOUREMAIL@domain.com" }]
 keywords = [
     "reflex",
@@ -28,8 +28,8 @@
 [project.urls]
 Homepage = "https://github.com"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.setuptools.packages.find]
-where = ["custom_components"]
+where = ["custom_components"]
```

