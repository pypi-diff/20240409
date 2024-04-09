# Comparing `tmp/accmt-0.0.7.tar.gz` & `tmp/accmt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-0.0.7.tar", last modified: Mon Apr  1 20:22:15 2024, max compression
+gzip compressed data, was "accmt-0.0.8.tar", last modified: Tue Apr  9 04:35:00 2024, max compression
```

## Comparing `accmt-0.0.7.tar` & `accmt-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.189455 accmt-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3274 2024-04-01 20:22:15.188387 accmt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2627 2024-04-01 01:48:15.000000 accmt-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      786 2024-04-01 20:22:15.189455 accmt-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.130118 accmt-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.162374 accmt-0.0.7/src/accmt/
--rw-rw-rw-   0        0        0       97 2024-04-01 00:10:31.000000 accmt-0.0.7/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    15050 2024-04-01 20:21:53.000000 accmt-0.0.7/src/accmt/accmt.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.7/src/accmt/config.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.186371 accmt-0.0.7/src/accmt.egg-info/
--rw-rw-rw-   0        0        0     3274 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.198601 accmt-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    12238 2024-04-09 04:35:00.196594 accmt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11517 2024-04-09 02:52:21.000000 accmt-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      837 2024-04-09 04:35:00.200597 accmt-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.142363 accmt-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.167593 accmt-0.0.8/src/accmt/
+-rw-rw-rw-   0        0        0       96 2024-04-09 02:00:37.000000 accmt-0.0.8/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    23923 2024-04-09 04:33:12.000000 accmt-0.0.8/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-0.0.8/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.8/src/accmt/config.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:35:00.195594 accmt-0.0.8/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    12238 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 04:35:00.000000 accmt-0.0.8/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-0.0.7/LICENSE` & `accmt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-0.0.7/setup.cfg` & `accmt-0.0.8/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 302e 302e 370d 0a61 7574 686f  n = 0.0.7..autho
+00000020: 6e20 3d20 302e 302e 380d 0a61 7574 686f  n = 0.0.8..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
@@ -37,14 +37,17 @@
 00000240: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
 00000250: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 00000260: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
 00000270: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 00000280: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 00000290: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 000002a0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-000002b0: 7265 7320 3d20 3e3d 332e 3130 0d0a 0d0a  res = >=3.10....
-000002c0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-000002d0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000002e0: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-000002f0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000300: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000310: 0d0a                                     ..
+000002b0: 7265 7320 3d20 3e3d 332e 3130 0d0a 696e  res = >=3.10..in
+000002c0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+000002d0: 200d 0a09 6163 6365 6c65 7261 7465 0d0a   ...accelerate..
+000002e0: 096e 756d 7079 0d0a 0950 7959 414d 4c0d  .numpy...PyYAML.
+000002f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000300: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000310: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
+00000320: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000330: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000340: 300d 0a0d 0a                             0....
```

### Comparing `accmt-0.0.7/src/accmt/accmt.py` & `accmt-0.0.8/src/accmt/accmt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,87 @@
 import numpy as np
 import torch
 import warnings
 
 from abc import ABC
 from accelerate import Accelerator
-from accelerate.utils import LoggerType, ProjectConfiguration
+from accelerate.utils import LoggerType, ProjectConfiguration, tqdm
 from .config import read, save_status, read_status
+import torch.optim
+import torch.optim.lr_scheduler as lr_scheduler
 from torch.utils.data import Dataset
 from typing import Any
 from typing_extensions import override
