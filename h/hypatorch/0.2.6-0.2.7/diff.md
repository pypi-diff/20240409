# Comparing `tmp/hypatorch-0.2.6.tar.gz` & `tmp/hypatorch-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypatorch-0.2.6.tar", last modified: Fri Apr  5 15:59:10 2024, max compression
+gzip compressed data, was "hypatorch-0.2.7.tar", last modified: Tue Apr  9 09:38:16 2024, max compression
```

## Comparing `hypatorch-0.2.6.tar` & `hypatorch-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 15:59:10.933603 hypatorch-0.2.6/
--rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.6/LICENSE
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-05 15:59:10.933380 hypatorch-0.2.6/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.6/README.md
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 15:59:10.932051 hypatorch-0.2.6/hypatorch/
--rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-05 15:58:41.000000 hypatorch-0.2.6/hypatorch/__init__.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     4729 2024-03-20 14:26:18.000000 hypatorch-0.2.6/hypatorch/assessments.py
--rw-r--r--   0 paulkrug   (502) staff       (20)    23425 2024-04-05 15:58:41.000000 hypatorch-0.2.6/hypatorch/core.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.6/hypatorch/losses.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     7421 2024-03-27 10:39:37.000000 hypatorch-0.2.6/hypatorch/utils.py
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-05 15:59:10.933136 hypatorch-0.2.6/hypatorch.egg-info/
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-05 15:59:10.000000 hypatorch-0.2.6/hypatorch.egg-info/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-05 15:59:10.000000 hypatorch-0.2.6/hypatorch.egg-info/SOURCES.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-05 15:59:10.000000 hypatorch-0.2.6/hypatorch.egg-info/dependency_links.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-05 15:59:10.000000 hypatorch-0.2.6/hypatorch.egg-info/requires.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-05 15:59:10.000000 hypatorch-0.2.6/hypatorch.egg-info/top_level.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-05 15:59:10.933650 hypatorch-0.2.6/setup.cfg
--rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.6/setup.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.759660 hypatorch-0.2.7/
+-rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.7/LICENSE
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-09 09:38:16.759399 hypatorch-0.2.7/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.7/README.md
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.757785 hypatorch-0.2.7/hypatorch/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-09 09:37:32.000000 hypatorch-0.2.7/hypatorch/__init__.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     4729 2024-03-20 14:26:18.000000 hypatorch-0.2.7/hypatorch/assessments.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)    24993 2024-04-09 09:37:24.000000 hypatorch-0.2.7/hypatorch/core.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.7/hypatorch/losses.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     7421 2024-03-27 10:39:37.000000 hypatorch-0.2.7/hypatorch/utils.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.759104 hypatorch-0.2.7/hypatorch.egg-info/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/requires.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/top_level.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-09 09:38:16.759706 hypatorch-0.2.7/setup.cfg
+-rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.7/setup.py
```

### Comparing `hypatorch-0.2.6/LICENSE` & `hypatorch-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.6/PKG-INFO` & `hypatorch-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.6
+Version: 0.2.7
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.6/hypatorch/assessments.py` & `hypatorch-0.2.7/hypatorch/assessments.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.6/hypatorch/core.py` & `hypatorch-0.2.7/hypatorch/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -412,30 +412,75 @@
                     #    print( f'module {submodule_name} not applied')
                 else:
                     raise ValueError(
                         f'No submodule {submodule_name} found. Forgot to define it?'
                         )
 
         return output_dict
+    
+
+    def get_optimizers(self) -> dict:
+        """ Repack the optimizers into a dictionary with the operation names as keys. """
+
+        opts = self.optimizers()
+        if not isinstance( opts, list ):
+            opts = [ opts ]
+
+        return { op: opt for op, opt in zip( self.operations.keys(), opts )}
+
+
+    def get_lr_schedulers(self) -> dict:
+        """ lr_schedulers() alternative method from LightningModule to return the full config, not just the scheduler. """
+
+        if not self.trainer.lr_scheduler_configs:
+            return None
+
+        return { op: config for op, config in zip( self.operations.keys(), self.trainer.lr_scheduler_configs ) }
+    
+
+    def lr_scheduler_step(self,
+                          lr_scheduler_config,
+                          ):
+        
+        if lr_scheduler_config is None:
+            return
+        
+        if lr_scheduler_config.monitor is not None:
+            raise NotImplementedError(
+                f"""
+                Scheduling currently does not work with monitored metrics.
+                @TODO: Implement this feature.
+                """
+                )
+
+        # Note: if not specified, interval defaults to 'epoch' and frequency defaults to 1.
+        if lr_scheduler_config.interval == 'step':
+            if self.global_step % lr_scheduler_config.frequency == 0:
+                lr_scheduler_config.scheduler.step()
+        elif lr_scheduler_config.interval == 'epoch':
+            if self.trainer.is_last_batch:
+                if (self.current_epoch + 1) % lr_scheduler_config.frequency == 0:
+                    lr_scheduler_config.scheduler.step()
+        else:
+            raise ValueError(f"Invalid interval {lr_scheduler_config.interval} for lr_scheduler_config.")
+        
+        return
+    
 
     def training_step(self, batch, batch_idx):
 
         mode = 'train'
         
         input_dict = batch
         output_dict = {}
 
