# Comparing `tmp/packet-framing-0.1.tar.gz` & `tmp/packet-framing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packet-framing-0.1.tar", last modified: Thu Feb 22 11:59:14 2024, max compression
+gzip compressed data, was "packet-framing-0.2.tar", last modified: Tue Apr  9 12:00:28 2024, max compression
```

## Comparing `packet-framing-0.1.tar` & `packet-framing-0.2.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:59:14.236432 packet-framing-0.1/
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     1097 2024-01-10 12:50:39.000000 packet-framing-0.1/LICENSE
--rw-r--r--   0 raulik    (1000) raulik    (1000)      408 2024-02-22 11:59:14.236432 packet-framing-0.1/PKG-INFO
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      292 2024-02-22 11:34:31.000000 packet-framing-0.1/README.md
-drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:59:14.232432 packet-framing-0.1/framing/
--rw-rw-r--   0 raulik    (1000) raulik    (1000)        0 2024-01-11 11:09:34.000000 packet-framing-0.1/framing/__init__.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)    16108 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/backends.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)    13828 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/base.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     4156 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/codecs.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     3164 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/data_queue.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)    23498 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/fields.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     2437 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_processors.py
-drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:59:14.236432 packet-framing-0.1/framing/frame_types/
--rw-rw-r--   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:21:42.000000 packet-framing-0.1/framing/frame_types/__init__.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      661 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/dhcp_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     5031 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/dns_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      759 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/ethernet_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     1602 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/ip_utilities.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     1788 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/ipv4_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     4007 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/ipv6_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     2096 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/pcap_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     2507 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/tcp_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      691 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frame_types/udp_frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     1675 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/frames.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)    16886 2024-02-22 09:10:35.000000 packet-framing-0.1/framing/pcap_analyzer.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)     2131 2024-01-10 12:49:10.000000 packet-framing-0.1/framing/pcap_dump.py
--rw-rw-r--   0 raulik    (1000) raulik    (1000)    19117 2024-02-22 09:11:07.000000 packet-framing-0.1/framing/raw_data.py
-drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:59:14.236432 packet-framing-0.1/packet_framing.egg-info/
--rw-r--r--   0 raulik    (1000) raulik    (1000)      408 2024-02-22 11:59:14.000000 packet-framing-0.1/packet_framing.egg-info/PKG-INFO
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      753 2024-02-22 11:59:14.000000 packet-framing-0.1/packet_framing.egg-info/SOURCES.txt
--rw-rw-r--   0 raulik    (1000) raulik    (1000)        1 2024-02-22 11:59:14.000000 packet-framing-0.1/packet_framing.egg-info/dependency_links.txt
--rw-rw-r--   0 raulik    (1000) raulik    (1000)        8 2024-02-22 11:59:14.000000 packet-framing-0.1/packet_framing.egg-info/top_level.txt
--rw-rw-r--   0 raulik    (1000) raulik    (1000)       38 2024-02-22 11:59:14.236432 packet-framing-0.1/setup.cfg
--rw-rw-r--   0 raulik    (1000) raulik    (1000)      559 2024-02-22 11:40:33.000000 packet-framing-0.1/setup.py
+drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-04-09 12:00:28.673954 packet-framing-0.2/
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     1097 2024-01-10 12:50:39.000000 packet-framing-0.2/LICENSE
+-rw-r--r--   0 raulik    (1000) raulik    (1000)      445 2024-04-09 12:00:28.669954 packet-framing-0.2/PKG-INFO
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     2563 2024-04-09 11:59:32.000000 packet-framing-0.2/README.md
+drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-04-09 12:00:28.669954 packet-framing-0.2/framing/
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)        0 2024-01-11 11:09:34.000000 packet-framing-0.2/framing/__init__.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)    17568 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/backends.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)    15737 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/base.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     5357 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/codecs.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     3301 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/data_queue.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)    26642 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/fields.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     4197 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_processors.py
+drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-04-09 12:00:28.669954 packet-framing-0.2/framing/frame_types/
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)        0 2024-02-22 11:21:42.000000 packet-framing-0.2/framing/frame_types/__init__.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)      661 2024-01-10 12:49:10.000000 packet-framing-0.2/framing/frame_types/dhcp_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     5031 2024-01-10 12:49:10.000000 packet-framing-0.2/framing/frame_types/dns_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)      759 2024-01-10 12:49:10.000000 packet-framing-0.2/framing/frame_types/ethernet_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     4555 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_types/ip_utilities.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     1788 2024-01-10 12:49:10.000000 packet-framing-0.2/framing/frame_types/ipv4_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     7091 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_types/ipv6_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     2714 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_types/pcap_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     2721 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_types/tcp_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     3230 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frame_types/tls_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)      691 2024-04-02 16:52:11.000000 packet-framing-0.2/framing/frame_types/udp_frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     2323 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/frames.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     5717 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/layer_stack.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)    16886 2024-03-27 11:22:27.000000 packet-framing-0.2/framing/pcap_analyzer.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     2131 2024-03-25 10:48:34.000000 packet-framing-0.2/framing/pcap_dump.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)     8837 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/pcap_tool.py
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)    20008 2024-04-09 11:59:32.000000 packet-framing-0.2/framing/raw_data.py
+drwxrwxr-x   0 raulik    (1000) raulik    (1000)        0 2024-04-09 12:00:28.669954 packet-framing-0.2/packet_framing.egg-info/
+-rw-r--r--   0 raulik    (1000) raulik    (1000)      445 2024-04-09 12:00:28.000000 packet-framing-0.2/packet_framing.egg-info/PKG-INFO
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)      868 2024-04-09 12:00:28.000000 packet-framing-0.2/packet_framing.egg-info/SOURCES.txt
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)        1 2024-04-09 12:00:28.000000 packet-framing-0.2/packet_framing.egg-info/dependency_links.txt
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)        7 2024-04-09 12:00:28.000000 packet-framing-0.2/packet_framing.egg-info/requires.txt
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)        8 2024-04-09 12:00:28.000000 packet-framing-0.2/packet_framing.egg-info/top_level.txt
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)       38 2024-04-09 12:00:28.673954 packet-framing-0.2/setup.cfg
+-rw-rw-r--   0 raulik    (1000) raulik    (1000)      662 2024-04-09 11:59:32.000000 packet-framing-0.2/setup.py
```

### Comparing `packet-framing-0.1/LICENSE` & `packet-framing-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/backends.py` & `packet-framing-0.2/framing/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,22 @@
         return f"{self.structure_name()}\n{self.copy().dump(copy_sub_frames=True)}"
 
 
 class RawFrame(Frame):
     structure = Structure['RawFrame']()
     data = structure.raw()
 
