# Comparing `tmp/chaturbate_poller-0.3.1.tar.gz` & `tmp/chaturbate_poller-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.1.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.2.tar", max compression
```

## Comparing `chaturbate_poller-0.3.1.tar` & `chaturbate_poller-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1071 2024-04-07 20:22:56.967820 chaturbate_poller-0.3.1/LICENSE
--rw-r--r--   0        0        0     2259 2024-04-07 20:22:56.967820 chaturbate_poller-0.3.1/README.md
--rw-r--r--   0        0        0     3129 2024-04-07 20:23:08.519926 chaturbate_poller-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      538 2024-04-07 20:22:56.967820 chaturbate_poller-0.3.1/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     3643 2024-04-07 20:22:56.967820 chaturbate_poller-0.3.1/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      669 2024-04-07 20:22:56.967820 chaturbate_poller-0.3.1/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     2635 2024-04-07 20:22:56.971820 chaturbate_poller-0.3.1/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     3428 2024-04-07 20:22:56.971820 chaturbate_poller-0.3.1/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/README.md
+-rw-r--r--   0        0        0     3129 2024-04-08 23:42:14.741685 chaturbate_poller-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      538 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     3838 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      669 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     2211 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     3441 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.2/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.1/LICENSE` & `chaturbate_poller-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.1/README.md` & `chaturbate_poller-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -34,25 +34,45 @@
 ```
 CB_USERNAME=your_chaturbate_username
 CB_TOKEN=your_api_token
 ```
 
 Replace `your_chaturbate_username` and `your_api_token` with your actual Chaturbate username and API token.
 
-## Usage
-
-To run the Chaturbate Poller, use the following command from the root directory of the project:
+## Usage Examples
 
 ```bash
-python examples/example.py
+import asyncio
+import logging
+import os
+
+from chaturbate_poller import ChaturbateClient
+from dotenv import load_dotenv
+
+load_dotenv()
+
+username = os.getenv("CB_USERNAME", "")
+token = os.getenv("CB_TOKEN", "")
+
+
+async def main() -> None:
+    async with ChaturbateClient(username, token, 20) as client:
+        response = await client.fetch_events()
+        for event in response.events:
+            logging.info(event.dict())  # Log the event as a dictionary
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+
 ```
 
-The application will start, log into the console, and begin fetching events from the Chaturbate API using the credentials provided in the `.env` file.
+The application will start and begin fetching and printing events from the Chaturbate API using the credentials provided in the `.env` file.
 
-See `examples/example.py` for more detailed usage instructions.
+See `examples/` for more detailed usage instructions, including usage regarding the included Pydantic models.
 
 ## Development
 
 For development purposes, especially to run tests or develop additional features, consider setting up a virtual environment and installing the development dependencies:
 
 ```bash
 python -m venv .venv
```

### Comparing `chaturbate_poller-0.3.1/pyproject.toml` & `chaturbate_poller-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.1"
+version = "0.3.2"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.1/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.2/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.1/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.2/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Chaturbate poller module."""
 
 import logging
+from logging.config import dictConfig
 from types import TracebackType
 
 import backoff
 import httpx
 from httpx import HTTPStatusError, RequestError
 
 from .constants import BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
+from .logging_config import LOGGING_CONFIG
 from .models import EventsAPIResponse
 
+dictConfig(LOGGING_CONFIG)
+"""Use the logging configuration from LOGGING_CONFIG."""
+
 logger = logging.getLogger(__name__)
+"""Logger for the module."""
 
 
 class ChaturbateClient:
     """Client for fetching Chaturbate events.
 
     Args:
         username (str): The Chaturbate username.
```

### Comparing `chaturbate_poller-0.3.1/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.2/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.1/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.2/src/chaturbate_poller/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     """str: The user's recent tips."""
     gender: str
     """str: The user's gender."""
     subgender: str | None = None
     """str: The user's subgender. (Optional)"""
 
 
-class CombinedObject(BaseModel):
-    """Model for the CombinedObject object."""
+class EventObject(BaseModel):
+    """Model for the EventObject object."""
 
     broadcaster: str | None = None
     """str: The broadcaster."""
     user: User | None = None
     """User: The user."""
     media: Media | None = None
     """Media: The media."""
@@ -83,25 +83,25 @@
 
 
 class Event(BaseModel):
     """Model for the Event object."""
 
     method: str
     """str: The event method."""
-    object: CombinedObject = Field(..., alias="object")
-    """CombinedObject: The event object."""
+    object: EventObject = Field(..., alias="object")
+    """EventObject: The event object."""
     id: str
     """str: The event ID."""
 
 
 class EventsAPIResponse(BaseModel):
     """Model for the EventsAPIResponse object."""
 
     events: list[Event]
-    """list[Event]: The events."""
+    """list[Event]: A list containing the event objects."""
     next_url: str | None = Field(..., alias="nextUrl")
     """str: The next URL."""
 
 
 json_string = """
 {
     "events":[
```

### Comparing `chaturbate_poller-0.3.1/PKG-INFO` & `chaturbate_poller-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.1
+Version: 0.3.2
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -56,25 +56,45 @@
 ```
 CB_USERNAME=your_chaturbate_username
 CB_TOKEN=your_api_token
 ```
 
 Replace `your_chaturbate_username` and `your_api_token` with your actual Chaturbate username and API token.
 
-## Usage
-
-To run the Chaturbate Poller, use the following command from the root directory of the project:
+## Usage Examples
 
 ```bash
-python examples/example.py
+import asyncio
+import logging
+import os
+
+from chaturbate_poller import ChaturbateClient
+from dotenv import load_dotenv
+
+load_dotenv()
+
+username = os.getenv("CB_USERNAME", "")
+token = os.getenv("CB_TOKEN", "")
+
+
+async def main() -> None:
+    async with ChaturbateClient(username, token, 20) as client:
+        response = await client.fetch_events()
+        for event in response.events:
+            logging.info(event.dict())  # Log the event as a dictionary
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+
 ```
 
-The application will start, log into the console, and begin fetching events from the Chaturbate API using the credentials provided in the `.env` file.
+The application will start and begin fetching and printing events from the Chaturbate API using the credentials provided in the `.env` file.
 
-See `examples/example.py` for more detailed usage instructions.
+See `examples/` for more detailed usage instructions, including usage regarding the included Pydantic models.
 
 ## Development
 
 For development purposes, especially to run tests or develop additional features, consider setting up a virtual environment and installing the development dependencies:
 
 ```bash
 python -m venv .venv
```

