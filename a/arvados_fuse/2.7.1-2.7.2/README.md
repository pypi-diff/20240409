# Comparing `tmp/arvados_fuse-2.7.1.tar.gz` & `tmp/arvados_fuse-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados_fuse-2.7.1.tar", last modified: Tue Dec 12 20:52:04 2023, max compression
+gzip compressed data, was ".upload_dist/arvados_fuse-2.7.2.tar", last modified: Tue Apr  9 20:11:35 2024, max compression
```

## Comparing `arvados_fuse-2.7.1.tar` & `arvados_fuse-2.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2495 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/README.rst
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/agpl-3.0.txt
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28592 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    22712 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/command.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/crunchstat.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4238 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/fresh.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    51578 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/fusedir.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4331 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/fusefile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6742 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_fuse/unmount.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      137 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/arvados_fuse.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/bin/arv-mount
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-12-12 20:52:04.000000 arvados_fuse-2.7.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1874 2023-12-12 20:51:23.000000 arvados_fuse-2.7.1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2495 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/README.rst
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/agpl-3.0.txt
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35946 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    25796 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/command.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/crunchstat.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4009 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/fresh.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    56792 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/fusedir.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4560 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/fusefile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7328 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_fuse/unmount.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3551 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      145 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/arvados_fuse.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/bin/arv-mount
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-04-09 20:11:35.000000 arvados_fuse-2.7.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1882 2024-04-09 20:11:07.000000 arvados_fuse-2.7.2/setup.py
```

### Comparing `arvados_fuse-2.7.1/PKG-INFO` & `arvados_fuse-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados_fuse
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.7.1/README.rst` & `arvados_fuse-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.1/agpl-3.0.txt` & `arvados_fuse-2.7.2/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.1/arvados_fuse/__init__.py` & `arvados_fuse-2.7.2/arvados_fuse/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,24 +43,23 @@
 - Call the relevant method on the file system object.
 
 - Return the result.
 
 The FUSE driver supports the Arvados event bus.  When an event is received for
 an object that is live in the inode cache, that object is immediately updated.
 
+Implementation note: in the code, the terms 'object', 'entry' and
+'inode' are used somewhat interchangeably, but generally mean an
+arvados_fuse.File or arvados_fuse.Directory object which has numeric
+inode assigned to it and appears in the Inodes._entries dictionary.
+
 """
 
 from __future__ import absolute_import
 from __future__ import division
-from future.utils import viewitems
-from future.utils import native
-from future.utils import listvalues
-from future.utils import listitems
-from future import standard_library
-standard_library.install_aliases()
 from builtins import next
 from builtins import str
 from builtins import object
 import os
 import llfuse
 import errno
 import stat
@@ -72,30 +71,19 @@
 import threading
 import itertools
 import collections
 import functools
 import arvados.keep
 from prometheus_client import Summary
 import queue
-
-# Default _notify_queue has a limit of 1000 items, but it really needs to be
-# unlimited to avoid deadlocks, see https://arvados.org/issues/3198#note-43 for
-# details.
-
-if hasattr(llfuse, 'capi'):
-    # llfuse < 0.42
-    llfuse.capi._notify_queue = queue.Queue()
-else:
-    # llfuse >= 0.42
-    llfuse._notify_queue = queue.Queue()
-
-LLFUSE_VERSION_0 = llfuse.__version__.startswith('0')
+from dataclasses import dataclass
+import typing
 
 from .fusedir import Directory, CollectionDirectory, TmpCollectionDirectory, MagicDirectory, TagsDirectory, ProjectDirectory, SharedDirectory, CollectionDirectoryBase
-from .fusefile import StringFile, FuseArvadosFile
+from .fusefile import File, StringFile, FuseArvadosFile
 
 _logger = logging.getLogger('arvados.arvados_fuse')
 
 # Uncomment this to enable llfuse debug logging.
 # log_handler = logging.StreamHandler()
 # llogger = logging.getLogger('llfuse')
 # llogger.addHandler(log_handler)
@@ -124,203 +112,420 @@
     def flush(self):
         if self.obj.writable():
             return self.obj.flush()
 
 
 class DirectoryHandle(Handle):
     """Connects a numeric file handle to a Directory object that has
-    been opened by the client."""
+    been opened by the client.
+
+    DirectoryHandle is used by opendir() and readdir() to get
+    directory listings.  Entries returned by readdir() don't increment
+    the lookup count (kernel references), so increment our internal
+    "use count" to avoid having an item being removed mid-read.
+
+    """
 
     def __init__(self, fh, dirobj, entries):
         super(DirectoryHandle, self).__init__(fh, dirobj)
         self.entries = entries
 
+        for ent in self.entries:
+            ent[1].inc_use()
+
+    def release(self):
+        for ent in self.entries:
+            ent[1].dec_use()
+        super(DirectoryHandle, self).release()
+
 
 class InodeCache(object):
     """Records the memory footprint of objects and when they are last used.
 
-    When the cache limit is exceeded, the least recently used objects are
-    cleared.  Clearing the object means discarding its contents to release
-    memory.  The next time the object is accessed, it must be re-fetched from
-    the server.  Note that the inode cache limit is a soft limit; the cache
-    limit may be exceeded if necessary to load very large objects, it may also
-    be exceeded if open file handles prevent objects from being cleared.
+    When the cache limit is exceeded, the least recently used objects
+    are cleared.  Clearing the object means discarding its contents to
+    release memory.  The next time the object is accessed, it must be
+    re-fetched from the server.  Note that the inode cache limit is a
+    soft limit; the cache limit may be exceeded if necessary to load
+    very large projects or collections, it may also be exceeded if an
+    inode can't be safely discarded based on kernel lookups
+    (has_ref()) or internal use count (in_use()).
 
     """
 
     def __init__(self, cap, min_entries=4):
-        self._entries = collections.OrderedDict()
-        self._by_uuid = {}
+        # Standard dictionaries are ordered, but OrderedDict is still better here, see
+        # https://docs.python.org/3.11/library/collections.html#ordereddict-objects
+        # specifically we use move_to_end() which standard dicts don't have.
+        self._cache_entries = collections.OrderedDict()
         self.cap = cap
         self._total = 0
         self.min_entries = min_entries
 
     def total(self):
         return self._total
 
-    def _remove(self, obj, clear):
-        if clear:
-            # Kernel behavior seems to be that if a file is
-            # referenced, its parents remain referenced too. This
-            # means has_ref() exits early when a collection is not
-            # candidate for eviction.
-            #
-            # By contrast, in_use() doesn't increment references on
-            # parents, so it requires a full tree walk to determine if
-            # a collection is a candidate for eviction.  This takes
-            # .07s for 240000 files, which becomes a major drag when
-            # cap_cache is being called several times a second and
-            # there are multiple non-evictable collections in the
-            # cache.
-            #
-            # So it is important for performance that we do the
-            # has_ref() check first.
+    def evict_candidates(self):
+        """Yield entries that are candidates to be evicted
+        and stop when the cache total has shrunk sufficiently.
+
+        Implements a LRU cache, when an item is added or touch()ed it
+        goes to the back of the OrderedDict, so items in the front are
+        oldest.  The Inodes._remove() function determines if the entry
+        can actually be removed safely.
 
-            if obj.has_ref(True):
-                _logger.debug("InodeCache cannot clear inode %i, still referenced", obj.inode)
-                return
+        """
 
-            if obj.in_use():
-                _logger.debug("InodeCache cannot clear inode %i, in use", obj.inode)
-                return
+        if self._total <= self.cap:
+            return
+
+        _logger.debug("InodeCache evict_candidates total %i cap %i entries %i", self._total, self.cap, len(self._cache_entries))
 
-            obj.kernel_invalidate()
-            _logger.debug("InodeCache sent kernel invalidate inode %i", obj.inode)
-            obj.clear()
-
-        # The llfuse lock is released in del_entry(), which is called by
-        # Directory.clear().  While the llfuse lock is released, it can happen
-        # that a reentrant call removes this entry before this call gets to it.
-        # Ensure that the entry is still valid before trying to remove it.
-        if obj.inode not in self._entries:
+        # Copy this into a deque for two reasons:
+        #
+        # 1. _cache_entries is modified by unmanage() which is called
+        # by _remove
+        #
+        # 2. popping off the front means the reference goes away
+        # immediately intead of sticking around for the lifetime of
+        # "values"
+        values = collections.deque(self._cache_entries.values())
+
+        while values:
+            if self._total < self.cap or len(self._cache_entries) < self.min_entries:
+                break
+            yield values.popleft()
+
+    def unmanage(self, entry):
+        """Stop managing an object in the cache.
+
+        This happens when an object is being removed from the inode
+        entries table.
+
+        """
+
+        if entry.inode not in self._cache_entries:
             return
 
-        self._total -= obj.cache_size
-        del self._entries[obj.inode]
-        if obj.cache_uuid:
-            self._by_uuid[obj.cache_uuid].remove(obj)
-            if not self._by_uuid[obj.cache_uuid]:
-                del self._by_uuid[obj.cache_uuid]
-            obj.cache_uuid = None
-        if clear:
-            _logger.debug("InodeCache cleared inode %i total now %i", obj.inode, self._total)
+        # manage cache size running sum
+        self._total -= entry.cache_size
+        entry.cache_size = 0
 
-    def cap_cache(self):
-        if self._total > self.cap:
-            for ent in listvalues(self._entries):
-                if self._total < self.cap or len(self._entries) < self.min_entries:
-                    break
-                self._remove(ent, True)
+        # Now forget about it
+        del self._cache_entries[entry.inode]
 
-    def manage(self, obj):
-        if obj.persisted():
-            obj.cache_size = obj.objsize()
-            self._entries[obj.inode] = obj
-            obj.cache_uuid = obj.uuid()
-            if obj.cache_uuid:
-                if obj.cache_uuid not in self._by_uuid:
-                    self._by_uuid[obj.cache_uuid] = [obj]
-                else:
-                    if obj not in self._by_uuid[obj.cache_uuid]:
-                        self._by_uuid[obj.cache_uuid].append(obj)
-            self._total += obj.objsize()
-            _logger.debug("InodeCache touched inode %i (size %i) (uuid %s) total now %i (%i entries)",
-                          obj.inode, obj.objsize(), obj.cache_uuid, self._total, len(self._entries))
-            self.cap_cache()
+    def update_cache_size(self, obj):
+        """Update the cache total in response to the footprint of an
+        object changing (usually because it has been loaded or
+        cleared).
+
+        Adds or removes entries to the cache list based on the object
+        cache size.
+
+        """
+
+        if not obj.persisted():
+            return
+
+        if obj.inode in self._cache_entries:
+            self._total -= obj.cache_size
+
+        obj.cache_size = obj.objsize()
+
+        if obj.cache_size > 0 or obj.parent_inode is None:
+            self._total += obj.cache_size
+            self._cache_entries[obj.inode] = obj
+        elif obj.cache_size == 0 and obj.inode in self._cache_entries:
+            del self._cache_entries[obj.inode]
 
     def touch(self, obj):
-        if obj.persisted():
-            if obj.inode in self._entries:
-                self._remove(obj, False)
-            self.manage(obj)
-
-    def unmanage(self, obj):
-        if obj.persisted() and obj.inode in self._entries:
-            self._remove(obj, True)
+        """Indicate an object was used recently, making it low
+        priority to be removed from the cache.
 
-    def find_by_uuid(self, uuid):
-        return self._by_uuid.get(uuid, [])
+        """
+        if obj.inode in self._cache_entries:
+            self._cache_entries.move_to_end(obj.inode)
+            return True
+        return False
 
     def clear(self):
