# Comparing `tmp/dogma-data-0.2.1.tar.gz` & `tmp/dogma-data-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogma-data-0.2.1.tar", last modified: Sun Apr  7 01:44:21 2024, max compression
+gzip compressed data, was "dogma-data-0.2.3.tar", last modified: Tue Apr  9 06:17:29 2024, max compression
```

## Comparing `dogma-data-0.2.1.tar` & `dogma-data-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-07 01:44:21.898805 dogma-data-0.2.1/
--rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-07 01:44:21.894805 dogma-data-0.2.1/PKG-INFO
--rw-r--r--   0 roed     (23269) users      (100)        0 2024-03-30 18:11:44.000000 dogma-data-0.2.1/README.md
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-07 01:44:21.894805 dogma-data-0.2.1/dogma_data/
--rw-r--r--   0 roed     (23269) users      (100)      234 2024-04-02 00:14:48.000000 dogma-data-0.2.1/dogma_data/__init__.py
--rw-r--r--   0 roed     (23269) users      (100)    10913 2024-04-07 01:41:56.000000 dogma-data-0.2.1/dogma_data/dogma_data.py
--rw-r--r--   0 roed     (23269) users      (100)      450 2024-04-02 00:00:59.000000 dogma-data-0.2.1/dogma_data/dogma_torch.py
--rw-r--r--   0 roed     (23269) users      (100)     6063 2024-04-03 01:56:05.000000 dogma-data-0.2.1/dogma_data/fasta.py
--rw-r--r--   0 roed     (23269) users      (100)      762 2024-03-31 04:28:41.000000 dogma-data-0.2.1/dogma_data/utils.py
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-07 01:44:21.894805 dogma-data-0.2.1/dogma_data.egg-info/
--rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-07 01:44:21.000000 dogma-data-0.2.1/dogma_data.egg-info/PKG-INFO
--rw-r--r--   0 roed     (23269) users      (100)      307 2024-04-07 01:44:21.000000 dogma-data-0.2.1/dogma_data.egg-info/SOURCES.txt
--rw-r--r--   0 roed     (23269) users      (100)        1 2024-04-07 01:44:21.000000 dogma-data-0.2.1/dogma_data.egg-info/dependency_links.txt
--rw-r--r--   0 roed     (23269) users      (100)       98 2024-04-07 01:44:21.000000 dogma-data-0.2.1/dogma_data.egg-info/requires.txt
--rw-r--r--   0 roed     (23269) users      (100)       11 2024-04-07 01:44:21.000000 dogma-data-0.2.1/dogma_data.egg-info/top_level.txt
--rw-r--r--   0 roed     (23269) users      (100)     1015 2024-04-07 01:43:52.000000 dogma-data-0.2.1/pyproject.toml
--rw-r--r--   0 roed     (23269) users      (100)       38 2024-04-07 01:44:21.898805 dogma-data-0.2.1/setup.cfg
+drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.084868 dogma-data-0.2.3/
+-rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-09 06:17:29.084868 dogma-data-0.2.3/PKG-INFO
+-rw-r--r--   0 roed     (23269) users      (100)        0 2024-03-30 18:11:44.000000 dogma-data-0.2.3/README.md
+drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.080868 dogma-data-0.2.3/dogma_data/
+-rw-r--r--   0 roed     (23269) users      (100)      235 2024-04-08 20:03:17.000000 dogma-data-0.2.3/dogma_data/__init__.py
+-rw-r--r--   0 roed     (23269) users      (100)    10688 2024-04-09 06:15:25.000000 dogma-data-0.2.3/dogma_data/_dogma_data.py
+-rw-r--r--   0 roed     (23269) users      (100)      450 2024-04-02 00:00:59.000000 dogma-data-0.2.3/dogma_data/dogma_torch.py
+-rw-r--r--   0 roed     (23269) users      (100)     7035 2024-04-08 23:40:28.000000 dogma-data-0.2.3/dogma_data/fasta.py
+-rw-r--r--   0 roed     (23269) users      (100)      762 2024-03-31 04:28:41.000000 dogma-data-0.2.3/dogma_data/utils.py
+drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.084868 dogma-data-0.2.3/dogma_data.egg-info/
+-rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/PKG-INFO
+-rw-r--r--   0 roed     (23269) users      (100)      308 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/SOURCES.txt
+-rw-r--r--   0 roed     (23269) users      (100)        1 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/dependency_links.txt
+-rw-r--r--   0 roed     (23269) users      (100)       98 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/requires.txt
+-rw-r--r--   0 roed     (23269) users      (100)       11 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/top_level.txt
+-rw-r--r--   0 roed     (23269) users      (100)     1078 2024-04-09 06:17:20.000000 dogma-data-0.2.3/pyproject.toml
+-rw-r--r--   0 roed     (23269) users      (100)       38 2024-04-09 06:17:29.084868 dogma-data-0.2.3/setup.cfg
```

### Comparing `dogma-data-0.2.1/PKG-INFO` & `dogma-data-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.1
+Version: 0.2.3
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dogma-data-0.2.1/dogma_data/dogma_data.py` & `dogma-data-0.2.3/dogma_data/_dogma_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 import awkward as ak
 
 from numba import njit, prange
 
 from dogma_data.utils import check_equality, timer, ceildiv
 from smart_open import open as smart_open
 