-        opts = self.optimizers()
+        opts = self.get_optimizers()
+        scheds = self.get_lr_schedulers()
 
-        # check if opts is iterable, if not, make it iterable
-        if not isinstance( opts, list ):
-            opts = [ opts ]
-
-        for operation_idx, _ in enumerate( self.operations ):
-            operation_name = list( self.operations.keys() )[ operation_idx ]
+        for operation_name in self.operations.keys():
 
             # Forward Pass
             operation_out, loss = self._forward_pass(
                 input_dict = shared_dict(
                     input_dict,
                     output_dict,
                     ),
@@ -445,25 +490,27 @@
             
             output_dict = self._handle_operation_output(
                 x = operation_out,
                 output_dict = output_dict,
                 operation_name = operation_name,
                 )
 
-            # Backward Pass if self.losses is not empty list
-            opt = opts[ operation_idx ]
+            # Backward Pass if operation has a loss.
+            opt = opts[ operation_name ]
             if self.losses[ operation_name ]:
-                #opt = opts[ operation_idx ]
                 self._backward_pass(
                     opt = opt,
                     loss = loss,
                     batch_idx = batch_idx,
                     )
             else:
                 opt.step()
+
+            if scheds is not None:
+                self.lr_scheduler_step( scheds[ operation_name ] )
             
             self._handle_assessments(
                 assessments = self.metrics,
                 data_dict = shared_dict(
                     input_dict,
                     output_dict,
                     ),
@@ -476,16 +523,15 @@
     def validation_step(self, batch, batch_idx):
 
         mode = 'val'
         
         input_dict = batch
         output_dict = {}
 
-        for operation_idx, _ in enumerate( self.operations ):
-            operation_name = list( self.operations.keys() )[ operation_idx ]
+        for operation_name in self.operations.keys():
             # Forward Pass
             with torch.no_grad():
                 operation_out, loss = self._forward_pass(
                     input_dict = shared_dict(
                         input_dict,
                         output_dict,
                         ),
@@ -643,28 +689,29 @@
     def predict_step(self, batch, batch_idx):
 
         mode = 'test'
 
         input_dict = batch
         output_dict = {}
 
-        for operation_idx, _ in enumerate( self.operations ):
-            operation_name = list( self.operations.keys() )[ operation_idx ]
+        for operation_name in self.operations.keys():
             # Forward Pass
             with torch.no_grad():
                 operation_out, loss = self._forward_pass(
                     input_dict = shared_dict(
                         input_dict,
                         output_dict,
                         ),
                     operation_name = operation_name,
                     mode = mode,
                     )
             
-            detached_loss_dict = { k: v.detach() for k, v in loss.items() }
+            detached_loss_dict = {}
+            if loss is not None:
+                detached_loss_dict = { k: v.detach() for k, v in loss.items() }
                 
             output_dict = self._handle_operation_output(
                 x = shared_dict(
                     operation_out,
                     detached_loss_dict,
                     ),
                 output_dict = output_dict,
```

### Comparing `hypatorch-0.2.6/hypatorch/losses.py` & `hypatorch-0.2.7/hypatorch/losses.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.6/hypatorch/utils.py` & `hypatorch-0.2.7/hypatorch/utils.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.6/hypatorch.egg-info/PKG-INFO` & `hypatorch-0.2.7/hypatorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.6
+Version: 0.2.7
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.6/setup.py` & `hypatorch-0.2.7/setup.py`

 * *Files identical despite different names*

