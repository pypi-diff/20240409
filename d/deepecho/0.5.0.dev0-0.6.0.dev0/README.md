# Comparing `tmp/deepecho-0.5.0.dev0.tar.gz` & `tmp/deepecho-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepecho-0.5.0.dev0.tar", last modified: Mon Nov 13 16:45:41 2023, max compression
+gzip compressed data, was "deepecho-0.6.0.dev0.tar", last modified: Tue Apr  9 21:49:21 2024, max compression
```

## Comparing `deepecho-0.5.0.dev0.tar` & `deepecho-0.6.0.dev0.tar`

### file list

```diff
@@ -1,37 +1,25 @@
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.562375 deepecho-0.5.0.dev0/
--rw-r--r--   0 johnla     (501) staff       (20)       61 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/AUTHORS.rst
--rw-r--r--   0 johnla     (501) staff       (20)     8319 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/CONTRIBUTING.rst
--rw-r--r--   0 johnla     (501) staff       (20)     3545 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/HISTORY.md
--rw-r--r--   0 johnla     (501) staff       (20)     4825 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/LICENSE
--rw-r--r--   0 johnla     (501) staff       (20)      296 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/MANIFEST.in
--rw-r--r--   0 johnla     (501) staff       (20)    14574 2023-11-13 16:45:41.562529 deepecho-0.5.0.dev0/PKG-INFO
--rw-r--r--   0 johnla     (501) staff       (20)     7887 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/README.md
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.559944 deepecho-0.5.0.dev0/deepecho/
--rw-r--r--   0 johnla     (501) staff       (20)      387 2023-11-13 16:37:46.000000 deepecho-0.5.0.dev0/deepecho/__init__.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.560741 deepecho-0.5.0.dev0/deepecho/data/
--rw-r--r--   0 johnla     (501) staff       (20)    28256 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/data/demo.csv
--rw-r--r--   0 johnla     (501) staff       (20)      266 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/demo.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.561465 deepecho-0.5.0.dev0/deepecho/models/
--rw-r--r--   0 johnla     (501) staff       (20)      166 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/models/__init__.py
--rw-r--r--   0 johnla     (501) staff       (20)    10617 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/models/base.py
--rw-r--r--   0 johnla     (501) staff       (20)    21506 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/models/basic_gan.py
--rw-r--r--   0 johnla     (501) staff       (20)    23067 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/models/par.py
--rw-r--r--   0 johnla     (501) staff       (20)     7223 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/deepecho/sequences.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.560633 deepecho-0.5.0.dev0/deepecho.egg-info/
--rw-r--r--   0 johnla     (501) staff       (20)    14574 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/PKG-INFO
--rw-r--r--   0 johnla     (501) staff       (20)      631 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/SOURCES.txt
--rw-r--r--   0 johnla     (501) staff       (20)        1 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/dependency_links.txt
--rw-r--r--   0 johnla     (501) staff       (20)        1 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/not-zip-safe
--rw-r--r--   0 johnla     (501) staff       (20)     1176 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/requires.txt
--rw-r--r--   0 johnla     (501) staff       (20)        9 2023-11-13 16:45:41.000000 deepecho-0.5.0.dev0/deepecho.egg-info/top_level.txt
--rw-r--r--   0 johnla     (501) staff       (20)     1670 2023-11-13 16:45:41.562866 deepecho-0.5.0.dev0/setup.cfg
--rw-r--r--   0 johnla     (501) staff       (20)     3341 2023-11-13 16:37:46.000000 deepecho-0.5.0.dev0/setup.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.561601 deepecho-0.5.0.dev0/tests/
--rw-r--r--   0 johnla     (501) staff       (20)       28 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/__init__.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.561929 deepecho-0.5.0.dev0/tests/integration/
--rw-r--r--   0 johnla     (501) staff       (20)       44 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/integration/__init__.py
--rw-r--r--   0 johnla     (501) staff       (20)     3942 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/integration/test_basic_gan.py
--rw-r--r--   0 johnla     (501) staff       (20)     4536 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/integration/test_par.py
-drwxr-xr-x   0 johnla     (501) staff       (20)        0 2023-11-13 16:45:41.562228 deepecho-0.5.0.dev0/tests/unit/
--rw-r--r--   0 johnla     (501) staff       (20)       37 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/unit/__init__.py
--rw-r--r--   0 johnla     (501) staff       (20)     6642 2023-10-19 18:37:14.000000 deepecho-0.5.0.dev0/tests/unit/test_sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.534925 deepecho-0.6.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.6.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10632 2024-04-09 21:49:21.534575 deepecho-0.6.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7887 2024-02-12 22:55:24.000000 deepecho-0.6.0.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.530548 deepecho-0.6.0.dev0/deepecho/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      387 2024-04-09 21:47:08.000000 deepecho-0.6.0.dev0/deepecho/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.531345 deepecho-0.6.0.dev0/deepecho/data/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.6.0.dev0/deepecho/data/demo.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532499 deepecho-0.6.0.dev0/deepecho/models/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.6.0.dev0/deepecho/models/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10776 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21539 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23504 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/models/par.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7142 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/deepecho/sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532881 deepecho-0.6.0.dev0/deepecho.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10632 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      398 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      746 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2024-04-09 21:49:21.000000 deepecho-0.6.0.dev0/deepecho.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4960 2024-04-09 21:48:53.000000 deepecho-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2024-04-09 21:49:21.534997 deepecho-0.6.0.dev0/setup.cfg
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-04-09 21:49:21.532677 deepecho-0.6.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2024-04-09 21:41:01.000000 deepecho-0.6.0.dev0/tests/test_tasks.py
```

### Comparing `deepecho-0.5.0.dev0/LICENSE` & `deepecho-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepecho-0.5.0.dev0/README.md` & `deepecho-0.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `deepecho-0.5.0.dev0/deepecho/data/demo.csv` & `deepecho-0.6.0.dev0/deepecho/data/demo.csv`

 * *Files identical despite different names*