-import os
-os.environ['EXTRA_CLING_ARGS'] = '-O3'
+from dogma_rust import awkward_from_list_of_numpy
 
-import cppyy
+# import os
+# os.environ['EXTRA_CLING_ARGS'] = '-O3'
 
-cppyy.add_include_path(np.get_include())
-cppyy.include(Path(__file__).parents[1] / "cpp_functions.hpp")
+# import cppyy
 
+# cppyy.add_include_path(np.get_include())
+# cppyy.include(Path(__file__).parents[1] / "cpp_functions.hpp")
 
-from cppyy.gbl import get_all_array_lengths, concatenate_arrays
 
 def _merge_cu_seqlens(cu_seqlens_l: list[np.ndarray]):
     i = 0
     ready_to_merge = [cu_seqlens_l[0]]
     while i < len(cu_seqlens_l) - 1:
         current = ready_to_merge[-1]
         next = cu_seqlens_l[i + 1][1:]  # Skip the first zero, since it's implied by the final element of the previous array
@@ -171,20 +171,15 @@
 #             stop = cu_seqlens[i + 1]
 #             all_tokens[start:stop] = all_rows[i]
 
 def make_random_access_buffer(all_rows: list[np.ndarray]):
     if all_rows[0].dtype != np.uint8:
         raise NotImplementedError('Only uint8 arrays are currently implemented. If you need any other types, please open an issue in the GitHub repository.')
     num_sequences = len(all_rows)
-    seqlens_out = np.zeros(num_sequences, dtype=np.int64)
-    with timer('get_all_array_lengths'):
-        get_all_array_lengths(all_rows, seqlens_out)
-    cu_seqlens = np.empty(num_sequences + 1, dtype=np.int64)
-    cu_seqlens[0] = 0
-    cu_seqlens[1:] = np.cumsum(seqlens_out)
+    all_tokens, cu_seqlens = concatenate_arrays(all_rows)
     assert len(cu_seqlens) == num_sequences + 1
 
     all_tokens = np.zeros(cu_seqlens[-1], dtype=all_rows[0].dtype)
     with timer('concat'):
         concatenate_arrays(all_rows, cu_seqlens.data, all_tokens.data)
     return all_tokens, cu_seqlens
```

### Comparing `dogma-data-0.2.1/dogma_data/fasta.py` & `dogma-data-0.2.3/dogma_data/fasta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,140 @@
 from typing import Any
 
 import numba as nb
 from numba.typed import List
 import awkward as ak
 import numpy as np
 from dogma_data.utils import ceildiv
