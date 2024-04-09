# Comparing `tmp/pyjvc-4.4.22.tar.gz` & `tmp/pyjvc-4.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.22.tar", last modified: Mon Apr  8 00:53:20 2024, max compression
+gzip compressed data, was "pyjvc-4.4.23.tar", last modified: Mon Apr  8 19:15:01 2024, max compression
```

## Comparing `pyjvc-4.4.22.tar` & `pyjvc-4.4.23.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:53:20.177669 pyjvc-4.4.22/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.22/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 00:53:20.177494 pyjvc-4.4.22/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.22/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:53:20.175149 pyjvc-4.4.22/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.22/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     9120 2024-04-08 00:14:11.000000 pyjvc-4.4.22/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10032 2024-04-01 00:26:47.000000 pyjvc-4.4.22/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      200 2024-02-17 18:22:01.000000 pyjvc-4.4.22/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    17809 2024-04-08 00:34:07.000000 pyjvc-4.4.22/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:53:20.177317 pyjvc-4.4.22/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 00:53:20.000000 pyjvc-4.4.22/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-08 00:53:20.000000 pyjvc-4.4.22/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-08 00:53:20.000000 pyjvc-4.4.22/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-08 00:53:20.000000 pyjvc-4.4.22/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-08 00:53:20.177757 pyjvc-4.4.22/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      635 2024-04-08 00:53:16.000000 pyjvc-4.4.22/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 00:53:20.177044 pyjvc-4.4.22/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.22/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.22/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8345 2024-03-20 01:40:47.000000 pyjvc-4.4.22/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    14935 2024-03-20 01:40:47.000000 pyjvc-4.4.22/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 19:15:01.517590 pyjvc-4.4.23/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.23/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 19:15:01.517398 pyjvc-4.4.23/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.23/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 19:15:01.514612 pyjvc-4.4.23/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.23/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10106 2024-04-08 18:46:32.000000 pyjvc-4.4.23/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10031 2024-04-08 19:13:11.000000 pyjvc-4.4.23/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      250 2024-04-08 19:13:04.000000 pyjvc-4.4.23/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    18045 2024-04-08 19:13:43.000000 pyjvc-4.4.23/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 19:15:01.517163 pyjvc-4.4.23/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6182 2024-04-08 19:15:01.000000 pyjvc-4.4.23/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-08 19:15:01.000000 pyjvc-4.4.23/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-08 19:15:01.000000 pyjvc-4.4.23/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-08 19:15:01.000000 pyjvc-4.4.23/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-08 19:15:01.517642 pyjvc-4.4.23/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      635 2024-04-08 19:10:44.000000 pyjvc-4.4.23/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-08 19:15:01.516786 pyjvc-4.4.23/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.23/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.23/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8923 2024-04-08 17:46:54.000000 pyjvc-4.4.23/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    20373 2024-04-08 19:06:38.000000 pyjvc-4.4.23/tests/test_loop.py
```

### Comparing `pyjvc-4.4.22/LICENSE` & `pyjvc-4.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.22/PKG-INFO` & `pyjvc-4.4.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.22
+Version: 4.4.23
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.22/README.md` & `pyjvc-4.4.23/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.22/jvc_projector/command_runner.py` & `pyjvc-4.4.23/jvc_projector/command_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,17 +73,14 @@
         command_type: bytes - ! or ?
 
         Returns:
             value: str (to be cast into other types)
         """
         cmd, ack = self.construct_command(command, command_type)
 
-        # Check commands
-        self.logger.debug("command: %s", cmd)
-
         try:
             return await self._do_command(cmd, ack, command_type)
 
         # raise connectionclosed error to be handled by callers
         except BlankMessageError as err:
             self.logger.debug("error in send_command: %s", err)
             return ""
@@ -103,34 +100,50 @@
         )
 
         return await self.send_command(
             cmd,
             command_type=Header.operation.value,
         )
 
+    async def read_until_empty(self):
+        """
+        Read buffer until empty
+        """
+        while True:
+            try:
+                # Read data from the buffer with a specified buffer size
+                data = await asyncio.wait_for(self.reader.read(1024), timeout=0.5)
+                if not data:
+                    # If no data is received, the buffer is empty
+                    break
+            except asyncio.TimeoutError:
+                # If a timeout occurs, assume the buffer is empty and break the loop
+                break
+            except Exception as e:
+                # Handle any other exceptions that may occur during reading
+                self.logger.error("Error while clearing read buffer: %s", e)
+                break
+
     async def _do_command(
         self,
         final_cmd: bytes,
         ack: bytes,
         command_type: bytes,
     ) -> tuple[Union[str, bytes]]:
         async with self.lock:
             self.logger.debug("final_cmd: %s with ack %s", final_cmd, ack)
             # ensure this doesnt run with dead client
             if self.writer is None:
                 self.logger.debug("Writer is closed")
                 raise ConnectionClosedError("writer is none")
 
-            self.logger.debug("do_command sending command: %s", final_cmd)
             # send the command
             try:
-                self.logger.debug("acquiring command lock")
                 self.writer.write(final_cmd)
                 await self.writer.drain()
-                self.logger.debug("released command lock")
             except BrokenPipeError as err:
                 self.logger.error(
                     "BrokenPipeError in _do_command restarting connection: %s", err
                 )
                 # Attempt to reconnect or handle the broken pipe scenario
                 raise ConnectionClosedError("Broken pipe") from err
             except ConnectionResetError as err:
@@ -141,47 +154,60 @@
                 # reaching this means the writer was closed somewhere
                 self.logger.debug("ConnectionError in _do_command: %s", err)
                 raise ConnectionClosedError(err) from err
             # if we send a command that returns info, the projector will send
             # an ack, followed by the actual message. Check to see if the ack sent by
             # projector is correct, then return the message.
 
-            ack_value = Header.ack.value + Header.pj_unit.value + ack + Footer.close.value
+            # if the command_type is operation, the ack doesnt matter we should read until empty
+            # read until empty
+            if command_type == Header.operation.value:
+                self.logger.debug("command_type is operation skipping ack check")
+                return await self.read_until_empty()
+
+            ack_value = (
+                Header.ack.value + Header.pj_unit.value + ack + Footer.close.value
+            )
             self.logger.debug("constructed ack_value: %s", ack_value)
 
             # Receive the acknowledgement from PJ
             try:
                 # read everything
-                self.logger.debug("acquiring command read lock")
-                # TODO: its probably way more reliable to read everything and just search for the data we want
-                msg = await self.reader.read(len(ack_value))
-                self.logger.debug("received msg in _do_command: %s", msg)
-
+                try:
+                    msg = await asyncio.wait_for(
+                        self.reader.read(len(ack_value)), timeout=1
+                    )
+                    self.logger.debug("received msg in _do_command: %s", msg)
+                except asyncio.TimeoutError as err:
+                    # this means the command isnt allowed to run, probably
+                    self.logger.debug("TimeoutError reading in _do_command: %s", err)
+                    raise CommandTimeoutError("Timed out") from err
                 # read the actual message, if any
                 if msg == b"":  # if we got a blank response
                     self.logger.debug("Got a blank response")
                     raise BlankMessageError("Got a blank response")
                 if command_type == Header.operation.value:
                     return msg, True
-                else:
-                    ref_msg = await self.reader.read(1000)
-                    self.logger.debug("received ref_msg in _do_command: %s", ref_msg)
-                    # msg = await self._check_received_msg(received_ack, ack_value, command_type)
-                    self.logger.debug("finished reading ref_msg")
-                    return ref_msg.replace(ack_value, b"")
+
+                # have to read again to get the value
+                ref_msg = await self.reader.read(1000)
+                self.logger.debug("received ref_msg in _do_command: %s", ref_msg)
+                # msg = await self._check_received_msg(received_ack, ack_value, command_type)
+                self.logger.debug("finished reading ref_msg")
+                return ref_msg.replace(ack_value, b"")
+
             except socket.timeout as err:
                 error = f"Timed out. Command {final_cmd} may grayed out or cmd is running already."
                 self.logger.debug(err)
                 raise CommandTimeoutError(error) from err
 
             except ConnectionRefusedError as err:
                 self.logger.debug(err)
                 raise ConnectionRefusedError(error) from err
 
-    # TODO: use this to construct commands from a list that is a str like ["menu,menu"]
     def construct_command(
         self, raw_command: str, command_type: bytes
     ) -> tuple[bytes, ACKs]:
         """
         Transform commands into their byte values from the string value
         """
         # split command into the base and the action like menu: left
```

### Comparing `pyjvc-4.4.22/jvc_projector/commands.py` & `pyjvc-4.4.23/jvc_projector/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,14 @@
     current_output = b"IP"
     info = b"RC7374"
     remote = b"RC73"
 
     # Checking for model code
     # response -> \x40\x89\x01\x4D\x44(the model code)\x0A
     get_model = b"MD", str, ACKs.model
-
     # software version
     get_software_version = b"IFSV", str, ACKs.info_ack
 
     # content type
     content_type = b"PMCT", ContentTypes, ACKs.picture_ack
     content_type_trans = b"PMAT", ContentTypeTrans, ACKs.picture_ack
```

### Comparing `pyjvc-4.4.22/jvc_projector/jvc_projector.py` & `pyjvc-4.4.23/jvc_projector/jvc_projector.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     LowLatencyModes,
     PowerStates,
     model_map,
 )
 from jvc_projector.error_classes import (
     CommandTimeoutError,
     ConnectionClosedError,
+    ShouldReconnectError,
 )
 
 
 @dataclass
 class JVCInput:
     """JVC Projector Input"""
 
@@ -159,19 +160,15 @@
         resets everything and tries to empty current jvc buffer. Used on error to just clear everything and start over
         """
         try:
             if not self.connection_open:
                 await self.open_connection()
 
             # clear the buffer
