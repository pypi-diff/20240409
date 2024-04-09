# Comparing `tmp/py2saber-0.12.1.tar.gz` & `tmp/py2saber-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.12.1.tar", last modified: Thu Mar 21 01:46:35 2024, max compression
+gzip compressed data, was "py2saber-0.12.2.tar", last modified: Tue Apr  9 01:21:08 2024, max compression
```

## Comparing `py2saber-0.12.1.tar` & `py2saber-0.12.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-03-21 01:46:35.020526 py2saber-0.12.1/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.12.1/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-03-21 01:46:35.020371 py2saber-0.12.1/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.12.1/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-03-21 01:46:35.020197 py2saber-0.12.1/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-03-21 01:46:35.000000 py2saber-0.12.1/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    25991 2024-03-21 01:03:57.000000 py2saber-0.12.1/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-03-21 01:45:26.000000 py2saber-0.12.1/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-03-21 01:46:35.020558 py2saber-0.12.1/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-04-09 01:21:08.048859 py2saber-0.12.2/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.12.2/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-04-09 01:21:08.048700 py2saber-0.12.2/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.12.2/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-04-09 01:21:08.048497 py2saber-0.12.2/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    26727 2024-04-08 21:02:56.000000 py2saber-0.12.2/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-03-22 23:21:26.000000 py2saber-0.12.2/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-04-09 01:21:08.048895 py2saber-0.12.2/setup.cfg
```

### Comparing `py2saber-0.12.1/COPYING` & `py2saber-0.12.2/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.12.1/PKG-INFO` & `py2saber-0.12.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.12.1
+Version: 0.12.2
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.12.1/README.md` & `py2saber-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.12.1/py2saber.egg-info/PKG-INFO` & `py2saber-0.12.2/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.12.1
+Version: 0.12.2
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.12.1/py2saber.py` & `py2saber-0.12.2/py2saber.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,35 +22,40 @@
 import sys
 import argparse
 import errno
 from getch import pause_exit
 import glob
 import time
 
-script_version = '0.12.1b'
+script_version = '0.12.2b'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
-
+# adapted from https://stackoverflow.com/a/66491013
+class DocDefaultException(Exception):
+    """Subclass exceptions use docstring as default message"""
+    def __init__(self, msg=None, detail="", *args, **kwargs):
+        super().__init__(msg or self.__doc__, *args, **kwargs)
+        self.detail = detail
 
 # Custom Exceptions
-class NoAnimaSaberException(Exception):
-    pass
+class NoAnimaSaberException(DocDefaultException):
+    '''No compatible Anima found. If an Anima is connected, try restarting it with the on/off switch. If the problem persists, try a different USB cable.'''
 
-class AnimaNotReadyException(Exception):
-    pass
+class AnimaNotReadyException(DocDefaultException):
+    '''Anima is not ready to receive commands. Try restarting the Anima using the on/off switch.'''
 
-class NotEnoughFreeSpaceException(Exception):
-    pass
+class NotEnoughFreeSpaceException(DocDefaultException):
+    '''Not enough free space on Anima to write the requested file(s).'''
 
-class AnimaFileWriteException(Exception):
-    pass
+class AnimaFileWriteException(DocDefaultException):
+    '''Error writing file(s) to Anima. Files are possibly corrupt. You should erase all files and re-upload.'''
 