+import dogma_rust
 
 
-
-@nb.njit(fastmath=True)
-def _parse_fasta_line(line: str, out_view: np.ndarray, mappings: np.ndarray):
-    for i, c in enumerate(line):
-        if c == 'A':
-            out_view[i] = mappings[0]
-        elif c == 'T':
-            out_view[i] = mappings[1]
-        elif c == 'C':
-            out_view[i] = mappings[2]
-        elif c == 'G':
-            out_view[i] = mappings[3]
-        elif c == 'U' or c == 'R' or c == 'Y' or c == 'K' or c == 'M' or c == 'S' or c == 'W' or c == 'B' or c == 'D' or c == 'H' or c == 'V' or c == 'N':
-            out_view[i] = mappings[4]
-        else:
-            out_view[i] = mappings[4]
-        # else:
-        #     raise ValueError(f"Invalid character {c} in fasta sequence")
-
-@nb.njit(parallel=True, fastmath=True)
-def _parse_fasta(complete_file: str, mappings: np.ndarray):
-    to_next_line = False
-    # [(start_file_index, end_file_index, cu_buffer_idx)]
-    # First find all the sequences to parse
-    total_len = len(complete_file)
-    n_threads = nb.config.NUMBA_DEFAULT_NUM_THREADS
-    if len(complete_file) < 10_000:
-        n_threads = 1
-    chunk_size = ceildiv(total_len, n_threads)
-
-    thread_buffer_sizes = [0 for _ in range(n_threads)]
-    thread_cu_seqlenss = List(nb.int64[:, :])# [np.array([], dtype=np.int64) for _ in range(n_threads)]
-    for _ in range(n_threads):
-        thread_cu_seqlenss.append(np.array([1, 2], dtype=np.int64))
-
-    for t in nb.prange(n_threads):
-        start_idx = t * chunk_size
-        end_idx = min((t + 1) * chunk_size, total_len)
-        while complete_file[start_idx] != '>':  # Scan until the first header
-            start_idx += 1
-        if t != n_threads - 1:
-            while complete_file[end_idx] != '>':  # Scan until the next header or until end of file
-                if end_idx == total_len - 1:
-                    break
-                end_idx += 1
+# @nb.njit(fastmath=True)
+# def _parse_fasta_line(line: str, out_view: np.ndarray, mappings: np.ndarray):
+#     for i, c in enumerate(line):
+#         if c == 'A':
+#             out_view[i] = mappings[0]
+#         elif c == 'T':
+#             out_view[i] = mappings[1]
+#         elif c == 'C':
+#             out_view[i] = mappings[2]
+#         elif c == 'G':
+#             out_view[i] = mappings[3]
+#         elif c == 'U' or c == 'R' or c == 'Y' or c == 'K' or c == 'M' or c == 'S' or c == 'W' or c == 'B' or c == 'D' or c == 'H' or c == 'V' or c == 'N':
+#             out_view[i] = mappings[4]
+#         else:
+#             out_view[i] = mappings[4]
+#         # else:
+#         #     raise ValueError(f"Invalid character {c} in fasta sequence")
+
+# @nb.njit(parallel=True, fastmath=True)
+# def _parse_fasta(complete_file: str, mappings: np.ndarray):
+#     to_next_line = False
+#     # [(start_file_index, end_file_index, cu_buffer_idx)]
+#     # First find all the sequences to parse
+#     total_len = len(complete_file)
+#     n_threads = nb.config.NUMBA_DEFAULT_NUM_THREADS
+#     if len(complete_file) < 10_000:
+#         n_threads = 1
+#     chunk_size = ceildiv(total_len, n_threads)
+
+#     thread_buffer_sizes = [0 for _ in range(n_threads)]
+#     thread_cu_seqlenss = List(nb.int64[:, :])# [np.array([], dtype=np.int64) for _ in range(n_threads)]
+#     for _ in range(n_threads):
+#         thread_cu_seqlenss.append(np.array([1, 2], dtype=np.int64))
+
+#     for t in nb.prange(n_threads):
+#         start_idx = t * chunk_size
+#         end_idx = min((t + 1) * chunk_size, total_len)
+#         while complete_file[start_idx] != '>':  # Scan until the first header
+#             start_idx += 1
+#         if t != n_threads - 1:
+#             while complete_file[end_idx] != '>':  # Scan until the next header or until end of file
+#                 if end_idx == total_len - 1:
+#                     break
+#                 end_idx += 1
             