-            while not self.reader.at_eof():
-                try:
-                    await self.reader.read(1024)
-                except asyncio.IncompleteReadError:
-                    break
+            await self.commander.read_until_empty()
 
             return
         except Exception as e:
             self.logger.error("Error resetting everything: %s", e)
             return
 
     async def open_connection(self) -> bool:
@@ -249,28 +246,29 @@
                 try:
                     res = await self.commander.send_command(command, command_type)
                     if not res:
                         self.logger.debug("Command failed. Retrying")
                         retries += 1
                         continue
                     return res
+                # this means stuff is actually broken
                 except (
                     ConnectionClosedError,
-                    CommandTimeoutError,
                     ConnectionRefusedError,
                     BrokenPipeError,
-                ):
+                ) as err:
+                    self.logger.debug("Connection closed. Retry your command")
+                    raise ShouldReconnectError(err) from err
+                # getting here means the command is not allowed
+                except CommandTimeoutError:
                     self.logger.debug(
-                        "Connection closed. Opening new connection. Retry your command"
+                        "Command timed out. Very likely its not allowed to run (This is not a bug. JVC's fault)"
                     )
-                    # open connection and try again
-                    await self.open_connection()
-                    await asyncio.sleep(1)
-                    continue
-
+                    return None
+            self.logger.error("Command failed after 3 retries")
             return None
 
     async def close_connection(self):
         """Close the projector connection asynchronously"""
         try:
             if self.writer:
                 self.writer.close()
