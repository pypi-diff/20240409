# Comparing `tmp/gif-steganography-0.0.1.tar.gz` & `tmp/gif-steganography-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif-steganography-0.0.1.tar", last modified: Sun Apr  7 12:54:24 2024, max compression
+gzip compressed data, was "gif-steganography-0.1.0.tar", last modified: Tue Apr  9 10:58:04 2024, max compression
```

## Comparing `gif-steganography-0.0.1.tar` & `gif-steganography-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1060 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/LICENSE
--rw-r--r--   0        0        0     2137 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/README.md
--rw-r--r--   0        0        0      628 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/__init__.py
--rw-r--r--   0        0        0     2764 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/cli.py
--rw-r--r--   0        0        0     1545 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/common.py
--rw-r--r--   0        0        0     3522 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/decode.py
--rw-r--r--   0        0        0     2705 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/encode.py
--rw-r--r--   0        0        0        0 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/lib/__init__.py
--rw-r--r--   0        0        0      190 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/lib/_compression.py
--rw-r--r--   0        0        0      482 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/lib/_ecc.py
--rw-r--r--   0        0        0     1215 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/lib/_encryption.py
--rw-r--r--   0        0        0     1276 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/lib/_gif.py
--rw-r--r--   0        0        0        0 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/modes/__init__.py
--rw-r--r--   0        0        0     1321 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/src/gif_steganography/modes/_lsb.py
--rw-r--r--   0        0        0        0 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0   199070 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/tests/data/input.gif
--rw-r--r--   0        0        0      903 2024-04-07 12:54:12.893238 gif-steganography-0.0.1/tests/test_integration.py
--rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 gif-steganography-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2865 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/README.md
+-rw-r--r--   0        0        0      628 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      161 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/__init__.py
+-rw-r--r--   0        0        0     2764 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/cli.py
+-rw-r--r--   0        0        0     1545 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/common.py
+-rw-r--r--   0        0        0     4197 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/decode.py
+-rw-r--r--   0        0        0     3383 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/encode.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/lib/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/lib/_compression.py
+-rw-r--r--   0        0        0      482 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/lib/_ecc.py
+-rw-r--r--   0        0        0     1215 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/lib/_encryption.py
+-rw-r--r--   0        0        0     1276 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/lib/_gif.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/modes/__init__.py
+-rw-r--r--   0        0        0     8070 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/modes/_cshift.py
+-rw-r--r--   0        0        0     1321 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/src/gif_steganography/modes/_lsb.py
+-rw-r--r--   0        0        0        0 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0   485470 2024-04-09 10:58:00.265508 gif-steganography-0.1.0/tests/data/input/dark.gif
+-rw-r--r--   0        0        0   199070 2024-04-09 10:58:00.269508 gif-steganography-0.1.0/tests/data/input/small.gif
+-rw-r--r--   0        0        0     1119 2024-04-09 10:58:00.269508 gif-steganography-0.1.0/tests/test_cshift.py
+-rw-r--r--   0        0        0     1116 2024-04-09 10:58:00.269508 gif-steganography-0.1.0/tests/test_lsb.py
+-rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 gif-steganography-0.1.0/PKG-INFO
```

### Comparing `gif-steganography-0.0.1/LICENSE` & `gif-steganography-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/README.md` & `gif-steganography-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # GIF Steganography
 