-class InvalidSaberResponseException(Exception):
-    pass
+class InvalidSaberResponseException(DocDefaultException):
+    '''Received invalid response from saber.'''
 
 class Saber_Controller:
     '''Controls communication with an OpenCore-based lightsaber.'''
     # Serial port communication settings
     _SERIAL_SETTINGS = {'baudrate': 115200, 
                         'bytesize': 8, 
                         'parity': 'N', 
@@ -84,15 +89,14 @@
             ports = Saber_Controller.get_ports()
             for p in ports:
                 if Saber_Controller.port_is_anima(p):
                     self.port = p
                     break
 
         if not self.port:
-            self.log.error('No OpenCore sabers found.')
             raise NoAnimaSaberException
         
         # Initialize the serial connection
         self._ser = serial.Serial(self.port)
         self._ser.apply_settings(self._SERIAL_SETTINGS)
 
     def __del__(self):
@@ -123,14 +127,19 @@
         elif system == 'Linux':
             match_string = r'^/dev/ttyS*'
         else: # You're on your own!
             match_string = r'*'
         
         for port in port_list:
             if re.match(match_string, port.device):
+                # on macOS (Darwin), serial module returns /dev/cu.usbmodem*, but we should really use the corresponding /dev/tty.usbmodem*
+                if system == 'Darwin':
+                    serial_ports.append(re.sub('cu.', 'tty.', port.device))
+                else:
+                    serial_ports.append(port.device)
                 serial_ports.append(port.device)
         
         _log.info(f'Found {len(serial_ports)} port(s).')
         _log.debug(f'Found ports: {serial_ports}')
         return serial_ports
 
     @staticmethod
@@ -142,23 +151,23 @@
 
         try:
             log = logging.getLogger('Saber_Controller')
 
             log.info(f'Checking if decvice on port {port} is a Polaris Anima EVO.')
             ser = serial.Serial(port)
             ser.apply_settings({'baudrate': 115200, 
-                           'bytesize': 8, 
-                           'parity': 'N', 
-                           'stopbits': 1, 
-                           'xonxoff': False, 
-                           'dsrdtr': False, 
-                           'rtscts': False, 
-                           'timeout': 3, 
-                           'write_timeout': None, 
-                           'inter_byte_timeout': None})
+                                'bytesize': 8, 
+                                'parity': 'N', 
+                                'stopbits': 1, 
+                                'xonxoff': False, 
+                                'dsrdtr': False, 
+                                'rtscts': False, 
+                                'timeout': 3, 
+                                'write_timeout': None, 
+                                'inter_byte_timeout': None})
             
             # Checking logic (based on Nuntis' script):
             # Send 'V?'. Return false if no response or respond with a 1.x version. Otherwise continue.
             # Send 'S?'. Return false if no response or response doesn't start with 'S='. Otherwise continue.
             # Send 'WR?'. Return false if empty or response doesn't sart with 'OK, Write'.
             # Otherwise return true.
             log.debug('Sending command: V?')
@@ -351,31 +360,30 @@
         # slice off first and last char ('2' and '3')
         return config.decode().strip()[1:-1]
 
     def write_files_to_saber(self, files: list[str], progress_callback: callable = None) -> None:
         '''Write file(s) to saber. Expects a list of file names.
 
         NB: This method does no checking that files exist either on disk or saber. Please verify files before calling this method.'''
-        
-        if self.saber_is_ready():
-            files.sort()
-            self.log.info(f'Preparing to write file(s) to saber: {files}')
-            for file in files:
-                self.log.info(f'Writing file to saber: {file}')
-                
-                # Check for enough free space
-                file_size = os.path.getsize(file)
-                self.log.debug(f'File size: {file_size}')
-                free_space = self.get_free_space()
-                if free_space < file_size:
-                    self.log.error(f'Not enough free space on saber for file {file}')
-                    raise NotEnoughFreeSpaceException
-
-                # Write the file
-                with open(file, mode='rb') as binary_file:
+        files.sort()
+        self.log.info(f'Preparing to write file(s) to saber: {files}')
+        for file in files:
+            self.log.info(f'Writing file to saber: {file}')
+            
+            # Check for enough free space
+            file_size = os.path.getsize(file)
+            self.log.debug(f'File size: {file_size}')
+            free_space = self.get_free_space()
+            if free_space < file_size:
+                self.log.error(f'Not enough free space on saber for file {file}')
+                raise NotEnoughFreeSpaceException
+
+            # Write the file
+            with open(file, mode='rb') as binary_file:
+                if self.saber_is_ready():
                     bytes_sent = 0
                     fname = os.path.basename(file)
                     report_every_n_bytes = 512 # How often to update the bytes sent display
                     system = platform.system()
 
                     cmd = b'WR=' + fname.encode('utf-8') + b', ' + str(file_size).encode('utf-8') + b'\n'
                     self.send_command(cmd)