### Comparing `deepecho-0.5.0.dev0/deepecho/models/base.py` & `deepecho-0.6.0.dev0/deepecho/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 import tqdm
 
 from deepecho.sequences import assemble_sequences
 
 
-class DeepEcho():
+class DeepEcho:
     """The base class for DeepEcho models."""
 
     _verbose = True
     _output_columns = None
     _data_columns = None
     _entity_columns = None
     _context_columns = None
@@ -24,15 +24,21 @@
             sequences:
                 See `fit`.
             context_types:
                 See `fit`.
             data_types:
                 See `fit`.
         """
-        dtypes = set(['continuous', 'categorical', 'ordinal', 'count', 'datetime'])
+        dtypes = set([
+            'continuous',
+            'categorical',
+            'ordinal',
+            'count',
+            'datetime',
+        ])
         assert all(dtype in dtypes for dtype in context_types)
         assert all(dtype in dtypes for dtype in data_types)
 
         for sequence in sequences:
             assert len(sequence['context']) == len(context_types)
             assert len(sequence['data']) == len(data_types)
             lengths = [len(x) for x in sequence['data']]
@@ -95,16 +101,23 @@
                     dtypes_list.append('datetime')
                 else:
                     error = f'Unsupported data_type for column {column}: {dtype}'
                     raise ValueError(error)
 
         return dtypes_list
 
-    def fit(self, data, entity_columns=None, context_columns=None,
-            data_types=None, segment_size=None, sequence_index=None):
+    def fit(
+        self,
+        data,
+        entity_columns=None,
+        context_columns=None,
+        data_types=None,
+        segment_size=None,
+        sequence_index=None,
+    ):
         """Fit the model to a dataframe containing time series data.
 
         Args:
             data (pd.DataFrame):
                 DataFrame containing all the timeseries data alongside the
                 entity and context columns.
             entity_columns (list[str]):