-
+from transformers import (
+    get_cosine_schedule_with_warmup,
+    get_constant_schedule,
+    get_constant_schedule_with_warmup,
+    get_cosine_with_hard_restarts_schedule_with_warmup,
+    get_inverse_sqrt_schedule,
+    get_linear_schedule_with_warmup,
+    get_polynomial_decay_schedule_with_warmup,
+    Adafactor
+)
+
+OPTIMIZERS = {
+    "Adam": torch.optim.Adam,
+    "Adadelta": torch.optim.Adadelta,
+    "Adagrad": torch.optim.Adagrad,
+    "Adamax": torch.optim.Adamax,
+    "AdamW": torch.optim.AdamW,
+    "Adafactor": Adafactor,
+    "ASGD": torch.optim.ASGD,
+    "LBFGS": torch.optim.LBFGS,
+    "NAdam": torch.optim.NAdam,
+    "RAdam": torch.optim.RAdam,
+    "RMSprop": torch.optim.RMSprop,
+    "Rprop": torch.optim.Rprop,
+    "SGD": torch.optim.SGD,
+    "SparseAdam": torch.optim.SparseAdam
+}
+
+SCHEDULERS = {
+    "StepLR": lr_scheduler.StepLR,
+    "LinearLR": lr_scheduler.LinearLR,
+    "ExponentialLR": lr_scheduler.ExponentialLR,
+    "CosineAnnealingLR": lr_scheduler.CosineAnnealingLR,
+    "CyclicLR": lr_scheduler.CyclicLR,
+    "OneCycleLR": lr_scheduler.OneCycleLR,
+    "CosineAnnealingWarmRestarts": lr_scheduler.CosineAnnealingWarmRestarts,
+    "CosineWithWarmup": get_cosine_schedule_with_warmup,
+    "Constant": get_constant_schedule,
+    "ConstantWithWarmup": get_constant_schedule_with_warmup,
+    "CosineWithHardRestartsWithWarmup": get_cosine_with_hard_restarts_schedule_with_warmup,
+    "InverseSQRT": get_inverse_sqrt_schedule,
+    "LinearWithWarmup": get_linear_schedule_with_warmup,
+    "PolynomialDecayWithWarmup": get_polynomial_decay_schedule_with_warmup
+}
 
 class AcceleratorModule(ABC):
     """
     Super class to define training and validation logic without the need
     to write a training loop.
 
     The constructor of this class must implement `self.model`, specifying the model
     from `torch.nn.Module`.
 
     Methods:
         `forward` (optional):
             Defines the flow of data of model. If not implemented, `__call__`
             will not be possible (e.g. `self(...)`).
-        `training_step`:
+        `training_step` (optional):
             Defines the training logic. Must return a loss `torch.Tensor` (scalar).
         `validation_step` (optional):
             Defines the validation logic. Must return a loss `torch.Tensor` (scalar).
             If not implemented, no validation will be executed.
+        `step` (optional):
+            Defines the training and validation logics. This is useful when training
+            and validation logics are the same.
+            NOTE: Cannot define `step` together with `training_step` and/or
+            `validation_step`.
     
     Special methods (no implementation required):
         `__call__`:
             When calling this module, it will execute `forward` method.
         `__repr__`:
             When reproducing this module (e.g. Jupyter Notebook cell), this will print
             the model structure from `torch.nn.Module` specified in `self.model`.
@@ -39,32 +89,61 @@
             When printing this module or using it as a `str` type, this will represent
             the `torch.nn.Module` specified in `self.model`.
         `__len__`:
             When casting this module with `len` Python function, it will return the
             number of parameters of the base model specified in `self.model` from
             `torch.nn.Module`.
     """