-        thread_out_sequences = List()
-        thread_buffer_size = 0
+#         thread_out_sequences = List()
+#         thread_buffer_size = 0
 
-        current_start = 0
-        for i in range(start_idx, end_idx):
-            c = complete_file[i]
-            if to_next_line:
-                if c == '\n' or i == len(complete_file) - 1:
-                    if current_start != -1:
-                        thread_out_sequences.append((current_start, i, thread_buffer_size))
-                        thread_buffer_size += i - current_start
-                    to_next_line = False
-                continue
-            if c == '>':
-                # Potentially parse the header
-                to_next_line = True
-                current_start = -1
-                continue
-            else:
-                current_start = i
-                to_next_line = True
-
-        out_buffer = np.zeros(thread_buffer_size, dtype=np.uint8)
-        seqlens = np.zeros(len(thread_out_sequences), dtype=np.int64)
-        for i in nb.prange(len(thread_out_sequences)):
-            start, end, buffer_start = thread_out_sequences[i]
-            _parse_fasta_line(complete_file[start:end], out_buffer[buffer_start:buffer_start + end - start], mappings)
-            seqlens[i] = end - start
+#         current_start = 0
+#         for i in range(start_idx, end_idx):
+#             c = complete_file[i]
+#             if to_next_line:
+#                 if c == '\n' or i == len(complete_file) - 1:
+#                     if current_start != -1:
+#                         thread_out_sequences.append((current_start, i, thread_buffer_size))
+#                         thread_buffer_size += i - current_start
+#                     to_next_line = False
+#                 continue
+#             if c == '>':
+#                 # Potentially parse the header
+#                 to_next_line = True
+#                 current_start = -1
+#                 continue
+#             else:
+#                 current_start = i
+#                 to_next_line = True
+
+#         out_buffer = np.zeros(thread_buffer_size, dtype=np.uint8)
+#         seqlens = np.zeros(len(thread_out_sequences), dtype=np.int64)
+#         for i in nb.prange(len(thread_out_sequences)):
+#             start, end, buffer_start = thread_out_sequences[i]
+#             _parse_fasta_line(complete_file[start:end], out_buffer[buffer_start:buffer_start + end - start], mappings)
+#             seqlens[i] = end - start
 
-        thread_cu_seqlenss[t] = np.zeros(len(thread_out_sequences) + 1, dtype=np.int64)
-        thread_cu_seqlenss[t][1:] = np.cumsum(seqlens)
+#         thread_cu_seqlenss[t] = np.zeros(len(thread_out_sequences) + 1, dtype=np.int64)
+#         thread_cu_seqlenss[t][1:] = np.cumsum(seqlens)
     
-    print('Stitching cu_seqlens')
-    for t in range(n_threads):
-        thread_cu_seqlenss[t] += thread_cu_seqlenss[t - 1][-1]
+#     print('Stitching cu_seqlens')
+#     for t in range(n_threads):
+#         thread_cu_seqlenss[t] += thread_cu_seqlenss[t - 1][-1]
     
-    cu_seqlens = np.zeros(thread_cu_seqlenss[-1][-1], dtype=np.int64)
-    # for t in nb.prange(n_threads):
-    #     cu_seqlens[thread_cu_seqlenss[t]] = thread_cu_seqlenss[t][1:]
+#     cu_seqlens = np.zeros(thread_cu_seqlenss[-1][-1], dtype=np.int64)
+#     # for t in nb.prange(n_threads):
+#     #     cu_seqlens[thread_cu_seqlenss[t]] = thread_cu_seqlenss[t][1:]
+
 
+    
+#     # return out_buffer, cu_seqlens
+#     return thread_cu_seqlenss[-1]
 