-        self._entries.clear()
-        self._by_uuid.clear()
+        self._cache_entries.clear()
         self._total = 0
 
+@dataclass
+class RemoveInode:
+    entry: typing.Union[Directory, File]
+    def inode_op(self, inodes, locked_ops):
+        if locked_ops is None:
+            inodes._remove(self.entry)
+            return True
+        else:
+            locked_ops.append(self)
+            return False
+
+@dataclass
+class InvalidateInode:
+    inode: int
+    def inode_op(self, inodes, locked_ops):
+        llfuse.invalidate_inode(self.inode)
+        return True
+
+@dataclass
+class InvalidateEntry:
+    inode: int
+    name: str
+    def inode_op(self, inodes, locked_ops):
+        llfuse.invalidate_entry(self.inode, self.name)
+        return True
+
+@dataclass
+class EvictCandidates:
+    def inode_op(self, inodes, locked_ops):
+        return True
+
+
 class Inodes(object):
-    """Manage the set of inodes.  This is the mapping from a numeric id
-    to a concrete File or Directory object"""
+    """Manage the set of inodes.
+
+    This is the mapping from a numeric id to a concrete File or
+    Directory object
 
-    def __init__(self, inode_cache, encoding="utf-8"):
+    """
+
+    def __init__(self, inode_cache, encoding="utf-8", fsns=None, shutdown_started=None):
         self._entries = {}
         self._counter = itertools.count(llfuse.ROOT_INODE)
         self.inode_cache = inode_cache
         self.encoding = encoding
-        self.deferred_invalidations = []
+        self._fsns = fsns
+        self._shutdown_started = shutdown_started or threading.Event()
+
+        self._inode_remove_queue = queue.Queue()
+        self._inode_remove_thread = threading.Thread(None, self._inode_remove)
+        self._inode_remove_thread.daemon = True
+        self._inode_remove_thread.start()
+
+        self.cap_cache_event = threading.Event()
+        self._by_uuid = collections.defaultdict(list)
 
     def __getitem__(self, item):
         return self._entries[item]
 
     def __setitem__(self, key, item):
         self._entries[key] = item
 
     def __iter__(self):
         return iter(self._entries.keys())
 
     def items(self):
-        return viewitems(self._entries.items())
+        return self._entries.items()
 
     def __contains__(self, k):
         return k in self._entries
 
     def touch(self, entry):
+        """Update the access time, adjust the cache position, and
+        notify the _inode_remove thread to recheck the cache.
+
+        """
+
         entry._atime = time.time()
-        self.inode_cache.touch(entry)
+        if self.inode_cache.touch(entry):
+            self.cap_cache()
+
+    def cap_cache(self):
+        """Notify the _inode_remove thread to recheck the cache."""
+        if not self.cap_cache_event.is_set():
+            self.cap_cache_event.set()
+            self._inode_remove_queue.put(EvictCandidates())
+
+    def update_uuid(self, entry):
+        """Update the Arvados uuid associated with an inode entry.
+
+        This is used to look up inodes that need to be invalidated
+        when a websocket event indicates the object has changed on the
+        API server.
+
+        """
+        if entry.cache_uuid and entry in self._by_uuid[entry.cache_uuid]:
+            self._by_uuid[entry.cache_uuid].remove(entry)
+
+        entry.cache_uuid = entry.uuid()
+        if entry.cache_uuid and entry not in self._by_uuid[entry.cache_uuid]:
+            self._by_uuid[entry.cache_uuid].append(entry)
+
+        if not self._by_uuid[entry.cache_uuid]:
+            del self._by_uuid[entry.cache_uuid]
 
     def add_entry(self, entry):
+        """Assign a numeric inode to a new entry."""
+
         entry.inode = next(self._counter)
         if entry.inode == llfuse.ROOT_INODE:
             entry.inc_ref()
         self._entries[entry.inode] = entry
-        self.inode_cache.manage(entry)
+
+        self.update_uuid(entry)
+        self.inode_cache.update_cache_size(entry)
+        self.cap_cache()
         return entry
 
     def del_entry(self, entry):
-        if entry.ref_count == 0:
-            self.inode_cache.unmanage(entry)
-            del self._entries[entry.inode]
+        """Remove entry from the inode table.
+
+        Indicate this inode entry is pending deletion by setting
+        parent_inode to None.  Notify the _inode_remove thread to try
+        and remove it.
+
+        """
+
+        entry.parent_inode = None
+        self._inode_remove_queue.put(RemoveInode(entry))
+        _logger.debug("del_entry on inode %i with refcount %i", entry.inode, entry.ref_count)
+
+    def _inode_remove(self):
+        """Background thread to handle tasks related to invalidating
+        inodes in the kernel, and removing objects from the inodes
+        table entirely.
+
+        """
+
+        locked_ops = collections.deque()
+        while True:
+            blocking_get = True
+            while True:
+                try:
+                    qentry = self._inode_remove_queue.get(blocking_get)
+                except queue.Empty:
+                    break
+                blocking_get = False
+                if qentry is None:
+                    return
+
+                if self._shutdown_started.is_set():
+                    continue
+
+                # Process this entry
+                if qentry.inode_op(self, locked_ops):
+                    self._inode_remove_queue.task_done()
+
+                # Give up the reference
+                qentry = None
+
+            with llfuse.lock:
+                while locked_ops:
+                    if locked_ops.popleft().inode_op(self, None):
+                        self._inode_remove_queue.task_done()
+                self.cap_cache_event.clear()
+                for entry in self.inode_cache.evict_candidates():
+                    self._remove(entry)
+
+    def wait_remove_queue_empty(self):
+        # used by tests
+        self._inode_remove_queue.join()
+
+    def _remove(self, entry):
+        """Remove an inode entry if possible.
+
+        If the entry is still referenced or in use, don't do anything.
+        If this is not referenced but the parent is still referenced,
+        clear any data held by the object (which may include directory
+        entries under the object) but don't remove it from the inode
+        table.
+
+        """
+        try:
+            if entry.inode is None:
+                # Removed already
+                return
+
+            if entry.inode == llfuse.ROOT_INODE:
+                return
+
+            if entry.in_use():
+                # referenced internally, stay pinned
+                #_logger.debug("InodeCache cannot clear inode %i, in use", entry.inode)
+                return
+
+            # Tell the kernel it should forget about it
+            entry.kernel_invalidate()
+
+            if entry.has_ref():
+                # has kernel reference, could still be accessed.
+                # when the kernel forgets about it, we can delete it.
+                #_logger.debug("InodeCache cannot clear inode %i, is referenced", entry.inode)
+                return
+
+            # commit any pending changes
             with llfuse.lock_released:
                 entry.finalize()
-            entry.inode = None
-        else:
-            entry.dead = True
-            _logger.debug("del_entry on inode %i with refcount %i", entry.inode, entry.ref_count)
+
+            # Clear the contents
+            entry.clear()
+
+            if entry.parent_inode is None:
+                _logger.debug("InodeCache forgetting inode %i, object cache_size %i, cache total %i, forget_inode True, inode entries %i, type %s",
+                              entry.inode, entry.cache_size, self.inode_cache.total(),
+                              len(self._entries), type(entry))
+
+                if entry.cache_uuid:
+                    self._by_uuid[entry.cache_uuid].remove(entry)
+                    if not self._by_uuid[entry.cache_uuid]:
+                        del self._by_uuid[entry.cache_uuid]
+                    entry.cache_uuid = None
+
+                self.inode_cache.unmanage(entry)
+
+                del self._entries[entry.inode]
+                entry.inode = None
+
+        except Exception as e:
+            _logger.exception("failed remove")
 
     def invalidate_inode(self, entry):
-        if entry.has_ref(False):
+        if entry.has_ref():
             # Only necessary if the kernel has previously done a lookup on this
             # inode and hasn't yet forgotten about it.
-            llfuse.invalidate_inode(entry.inode)
+            self._inode_remove_queue.put(InvalidateInode(entry.inode))
 
     def invalidate_entry(self, entry, name):
-        if entry.has_ref(False):
+        if entry.has_ref():
             # Only necessary if the kernel has previously done a lookup on this
             # inode and hasn't yet forgotten about it.
-            llfuse.invalidate_entry(entry.inode, native(name.encode(self.encoding)))
+            self._inode_remove_queue.put(InvalidateEntry(entry.inode, name.encode(self.encoding)))
+
+    def begin_shutdown(self):
+        self._inode_remove_queue.put(None)
+        if self._inode_remove_thread is not None:
+            self._inode_remove_thread.join()
+        self._inode_remove_thread = None
 
     def clear(self):
+        with llfuse.lock_released:
+            self.begin_shutdown()
+
         self.inode_cache.clear()
+        self._by_uuid.clear()
 
-        for k,v in viewitems(self._entries):
+        for k,v in self._entries.items():
             try:
                 v.finalize()
             except Exception as e:
                 _logger.exception("Error during finalize of inode %i", k)
 
         self._entries.clear()
 
+    def forward_slash_subst(self):
+        return self._fsns
+
+    def find_by_uuid(self, uuid):
+        """Return a list of zero or more inode entries corresponding
+        to this Arvados UUID."""
+        return self._by_uuid.get(uuid, [])
+
 
 def catch_exceptions(orig_func):
     """Catch uncaught exceptions and log them consistently."""
 
     @functools.wraps(orig_func)
     def catch_exceptions_wrapper(self, *args, **kwargs):
         try:
@@ -373,40 +578,52 @@
     create_time = fuse_time.labels(op='create')
     mkdir_time = fuse_time.labels(op='mkdir')
     unlink_time = fuse_time.labels(op='unlink')
     rmdir_time = fuse_time.labels(op='rmdir')
     rename_time = fuse_time.labels(op='rename')
     flush_time = fuse_time.labels(op='flush')
 
-    def __init__(self, uid, gid, api_client, encoding="utf-8", inode_cache=None, num_retries=4, enable_write=False):
+    def __init__(self, uid, gid, api_client, encoding="utf-8", inode_cache=None, num_retries=4, enable_write=False, fsns=None):
         super(Operations, self).__init__()
 
         self._api_client = api_client
 
         if not inode_cache:
             inode_cache = InodeCache(cap=256*1024*1024)
-        self.inodes = Inodes(inode_cache, encoding=encoding)
+
+        if fsns is None:
+            try:
+                fsns = self._api_client.config()["Collections"]["ForwardSlashNameSubstitution"]
+            except KeyError:
+                # old API server with no FSNS config
+                fsns = '_'
+            else:
+                if fsns == '' or fsns == '/':
+                    fsns = None
+
+        # If we get overlapping shutdown events (e.g., fusermount -u
+        # -z and operations.destroy()) llfuse calls forget() on inodes
+        # that have already been deleted. To avoid this, we make
+        # forget() a no-op if called after destroy().
+        self._shutdown_started = threading.Event()
+
+        self.inodes = Inodes(inode_cache, encoding=encoding, fsns=fsns,
+                             shutdown_started=self._shutdown_started)
         self.uid = uid
         self.gid = gid
         self.enable_write = enable_write
 
         # dict of inode to filehandle
         self._filehandles = {}
         self._filehandles_counter = itertools.count(0)
 
         # Other threads that need to wait until the fuse driver
         # is fully initialized should wait() on this event object.
         self.initlock = threading.Event()
 