@@ -131,16 +144,15 @@
                 such as integer values or datetimes.
         """
         if not entity_columns and segment_size is None:
             raise TypeError('If the data has no `entity_columns`, `segment_size` must be given.')
         if segment_size is not None and not isinstance(segment_size, int):
             if sequence_index is None:
                 raise TypeError(
-                    '`segment_size` must be of type `int` if '
-                    'no `sequence_index` is given.'
+                    '`segment_size` must be of type `int` if ' 'no `sequence_index` is given.'
                 )
             if data[sequence_index].dtype.kind != 'M':
                 raise TypeError(
                     '`segment_size` must be of type `int` if '
                     '`sequence_index` is not a `datetime` column.'
                 )
 
@@ -157,15 +169,20 @@
         if sequence_index:
             self._output_columns.remove(sequence_index)
             self._data_columns.remove(sequence_index)
 
         data_types = self._get_data_types(data, data_types, self._data_columns)
         context_types = self._get_data_types(data, data_types, self._context_columns)
         sequences = assemble_sequences(
-            data, self._entity_columns, self._context_columns, segment_size, sequence_index)
+            data,
+            self._entity_columns,
+            self._context_columns,
+            segment_size,
+            sequence_index,
+        )
 
         # Validate and fit
         self._validate(sequences, context_types, data_types)
         self.fit_sequences(sequences, context_types, data_types)
 
         # Store context values
         self._context_values = data[self._context_columns]
@@ -238,15 +255,15 @@
         for entity_values, context_values in iterator:
             context_values = context_values.tolist()
             sequence = self.sample_sequence(context_values, sequence_length)
 
             # Reformat as a DataFrame
             group = pd.DataFrame(
                 dict(zip(self._data_columns, sequence)),
-                columns=self._data_columns
+                columns=self._data_columns,
             )
             group[self._entity_columns] = entity_values
             for column, value in zip(self._context_columns, context_values):
                 group[column] = value
 
             output = pd.concat([output, group])
```

### Comparing `deepecho-0.5.0.dev0/deepecho/models/basic_gan.py` & `deepecho-0.6.0.dev0/deepecho/models/basic_gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 
 from deepecho.models.base import DeepEcho
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _expand_context(data, context):
-    return torch.cat([
-        data,
-        context.unsqueeze(0).expand(data.shape[0], context.shape[0], context.shape[1])
-    ], dim=2)
+    return torch.cat(
+        [
+            data,
+            context.unsqueeze(0).expand(data.shape[0], context.shape[0], context.shape[1]),
+        ],
+        dim=2,
+    )
 
 
 class BasicGenerator(torch.nn.Module):
     """Generator for the BasicGAN model.
 
     This generator consist on a RNN layer followed by a Linear layer with
     the following schema:
@@ -61,15 +64,15 @@
             context (tensor):
                 Context values to use for each generated sequence.
             sequence_length (int):
                 Amount of data points to generate for each sequence.
         """
         latent = torch.randn(
             size=(sequence_length, context.size(0), self.latent_size),
-            device=self.device
+            device=self.device,
         )
         latent = _expand_context(latent, context)
 
         rnn_out, _ = self.rnn(latent)
         return self.linear(rnn_out)
 
 
@@ -146,16 +149,24 @@
     _context_map = None
     _context_size = None
     _data_map = None
     _data_size = None
     _model_data_size = None
     _generator = None
 
-    def __init__(self, epochs=1024, latent_size=32, hidden_size=16,
-                 gen_lr=1e-3, dis_lr=1e-3, cuda=True, verbose=True):
+    def __init__(
+        self,
+        epochs=1024,
+        latent_size=32,
+        hidden_size=16,
+        gen_lr=1e-3,
+        dis_lr=1e-3,
+        cuda=True,
+        verbose=True,
+    ):
         self._epochs = epochs
         self._gen_lr = gen_lr
         self._dis_lr = dis_lr
         self._latent_size = latent_size
         self._hidden_size = hidden_size
 
         if not cuda or not torch.cuda.is_available():
@@ -207,28 +218,25 @@
         for column, column_type in enumerate(types):
             values = columns[column]
             if column_type in ('continuous', 'count'):
                 mapping[column] = {
                     'type': column_type,
                     'min': np.min(values),
                     'max': np.max(values),
-                    'indices': (dimensions, dimensions + 1)
+                    'indices': (dimensions, dimensions + 1),
                 }
                 dimensions += 2
 
             elif column_type in ('categorical', 'ordinal'):
                 indices = {}
                 for value in set(values):
                     indices[value] = dimensions
                     dimensions += 1
 
-                mapping[column] = {
-                    'type': column_type,
-                    'indices': indices
-                }
+                mapping[column] = {'type': column_type, 'indices': indices}
 
             else:
                 raise ValueError(f'Unsupported type: {column_type}')
 
         return mapping, dimensions
 
     def _analyze_data(self, sequences, context_types, data_types):
@@ -313,15 +321,15 @@
         column_type = properties['type']
         if column_type in ('continuous', 'count'):
             self._normalize(tensor, value, properties)
         elif column_type in ('categorical', 'ordinal'):
             self._one_hot_encode(tensor, value, properties)
 
         else:
-            raise ValueError()   # Theoretically unreachable
+            raise ValueError()  # Theoretically unreachable
 
     def _data_to_tensor(self, data):
         """Convert the input data to the corresponding tensor.
 
         If ``self._fixed_length`` is ``False``, add a 1.0 to indicate
         the sequence end and pad the rest of the sequence with 0.0s.
         """
@@ -366,15 +374,15 @@
             for row in range(sequence_length):
                 if column_type in ('continuous', 'count'):
                     round_value = column_type == 'count'
                     value = self._denormalize(tensor, row, properties, round_value=round_value)
                 elif column_type in ('categorical', 'ordinal'):
                     value = self._one_hot_decode(tensor, row, properties)
                 else:
-                    raise ValueError()   # Theoretically unreachable
+                    raise ValueError()  # Theoretically unreachable
 
                 column_data.append(value)
 
         return data
 
     def _build_tensor(self, transform, sequences, key, dim):
         """Convert input sequences to tensors."""
@@ -408,15 +416,15 @@
 
         for sequence_idx in range(generated.shape[1]):
             # Pad with zeroes after end_flag == 1
             sequence = generated[:, sequence_idx]
             end_flag = sequence[:, self._data_size]
             if (end_flag == 1.0).any():
                 cut_idx = end_flag.detach().cpu().numpy().argmax()
-                sequence[cut_idx + 1:] = 0.0
+                sequence[cut_idx + 1 :] = 0.0
 
     def _generate(self, context, sequence_length=None):
         generated = self._generator(
             context=context,
             sequence_length=sequence_length or self._max_sequence_length,
         )
```

### Comparing `deepecho-0.5.0.dev0/deepecho/models/par.py` & `deepecho-0.6.0.dev0/deepecho/models/par.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,32 +23,38 @@
         self.up = torch.nn.Linear(hidden_size, data_size)
 
     def forward(self, x, c):
         """Forward passing computation."""
         if isinstance(x, torch.nn.utils.rnn.PackedSequence):
             x, lengths = torch.nn.utils.rnn.pad_packed_sequence(x)
             if self.context_size:
-                x = torch.cat([
-                    x,
-                    c.unsqueeze(0).expand(x.shape[0], c.shape[0], c.shape[1])
-                ], dim=2)
+                x = torch.cat(
+                    [
+                        x,
+                        c.unsqueeze(0).expand(x.shape[0], c.shape[0], c.shape[1]),
+                    ],
+                    dim=2,
+                )
 
             x = self.down(x)
             x = torch.nn.utils.rnn.pack_padded_sequence(x, lengths, enforce_sorted=False)
             x, _ = self.rnn(x)
             x, lengths = torch.nn.utils.rnn.pad_packed_sequence(x)
             x = self.up(x)
             x = torch.nn.utils.rnn.pack_padded_sequence(x, lengths, enforce_sorted=False)
 
         else:
             if self.context_size:
-                x = torch.cat([
-                    x,
-                    c.unsqueeze(0).expand(x.shape[0], c.shape[0], c.shape[1])
-                ], dim=2)
+                x = torch.cat(
+                    [
+                        x,
+                        c.unsqueeze(0).expand(x.shape[0], c.shape[0], c.shape[1]),
+                    ],
+                    dim=2,
+                )
 
             x = self.down(x)
             x, _ = self.rnn(x)
             x = self.up(x)
 
         return x
 
@@ -122,33 +128,30 @@
         for i, t in enumerate(t):
             if t == 'continuous' or t == 'datetime':
                 idx_map[i] = {
                     'type': t,
                     'mu': np.nanmean(x[i]),
                     'std': np.nanstd(x[i]),
                     'nulls': pd.isnull(x[i]).any(),
-                    'indices': (idx, idx + 1, idx + 2)
+                    'indices': (idx, idx + 1, idx + 2),
                 }
                 idx += 3
 
             elif t == 'count':
                 idx_map[i] = {
                     'type': t,
                     'min': np.nanmin(x[i]),
                     'range': np.nanmax(x[i]) - np.nanmin(x[i]),
                     'nulls': pd.isnull(x[i]).any(),
-                    'indices': (idx, idx + 1, idx + 2)
+                    'indices': (idx, idx + 1, idx + 2),
                 }
                 idx += 3
 
             elif t == 'categorical' or t == 'ordinal':
-                idx_map[i] = {
-                    'type': t,
-                    'indices': {}
-                }
+                idx_map[i] = {'type': t, 'indices': {}}
                 idx += 1
                 for v in set(x[i]):
                     if pd.isnull(v):
                         v = None
 
                     idx_map[i]['indices'][v] = idx
                     idx += 1
@@ -182,16 +185,16 @@
         self._ctx_map, self._ctx_dims = self._idx_map(contexts, context_types)
         self._data_map, self._data_dims = self._idx_map(data, data_types)
         self._data_map['<TOKEN>'] = {
             'type': 'categorical',
             'indices': {
                 '<START>': self._data_dims,
                 '<END>': self._data_dims + 1,
-                '<BODY>': self._data_dims + 2
-            }
+                '<BODY>': self._data_dims + 2,
+            },
         }
         self._data_dims += 3
 
     def _data_to_tensor(self, data):
         seq_len = len(data[0])
         X = []
 
@@ -221,15 +224,18 @@
                         x[r_idx] = 0.0
                     else:
                         x[r_idx] = (data[key][i] - props['min']) / props['range']
 
                     x[p_idx] = 0.0
                     x[missing_idx] = 1.0 if pd.isnull(data[key][i]) else 0.0
 
-                elif props['type'] in ['categorical', 'ordinal']:   # categorical
+                elif props['type'] in [
+                    'categorical',
+                    'ordinal',
+                ]:  # categorical
                     value = data[key][i]
                     if pd.isnull(value):
                         value = None
                     x[props['indices'][value]] = 1.0
 
                 else:
                     raise ValueError()
@@ -246,23 +252,29 @@
         if not self._ctx_dims:
             return None
 
         x = torch.zeros(self._ctx_dims)
         for key, props in self._ctx_map.items():
             if props['type'] in ['continuous', 'datetime']:
                 mu_idx, sigma_idx, missing_idx = props['indices']
-                x[mu_idx] = 0.0 if (pd.isnull(context[key]) or props['std'] == 0) else (
-                    context[key] - props['mu']) / props['std']
+                x[mu_idx] = (
+                    0.0
+                    if (pd.isnull(context[key]) or props['std'] == 0)
+                    else (context[key] - props['mu']) / props['std']
+                )
                 x[sigma_idx] = 0.0
                 x[missing_idx] = 1.0 if pd.isnull(context[key]) else 0.0
 
             elif props['type'] in ['count']:
                 r_idx, p_idx, missing_idx = props['indices']
-                x[r_idx] = 0.0 if (pd.isnull(context[key]) or props['range'] == 0) else (
-                    context[key] - props['min']) / props['range']
+                x[r_idx] = (
+                    0.0
+                    if (pd.isnull(context[key]) or props['range'] == 0)
+                    else (context[key] - props['min']) / props['range']
+                )
                 x[p_idx] = 0.0
                 x[missing_idx] = 1.0 if pd.isnull(context[key]) else 0.0
 
             elif props['type'] in ['categorical', 'ordinal']:
                 value = context[key]
                 if pd.isnull(value):
                     value = None
@@ -337,20 +349,21 @@
 
             optimizer.zero_grad()
             loss = self._compute_loss(X_padded[1:, :, :], Y_padded[:-1, :, :], seq_len)
             loss.backward()
 
             epoch_loss_df = pd.DataFrame({
                 'Epoch': [epoch],
-                'Loss': [loss.item()]
+                'Loss': [loss.item()],
             })
             if not self.loss_values.empty:
-                self.loss_values = pd.concat(
-                    [self.loss_values, epoch_loss_df]
-                ).reset_index(drop=True)
+                self.loss_values = pd.concat([
+                    self.loss_values,
+                    epoch_loss_df,
+                ]).reset_index(drop=True)
             else:
                 self.loss_values = epoch_loss_df
 
             if self.verbose:
                 iterator.set_description(pbar_description.format(loss=loss.item()))
 
             optimizer.step()
@@ -371,59 +384,65 @@
                 This contains the input to the model.
             Y_padded (tensor):
                 This contains the output of the model.
             seq_len (list):
                 This list contains the length of each sequence.
         """
         log_likelihood = 0.0