+    def build_with_lengths(bits: int = None, bytes: int = None, min_bits: int = None, min_bytes: int = None,
+                           default: RawData = Raw.empty) -> Type[Frame]:
+        """Build raw frame with length limits"""
+        class RawFrameWithLength(Frame):
+            structure = Structure['RawFrameWithLength']()
+            data = structure.raw(bits=bits, bytes=bytes, min_bits=min_bits, min_bytes=min_bytes)
+        return RawFrameWithLength
+
 
 class ComposingBackend(BackendImplementation):
     """Backend to compose a frame"""
     def __init__(self, frame: Frame, mappings: LayerMapping):
         super().__init__(frame, mappings)
 
     def get(self, field: Field[F, T]) -> T:
@@ -223,35 +231,53 @@
         self.is_decoder = True
         self.data = data
         self.end_offset_cache: Dict[Field, int] = {}
 
     def get(self, field: Field[F, T]) -> T:
         v = self.field_values.get(field)
         if v is None:
-            assert field.structure == self.structure, self._bad_field_access(field)
-            data, d_len = self.get_raw(field)
-            layer_map = self.mappings.get_mappings(field)
-            try:
-                if layer_map:
-                    # override field to decode as payload frame
-                    v = self.decode_as_frame(layer_map, data)
-                else:
-                    v = field.decode(data, d_len, self)
-            except EOFError as e:
-                raise EOFError(f"{field.field_name} {e}")
+            v = self.get_not_cached(field)
             self.field_values[field] = v
         return v
 
+    def get_not_cached(self, field: Field[F, T]) -> T:
+        assert field.structure == self.structure, self._bad_field_access(field)
+        layer_map = self.mappings.get_mappings(field)
+        if not layer_map and field.direct_decode:
+            v = field.decode_direct(self.data, self)  # quick (hopefully)
+            return v
+        data, d_len = self.get_raw(field)
+        try:
+            if layer_map:
+                # override field to decode as payload frame
+                v = self.decode_as_frame(layer_map, data)
+            else:
+                v = field.decode(data, d_len, self)
+        except EOFError as e:
+            raise EOFError(f"{field.field_name} {e}")
+        return v
+
     def get_raw(self, field: Field) -> Tuple[RawData, int]:
         bit_offset = self.get_bit_offset(field.offset)
         bit_length = field.decode_bit_length(self.data, bit_offset, None, self)
 
         if bit_length < 0 and field.offset.min_tail_length:
             # length not known, limited by space required by later field(s)
             bit_length = max(0, self.data.bit_length() - bit_length - field.offset.min_tail_length)
+            bit_length = field._validate_length(bit_length)
+
+        if field.min_bit_length < field.max_bit_length:
+            # variable length, check find out how much to read
+            avail = self.data.bits_available()
+            if avail >= field.max_bit_length:
+                # maximum amount of data available
+                return self.data.subBlockBits(0, field.max_bit_length), field.max_bit_length
+            # less than maximum surely available, must read to find out
+            data_len = self.data.bit_length()
+            bit_length = field._validate_length(data_len)
 
         if bit_length < 0:
             data = self.data.tailBits(bit_offset)
         else:
             data = self.data.subBlockBits(bit_offset, bit_length)
         return data, bit_length
 
@@ -274,32 +300,39 @@
         v = item_field.decode(data, -1, self)
         return v
 
     def get_bit_offset(self, offset: FieldOffset) -> int:
         prefix = offset.prefix
         if prefix:
             # get offset of the prefix
-            off = self.end_offset_cache.get(prefix.field)
+            field = prefix.field
+            off = self.end_offset_cache.get(field)
             if off is None:
                 # not found from the cache
-                if prefix.field.end_offset_resolver:
+                if field.end_offset_resolver:
                     # Note: field.decode_bit_length would also use the resolver, but it needs the offset
-                    off = int(prefix.field.end_offset_resolver.pull(self))
+                    off = int(field.end_offset_resolver.pull(self))
                 else:
                     # prefix offset + variable length
                     off = self.get_bit_offset(prefix)
-                    p_len = prefix.field.decode_bit_length(self.data, off, None, self)
+                    p_len = field.decode_bit_length(self.data, off, None, self)
+                    if p_len < 0 and field.min_bit_length < field.max_bit_length and not field.offset.min_tail_length:
+                        # maximum length is known
+                        if self.data.bit(off + field.max_bit_length - 1) >= 0:
+                            # maximum data available
+                            p_len = field.max_bit_length
                     if p_len < 0:
                         # no length information, assuming all available
                         p_len = self.data.read_all().bit_length() - off
-                        if prefix.field.offset.min_tail_length:
+                        if field.offset.min_tail_length:
                             # data limited by space required by later field(s)
-                            p_len = max(0, p_len - prefix.field.offset.min_tail_length)
+                            p_len = max(0, p_len - field.offset.min_tail_length)
+                        p_len = field._validate_length(p_len)
                     off += p_len
-                self.end_offset_cache[prefix.field] = off  # cache for next call
+                self.end_offset_cache[field] = off  # cache for next call
         else:
             off = 0
         off += offset.fixed_bit_offset
         return off
 
     def factory(self, decode: RawData = None) -> Callable[[Frame], FrameBackend]:
         def f(frame: Frame):
@@ -314,44 +347,44 @@
     def iterate(self, sequence_field: Field, item_field: Field[F, FT],
                 count=-1, terminator: Optional[Callable[[T], bool]] = None) -> Iterator[FT]:
         v = self.field_values.get(sequence_field)
         if v is not None:
             return v.__iter__()  # already value in memory (we do not store it here)
 
         backend = self
-        data = self.data
 
         class ItemIterator(Iterator[FT]):
-            def __init__(self, offset: int, count: int):
-                self.offset = offset
+            def __init__(self, window: RawData, count: int):
+                self.window = window  # sliding to avoid starting from first sub-block each time
                 self.count = count
                 self.items = 0
                 self.previous = None
 
             def __next__(self) -> Optional[FT]:
                 if 0 <= count <= self.items:
-                    raise StopIteration()
+                    raise StopIteration()  # hit max. count
 
                 if self.previous is not None:
-                    v_len = item_field.decode_bit_length(data, self.offset, self.previous, backend)
-                    self.offset += v_len
+                    # move buffer to next item
+                    v_len = item_field.decode_bit_length(self.window, 0, self.previous, backend)
+                    self.window = self.window.tailBits(v_len)
 