+    _implemented_collate_fn = False
 
     @override
     def forward(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         """Defines the flow of data."""
+
+    @override
+    def step(self, *args: Any, **kwargs: Any) -> torch.Tensor:
+        """Defines the logic for both training and validation."""
     
     @override
     def training_step(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         """Defines the training logic. Must return a loss tensor (scalar)."""
     
     @override
     def validation_step(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         """Defines the validation logic. Must return a loss tensor (scalar)."""
+
+    @override
+    def collate_fn(self, batch: list) -> Any:
+        """Defines a collate function for PyTorch DataLoader."""
     
     def __init_subclass__(cls, **kwargs):
-        if cls.training_step == AcceleratorModule.training_step and cls.validation_step == AcceleratorModule.validation_step:
+        if (
+            cls.training_step == AcceleratorModule.training_step and
+            cls.validation_step == AcceleratorModule.validation_step and
+            cls.step == AcceleratorModule.step
+        ):
+            raise TypeError(
+                "Subclasses of 'Trainer' must override 'training_step' and/or "
+                "'validation_step' methods. If you want training and validation "
+                "logics to be the same, then override 'step' method."
+            )
+        elif (
+            (cls.training_step != AcceleratorModule.training_step or
+            cls.validation_step != AcceleratorModule.validation_step)
+            and cls.step != AcceleratorModule.step
+        ):
             raise TypeError(
-                "Subclasses of 'Trainer' must override 'training_step' and/or 'validation_step' methods."
+                "Subclasses of 'Trainer' cannot have training or validation logic "
+                "together with 'step' method. It is either 'step', or at least of "
+                "'training_step' or 'validation_step' methods."
             )
+        
+        if cls.collate_fn != AcceleratorModule.collate_fn:
+            cls._implemented_collate_fn = True
+
         super().__init_subclass__(**kwargs)
 
     def __call__(self, *args: Any, **kwargs: Any):
         return self.forward(*args, **kwargs)
 
     def __repr__(self):
         return self.model
@@ -77,26 +156,32 @@
 
 class Trainer:
     """
     Class to implement the training configuration.
     """
 
     def __init__(self,
-                hps_file_config: str,
+                hps_file_config: str = None,
                 checkpoint = "checkpoint1",
                 resume = False,
                 model_path: str = None,
                 model_saving = "best_valid_loss",
                 enable_checkpointing = True,
                 checkpoint_every = 1,
                 logging_dir = "logs",
                 log_with = LoggerType.TENSORBOARD,
                 log_every = 1,
-                grad_accumulation_steps=1,
-                set_to_none=True
+                grad_accumulation_steps=None,
+                set_to_none=True,
+                shuffle_train=True,
+                shuffle_validation=False,
+                model_saving_below_loss=float("inf"),
+                collate_fn=None,
+                max_shard_size="10GB",
+                safe_serialization=False
     ):
         """
         Trainer constructor to set configuration.
 
         Args:
             hps_file_config (`str`):
                 YAML hyperparameters file path.
@@ -120,37 +205,53 @@
                 Checkpoint every N steps. Only works if `enable_checkpointing` is set to `True`.
             logging_dir (`str`, *optional*, defaults to `logs`):
                 Path where to save logs to show progress.
             log_with (`str`, *optional*, defaults to `LoggerType.TENSORBOARD`):
                 `LoggerType` to log progress.
             log_every (`int`, *optional*, defaults to `1`):
                 Log every N steps.
-            grad_accumulation_steps (`int`, *optional*, defaults to `1`):
+            grad_accumulation_steps (`int`, *optional*, defaults to `None`):
                 Accumulate gradients for N steps. Useful for training large models and simulate
-                large batches when memory is not enough. If set to `1`, no accumulation will be perfomed.
+                large batches when memory is not enough. If set to `None` or `1`, no accumulation will be perfomed.
             set_to_none (`bool`, *optional*, defaults to `True`):
                 From PyTorch documentation: "instead of setting to zero, set the grads to None. This will
                 in general have lower memory footprint, and can modestly improve performance." Some
                 optimizers have a different behaviour if the gradient is 0 or None. See PyTorch docs
                 for more information: https://pytorch.org/docs/stable/generated/torch.optim.Optimizer.zero_grad.html
+            shuffle_train (`bool`, *optional*, defaults to `True`):
+                Whether to shuffle train DataLoader or not.
+            shuffle_validation (`bool`, *optional*, defaults to `False`):
+                Whether to shuffle validation DataLoader or not.
+            model_saving_below_loss (`float`, *optional*, defaults to `float("inf")`):
+                Start saving model on this loss (based on `model_saving`). Default is always.
+            collate_fn (`function`, *optional*, defaults to `None`):
+                Collate function to be implemented in dataloaders. If `module` overrides `collate_fn` from
+                `AcceleratorModule` class, then that function will be used instead of the one specified on
+                this constructor.
         """
 
-        self.accelerator = Accelerator()
         self.hps_config = hps_file_config
         self.checkpoint = checkpoint
         self.resume = resume
         self.model_path = model_path
         self.model_saving = model_saving.lower()
         self.enable_checkpointing = enable_checkpointing
         self.checkpoint_every = checkpoint_every
         self.logging_dir = logging_dir
         self.log_every = log_every
-        self.grad_accumulation_steps = grad_accumulation_steps
+        self.grad_accumulation_steps = grad_accumulation_steps if grad_accumulation_steps else 1
         self.set_to_none = set_to_none
+        self.shuffle_train = shuffle_train
+        self.shuffle_validation = shuffle_validation
+        self.model_saving_below_loss = model_saving_below_loss
+        self.collate_fn = collate_fn
+        self.max_shard_size = max_shard_size
+        self.safe_serialization = safe_serialization
 
+        self.accelerator = Accelerator(gradient_accumulation_steps=self.grad_accumulation_steps)
         self.accelerator.project_configuration = ProjectConfiguration(project_dir=".", logging_dir=logging_dir, total_limit=1)
         self.accelerator.log_with = [log_with]
 
     def fit(self,
             module: AcceleratorModule,
             train_dataset: Dataset,
             val_dataset: Dataset = None
@@ -168,143 +269,205 @@
                 dataset is not specified, then the validation logic of `AcceleratorModule`
                 (if specified) will be skipped. If `model_saving` parameter in the constructor is set
                 to `best_valid_loss`, this will be converted to `best_train_loss` in the background.
         """
         import os
         import torch
 
-        from tqdm.auto import tqdm
         from torch.utils.data import DataLoader
 
+        if self.hps_config is None:
+            raise AttributeError("Cannot train without HPS file config.")
+
         model = getattr(module, "model", None)
-        
-        if not model:
+        if model is None:
             raise AttributeError("'self.model' needs to be declared in the AcceleratorModule class.")
         
         cfg = read(self.hps_config)
         hps = cfg["hps"]
         optim = hps["optim"]
-        schlr = hps["scheduler"]
+        schlr = hps["scheduler"] if "scheduler" in hps else None
 
-        if not self.model_path:
+        if self.model_path is not None:
             self.model_path = cfg["version"]
 
         if self.model_saving:
             os.makedirs(self.model_path, exist_ok=True)
 
-        train_dataloader = DataLoader(train_dataset, batch_size=hps["batch_size"], shuffle=True)
+        best_train_loss = float("inf")
+        best_valid_loss = float("inf")
+        status_epoch = 0
+        current_epoch_step = 0
+        global_step = 0
+
+        if self.resume:
+            status = read_status(f"{self.checkpoint}/status.json")
+            best_valid_loss = status["best_valid_loss"]
+            best_train_loss = status["best_train_loss"]
+            status_epoch = status["epoch"]
+            global_step = status["global_step"]
+
+        if module._implemented_collate_fn:
+            self.collate_fn = module.collate_fn
+        train_dataloader = DataLoader(train_dataset, batch_size=hps["batch_size"], shuffle=self.shuffle_train, collate_fn=self.collate_fn)
 
         val_dataloader = None
         if val_dataset is not None:
-            val_dataloader = DataLoader(val_dataset, batch_size=hps["batch_size"], shuffle=True)
+            val_dataloader = DataLoader(val_dataset, batch_size=hps["batch_size"], shuffle=self.shuffle_validation, collate_fn=self.collate_fn)
         else:
             if self.model_saving == "best_valid_loss":
                 self.model_saving = "best_train_loss"
-        
-        optimizer = getattr(torch.optim, optim["type"])(model.parameters(), lr=float(optim["lr"]), weight_decay=float(optim["weight_decay"]))
+
+        optimizer = self._get_optimizer(optim, model)
         scheduler = None
-        if "type" in schlr:
-            scheduler = getattr(torch.optim.lr_scheduler, schlr["type"])(optimizer, max_lr=float(schlr["max_lr"]), steps_per_epoch=len(train_dataloader), epochs=hps["epochs"])
+        if schlr is not None:
+            scheduler = self._get_scheduler(schlr, optimizer, -1, len(train_dataloader), hps["epochs"])
+            # -1 for last_epoch since Accelerate will take care of recovering the progress
 
         if "log_every" in cfg:
             self.log_every = cfg["log_every"]
-            warnings.warn("'log_every' parameter in HPS config file is deprecated and it'll be removed in "
-                          "v1.0.0. Use 'log_every' in Trainer constructor instead.\n"
+            warnings.warn("'log_every' parameter in HPS config file is deprecated and it'll be removed in v1.0.0 "
+                          "Use 'log_every' in Trainer constructor instead.\n"
                           "Using 'log_every' from HPS config file.")
 
         model, train_dataloader, val_dataloader, optimizer, scheduler = self.accelerator.prepare(
             model, train_dataloader, val_dataloader, optimizer, scheduler
         )
+        if scheduler:
+            self.accelerator.register_for_checkpointing(scheduler)
         self.accelerator.init_trackers(cfg["version"])
 
-        best_valid_loss = float("inf")
-        best_train_loss = float("inf")
-        status_epoch = 0
-
         if self.resume:
             if os.path.exists(self.checkpoint):
                 self.accelerator.load_state(self.checkpoint)
-                status = read_status(f"{self.checkpoint}/status.json")
-                best_valid_loss = status["best_valid_loss"]
-                best_train_loss = status["best_train_loss"]
-                status_epoch = status["epoch"]
             else:
-                print(f"{self.checkpoint} does not exist. Starting process from zero...")
+                raise FileNotFoundError(f"{self.checkpoint} was not found.")
 
         epochs = hps["epochs"]
-        global_step = 0
-        eval_step = len(train_dataloader) // len(val_dataloader)
+        eval_step = (len(train_dataloader) // len(val_dataloader)) if val_dataloader else None
         for epoch in range(status_epoch, epochs):
             eval_global_step = global_step
             model.train()
-            train_losses = []
-            for step, batch in tqdm(enumerate(train_dataloader, 1), total=len(train_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
-                loss = module.training_step(batch)
-
-                if self.grad_accumulation_steps > 1:
-                    loss /= self.grad_accumulation_steps
-
-                train_losses.append(loss.item())
-                if step % self.log_every == 0:
-                    self.accelerator.log({"loss": {"train": loss.item()}}, step=global_step)
-
-                self.accelerator.backward(loss)
-
-                if (step % self.grad_accumulation_steps == 0) or (step == len(train_dataloader)):
-                    optimizer.step()
-                    if scheduler:
-                        scheduler.step()
-                    optimizer.zero_grad(set_to_none=self.set_to_none)
-
-                global_step += 1
+            train_losses = [] 
+            for step, batch in tqdm(
+                iterable=enumerate(train_dataloader, current_epoch_step+1),
+                total=len(train_dataloader),
+                desc=f"Epoch {epoch}/{epochs}",
+                unit="batch"
+            ):
+                global_step, current_epoch_step = self._train_logic(
+                    module, optimizer, batch, train_losses, step, scheduler, train_dataloader, global_step, current_epoch_step
+                )
             
             if all([val_dataloader, getattr(module, "validation_step", False)]):
                 model.eval()
                 eval_losses = []
                 with torch.no_grad():
-                    for step, batch in tqdm(enumerate(val_dataloader, 1), total=len(val_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
-                        loss = module.validation_step(batch)
-
-                        eval_losses.append(loss.item())
-                        if step % self.log_every == 0:
-                            self.accelerator.log({"loss": {"valid": loss.item()}}, step=eval_global_step)
-
-                        eval_global_step += eval_step
+                    for step, batch in tqdm(
+                        iterable=enumerate(val_dataloader, 1),
+                        total=len(val_dataloader),
+                        desc=f"Epoch {epoch}/{epochs}",
+                        unit="batch"
+                    ):
+                        eval_global_step = self._validation_logic(
+                            module, batch, eval_losses, step, eval_step, eval_global_step
+                        )
 
                 best_valid_loss, best_train_loss = self._save_model_on_criteria(
                     model, eval_losses, train_losses, best_valid_loss, best_train_loss
                 )
             else:
                 if self.model_saving:
                     avg_train_loss = np.mean(train_losses)
                     if avg_train_loss < best_train_loss:
+                        self.accelerator.print("Saving model...")
                         self._save_model(model, best_valid_loss, best_train_loss)
                         best_train_loss = avg_train_loss
 
-            if self.enable_checkpointing and epoch % self.checkpoint_every == 0:
-                self.accelerator.save_state(self.checkpoint)
-                save_status({
-                    "best_valid_loss": best_valid_loss,
-                    "best_train_loss": best_train_loss,
-                    "epoch": epoch
-                }, to=f"{self.checkpoint}/status.json")
+            self._save_checkpoint(epoch+1, best_valid_loss, best_train_loss, global_step)
 
         self.accelerator.end_training()
 
+    def eval(self, module, val_dataset: Dataset, batch_size=1) -> float:
+        from torch.utils.data import DataLoader
+
+        model = getattr(module, "model", None)
+        if model is None:
+            raise AttributeError("'self.model' needs to be declared in the AcceleratorModule class.")
+        
+        if module._implemented_collate_fn:
+            self.collate_fn = module.collate_fn
+        val_dataloader = DataLoader(val_dataset, batch_size=batch_size, shuffle=False, collate_fn=self.collate_fn)
+
+        model, val_dataloader = self.accelerator.prepare(
+            model, val_dataloader
+        )
+
+        model.eval()
+        eval_losses = []
+        with torch.no_grad():
+            for batch in tqdm(iterable=val_dataloader, total=len(val_dataloader), desc=f"Evaluating", unit="batch"):
+                loss = module.validation_step(batch)
+                loss = self.accelerator.gather_for_metrics(loss).cpu().numpy()
+                eval_losses.append(np.mean(loss))
+        
+        avg_eval_loss = np.mean(eval_losses)
+
+        return avg_eval_loss
     
+    def _train_logic(
+            self, module, optimizer, batch, train_losses, step, scheduler, dataloader, global_step, current_epoch_step
+    ):
+        loss = module.training_step(batch)
+        if loss is None:
+            loss = module.step(batch)
+
+        if self.grad_accumulation_steps > 1:
+            loss /= self.grad_accumulation_steps
+
+        train_losses.append(loss.item())
+        if step % self.log_every == 0 and self.accelerator.is_main_process:
+            self.accelerator.log({"loss": {"train": loss}}, step=global_step)
+        
+        self.accelerator.backward(loss)
+
+        if (step % self.grad_accumulation_steps == 0) or (step == len(dataloader)):
+            optimizer.step()
+            if scheduler is not None:
+                scheduler.step()
+            optimizer.zero_grad(set_to_none=self.set_to_none)
+
+        global_step += 1
+        current_epoch_step += 1
+
+        return global_step, current_epoch_step
+    
+    def _validation_logic(self, module, batch, eval_losses, step, eval_step, eval_global_step):
+        loss = module.validation_step(batch)
+        if loss is None:
+            loss = module.step(batch)
+
+        eval_losses.append(loss.item())
+        if step % self.log_every == 0:
+            self.accelerator.log({"loss": {"valid": loss.item()}}, step=eval_global_step)
+
+        eval_global_step += eval_step
+
+        return eval_global_step
+
     def _save_model(self, model, best_valid_loss, best_train_loss):
         state_dict = self.accelerator.get_state_dict(model)
         unwrapped_model = self.accelerator.unwrap_model(model)
         unwrapped_model.save_pretrained(
             self.model_path,
             is_main_process=self.accelerator.is_main_process,
             state_dict=state_dict,
-            max_shard_size="10GB",
+            max_shard_size=self.max_shard_size,
             save_function=self.accelerator.save,
-            safe_serialization=False # if True, some tensors will not be saved
+            safe_serialization=self.safe_serialization
         )
 
         save_status({
             "best_valid_loss": best_valid_loss,
             "best_train_loss": best_train_loss,
         }, to=f"{self.model_path}/status.json")
 
@@ -313,16 +476,16 @@
         if self.model_saving is None:
             return
 
         avg_valid_loss = np.mean(eval_losses)
         avg_train_loss = np.mean(train_losses)
 
         saving_criteria = {
-            "best_valid_loss": (avg_valid_loss < best_valid_loss),
-            "best_train_loss": (avg_train_loss < best_train_loss),
+            "best_valid_loss": avg_valid_loss < best_valid_loss and avg_valid_loss < self.model_saving_below_loss,
+            "best_train_loss": avg_train_loss < best_train_loss and avg_train_loss < self.model_saving_below_loss,
             "always": True
         }
 
         if self.model_saving in saving_criteria:
             if saving_criteria[self.model_saving]:
                 self._save_model(model, best_valid_loss, best_train_loss)
         else:
@@ -330,8 +493,53 @@
                               "'best_valid_train_loss', "
                               "'best_train_loss', or "
                               "'always'.")
         
         return (
             avg_valid_loss if avg_valid_loss < best_valid_loss else best_valid_loss,
             avg_train_loss if avg_train_loss < best_train_loss else best_train_loss
-        )
+        )
+    
+    def _fix_kwargs(self, dictionary: dict):
+        for k, v in dictionary.items():
+            if isinstance(v, list):
+                dictionary[k] = [float(item) for item in v if isinstance(item, str)]
+            elif isinstance(v, str):
+                try:
+                    dictionary[k] = float(v)
+                except ValueError:
+                    continue
+
+    def _save_checkpoint(self, epoch, best_valid_loss, best_train_loss, global_step):
+        if (self.enable_checkpointing and epoch % self.checkpoint_every == 0):
+            self.accelerator.print("Saving checkpoint...")
+            self.accelerator.save_state(self.checkpoint, safe_serialization=self.safe_serialization)
+            save_status({
+                "best_valid_loss": best_valid_loss,
+                "best_train_loss": best_train_loss,
+                "epoch": epoch,
+                "global_step": global_step
+            }, to=f"{self.checkpoint}/status.json")
+
+    def _get_optimizer(self, optim: dict, model):
+        t = optim["type"]
+        optim_kwargs = optim.copy()
+        del optim_kwargs["type"]
+        self._fix_kwargs(optim_kwargs)
+
+        return OPTIMIZERS[t](model.parameters(), **optim_kwargs)
+
+    def _filter_kwargs(self, _kwargs: dict, fn):
+        return {k:v for k,v in _kwargs.items() if k in fn.__init__.__code__.co_varnames}
+
+    def _get_scheduler(self, schlr: dict, optimizer, last_epoch, steps_per_epoch, epochs):
+        t = schlr["type"]
+        schlr_kwargs = schlr.copy()
+        del schlr_kwargs["type"]
+        self._fix_kwargs(schlr_kwargs)
+
+        schlr_kwargs["last_epoch"] = last_epoch
+        schlr_kwargs["steps_per_epoch"] = steps_per_epoch
+        schlr_kwargs["epochs"] = epochs
+        filtered_kwargs = self._filter_kwargs(schlr_kwargs, SCHEDULERS[t])
+
+        return SCHEDULERS[t](optimizer, **filtered_kwargs)
```