-        _, batch_size, input_size = X_padded.shape
+        _, batch_size, _input_size = X_padded.shape
 
         for key, props in self._data_map.items():
             if props['type'] in ['continuous', 'timestamp']:
                 mu_idx, sigma_idx, missing_idx = props['indices']
                 mu = Y_padded[:, :, mu_idx]
                 sigma = torch.nn.functional.softplus(Y_padded[:, :, sigma_idx])
                 missing = torch.nn.LogSigmoid()(Y_padded[:, :, missing_idx])
 
                 for i in range(batch_size):
                     dist = torch.distributions.normal.Normal(
-                        mu[:seq_len[i], i], sigma[:seq_len[i], i])
-                    log_likelihood += torch.sum(dist.log_prob(X_padded[-seq_len[i]:, i, mu_idx]))
+                        mu[: seq_len[i], i], sigma[: seq_len[i], i]
+                    )
+                    log_likelihood += torch.sum(dist.log_prob(X_padded[-seq_len[i] :, i, mu_idx]))
 
-                    p_true = X_padded[:seq_len[i], i, missing_idx]
-                    p_pred = missing[:seq_len[i], i]
+                    p_true = X_padded[: seq_len[i], i, missing_idx]
+                    p_pred = missing[: seq_len[i], i]
                     log_likelihood += torch.sum(p_true * p_pred)