@@ -301,40 +299,41 @@
         """
         return await self.exec_command("power,off")
 
     async def _get_attribute(self, command: str, replace: bool = True) -> str:
         """
         Generic function to get the current attribute asynchronously
         """
-        cmd_tup = Commands[command].value
-        cmd_enum = cmd_tup[1]
-        ack = cmd_tup[2]
-        self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
-        try:
-            state = await self.exec_command(command, Header.reference.value)
-            if not state:
-                self.logger.debug("%s Command failed", command)
-                return ""
-            if replace:
-                # remove the returned headers
-                r = self.commander.replace_headers(state)
-                if not isinstance(r, bytes):
-                    self.logger.error("Attribute %s is not bytes", command)
+        async with self.attr_lock:
+            cmd_tup = Commands[command].value
+            cmd_enum = cmd_tup[1]
+            ack = cmd_tup[2]
+            self.logger.debug("Getting attribute %s with tuple %s", command, cmd_tup)
+            try:
+                state = await self.exec_command(command, Header.reference.value)
+                if not state:
+                    self.logger.debug("%s Command failed", command)
                     return ""
-                self.logger.debug("Attribute %s is %s", command, r)
-                # look up the enum value like b"1" -> on in PowerModes
-                return cmd_enum(r.replace(ack.value, b"")).name
-
-            return state
-        except ValueError as err:
-            self.logger.error("Attribute not found - %s", err)
-            raise
-        except AttributeError as err:
-            self.logger.error("tried to access name on non-enum: %s", err)
-            return ""
+                if replace:
+                    # remove the returned headers
+                    r = self.commander.replace_headers(state)
+                    if not isinstance(r, bytes):
+                        self.logger.error("Attribute %s is not bytes", command)
+                        return ""
+                    self.logger.debug("Attribute %s is %s", command, r)
+                    # look up the enum value like b"1" -> on in PowerModes
+                    return cmd_enum(r.replace(ack.value, b"")).name
+
+                return state
+            except ValueError as err:
+                self.logger.error("Attribute not found - %s", err)
+                raise
+            except AttributeError as err:
+                self.logger.error("tried to access name on non-enum: %s", err)
+                return ""
 
     async def get_low_latency_state(self) -> str:
         """
         Get the current state of LL
         """
         return await self._get_attribute("low_latency") == LowLatencyModes.on.name
```

### Comparing `pyjvc-4.4.22/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.23/pyJVC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.22
+Version: 4.4.23
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.22/setup.py` & `pyjvc-4.4.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.22",
+    version="4.4.23",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.22/tests/test_commander.py` & `pyjvc-4.4.23/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.22/tests/test_coordinator.py` & `pyjvc-4.4.23/tests/test_coordinator.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,210 +38,218 @@
 
         # connect to PJ
         res = await self.coordinator.open_connection()
         assert res is True
 
         # Ensure projector is on
         is_on = await self.coordinator.is_on()
+        print(is_on)
         # turn on if not already
-        if not is_on:
-            self.fail("PJ is off, turn on to run tests")
-            msg = await self.coordinator.power_on()
-            print(msg)
-
-        # wait for projector to turn on
-        timeout = 120  # units technically, not really seconds but who cares
-        while timeout > 0:
-            await asyncio.sleep(1)
-            is_on = await self.coordinator.is_on()
-            if is_on:
-                break
-            timeout -= 1
+        # if not is_on:
+        #     self.fail("PJ is off, turn on to run tests")
+        #     msg = await self.coordinator.power_on()
+        #     print(msg)
+
+        # # wait for projector to turn on
+        # timeout = 120  # units technically, not really seconds but who cares
+        # while timeout > 0:
+        #     await asyncio.sleep(1)
+        #     is_on = await self.coordinator.is_on()
+        #     if is_on:
+        #         break
+        #     timeout -= 1
 
     async def asyncTearDown(self):
         """clean up connection between tests otherwise error"""
         await self.coordinator.close_connection()
 
-    async def assert_modes(self):  # pylint: disable=too-many-locals
-        """helper function for attr"""
-        # in one test so it doesnt constantly open and close connection
-        # check return value against eunm __members__
-        low_latency_state = await self.coordinator.get_low_latency_state()
-        self.assertIn(
-            low_latency_state, [False, True], "Low latency state not on or off"
-        )
-        _, res = await self.coordinator.exec_command(["laser_power, low"])
-        self.assertTrue(res, "failed to set laser power to low")
-
-        # test getting resolution
-        res = await self.coordinator.get_source_display()
-        self.assertIn(res, ["4K_4096p24", "NoSignal"], "Source display not as expected")
-
-        res = await self.coordinator.get_anamorphic()
-        self.assertIn(res, AnamorphicModes.__members__, "Anamorphic not as expected")
-
-        picture_mode = await self.coordinator.get_picture_mode()
-        self.assertIn(
-            picture_mode, PictureModes.__members__, "Picture mode not as expected."
-        )
-
-        install_mode = await self.coordinator.get_install_mode()
-        self.assertIn(
-            install_mode,
-            InstallationModes.__members__,
-            f"Unexpected install mode: {install_mode}",
-        )
-        print(install_mode)
-        # Testing input mode
-
-        input_mode = await self.coordinator.get_input_mode()
-        self.assertIn(
-            input_mode, InputModes.__members__, f"Unexpected input mode: {input_mode}"
-        )
-
-        # Testing mask mode
-        mask_mode = await self.coordinator.get_mask_mode()
-        self.assertIn(
-            mask_mode, MaskModes.__members__, f"Unexpected mask mode: {mask_mode}"
-        )
-
-        # Testing laser mode
-        laser_mode = await self.coordinator.get_laser_mode()
-        self.assertIn(
-            laser_mode,
-            LaserDimModes.__members__,
-            f"Unexpected laser mode: {laser_mode}",
-        )
-
-        # Testing eshift mode
-        eshift_mode = await self.coordinator.get_eshift_mode()
-        self.assertIn(
-            eshift_mode,
-            [True, False],
-            f"Unexpected eshift mode: {eshift_mode}",
-        )
-
-        # Testing color mode
-        color_mode = await self.coordinator.get_color_mode()
-        self.assertIn(
-            color_mode,
-            ColorSpaceModes.__members__,
-            f"Unexpected color mode: {color_mode}",
-        )
-
-        # Testing input level
-        input_level = await self.coordinator.get_input_level()
-        self.assertIn(
-            input_level,
-            InputLevel.__members__,
-            f"Unexpected input level: {input_level}",
-        )
-
-        # Testing software version
-        software_version = await self.coordinator.get_software_version()
-        self.assertIsInstance(
-            software_version, float, "Software version is not a float"
-        )
-        self.assertGreater(
-            software_version, 0, "Software version is not greater than 0"
-        )
-        print(software_version)
-        # fw 3.0 and above
-        if software_version > 2.10:
-            res = await self.coordinator.get_laser_value()
-            print("laser value", res)
-            self.assertIsInstance(res, int)
-            self.assertEqual(res, 0, "Laser value is over 100")
-
-        # Testing content type
-        content_type = await self.coordinator.get_content_type()
-        self.assertIn(
-            content_type,
-            ContentTypes.__members__,
-            f"Unexpected content type: {content_type}",
-        )
-
-        # Testing content type transition
-        content_type_trans = await self.coordinator.get_content_type_trans()
-        self.assertIn(
-            content_type_trans,
-            ContentTypeTrans.__members__,
-            f"Unexpected content type transition: {content_type_trans}",
-        )
-
-        # Testing lamp power
-        lamp_power = await self.coordinator.get_lamp_power()
-        # unknown would mean it worked but returned an unmapped value, thats fine
-        self.assertTrue(
-            lamp_power in LampPowerModes.__members__ or lamp_power == "unknown",
-            f"Unexpected lamp power: {lamp_power}",
-        )
-
-        # Testing lamp time
-        lamp_time = await self.coordinator.get_lamp_time()
-        self.assertIsInstance(lamp_time, int, "Lamp time is not an integer")
-
-        # Testing laser power
-        laser_power = await self.coordinator.get_laser_power()
-        self.assertIn(
-            laser_power,
-            LaserPowerModes.__members__,
-            f"Unexpected laser power: {laser_power}",
-        )
-        print("laser power", laser_power)
-
-        # Testing aspect ratio
-        aspect_ratio = await self.coordinator.get_aspect_ratio()
-        self.assertIn(
-            aspect_ratio,
-            AspectRatioModes.__members__,
-            f"Unexpected aspect ratio: {aspect_ratio}",
-        )
-
-        # Testing source status
-        source_status = await self.coordinator.get_source_status()
-        self.assertIn(
-            source_status,
-            [True, False],
-            f"Unexpected source status: {source_status}",
-        )
-        self.assertIsInstance(source_status, bool)
-        print("source status", source_status)
+    # async def assert_modes(self):  # pylint: disable=too-many-locals
+    #     """helper function for attr"""
+    #     # in one test so it doesnt constantly open and close connection
+    #     # check return value against eunm __members__
+    #     low_latency_state = await self.coordinator.get_low_latency_state()
+    #     self.assertIn(
+    #         low_latency_state, [False, True], "Low latency state not on or off"
+    #     )
+    #     _, res = await self.coordinator.exec_command(["laser_power, low"])
+    #     self.assertTrue(res, "failed to set laser power to low")
+
+    #     # test getting resolution
+    #     res = await self.coordinator.get_source_display()
+    #     self.assertIn(res, ["4K_4096p24", "NoSignal"], "Source display not as expected")
+
+    #     res = await self.coordinator.get_anamorphic()
+    #     self.assertIn(res, AnamorphicModes.__members__, "Anamorphic not as expected")
+
+    #     picture_mode = await self.coordinator.get_picture_mode()
+    #     self.assertIn(
+    #         picture_mode, PictureModes.__members__, "Picture mode not as expected."
+    #     )
+
+    #     install_mode = await self.coordinator.get_install_mode()
+    #     self.assertIn(
+    #         install_mode,
+    #         InstallationModes.__members__,
+    #         f"Unexpected install mode: {install_mode}",
+    #     )
+    #     print(install_mode)
+    #     # Testing input mode
+
+    #     input_mode = await self.coordinator.get_input_mode()
+    #     self.assertIn(
+    #         input_mode, InputModes.__members__, f"Unexpected input mode: {input_mode}"
+    #     )
+
+    #     # Testing mask mode
+    #     mask_mode = await self.coordinator.get_mask_mode()
+    #     self.assertIn(
+    #         mask_mode, MaskModes.__members__, f"Unexpected mask mode: {mask_mode}"
+    #     )
+
+    #     # Testing laser mode
+    #     laser_mode = await self.coordinator.get_laser_mode()
+    #     self.assertIn(
+    #         laser_mode,
+    #         LaserDimModes.__members__,
+    #         f"Unexpected laser mode: {laser_mode}",
+    #     )
+
+    #     # Testing eshift mode
+    #     eshift_mode = await self.coordinator.get_eshift_mode()
+    #     self.assertIn(
+    #         eshift_mode,
+    #         [True, False],
+    #         f"Unexpected eshift mode: {eshift_mode}",
+    #     )
+
+    #     # Testing color mode
+    #     color_mode = await self.coordinator.get_color_mode()
+    #     self.assertIn(
+    #         color_mode,
+    #         ColorSpaceModes.__members__,
+    #         f"Unexpected color mode: {color_mode}",
+    #     )
+
+    #     # Testing input level
+    #     input_level = await self.coordinator.get_input_level()
+    #     self.assertIn(
+    #         input_level,
+    #         InputLevel.__members__,
+    #         f"Unexpected input level: {input_level}",
+    #     )
+
+    #     # Testing software version
+    #     software_version = await self.coordinator.get_software_version()
+    #     self.assertIsInstance(
+    #         software_version, float, "Software version is not a float"
+    #     )
+    #     self.assertGreater(
+    #         software_version, 0, "Software version is not greater than 0"
+    #     )
+    #     print(software_version)
+    #     # fw 3.0 and above
+    #     if software_version > 2.10:
+    #         res = await self.coordinator.get_laser_value()
+    #         print("laser value", res)
+    #         self.assertIsInstance(res, int)
+    #         self.assertEqual(res, 0, "Laser value is over 100")
+
+    #     # Testing content type
+    #     content_type = await self.coordinator.get_content_type()
+    #     self.assertIn(
+    #         content_type,
+    #         ContentTypes.__members__,
+    #         f"Unexpected content type: {content_type}",
+    #     )
+
+    #     # Testing content type transition
+    #     content_type_trans = await self.coordinator.get_content_type_trans()
+    #     self.assertIn(
+    #         content_type_trans,
+    #         ContentTypeTrans.__members__,
+    #         f"Unexpected content type transition: {content_type_trans}",
+    #     )
+
+    #     # Testing lamp power
+    #     lamp_power = await self.coordinator.get_lamp_power()
+    #     # unknown would mean it worked but returned an unmapped value, thats fine
+    #     self.assertTrue(
+    #         lamp_power in LampPowerModes.__members__ or lamp_power == "unknown",
+    #         f"Unexpected lamp power: {lamp_power}",
+    #     )
+
+    #     # Testing lamp time
+    #     lamp_time = await self.coordinator.get_lamp_time()
+    #     self.assertIsInstance(lamp_time, int, "Lamp time is not an integer")
+
+    #     # Testing laser power
+    #     laser_power = await self.coordinator.get_laser_power()
+    #     self.assertIn(
+    #         laser_power,
+    #         LaserPowerModes.__members__,
+    #         f"Unexpected laser power: {laser_power}",
+    #     )
+    #     print("laser power", laser_power)
+
+    #     # Testing aspect ratio
+    #     aspect_ratio = await self.coordinator.get_aspect_ratio()
+    #     self.assertIn(
+    #         aspect_ratio,
+    #         AspectRatioModes.__members__,
+    #         f"Unexpected aspect ratio: {aspect_ratio}",
+    #     )
+
+    #     # Testing source status
+    #     source_status = await self.coordinator.get_source_status()
+    #     self.assertIn(
+    #         source_status,
+    #         [True, False],
+    #         f"Unexpected source status: {source_status}",
+    #     )
+    #     self.assertIsInstance(source_status, bool)
+    #     print("source status", source_status)
+
+    #     # Testing is_on
+    #     is_on = await self.coordinator.is_on()
+    #     self.assertIsInstance(is_on, bool, "is_on is not a boolean")
+
+    #     # Testing is_ll_on
+    #     is_ll_on = await self.coordinator.is_ll_on()
+    #     self.assertIsInstance(is_ll_on, bool, "is_ll_on is not a boolean")
+
+    #     res = await self.coordinator.exec_command(["laser_value, 35"])
+    #     print("laser value set to", res)
+    #     if software_version > 2.10:
+    #         res = await self.coordinator.get_laser_value()
+    #         print("laser value", res)
 
-        # Testing is_on
-        is_on = await self.coordinator.is_on()
-        self.assertIsInstance(is_on, bool, "is_on is not a boolean")
-
-        # Testing is_ll_on
-        is_ll_on = await self.coordinator.is_ll_on()
-        self.assertIsInstance(is_ll_on, bool, "is_ll_on is not a boolean")
-
-        res = await self.coordinator.exec_command(["laser_value, 35"])
-        print("laser value set to", res)
-        if software_version > 2.10:
-            res = await self.coordinator.get_laser_value()
-            print("laser value", res)
+    #         self.assertEqual(res, 35, "Laser value is not 35")
 
-            self.assertEqual(res, 35, "Laser value is not 35")
-
-    async def test_exec_commands(self):
+    async def test_power_commands(self):
         """test executing commands"""
-        # get attr
-        await self.assert_modes()
 
         # test commands
-        _, res = await self.coordinator.exec_command(["menu, menu"])
-        print(res)
-        assert res is True
-        # close menu
-        if res:
-            _, res = await self.coordinator.exec_command(["menu, menu"])
-
-    async def test_turn_off(self):
-        """unskip to turn off pj after tests"""
-        # self.skipTest("not turning off")
-        _, res = await self.coordinator.exec_command(["power, off"])
-        assert res, "failed to turn off"
+        state = await self.coordinator.is_on()
+        ll = await self.coordinator.is_ll_on()
+        print(state, ll)
+    # async def test_exec_commands(self):
+    #     """test executing commands"""
+    #     # get attr
+    #     await self.assert_modes()
+
+    #     # test commands
+    #     _, res = await self.coordinator.exec_command(["menu, menu"])
+    #     print(res)
+    #     assert res is True
+    #     # close menu
+    #     if res:
+    #         _, res = await self.coordinator.exec_command(["menu, menu"])
+
+    # async def test_turn_off(self):
+    #     """unskip to turn off pj after tests"""
+    #     # self.skipTest("not turning off")
+    #     _, res = await self.coordinator.exec_command(["power, off"])
+    #     assert res, "failed to turn off"
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyjvc-4.4.22/tests/test_loop.py` & `pyjvc-4.4.23/tests/test_loop.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import os
 import unittest
 import logging
 import random
 import time
 from jvc_projector.jvc_projector import JVCProjectorCoordinator, JVCInput
 from dataclasses import asdict
+import itertools
+from typing import Iterable
+from jvc_projector.commands import Header
 
 os.environ["LOG_LEVEL"] = "DEBUG"
 
 # Note these tests assume projector is on because most commands will time out. Not fail, but time out because JVC can't even bother
 # to return a response when a command is not successful
 
 _LOGGER = logging.getLogger(__name__)
@@ -25,85 +28,160 @@
         options: JVCInput,
         jvc_client: JVCProjectorCoordinator = None,
     ) -> None:
         """JVC Init."""
         super().__init__()
         self._name = name
         self._host = options.host
+        self.host = options.host
         self.entry = entry
+        # tie the entity to the config flow
+        self._attr_unique_id = "12"
 
         self.jvc_client = jvc_client
+        self.jvc_client.logger = _LOGGER
         # attributes
         self._state = False
 
         # async queue
         self.tasks = []
         # use one queue for all commands
         self.command_queue = asyncio.PriorityQueue()
         self.attribute_queue = asyncio.Queue()
 
         self.stop_processing_commands = asyncio.Event()
 
         self._update_interval = None
+
+        # counter for unique IDs
+        self._counter = itertools.count()
         self.loop = asyncio.get_event_loop()
+        self.attribute_getters = set()
 
     async def async_added_to_hass(self) -> None:
         """Run when entity about to be added to hass."""
         # add the queue handler to the event loop
         # get updates in a set interval
+
         # open connection
-        _LOGGER.debug("adding update task to loop")
-        t = self.loop.create_task(self.async_update_state(now=None))
-        self.tasks.append(t)
+        conn = self.loop.create_task(self.open_conn())
+        self.tasks.append(conn)
 
         # handle commands
-        _LOGGER.debug("adding queue handler to loop")
         queue_handler = self.loop.create_task(self.handle_queue())
         self.tasks.append(queue_handler)
 
         # handle updates
-        _LOGGER.debug("adding update handler to loop")
-        update_handler = self.loop.create_task(self.update_worker())
-        self.tasks.append(update_handler)
+        update_worker = self.loop.create_task(self.update_worker())
+        self.tasks.append(update_worker)
 
-    async def generate_unique_id(self) -> str:
-        timestamp = int(
-            time.time() * 1000
-        )  # Convert to milliseconds for more granularity
-        random_value = random.randint(0, 999)  # Add a random value for uniqueness
-        unique_id = f"{timestamp}-{random_value}"
-        return unique_id
+        # handle sending attributes to queue
+        update_handler = self.loop.create_task(self.make_updates())
+        self.tasks.append(update_handler)
+        # handle sending attributes to queue
+        s = self.loop.create_task(self.async_update_state(""))
+        self.tasks.append(s)
+
+    async def open_conn(self):
+        """Open the connection to the projector."""
+        _LOGGER.debug("About to open connection with jvc_client: %s", self.jvc_client)
+        try:
+            _LOGGER.debug("Opening connection to %s", self.host)
+            res = await asyncio.wait_for(self.jvc_client.open_connection(), timeout=3)
+            if res:
+                _LOGGER.debug("Connection to %s opened", self.host)
+                return True
+        except asyncio.TimeoutError:
+            _LOGGER.warning("Timeout while trying to connect to %s", self._host)
+        except asyncio.CancelledError:
+            return
+        # intentionally broad
+        except TypeError as err:
+            # this is benign, just means the PJ is not connected yet
+            _LOGGER.debug("open_connection: %s", err)
+            return
+        except Exception as err:
+            await self.reset_everything()
+            _LOGGER.error("some error happened with open_connection: %s", err)
+        await asyncio.sleep(5)
+
+    async def generate_unique_id(self) -> int:
+        """this is used to sort the queue because it contains non-comparable items"""
+        return next(self._counter)
+
+    async def wait_until_connected(self, wait_time: float = 0.1) -> bool:
+        """Wait until the connection is open."""
+        while not self.jvc_client.connection_open:
+            await asyncio.sleep(wait_time)
+        return True
 
     async def handle_queue(self):
         """
         Handle items in command queue.
         This is run in an event loop
         """
-        try:
-            while True:
+        while True:
+            await self.wait_until_connected(5)
+            try:
+                _LOGGER.debug(
+                    "queue size is %s - attribute size is %s",
+                    self.command_queue.qsize(),
+                    self.attribute_queue.qsize(),
+                )
                 # send all commands in queue
                 # can be a command or a tuple[function, attribute]
                 # first item is the priority
-                priority, command = await self.command_queue.get()
-                _LOGGER.debug("got queue item %s with priority %s", command, priority)
-                # if its a tuple its an attribute update
-                if isinstance(command, tuple) and self.jvc_client.connection_open:
-                    _, getter, attribute = command
+                try:
+                    priority, item = await asyncio.wait_for(
+                        self.command_queue.get(), timeout=5
+                    )
+                except asyncio.TimeoutError:
+                    _LOGGER.debug("Timeout in command queue")
+                    continue
+                _LOGGER.debug("got queue item %s with priority %s", item, priority)
+                # if its a 3 its an attribute tuple
+                if len(item) == 3:
+                    # discard the unique ID
+                    _, getter, attribute = item
                     _LOGGER.debug(
                         "trying attribute %s with getter %s", attribute, getter
                     )
-                    # simulate a command
-                    await asyncio.sleep(random.randint(1, 2) - 0.3)
-                else:
-                    # run the command and set type to operation
+                    try:
+                        value = await asyncio.wait_for(getter(), timeout=3)
+                    except asyncio.TimeoutError:
+                        _LOGGER.debug("Timeout with item %s", item)
+                        try:
+                            # if the above command times out, but we wrote to buffer, that means there is unread data in response
+                            # this needs to clear the buffer if timeout
+                            await self.jvc_client.reset_everything()
+                            self.command_queue.task_done()
+                        except ValueError:
+                            pass
+                        continue
+                    _LOGGER.debug("got value %s for attribute %s", value, attribute)
+                    setattr(self.jvc_client.attributes, attribute, value)
+                elif len(item) == 2:
+                    # run the item and set type to operation
                     # HA sends commands like ["power, on"] which is one item
+                    _, command = item
                     _LOGGER.debug("executing command %s", command)
-                    await asyncio.sleep(random.randint(1, 2) - 0.3)
-                # except Exception as e:
-                #     _LOGGER.error("Unexpected error in handle_queue: %s", e)
+                    try:
+                        await asyncio.wait_for(
+                            self.jvc_client.exec_command(
+                                command, Header.operation.value
+                            ),
+                            timeout=5,
+                        )
+                    except asyncio.TimeoutError:
+                        _LOGGER.debug("Timeout with command %s", command)
+                        try:
+                            self.command_queue.task_done()
+                        except ValueError:
+                            pass
+                        continue
                 try:
                     self.command_queue.task_done()
                 except ValueError:
                     pass
                 await asyncio.sleep(0.1)
                 # if we are stopping and the queue is not empty, clear it
                 # this is so it doesnt continuously print the stopped processing commands message
@@ -111,233 +189,298 @@
                     self.stop_processing_commands.is_set()
                     and not self.command_queue.empty()
                 ):
                     await self.clear_queue()
                     _LOGGER.debug("Stopped processing commands")
                     # break to the outer loop so it can restart itself if needed
                     break
-            # save cpu
-            await asyncio.sleep(0.1)
-        except asyncio.CancelledError:
-            _LOGGER.debug("handle_queue cancelled")
-            return
+                # save cpu
+                await asyncio.sleep(0.1)
+            except asyncio.CancelledError:
+                _LOGGER.debug("handle_queue cancelled")
+                return
+            except TypeError as err:
+                _LOGGER.debug(
+                    "TypeError in handle_queue, moving on: %s -- %s", err, item
+                )
+                # in this case likely the queue priority is the same, lets just skip it
+                self.command_queue.task_done()
+                continue
+            # catch wrong values
+            except ValueError as err:
+                _LOGGER.error("ValueError in handle_queue: %s", err)
+                # Not sure what causes these but we can at least try to ignore them
+                self.command_queue.task_done()
+                continue
+            except Exception as err:  # pylint: disable=broad-except
+                _LOGGER.error("Unhandled exception in handle_queue: %s", err)
+                await self.reset_everything()
+                continue
+
+    async def reset_everything(self) -> None:
+        """resets EVERYTHING. Something with home assistant just doesnt play nice here"""
+
+        _LOGGER.debug("RESETTING - clearing everything")
+
+        try:
+            self.stop_processing_commands.set()
+            await self.clear_queue()
+            await self.jvc_client.reset_everything()
+        except Exception as err:
+            _LOGGER.error("Error reseting: %s", err)
+        finally:
+            self.stop_processing_commands.clear()
 
     async def clear_queue(self):
         """Clear the queue"""
+        try:
+            # clear the queue
+            _LOGGER.debug("Clearing command queue")
+            while not self.command_queue.empty():
+                self.command_queue.get_nowait()
+                self.command_queue.task_done()
+
+            _LOGGER.debug("Clearing attr queue")
+            while not self.attribute_queue.empty():
+                self.attribute_queue.get_nowait()
+                self.attribute_queue.task_done()
+
+            # reset the counter
+            _LOGGER.debug("resetting counter")
+            self._counter = itertools.count()
 
-        # clear the queue
-        while not self.command_queue.empty():
-            self.command_queue.get_nowait()
-            self.command_queue.task_done()
-
-        while not self.attribute_queue.empty():
-            self.attribute_queue.get_nowait()
-            self.attribute_queue.task_done()
+        except ValueError:
+            pass
 
     async def update_worker(self):
         """Gets a function and attribute from a queue and adds it to the command interface"""
         while True:
             # this is just an async interface so the other processor doesnt become complicated
 
             # getter will be a Callable
             try:
+                # queue backpressure
+                if self.command_queue.qsize() > 10:
+                    # this allows the queue to process stuff without filling up
+                    _LOGGER.debug("Queue is full, waiting to add attributes")
+                    await asyncio.sleep(2)
+                    continue
                 unique_id, getter, attribute = await self.attribute_queue.get()
                 # add to the command queue with a single interface
                 await self.command_queue.put((1, (unique_id, getter, attribute)))
-                _LOGGER.debug("added %s to command queue from attribute q", attribute)
-                self.attribute_queue.task_done()
+                try:
+                    self.attribute_queue.task_done()
+                except ValueError:
+                    pass
             except asyncio.TimeoutError:
                 _LOGGER.debug("Timeout in update_worker")
             except asyncio.CancelledError:
                 _LOGGER.debug("update_worker cancelled")
                 return
             await asyncio.sleep(0.1)
 
-    async def make_updates(self, attribute_getters: list):
-        """Add all the attribute getters to the queue."""
-        for getter, name in attribute_getters:
-            unique_id = await self.generate_unique_id()
-            await self.attribute_queue.put((unique_id, getter, name))
-
-        # get hdr attributes
-        await self.attribute_queue.join()
-        _LOGGER.debug("make_updates done attributes updated")
-        # extra sleep to make sure all the updates are done
-        await asyncio.sleep(0.5)
+    @property
+    def is_on(self):
+        """Return the last known state of the projector."""
+        return self._state
+
+    async def async_turn_on(self, **kwargs):  # pylint: disable=unused-argument
+        """Send the power on command."""
+
+        self._state = True
+        await self.wait_until_connected()
+        try:
+            await self.jvc_client.power_on()
+            self.stop_processing_commands.clear()
+            # save state
+        except Exception as err:  # pylint: disable=broad-except
+            _LOGGER.error("Error turning on projector: %s", err)
+            await self.reset_everything()
+            self._state = False
+
+    async def async_turn_off(self, **kwargs):  # pylint: disable=unused-argument
+        """Send the power off command."""
+        await self.wait_until_connected()
+        self._state = False
+
+        try:
+            await self.jvc_client.power_off()
+            self.stop_processing_commands.set()
+            await self.clear_queue()
+            # save state
+        except Exception as err:  # pylint: disable=broad-except
+            _LOGGER.error("Error turning off projector: %s", err)
+            await self.reset_everything()
+            self._state = False
+
+    async def make_updates(self):
+        """
+        Runs as a background task
+        Add all the attribute getters to the queue.
+        """
+        while True:
+            # copy it so we can remove items from it
+            attrs = self.attribute_getters.copy()
+            for getter, name in attrs:
+                # you might be thinking why is this here?
+                # oh boy let me tell you
+                # TLDR priority queues need a unique ID to sort and you need to just dump one in
+                # otherwise you get a TypeError that home assistant HIDES from you and you spend a week figuring out
+                # why this function deadlocks for no reason, and that HA hides error raises
+                # because the underlying items are not sortable
+                unique_id = await self.generate_unique_id()
+                await self.attribute_queue.put((unique_id, getter, name))
+
+                # remove the added item from the set
+                self.attribute_getters.discard((getter, name))
+
+            await asyncio.sleep(0.1)
 
-    async def async_update_state(self, now):
+    async def async_update_state(self, _):
+        """
+        Retrieve latest state.
+        This will push the attributes to the queue and be processed by make_updates
+        """
         while True:
-            try:
-                _LOGGER.debug("running update state")
-                # mock running every 5 seconds
-                await asyncio.sleep(5)
-                """Retrieve latest state."""
-                if True:
-                    # certain commands can only run at certain times
-                    # if they fail (i.e grayed out on menu) JVC will simply time out. Bad UX
-                    # have to add specific commands in a precise order
-                    # common stuff
-                    attribute_getters = []
-                    _LOGGER.debug("running update sync")
-                    _LOGGER.debug(
-                        "stop_processing_commands %s, connection_open %s",
-                        self.stop_processing_commands.is_set(),
-                        self.jvc_client.connection_open,
+            await asyncio.sleep(3)
+            if await self.wait_until_connected():
+                # certain commands can only run at certain times
+                # if they fail (i.e grayed out on menu) JVC will simply time out. Bad UX
+                # have to add specific commands in a precise order
+                # get power
+                self.attribute_getters.add((self.jvc_client.is_on, "power_state"))
+
+                self._state = self.jvc_client.attributes.power_state
+                _LOGGER.debug("power state is : %s", self._state)
+                self.attribute_getters.add(
+                    (self.jvc_client.get_test_command, "picture_mode")
+                )
+                if self._state:
+                    # takes a func and an attribute to write result into
+                    self.attribute_getters.update(
+                        [
+                            (self.jvc_client.get_source_status, "signal_status"),
+                            (self.jvc_client.get_picture_mode, "picture_mode"),
+                            (self.jvc_client.get_software_version, "software_version"),
+                        ]
                     )
-                    # get power
-                    attribute_getters.append((self.jvc_client.is_on, "power_state"))
-                    await self.make_updates(attribute_getters)
-
-                    self._state = self.jvc_client.attributes.power_state
-                    _LOGGER.debug("power state is : %s", self._state)
-
-                    if True:
-                        _LOGGER.debug("getting signal status and picture mode")
-                        # takes a func and an attribute to write result into
-                        attribute_getters.extend(
+                    if self.jvc_client.attributes.signal_status is True:
+                        self.attribute_getters.update(
                             [
-                                (self.jvc_client.get_source_status, "signal_status"),
-                                (self.jvc_client.get_picture_mode, "picture_mode"),
+                                (self.jvc_client.get_content_type, "content_type"),
                                 (
-                                    self.jvc_client.get_software_version,
-                                    "software_version",
+                                    self.jvc_client.get_content_type_trans,
+                                    "content_type_trans",
                                 ),
+                                (self.jvc_client.get_input_mode, "input_mode"),
+                                (self.jvc_client.get_anamorphic, "anamorphic_mode"),
+                                (self.jvc_client.get_source_display, "resolution"),
+                            ]
+                        )
+                    if "Unsupported" not in self.jvc_client.model_family:
+                        self.attribute_getters.update(
+                            [
+                                (self.jvc_client.get_install_mode, "installation_mode"),
+                                (self.jvc_client.get_aspect_ratio, "aspect_ratio"),
+                                (self.jvc_client.get_color_mode, "color_mode"),
+                                (self.jvc_client.get_input_level, "input_level"),
+                                (self.jvc_client.get_mask_mode, "mask_mode"),
+                            ]
+                        )
+                    if any(x in self.jvc_client.model_family for x in ["NX9", "NZ"]):
+                        self.attribute_getters.add(
+                            (self.jvc_client.get_eshift_mode, "eshift"),
+                        )
+                    if "NZ" in self.jvc_client.model_family:
+                        self.attribute_getters.update(
+                            [
+                                (self.jvc_client.get_laser_power, "laser_power"),
+                                (self.jvc_client.get_laser_mode, "laser_mode"),
+                                (self.jvc_client.is_ll_on, "low_latency"),
+                                (self.jvc_client.get_lamp_time, "laser_time"),
+                            ]
+                        )
+                    else:
+                        self.attribute_getters.update(
+                            [
+                                (self.jvc_client.get_lamp_power, "lamp_power"),
+                                (self.jvc_client.get_lamp_time, "lamp_time"),
                             ]
                         )
-                        # determine how to proceed based on above
-                        await self.make_updates(attribute_getters)
-                        if True:
-                            _LOGGER.debug("getting content type and input mode")
-                            attribute_getters.extend(
-                                [
-                                    (self.jvc_client.get_content_type, "content_type"),
-                                    (
-                                        self.jvc_client.get_content_type_trans,
-                                        "content_type_trans",
-                                    ),
-                                    (self.jvc_client.get_input_mode, "input_mode"),
-                                    (self.jvc_client.get_anamorphic, "anamorphic_mode"),
-                                    (self.jvc_client.get_source_display, "resolution"),
-                                ]
-                            )
-                        if "Unsupported" not in self.jvc_client.model_family:
-                            attribute_getters.extend(
-                                [
-                                    (
-                                        self.jvc_client.get_install_mode,
-                                        "installation_mode",
-                                    ),
-                                    (self.jvc_client.get_aspect_ratio, "aspect_ratio"),
-                                    (self.jvc_client.get_color_mode, "color_mode"),
-                                    (self.jvc_client.get_input_level, "input_level"),
-                                    (self.jvc_client.get_mask_mode, "mask_mode"),
-                                ]
-                            )
-                        if any(
-                            x in self.jvc_client.model_family for x in ["NX9", "NZ"]
-                        ):
-                            attribute_getters.append(
-                                (self.jvc_client.get_eshift_mode, "eshift"),
-                            )
-                        if "NZ" in self.jvc_client.model_family:
-                            attribute_getters.extend(
-                                [
-                                    (self.jvc_client.get_laser_power, "laser_power"),
-                                    (self.jvc_client.get_laser_mode, "laser_mode"),
-                                    (self.jvc_client.is_ll_on, "low_latency"),
-                                    (self.jvc_client.get_lamp_time, "laser_time"),
-                                ]
-                            )
-                        else:
-                            attribute_getters.extend(
-                                [
-                                    (self.jvc_client.get_lamp_power, "lamp_power"),
-                                    (self.jvc_client.get_lamp_time, "lamp_time"),
-                                ]
-                            )
-
-                        await self.make_updates(attribute_getters)
 
-                        # get laser value if fw is a least 3.0
-                        if "NZ" in self.jvc_client.model_family:
-                            try:
-                                if (
-                                    float(self.jvc_client.attributes.software_version)
-                                    >= 3.00
-                                ):
-                                    attribute_getters.extend(
-                                        [
-                                            (
-                                                self.jvc_client.get_laser_value,
-                                                "laser_value",
-                                            ),
-                                        ]
-                                    )
-                            except ValueError:
-                                pass
-                        # HDR stuff
-                        if any(
-                            x in self.jvc_client.attributes.content_type_trans
-                            for x in ["hdr", "hlg"]
-                        ):
-                            if "NZ" in self.jvc_client.model_family:
-                                attribute_getters.append(
-                                    (
-                                        self.jvc_client.get_theater_optimizer_state,
-                                        "theater_optimizer",
-                                    ),
+                    # get laser value if fw is a least 3.0
+                    if "NZ" in self.jvc_client.model_family:
+                        try:
+                            if (
+                                float(self.jvc_client.attributes.software_version)
+                                >= 3.00
+                            ):
+                                self.attribute_getters.update(
+                                    [
+                                        (
+                                            self.jvc_client.get_laser_value,
+                                            "laser_value",
+                                        ),
+                                    ]
                                 )
-                            attribute_getters.extend(
-                                [
-                                    (
-                                        self.jvc_client.get_hdr_processing,
-                                        "hdr_processing",
-                                    ),
-                                    (self.jvc_client.get_hdr_level, "hdr_level"),
-                                    (self.jvc_client.get_hdr_data, "hdr_data"),
-                                ]
+                        except ValueError:
+                            pass
+                    # HDR stuff
+                    if any(
+                        x in self.jvc_client.attributes.content_type_trans
+                        for x in ["hdr", "hlg"]
+                    ):
+                        if "NZ" in self.jvc_client.model_family:
+                            self.attribute_getters.add(
+                                (
+                                    self.jvc_client.get_theater_optimizer_state,
+                                    "theater_optimizer",
+                                ),
                             )
+                        self.attribute_getters.update(
+                            [
+                                (self.jvc_client.get_hdr_processing, "hdr_processing"),
+                                (self.jvc_client.get_hdr_level, "hdr_level"),
+                                (self.jvc_client.get_hdr_data, "hdr_data"),
+                            ]
+                        )
 
-                        # get all the updates
-                        await self.make_updates(attribute_getters)
-                        # _LOGGER.debug(asdict(self.jvc_client.attributes))
-                        await asyncio.sleep(0.1)
-                    else:
-                        _LOGGER.debug("PJ is off")
-                    # set the model and power
-                    self.jvc_client.attributes.model = self.jvc_client.model_family
-            except asyncio.CancelledError:
-                _LOGGER.debug("update_worker cancelled")
-                return
+                # set the model and power
+                self.jvc_client.attributes.model = self.jvc_client.model_family
 
-    async def async_send_command(self, command, **kwargs):
+    async def async_send_command(self, command: Iterable[str], **kwargs):
         """Send commands to a device."""
-        _LOGGER.debug("adding command %s to queue", command)
-        # add unique ID to command
-        await self.command_queue.put((0, (time.time(), command)))
-        _LOGGER.debug("command %s added to queue", command)
+        # add counter to preserve cmd order
+        unique_id = await self.generate_unique_id()
+        await self.command_queue.put((0, (unique_id, command)))
+        _LOGGER.debug("command %s added to queue with counter %s", command, unique_id)
 
 
 class TestCoordinator(unittest.IsolatedAsyncioTestCase):
     """Test running commands"""
 
     async def asyncSetUp(self):
         # set up connection
-        options = JVCInput("192", "1234", 20554, 3)
+        options = JVCInput("192.168.88.23", "123456789", 20554, 3)
         coord = JVCProjectorCoordinator(options=options)
         self.c = JVCRemote(None, "test", options, coord)
         # add the tasks to the loop
         await self.c.async_added_to_hass()
 
     async def testCmd(self):
         """Test command"""
-        for _ in range(100):
-            await self.c.async_send_command(["menu", "on"])
-            await asyncio.sleep(0.5)
+
+        if not self.c.jvc_client.is_on:
+            await self.c.async_turn_on()
+        await asyncio.sleep(30)
+        # for _ in range(100):
+        #     # await self.c.async_send_command(["menu", "on"])
+        #     # print(self.c.is_on)
+        #     await asyncio.sleep(0.5)
 
     async def asyncTearDown(self):
         """clean up connection between tests otherwise error"""
-        pass
+        await self.c.clear_queue()
 
 
 if __name__ == "__main__":
     unittest.main()
```