@@ -390,24 +398,24 @@
                         bytes_sent += 1
                         byte = binary_file.read(1)
                         if bytes_sent % report_every_n_bytes == 0:
                             print(f'\r{fname} - Bytes sent: {bytes_sent} - Bytes remaining: {file_size - bytes_sent}', end='', flush=True)
                             if self.gui:
                                 progress_callback.emit(bytes_sent)
                     print(f'\r{fname} - Bytes sent: {bytes_sent} - Bytes remaining: {file_size - bytes_sent}     ')
-                
-                response = self.read_line()
-                if not response == b'OK, Write Complete\n':
-                    self.log.error(f'Error writing file to saber. Error message: {response}')
-                    raise AnimaFileWriteException
+                else:
+                    raise AnimaNotReadyException
             
-                self.log.info(f'Successfully wrote file to saber: {file}')
-                time.sleep(1)
-        else:
-            raise AnimaNotReadyException
+            response = self.read_line()
+            if not response == b'OK, Write Complete\n':
+                self.log.error(f'Error writing file to saber. Error message: {response}')
+                raise AnimaFileWriteException
+        
+            self.log.info(f'Successfully wrote file to saber: {file}')
+            time.sleep(1)
 
     @staticmethod
     def rgbw_to_byte_str(r: int, g: int, b:int, w: int):
         return bytes(str(r), 'ascii') + b',' + bytes(str(g), 'ascii') + b',' + bytes(str(b), 'ascii') + b','+ bytes(str(w), 'ascii')
 
     def preview_color(self, r: int, g: int, b: int, w: int):
         cmd = b'P=' + self.rgbw_to_byte_str(r, g, b, w) + b'\n'
@@ -449,21 +457,25 @@
             self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
             raise InvalidSaberResponseException
     
 # ---------------------------------------------------------------------- #
 # Command Line Operations                                                #
 # ---------------------------------------------------------------------- #
 
+def error_handler(e: DocDefaultException):
+    '''Print an exception to the log, with details if provided in Exception'''
+    log = logging.getLogger()
+    log.debug(e, exc_info=True)
+    if e.detail:
+        log.error(str(e) + '\nDetails: ' + e.detail)
+    else:
+        log.error(e)
+
 def main_func():
     log = logging.getLogger()
-    if not log.hasHandlers():
-        log.setLevel(logging.ERROR)
-        stream = logging.StreamHandler(sys.stdout)
-        stream.setFormatter(logging.Formatter('%(levelname)s: %(message)s'))
-        log.addHandler(stream)
 
     exit_code = 0
 
     # configure command line parser and options
     parser = argparse.ArgumentParser(prog='py2saber',
                                      description='A utility for working with OpenCore-based sabers, based on "sendtosaber" by Nuntis')
     parser.add_argument('-v', '--version',
@@ -571,23 +583,16 @@
             try:
                 sc.write_files_to_saber(verified_files)
                 print(f'\nSuccessfully wrote file{"s" if len(verified_files)>1 else ""} to saber: {verified_files}')
             except AnimaFileWriteException:
                 log.error('Error writing to saber. You should erase your saber and re-upload all files to avoid corrupted files.')
                 exit_code = 1
 
-    except NoAnimaSaberException as e:
-        log.error('No OpenCore saber found. If the saber is connected, try restarting it with the on/off switch. If the problem persists, try a different USB cable.')
-        exit_code = 1
-
-    except AnimaNotReadyException:
-        log.error('Saber is not ready to receive commands. Try restarting the saber using the on/off switch.')
-
     except Exception as e:
-        log.error(e)
+        error_handler(e)
         exit_code = 1
     
     finally:
         if args.wait:
             pause_exit(exit_code, '\nPress any key to exit.')
         else:
             sys.exit(exit_code)
```

### Comparing `py2saber-0.12.1/pyproject.toml` & `py2saber-0.12.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.12.1"
+version = "0.12.2"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