+[![Tests](https://github.com/nebmit/gif-steganography/actions/workflows/python-package.yml/badge.svg)](https://github.com/nebmit/gif-steganography/actions/workflows/python-package.yml)
+[![PyPI version](https://badge.fury.io/py/gif-steganography.svg)](https://badge.fury.io/py/gif-steganography)
+[![Dependencies](https://img.shields.io/librariesio/release/pypi/gif-steganography)](https://libraries.io/pypi/gif-steganography)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Python version](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+
 ## Overview
 
-This project implements GIF steganography using the Least Significant Bit (LSB) technique, coupled with additional layers of security and integrity verification. It enables the encoding of secret messages into GIF images and the decoding of these messages from the images, ensuring the message's secrecy and integrity through encryption, compression, and error correction.
+This project implements GIF steganography using various techniques, coupled with additional layers of security and integrity verification. It enables the encoding of secret messages into GIF images and the decoding of these messages from the images, ensuring the message's secrecy and integrity through encryption, compression, and error correction.
 
 ## Installation
 
 ```bash
 pip install gif-steganography
 ```
-Requires Python 3.10^. Installs the package and all necessary dependencies.
+Requires Python >= 3.10. Installs the package and all necessary dependencies.
 
 ## Usage
 
-### CLI
-
 #### Encode a Message
 
 ```bash
 gif-steganography encode <input.gif> <output.gif> "Secret Message" "Passphrase" [--nsym 10]
 ```
 - `--nsym` (optional): Sets the Reed-Solomon error correction level. Default is 10.
 
@@ -34,33 +38,33 @@
 Beyond the command-line interface, `gif-steganography` also provides direct API access for integrating steganographic functionalities into Python scripts.
 
 #### Basic Encoding and Decoding
 
 Embed and retrieve messages programmatically:
 
 ```python
-from gif_steganography import encode, decode
+from gif_steganography import SteganographyMethod, decode, encode
 
 # Embed a message
-encode("input.gif", "output.gif", "Hello, world!")
+encode("input.gif", "output.gif", "Hello, world!", mode=SteganographyMethod.LSB)
 
 # Retrieve a message
 message, _ = decode("output.gif")
 print(message)  # Output: Hello, world!
 ```
 
 #### Secure Encoding and Decoding
 
 For added security, use encryption with your messages:
 
 ```python
-from gif_steganography import encode, decode
+from gif_steganography import SteganographyMethod, decode, encode
 
 # Securely embed a message
-encode("input.gif", "output.gif", "Hello, world!", passphrase="password")
+encode("input.gif", "output.gif", "Hello, world!", passphrase="password", mode=SteganographyMethod.CSHIFT)
 
 # Securely retrieve a message
 message, _ = decode("output.gif", passphrase="password")
 print(message)  # Output: Hello, world!
 ```
 
 ## Project Structure
```

### Comparing `gif-steganography-0.0.1/pyproject.toml` & `gif-steganography-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gif-steganography"
-version = "0.0.1"
+version = "0.1.0"
 description = "A Python GIF steganography library supporting encryption to embed and extract secure messages within GIF images."
 authors = [
     { name = "nebmit", email = "76664673+nebmit@users.noreply.github.com" },
 ]
 dependencies = [
     "Pillow==10.3.0",
     "reedsolo==1.7.0",
```

### Comparing `gif-steganography-0.0.1/src/gif_steganography/cli.py` & `gif-steganography-0.1.0/src/gif_steganography/cli.py`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/src/gif_steganography/common.py` & `gif-steganography-0.1.0/src/gif_steganography/common.py`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/src/gif_steganography/decode.py` & `gif-steganography-0.1.0/src/gif_steganography/decode.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from cryptography.fernet import InvalidToken
 from reedsolo import ReedSolomonError
 
 from .common import CorruptDataError, InvalidPassphraseError, SteganographyMethod
 from .lib._compression import _decompress
 from .lib._ecc import _rs_decode_from_binary
 from .lib._encryption import _decrypt_message
-from .lib._gif import _read_frames_as_rgb
+from .lib._gif import _read_frames_as_p, _read_frames_as_rgb
+from .modes._cshift import _extract_data_from_frame_cshift
 from .modes._lsb import _extract_data_from_frame_lsb
 
 
 def decode(
     input_filename: str,
     mode: SteganographyMethod = SteganographyMethod.LSB,
     nsym: int = 10,
@@ -31,25 +32,41 @@
     Raises:
         CorruptDataError: If the message is corrupted.
         InvalidPassphraseError: If the passphrase is incorrect.
 
     Returns:
         Tuple[str, bool]: A tuple containing the decoded message and a boolean indicating if the message is corrupt.
     """
-    frames = _read_frames_as_rgb(input_filename)
-
+    binary_data_list: List[str] = []
     messages: List[bytes] = []
     is_corrupt: bool = False
 
-    for frame in frames:
-        # Extract the binary data from the frame
-        binary_data: str = _extract_data_from_frame_lsb(frame)
-        if len(binary_data) == 0:
-            continue  # An empty frame could exist if it's a palette frame
+    if mode == SteganographyMethod.LSB:
+        frames = _read_frames_as_rgb(input_filename)
+        for frame in frames:
+            # Extract the binary data from the frame
+            binary_data: str = _extract_data_from_frame_lsb(frame)
+            if len(binary_data) == 0:
+                continue
+
+            binary_data_list.append(binary_data)
+
+    elif mode == SteganographyMethod.CSHIFT:
+        frames = _read_frames_as_p(input_filename)
+        for frame in frames:
+            # Extract the binary data from the frame
+            binary_data: str = _extract_data_from_frame_cshift(frame)
+            if len(binary_data) == 0:
+                continue
+
+            binary_data_list.append(binary_data)
+    else:
+        raise NotImplementedError(f"Steganography method '{mode}' is not implemented.")
 
+    for binary_data in binary_data_list:
         # Decode the Reed-Solomon encoded data
         try:
             data_bytes: bytes = _rs_decode_from_binary(binary_data, nsym)
             data: bytes = _decompress(data_bytes)
 
             messages.append(data)
         except ReedSolomonError:
```

### Comparing `gif-steganography-0.0.1/src/gif_steganography/encode.py` & `gif-steganography-0.1.0/src/gif_steganography/encode.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 
 from PIL import Image
 
 from .common import CapacityError, SteganographyMethod
 from .lib._compression import _compress
 from .lib._ecc import _rs_encode_to_binary
 from .lib._encryption import _encrypt_message
-from .lib._gif import _read_frames_as_rgb, _write_frames_as_rgb
+from .lib._gif import (
+    _read_frames_as_rgb,
+    _write_frames_as_rgb,
+    _read_frames_as_p,
+    _write_frames_as_p,
+)
+from .modes._cshift import _embed_data_in_frame_cshift
 from .modes._lsb import _embed_data_in_frame_lsb
 
 
 def encode(
     input_filename: str,
     output_filename: str,
     message: str,
@@ -39,40 +45,56 @@
     # If as password is provided, encrypt the data
     if passphrase is not None:
         data = _encrypt_message(message, passphrase)
     else:
         # Convert the message to bytes
         data = message.encode()
 
-    frames: List[Image.Image] = _read_frames_as_rgb(input_filename)
+    data_bytes: bytes = _compress(data)
 
-    # The save operation changes a GIF's palette, so we need to re-read it
-    with tempfile.NamedTemporaryFile(suffix=".gif") as temp_file:
-        temp_filename: str = temp_file.name
-        _write_frames_as_rgb(frames, temp_filename)
-        frames = _read_frames_as_rgb(temp_filename)
+    if mode == SteganographyMethod.LSB:
+        frames: List[Image.Image] = _read_frames_as_rgb(input_filename)
 
-    if frames:
-        data_bytes: bytes = _compress(data)
+        # The save operation changes a GIF's palette, so we need to re-read it
+        with tempfile.NamedTemporaryFile(suffix=".gif") as temp_file:
+            temp_filename: str = temp_file.name
+            _write_frames_as_rgb(frames, temp_filename)
+            frames = _read_frames_as_rgb(temp_filename)
 
         # Calculate the total available space in the smallest frame
         smallest_frame: Image.Image = min(
             frames, key=lambda frame: frame.size[0] * frame.size[1]
         )
-        total_bits: int = smallest_frame.size[0] * smallest_frame.size[1] * 3
-        total_bytes: int = total_bits // 8  # Convert bits to bytes
+
+        total_bytes = (smallest_frame.size[0] * smallest_frame.size[1] * 3) // 8
 
         if len(data_bytes) > total_bytes:
             raise CapacityError("Input data too large to fit in the input file.")
 
         # Pad the data with null bytes to fill the frame
         filler_bytes: bytes = b"\x00" * (total_bytes - len(data_bytes) - nsym)
 
         # Encode the data with the Reed-Solomon codec
-        binary_data: bytes = _rs_encode_to_binary(data_bytes + filler_bytes, nsym)
+        binary_data: str = _rs_encode_to_binary(data_bytes + filler_bytes, nsym)
 
         # Embed the data in the frames
         for frame in frames:
             # Mirror the data to embed it in all frames
             _embed_data_in_frame_lsb(frame, binary_data)
 
         _write_frames_as_rgb(frames, output_filename)
+
+    elif mode == SteganographyMethod.CSHIFT:
+        frames: List[Image.Image] = _read_frames_as_p(input_filename)
+
+        # Encode the data with the Reed-Solomon codec
+        binary_data: str = _rs_encode_to_binary(data_bytes + b"\x00", nsym)
+
+        # Embed the data in the frames
+        for frame in frames:
+            # Mirror the data to embed it in all frames
+            _embed_data_in_frame_cshift(frame, binary_data)
+
+        _write_frames_as_p(frames, output_filename)
+
+    else:
+        raise NotImplementedError(f"Steganography method '{mode}' is not implemented.")
```

### Comparing `gif-steganography-0.0.1/src/gif_steganography/lib/_encryption.py` & `gif-steganography-0.1.0/src/gif_steganography/lib/_encryption.py`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/src/gif_steganography/lib/_gif.py` & `gif-steganography-0.1.0/src/gif_steganography/lib/_gif.py`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/src/gif_steganography/modes/_lsb.py` & `gif-steganography-0.1.0/src/gif_steganography/modes/_lsb.py`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/tests/data/input.gif` & `gif-steganography-0.1.0/tests/data/input/small.gif`

 * *Files identical despite different names*

### Comparing `gif-steganography-0.0.1/PKG-INFO` & `gif-steganography-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: gif-steganography
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Python GIF steganography library supporting encryption to embed and extract secure messages within GIF images.
 License: MIT
 Author-email: nebmit <76664673+nebmit@users.noreply.github.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # GIF Steganography
 
+[![Tests](https://github.com/nebmit/gif-steganography/actions/workflows/python-package.yml/badge.svg)](https://github.com/nebmit/gif-steganography/actions/workflows/python-package.yml)
+[![PyPI version](https://badge.fury.io/py/gif-steganography.svg)](https://badge.fury.io/py/gif-steganography)
+[![Dependencies](https://img.shields.io/librariesio/release/pypi/gif-steganography)](https://libraries.io/pypi/gif-steganography)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Python version](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+
 ## Overview
 
-This project implements GIF steganography using the Least Significant Bit (LSB) technique, coupled with additional layers of security and integrity verification. It enables the encoding of secret messages into GIF images and the decoding of these messages from the images, ensuring the message's secrecy and integrity through encryption, compression, and error correction.
+This project implements GIF steganography using various techniques, coupled with additional layers of security and integrity verification. It enables the encoding of secret messages into GIF images and the decoding of these messages from the images, ensuring the message's secrecy and integrity through encryption, compression, and error correction.
 
 ## Installation
 
 ```bash
 pip install gif-steganography
 ```
-Requires Python 3.10^. Installs the package and all necessary dependencies.
+Requires Python >= 3.10. Installs the package and all necessary dependencies.
 
 ## Usage
 
-### CLI
-
 #### Encode a Message
 
 ```bash
 gif-steganography encode <input.gif> <output.gif> "Secret Message" "Passphrase" [--nsym 10]
 ```
 - `--nsym` (optional): Sets the Reed-Solomon error correction level. Default is 10.
 
@@ -43,33 +47,33 @@
 Beyond the command-line interface, `gif-steganography` also provides direct API access for integrating steganographic functionalities into Python scripts.
 
 #### Basic Encoding and Decoding
 
 Embed and retrieve messages programmatically:
 
 ```python
-from gif_steganography import encode, decode
+from gif_steganography import SteganographyMethod, decode, encode
 
 # Embed a message
-encode("input.gif", "output.gif", "Hello, world!")
+encode("input.gif", "output.gif", "Hello, world!", mode=SteganographyMethod.LSB)
 
 # Retrieve a message
 message, _ = decode("output.gif")
 print(message)  # Output: Hello, world!
 ```
 
 #### Secure Encoding and Decoding
 
 For added security, use encryption with your messages:
 
 ```python
-from gif_steganography import encode, decode
+from gif_steganography import SteganographyMethod, decode, encode
 
 # Securely embed a message
-encode("input.gif", "output.gif", "Hello, world!", passphrase="password")
+encode("input.gif", "output.gif", "Hello, world!", passphrase="password", mode=SteganographyMethod.CSHIFT)
 
 # Securely retrieve a message
 message, _ = decode("output.gif", passphrase="password")
 print(message)  # Output: Hello, world!
 ```
 
 ## Project Structure
```