-                n_data = data.tailBits(self.offset)
-                if n_data.octet(0) < 0:
+                if self.window.octet(0) < 0:
                     self.count = self.items
                     raise StopIteration()
-                v = item_field.decode(n_data, -1, backend)
+                v = item_field.decode(self.window, -1, backend)
                 self.items += 1
                 self.previous = v
                 if terminator is not None and terminator(v):
-                    self.count = self.items
+                    self.count = self.items  # hit terminator
                 return v
 
         off = self.get_bit_offset(sequence_field.offset)
-        return ItemIterator(off, count)
+        window = self.data.tailBits(off)
+        return ItemIterator(window, count)
 
     def get_as_frame(self, field: Field[F, T], frame_type: Optional[Type[F]] = None,
                      default_frame=False) -> Optional[Frame]:
         if frame_type:
             raw_data, _ = self.get_raw(field)
             return frame_type(self.factory(raw_data))
         v = self.get(field)
@@ -370,24 +403,17 @@
 
     def get_bit_length(self) -> int:
         if self.known_bit_length < 0:
             if self.choice is not None:
                 rl = self.choice.get_bit_length(self.frame)
             else:
                 rl = self.get_bit_offset(self.structure.fields_length)
-            data_len = self.data.bit_length()
-            if data_len >= 0:
-                if data_len < rl:
-                    # input data is known to be shorter...
-                    raise EOFError(f"Only {self.data.byte_length()} bytes available for " + self.structure_name())
-            elif rl > 0:
-                # length of data is not known
-                last_d = self.data.octet(rl // 8 - 1) if rl % 8 == 0 else self.data.bit(rl - 1)
-                if last_d < 0:
-                    raise EOFError(f"Not enough data for " + self.structure_name())
+            if self.data.bit(rl - 1) < 0:
+                # input data is known to be shorter...
+                raise EOFError(f"Only {self.data.byte_length()} bytes available for " + self.structure_name())
             self.known_bit_length = rl
         return self.known_bit_length
 
     def input_data(self) -> RawData:
         return self.data
 
     def copy(self, parent: Optional[FrameBackend] = None) -> Self:
```

### Comparing `packet-framing-0.1/framing/base.py` & `packet-framing-0.2/framing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,42 +52,61 @@
     """Path pointing to a field"""
     def get(self, frame: 'Frame') -> T:
         raise NotImplementedError()
 
 
 class Field(FieldPointer[F, T]):
     """Base class for fields"""
-    def __init__(self, type_name: str, default_value: T):
+    def __init__(self, type_name: str, default_value: T, fixed_bit_offset=-1):
         self.field_name = "field?"
         self.type_name = type_name
         self.default_value = default_value
+        self.fixed_bit_offset = fixed_bit_offset
         self.fixed_bit_length = -1
+        self.max_bit_length = -1
+        self.min_bit_length = -1
+        self.direct_decode = False
         self.offset = FieldOffset(self)
-        self.structure: Optional['Sturcture'] = None  # set by structure herself
+        self.structure: Optional['Structure'] = None  # set by structure herself
         self.end_offset_resolver: Optional[Calculator] = None
         self.length_resolver: Optional[Calculator] = None
         self.consumed_by: Optional[Field[F, Any]] = None
 
     def get(self, frame: F) -> T:
         return frame.backend.get(self)
 
+    def get_choice(self, frame: F) -> T:
+        """Return the selected choice, when this is a selection field, otherwise the value itself"""
+        v = self.get(frame)
+        if v.backend.choice:
+            return v.backend.choice.get(v)
+        return v
+
     def get_default_value(self, frame: F) -> T:
         return self.default_value
 
     def __getitem__(self, frame: F) -> T:
         return frame.backend.get(self)
 
     def set(self, frame: F, value: T) -> F:
         frame.backend.set(self, value)
         return frame
 
     def __setitem__(self, frame: F, value: T) -> F:
         frame.backend.set(self, value)
         return frame
 
+    def _validate_length(self, bit_length: int) -> int:
+        """Validate bit length against minimum and maximum lengths, raise error if too short"""
+        if self.min_bit_length >= 0 and bit_length < self.min_bit_length:
+            raise EOFError(f"Field '{self.field_name}' too short: {bit_length} < {self.min_bit_length} bits")
+        if self.max_bit_length > 0:
+            bit_length = min(bit_length, self.max_bit_length)
+        return bit_length
+
     def get_bit_length(self, frame: F) -> int:
         """Get bit length for a value"""
         v = frame.backend.get(self)
         return self.encoding_bit_length(frame.backend, v)
 
     def as_frame(self, frame: F, frame_type: Optional[Type[F]] = None, default_frame=True) -> Optional['Frame']:
         """Return value as frame, use type information when available"""
@@ -132,14 +151,18 @@
             bit_length = int(self.length_resolver.pull(backend))
         return bit_length
 
     def decode(self, data: RawData, bit_length: int, backend: 'FrameBackend') -> T:
         """Decode value. Bit length is provided if it is resolved earlier and available"""
         raise NotImplementedError()
 
+    def decode_direct(self, frame_data: RawData, backend: 'FrameBackend') -> T:
+        """Decode value directly from frame data. Called when direct decode is true"""
+        raise NotImplementedError()
+
 
 class FrameBackend:
     """Base class for frame backend"""
     def __init__(self, frame: 'Frame'):
         self.frame = frame
         self.is_decoder = False
         self.structure = FrameStructure.get_struct(frame)
@@ -210,15 +233,15 @@
 
 
 TF = typing.TypeVar("TF", bound='Frame')
 
 
 class Frame(LengthEntity):
     """Base class for frames"""
-    def __init__(self, backend_factory: Callable[['Frame'], FrameBackend]) -> object:
+    def __init__(self, backend_factory: Callable[['Frame'], FrameBackend]):
         self.backend = backend_factory(self)
 
     def bit_length(self) -> int:
         return self.backend.get_bit_length()
 
     def byte_length(self) -> int:
         return self.backend.get_bit_length() // 8
@@ -236,14 +259,15 @@
 
 class FrameStructure(typing.Generic[F]):
     """Frame structure definition"""
     def __init__(self):
         self.structure_name = "Unnamed"
         self.is_selection = False
         self.fields: typing.Dict[str, Field] = {}
+        self.fields_fixed_bit_offset = 0
         self.fields_length = FieldOffset()
         self.commit_procedures: List[typing.Tuple[Optional[Field], Callable[[F], None]]] = []
         self.built = False
 
     def field(self, field: Field) -> Field:
         raise NotImplementedError()
 
@@ -273,20 +297,22 @@
         """Get name or temporary name for a field"""
         return override if override else f"__{len(self.fields)}"
 
     def finish_building(self, frame: F):
         # find field names
         self.structure_name = type(frame).__name__
         i_names: typing.Dict[Field, str] = {}
-        for member in inspect.getmembers(frame):
+        all_members = inspect.getmembers(frame)
+        for member in all_members:
             name, v = member
             if isinstance(v, Field):
                 i_names[v] = name
         # ...keep order of fields
         old_names = self.fields.copy()
+        assert old_names, f"No fields defined for Selection '{self.structure_name}'"
         self.fields.clear()
         for n, v in old_names.items():
             while v.consumed_by:
                 v = v.consumed_by  # wrapped by another field
             nn = i_names[v] if n.startswith("__") else n
             self.fields[nn] = v
             v.field_name = nn
@@ -331,18 +357,33 @@
         self._payload = payload
         if payload:
             self._mappings[payload] = {}
         if base is not None:
             self._payload = base._payload
             base.merge(self)
 
-    def resolve_payload(self, frame: Frame, field: Field, data: Optional[RawData]) -> Frame:
+    def resolve_payload_type(self, frame: Frame, field: Field) -> Type[Frame]:
+        """Resolve payload type, return raw frame if no mapping found"""
+        layer_map = self.get_mappings(field)
+        assert layer_map, f"No known payload mapping for {field}"
+        for type_f, m in layer_map.items():
+            type_v = type_f.get(frame)
+            p_type = m.get(type_v)
+            if p_type is not None:
+                return p_type
+        from framing.backends import RawFrame
+        return RawFrame
+
+    def decode_payload(self, frame: Frame, field: Field, data: Optional[RawData] = None) -> Frame:
+        """Resolve payload type and decode the frame using this mapping"""
         layer_map = self.get_mappings(field)
         assert layer_map, f"No known payload mapping for {field}"
         be = frame.backend
+        if data is None:
+            data = be.get_raw(field)[0]
         return be.decode_as_frame(layer_map, data)
 
     def by(self, type_field: FieldPointer[Any, T], mappings: typing.Dict[T, Type[Frame]]) -> Self:
         """Add mappings for defined payload"""
         mp = self._mappings[self._payload]
         mp.setdefault(type_field, {}).update(mappings)
         return self
```

### Comparing `packet-framing-0.1/framing/codecs.py` & `packet-framing-0.2/framing/codecs.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 
 class IntegerCodec(ValueCodec[int]):
     """Base class for integer codecs"""
     def default_value(self) -> int:
         return 0
 
+    def decode_direct(self, bit_offset: int, data: RawData) -> int:
+        """Decode directly from frame data. Caller must know when supported"""
+        return self.decode(data.tailBits(bit_offset))
+
 
 class FixedByteIntegerCodec(IntegerCodec):
     def __init__(self, byte_length: int, little_end=False):
         self.length = byte_length
         self.little_end = little_end
         if little_end:
             self.steps = list(range(byte_length - 1, -1, -1))
@@ -71,21 +75,30 @@
         v = value
         for i in self.steps:
             b[i] = v % 256
             v >>= 8
         return Raw.bytes(b)
 
     def decode(self, data: RawData) -> int:
+        return self.decode_direct(0, data)
+
+    def decode_direct(self, bit_offset: int, data: RawData) -> int:
+        if bit_offset % 8 == 0:
+            d = data
+            offset = bit_offset // 8
+        else:
+            d = data.tailBits(bit_offset)
+            offset = 0
         v = 0
-        d = 0
+        octet = 0
         for i in self.reverse:
             v <<= 8
-            d = data.octet(i)
-            v |= d
-        if d < 0:
+            octet = d.octet(offset + i)
+            v |= octet
+        if octet < 0:
             raise EOFError()  # only check the last part to minimize impact
         return v
 
     def get_bit_length(self, value: int) -> int:
         return self.length * 8
 
     def get_fixed_bit_length(self) -> int:
@@ -108,14 +121,32 @@
     def decode(self, data: RawData) -> int:
         if self.byte_codec.little_end:
             b = Raw.zeroes(bit_length=8 - self.length % 8) + data
         else:
             b = data + Raw.zeroes(bit_length=8 - self.length % 8)
         return self.byte_codec.decode(b)
 
+    def decode_direct(self, bit_offset: int, data: RawData) -> int:
+        octet_off = bit_offset // 8
+        l_mask = 0xff >> (bit_offset % 8)
+        octet = data.octet(octet_off)
+        v = octet & l_mask if l_mask else octet
+        for i in range(0, self.length // 8):
+            v <<= 8
+            octet = data.octet(octet_off + 1 + i)
+            v |= octet
+        if octet < 0:
+            raise EOFError()  # only check the last part to minimize impact
+        r_shift = 8 - ((bit_offset + self.length) % 8)
+        v = v >> r_shift if r_shift < 8 else v
+        if not self.byte_codec.little_end:
+            # big endian
+            raise NotImplementedError()
+        return v
+
     def get_bit_length(self, value: int) -> int:
         return self.length
 
     def get_fixed_bit_length(self) -> int:
         return self.length
```

### Comparing `packet-framing-0.1/framing/data_queue.py` & `packet-framing-0.2/framing/data_queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,19 @@
         self.modulus = modulus
         self.head = AppendableRawData(prefix or Raw.empty)
         # fragment offset relative to self.offset
         self.fragments: List[Tuple[int, RawData]] = []
 
     # FIXME: Offset wrapping is not working, especially with forwarding!!!
 
-    def push(self, data: RawData, offset: int) -> RawData:
+    def push(self, data: RawData, offset: int = None) -> RawData:
         """Push data to end of the queue"""
+        if offset is None:
+            # as default, continuous data
+            offset = self.offset + self.head.bytes_available()
         # avoid off-set wrapping, trust Python has enough bits in int
         off = (offset + self.modulus - self.offset) % self.modulus
         fix_length = self.head.fixed.byte_length()
         if off < fix_length:
             # part of the data already in
             data = data.tailBytes(fix_length - off)
             if data.byte_length() == 0:
@@ -43,15 +46,15 @@
             self.fragments = self.fragments[1:]
             head_len += add_data.byte_length()
         return data
 
     def forward(self, length) -> Self:
         """Forward offset from beginning of the queue"""
         assert length <= self.head.fixed.byte_length(), "Forwarding queue too fast"
-        self.head = self.head.tailBytes(length)
+        self.head = self.head.forward(length)
         new_offset = (self.offset + length) % self.modulus
         offset_d = new_offset - self.offset
         for i, f in enumerate(self.fragments):
             self.fragments[i] = f[0] - offset_d, f[1]
         self.offset += offset_d
         return self
```

### Comparing `packet-framing-0.1/framing/fields.py` & `packet-framing-0.2/framing/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import enum
 from typing import Iterator
 
 from framing.base import *
+from framing.base import Field, FrameBackend
+from framing.raw_data import RawData
 
 
 class Multiplier(Calculator):
     """Multiply (or divide) the value"""
     def __init__(self, multiplier: float, next_step: Calculator):
         super().__init__(next_step)
         self.multiplier = multiplier
@@ -208,19 +210,22 @@
 
         self.structure.commit_procedures.append((self, commit_proc))
         return self
 
 
 class RawField(ConfigurableField[F, RawData]):
     """Raw data field"""
-    def __init__(self, default_value: RawData):
-        super().__init__("raw", default_value)
-
-    def fixed_length(self, bit_length: int):
-        self.fixed_bit_length = bit_length
+    def __init__(self, default_value: RawData, min_bit_length=-1, max_bit_length=-1, fixed_bit_offset=-1):
+        super().__init__("raw", default_value, fixed_bit_offset)
+        self.max_bit_length = max_bit_length
+        self.min_bit_length = min_bit_length
+        if max_bit_length == min_bit_length and max_bit_length > 0:
+            # fixed length field
+            self.fixed_bit_length = min_bit_length
+            self.direct_decode = self.fixed_bit_offset >= 0 and self.fixed_bit_length >= 0
 
     def get(self, frame: F) -> RawData:
         v = frame.backend.get(self)
         if isinstance(v, Frame):
             # payload can be a frame
             return v.encode()
         return v
@@ -233,42 +238,64 @@
         v = self.as_frame(frame, default_frame=False)
         proc = procedures.get(type(v))
         return proc(v) if proc else None
 
     def get_bit_length(self, frame: F) -> int:
         """Get bit length for a value"""
         v = frame.backend.get(self)
-        return v.bit_length() if isinstance(v, Frame) else v.bit_length()
+        return v.bit_length()
 
     def encoding_bit_length(self, backend: FrameBackend, value: RawData) -> int:
         return value.bit_length()
 
     def encode(self, value: RawData, state: EncodingState) -> RawData:
         return value
 
     def decode_bit_length(self, data: RawData, bit_offset: int, value: Optional[RawData],
                           backend: 'FrameBackend') -> int:
         if value is not None:
             return value.bit_length()  # Pst... value could be Frame, as well
-        return super().decode_bit_length(data, bit_offset, None, backend)
+        bit_len = super().decode_bit_length(data, bit_offset, None, backend)
+        if bit_len >= 0 and self.min_bit_length < self.max_bit_length:
+            # variable length, check limits
+            bit_len = self._validate_length()
+        return bit_len
 
     def decode(self, data: RawData, bit_length: int, backend: FrameBackend) -> RawData:
-        if self.fixed_bit_length < 0:
-            if bit_length >= 0:
-                return data.subBlockBits(0, bit_length)
-            return data  # read it all
-        return data.subBlockBits(0, self.fixed_bit_length)
+        if self.fixed_bit_length >= 0:
+            return data.subBlockBits(0, self.fixed_bit_length)
+        if bit_length >= 0:
+            return data.subBlockBits(0, bit_length)
+        if self.min_bit_length < self.max_bit_length:
+            # variable length, check find out how much to read
+            avail = data.bits_available()
+            if avail >= self.max_bit_length:
+                # maximum amount of data available
+                return data.subBlockBits(0, self.max_bit_length)
+            # less than maximum surely available, must read to find out
+            data_len = data.bit_length()
+            dec_len = self._validate_length(data_len)
+            return data.subBlockBits(0, dec_len)
+        return data  # read it all
+
+    def decode_direct(self, frame_data: RawData, backend: FrameBackend) -> RawData:
+        v = frame_data.subBlockBits(self.fixed_bit_offset, self.fixed_bit_length)
+        return v
 
 
 class IntField(ConfigurableField[F, int], Calculator, CalculatorSource):
     """Integer field"""
-    def __init__(self, codec: IntegerCodec, default_value: int):
+    def __init__(self, codec: IntegerCodec, default_value: int, fixed_bit_offset: int):
         super().__init__("int", default_value)
         self.codec = codec
         self.fixed_bit_length = codec.get_fixed_bit_length()
+        self.fixed_bit_offset = fixed_bit_offset
+        if fixed_bit_offset >= 0 and self.fixed_bit_length >= 0:
+            # fixed integer in fixed offset - fast value decode from frame data
+            self.direct_decode = True
 
     def flag_values(self, definition: Type[enum.IntFlag]) -> Self:
         return self
 
     def encoding_bit_length(self, backend: FrameBackend, value: int) -> int:
         return self.codec.get_bit_length(value)
 
@@ -278,21 +305,33 @@
     def decode_bit_length(self, data: RawData, bit_offset: int, value: Optional[int],
                           backend: 'FrameBackend') -> int:
         if value is not None:
             return self.codec.get_bit_length(value)
         return super().decode_bit_length(data, bit_offset, None, backend)
 
     def decode(self, data: RawData, bit_length: int, backend: FrameBackend) -> int:
-        return self.codec.decode(data)
+        v = self.codec.decode(data)
+        return v
+
+    def decode_direct(self, frame_data: RawData, backend: FrameBackend) -> int:
+        v = self.codec.decode_direct(self.fixed_bit_offset, frame_data)
+        return v
 
     def calculator(self) -> Calculator:
         return self
 
     def pull(self, backend: FrameBackend) -> float:
-        return backend.get(self)
+        # NOTE: Looks like marginal/non-existent improvement
+        # if self.direct_decode and backend.is_decoder:
+        #     # take the shortcut, we are decoding, thus raw data should be available
+        #     raw = backend.input_data()
+        #     r = self.codec.decode_direct(self.fixed_bit_offset, raw)
+        # else:
+        r = backend.get(self)
+        return r
 
     def push(self, backend: FrameBackend, value: float) -> float:
         backend.set(self, int(value))
         return value
 
 
 class SubStructureField(ConfigurableField[F, FT]):
@@ -579,68 +618,91 @@
             previous = v
         return items
 
 
 class Structure(FrameStructure[F]):
     """Frame structure definition"""
 
+    def _update_fixed_length(self, field: Field):
+        """Update fixed length or reset it to -1"""
+        if self.fields_fixed_bit_offset < 0 or field.fixed_bit_length < 0:
+            self.fields_fixed_bit_offset = -1
+        else:
+            self.fields_fixed_bit_offset += field.fixed_bit_length
+
     def field(self, field: Field, name: str = None) -> Field:
         fn = self._get_a_name(name)
         field.structure = self
         self.fields[fn] = field
+        self._update_fixed_length(field)
         return field
 
-    def raw(self, bits: int = None, bytes: int = None, default: RawData = Raw.empty,
+    def raw(self, bits: int = None, bytes: int = None, min_bits: int = None, min_bytes: int = None, default: RawData = None,
             name: str = None) -> RawField[F]:
         fn = self._get_a_name(name)
-        default = default if default else Raw.zeroes(bit_length=bits, byte_length=bytes)
-        f: RawField[F] = RawField(default)
-        f.structure = self
+        fix_len = -1
         if bits is not None:
-            f.fixed_length(bits)
+            fix_len = bits
         if bytes is not None:
-            f.fixed_length(bytes * 8)
+            fix_len = bytes * 8
+        min_len = fix_len
+        if min_bits is not None:
+            min_len = min_bits
+        if min_bytes is not None:
+            min_len = min_bytes * 8
+        assert min_len <= fix_len, f"Minimun length is {min_len} bits and max length is {fix_len} bits"
+        if default is None:
+            default = Raw.empty if min_len < 0 else Raw.zeroes(bit_length=min_len)
+        f: RawField[F] = RawField(default, min_len, fix_len, self.fields_fixed_bit_offset)
+        f.structure = self
         self.fields[fn] = f
+        self._update_fixed_length(f)
         return f
 
     def integer(self, int_format=IntegerFormat(), bytes=-1, bits=-1,
                 default=0, name: str = None) -> IntField[F]:
         fn = self._get_a_name(name)
         if bytes > 0:
             int_format = int_format.bytes(bytes)
         if bits > 0:
             int_format = int_format.bits(bits)
         codec = int_format.create_codec()
-        f = IntField(codec, default)
+        f = IntField(codec, default, fixed_bit_offset=self.fields_fixed_bit_offset)
         f.structure = self
         self.fields[fn] = f
+        self._update_fixed_length(f)
         return f
 
     def sub(self, sub_frame: Type[FT], name: str = None) -> SubStructureField[F, FT]:
         fn = self._get_a_name(name)
         f = SubStructureField(sub_frame)
         f.structure = self
         self.fields[fn] = f
+        self._update_fixed_length(f)
         return f
 
     def at_commit(self, update: Callable[[F], None]):
         self.commit_procedures.append((None, update))
 
 
 class Selection(Structure[F]):
     """A frame which only the chosen field is present"""
     def __init__(self):
         super().__init__()
         self.is_selection = True
         self.choice_map: Dict[Any, ConfigurableField] = {}
         self.reverse_map: Dict[Structure, Any] = {}
 
+    def _update_fixed_length(self, field: Field):
+        self.fields_fixed_bit_offset = 0  # all choices start from offset 0
+
     def choice(self, key, value: ConfigurableField[F, T]) -> ConfigurableField[F, T]:
         if key in self.choice_map or value in self.reverse_map:
             raise Exception(f"Duplicate entry for key {key}")
+        assert isinstance(value, ConfigurableField), "Provide a field for choice(...)"
         self.choice_map[key] = value
         self.reverse_map[value.structure] = key
         return value
 
     def get_field_by(self, key=None) -> Field[F, Any]:
         if key is not None:
             f = self.choice_map.get(key)
```

### Comparing `packet-framing-0.1/framing/frame_types/dhcp_frames.py` & `packet-framing-0.2/framing/frame_types/dhcp_frames.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/frame_types/dns_frames.py` & `packet-framing-0.2/framing/frame_types/dns_frames.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/frame_types/ethernet_frames.py` & `packet-framing-0.2/framing/frame_types/ethernet_frames.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/frame_types/ipv4_frames.py` & `packet-framing-0.2/framing/frame_types/ipv4_frames.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/frame_types/pcap_frames.py` & `packet-framing-0.2/framing/frame_types/pcap_frames.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pathlib
-from typing import Optional, Iterator
+from typing import Iterable, Optional, Iterator
 
 from framing.base import Frame, LayerMapping
 from framing.codecs import IntegerFormat
 from framing.fields import Structure, Sequence, ValueOf
 from framing.frame_types.ethernet_frames import EthernetII
 from framing.frames import Frames
+from framing.layer_stack import StackLayer, StackState
 from framing.raw_data import Raw
 
 # https://datatracker.ietf.org/doc/id/draft-gharris-opsawg-pcap-00.html
 
 Int = IntegerFormat().big_endian()  # big endian integers
 
 
@@ -56,7 +57,23 @@
 class PCAPRecordIterator(Iterator[PacketRecord]):
     """Record iterator"""
     def __init__(self, file: PCAPFile):
         self.source = PCAPFile.Packet_Records.iterate(file)
 
     def __next__(self) -> PacketRecord:
         return self.source.__next__()
+
+
+class PCAPStackLayer(StackLayer):
+    """PCAP stack layer"""
+    def __init__(self):
+        super().__init__(PCAPFile)
+
+    def receive(self, state: StackState) -> Iterable[StackState]:
+        file = PCAPFile(Frames.dissect(state.data))
+        hdr = PCAPFile.File_Header[file]
+        pay_type = FileHeader.LinkType[hdr]
+        state = state.add(file)
+        for i, rec in enumerate(PCAPRecordIterator(file)):
+            pay_data = PacketRecord.Packet_Data[rec]
+            n_state = state.add(rec, pay_type, pay_data)
+            yield n_state
```

### Comparing `packet-framing-0.1/framing/frame_types/tcp_frames.py` & `packet-framing-0.2/framing/frame_types/tcp_frames.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import enum
-from typing import Tuple, Optional
+from typing import Dict, Set, Tuple, Optional
 
 from framing.base import Frame
 from framing.codecs import IntegerFormat
 from framing.data_queue import RawDataQueue
 from framing.fields import Structure, ValueOf
-from framing.raw_data import RawData
+from framing.raw_data import Raw, RawData
 
 
 # https://www.ietf.org/rfc/rfc793.txt
 
 class TCP(Frame):
     structure = Structure['TCP']()
 
@@ -43,19 +43,24 @@
     RST = 0b000000100
     SYN = 0b000000010
     FIN = 0b000000001
 
 
 TCP.Flags.flag_values(TCPFlag)
 
-# source IP address, source port, destination IP address, destination port
+# TCP stream id: source IP address, source port, destination IP address, destination port
 TCP_Stream_Id = Tuple[RawData, int, RawData, int]
+# Null TCP stream id
+TCP_Null_Stream_Id = Tuple[Raw.empty, 0, Raw.empty, 0]
+
+def flip_tcp_stream_id(stream_id: TCP_Stream_Id) -> TCP_Stream_Id:
+    """Flip TCP stream id"""
+    return stream_id[2], stream_id[3], stream_id[0], stream_id[1]
 
 
-# FIXME: Replace by similar class then IPv4Reassembler!
 class TCPDataQueue(RawDataQueue):
     """TCP data queue, one connection to one direction"""
     def __init__(self, start: TCP):
         super().__init__(offset=TCP.Sequence_number[start], modulus=2 ** 32)
         if TCP.Flags[start] & TCPFlag.SYN:
             self.offset += 1
         self.end_offset = -1
```

### Comparing `packet-framing-0.1/framing/frame_types/udp_frames.py` & `packet-framing-0.2/framing/frame_types/udp_frames.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/frames.py` & `packet-framing-0.2/framing/frames.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pathlib
 from typing import Callable, cast, Type, Dict, Any, TypeVar, Optional
 
 from framing.backends import ComposingBackend, FrameBackend, DissectorBackend, BackendImplementation
 from framing.base import Frame, LayerMapping, F
+from framing.data_queue import RawDataQueue
+from framing.fields import Structure, SubStructureField
 from framing.raw_data import RawData, Raw
 
+F = TypeVar("F", bound=Frame)
 V = TypeVar("V")
 
 
 class Frames:
     @classmethod
     def compose(cls) -> Callable[['Frame'], FrameBackend]:
         """Create new frame for composing"""
@@ -20,14 +23,27 @@
 
     @classmethod
     def dissect_file(cls, file: pathlib.Path) -> Callable[['Frame'], FrameBackend]:
         data = Raw.file(file)
         return lambda f: DissectorBackend(f, LayerMapping(), data)
 
     @classmethod
+    def dissect_pull(cls, frame_type: Type[F], queue: RawDataQueue, mappings=LayerMapping()) -> Optional[F]:
+        """Dissect frame from queue, if enough data. Pulls the frame data if success."""
+        if not queue.head:
+            return None  # no data
+        try:
+            f = frame_type(cls.dissect(queue.head.fixed, mappings=mappings))
+            length = f.byte_length()
+            queue.pull(byte_length=length)
+            return f
+        except EOFError:
+            return None
+
+    @classmethod
     def process(cls, frame: F, procedures: Dict[Type[Frame], Callable[[Any], V]]) -> Optional[V]:
         """Process frame here differentiating by frame type"""
         proc = procedures.get(type(frame))
         if not proc:
             proc = procedures.get(Frame)  # fallback
         return proc(frame) if proc else None
```

### Comparing `packet-framing-0.1/framing/pcap_analyzer.py` & `packet-framing-0.2/framing/pcap_analyzer.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/pcap_dump.py` & `packet-framing-0.2/framing/pcap_dump.py`

 * *Files identical despite different names*

### Comparing `packet-framing-0.1/framing/raw_data.py` & `packet-framing-0.2/framing/raw_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 
 # IP address, shouldn't this be defined by Python?
 IPAddress = Union[ipaddress.IPv6Address, ipaddress.IPv4Address]
 
 
 class LengthEntity:
     def bit_length(self) -> int:
-        """Length in bits or -1 if a stream"""
+        """Length in bits or EOFError if unclosed stream"""
         raise NotImplementedError()
 
     def byte_length(self) -> int:
-        """Length in full bytes or -1 if a stream"""
+        """Length in full bytes or EOFError if unclosed stream"""
         return self.bit_length() // 8
 
 
-class RawData:
+class RawData(LengthEntity):
     """Raw data buffer"""
-    def bit_length(self) -> int:
-        raise NotImplementedError()
-
-    def byte_length(self) -> int:
-        return self.bit_length() // 8
+    def get_bit_length(self) -> int:
+        """Get length in bits or -8 if unknown"""
+        try:
+            return self.bit_length()
+        except EOFError:
+            return -8
+
+    def get_byte_length(self) -> int:
+        """Get length in bytes or -1 if unknown"""
+        try:
+            return self.byte_length()
+        except EOFError:
+            return -1
 
     def bits_available(self) -> int:
         """Number of bits available without waiting"""
         return self.bit_length()
 
     def bytes_available(self) -> int:
         """Number of bytes available without waiting"""
@@ -103,21 +111,21 @@
             d0 = self.octet(i)
         return self.subBlock(0, i)
 
     def __repr__(self):
         return self.dump()
 
     def __bool__(self):
-        return self.bit_length() > 0
+        return self.get_bit_length() != 0
 
     def __eq__(self, other):
         if not isinstance(other, RawData):
             return False
-        blen = self.bit_length()
-        if blen < 0 or other.bit_length() < 0 or (blen != other.bit_length()):
+        blen = self.get_bit_length()
+        if blen < 0 or other.get_bit_length() < 0 or (blen != other.bit_length()):
             return False  # streams cannot be compared or different length
         for i in range(0, blen // 8):
             if self.octet(i) != other.octet(i):
                 return False
         for i in range(blen // 8 * 8, blen):
             if self.bit(i) != other.bit(i):
                 return False
@@ -203,21 +211,15 @@
     def tailBytes(self, byte_offset: int) -> 'RawData':
         ml = max(0, self.length - byte_offset)
         return ByteData(self.data, self.start + byte_offset, ml)
 
 
 class RawDataSequence(RawData):
     def __init__(self, components: List[RawData]):
-        cs = []
-        for c in components:
-            if isinstance(c, RawDataSequence):
-                cs.extend(c.components)
-            elif c.bit_length() > 0:
-                cs.append(c)
-        self.components = cs
+        self.components = components
         self.length = sum([c.bit_length() for c in components])
 
     def bit_length(self) -> int:
         return self.length
 
     def byte_length(self) -> int:
         return self.length // 8
@@ -226,46 +228,52 @@
         off = byte_offset * 8
         for ci, c in enumerate(self.components):
             c_len = c.bit_length()
             if off < c_len:
                 if off % 8 == 0 and off + 8 <= c_len:
                     return c.octet(off // 8)
                 # octet must be collected bit-by-bit (slow!)
-                v = 0
-                for i in range(0, 8):
-                    if off >= c_len:
-                        # next component buffer
-                        off = 0
-                        ci += 1
-                        if ci >= len(self.components):
-                            return -1  # run out of data
-                        c = self.components[ci]
-                        c_len = c.bit_length()
-                    v <<= 1
-                    v |= c.bit(off)
-                    off += 1
+                v = self._collect_octet(off, ci)
                 return v
             off -= c_len
         return -1
 
+    def _collect_octet(self, bit_offset: int, index: int) -> int:
+        v = 0
+        c = self.components[index]
+        c_len = c.bit_length()
+        for i in range(0, 8):
+            if bit_offset >= c_len:
+                # next component buffer
+                bit_offset = 0
+                index += 1
+                if index >= len(self.components):
+                    return -1  # run out of data
+                c = self.components[index]
+                c_len = c.bit_length()
+            v <<= 1
+            v |= c.bit(bit_offset)
+            bit_offset += 1
+        return v
+
+
     def bit(self, bit_offset: int) -> int:
         off = bit_offset
         for c in self.components:
             c_len = c.bit_length()
             if off < c_len:
                 return c.bit(off)
             off -= c_len
         return -1
 
     def subBlockBits(self, bit_offset: int, bit_length: int) -> 'RawData':
         """Get sub-block"""
         if bit_offset == 0 and bit_length == self.bit_length():
             return self
         off = 0
-        end_offset = min(bit_offset + bit_length, self.bit_length())
         nc = []
         got = 0
         for c in self.components:
             c_len = c.bit_length()
             if off + c_len > bit_offset:
                 st = max(0, bit_offset - off)
                 ln = min(c_len - st, bit_length - got)
@@ -292,15 +300,19 @@
             return Raw.empty
         off = bit_offset
         for i, c in enumerate(self.components):
             c_len = c.bit_length()
             if off < c_len:
                 nc = [c.tailBits(off)]
                 nc.extend(self.components[i + 1:])
-                return Raw.sequence(nc)
+                # do not call Raw.sequence(), these components already optimized
+                if len(nc) == 1:
+                    return nc[0]
+                return RawDataSequence(nc)
+                # return Raw.sequence(nc)
             off -= c_len
         return Raw.empty
 
 
 class ZeroData(RawData):
     """All bits zero"""
     def __init__(self, bit_length: int):
@@ -404,19 +416,28 @@
 
     def append(self, data: RawData) -> Self:
         """Append new block to the chain"""
         assert not self.closed, "Cannot append to closed data"
         self.fixed = Raw.sequence([self.fixed, data])
         return self
 
+    def forward(self, byte_length: int) -> 'AppedableRawData':
+        r = AppendableRawData(self.fixed.tailBytes(byte_length))
+        r.closed = self.closed
+        return r
+
     def bit_length(self) -> int:
-        return self.fixed.bit_length() if self.closed else -1
+        if not self.closed:
+            raise EOFError("Stream not closed")
+        return self.fixed.bit_length()
 
     def byte_length(self) -> int:
-        return self.fixed.byte_length() if self.closed else -1
+        if not self.closed:
+            raise EOFError("Stream not closed")
+        return self.fixed.byte_length()
 
     def bits_available(self) -> int:
         return self.fixed.bit_length()
 
     def bytes_available(self) -> int:
         return self.fixed.byte_length()
 
@@ -429,31 +450,32 @@
     def subBlockBits(self, bit_offset: int, bit_length: int) -> 'RawData':
         return self.fixed.subBlockBits(bit_offset, bit_length)
 
     def subBlock(self, byte_offset: int, byte_length: int) -> 'RawData':
         return self.fixed.subBlock(byte_offset, byte_length)
 
     def tailBits(self, bit_offset: int) -> 'RawData':
-        f = self.fixed.tailBits(bit_offset)
-        return f if self.closed else AppendableRawData(f)
+        return self.fixed.tailBits(bit_offset)
 
     def tailBytes(self, byte_offset: int) -> 'RawData':
-        f = self.fixed.tailBytes(byte_offset)
-        return f if self.closed else AppendableRawData(f)
+        return self.fixed.tailBytes(byte_offset)
 
     def close(self) -> 'RawData':
         self.closed = True
         return self
 
     def __repr__(self):
         return self.fixed.__repr__()
 
     def __eq__(self, other):
         return self.fixed == other
 
+    def __bool__(self):
+        return (not self.closed) or self.fixed.bit_length() > 0
+
 
 class StreamData(RawData):
     """Stream data, input stream should be in blocking mode"""
     def __init__(self, stream: BinaryIO, name: str, request_size=65536):
         self.stream = stream
         self.stream_name = name
         self.buffer = AppendableRawData(Raw.empty)
@@ -551,22 +573,31 @@
             return ZeroData(byte_length * 8)
         if bit_length is not None:
             return ZeroData(bit_length)
         return cls.empty
 
     @classmethod
     def sequence(cls, components: Iterable[RawData]) -> RawData:
-        cs = list(components)
+        cs = []
+        for c in components:
+            if isinstance(c, RawDataSequence):
+                cs.extend(c.components)
+            elif c.bit_length() > 0:
+                cs.append(c)
         if not cs:
             return cls.empty
         if len(cs) == 1:
             return cs[0]
         return RawDataSequence(cs)
 
     @classmethod
+    def concat(cls, *components: RawData) -> RawData:
+        return cls.sequence(components)
+
+    @classmethod
     def file(cls, file_path: pathlib.Path) -> FileData:
         f = file_path.open("rb")
         return FileData(f, file_path)
 
     @classmethod
     def stream(cls, stream: BinaryIO, name="stream", request_size=65536) -> StreamData:
         return StreamData(stream, name, request_size)
```

### Comparing `packet-framing-0.1/packet_framing.egg-info/SOURCES.txt` & `packet-framing-0.2/packet_framing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 framing/backends.py
 framing/base.py
 framing/codecs.py
 framing/data_queue.py
 framing/fields.py
 framing/frame_processors.py
 framing/frames.py
+framing/layer_stack.py
 framing/pcap_analyzer.py
 framing/pcap_dump.py
+framing/pcap_tool.py
 framing/raw_data.py
 framing/frame_types/__init__.py
 framing/frame_types/dhcp_frames.py
 framing/frame_types/dns_frames.py
 framing/frame_types/ethernet_frames.py
 framing/frame_types/ip_utilities.py
 framing/frame_types/ipv4_frames.py
 framing/frame_types/ipv6_frames.py
 framing/frame_types/pcap_frames.py
 framing/frame_types/tcp_frames.py
+framing/frame_types/tls_frames.py
 framing/frame_types/udp_frames.py
 packet_framing.egg-info/PKG-INFO
 packet_framing.egg-info/SOURCES.txt
 packet_framing.egg-info/dependency_links.txt
+packet_framing.egg-info/requires.txt
 packet_framing.egg-info/top_level.txt
```