-                    log_likelihood += torch.sum((1.0 - p_true) * torch.log(
-                        1.0 - torch.exp(p_pred)))
+                    log_likelihood += torch.sum(
+                        (1.0 - p_true) * torch.log(1.0 - torch.exp(p_pred))
+                    )
 
             elif props['type'] in ['count']:
                 r_idx, p_idx, missing_idx = props['indices']
                 r = torch.nn.functional.softplus(Y_padded[:, :, r_idx]) * props['range']
                 p = torch.sigmoid(Y_padded[:, :, p_idx])
                 x = X_padded[:, :, r_idx] * props['range']
                 missing = torch.nn.LogSigmoid()(Y_padded[:, :, missing_idx])
 
                 for i in range(batch_size):
                     dist = torch.distributions.negative_binomial.NegativeBinomial(
-                        r[:seq_len[i], i], p[:seq_len[i], i], validate_args=False)
-                    log_likelihood += torch.sum(dist.log_prob(x[:seq_len[i], i]))
+                        r[: seq_len[i], i],
+                        p[: seq_len[i], i],
+                        validate_args=False,
+                    )
+                    log_likelihood += torch.sum(dist.log_prob(x[: seq_len[i], i]))
 
-                    p_true = X_padded[:seq_len[i], i, missing_idx]
-                    p_pred = missing[:seq_len[i], i]
+                    p_true = X_padded[: seq_len[i], i, missing_idx]
+                    p_pred = missing[: seq_len[i], i]
                     log_likelihood += torch.sum(p_true * p_pred)
-                    log_likelihood += torch.sum((1.0 - p_true) * torch.log(
-                        1.0 - torch.exp(p_pred)))
+                    log_likelihood += torch.sum(
+                        (1.0 - p_true) * torch.log(1.0 - torch.exp(p_pred))
+                    )
 
             elif props['type'] in ['categorical', 'ordinal']:
                 idx = list(props['indices'].values())
                 log_softmax = torch.nn.functional.log_softmax(Y_padded[:, :, idx], dim=2)
 
                 for i in range(batch_size):