-        # If we get overlapping shutdown events (e.g., fusermount -u
-        # -z and operations.destroy()) llfuse calls forget() on inodes
-        # that have already been deleted. To avoid this, we make
-        # forget() a no-op if called after destroy().
-        self._shutdown_started = threading.Event()
-
         self.num_retries = num_retries
 
         self.read_counter = arvados.keep.Counter()
         self.write_counter = arvados.keep.Counter()
         self.read_ops_counter = arvados.keep.Counter()
         self.write_ops_counter = arvados.keep.Counter()
 
@@ -434,31 +651,34 @@
 
     def metric_sum_func(self, opname):
         return lambda: self.metric_value(opname, "arvmount_fuse_operations_seconds_sum")
 
     def metric_count_func(self, opname):
         return lambda: int(self.metric_value(opname, "arvmount_fuse_operations_seconds_count"))
 
+    def begin_shutdown(self):
+        self._shutdown_started.set()
+        self.inodes.begin_shutdown()
+
     @destroy_time.time()
     @catch_exceptions
     def destroy(self):
-        self._shutdown_started.set()
+        _logger.debug("arv-mount destroy: start")
+
+        with llfuse.lock_released:
+            self.begin_shutdown()
+
         if self.events:
             self.events.close()
             self.events = None
 
-        # Different versions of llfuse require and forbid us to
-        # acquire the lock here. See #8345#note-37, #10805#note-9.
-        if LLFUSE_VERSION_0 and llfuse.lock.acquire():
-            # llfuse < 0.42
-            self.inodes.clear()
-            llfuse.lock.release()
-        else:
-            # llfuse >= 0.42
-            self.inodes.clear()
+        self.inodes.clear()
+
+        _logger.debug("arv-mount destroy: complete")
+
 
     def access(self, inode, mode, ctx):
         return True
 
     def listen_for_events(self):
         self.events = arvados.events.subscribe(
             self._api_client,
@@ -471,36 +691,42 @@
         if 'event_type' not in ev or ev["event_type"] not in ("create", "update", "delete"):
             return
         with llfuse.lock:
             properties = ev.get("properties") or {}
             old_attrs = properties.get("old_attributes") or {}
             new_attrs = properties.get("new_attributes") or {}
 
-            for item in self.inodes.inode_cache.find_by_uuid(ev["object_uuid"]):
+            for item in self.inodes.find_by_uuid(ev["object_uuid"]):
                 item.invalidate()
 
             oldowner = old_attrs.get("owner_uuid")
             newowner = ev.get("object_owner_uuid")
             for parent in (
-                    self.inodes.inode_cache.find_by_uuid(oldowner) +
-                    self.inodes.inode_cache.find_by_uuid(newowner)):
+                    self.inodes.find_by_uuid(oldowner) +
+                    self.inodes.find_by_uuid(newowner)):
                 parent.invalidate()
 
     @getattr_time.time()
     @catch_exceptions
     def getattr(self, inode, ctx=None):
         if inode not in self.inodes:
+            _logger.debug("arv-mount getattr: inode %i missing", inode)
             raise llfuse.FUSEError(errno.ENOENT)
 
         e = self.inodes[inode]
+        self.inodes.touch(e)
+        parent = None
+        if e.parent_inode:
+            parent = self.inodes[e.parent_inode]
+            self.inodes.touch(parent)
 
         entry = llfuse.EntryAttributes()
         entry.st_ino = inode
         entry.generation = 0
-        entry.entry_timeout = 0
+        entry.entry_timeout = parent.time_to_next_poll() if parent is not None else 0
         entry.attr_timeout = e.time_to_next_poll() if e.allow_attr_cache else 0
 
         entry.st_mode = stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH
         if isinstance(e, Directory):
             entry.st_mode |= stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH | stat.S_IFDIR
         else:
             entry.st_mode |= stat.S_IFREG
@@ -560,26 +786,31 @@
     @catch_exceptions
     def lookup(self, parent_inode, name, ctx=None):
         name = str(name, self.inodes.encoding)
         inode = None
 
         if name == '.':
             inode = parent_inode
-        else:
-            if parent_inode in self.inodes:
-                p = self.inodes[parent_inode]
-                self.inodes.touch(p)
-                if name == '..':
-                    inode = p.parent_inode
-                elif isinstance(p, Directory) and name in p:
-                    inode = p[name].inode
+        elif parent_inode in self.inodes:
+            p = self.inodes[parent_inode]
+            self.inodes.touch(p)
+            if name == '..':
+                inode = p.parent_inode
+            elif isinstance(p, Directory) and name in p:
+                if p[name].inode is None:
+                    _logger.debug("arv-mount lookup: parent_inode %i name '%s' found but inode was None",
+                                  parent_inode, name)
+                    raise llfuse.FUSEError(errno.ENOENT)
+
+                inode = p[name].inode
 
         if inode != None:
             _logger.debug("arv-mount lookup: parent_inode %i name '%s' inode %i",
                       parent_inode, name, inode)
+            self.inodes.touch(self.inodes[inode])
             self.inodes[inode].inc_ref()
             return self.getattr(inode)
         else:
             _logger.debug("arv-mount lookup: parent_inode %i name '%s' not found",
                       parent_inode, name)
             raise llfuse.FUSEError(errno.ENOENT)
 
@@ -587,23 +818,24 @@
     @catch_exceptions
     def forget(self, inodes):
         if self._shutdown_started.is_set():
             return
         for inode, nlookup in inodes:
             ent = self.inodes[inode]
             _logger.debug("arv-mount forget: inode %i nlookup %i ref_count %i", inode, nlookup, ent.ref_count)
-            if ent.dec_ref(nlookup) == 0 and ent.dead:
+            if ent.dec_ref(nlookup) == 0 and ent.parent_inode is None:
                 self.inodes.del_entry(ent)
 
     @open_time.time()
     @catch_exceptions
     def open(self, inode, flags, ctx=None):
         if inode in self.inodes:
             p = self.inodes[inode]
         else:
+            _logger.debug("arv-mount open: inode %i missing", inode)
             raise llfuse.FUSEError(errno.ENOENT)
 
         if isinstance(p, Directory):
             raise llfuse.FUSEError(errno.EISDIR)
 
         if ((flags & os.O_WRONLY) or (flags & os.O_RDWR)) and not p.writable():
             raise llfuse.FUSEError(errno.EPERM)
@@ -677,57 +909,64 @@
             try:
                 self._filehandles[fh].flush()
             except Exception:
                 raise
             finally:
                 self._filehandles[fh].release()
                 del self._filehandles[fh]
-        self.inodes.inode_cache.cap_cache()
+        self.inodes.cap_cache()
 
     def releasedir(self, fh):
         self.release(fh)
 
     @opendir_time.time()
     @catch_exceptions
     def opendir(self, inode, ctx=None):
         _logger.debug("arv-mount opendir: inode %i", inode)
 
         if inode in self.inodes:
             p = self.inodes[inode]
         else:
+            _logger.debug("arv-mount opendir: called with unknown or removed inode %i", inode)
             raise llfuse.FUSEError(errno.ENOENT)
 
         if not isinstance(p, Directory):
             raise llfuse.FUSEError(errno.ENOTDIR)
 
         fh = next(self._filehandles_counter)
         if p.parent_inode in self.inodes:
             parent = self.inodes[p.parent_inode]
         else:
+            _logger.warning("arv-mount opendir: parent inode %i of %i is missing", p.parent_inode, inode)
             raise llfuse.FUSEError(errno.EIO)
 
+        _logger.debug("arv-mount opendir: inode %i fh %i ", inode, fh)
+
         # update atime
+        p.inc_use()
+        self._filehandles[fh] = DirectoryHandle(fh, p, [('.', p), ('..', parent)] + p.items())
+        p.dec_use()
         self.inodes.touch(p)
-        self._filehandles[fh] = DirectoryHandle(fh, p, [('.', p), ('..', parent)] + listitems(p))
         return fh
 
     @readdir_time.time()
     @catch_exceptions
     def readdir(self, fh, off):
         _logger.debug("arv-mount readdir: fh %i off %i", fh, off)
 
         if fh in self._filehandles:
             handle = self._filehandles[fh]
         else:
             raise llfuse.FUSEError(errno.EBADF)
 
         e = off
         while e < len(handle.entries):