+# def parse_fasta(complete_file_text: str, vocab: Any) -> ak.Array:
+#     """
+#     complete_file_text: The entire contents of a fasta file as a string, including newlines
+#     vocab: The vocabulary to use for parsing the fasta file, must contain the tokens 'a', 't', 'c', 'g', and '<unk>'
+#     """
+#     # Only parsing ATCG, which are lowercase in the vocab
+#     mapping_values = [*[vocab[token] for token in ['a', 't', 'c', 'g']], vocab['<unk>']]
+#     for val in mapping_values:
+#         assert val < 256, 'Must fit in a uint8'
+#     mappings = np.array(mapping_values, dtype=np.uint8)
+#     buffer, cu_seqlens = _parse_fasta(complete_file_text, mappings)
+
+#     offsets = ak.index.Index64(cu_seqlens)
+#     tokens = ak.contents.NumpyArray(buffer)
+#     return ak.Array(ak.contents.ListOffsetArray(offsets, tokens))
     
-    # return out_buffer, cu_seqlens
-    return thread_cu_seqlenss[-1]
 
-def parse_fasta(complete_file_text: str, vocab: Any) -> ak.Array:
+def parse_fasta(path: str, vocab: Any) -> ak.Array:
     """
     complete_file_text: The entire contents of a fasta file as a string, including newlines
     vocab: The vocabulary to use for parsing the fasta file, must contain the tokens 'a', 't', 'c', 'g', and '<unk>'
     """
     # Only parsing ATCG, which are lowercase in the vocab
     mapping_values = [*[vocab[token] for token in ['a', 't', 'c', 'g']], vocab['<unk>']]
-    for val in mapping_values:
-        assert val < 256, 'Must fit in a uint8'
-    mappings = np.array(mapping_values, dtype=np.uint8)
-    buffer, cu_seqlens = _parse_fasta(complete_file_text, mappings)
+
+    buffer, cu_seqlens,  = dogma_rust.parse_fasta(path, np.array(mapping_values, dtype=np.uint8))
 
     offsets = ak.index.Index64(cu_seqlens)
     tokens = ak.contents.NumpyArray(buffer)
     return ak.Array(ak.contents.ListOffsetArray(offsets, tokens))
     
 
 
-
 if __name__ == '__main__':
     from torchtext import vocab
     from collections import OrderedDict
     AA_VOCAB = vocab.vocab(
         OrderedDict(
             [
                 (token, 1)
@@ -159,11 +173,12 @@
                     "<seq_protein_masked>",
                 ]
             ]
         ),
         specials=["<pad>", "<sos>", "<eos>", "<unk>"],
     )
     AA_VOCAB.set_default_index(AA_VOCAB["<aaunk>"])
-    with open('fasta_example.fasta', 'r') as f:
-        fasta_lines = parse_fasta(f.read(), AA_VOCAB)
+    fasta_lines = parse_fasta('fasta_data/result_rep_seq.fasta', AA_VOCAB)
+    # with open('fasta_data/result_rep_seq.fasta', 'r') as f:
+    #     fasta_lines = parse_fasta(f.read(), AA_VOCAB)
     print(fasta_lines)
     breakpoint()
```

### Comparing `dogma-data-0.2.1/dogma_data/utils.py` & `dogma-data-0.2.3/dogma_data/utils.py`

 * *Files identical despite different names*

### Comparing `dogma-data-0.2.1/dogma_data.egg-info/PKG-INFO` & `dogma-data-0.2.3/dogma_data.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.1
+Version: 0.2.3
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dogma-data-0.2.1/pyproject.toml` & `dogma-data-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dogma-data"
 description = "Data processing for Dogma"
-version = "0.2.1"
+version = "0.2.3"
 requires-python = ">=3.11"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["single-cell", "RNA-seq", "embedding", "pytorch", "uce"]
 dependencies = [
     "lightning",
     "numpy",
@@ -31,14 +31,17 @@
 authors = [
     {name = "Marcel Rød", email = "roed@stanford.edu"},
 ]
 
 [tool.setuptools.packages.find]
 include = ["dogma_data"]
 
+# [tool.setuptools.package-data]
+# "" = ["cpp_functions.hpp"]
+
 [project.urls]
 Homepage = "https://github.com/marcelroed/dogma-data"
 Repository = "https://github.com/marcelroed/dogma-data.git"
 
 # [project.optional-dependencies]
 # train = [
 #     "accelerate"
```