-                    target = X_padded[:seq_len[i], i, idx]
-                    predicted = log_softmax[:seq_len[i], i]
+                    target = X_padded[: seq_len[i], i, idx]
+                    predicted = log_softmax[: seq_len[i], i]
                     target = torch.argmax(target, dim=1).unsqueeze(dim=1)
                     log_likelihood += torch.sum(predicted.gather(dim=1, index=target))
 
             else:
                 raise ValueError()
 
         return -log_likelihood / (batch_size * len(self._data_map) * batch_size)
@@ -439,22 +458,22 @@
         for key, props in self._data_map.items():
             if key == '<TOKEN>':
                 continue
 
             data[key] = []
             for i in range(seq_len):
                 if props['type'] in ['continuous', 'datetime']:
-                    mu_idx, sigma_idx, missing_idx = props['indices']
+                    mu_idx, _sigma_idx, missing_idx = props['indices']
                     if (x[i, 0, missing_idx] > 0) and props['nulls']:
                         data[key].append(None)
                     else:
                         data[key].append(x[i, 0, mu_idx].item() * props['std'] + props['mu'])
 
                 elif props['type'] in ['count']:
-                    r_idx, p_idx, missing_idx = props['indices']
+                    r_idx, _p_idx, missing_idx = props['indices']
                     if x[i, 0, missing_idx] > 0 and props['nulls']:
                         data[key].append(None)
                     else:
                         sample = x[i, 0, r_idx].item() * props['range'] + props['min']
                         data[key].append(int(sample))
 
                 elif props['type'] in ['categorical', 'ordinal']:
@@ -469,15 +488,15 @@
                 else:
                     raise ValueError()
 
         return data
 
     def _sample_state(self, x):
         log_likelihood = 0.0
-        seq_len, batch_size, input_size = x.shape
+        seq_len, batch_size, _input_size = x.shape
         assert seq_len == 1 and batch_size == 1
 
         for key, props in self._data_map.items():
             if props['type'] in ['continuous', 'timestamp']:
                 mu_idx, sigma_idx, missing_idx = props['indices']
                 mu = x[0, 0, mu_idx]
                 sigma = torch.nn.functional.softplus(x[0, 0, sigma_idx])
```

### Comparing `deepecho-0.5.0.dev0/deepecho/sequences.py` & `deepecho-0.6.0.dev0/deepecho/sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,28 +113,28 @@
                 raise ValueError('Context columns are not constant within each segment.')
 
             context = context.iloc[0].values
             segment = segment.drop(context_columns, axis=1)
         else:
             context = []
 
-        lists = [
-            list(row)
-            for _, row in segment.items()
-        ]
-        sequences.append({
-            'context': context,
-            'data': lists
-        })
+        lists = [list(row) for _, row in segment.items()]
+        sequences.append({'context': context, 'data': lists})
 
     return sequences
 
 
-def assemble_sequences(data, entity_columns, context_columns, segment_size,
-                       sequence_index, drop_sequence_index=True):
+def assemble_sequences(
+    data,
+    entity_columns,
+    context_columns,
+    segment_size,
+    sequence_index,
+    drop_sequence_index=True,
+):
     """Build sequences from the data, grouping first by entity and then segmenting by size.
 
     Input is a ``pandas.DataFrame`` containing all the data, lists of entity and context
     columns and instructions about how to segment each entity sequence.
 
     The process of building the sequences consists on:
 
@@ -181,12 +181,13 @@
         groupby_columns = entity_columns[0] if len(entity_columns) == 1 else entity_columns
         for _, sequence in data.groupby(groupby_columns):
             sequence.drop(entity_columns, axis=1, inplace=True)
             if context_columns:
                 if len(sequence[context_columns].drop_duplicates()) > 1:
                     raise ValueError('Context columns are not constant within each entity.')
 
-            entity_segments = segment_sequence(sequence, segment_size,
-                                               sequence_index, drop_sequence_index)
+            entity_segments = segment_sequence(
+                sequence, segment_size, sequence_index, drop_sequence_index
+            )
             segments.extend(entity_segments)
 
     return _convert_to_dicts(segments, context_columns)
```