-            if handle.entries[e][1].inode in self.inodes:
-                yield (handle.entries[e][0].encode(self.inodes.encoding), self.getattr(handle.entries[e][1].inode), e+1)
+            ent = handle.entries[e]
+            if ent[1].inode in self.inodes:
+                yield (ent[0].encode(self.inodes.encoding), self.getattr(ent[1].inode), e+1)
             e += 1
 
     @statfs_time.time()
     @catch_exceptions
     def statfs(self, ctx=None):
         st = llfuse.StatvfsData()
         st.f_bsize = 128 * 1024
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse/command.py` & `arvados_fuse-2.7.2/arvados_fuse/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,108 +24,344 @@
 from arvados_fuse.unmount import unmount
 from arvados_fuse._version import __version__
 
 class ArgumentParser(argparse.ArgumentParser):
     def __init__(self):
         super(ArgumentParser, self).__init__(
             parents=[arv_cmd.retry_opt],
-            description='''Mount Keep data under the local filesystem.  Default mode is --home''',
-            epilog="""
-    Note: When using the --exec feature, you must either specify the
-    mountpoint before --exec, or mark the end of your --exec arguments
-    with "--".
-            """)
-        self.add_argument('--version', action='version',
-                          version=u"%s %s" % (sys.argv[0], __version__),
-                          help='Print version and exit.')
-        self.add_argument('mountpoint', type=str, help="""Mount point.""")
-        self.add_argument('--allow-other', action='store_true',
-                            help="""Let other users read the mount""")
-        self.add_argument('--subtype', type=str, metavar='STRING',
-                            help="""Report mounted filesystem type as "fuse.STRING", instead of just "fuse".""")
-
-        mode = self.add_mutually_exclusive_group()
-
-        mode.add_argument('--all', action='store_const', const='all', dest='mode',
-                                help="""Mount a subdirectory for each mode: home, shared, by_tag, by_id (default if no --mount-* arguments are given).""")
-        mode.add_argument('--custom', action='store_const', const=None, dest='mode',
-                                help="""Mount a top level meta-directory with subdirectories as specified by additional --mount-* arguments (default if any --mount-* arguments are given).""")
-        mode.add_argument('--home', action='store_const', const='home', dest='mode',
-                                help="""Mount only the user's home project.""")
-        mode.add_argument('--shared', action='store_const', const='shared', dest='mode',
-                                help="""Mount only list of projects shared with the user.""")
-        mode.add_argument('--by-tag', action='store_const', const='by_tag', dest='mode',
-                                help="""Mount subdirectories listed by tag.""")
-        mode.add_argument('--by-id', action='store_const', const='by_id', dest='mode',
-                                help="""Mount subdirectories listed by portable data hash or uuid.""")
-        mode.add_argument('--by-pdh', action='store_const', const='by_pdh', dest='mode',
-                                help="""Mount subdirectories listed by portable data hash.""")
-        mode.add_argument('--project', type=str, metavar='UUID',
-                                help="""Mount the specified project.""")
-        mode.add_argument('--collection', type=str, metavar='UUID_or_PDH',
-                                help="""Mount only the specified collection.""")
-
-        mounts = self.add_argument_group('Custom mount options')
-        mounts.add_argument('--mount-by-pdh',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Mount each readable collection at mountpoint/PATH/P where P is the collection's portable data hash.")
-        mounts.add_argument('--mount-by-id',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Mount each readable collection at mountpoint/PATH/UUID and mountpoint/PATH/PDH where PDH is the collection's portable data hash and UUID is its UUID.")
-        mounts.add_argument('--mount-by-tag',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Mount all collections with tag TAG at mountpoint/PATH/TAG/UUID.")
-        mounts.add_argument('--mount-home',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Mount the current user's home project at mountpoint/PATH.")
-        mounts.add_argument('--mount-shared',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Mount projects shared with the current user at mountpoint/PATH.")
-        mounts.add_argument('--mount-tmp',
-                            type=str, metavar='PATH', action='append', default=[],
-                            help="Create a new collection, mount it in read/write mode at mountpoint/PATH, and delete it when unmounting.")
-
-
-        self.add_argument('--debug', action='store_true', help="""Debug mode""")
-        self.add_argument('--logfile', help="""Write debug logs and errors to the specified file (default stderr).""")
-        self.add_argument('--foreground', action='store_true', help="""Run in foreground (default is to daemonize unless --exec specified)""", default=False)
-        self.add_argument('--encoding', type=str, help="Character encoding to use for filesystem, default is utf-8 (see Python codec registry for list of available encodings)", default="utf-8")
-
-        self.add_argument('--file-cache', type=int, help="File data cache size, in bytes (default 8 GiB for disk-based cache or 256 MiB with RAM-only cache)", default=0)
-        self.add_argument('--directory-cache', type=int, help="Directory data cache size, in bytes (default 128 MiB)", default=128*1024*1024)
-
-        cachetype = self.add_mutually_exclusive_group()
-        cachetype.add_argument('--ram-cache', action='store_false', dest='disk_cache', help="Use in-memory caching only", default=True)
-        cachetype.add_argument('--disk-cache', action='store_true', dest='disk_cache', help="Use disk based caching (default)", default=True)
-
-        self.add_argument('--disk-cache-dir', type=str, help="Disk cache location (default ~/.cache/arvados/keep)", default=None)
-
-        self.add_argument('--disable-event-listening', action='store_true', help="Don't subscribe to events on the API server", dest="disable_event_listening", default=False)
-
-        self.add_argument('--read-only', action='store_false', help="Mount will be read only (default)", dest="enable_write", default=False)
-        self.add_argument('--read-write', action='store_true', help="Mount will be read-write", dest="enable_write", default=False)
-        self.add_argument('--storage-classes', type=str, metavar='CLASSES', help="Specify comma separated list of storage classes to be used when saving data of new collections", default=None)
-
-        self.add_argument('--crunchstat-interval', type=float, help="Write stats to stderr every N seconds (default disabled)", default=0)
-
-        unmount = self.add_mutually_exclusive_group()
-        unmount.add_argument('--unmount', action='store_true', default=False,
-                             help="Forcefully unmount the specified mountpoint (if it's a fuse mount) and exit. If --subtype is given, unmount only if the mount has the specified subtype. WARNING: This command can affect any kind of fuse mount, not just arv-mount.")
-        unmount.add_argument('--unmount-all', action='store_true', default=False,
-                             help="Forcefully unmount every fuse mount at or below the specified path and exit. If --subtype is given, unmount only mounts that have the specified subtype. Exit non-zero if any other types of mounts are found at or below the given path. WARNING: This command can affect any kind of fuse mount, not just arv-mount.")
-        unmount.add_argument('--replace', action='store_true', default=False,
-                             help="If a fuse mount is already present at mountpoint, forcefully unmount it before mounting")
-        self.add_argument('--unmount-timeout',
-                          type=float, default=2.0,
-                          help="Time to wait for graceful shutdown after --exec program exits and filesystem is unmounted")
-
-        self.add_argument('--exec', type=str, nargs=argparse.REMAINDER,
-                            dest="exec_args", metavar=('command', 'args', '...', '--'),
-                            help="""Mount, run a command, then unmount and exit""")
-
+            description="Interact with Arvados data through a local filesystem",
+        )
+        self.add_argument(
+            '--version',
+            action='version',
+            version=u"%s %s" % (sys.argv[0], __version__),
+            help="Print version and exit",
+        )
+        self.add_argument(
+            'mountpoint',
+            metavar='MOUNT_DIR',
+            help="Directory path to mount data",
+        )
+
+        mode_group = self.add_argument_group("Mount contents")
+        mode = mode_group.add_mutually_exclusive_group()
+        mode.add_argument(
+            '--all',
+            action='store_const',
+            const='all',
+            dest='mode',
+            help="""
+Mount a subdirectory for each mode: `home`, `shared`, `by_id`, and `by_tag`
+(default if no `--mount-*` options are given)
+""",
+        )
+        mode.add_argument(
+            '--custom',
+            action='store_const',
+            const=None,
+            dest='mode',
+            help="""
+Mount a subdirectory for each mode specified by a `--mount-*` option
+(default if any `--mount-*` options are given;
+see "Mount custom layout and filtering" section)
+""",
+        )
+        mode.add_argument(
+            '--collection',
+            metavar='UUID_OR_PDH',
+            help="Mount the specified collection",
+        )
+        mode.add_argument(
+            '--home',
+            action='store_const',
+            const='home',
+            dest='mode',
+            help="Mount your home project",
+        )
+        mode.add_argument(
+            '--project',
+            metavar='UUID',
+            help="Mount the specified project",
+        )
+        mode.add_argument(
+            '--shared',
+            action='store_const',
+            const='shared',
+            dest='mode',
+            help="Mount a subdirectory for each project shared with you",
+        )
+        mode.add_argument(
+            '--by-id',
+            action='store_const',
+            const='by_id',
+            dest='mode',
+            help="""
+Mount a magic directory where collections and projects are accessible through
+subdirectories named after their UUID or portable data hash
+""",
+        )
+        mode.add_argument(
+            '--by-pdh',
+            action='store_const',
+            const='by_pdh',
+            dest='mode',
+            help="""
+Mount a magic directory where collections are accessible through
+subdirectories named after their portable data hash
+""",
+        )
+        mode.add_argument(
+            '--by-tag',
+            action='store_const',
+            const='by_tag',
+            dest='mode',
+            help="Mount a subdirectory for each tag attached to a collection or project",
+        )
+
+        mounts = self.add_argument_group("Mount custom layout and filtering")
+        mounts.add_argument(
+            '--filters',
+            type=arv_cmd.JSONArgument(arv_cmd.validate_filters),
+            help="""
+Filters to apply to all project, shared, and tag directory contents.
+Pass filters as either a JSON string or a path to a JSON file.
+The JSON object should be a list of filters in Arvados API list filter syntax.
+""",
+        )
+        mounts.add_argument(
+            '--mount-home',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="Make your home project available under the mount at `PATH`",
+        )
+        mounts.add_argument(
+            '--mount-shared',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="Make projects shared with you available under the mount at `PATH`",
+        )
+        mounts.add_argument(
+            '--mount-tmp',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="""
+Make a new temporary writable collection available under the mount at `PATH`.
+This collection is deleted when the mount is unmounted.
+""",
+        )
+        mounts.add_argument(
+            '--mount-by-id',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="""
+Make a magic directory available under the mount at `PATH` where collections and
+projects are accessible through subdirectories named after their UUID or
+portable data hash
+""",
+        )
+        mounts.add_argument(
+            '--mount-by-pdh',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="""
+Make a magic directory available under the mount at `PATH` where collections
+are accessible through subdirectories named after portable data hash
+""",
+        )
+        mounts.add_argument(
+            '--mount-by-tag',
+            metavar='PATH',
+            action='append',
+            default=[],
+            help="""
+Make a subdirectory for each tag attached to a collection or project available
+under the mount at `PATH`
+""" ,
+        )
+
+        perms = self.add_argument_group("Mount access and permissions")
+        perms.add_argument(
+            '--allow-other',
+            action='store_true',
+            help="Let other users on this system read mounted data (default false)",
+        )
+        perms.add_argument(
+            '--read-only',
+            action='store_false',
+            default=False,
+            dest='enable_write',
+            help="Mounted data cannot be modified from the mount (default)",
+        )
+        perms.add_argument(
+            '--read-write',
+            action='store_true',
+            default=False,
+            dest='enable_write',
+            help="Mounted data can be modified from the mount",
+        )
+
+        lifecycle = self.add_argument_group("Mount lifecycle management")
+        lifecycle.add_argument(
+            '--exec',
+            nargs=argparse.REMAINDER,
+            dest="exec_args",
+            help="""
+Mount data, run the specified command, then unmount and exit.
+`--exec` reads all remaining options as the command to run,
+so it must be the last option you specify.
+Either end your command arguments (and other options) with a `--` argument,
+or specify `--exec` after your mount point.
+""",
+        )
+        lifecycle.add_argument(
+            '--foreground',
+            action='store_true',
+            default=False,
+            help="Run mount process in the foreground instead of daemonizing (default false)",
+        )
+        lifecycle.add_argument(
+            '--subtype',
+            help="Set mounted filesystem type to `fuse.SUBTYPE` (default is just `fuse`)",
+        )
+        unmount = lifecycle.add_mutually_exclusive_group()
+        unmount.add_argument(
+            '--replace',
+            action='store_true',
+            default=False,
+            help="""
+If a FUSE mount is already mounted at the given directory,
+unmount it before mounting the requested data.
+If `--subtype` is specified, unmount only if the mount has that subtype.
+WARNING: This command can affect any kind of FUSE mount, not just arv-mount.
+""",
+        )
+        unmount.add_argument(
+            '--unmount',
+            action='store_true',
+            default=False,
+            help="""
+If a FUSE mount is already mounted at the given directory, unmount it and exit.
+If `--subtype` is specified, unmount only if the mount has that subtype.
+WARNING: This command can affect any kind of FUSE mount, not just arv-mount.
+""",
+        )
+        unmount.add_argument(
+            '--unmount-all',
+            action='store_true',
+            default=False,
+            help="""
+Unmount all FUSE mounts at or below the given directory, then exit.
+If `--subtype` is specified, unmount only if the mount has that subtype.
+WARNING: This command can affect any kind of FUSE mount, not just arv-mount.
+""",
+        )
+        lifecycle.add_argument(
+            '--unmount-timeout',
+            type=float,
+            default=2.0,
+            metavar='SECONDS',
+            help="""
+The number of seconds to wait for a clean unmount after an `--exec` command has
+exited (default %(default).01f).
+After this time, the mount will be forcefully unmounted.
+""",
+        )
+
+        reporting = self.add_argument_group("Mount logging and statistics")
+        reporting.add_argument(
+            '--crunchstat-interval',
+            type=float,
+            default=0.0,
+            metavar='SECONDS',
+            help="Write stats to stderr every N seconds (default disabled)",
+        )
+        reporting.add_argument(
+            '--debug',
+            action='store_true',
+            help="Log debug information",
+        )
+        reporting.add_argument(
+            '--logfile',
+            help="Write debug logs and errors to the specified file (default stderr)",
+        )
+
+        cache = self.add_argument_group("Mount local cache setup")
+        cachetype = cache.add_mutually_exclusive_group()
+        cachetype.add_argument(
+            '--disk-cache',
+            action='store_true',
+            default=True,
+            dest='disk_cache',
+            help="Cache data on the local filesystem (default)",
+        )
+        cachetype.add_argument(
+            '--ram-cache',
+            action='store_false',
+            default=True,
+            dest='disk_cache',
+            help="Cache data in memory",
+        )
+        cache.add_argument(
+            '--disk-cache-dir',
+            metavar="DIRECTORY",
+            help="Filesystem cache location (default `~/.cache/arvados/keep`)",
+        )
+        cache.add_argument(
+            '--directory-cache',
+            type=int,
+            default=128*1024*1024,
+            metavar='BYTES',
+            help="Size of directory data cache in bytes (default 128 MiB)",
+        )
+        cache.add_argument(
+            '--file-cache',
+            type=int,
+            default=0,
+            metavar='BYTES',
+            help="""
+Size of file data cache in bytes
+(default 8 GiB for filesystem cache, 256 MiB for memory cache)
+""",
+        )
+
+        plumbing = self.add_argument_group("Mount interactions with Arvados and Linux")
+        plumbing.add_argument(
+            '--disable-event-listening',
+            action='store_true',
+            dest='disable_event_listening',
+            default=False,
+            help="Don't subscribe to events on the API server to update mount contents",
+        )
+        plumbing.add_argument(
+            '--encoding',
+            default="utf-8",
+            help="""
+Filesystem character encoding
+(default %(default)r; specify a name from the Python codec registry)
+""",
+        )
+        plumbing.add_argument(
+            '--storage-classes',
+            metavar='CLASSES',
+            help="Comma-separated list of storage classes to request for new collections",
+        )
+        # This is a hidden argument used by tests.  Normally this
+        # value will be extracted from the cluster config, but mocking
+        # the cluster config under the presence of multiple threads
+        # and processes turned out to be too complicated and brittle.
+        plumbing.add_argument(
+            '--fsns',
+            type=str,
+            default=None,
+            help=argparse.SUPPRESS)
 
 class Mount(object):
     def __init__(self, args, logger=logging.getLogger('arvados.arv-mount')):
         self.daemon = False
         self.logger = logger
         self.args = args
         self.listen_for_events = False
@@ -250,29 +486,21 @@
             # default value of file_cache is 0, this tells KeepBlockCache to
             # choose a default based on whether disk_cache is enabled or not.
 
             block_cache = arvados.keep.KeepBlockCache(cache_max=self.args.file_cache,
                                                       disk_cache=self.args.disk_cache,
                                                       disk_cache_dir=self.args.disk_cache_dir)
 
-            # If there's too many prefetch threads and you
-            # max out the CPU, delivering data to the FUSE
-            # layer actually ends up being slower.
-            # Experimentally, capping 7 threads seems to
-            # be a sweet spot.
-            prefetch_threads = min(max((block_cache.cache_max // (64 * 1024 * 1024)) - 1, 1), 7)
-
             self.api = arvados.safeapi.ThreadSafeApiCache(
                 apiconfig=arvados.config.settings(),
                 api_params={
                     'num_retries': self.args.retries,
                 },
                 keep_params={
                     'block_cache': block_cache,
-                    'num_prefetch_threads': prefetch_threads,
                     'num_retries': self.args.retries,
                 },
                 version='v1',
             )
         except KeyError as e:
             self.logger.error("Missing environment: %s", e)
             exit(1)
@@ -282,29 +510,37 @@
     def _setup_mount(self):
         self.operations = Operations(
             os.getuid(),
             os.getgid(),
             api_client=self.api,
             encoding=self.args.encoding,
             inode_cache=InodeCache(cap=self.args.directory_cache),
-            enable_write=self.args.enable_write)
+            enable_write=self.args.enable_write,
+            fsns=self.args.fsns)
 
         if self.args.crunchstat_interval:
             statsthread = threading.Thread(
                 target=crunchstat.statlogger,
                 args=(self.args.crunchstat_interval,
                       self.api.keep,
                       self.operations))
             statsthread.daemon = True
             statsthread.start()
 
         usr = self.api.users().current().execute(num_retries=self.args.retries)
         now = time.time()
         dir_class = None
-        dir_args = [llfuse.ROOT_INODE, self.operations.inodes, self.api, self.args.retries, self.args.enable_write]
+        dir_args = [
+            llfuse.ROOT_INODE,
+            self.operations.inodes,
+            self.api,
+            self.args.retries,
+            self.args.enable_write,
+            self.args.filters,
+        ]
         mount_readme = False
 
         storage_classes = None
         if self.args.storage_classes is not None:
             storage_classes = self.args.storage_classes.replace(' ', '').split(',')
             self.logger.info("Storage classes requested for new collections: {}".format(', '.join(storage_classes)))
 
@@ -362,15 +598,19 @@
             else:
                 ent = dir_class(*dir_args, storage_classes=storage_classes)
             self.operations.inodes.add_entry(ent)
             self.listen_for_events = ent.want_event_subscribe()
             return
 
         e = self.operations.inodes.add_entry(Directory(
-            llfuse.ROOT_INODE, self.operations.inodes, self.api.config, self.args.enable_write))
+            llfuse.ROOT_INODE,
+            self.operations.inodes,
+            self.args.enable_write,
+            self.args.filters,
+        ))
         dir_args[0] = e.inode
 
         for name in self.args.mount_by_id:
             self._add_mount(e, name, MagicDirectory(*dir_args, pdh_only=False, storage_classes=storage_classes))
         for name in self.args.mount_by_pdh:
             self._add_mount(e, name, MagicDirectory(*dir_args, pdh_only=True))
         for name in self.args.mount_by_tag:
@@ -444,12 +684,13 @@
         except Exception as e:
             self.logger.exception('arv-mount: exception during mount: %s', e)
             exit(getattr(e, 'errno', 1))
         exit(0)
 
     def _llfuse_main(self):
         try:
-            llfuse.main()
+            llfuse.main(workers=10)
         except:
             llfuse.close(unmount=False)
             raise
+        self.operations.begin_shutdown()
         llfuse.close()
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse/crunchstat.py` & `arvados_fuse-2.7.2/arvados_fuse/crunchstat.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.1/arvados_fuse/fresh.py` & `arvados_fuse-2.7.2/arvados_fuse/fresh.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,25 +58,24 @@
     * Record Arvados uuid at the time the object is placed in the cache
 
     * Clear the object contents (invalidates the object)
 
     """
 
     __slots__ = ("_stale", "_poll", "_last_update", "_atime", "_poll_time", "use_count",
-                 "ref_count", "dead", "cache_size", "cache_uuid", "allow_attr_cache")
+                 "ref_count", "cache_size", "cache_uuid", "allow_attr_cache")
 
     def __init__(self):
         self._stale = True
         self._poll = False
         self._last_update = time.time()
         self._atime = time.time()
         self._poll_time = 60
         self.use_count = 0
         self.ref_count = 0
-        self.dead = False
         self.cache_size = 0
         self.cache_uuid = None
 
         # Can the kernel cache attributes?
         self.allow_attr_cache = True
 
     def invalidate(self):
@@ -121,25 +120,19 @@
         self.ref_count += 1
         return self.ref_count
 
     def dec_ref(self, n):
         self.ref_count -= n
         return self.ref_count
 
-    def has_ref(self, only_children):
+    def has_ref(self):
         """Determine if there are any kernel references to this
-        object or its children.
-
-        If only_children is True, ignore refcount of self and only consider
-        children.
+        object.
         """
-        if only_children:
-            return False
-        else:
-            return self.ref_count > 0
+        return self.ref_count > 0
 
     def objsize(self):
         return 0
 
     def uuid(self):
         return None
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse/fusedir.py` & `arvados_fuse-2.7.2/arvados_fuse/fusedir.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,46 +32,46 @@
 class Directory(FreshBase):
     """Generic directory object, backed by a dict.
 
     Consists of a set of entries with the key representing the filename
     and the value referencing a File or Directory object.
     """
 
-    def __init__(self, parent_inode, inodes, apiconfig, enable_write):
+    __slots__ = ("inode", "parent_inode", "inodes", "_entries", "_mtime", "_enable_write", "_filters")
+
+    def __init__(self, parent_inode, inodes, enable_write, filters):
         """parent_inode is the integer inode number"""
 
         super(Directory, self).__init__()
 
         self.inode = None
         if not isinstance(parent_inode, int):
             raise Exception("parent_inode should be an int")
         self.parent_inode = parent_inode
         self.inodes = inodes
-        self.apiconfig = apiconfig
         self._entries = {}
         self._mtime = time.time()
         self._enable_write = enable_write
+        self._filters = filters or []
 
-    def forward_slash_subst(self):
-        if not hasattr(self, '_fsns'):
-            self._fsns = None
-            config = self.apiconfig()
-            try:
-                self._fsns = config["Collections"]["ForwardSlashNameSubstitution"]
-            except KeyError:
-                # old API server with no FSNS config
-                self._fsns = '_'
+    def _filters_for(self, subtype, *, qualified):
+        for f in self._filters:
+            f_type, _, f_name = f[0].partition('.')
+            if not f_name:
+                yield f
+            elif f_type != subtype:
+                pass
+            elif qualified:
+                yield f
             else:
-                if self._fsns == '' or self._fsns == '/':
-                    self._fsns = None
-        return self._fsns
+                yield [f_name, *f[1:]]
 
     def unsanitize_filename(self, incoming):
         """Replace ForwardSlashNameSubstitution value with /"""
-        fsns = self.forward_slash_subst()
+        fsns = self.inodes.forward_slash_subst()
         if isinstance(fsns, str):
             return incoming.replace(fsns, '/')
         else:
             return incoming
 
     def sanitize_filename(self, dirty):
         """Replace disallowed filename characters according to
@@ -82,15 +82,15 @@
         elif dirty == '':
             return '_'
         elif dirty == '.':
             return '_'
         elif dirty == '..':
             return '__'
         else:
-            fsns = self.forward_slash_subst()
+            fsns = self.inodes.forward_slash_subst()
             if isinstance(fsns, str):
                 dirty = dirty.replace('/', fsns)
             return _disallowed_filename_characters.sub('_', dirty)
 
 
     #  Overridden by subclasses to implement logic to update the
     #  entries dict when the directory is stale
@@ -133,95 +133,114 @@
     def __len__(self):
         return len(self._entries)
 
     def fresh(self):
         self.inodes.touch(self)
         super(Directory, self).fresh()
 
+    def objsize(self):
+        # Rough estimate of memory footprint based on using pympler
+        return len(self._entries) * 1024
+
     def merge(self, items, fn, same, new_entry):
         """Helper method for updating the contents of the directory.
 
         Takes a list describing the new contents of the directory, reuse
         entries that are the same in both the old and new lists, create new
         entries, and delete old entries missing from the new list.
 
-        :items: iterable with new directory contents
+        Arguments:
+        * items: Iterable --- New directory contents
 
-        :fn: function to take an entry in 'items' and return the desired file or
+        * fn: Callable --- Takes an entry in 'items' and return the desired file or
         directory name, or None if this entry should be skipped
 
-        :same: function to compare an existing entry (a File or Directory
+        * same: Callable --- Compare an existing entry (a File or Directory
         object) with an entry in the items list to determine whether to keep
         the existing entry.
 
-        :new_entry: function to create a new directory entry (File or Directory
+        * new_entry: Callable --- Create a new directory entry (File or Directory
         object) from an entry in the items list.
 
         """
 
         oldentries = self._entries
         self._entries = {}
         changed = False
         for i in items:
             name = self.sanitize_filename(fn(i))
-            if name:
-                if name in oldentries and same(oldentries[name], i):
+            if not name:
+                continue
+            if name in oldentries:
+                ent = oldentries[name]
+                if same(ent, i) and ent.parent_inode == self.inode:
                     # move existing directory entry over
-                    self._entries[name] = oldentries[name]
+                    self._entries[name] = ent
                     del oldentries[name]
-                else:
-                    _logger.debug("Adding entry '%s' to inode %i", name, self.inode)
-                    # create new directory entry
-                    ent = new_entry(i)
-                    if ent is not None:
-                        self._entries[name] = self.inodes.add_entry(ent)
-                        changed = True
+                    self.inodes.inode_cache.touch(ent)
+
+        for i in items:
+            name = self.sanitize_filename(fn(i))
+            if not name:
+                continue
+            if name not in self._entries:
+                # create new directory entry
+                ent = new_entry(i)
+                if ent is not None:
+                    self._entries[name] = self.inodes.add_entry(ent)
+                    # need to invalidate this just in case there was a
+                    # previous entry that couldn't be moved over or a
+                    # lookup that returned file not found and cached
+                    # a negative result
+                    self.inodes.invalidate_entry(self, name)
+                    changed = True
+                _logger.debug("Added entry '%s' as inode %i to parent inode %i", name, ent.inode, self.inode)
 
         # delete any other directory entries that were not in found in 'items'
-        for i in oldentries:
-            _logger.debug("Forgetting about entry '%s' on inode %i", i, self.inode)
-            self.inodes.invalidate_entry(self, i)
-            self.inodes.del_entry(oldentries[i])
+        for name, ent in oldentries.items():
+            _logger.debug("Detaching entry '%s' from parent_inode %i", name, self.inode)
+            self.inodes.invalidate_entry(self, name)
+            self.inodes.del_entry(ent)
             changed = True
 
         if changed:
-            self.inodes.invalidate_inode(self)
             self._mtime = time.time()
+            self.inodes.inode_cache.update_cache_size(self)
 
         self.fresh()
 
     def in_use(self):
         if super(Directory, self).in_use():
             return True
         for v in self._entries.values():
             if v.in_use():
                 return True
         return False
 
-    def has_ref(self, only_children):
-        if super(Directory, self).has_ref(only_children):
-            return True
-        for v in self._entries.values():
-            if v.has_ref(False):
-                return True
-        return False
-
     def clear(self):
         """Delete all entries"""
+        if not self._entries:
+            return
         oldentries = self._entries
         self._entries = {}
-        for n in oldentries:
-            oldentries[n].clear()
-            self.inodes.del_entry(oldentries[n])
         self.invalidate()
+        for name, ent in oldentries.items():
+            ent.clear()
+            self.inodes.invalidate_entry(self, name)
+            self.inodes.del_entry(ent)
+        self.inodes.inode_cache.update_cache_size(self)
 
     def kernel_invalidate(self):
         # Invalidating the dentry on the parent implies invalidating all paths
         # below it as well.
-        parent = self.inodes[self.parent_inode]
+        if self.parent_inode in self.inodes:
+            parent = self.inodes[self.parent_inode]
+        else:
+            # parent was removed already.
+            return
 
         # Find self on the parent in order to invalidate this path.
         # Calling the public items() method might trigger a refresh,
         # which we definitely don't want, so read the internal dict directly.
         for k,v in parent._entries.items():
             if v is self:
                 self.inodes.invalidate_entry(parent, k)
@@ -266,32 +285,40 @@
     `Collection` object signals via a notify callback to
     `CollectionDirectoryBase.on_event` that an item was added, removed or
     modified.  FUSE inodes and directory entries are created, deleted or
     invalidated in response to these events.
 
     """
 
-    def __init__(self, parent_inode, inodes, apiconfig, enable_write, collection, collection_root):
-        super(CollectionDirectoryBase, self).__init__(parent_inode, inodes, apiconfig, enable_write)
-        self.apiconfig = apiconfig
+    __slots__ = ("collection", "collection_root", "collection_record_file")
+
+    def __init__(self, parent_inode, inodes, enable_write, filters, collection, collection_root):
+        super(CollectionDirectoryBase, self).__init__(parent_inode, inodes, enable_write, filters)
         self.collection = collection
         self.collection_root = collection_root
         self.collection_record_file = None
 
     def new_entry(self, name, item, mtime):
         name = self.sanitize_filename(name)
         if hasattr(item, "fuse_entry") and item.fuse_entry is not None:
-            if item.fuse_entry.dead is not True:
-                raise Exception("Can only reparent dead inode entry")
+            if item.fuse_entry.parent_inode is not None:
+                raise Exception("Can only reparent unparented inode entry")
             if item.fuse_entry.inode is None:
                 raise Exception("Reparented entry must still have valid inode")
-            item.fuse_entry.dead = False
+            item.fuse_entry.parent_inode = self.inode
             self._entries[name] = item.fuse_entry
         elif isinstance(item, arvados.collection.RichCollectionBase):
-            self._entries[name] = self.inodes.add_entry(CollectionDirectoryBase(self.inode, self.inodes, self.apiconfig, self._enable_write, item, self.collection_root))
+            self._entries[name] = self.inodes.add_entry(CollectionDirectoryBase(
+                self.inode,
+                self.inodes,
+                self._enable_write,
+                self._filters,
+                item,
+                self.collection_root,
+            ))
             self._entries[name].populate(mtime)
         else:
             self._entries[name] = self.inodes.add_entry(FuseArvadosFile(self.inode, item, mtime, self._enable_write))
         item.fuse_entry = self._entries[name]
 
     def on_event(self, event, collection, name, item):
         # These are events from the Collection object (ADD/DEL/MOD)
@@ -424,22 +451,31 @@
         with llfuse.lock_released:
             self.collection.rename(name_old, name_new, source_collection=src.collection, overwrite=True)
         self.flush()
         src.flush()
 
     def clear(self):
         super(CollectionDirectoryBase, self).clear()
+        if self.collection is not None:
+            self.collection.unsubscribe()
         self.collection = None
 
+    def objsize(self):
+        # objsize for the whole collection is represented at the root,
+        # don't double-count it
+        return 0
 
 class CollectionDirectory(CollectionDirectoryBase):
     """Represents the root of a directory tree representing a collection."""
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, collection_record=None, explicit_collection=None):
-        super(CollectionDirectory, self).__init__(parent_inode, inodes, api.config, enable_write, None, self)
+    __slots__ = ("api", "num_retries", "collection_locator",
+                 "_manifest_size", "_writable", "_updating_lock")
+
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters=None, collection_record=None, explicit_collection=None):
+        super(CollectionDirectory, self).__init__(parent_inode, inodes, enable_write, filters, None, self)
         self.api = api
         self.num_retries = num_retries
         self._poll = True
         try:
             self._poll_time = (api._rootDesc.get('blobSignatureTtl', 60*60*2) // 2)
         except:
             _logger.debug("Error getting blobSignatureTtl from discovery document: %s", sys.exc_info()[0])
@@ -489,15 +525,18 @@
             raise Exception("invalid new_collection_record")
         self._mtime = convertTime(new_collection_record.get('modified_at'))
         self._manifest_size = len(new_collection_record["manifest_text"])
         self.collection_locator = new_collection_record["uuid"]
         if self.collection_record_file is not None:
             self.collection_record_file.invalidate()
             self.inodes.invalidate_inode(self.collection_record_file)
-            _logger.debug("%s invalidated collection record file", self)
+            _logger.debug("parent_inode %s invalidated collection record file inode %s", self.inode,
+                          self.collection_record_file.inode)
+        self.inodes.update_uuid(self)
+        self.inodes.inode_cache.update_cache_size(self)
         self.fresh()
 
     def uuid(self):
         return self.collection_locator
 
     @use_counter
     def update(self):
@@ -567,14 +606,15 @@
             _logger.exception("arv-mount %s: error", self.collection_locator)
             if new_collection_record is not None and "manifest_text" in new_collection_record:
                 _logger.error("arv-mount manifest_text is: %s", new_collection_record["manifest_text"])
         self.invalidate()
         return False
 
     @use_counter
+    @check_update
     def collection_record(self):
         self.flush()
         return self.collection.api_response()
 
     @use_counter
     @check_update
     def __getitem__(self, item):
@@ -600,30 +640,40 @@
             self.inodes.invalidate_inode(self.collection_record_file)
         super(CollectionDirectory, self).invalidate()
 
     def persisted(self):
         return (self.collection_locator is not None)
 
     def objsize(self):
-        # This is an empirically-derived heuristic to estimate the memory used
-        # to store this collection's metadata.  Calculating the memory
-        # footprint directly would be more accurate, but also more complicated.
-        return self._manifest_size * 128
+        # This is a rough guess of the amount of overhead involved for
+        # a collection; the assumptions are that that each file
+        # averages 128 bytes in the manifest, but consume 1024 bytes
+        # of Python data structures, so 1024/128=8 means we estimate
+        # the RAM footprint at 8 times the size of bare manifest text.
+        return self._manifest_size * 8
 
     def finalize(self):
-        if self.collection is not None:
-            if self.writable():
+        if self.collection is None:
+            return
+
+        if self.writable():
+            try:
                 self.collection.save()
-            self.collection.stop_threads()
+            except Exception as e:
+                _logger.exception("Failed to save collection %s", self.collection_locator)
+        self.collection.stop_threads()
 
     def clear(self):
         if self.collection is not None:
             self.collection.stop_threads()
-        super(CollectionDirectory, self).clear()
         self._manifest_size = 0
+        super(CollectionDirectory, self).clear()
+        if self.collection_record_file is not None:
+            self.inodes.del_entry(self.collection_record_file)
+        self.collection_record_file = None
 
 
 class TmpCollectionDirectory(CollectionDirectoryBase):
     """A directory backed by an Arvados collection that never gets saved.
 
     This supports using Keep as scratch space. A userspace program can
     read the .arvados#collection file to get a current manifest in
@@ -633,24 +683,24 @@
 
     class UnsaveableCollection(arvados.collection.Collection):
         def save(self):
             pass
         def save_new(self):
             pass
 
-    def __init__(self, parent_inode, inodes, api_client, num_retries, enable_write, storage_classes=None):
+    def __init__(self, parent_inode, inodes, api_client, num_retries, enable_write, filters=None, storage_classes=None):
         collection = self.UnsaveableCollection(
             api_client=api_client,
             keep_client=api_client.keep,
             num_retries=num_retries,
             storage_classes_desired=storage_classes)
         # This is always enable_write=True because it never tries to
         # save to the backend
         super(TmpCollectionDirectory, self).__init__(
-            parent_inode, inodes, api_client.config, True, collection, self)
+            parent_inode, inodes, True, filters, collection, self)
         self.populate(self.mtime())
 
     def on_event(self, *args, **kwargs):
         super(TmpCollectionDirectory, self).on_event(*args, **kwargs)
         if self.collection_record_file is None:
             return
 
@@ -664,15 +714,15 @@
             pass
 
         try:
             with llfuse.lock:
                 with self.collection.lock:
                     self.collection_record_file.invalidate()
                     self.inodes.invalidate_inode(self.collection_record_file)
-                    _logger.debug("%s invalidated collection record", self)
+                    _logger.debug("%s invalidated collection record", self.inode)
         finally:
             while lockcount > 0:
                 self.collection.lock.acquire()
                 lockcount -= 1
 
     def collection_record(self):
         with llfuse.lock_released:
@@ -738,16 +788,16 @@
 Note that this directory will appear empty until you attempt to access a
 specific collection or project subdirectory (such as trying to 'cd' into it),
 at which point the collection or project will actually be looked up on the server
 and the directory will appear if it exists.
 
 """.lstrip()
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, pdh_only=False, storage_classes=None):
-        super(MagicDirectory, self).__init__(parent_inode, inodes, api.config, enable_write)
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters, pdh_only=False, storage_classes=None):
+        super(MagicDirectory, self).__init__(parent_inode, inodes, enable_write, filters)
         self.api = api
         self.num_retries = num_retries
         self.pdh_only = pdh_only
         self.storage_classes = storage_classes
 
     def __setattr__(self, name, value):
         super(MagicDirectory, self).__setattr__(name, value)
@@ -755,38 +805,63 @@
         if ((name == 'inode') and (self.inode is not None) and
               (not self._entries)):
             self._entries['README'] = self.inodes.add_entry(
                 StringFile(self.inode, self.README_TEXT, time.time()))
             # If we're the root directory, add an identical by_id subdirectory.
             if self.inode == llfuse.ROOT_INODE:
                 self._entries['by_id'] = self.inodes.add_entry(MagicDirectory(
-                    self.inode, self.inodes, self.api, self.num_retries, self._enable_write,
-                    self.pdh_only))
+                    self.inode,
+                    self.inodes,
+                    self.api,
+                    self.num_retries,
+                    self._enable_write,
+                    self._filters,
+                    self.pdh_only,
+                ))
 
     def __contains__(self, k):
         if k in self._entries:
             return True
 
         if not portable_data_hash_pattern.match(k) and (self.pdh_only or not uuid_pattern.match(k)):
             return False
 
         try:
             e = None
 
             if group_uuid_pattern.match(k):
                 project = self.api.groups().list(
-                    filters=[['group_class', 'in', ['project','filter']], ["uuid", "=", k]]).execute(num_retries=self.num_retries)
+                    filters=[
+                        ['group_class', 'in', ['project','filter']],
+                        ["uuid", "=", k],
+                        *self._filters_for('groups', qualified=False),
+                    ],
+                ).execute(num_retries=self.num_retries)
                 if project[u'items_available'] == 0:
                     return False
                 e = self.inodes.add_entry(ProjectDirectory(
-                    self.inode, self.inodes, self.api, self.num_retries, self._enable_write,
-                    project[u'items'][0], storage_classes=self.storage_classes))
+                    self.inode,
+                    self.inodes,
+                    self.api,
+                    self.num_retries,
+                    self._enable_write,
+                    self._filters,
+                    project[u'items'][0],
+                    storage_classes=self.storage_classes,
+                ))
             else:
                 e = self.inodes.add_entry(CollectionDirectory(
-                        self.inode, self.inodes, self.api, self.num_retries, self._enable_write, k))
+                    self.inode,
+                    self.inodes,
+                    self.api,
+                    self.num_retries,
+                    self._enable_write,
+                    self._filters,
+                    k,
+                ))
 
             if e.update():
                 if k not in self._entries:
                     self._entries[k] = e
                 else:
                     self.inodes.del_entry(e)
                 return True
@@ -812,47 +887,69 @@
     def want_event_subscribe(self):
         return not self.pdh_only
 
 
 class TagsDirectory(Directory):
     """A special directory that contains as subdirectories all tags visible to the user."""
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, poll_time=60):
-        super(TagsDirectory, self).__init__(parent_inode, inodes, api.config, enable_write)
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters, poll_time=60):
+        super(TagsDirectory, self).__init__(parent_inode, inodes, enable_write, filters)
         self.api = api
         self.num_retries = num_retries
         self._poll = True
         self._poll_time = poll_time
         self._extra = set()
 
     def want_event_subscribe(self):
         return True
 
     @use_counter
     def update(self):
         with llfuse.lock_released:
             tags = self.api.links().list(
-                filters=[['link_class', '=', 'tag'], ["name", "!=", ""]],
-                select=['name'], distinct=True, limit=1000
-                ).execute(num_retries=self.num_retries)
+                filters=[
+                    ['link_class', '=', 'tag'],
+                    ['name', '!=', ''],
+                    *self._filters_for('links', qualified=False),
+                ],
+                select=['name'],
+                distinct=True,
+                limit=1000,
+            ).execute(num_retries=self.num_retries)
         if "items" in tags:
-            self.merge(tags['items']+[{"name": n} for n in self._extra],
-                       lambda i: i['name'],
-                       lambda a, i: a.tag == i['name'],
-                       lambda i: TagDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write,
-                                              i['name'], poll=self._poll, poll_time=self._poll_time))
+            self.merge(
+                tags['items']+[{"name": n} for n in self._extra],
+                lambda i: i['name'],
+                lambda a, i: a.tag == i['name'],
+                lambda i: TagDirectory(
+                    self.inode,
+                    self.inodes,
+                    self.api,
+                    self.num_retries,
+                    self._enable_write,
+                    self._filters,
+                    i['name'],
+                    poll=self._poll,
+                    poll_time=self._poll_time,
+                ),
+            )
 
     @use_counter
     @check_update
     def __getitem__(self, item):
         if super(TagsDirectory, self).__contains__(item):
             return super(TagsDirectory, self).__getitem__(item)
         with llfuse.lock_released:
             tags = self.api.links().list(
-                filters=[['link_class', '=', 'tag'], ['name', '=', item]], limit=1
+                filters=[
+                    ['link_class', '=', 'tag'],
+                    ['name', '=', item],
+                    *self._filters_for('links', qualified=False),
+                ],
+                limit=1,
             ).execute(num_retries=self.num_retries)
         if tags["items"]:
             self._extra.add(item)
             self.update()
         return super(TagsDirectory, self).__getitem__(item)
 
     @use_counter
@@ -869,71 +966,101 @@
 
 
 class TagDirectory(Directory):
     """A special directory that contains as subdirectories all collections visible
     to the user that are tagged with a particular tag.
     """
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, tag,
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters, tag,
                  poll=False, poll_time=60):
-        super(TagDirectory, self).__init__(parent_inode, inodes, api.config, enable_write)
+        super(TagDirectory, self).__init__(parent_inode, inodes, enable_write, filters)
         self.api = api
         self.num_retries = num_retries
         self.tag = tag
         self._poll = poll
         self._poll_time = poll_time
 
     def want_event_subscribe(self):
         return True
 
     @use_counter
     def update(self):
         with llfuse.lock_released:
             taggedcollections = self.api.links().list(
-                filters=[['link_class', '=', 'tag'],
-                         ['name', '=', self.tag],
-                         ['head_uuid', 'is_a', 'arvados#collection']],
-                select=['head_uuid']
-                ).execute(num_retries=self.num_retries)
-        self.merge(taggedcollections['items'],
-                   lambda i: i['head_uuid'],
-                   lambda a, i: a.collection_locator == i['head_uuid'],
-                   lambda i: CollectionDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write, i['head_uuid']))
+                filters=[
+                    ['link_class', '=', 'tag'],
+                    ['name', '=', self.tag],
+                    ['head_uuid', 'is_a', 'arvados#collection'],
+                    *self._filters_for('links', qualified=False),
+                ],
+                select=['head_uuid'],
+            ).execute(num_retries=self.num_retries)
+        self.merge(
+            taggedcollections['items'],
+            lambda i: i['head_uuid'],
+            lambda a, i: a.collection_locator == i['head_uuid'],
+            lambda i: CollectionDirectory(
+                self.inode,
+                self.inodes,
+                self.api,
+                self.num_retries,
+                self._enable_write,
+                self._filters,
+                i['head_uuid'],
+            ),
+        )
 
 
 class ProjectDirectory(Directory):
     """A special directory that contains the contents of a project."""
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, project_object,
-                 poll=True, poll_time=3, storage_classes=None):
-        super(ProjectDirectory, self).__init__(parent_inode, inodes, api.config, enable_write)
+    __slots__ = ("api", "num_retries", "project_object", "project_object_file",
+                 "project_uuid", "_updating_lock",
+                 "_current_user", "_full_listing", "storage_classes", "recursively_contained")
+
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters,
+                 project_object, poll=True, poll_time=3, storage_classes=None):
+        super(ProjectDirectory, self).__init__(parent_inode, inodes, enable_write, filters)
         self.api = api
         self.num_retries = num_retries
         self.project_object = project_object
         self.project_object_file = None
         self.project_uuid = project_object['uuid']
         self._poll = poll
         self._poll_time = poll_time
         self._updating_lock = threading.Lock()
         self._current_user = None
         self._full_listing = False
         self.storage_classes = storage_classes
+        self.recursively_contained = False
+
+        # Filter groups can contain themselves, which causes tools
+        # that walk the filesystem to get stuck in an infinite loop,
+        # so suppress returning a listing in that case.
+        if self.project_object.get("group_class") == "filter":
+            iter_parent_inode = parent_inode
+            while iter_parent_inode != llfuse.ROOT_INODE:
+                parent_dir = self.inodes[iter_parent_inode]
+                if isinstance(parent_dir, ProjectDirectory) and parent_dir.project_uuid == self.project_uuid:
+                    self.recursively_contained = True
+                    break
+                iter_parent_inode = parent_dir.parent_inode
 
     def want_event_subscribe(self):
         return True
 
     def createDirectory(self, i):
+        common_args = (self.inode, self.inodes, self.api, self.num_retries, self._enable_write, self._filters)
         if collection_uuid_pattern.match(i['uuid']):
-            return CollectionDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write, i)
+            return CollectionDirectory(*common_args, i)
         elif group_uuid_pattern.match(i['uuid']):
-            return ProjectDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write,
-                                    i, self._poll, self._poll_time, self.storage_classes)
+            return ProjectDirectory(*common_args, i, self._poll, self._poll_time, self.storage_classes)
         elif link_uuid_pattern.match(i['uuid']):
             if i['head_kind'] == 'arvados#collection' or portable_data_hash_pattern.match(i['head_uuid']):
-                return CollectionDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write, i['head_uuid'])
+                return CollectionDirectory(*common_args, i['head_uuid'])
             else:
                 return None
         elif uuid_pattern.match(i['uuid']):
             return ObjectFile(self.parent_inode, i)
         else:
             return None
 
@@ -963,15 +1090,15 @@
 
     @use_counter
     def update(self):
         if self.project_object_file == None:
             self.project_object_file = ObjectFile(self.inode, self.project_object)
             self.inodes.add_entry(self.project_object_file)
 
-        if not self._full_listing:
+        if self.recursively_contained or not self._full_listing:
             return True
 
         def samefn(a, i):
             if isinstance(a, CollectionDirectory) or isinstance(a, ProjectDirectory):
                 return a.uuid() == i['uuid']
             elif isinstance(a, ObjectFile):
                 return a.uuid() == i['uuid'] and not a.stale()
@@ -986,28 +1113,35 @@
                 if group_uuid_pattern.match(self.project_uuid):
                     self.project_object = self.api.groups().get(
                         uuid=self.project_uuid).execute(num_retries=self.num_retries)
                 elif user_uuid_pattern.match(self.project_uuid):
                     self.project_object = self.api.users().get(
                         uuid=self.project_uuid).execute(num_retries=self.num_retries)
                 # do this in 2 steps until #17424 is fixed
-                contents = list(arvados.util.keyset_list_all(self.api.groups().contents,
-                                                        order_key="uuid",
-                                                        num_retries=self.num_retries,
-                                                        uuid=self.project_uuid,
-                                                        filters=[["uuid", "is_a", "arvados#group"],
-                                                                 ["groups.group_class", "in", ["project","filter"]]]))
-                contents.extend(filter(lambda i: i["current_version_uuid"] == i["uuid"],
-                                       arvados.util.keyset_list_all(self.api.groups().contents,
-                                                             order_key="uuid",
-                                                             num_retries=self.num_retries,
-                                                             uuid=self.project_uuid,
-                                                             filters=[["uuid", "is_a", "arvados#collection"]])))
-
-
+                contents = list(arvados.util.keyset_list_all(
+                    self.api.groups().contents,
+                    order_key='uuid',
+                    num_retries=self.num_retries,
+                    uuid=self.project_uuid,
+                    filters=[
+                        ['uuid', 'is_a', 'arvados#group'],
+                        ['groups.group_class', 'in', ['project', 'filter']],
+                        *self._filters_for('groups', qualified=True),
+                    ],
+                ))
+                contents.extend(obj for obj in arvados.util.keyset_list_all(
+                    self.api.groups().contents,
+                    order_key='uuid',
+                    num_retries=self.num_retries,
+                    uuid=self.project_uuid,
+                    filters=[
+                        ['uuid', 'is_a', 'arvados#collection'],
+                        *self._filters_for('collections', qualified=True),
+                    ],
+                ) if obj['current_version_uuid'] == obj['uuid'])
             # end with llfuse.lock_released, re-acquire lock
 
             self.merge(contents,
                        self.namefn,
                        samefn,
                        self.createDirectory)
             return True
@@ -1028,22 +1162,32 @@
             return super(ProjectDirectory, self).__getitem__(k)
         with llfuse.lock_released:
             k2 = self.unsanitize_filename(k)
             if k2 == k:
                 namefilter = ["name", "=", k]
             else:
                 namefilter = ["name", "in", [k, k2]]
-            contents = self.api.groups().list(filters=[["owner_uuid", "=", self.project_uuid],
-                                                       ["group_class", "in", ["project","filter"]],
-                                                       namefilter],
-                                              limit=2).execute(num_retries=self.num_retries)["items"]
+            contents = self.api.groups().list(
+                filters=[
+                    ["owner_uuid", "=", self.project_uuid],
+                    ["group_class", "in", ["project","filter"]],
+                    namefilter,
+                    *self._filters_for('groups', qualified=False),
+                ],
+                limit=2,
+            ).execute(num_retries=self.num_retries)["items"]
             if not contents:
-                contents = self.api.collections().list(filters=[["owner_uuid", "=", self.project_uuid],
-                                                                namefilter],
-                                                       limit=2).execute(num_retries=self.num_retries)["items"]
+                contents = self.api.collections().list(
+                    filters=[
+                        ["owner_uuid", "=", self.project_uuid],
+                        namefilter,
+                        *self._filters_for('collections', qualified=False),
+                    ],
+                    limit=2,
+                ).execute(num_retries=self.num_retries)["items"]
         if contents:
             if len(contents) > 1 and contents[1]['name'] == k:
                 # If "foo/bar" and "foo[SUBST]bar" both exist, use
                 # "foo[SUBST]bar".
                 contents = [contents[1]]
             name = self.sanitize_filename(self.namefn(contents[0]))
             if name != k:
@@ -1072,14 +1216,20 @@
             if not self._current_user:
                 self._current_user = self.api.users().current().execute(num_retries=self.num_retries)
             return self._current_user["uuid"] in self.project_object.get("writable_by", [])
 
     def persisted(self):
         return True
 
+    def clear(self):
+        super(ProjectDirectory, self).clear()
+        if self.project_object_file is not None:
+            self.inodes.del_entry(self.project_object_file)
+        self.project_object_file = None
+
     @use_counter
     @check_update
     def mkdir(self, name):
         if not self.writable():
             raise llfuse.FUSEError(errno.EROFS)
 
         try:
@@ -1189,17 +1339,17 @@
             elif ent is not None:
                 self.inodes.del_entry(ent)
 
 
 class SharedDirectory(Directory):
     """A special directory that represents users or groups who have shared projects with me."""
 
-    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, exclude,
-                 poll=False, poll_time=60, storage_classes=None):
-        super(SharedDirectory, self).__init__(parent_inode, inodes, api.config, enable_write)
+    def __init__(self, parent_inode, inodes, api, num_retries, enable_write, filters,
+                 exclude, poll=False, poll_time=60, storage_classes=None):
+        super(SharedDirectory, self).__init__(parent_inode, inodes, enable_write, filters)
         self.api = api
         self.num_retries = num_retries
         self.current_user = api.users().current().execute(num_retries=num_retries)
         self._poll = True
         self._poll_time = poll_time
         self._updating_lock = threading.Lock()
         self.storage_classes = storage_classes
@@ -1217,55 +1367,72 @@
                 root_owners = set()
                 objects = {}
 
                 methods = self.api._rootDesc.get('resources')["groups"]['methods']
                 if 'httpMethod' in methods.get('shared', {}):
                     page = []
                     while True:
-                        resp = self.api.groups().shared(filters=[['group_class', 'in', ['project','filter']]]+page,
-                                                        order="uuid",
-                                                        limit=10000,
-                                                        count="none",
-                                                        include="owner_uuid").execute()
+                        resp = self.api.groups().shared(
+                            filters=[
+                                ['group_class', 'in', ['project','filter']],
+                                *page,
+                                *self._filters_for('groups', qualified=False),
+                            ],
+                            order="uuid",
+                            limit=10000,
+                            count="none",
+                            include="owner_uuid",
+                        ).execute()
                         if not resp["items"]:
                             break
                         page = [["uuid", ">", resp["items"][len(resp["items"])-1]["uuid"]]]
                         for r in resp["items"]:
                             objects[r["uuid"]] = r
                             roots.append(r["uuid"])
                         for r in resp["included"]:
                             objects[r["uuid"]] = r
                             root_owners.add(r["uuid"])
                 else:
                     all_projects = list(arvados.util.keyset_list_all(
                         self.api.groups().list,
                         order_key="uuid",
                         num_retries=self.num_retries,
-                        filters=[['group_class','in',['project','filter']]],
-                        select=["uuid", "owner_uuid"]))
+                        filters=[
+                            ['group_class', 'in', ['project','filter']],
+                            *self._filters_for('groups', qualified=False),
+                        ],
+                        select=["uuid", "owner_uuid"],
+                    ))
                     for ob in all_projects:
                         objects[ob['uuid']] = ob
 
                     current_uuid = self.current_user['uuid']
                     for ob in all_projects:
                         if ob['owner_uuid'] != current_uuid and ob['owner_uuid'] not in objects:
                             roots.append(ob['uuid'])
                             root_owners.add(ob['owner_uuid'])
 
                     lusers = arvados.util.keyset_list_all(
                         self.api.users().list,
                         order_key="uuid",
                         num_retries=self.num_retries,
-                        filters=[['uuid','in', list(root_owners)]])
+                        filters=[
+                            ['uuid', 'in', list(root_owners)],
+                            *self._filters_for('users', qualified=False),
+                        ],
+                    )
                     lgroups = arvados.util.keyset_list_all(
                         self.api.groups().list,
                         order_key="uuid",
                         num_retries=self.num_retries,
-                        filters=[['uuid','in', list(root_owners)+roots]])
-
+                        filters=[
+                            ['uuid', 'in', list(root_owners)+roots],
+                            *self._filters_for('groups', qualified=False),
+                        ],
+                    )
                     for l in lusers:
                         objects[l["uuid"]] = l
                     for l in lgroups:
                         objects[l["uuid"]] = l
 
                 for r in root_owners:
                     if r in objects:
@@ -1279,19 +1446,31 @@
                     if r in objects:
                         obr = objects[r]
                         if obr['owner_uuid'] not in objects:
                             contents[obr["name"]] = obr
 
             # end with llfuse.lock_released, re-acquire lock
 
-            self.merge(contents.items(),
-                       lambda i: i[0],
-                       lambda a, i: a.uuid() == i[1]['uuid'],
-                       lambda i: ProjectDirectory(self.inode, self.inodes, self.api, self.num_retries, self._enable_write,
-                                                  i[1], poll=self._poll, poll_time=self._poll_time, storage_classes=self.storage_classes))
+            self.merge(
+                contents.items(),
+                lambda i: i[0],
+                lambda a, i: a.uuid() == i[1]['uuid'],
+                lambda i: ProjectDirectory(
+                    self.inode,
+                    self.inodes,
+                    self.api,
+                    self.num_retries,
+                    self._enable_write,
+                    self._filters,
+                    i[1],
+                    poll=self._poll,
+                    poll_time=self._poll_time,
+                    storage_classes=self.storage_classes,
+                ),
+            )
         except Exception:
             _logger.exception("arv-mount shared dir error")
         finally:
             self._updating_lock.release()
 
     def want_event_subscribe(self):
         return True
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse/fusefile.py` & `arvados_fuse-2.7.2/arvados_fuse/fusefile.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,31 +76,41 @@
         return self._enable_write and self.arvfile.writable()
 
     def flush(self):
         with llfuse.lock_released:
             if self.writable():
                 self.arvfile.parent.root_collection().save()
 
+    def clear(self):
+        if self.parent_inode is None:
+            self.arvfile.fuse_entry = None
+            self.arvfile = None
+
 
 class StringFile(File):
     """Wrap a simple string as a file"""
+
+    __slots__ = ("contents",)
+
     def __init__(self, parent_inode, contents, _mtime):
         super(StringFile, self).__init__(parent_inode, _mtime)
         self.contents = contents
 
     def size(self):
         return len(self.contents)
 
     def readfrom(self, off, size, num_retries=0):
         return bytes(self.contents[off:(off+size)], encoding='utf-8')
 
 
 class ObjectFile(StringFile):
     """Wrap a dict as a serialized json object."""
 
+    __slots__ = ("object_uuid",)
+
     def __init__(self, parent_inode, obj):
         super(ObjectFile, self).__init__(parent_inode, "", 0)
         self.object_uuid = obj['uuid']
         self.update(obj)
 
     def uuid(self):
         return self.object_uuid
@@ -121,14 +131,17 @@
 
 class FuncToJSONFile(StringFile):
     """File content is the return value of a given function, encoded as JSON.
 
     The function is called at the time the file is read. The result is
     cached until invalidate() is called.
     """
+
+    __slots__ = ("func",)
+
     def __init__(self, parent_inode, func):
         super(FuncToJSONFile, self).__init__(parent_inode, "", 0)
         self.func = func
 
         # invalidate_inode() is asynchronous with no callback to wait for. In
         # order to guarantee userspace programs don't get stale data that was
         # generated before the last invalidate(), we must disallow inode
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse/unmount.py` & `arvados_fuse-2.7.2/arvados_fuse/unmount.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,14 +150,24 @@
             # calling realpath(); and (2) the specified path is not a
             # mount point (e.g., it was already unmounted by someone
             # else, or it's a typo), and realpath() can determine that
             # without hitting any other unresponsive mounts.
             path = os.path.realpath(path)
             continue
         elif not mounted:
+            if was_mounted:
+                # This appears to avoid a race condition where we
+                # return control to the caller after running
+                # "fusermount -u -z" (see below), the caller (e.g.,
+                # arv-mount --replace) immediately tries to attach a
+                # new fuse mount at the same mount point, the
+                # lazy-unmount process unmounts that _new_ mount while
+                # it is being initialized, and the setup code waits
+                # forever for the new mount to be initialized.
+                time.sleep(1)
             return was_mounted
 
         if attempted:
             # Report buffered stderr from previous call to fusermount,
             # now that we know it didn't succeed.
             sys.stderr.buffer.write(fusermount_output)
```

### Comparing `arvados_fuse-2.7.1/arvados_fuse.egg-info/PKG-INFO` & `arvados_fuse-2.7.2/arvados_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-fuse
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.7.1/arvados_version.py` & `arvados_fuse-2.7.2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.7.1/setup.py` & `arvados_fuse-2.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         'bin/arv-mount'
         ],
       data_files=[
           ('share/doc/arvados_fuse', ['agpl-3.0.txt', 'README.rst']),
       ],
       install_requires=[
         'arvados-python-client{}'.format(pysdk_dep),
-        'llfuse >= 1.3.6',
+        'arvados-llfuse >= 1.5.1',
         'future',
         'python-daemon',
         'ciso8601 >= 2.0.0',
         'setuptools',
         "prometheus_client"
         ],
       extras_require={
```

