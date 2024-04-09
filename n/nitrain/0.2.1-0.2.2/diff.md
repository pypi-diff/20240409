# Comparing `tmp/nitrain-0.2.1.tar.gz` & `tmp/nitrain-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrain-0.2.1.tar", max compression
+gzip compressed data, was "nitrain-0.2.2.tar", max compression
```

## Comparing `nitrain-0.2.1.tar` & `nitrain-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,44 @@
--rw-r--r--   0        0        0     1073 2024-03-14 23:40:42.517034 nitrain-0.2.1/LICENSE
--rw-r--r--   0        0        0    12441 2024-03-14 23:40:42.517034 nitrain-0.2.1/README.md
--rw-r--r--   0        0        0       96 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/__init__.py
--rw-r--r--   0        0        0      333 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/__init__.py
--rw-r--r--   0        0        0     8673 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/bids_dataset.py
--rw-r--r--   0        0        0     1756 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/csv_dataset.py
--rw-r--r--   0        0        0      870 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/fetch_data.py
--rw-r--r--   0        0        0     8487 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/folder_dataset.py
--rw-r--r--   0        0        0     6091 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/google_cloud_dataset.py
--rw-r--r--   0        0        0      786 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/memory_dataset.py
--rw-r--r--   0        0        0      733 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/datasets/random_transform_dataset.py
--rw-r--r--   0        0        0       73 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/explainers/__init__.py
--rw-r--r--   0        0        0       27 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/explainers/explainer.py
--rw-r--r--   0        0        0       96 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/loaders/__init__.py
--rw-r--r--   0        0        0     4741 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/loaders/dataset_loader.py
--rw-r--r--   0        0        0     2672 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/loaders/keras_loader.py
--rw-r--r--   0        0        0      569 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/loaders/torch_loader.py
--rw-r--r--   0        0        0      122 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/models/__init__.py
--rw-r--r--   0        0        0     2327 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/models/fetch_architecture.py
--rw-r--r--   0        0        0      612 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/models/fetch_pretrained.py
--rw-r--r--   0        0        0      375 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/__init__.py
--rw-r--r--   0        0        0      962 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/base_sampler.py
--rw-r--r--   0        0        0     2836 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/block_sampler.py
--rw-r--r--   0        0        0     2643 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/patch_sampler.py
--rw-r--r--   0        0        0     2021 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/slice_patch_sampler.py
--rw-r--r--   0        0        0     1757 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/samplers/slice_sampler.py
--rw-r--r--   0        0        0       67 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/trainers/__init__.py
--rw-r--r--   0        0        0      260 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/trainers/cloud_trainer.py
--rw-r--r--   0        0        0      643 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/trainers/model_trainer.py
--rw-r--r--   0        0        0      376 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/__init__.py
--rw-r--r--   0        0        0     4785 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/ants_transforms.py
--rw-r--r--   0        0        0      475 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/base_transform.py
--rw-r--r--   0        0        0     5408 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/intensity_transforms.py
--rw-r--r--   0        0        0     2357 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/spatial_transforms.py
--rw-r--r--   0        0        0     5297 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/structural_transforms.py
--rw-r--r--   0        0        0     1553 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/transforms/utility_transforms.py
--rw-r--r--   0        0        0      479 2024-03-14 23:40:42.521034 nitrain-0.2.1/nitrain/utils.py
--rw-r--r--   0        0        0      708 2024-03-14 23:40:42.525034 nitrain-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    13653 1970-01-01 00:00:00.000000 nitrain-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-04-09 10:29:00.544266 nitrain-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10716 2024-04-09 10:29:00.544266 nitrain-0.2.2/README.md
+-rw-r--r--   0        0        0      121 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/base_dataset.py
+-rw-r--r--   0        0        0     4070 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/bids_dataset.py
+-rw-r--r--   0        0        0     6925 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/configs.py
+-rw-r--r--   0        0        0     3027 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/csv_dataset.py
+-rw-r--r--   0        0        0     3847 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/folder_dataset.py
+-rw-r--r--   0        0        0     7700 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/google_cloud_dataset.py
+-rw-r--r--   0        0        0     1574 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/memory_dataset.py
+-rw-r--r--   0        0        0     5853 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/platform_dataset.py
+-rw-r--r--   0        0        0     2250 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/datasets/utils.py
+-rw-r--r--   0        0        0      125 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/explainers/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/explainers/occlusion_explainer.py
+-rw-r--r--   0        0        0       86 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/__init__.py
+-rw-r--r--   0        0        0     4930 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/dataset_loader.py
+-rw-r--r--   0        0        0      868 2024-04-09 10:29:00.552266 nitrain-0.2.2/nitrain/loaders/keras_loader.py
+-rw-r--r--   0        0        0      401 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/loaders/torch_loader.py
+-rw-r--r--   0        0        0      145 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/__init__.py
+-rw-r--r--   0        0        0     2293 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/fetch_architecture.py
+-rw-r--r--   0        0        0      728 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/fetch_pretrained.py
+-rw-r--r--   0        0        0      107 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/models/load.py
+-rw-r--r--   0        0        0     7021 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/platform.py
+-rw-r--r--   0        0        0      375 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/base_sampler.py
+-rw-r--r--   0        0        0     2828 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/block_sampler.py
+-rw-r--r--   0        0        0     2615 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/patch_sampler.py
+-rw-r--r--   0        0        0     1993 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/slice_patch_sampler.py
+-rw-r--r--   0        0        0     2421 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/samplers/slice_sampler.py
+-rw-r--r--   0        0        0      153 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/cloud_trainer.py
+-rw-r--r--   0        0        0     3379 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/model_trainer.py
+-rw-r--r--   0        0        0     5825 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/trainers/platform_trainer.py
+-rw-r--r--   0        0        0      376 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/__init__.py
+-rw-r--r--   0        0        0     5189 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/ants_transforms.py
+-rw-r--r--   0        0        0      475 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/base_transform.py
+-rw-r--r--   0        0        0     5620 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/intensity_transforms.py
+-rw-r--r--   0        0        0     4672 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/spatial_transforms.py
+-rw-r--r--   0        0        0     5865 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/structural_transforms.py
+-rw-r--r--   0        0        0     1553 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/transforms/utility_transforms.py
+-rw-r--r--   0        0        0      674 2024-04-09 10:29:00.556266 nitrain-0.2.2/nitrain/utils.py
+-rw-r--r--   0        0        0      724 2024-04-09 10:29:00.556266 nitrain-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11944 1970-01-01 00:00:00.000000 nitrain-0.2.2/PKG-INFO
```

### Comparing `nitrain-0.2.1/README.md` & `nitrain-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,82 @@
 # Nitrain - a framework for medical imaging-native AI
 
 [![Coverage Status](https://coveralls.io/repos/github/ncullen93/nitrain/badge.svg?branch=main)](https://coveralls.io/github/ncullen93/nitrain?branch=main)
+[![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
-Nitrain is a medical imaging-native framework for training and visualizing deep learning models. It provides tools for sampling and augmenting neuroimaging datasets, training deep learning models on neuroimages, and visualizing or explaining deep learning model results in a neuroimaging context. Nitrain also makes it easy to use pre-trained models for training or integration into imaging pipelines.
+Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
+
+You can also train models HIPAA-compliantly in the cloud using nitrain. You are encouraged to make your fitted models available to the community via nitrain, or you can easily use other's pretrained models for fine-tuning or standard image processing.
 
 <br />
 
 ## Installation
 
-The package can be installed from github:
+The latest release of nitrain can be installed from pypi:
+
+```
+pip install nitrain
+```
+
+Or you can install the latest development version directly from github:
 
 ```
 python -m pip install git+github.com/ncullen93/nitrain.git
 ```
 
 ### Dependencies
 
-The nitrain package is developed with Python3.10 as the focus. In terms of dependencies, it requires `ants` and `antspynet` and works with either tensorflow/keras or pytorch. Support for Keras 3 is on the roadmap.
+The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
 
 <br />
 
 ## Quickstart
 
-Here is a canonical example of using nitrain to give you a quick overview. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
-
-Alternatively, you can check out the [tutorials](github.com/ncullen93/nitrain) for an in-depth introduction to everything that nitrain has to offer or the [examples](github.com/ncullen93/nitrain) for self-contained, end-to-end examples of how to perform common deep learning tasks.
+Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
 
 ```python
 from nitrain import datasets, loaders, models, trainers, transforms as tx
 
-#### Brain-age example ####
-
 # create dataset from folder of images + participants file
 dataset = datasets.FolderDataset(base_dir='ds004711',
-                            x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
-                            y={'file': 'participants.tsv',
-                                    'column': 'age'},
-                            x_transforms=[nit.ResizeImage((64,64,64)),
-                                          nit.NormalizeIntensity(0,1)])
+                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
+                                 y={'file': 'participants.tsv',
+                                         'column': 'age'},
+                                 x_transforms=[tx.Resize((64,64,64)),
+                                               tx.NormalizeIntensity(0,1)])
 
 # create loader with random transforms
 loader = loaders.DatasetLoader(dataset,
-                           batch_size=32,
-                           shuffle=True,
-                           x_transforms=[nit.RandomSlice(axis=2),
-                                         nit.RandomNoise(sd=0.2)])
+                               images_per_batch=4,
+                               shuffle=True,
+                               sampler=samplers.SliceSampler(batch_size=32, axis=2)
+                               x_transforms=[tx.RandomNoise(sd=0.2)])
 
 # create model from architecture
-architecture_fn = models.fetch_architecture('alexnet', task='continuous_prediction')
-model = architecture_fn(layers=[128, 64, 32, 10], n_outcomes=1)
+arch_fn = models.fetch_architecture('alexnet', dim=2)
+model = arch_fn(input_image_size=(64,64,1),
+                number_of_outcomes=1,
+                mode='regression')
 
 # create trainer and fit model
 trainer = trainers.ModelTrainer(model,
-                           loss='mse',
-                           optimizer='adam',
-                           lr=1e-3,
-                           callbacks=[nit.EarlyStopping(),
-                                      nit.ModelCheckpoints(freq=25)])
+                                loss='mse',
+                                optimizer='adam',
+                                lr=1e-3,
+                                callbacks=[utils.EarlyStopping(),
+                                           utils.ModelCheckpoints(freq=25)])
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-models.register_model(trainer.model, 'nick/t1-brainage-model')
+models.register_model(trainer.model, 'nick/t1-brain-age')
 ```
 
+A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
+
 <br />
 
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
 - [Datasets and Loaders](#datasets-and-loaders)
@@ -74,90 +84,89 @@
 - [Transforms](#transforms)
 - [Architectures and pretrained models](#architectures-and-pretrained-models)
 - [Model trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
-## Datasets and Loaders
-
-Nitrain provides extensive functionality to help you sample neuroimages with imaging-native data augmentation techniques. Our focus is on speed, meaning you never have to convert your neuroimages into numpy arrays.
+### Datasets and Loaders
 
-You start by creating a `dataset` from wherever your images are stored -- in a local folder, in a bids folder, in memory, on a cloud service, etc. Say that your data is stored in a local folder. To grab inputs (`x`), supply a dictionary with a glob pattern and optional exclude pattern. To grab outputs (`y`), specify a dataframe file to read and a column to pull from that dataframe. Both x and y can be image configs, and they can also be lists of configs if you want to grab multiple images at once.
+Datasets help you read in your images from wherever they are stored -- in a local folder with BIDS or datalad, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, BIDS entities, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
-from nitrain import datasets
-dataset = datasets.FolderDataset(base_dir='ds004711',
+from nitrain import datasets, transforms as tx
+
+dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
                                  x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
-                                 x_transforms=[tx.Resample((4,4,4), use_spacing=True),
-                                               tx.RangeNormalize(0,1)])
-
+                                 x_transforms=[tx.Resample((64,64,64))])
 ```
 
-Notice also that there the `x_transforms` argument has been supplied. These transforms are applied every time the input image is read into file. These are meant to be "fixed" transforms - i.e., not random - because the results can be cached to speed up sampling in the long-run.
-
-Once you have a dataset, you can grab images from it as you would with any iterator. This gives you the first input image (with transforms applied) and the first age value.
+Although you will rarely need to do this, data can be read into memory by indexing the dataset:
 
 ```python
-x, y = dataset[0]
+x_raw, y_raw = dataset[:3]
 ```
 
-The dataset can then be passed into a `loader` in order to actually sample batches. With loaders, you can specify parameters like batch size and whether to expand dims. You can also pass in more transforms that will be applied at each batch sampling. These transforms, in contrast, are meant to be random data augmentation transforms.
+To prepare your images for batch generation during training, you pass the dataset into one the loaders. Here is where you can also pass in random transforms that will act as data augmentation. If you want to train on slices, patches, or blocks of images then you will additionally provide a sampler. The different samplers are explained later.
 
 ```python
+from nitrain import loaders, samplers
+
 loader = loaders.DatasetLoader(dataset,
-                               batch_size=32,
-                               x_transforms=[tx.RandomSmoothing(0, 1)],
-                               expand_dims=-1)
+                               images_per_batch=32,
+                               x_transforms=[tx.RandomSmoothing(0, 1)])
 
 # loop through all images in batches for one epoch
 for x_batch, y_batch in loader:
         print(y_batch)
 ```
 
-The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework. Note that we also have loaders geared specifically towards those frameworks to allow you to use some additional loading functionality that they provide.
+The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework.
 
 <br />
 
-## Samplers
+### Samplers
 
 Samplers allow you to keep the same dataset + loader workflow that batches entire images and applies transforms to them, but then expand on those transformed image batches to create special "sub-batches".
 
 For instance, samplers let you serve batches of 2D slices from 3D images, or 3D blocks from 3D images, and so forth. Samplers are essntial for common deep learning workflows in medical imaging where you often want to train a model on only parts of the image at once.
 
-All you have to do is supply a sampler instance to your dataset loader. Here is an example:
-
 ```python
-from nitrain import loaders, samplers as sp, transforms as tx
+from nitrain import loaders, samplers, transforms as tx
 loader = loaders.DatasetLoader(dataset,
-                               batch_size=3,
+                               images_per_batch=4,
                                x_transforms=[tx.RandomSmoothing(0, 1)],
-                               expand_dims=-1,
-                               sampler=sp.SliceSampler(sub_batch_size=24, axis=0, shuffle=True))
+                               sampler=samplers.SliceSampler(batch_size=24, axis=2))
 ```
 
-What happens is that we start with the ~190 images from the dataset, but 3 images will be read in from file at a time. Then, all possible 2D slices will be created from those 3 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 3 images) have been served, the loader will move on to the next 3 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
-
-The important thing to remember is that the batch size your model will see is 24. In total, then, there are (n_images \* n_slices_per_image / sampler_batch_size) total batches in one epoch instead of (n_images / loader_batch_size) like there normally are.
+What happens is that we start with the ~190 images from the dataset, but 4 images will be read in from file at a time. Then, all possible 2D slices will be created from those 4 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 4 images) have been served, the loader will move on to the next 4 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
 
 <br />
 
-## Transforms
+### Transforms
 
-The philosophy of nitrain is to be as neuroimaging-native as possible. That means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to numpy arrays.
+The philosophy of nitrain is to be medical imaging-native. This means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to arrays / tensors for model consumption.
 
-The nitrain package supports an extensive amount of neuroimaging-based transforms:
+The nitrain package supports an extensive amount of medical imaging transforms:
 
 - Affine (Rotate, Translate, Shear, Zoom)
 - Flip, Pad, Crop, Slice
 - Noise
 - Motion
 - Intensity normalization
 
+You can create your own transform with the `CustomTransform` class:
+
+```python
+from nitrain import transforms as tx
+
+my_tx = tx.CustomTransform(lambda x: x * 2)
+```
+
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
 import ants
 import numpy as np
 from nitrain import transforms as tx
 
@@ -165,33 +174,17 @@
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
 ants.plot_grid(np.array(imgs).reshape(4,3))
 ```
 
-Writing your own transform is extremely easy! Just remember that the transform will operate on the `antsImage` type and that you should inherit from the `BaseTransform` class.
-
-```python
-from nitrain.transforms import BaseTransform
-
-class CoolTransform(BaseTransform):
-        def __init__(self, parameters):
-                self.parameters = parameters
-        def __call__(self, image):
-                image = my_function(image, self.parameters)
-                return image
-
-tx_fn = CoolTransform(parameters=123)
-img_transformed = tx_fn(img)
-```
-
 <br />
 
-## Architectures and pretrained models
+### Architectures and pretrained models
 
 The nitrain package provides an interface to an extensive amount of deep learning model architectures for all kinds of tasks - regression, classification, image-to-image generation, segmentation, autoencoders, etc.
 
 The available architectures can be listed and explored:
 
 ```python
 from nitrain import models
@@ -206,66 +199,47 @@
 vgg_fn = models.fetch_architecture('vgg', dim=3)
 vgg_model = vgg_fn((128, 128, 128, 1))
 
 autoencoder_fn = models.fetch_architecture('autoencoder')
 autoencoder_model = autoencoder_fn((784, 500, 500, 2000, 10))
 ```
 
-There is also a large collection of pretrained models available as a starting point for your training or simply to use for inference. If your dataset is small (<500 participants) than you may especially benefit from using pre-trained models.
-
-Similarly to architectures, you fetch a pretrained model based on its name. The result of fetching a pretrained model is the actual instantianed model with the pretrained weights loaded.
-
-```python
-from nitrain import models
-model = models.fetch_pretrained('basic-t1')
-```
-
-If you have trained an interested deep learning model on neuroimages and would like to share it with the community, it is possible to do so directly from nitrain. Any model you share will be hosted and available for use by anyone else through the `fetch_pretrained` function.
-
-```python
-from nitrain import models
-models.register_pretrained(model, 'my-cool-model')
-```
-
 <br />
 
-## Model trainers
+### Trainers
 
-After you have either fetched and created an architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
+After you have created a model from a nitrain architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
 
-To train with Pytorch, use the `nitrain.torch` module:
+Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `ModelTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
 
 ```python
-import nitrain
-```
-
-To train with Keras, use the `nitrain.keras` module:
+trainer = trainers.ModelTrainer(model=vgg_model, task='regression')
+trainer.fit(loader, epochs=10)
 
-```python
-import nitrain
+# access fitted model
+print(trainer.model)
 ```
 
-To train with Tensorflow, use the `nitrain.tensorflow` module:
+If you have signed up for an account at [nitrain.dev](https://www.nitrain.dev) then you can also train your model in the cloud using the `PlatformTrainer` class. All training takes place on HIPAA-compliant GPU servers with competitive pricing.
 
 ```python
-import nitrain
+trainer = trainers.PlatformTrainer(model=model, task='regression',
+                                name='brain-age', resource='gpu-small')
+trainer.fit(loader, epochs=10)
+
+# check job status
+print(trainer.status)
 ```
 
 <br />
 
-## Explainers
+### Explainers
 
 The idea that deep learning models are "black boxes" is out-dated, particularly when it comes to images. There are numerous techiques to help you understand which parts of the brain a trained model is weighing most when making predictions.
 
-One such technique is called the occlusion method, where you systematically "black out" different patches of an input image and see how the model prediction is affected. The idea is that when, when occluded, important areas result in a large change in model prediction compared to the original image.
-
 Nitrain provides tools to perform this techique - along with many others - and can help you visualize the results of such explainability experiments directly in brain space. Here is what that might look like:
 
-```python
-from nitrain import explain
-```
-
 <br />
 
 ## Contributing
 
 If you would like to contribute to nitrain, we would be extremely thankful. The best way to start is by posting an issue to discuss your proposed feature.
```

### Comparing `nitrain-0.2.1/nitrain/datasets/folder_dataset.py` & `nitrain-0.2.2/nitrain/datasets/google_cloud_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,221 +1,168 @@
 import warnings
-from parse import parse
-import copy
+import re
 import os
-import json
-import ants
-import datalad.api as dl
-import numpy as np
-import pandas as pd
 import glob
+import tempfile
+import pandas as pd
+import numpy as np
 from fnmatch import fnmatch
-
+from google.cloud import storage
+from google.oauth2 import service_account
 from torch.utils.data import Dataset
 
+import ants
 
 from .. import utils
 
 
-class FolderDataset:
+class GoogleCloudDataset:
     
     def __init__(self,
-                 base_dir, 
+                 bucket, 
+                 base_dir,
                  x,
                  y,
                  x_transforms=None,
                  y_transforms=None,
-                 datalad=False):
+                 credentials=None,
+                 fuse=False,
+                 lazy=False):
         """
         Initialize a nitrain dataset consisting of local filepaths.
         
         Arguments
         ---------
-        x : dict or list of dicts
-            Info used to grab the correct images from the folder. A list
-            of dicts means you want to return multiple images. This is helpful
-            if you need some other image(s) to help process the primary image - e.g.,
-            you can supply a list of 2-dicts to read in T1w images + the associated
-            mask. Then, you could use `x_transforms` to mask the T1w image and only
-            return the masked T1w image from the dataset.
-
         
         Example
         -------
-        >>> dataset = FolderDataset('ds000711', 
-                                    x={'datatype': 'anat', 'suffix': 'T1w'},
-                                    y={'file':'participants.tsv', 'column':'age'})
-        >>> model = nitrain.models.fetch_pretrained('t1-brainage', finetune=True)
-        >>> model.fit(dataset)
-        """        
+        >>> dataset = datasets.GoogleCloudDataset(bucket='ants-dev',
+                                         base_dir='datasets/nick-2/my-first-job', 
+                                         x={'pattern': '*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
+                                         y={'file': 'participants.tsv', 'column': 'age'})
+        """
+        if lazy:
+            self.bucket = bucket
+            self.base_dir = base_dir
+            self.x = None
+            self.x_config = x
+            self.y = None
+            self.y_config = y
+            self.x_transforms = x_transforms
+            self.y_transforms = y_transforms
+            self.credentials = credentials
+            self.fuse = fuse
+            self.lazy = True
+            return
+        
         x_config = x
         y_config = y
         
-        pattern = x_config['pattern']
-        glob_pattern = pattern.replace('{id}','*')
-        x = sorted(glob.glob(glob_pattern, root_dir=base_dir))
-        if 'exclude' in x_config.keys():
-            x = [file for file in x if not fnmatch(file, x_config['exclude'])]
-        
-        # TODO: support '{id}/*' but 
-        if '{id}' in pattern:
-            x_ids = [parse(pattern.replace('*','{other}'), file).named['id'] for file in x]
+        if fuse:
+            base_dir = os.path.join('/gcs/', bucket, base_dir)
+            if not base_dir.endswith('/'): 
+                base_dir += '/'
+            
+            # GET X
+            x = glob.glob(os.path.join(base_dir, x_config['pattern']))
+            x = [os.path.relpath(xx, base_dir) for xx in x]
+            if 'exclude' in x_config.keys():
+                x = [file for file in x if not fnmatch(file, x_config['exclude'])]
+            x_ids = [xx.split('/')[0] for xx in x]
+            x = [os.path.join('/gcs/', bucket, base_dir, file) for file in sorted(x)]
+            
+            if len(x) == 0:
+                raise Exception('Did not find any x values corresponding to the x config.')
+
+            # GET Y
+            y_file = os.path.join(base_dir, y_config['file'])
+            y_df = pd.read_csv(y_file, sep='\t')
+            
         else:
+            if isinstance(credentials, str):
+                credentials = service_account.Credentials.from_service_account_file(credentials)
+            if credentials is not None:
+                storage_client = storage.Client(credentials=credentials)
+            bucket_client = storage_client.bucket(bucket)
+        
+            # GET X
+            if not base_dir.endswith('/'): base_dir += '/'
+            x_blobs = storage_client.list_blobs(bucket, match_glob=f'{base_dir}{x_config["pattern"]}')
+            x = list([blob.name.replace(base_dir, '') for blob in x_blobs])
+            if 'exclude' in x_config.keys():
+                x = [file for file in x if not fnmatch(file, x_config['exclude'])]
             x_ids = [xx.split('/')[0] for xx in x]
-        x = [os.path.join(base_dir, file) for file in x]
-        
-        # GET Y
-        participants_file = os.path.join(base_dir, y_config['file'])
-        participants = pd.read_csv(participants_file, sep='\t')
-        
+            x = [os.path.join(base_dir, file) for file in sorted(x)]
+            
+            if len(x) == 0:
+                raise Exception('Did not find any x values corresponding to the x config.')
+
+            # GET Y
+            y_file = os.path.join(base_dir, y_config['file'])
+            y_blob = bucket_client.blob(y_file)
+            tmp_file = tempfile.NamedTemporaryFile()
+            y_blob.download_to_filename(tmp_file.name)
+            y_df = pd.read_csv(tmp_file.name, sep='\t')
+            tmp_file.close()
+            
+            # properties specific to non-fuse scenarios
+            self.credentials = credentials
+            self.storage_client = storage_client
+            self.bucket_client = bucket_client
+            self.tmp_dir = tempfile.TemporaryDirectory()
+
         # match x and y ids
-        p_col = participants.columns[0] # assume participant id is first row
-        participants = participants.sort_values(p_col)
-        all_y_ids = participants[p_col].to_numpy()
+        p_col = y_df.columns[0] # assume participant id is first row
+        y_df = y_df.sort_values(p_col)
+        all_y_ids = y_df[p_col].to_numpy()
         if len(x_ids) != len(all_y_ids):
             warnings.warn(f'Mismatch between x ids {len(x_ids)} and y ids {len(all_y_ids)} - finding intersection')
         y_ids = sorted(list(set(x_ids) & set(all_y_ids)))
-        
-        participants = participants[participants[p_col].isin(y_ids)]
-        y = participants[y_config['column']].to_numpy()
-        
+
+        y_df = y_df[y_df[p_col].isin(y_ids)]
+        y = y_df[y_config['column']].to_numpy()
+
         # remove x values that are not found in y
         x = [x[idx] for idx in range(len(x)) if x_ids[idx] in y_ids]
         x_ids = y_ids
-
-
-        if len(x) != len(y):
-            warnings.warn(f'len(x) [{len(x)}] != len(y) [{len(y)}]. Do some participants have multiple runs?')
         
+        self.bucket = bucket
         self.base_dir = base_dir
-        self.datalad = datalad
         self.x_config = x_config
         self.y_config = y_config
-        self.x_transforms = x_transforms
-        self.y_transforms = y_transforms
-        self.participants = participants
         self.x = x
-        self.x_ids = x_ids
         self.y = y
-        self.y_ids = y_ids
-        
-    def filter(self, expr, inplace=False):
-        """
-        Filter the dataset by column values in the participants file
-        """
-        ds = copy.copy(self)
-        
-        participants = ds.participants.query(expr)
-        
-        p_col = participants.columns[0] # assume participant id is first row
-        p_suffix = 'sub-' # assume participant col starts with 'sub-'
-        query_ids = [id.split('-')[1] for id in participants[p_col]]
-        
-        file_ids = ds.layout.get(return_type='id', target='subject', **ds.x)
-        ids = sorted(list(set(file_ids).intersection(query_ids)))
-
-        # only keep ids that are in the participants file
-        x = ds.layout.get(return_type='filename', subject=ids, **ds.x)
-        
-        # GET Y
-        p_col = participants.columns[0] # assume participant id is first row
-        p_suffix = 'sub-' # assume participant col starts with 'sub-'
-        participants = participants[participants[p_col].isin([p_suffix+id for id in ids])]
-        y = participants[ds.y['column']].to_numpy()
-        
-        # make changes to instance
-        ds.participants = participants
-        ds.x = x
-        ds.y = y
-        return ds
-    
-    def precompute_transforms(self, desc='precompute'):
-        """
-        Compute all transforms on the input images and save
-        them to file as a derivative. The original filepaths
-        will be replaced with paths to the transformed images.
-        Precomputing transforms is a good idea if you plan to
-        read from disk.
-        """
-        if self.x_transforms is None:
-            raise Exception('No transforms set, so nothing to precompute.')
-        
-        # create derivatives/nitrain directory if necessary
-        derivatives_dir = os.path.join(self.base_dir, 'derivatives/')
-        save_dir = os.path.join(derivatives_dir, 'nitrain/')
-
-        if not os.path.exists(derivatives_dir):
-            os.mkdir(derivatives_dir)
-        if not os.path.exists(save_dir):
-            os.mkdir(save_dir)
-            
-            data_description = {"Name": "nitrain precomputed transforms",
-                                "BIDSVersion": "v1.8.0 (2022-10-29)", 
-                                "DatasetType": "derivatives",
-                                "GeneratedBy": [{"Name": "nitrain precomputed transforms"}]}
-            with open(os.path.join(save_dir, "dataset_description.json"), "w") as outfile: 
-                json.dump(data_description, outfile, indent=1)
-        
-        # make sure files are downloaded
-        files = self.x
-        ds = dl.Dataset(path = self.base_dir)
-        res = ds.get(files)
-        
-        for file in files:
-            img = ants.image_read(file)
-            
-            if self.x_transforms:
-                for x_tx in self.x_transforms:
-                    img = x_tx(img)
-            
-            file_ending = file.replace(f'{self.base_dir}/', '')
-            
-            try:
-                os.makedirs(os.path.dirname(os.path.join(save_dir, file_ending)))
-            except:
-                pass
-            
-            # add `desc` entity manually because `layout.build_path` doesnt work with new entities?
-            suffix = self.layout.parse_file_entities(file)['suffix']
-            save_filename = os.path.join(save_dir, 
-                                         file_ending.replace(suffix, 
-                                                             f'desc-{desc}_{suffix}'))
-            ants.image_write(img, save_filename)
-        
-        # add derivative layout
-        try:
-            self.layout.add_derivatives(os.path.join(self.base_dir, 'derivatives/nitrain'))
-        except:
-            pass
-        
-        # replace existing filename with the transformed ones from derivatives/nitrain
-        config = self.x_config
-        config['desc'] = desc
-        self.x = self.layout.derivatives['nitrain'].get(return_type='filename', **config)
-        self.x = config
-        self.x_transforms = None
+        self.x_transforms = x_transforms
+        self.y_transforms = y_transforms
+        self.fuse = fuse
+        self.lazy = False
 
     def __getitem__(self, idx):
         files = self.x[idx]
         if not isinstance(idx, slice):
             files = [files]
         y = self.y[idx]
         
         if self.y_transforms is not None:
             for y_tx in self.y_transforms:
                 y = y_tx(y)
         
-        # make sure files are downloaded
-        if self.datalad:
-            ds = dl.Dataset(path = self.base_dir)
-            res = ds.get(files)
-        
         x = []
         for file in files:
-            img = ants.image_read(file)
+            # if on vertex, file will be available to access. otherwise, download it to local tmp dir.
+            if self.fuse:
+                local_filepath = file
+            else:
+                local_filepath = os.path.join(self.tmp_dir.name, file)
+                if not os.path.exists(local_filepath):
+                    os.makedirs('/'.join(local_filepath.split('/')[:-1]), exist_ok=True)
+                    file_blob = self.bucket_client.blob(file)
+                    file_blob.download_to_filename(local_filepath)
+            
+            img = ants.image_read(local_filepath)
         
             if self.x_transforms:
                 for x_tx in self.x_transforms:
                     img = x_tx(img)
             
             x.append(img)
         
@@ -224,14 +171,50 @@
 
         return x, y
     
     def __len__(self):
         return len(self.x)
     
     def __copy__(self):
-        return FolderDataset(
-            path=self.base_dir,
-            x=self.x,
-            y=self.y,
-            x_transforms=self.x_transforms
+        return GoogleCloudDataset(
+            bucket = self.bucket,
+            base_dir = self.base_dir,
+            x = self.x_config,
+            y = self.y_config,
+            x_transforms = self.x_transforms,
+            y_transforms = self.y_transforms,
+            fuse = self.fuse,
+            credentials = self.credentials
         )
     
+    def __str__(self):
+        if self.lazy:
+            return f'GoogleCloudDataset (lazy) at {self.bucket}/{self.base_dir}'
+        else:
+            return f'GoogleCloudDataset with {len(self.x)} records at {self.bucket}/{self.base_dir}'
+    
+    def __repr__(self):
+        if self.x_transforms:
+            tx_repr = '[' + ', '.join([repr(x_tx) for x_tx in self.x_transforms]) + ']'
+            x_tx = f'x_transforms = {tx_repr},'
+        else:
+            x_tx = ''
+        
+        if self.y_transforms:
+            tx_repr = '[' + ', '.join([repr(y_tx) for y_tx in self.y_transforms]) + ']'
+            y_tx = f'y_transforms = {tx_repr},'
+        else:
+            y_tx = ''
+            
+        text = f"""GoogleCloudDataset(bucket = '{self.bucket}',
+                   base_dir = '{self.base_dir}',
+                   x = {self.x_config},
+                   y = {self.y_config},
+                   {x_tx}
+                   {y_tx}
+                   fuse = {self.fuse},
+                   credentials = None)"""
+        
+        text = re.sub(r'\n\s*\n', '\n\n', text)
+        text = re.sub('[\n]+', '\n', text) 
+        return text
+
```

### Comparing `nitrain-0.2.1/nitrain/datasets/google_cloud_dataset.py` & `nitrain-0.2.2/nitrain/datasets/platform_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,124 @@
 import warnings
 import os
 import glob
-import tempfile
 import pandas as pd
 import numpy as np
 from fnmatch import fnmatch
 from google.cloud import storage
 from google.oauth2 import service_account
-from torch.utils.data import Dataset
-
+from parse import parse
 import ants
 
-from .. import utils
-
 
-class GoogleCloudDataset:
+class PlatformDataset:
     
     def __init__(self,
-                 bucket, 
                  base_dir,
                  x,
                  y,
                  x_transforms=None,
                  y_transforms=None,
-                 credentials=None,
-                 fuse=False):
+                 fuse=False,
+                 credentials=None):
         """
         Initialize a nitrain dataset consisting of local filepaths.
         
         Arguments
         ---------
-        
+        x : dict or list of dicts
+            The config dict to specify how input files should be found. This generally
+            takes one of two forms:
+            - pattern-based: {'pattern': '*/anat/*_T1w.nii.gz'}
+            - filename-based: {'filenames': ['sub-001/anat/sub-001_T1w.nii.gz', '...']}
+            If the input to the model is multiple images, then x should be a list of configs:
+            e.g., [{'pattern': '*/anat/*_T1w.nii.gz'}, {'pattern': '*/anat/*_T2w.nii.gz'}] 
+            
         Example
         -------
-        >>> dataset = GoogleCloudDataset(bucket='ants-dev',
-                                         base_dir='datasets/nick_2/ds000711', 
-                                         x={'pattern': '*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
-                                         y={'file': 'participants.tsv', 'column': 'age'},
-                                         credentials='/Users/ni5875cu/Desktop/ants.dev/engine/deep-dynamics-415608-4046316ec2f1.json')
+        >>> dataset = PlatformDataset(name='ds000711', 
+                                      x={'pattern': '*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
+                                      y={'file': 'participants.tsv', 'column': 'age'})
+        >>> dataset = PlatformDataset(name='ds000711', 
+                                      x={'filenames': ['sub-001/anat/T1.nii.gz', '...']},
+                                      y={'file': 'participants.tsv', 'column': 'age'})
         """
+        # convert base_dir (nick-2/first-dataset) to gcs fuse
+        if fuse:
+            base_dir = os.path.join('/gcs/ants-dev/datasets/', base_dir)
+        else:
+            base_dir = os.path.join('datasets/', base_dir)
+            
         x_config = x
         y_config = y
         
-        if fuse:
-            base_dir = os.path.join('/gcs/', bucket, base_dir)
-            if not base_dir.endswith('/'): 
-                base_dir += '/'
-            
-            # GET X
-            x = glob.glob(x_config['pattern'], root_dir=base_dir)
-            if 'exclude' in x_config.keys():
-                x = [file for file in x if not fnmatch(file, x_config['exclude'])]
-            x_ids = [xx.split('/')[0] for xx in x]
-            x = [os.path.join('/gcs/', bucket, base_dir, file) for file in sorted(x)]
-            
-            if len(x) == 0:
-                raise Exception('Did not find any x values corresponding to the x config.')
-
-            # GET Y
-            y_file = os.path.join(base_dir, y_config['file'])
-            y_df = pd.read_csv(y_file, sep='\t')
-            
+        pattern = x_config['pattern']
+        glob_pattern = pattern.replace('{id}','*')
+        x = sorted(glob.glob(os.path.join(glob_pattern, base_dir)))
+        x = [os.path.relpath(xx, base_dir) for xx in x]
+        if 'exclude' in x_config.keys():
+            x = [file for file in x if not fnmatch(file, x_config['exclude'])]
+        
+        if '{id}' in pattern:
+            x_ids = [parse(pattern.replace('*','{other}'), file).named['id'] for file in x]
         else:
-            if isinstance(credentials, str):
-                credentials = service_account.Credentials.from_service_account_file(credentials)
-            if credentials is not None:
-                storage_client = storage.Client(credentials=credentials)
-            bucket_client = storage_client.bucket(bucket)
-        
-            # GET X
-            if not base_dir.endswith('/'): base_dir += '/'
-            x_blobs = storage_client.list_blobs(bucket, match_glob=f'{base_dir}{x_config["pattern"]}')
-            x = list([blob.name.replace(base_dir, '') for blob in x_blobs])
-            if 'exclude' in x_config.keys():
-                x = [file for file in x if not fnmatch(file, x_config['exclude'])]
             x_ids = [xx.split('/')[0] for xx in x]
-            x = [os.path.join(base_dir, file) for file in sorted(x)]
-            
-            if len(x) == 0:
-                raise Exception('Did not find any x values corresponding to the x config.')
-
-            # GET Y
-            y_file = os.path.join(base_dir, y_config['file'])
-            y_blob = bucket_client.blob(y_file)
-            tmp_file = tempfile.NamedTemporaryFile()
-            y_blob.download_to_filename(tmp_file.name)
-            y_df = pd.read_csv(tmp_file.name, sep='\t')
-            tmp_file.close()
-            
-            # properties specific to non-fuse scenarios
-            self.credentials = credentials
-            self.storage_client = storage_client
-            self.bucket_client = bucket_client
-            self.tmp_dir = tempfile.TemporaryDirectory()
-
+        x = [os.path.join(base_dir, file) for file in x]
+        
+        # GET Y
+        participants_file = os.path.join(base_dir, y_config['file'])
+        participants = pd.read_csv(participants_file, sep='\t')
+        
         # match x and y ids
-        p_col = y_df.columns[0] # assume participant id is first row
-        y_df = y_df.sort_values(p_col)
-        all_y_ids = y_df[p_col].to_numpy()
+        p_col = participants.columns[0] # assume participant id is first row
+        participants = participants.sort_values(p_col)
+        all_y_ids = participants[p_col].to_numpy()
         if len(x_ids) != len(all_y_ids):
             warnings.warn(f'Mismatch between x ids {len(x_ids)} and y ids {len(all_y_ids)} - finding intersection')
         y_ids = sorted(list(set(x_ids) & set(all_y_ids)))
-
-        y_df = y_df[y_df[p_col].isin(y_ids)]
-        y = y_df[y_config['column']].to_numpy()
-
+        
+        participants = participants[participants[p_col].isin(y_ids)]
+        y = participants[y_config['column']].to_numpy()
+        
         # remove x values that are not found in y
         x = [x[idx] for idx in range(len(x)) if x_ids[idx] in y_ids]
         x_ids = y_ids
+
+
+        if len(x) != len(y):
+            warnings.warn(f'len(x) [{len(x)}] != len(y) [{len(y)}]. Do some participants have multiple runs?')
         
-        self.bucket = bucket
         self.base_dir = base_dir
+        self.fuse = fuse
         self.x_config = x_config
         self.y_config = y_config
-        self.x = x
-        self.y = y
         self.x_transforms = x_transforms
         self.y_transforms = y_transforms
-        self.fuse = fuse
+        self.participants = participants
+        self.x = x
+        self.x_ids = x_ids
+        self.y = y
+        self.y_ids = y_ids
+        
+    def initialize(self):
+        pass
 
     def __getitem__(self, idx):
         files = self.x[idx]
         if not isinstance(idx, slice):
             files = [files]
         y = self.y[idx]
         
         if self.y_transforms is not None:
             y = np.array([self.y_transforms(yy) for yy in y])
         
         x = []
         for file in files:
             # if on vertex, file will be available to access. otherwise, download it to local tmp dir.
-            if self.fuse:
+            if True:
                 local_filepath = file
             else:
                 local_filepath = os.path.join(self.tmp_dir.name, file)
                 if not os.path.exists(local_filepath):
                     os.makedirs('/'.join(local_filepath.split('/')[:-1]), exist_ok=True)
                     file_blob = self.bucket_client.blob(file)
                     file_blob.download_to_filename(local_filepath)
@@ -153,17 +136,25 @@
 
         return x, y
     
     def __len__(self):
         return len(self.x)
     
     def __copy__(self):
-        return GoogleCloudDataset(
-            bucket = self.bucket,
-            base_dir = self.base_dir,
+        return PlatformDataset(
+            name = self.name,
             x = self.x_config,
             y = self.y_config,
             x_transforms = self.x_transforms,
             y_transforms = self.y_transforms,
             credentials = self.credentials
         )
     
+    def __repr__(self):
+        tx_repr = ', '.join([repr(x_tx) for x_tx in self.x_transforms])
+        return f'''PlatformDataset(name = "{self.name}",
+                    x = {self.x_config},
+                    y = {self.y_config},
+                    x_transforms = [{tx_repr}],
+                    y_transforms = {self.y_transforms},
+                    fuse = {self.fuse},
+                    credentials = None)'''
```

### Comparing `nitrain-0.2.1/nitrain/loaders/dataset_loader.py` & `nitrain-0.2.2/nitrain/loaders/dataset_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,101 +3,85 @@
 
 from .. import samplers
 
 class DatasetLoader:
     
     def __init__(self, 
                  dataset, 
-                 batch_size, 
+                 images_per_batch, 
                  x_transforms=None, 
                  y_transforms=None, 
                  co_transforms=None,
                  expand_dims=-1,
+                 shuffle=False,
                  sampler=None):
         """
         Arguments
         ---------
         
         Examples
         --------
         ds = Dataset()
         ld = DatasetLoader(ds)
         xb, yb = next(iter(ld))
 
         """
         self.dataset = dataset
-        self.batch_size = batch_size
+        self.images_per_batch = images_per_batch
         self.expand_dims = expand_dims
         self.x_transforms = x_transforms
         self.y_transforms = y_transforms
         self.co_transforms = co_transforms
+        self.shuffle = shuffle
+        
         if sampler is None:
-            sampler = samplers.BaseSampler()
+            sampler = samplers.BaseSampler(batch_size=images_per_batch)
         self.sampler = sampler
         
-    def as_keras_loader(self):
-        def my_func(batch_size, dataset, x_transforms, y_transforms, co_transforms,
-                    sampler, expand_dims):
-            n_batches = math.ceil(len(dataset) / batch_size)
-            
-            # TODO: apply shuffling to indices before we get to the batch loop
-            
-            batch_idx = 0
-            while True:
-                if batch_idx >= n_batches:
-                    batch_idx = 0
-                
-                data_indices = slice(batch_idx*batch_size, min((batch_idx+1)*batch_size, len(dataset)))
-                x, y = dataset[data_indices]
-                
-                batch_idx += 1
-                # perform transforms
-                if self.x_transforms:
-                    for tx_fn in x_transforms:
-                        x = [tx_fn(xx) for xx in x]
-                
-                if self.y_transforms:
-                    for tx_fn in y_transforms:
-                        y = [tx_fn(yy) for yy in y]
-                
-                if self.co_transforms:
-                    for tx_fn in co_transforms:
-                        for i in range(len(x)):
-                            x[i], y[i] = tx_fn(x[i], y[i])
-
-                # sample the batch
-                sampled_batch = sampler(x, y)
-                
-                # a normal sampler will just return the entire (shuffled, if specified) batch once
-                # a slice sampler will return shuffled slices with batch size = sampler.batch_size
-                for x_batch, y_batch in sampled_batch:
-                    if self.expand_dims is not None:
-                        x_batch = np.array([np.expand_dims(xx.numpy(), expand_dims) for xx in x_batch])
-                    else:
-                        x_batch = np.array([xx.numpy() for xx in x_batch])
-                    
-                    yield x_batch, y_batch
-
-        return my_func(self.batch_size, self.dataset, self.x_transforms, self.y_transforms, self.co_transforms,
-                    self.sampler, self.expand_dims)
+    def to_keras(self, output_signature=None):
+        import tensorflow as tf
+        
+        def batch_generator():
+            my_iter = iter(self)
+            for x_batch, y_batch in my_iter:
+                for i in range(x_batch.shape[0]):
+                    yield x_batch[i,:], y_batch[i]
+ 
+        # generate a training batch to infer the output signature
+        if output_signature is None:
+            tmp_batch_size = self.images_per_batch
+            self.images_per_batch = 1
+            x_batch, y_batch = next(iter(self))
+            self.images_per_batch = tmp_batch_size
+            x_spec = tf.type_spec_from_value(x_batch[0,:])
+            y_spec = tf.type_spec_from_value(y_batch[0])
+        
+        generator = tf.data.Dataset.from_generator(
+            lambda: batch_generator(),
+            output_signature=(x_spec, y_spec)
+        ).batch(self.sampler.batch_size)
+        
+        return generator
                 
     def __iter__(self):
-        batch_size = self.batch_size
+        images_per_batch = self.images_per_batch
         dataset = self.dataset
-        n_batches = math.ceil(len(dataset) / batch_size)
+        n_image_batches = math.ceil(len(dataset) / images_per_batch)
         
-        # TODO: apply shuffling to indices before we get to the batch loop
+        original_indices = np.arange(len(dataset))
+        if self.shuffle:
+            np.random.shuffle(original_indices)
         
-        batch_idx = 0
-        while batch_idx < n_batches:
-            
-            batch_idx += 1
+        image_batch_idx = 0
+        while image_batch_idx < n_image_batches:
             
-            data_indices = slice(batch_idx*batch_size, min((batch_idx+1)*batch_size, len(dataset)))
+            data_indices = slice(image_batch_idx*images_per_batch, min((image_batch_idx+1)*images_per_batch, len(dataset)))
             x, y = dataset[data_indices]
+            
+            image_batch_idx += 1
            
             # perform transforms
             if self.x_transforms:
                 for tx_fn in self.x_transforms:
                     x = [tx_fn(xx) for xx in x]
             
             if self.y_transforms:
@@ -109,23 +93,40 @@
                     for i in range(len(x)):
                         x[i], y[i] = tx_fn(x[i], y[i])
 
             # sample the batch
             sampled_batch = self.sampler(x, y)
             
             # a normal sampler will just return the entire (shuffled, if specified) batch once
-            # a slice sampler will return shuffled slices with batch size = sampler.batch_size
+            # a slice sampler will return shuffled slices with batch size = sampler.images_per_batch
             for x_batch, y_batch in sampled_batch:
                 
                 if self.expand_dims is not None:
-                    x_batch = np.array([np.expand_dims(xx.numpy(), self.expand_dims) for xx in x_batch])
+                    if isinstance(x_batch[0], list):
+                        print('got multiple inputs')
+                        x_batch_return = []
+                        for i in range(len(x_batch[0])):
+                            tmp_x_batch = np.array([np.expand_dims(xx[i].numpy(), self.expand_dims) for xx in x_batch])
+                            x_batch_return.append(tmp_x_batch)
+                        x_batch = x_batch_return
+                    else:
+                        x_batch = np.array([np.expand_dims(xx.numpy(), self.expand_dims) for xx in x_batch])
+                    if 'ANTsImage' in str(type(y[0])):
+                        y_batch = np.array([np.expand_dims(yy.numpy(), self.expand_dims) for yy in y_batch])
                 else:
                     x_batch = np.array([xx.numpy() for xx in x_batch])
+                    if 'ANTsImage' in str(type(y[0])):
+                        y_batch = np.array([yy.numpy() for yy in y_batch])
                 
                 yield x_batch, y_batch
                 
-            
-
     def __len__(self):
-        return math.ceil((len(self.dataset) / self.batch_size) * len(self.sampler))
+        return math.ceil((len(self.dataset) / self.images_per_batch) * len(self.sampler))
+    
+    def __repr__(self):
+        x_tx_repr = ', '.join([repr(x_tx) for x_tx in self.x_transforms])
+        return f'''DatasetLoader(dataset,
+                   images_per_batch={self.images_per_batch},
+                   sampler={repr(self.sampler)},
+                   x_transforms=[{x_tx_repr}])'''
```

### Comparing `nitrain-0.2.1/nitrain/models/fetch_architecture.py` & `nitrain-0.2.2/nitrain/models/fetch_architecture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 
 from inspect import getmembers, isfunction
 
-import antspynet
-
-import tensorflow as tf
-import tensorflow.keras.backend as K
-
-
 def fetch_architecture(name, dim=None):
     """
     Fetch an architecture function based on its name and input image 
     dimensions (2, 3, or None).
     
     Arguments
     ---------
@@ -28,14 +22,16 @@
     -------
     >>> from nitrain import models
     >>> vgg_fn = models.fetch_architecture('vgg', dim=3)
     >>> vgg_model = vgg_fn((128, 128, 128, 1))
     >>> autoencoder_fn = models.fetch_architecture('autoencoder')
     >>> autoencoder_model = autoencoder_fn((784, 500, 500, 2000, 10))
     """
+    import antspynet
+    
     try:
         if dim is not None:
             fstr = f'create_{name}_model_{dim}d'
             fn = getattr(antspynet.architectures, fstr)
         else:
             fstr = f'create_{name}_model'
             fn = getattr(antspynet.architectures, fstr)
@@ -60,14 +56,15 @@
     function via 'create_{alexnet}_model_{2d}'
     
     Example
     -------
     >>> from nitrain import models
     >>> models.list_architectures()    
     """
+    import antspynet
     archs = [f[0].split('create_')[1].split('_model_') for f in getmembers(antspynet.architectures, isfunction) if f[0].startswith('create_')]
     # add empty string for non-dimensioned models just to be consistent
     def add_empty(x):
         if len(x) == 1:
             x.append('')
         return x
     archs = [add_empty(arch) for arch in archs]
```

### Comparing `nitrain-0.2.1/nitrain/samplers/base_sampler.py` & `nitrain-0.2.2/nitrain/samplers/base_sampler.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     """
     Standard sampler that just returns the batch with or without shuffling
     
     Examples
     --------
     
     """
-    def __init__(self, shuffle=False):
+    def __init__(self, batch_size, shuffle=False):
+        self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         self.x = x
         self.y = y
         return self
 
@@ -30,15 +31,18 @@
             self.idx += 1
             x = self.x
             y = self.y
                 
             if self.shuffle:
                 indices = random.sample(range(len(y)), len(y))
                 x = [x[i] for i in indices]
-                y = y[indices]
+                if 'ANTsImage' in str(type(y[0])):
+                    y = [y[i] for i in indices]
+                else:
+                    y = y[indices]
             
             return x, y
         else:
             raise StopIteration
     
     def __len__(self):
         """
```

### Comparing `nitrain-0.2.1/nitrain/samplers/block_sampler.py` & `nitrain-0.2.2/nitrain/samplers/block_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import math
 
 
 class BlockSampler:
     """
     Sampler that returns 3D blocks from 3D images.
     """
-    def __init__(self, block_size, stride, sub_batch_size, shuffle=False):
+    def __init__(self, block_size, stride, batch_size, shuffle=False):
         
         if isinstance(block_size, int):
-            block_size = [block_size, block_size]
+            block_size = [block_size, block_size, block_size]
         
         if isinstance(stride, int):
-            stride = [stride, stride]
+            stride = [stride, stride, stride]
             
         self.block_size = block_size
         self.stride = stride
-        self.sub_batch_size = sub_batch_size
+        self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         # create patches of all images
         self.x, self.y = create_patches(x, y, self.block_size, self.stride)
-        self.n_batches = math.ceil(len(self.x) / self.sub_batch_size)
+        self.n_batches = math.ceil(len(self.x) / self.batch_size)
                 
         return self
 
     def __iter__(self):
         """
         Apply shuffling whenever the sampler is instantiated
         as an iterator.
@@ -40,29 +40,29 @@
             self.x = [self.x[i] for i in indices]
             self.y = self.y[indices]
             
         return self
 
     def __next__(self):
         if self.idx < self.n_batches:
-            data_indices = slice(self.idx*self.sub_batch_size, min((self.idx+1)*self.sub_batch_size, len(self.x)))
+            data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
     
     def __len__(self):
         """
         number of batches from the sampler
         """
         if not self.x:
             return 0
-        return math.ceil(len(self.x) / self.sub_batch_size)
+        return math.ceil(len(self.x) / self.batch_size)
 
 
 def create_patches(images, values, block_size, stride):
     cropped_images = []
     new_values = []
     for image, value in zip(images, values):
         # extract all blocks
```

### Comparing `nitrain-0.2.1/nitrain/samplers/patch_sampler.py` & `nitrain-0.2.2/nitrain/samplers/patch_sampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import math
 
 
 class PatchSampler:
     """
     Sampler that returns 2D patches from 2D images.
     """
-    def __init__(self, patch_size, stride, sub_batch_size, shuffle=False):
+    def __init__(self, patch_size, stride, batch_size, shuffle=False):
         
         if isinstance(patch_size, int):
             patch_size = [patch_size, patch_size]
         
         if isinstance(stride, int):
             stride = [stride, stride]
             
         self.patch_size = patch_size
         self.stride = stride
-        self.sub_batch_size = sub_batch_size
+        self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         # create patches of all images
         self.x, self.y = create_patches(x, y, self.patch_size, self.stride)
-        self.n_batches = math.ceil(len(self.x) / self.sub_batch_size)
+        self.n_batches = math.ceil(len(self.x) / self.batch_size)
                 
         return self
 
     def __iter__(self):
         """
         Apply shuffling whenever the sampler is instantiated
         as an iterator.
@@ -41,29 +41,29 @@
             self.x = [x[i] for i in indices]
             self.y = self.y[indices]
             
         return self
 
     def __next__(self):
         if self.idx < self.n_batches:
-            data_indices = slice(self.idx*self.sub_batch_size, min((self.idx+1)*self.sub_batch_size, len(self.x)))
+            data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
     
     def __len__(self):
         """
         number of batches from the sampler
         """
         if not self.x:
             return 0
-        return math.ceil(len(self.x) / self.sub_batch_size)
+        return math.ceil(len(self.x) / self.batch_size)
 
 
 def create_patches(images, values, patch_size, stride):
     cropped_images = []
     new_values = []
     for image, value in zip(images, values):
         # extract all patches
```

### Comparing `nitrain-0.2.1/nitrain/samplers/slice_patch_sampler.py` & `nitrain-0.2.2/nitrain/samplers/slice_patch_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 from .patch_sampler import create_patches
 from .slice_sampler import create_slices
 
 class SlicePatchSampler:
     """
     Sampler that returns 2D patches from 3D images.
     """
-    def __init__(self, patch_size, stride, axis, sub_batch_size, shuffle=False):
+    def __init__(self, patch_size, stride, axis, batch_size, shuffle=False):
         
         if isinstance(patch_size, int):
             patch_size = [patch_size, patch_size]
         
         if isinstance(stride, int):
             stride = [stride, stride]
             
         self.patch_size = patch_size
         self.stride = stride
         self.axis = axis
-        self.sub_batch_size = sub_batch_size
+        self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         # create slices of all images
         x, y = create_slices(x, y, self.axis)
         # then create patches from all those slices
         x, y = create_patches(x, y, self.patch_size, self.stride)
         
         self.x = x
         self.y = y
-        self.n_batches = math.ceil(len(x) / self.sub_batch_size)
+        self.n_batches = math.ceil(len(x) / self.batch_size)
                 
         return self
 
     def __iter__(self):
         """
         Apply shuffling whenever the sampler is instantiated
         as an iterator.
@@ -49,22 +49,22 @@
             self.x = [x[i] for i in indices]
             self.y = self.y[indices]
             
         return self
 
     def __next__(self):
         if self.idx < self.n_batches:
-            data_indices = slice(self.idx*self.sub_batch_size, min((self.idx+1)*self.sub_batch_size, len(self.x)))
+            data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
     
     def __len__(self):
         """
         number of batches from the sampler
         """
         if not self.x:
             return 0
-        return math.ceil(len(self.x) / self.sub_batch_size)
+        return math.ceil(len(self.x) / self.batch_size)
```

### Comparing `nitrain-0.2.1/nitrain/samplers/slice_sampler.py` & `nitrain-0.2.2/nitrain/samplers/slice_sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,46 @@
 import math
 
     
 class SliceSampler:
     """
     Sampler that returns batches of 2D slices from 3D images.
     """
-    def __init__(self, sub_batch_size, axis=0, shuffle=False):
-        self.sub_batch_size = sub_batch_size
+    def __init__(self, batch_size, axis=0, shuffle=False):
+        self.batch_size = batch_size
         self.axis = axis
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         # create slices of all images
         self.x, self.y = create_slices(x, y, self.axis)
-        self.n_batches = math.ceil(len(self.x) / self.sub_batch_size)
+        self.n_batches = math.ceil(len(self.x) / self.batch_size)
                 
         return self
 
     def __iter__(self):
         """
         Get a sampled batch
         """
         self.idx = 0
         
         # apply shuffling
         if self.shuffle:
             indices = random.sample(range(len(self.y)), len(self.y))
             self.x = [self.x[i] for i in indices]
-            self.y = self.y[indices]
+            if 'ANTsImage' in str(type(self.y[0])):
+                self.y = [self.y[i] for i in indices]
+            else:
+                self.y = self.y[indices]
             
         return self
 
     def __next__(self):
         if self.idx < self.n_batches:
-            data_indices = slice(self.idx*self.sub_batch_size, min((self.idx+1)*self.sub_batch_size, len(self.x)))
+            data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
     
@@ -47,18 +50,33 @@
         """
         number of batches from the sampler
         """
         if self.n_batches is not None:
             return self.n_batches
         else:
             return 0
+    
+    def __repr__(self):
+        return f'''samplers.SliceSampler(axis={self.axis}, batch_size={self.batch_size}, shuffle={self.shuffle})'''
+
 
 
 def create_slices(images, values, axis):
-    slices = []
-    new_values = []
-    for image, value in zip(images, values):
-        for i in range(image.shape[axis]):
-            slices.append(image.slice_image(axis, i))
-            new_values.append(value)
-            
-    return slices, np.array(new_values)
+    
+    if 'ANTsImage' in str(type(values[0])):
+        slices = []
+        co_slices = []
+        for image, co_image in zip(images, values):
+            for i in range(image.shape[axis]):
+                slices.append(image.slice_image(axis, i, 1))
+                co_slices.append(co_image.slice_image(axis, i, 1))
+                
+        return slices, co_slices
+    else:
+        slices = []
+        new_values = []
+        for image, value in zip(images, values):
+            for i in range(image.shape[axis]):
+                slices.append(image.slice_image(axis, i, 1))
+                new_values.append(value)
+                
+        return slices, np.array(new_values)
```

### Comparing `nitrain-0.2.1/nitrain/transforms/ants_transforms.py` & `nitrain-0.2.2/nitrain/transforms/ants_transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # Transforms that apply specific antspy functions to images
 import ants
-import antspynet
+
 
 import random
 import numpy as np
 
 from .base_transform import BaseTransform
 
 
 class ApplyAntsTransform(BaseTransform):
     """
     Apply an ANTs transform to an image
     """
-    def __init__(self, transform):
+    def __init__(self, transform, reference=None):
         self.transform = transform
+        self.reference = reference
         
     def __call__(self, image):
-        new_image = ants.apply_ants_transform_to_image(self.transform, image)
+        reference = self.reference
+        if reference is None:
+            reference = image
+            
+        new_image = ants.apply_ants_transform_to_image(self.transform, image, reference)
         return new_image
 
 
 class BrainExtraction(BaseTransform):
     """
     Extract brain from image 
     """
@@ -28,14 +33,18 @@
     def __init__(self):
         pass
     
     def __call__(self, image):
         new_image = ants.get_mask(image)
         return new_image * image
 
+    def __repr__(self):
+        return f'tx.BrainExtraction()'
+
+
 
 class DisplacementField(BaseTransform):
     """
     Simulate and apply a random displacement field
     
     Examples
     --------
@@ -97,14 +106,15 @@
         self.n_points = n_points
         self.n_levels = n_levels
         self.mesh_size = mesh_size
         self.field_power = field_power
         self.normalize = normalize
     
     def __call__(self, image):
+        import antspynet
         log_field = antspynet.simulate_bias_field(image, 
                                                   number_of_points=self.n_points, 
                                                   sd_bias_field=self.sd, 
                                                   number_of_fitting_levels=self.n_levels, 
                                                   mesh_size=self.mesh_size)
         log_field = log_field.iMath("Normalize")
         field_array = np.power(np.exp(log_field.numpy()), self.field_power)
@@ -124,14 +134,18 @@
     def __init__(self, template):
         self.template = template
 
     def __call__(self, image):
         center_of_mass_template = ants.get_center_of_mass(self.template)
         center_of_mass_image = ants.get_center_of_mass(image)
         translation = tuple(np.array(center_of_mass_image) - np.array(center_of_mass_template))
-        xfrm = ants.create_ants_transform(transform_type="Euler3DTransform", 
+        if image.dimension == 2:
+            transform_type = 'Euler2DTransform'
+        elif image.dimension == 3:
+            transform_type = 'Euler3DTransform'
+        xfrm = ants.create_ants_transform(transform_type=transform_type, 
                                           center = center_of_mass_template,
                                           translation=translation,precision='float',
                                           dimension=image.dimension)
 
         new_image = ants.apply_ants_transform_to_image(xfrm, image, self.template)
         return new_image
```

### Comparing `nitrain-0.2.1/nitrain/transforms/intensity_transforms.py` & `nitrain-0.2.2/nitrain/transforms/intensity_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ants
-import antspynet
 
 import random
 import numpy as np
 
 from .base_transform import BaseTransform
 
 
@@ -82,15 +81,15 @@
         self.physical_space = physical_space
         
     def __call__(self, *images):
         new_images = []
         for image in images:
             new_image = ants.smooth_image(image, 
                                           self.std,
-                                          physical_space=self.physical_space)
+                                          self.physical_space)
             new_images.append(new_image)
         return new_images if len(new_images) > 1 else new_images[0]
 
 
 class RandomSmoothing(BaseTransform):
 
     def __init__(self, min_std, max_std, physical_space=True):
@@ -104,15 +103,17 @@
         new_images = []
         for image in images:
             new_image = ants.smooth_image(image, 
                                           std,
                                           self.physical_space)
             new_images.append(new_image)
         return new_images if len(new_images) > 1 else new_images[0]
-        
+
+    def __repr__(self):
+        return f'''tx.RandomSmoothing({self.min_std}, {self.max_std}, {self.physical_space})'''
 
 class RandomNoise(BaseTransform):
     """
     Apply random additive gaussian noise to an image.
     
     import ants
     img = ants.image_read(ants.get_ants_data('r16'))
@@ -128,14 +129,17 @@
         new_images = []
         for image in images:
             new_image = ants.add_noise_to_image(image,
                                                 'additivegaussian',
                                                 (0, std))
             new_images.append(new_image)
         return new_images if len(new_images) > 1 else new_images[0]
+    
+    def __repr__(self):
+        return f'''tx.RandomNoise({self.min_std}, {self.max_std})'''
 
 
 class HistogramWarpIntensity(BaseTransform):
     """
     See https://github.com/ANTsX/ANTsPyNet/blob/master/antspynet/utilities/histogram_warp_image_intensities.py
     """
     def __init__(self, 
@@ -147,14 +151,16 @@
         self.break_points = break_points
         self.displacements = displacements
         self.clamp_end_points = clamp_end_points
         self.sd_displacements = sd_displacements
         self.transform_domain_size = transform_domain_size
 
     def __call__(self, *images):
+        import antspynet
+        
         new_images = []
         for image in images:
             new_image = antspynet.histogram_warp_image_intensities(
                 image = image,
                 break_points = self.break_points,
                 displacements = self.displacements,
                 clamp_end_points = self.clamp_end_points,
```

### Comparing `nitrain-0.2.1/nitrain/transforms/structural_transforms.py` & `nitrain-0.2.2/nitrain/transforms/structural_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,29 @@
     # resample with spacing so you dont have to figure out uneven dimensions
     my_tx2 = ResampleImage((4,4,4), use_spacing=True)
     img3 = my_tx2(img)
     """
     def __init__(self, params, use_spacing=False, interpolation='linear'):
         self.params = params
         self.use_spacing = use_spacing
-        self.interpolation = 0 if interpolation != 'nearest_neighbor' else 1 
+        self.interpolation = interpolation
+        
     
-    def __call__(self, image):
-        image = ants.resample_image(image, self.params, not self.use_spacing, self.interpolation)
+    def __call__(self, image, co_image=None):
+        interpolation_value = 0 if self.interpolation != 'nearest_neighbor' else 1 
+        image = ants.resample_image(image, self.params, not self.use_spacing, interpolation_value)
+        
+        if co_image is not None:
+            co_image = ants.resample_image(co_image, self.params, not self.use_spacing, interpolation_value)
+            return image, co_image
+        
         return image
 
+    def __repr__(self):
+        return f'tx.Resample({self.params}, {self.use_spacing}, "{self.interpolation}")'
 
 class ResampleToTarget(BaseTransform):
     """
     img = ants.image_read(ants.get_ants_data('mni'))
     img2 = img.clone().resample_image((4,4,4))
     my_tx = ResampleImageToTarget(img2)
     img3 = my_tx(img)
@@ -52,31 +61,36 @@
     An image orientation consists of three letters - one from each
     of the three axes - with the letter for each axes determining
     where the indexing starts. Orientation is important for slicing.
     """
     def __init__(self, orientation='RAS'):
         self.orientation = orientation
     
-    def __call__(self, image):
+    def __call__(self, image, co_image=None):
         image = ants.reorient_image2(image, self.orientation)
         
+        if co_image is not None:
+            co_image = ants.reorient_image2(co_image, self.orientation)
+            return image, co_image
+
+        return image
 
 class Slice(BaseTransform):
     """
     Slice a 3D image into 2D. 
     """
     def __init__(self, axis, idx):
         self.axis = axis
         self.idx = idx
     
     def __call__(self, image):
         if self.idx is None:
-            new_image = [image.slice_image(self.axis, idx) for idx in range(image.shape[self.axis])]
+            new_image = [image.slice_image(self.axis, idx, 1) for idx in range(image.shape[self.axis])]
         else:
-            new_image = image.slice_image(self.axis, self.idx)
+            new_image = image.slice_image(self.axis, self.idx, 1)
         return new_image
 
 
 class RandomSlice(BaseTransform):
     """
     Randomly slice a 3D image into 2D. 
     
@@ -85,15 +99,15 @@
         self.axis = axis
         self.allow_blank = allow_blank
     
     def __call__(self, image):
         if not self.allow_blank:
             image = image.crop_image()
         
-        idx = random.sample(range(image.shape[self.axis]))[0]
+        idx = random.sample(range(image.shape[self.axis]), 1)[0]
         new_image = image.slice_image(self.axis, idx)
         
         return new_image
 
 
 class Crop(BaseTransform):
     """
```

### Comparing `nitrain-0.2.1/nitrain/transforms/utility_transforms.py` & `nitrain-0.2.2/nitrain/transforms/utility_transforms.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.2.1/pyproject.toml` & `nitrain-0.2.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nitrain"
-version = "0.2.1"
-description = "Neuroimaging-native tools for deep learning"
+version = "0.2.2"
+description = "High-level framework for training medical imaging AI models"
 authors = ["ncullen93 <nicholas.cullen@med.lu.se>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nibabel = "^5.2.0"
```

### Comparing `nitrain-0.2.1/PKG-INFO` & `nitrain-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nitrain
-Version: 0.2.1
-Summary: Neuroimaging-native tools for deep learning
+Version: 0.2.2
+Summary: High-level framework for training medical imaging AI models
 License: MIT
 Author: ncullen93
 Author-email: nicholas.cullen@med.lu.se
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -29,76 +29,86 @@
 Requires-Dist: tensorflow-probability (==0.20)
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Nitrain - a framework for medical imaging-native AI
 
 [![Coverage Status](https://coveralls.io/repos/github/ncullen93/nitrain/badge.svg?branch=main)](https://coveralls.io/github/ncullen93/nitrain?branch=main)
+[![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
-Nitrain is a medical imaging-native framework for training and visualizing deep learning models. It provides tools for sampling and augmenting neuroimaging datasets, training deep learning models on neuroimages, and visualizing or explaining deep learning model results in a neuroimaging context. Nitrain also makes it easy to use pre-trained models for training or integration into imaging pipelines.
+Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
+
+You can also train models HIPAA-compliantly in the cloud using nitrain. You are encouraged to make your fitted models available to the community via nitrain, or you can easily use other's pretrained models for fine-tuning or standard image processing.
 
 <br />
 
 ## Installation
 
-The package can be installed from github:
+The latest release of nitrain can be installed from pypi:
+
+```
+pip install nitrain
+```
+
+Or you can install the latest development version directly from github:
 
 ```
 python -m pip install git+github.com/ncullen93/nitrain.git
 ```
 
 ### Dependencies
 
-The nitrain package is developed with Python3.10 as the focus. In terms of dependencies, it requires `ants` and `antspynet` and works with either tensorflow/keras or pytorch. Support for Keras 3 is on the roadmap.
+The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
 
 <br />
 
 ## Quickstart
 
-Here is a canonical example of using nitrain to give you a quick overview. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
-
-Alternatively, you can check out the [tutorials](github.com/ncullen93/nitrain) for an in-depth introduction to everything that nitrain has to offer or the [examples](github.com/ncullen93/nitrain) for self-contained, end-to-end examples of how to perform common deep learning tasks.
+Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
 
 ```python
 from nitrain import datasets, loaders, models, trainers, transforms as tx
 
-#### Brain-age example ####
-
 # create dataset from folder of images + participants file
 dataset = datasets.FolderDataset(base_dir='ds004711',
-                            x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
-                            y={'file': 'participants.tsv',
-                                    'column': 'age'},
-                            x_transforms=[nit.ResizeImage((64,64,64)),
-                                          nit.NormalizeIntensity(0,1)])
+                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz'},
+                                 y={'file': 'participants.tsv',
+                                         'column': 'age'},
+                                 x_transforms=[tx.Resize((64,64,64)),
+                                               tx.NormalizeIntensity(0,1)])
 
 # create loader with random transforms
 loader = loaders.DatasetLoader(dataset,
-                           batch_size=32,
-                           shuffle=True,
-                           x_transforms=[nit.RandomSlice(axis=2),
-                                         nit.RandomNoise(sd=0.2)])
+                               images_per_batch=4,
+                               shuffle=True,
+                               sampler=samplers.SliceSampler(batch_size=32, axis=2)
+                               x_transforms=[tx.RandomNoise(sd=0.2)])
 
 # create model from architecture
-architecture_fn = models.fetch_architecture('alexnet', task='continuous_prediction')
-model = architecture_fn(layers=[128, 64, 32, 10], n_outcomes=1)
+arch_fn = models.fetch_architecture('alexnet', dim=2)
+model = arch_fn(input_image_size=(64,64,1),
+                number_of_outcomes=1,
+                mode='regression')
 
 # create trainer and fit model
 trainer = trainers.ModelTrainer(model,
-                           loss='mse',
-                           optimizer='adam',
-                           lr=1e-3,
-                           callbacks=[nit.EarlyStopping(),
-                                      nit.ModelCheckpoints(freq=25)])
+                                loss='mse',
+                                optimizer='adam',
+                                lr=1e-3,
+                                callbacks=[utils.EarlyStopping(),
+                                           utils.ModelCheckpoints(freq=25)])
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-models.register_model(trainer.model, 'nick/t1-brainage-model')
+models.register_model(trainer.model, 'nick/t1-brain-age')
 ```
 
+A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
+
 <br />
 
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
 - [Datasets and Loaders](#datasets-and-loaders)
@@ -106,90 +116,89 @@
 - [Transforms](#transforms)
 - [Architectures and pretrained models](#architectures-and-pretrained-models)
 - [Model trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
-## Datasets and Loaders
-
-Nitrain provides extensive functionality to help you sample neuroimages with imaging-native data augmentation techniques. Our focus is on speed, meaning you never have to convert your neuroimages into numpy arrays.
+### Datasets and Loaders
 
-You start by creating a `dataset` from wherever your images are stored -- in a local folder, in a bids folder, in memory, on a cloud service, etc. Say that your data is stored in a local folder. To grab inputs (`x`), supply a dictionary with a glob pattern and optional exclude pattern. To grab outputs (`y`), specify a dataframe file to read and a column to pull from that dataframe. Both x and y can be image configs, and they can also be lists of configs if you want to grab multiple images at once.
+Datasets help you read in your images from wherever they are stored -- in a local folder with BIDS or datalad, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, BIDS entities, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
-from nitrain import datasets
-dataset = datasets.FolderDataset(base_dir='ds004711',
+from nitrain import datasets, transforms as tx
+
+dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
                                  x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
-                                 x_transforms=[tx.Resample((4,4,4), use_spacing=True),
-                                               tx.RangeNormalize(0,1)])
-
+                                 x_transforms=[tx.Resample((64,64,64))])
 ```
 
-Notice also that there the `x_transforms` argument has been supplied. These transforms are applied every time the input image is read into file. These are meant to be "fixed" transforms - i.e., not random - because the results can be cached to speed up sampling in the long-run.
-
-Once you have a dataset, you can grab images from it as you would with any iterator. This gives you the first input image (with transforms applied) and the first age value.
+Although you will rarely need to do this, data can be read into memory by indexing the dataset:
 
 ```python
-x, y = dataset[0]
+x_raw, y_raw = dataset[:3]
 ```
 
-The dataset can then be passed into a `loader` in order to actually sample batches. With loaders, you can specify parameters like batch size and whether to expand dims. You can also pass in more transforms that will be applied at each batch sampling. These transforms, in contrast, are meant to be random data augmentation transforms.
+To prepare your images for batch generation during training, you pass the dataset into one the loaders. Here is where you can also pass in random transforms that will act as data augmentation. If you want to train on slices, patches, or blocks of images then you will additionally provide a sampler. The different samplers are explained later.
 
 ```python
+from nitrain import loaders, samplers
+
 loader = loaders.DatasetLoader(dataset,
-                               batch_size=32,
-                               x_transforms=[tx.RandomSmoothing(0, 1)],
-                               expand_dims=-1)
+                               images_per_batch=32,
+                               x_transforms=[tx.RandomSmoothing(0, 1)])
 
 # loop through all images in batches for one epoch
 for x_batch, y_batch in loader:
         print(y_batch)
 ```
 
-The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework. Note that we also have loaders geared specifically towards those frameworks to allow you to use some additional loading functionality that they provide.
+The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework.
 
 <br />
 
-## Samplers
+### Samplers
 
 Samplers allow you to keep the same dataset + loader workflow that batches entire images and applies transforms to them, but then expand on those transformed image batches to create special "sub-batches".
 
 For instance, samplers let you serve batches of 2D slices from 3D images, or 3D blocks from 3D images, and so forth. Samplers are essntial for common deep learning workflows in medical imaging where you often want to train a model on only parts of the image at once.
 
-All you have to do is supply a sampler instance to your dataset loader. Here is an example:
-
 ```python
-from nitrain import loaders, samplers as sp, transforms as tx
+from nitrain import loaders, samplers, transforms as tx
 loader = loaders.DatasetLoader(dataset,
-                               batch_size=3,
+                               images_per_batch=4,
                                x_transforms=[tx.RandomSmoothing(0, 1)],
-                               expand_dims=-1,
-                               sampler=sp.SliceSampler(sub_batch_size=24, axis=0, shuffle=True))
+                               sampler=samplers.SliceSampler(batch_size=24, axis=2))
 ```
 
-What happens is that we start with the ~190 images from the dataset, but 3 images will be read in from file at a time. Then, all possible 2D slices will be created from those 3 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 3 images) have been served, the loader will move on to the next 3 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
-
-The important thing to remember is that the batch size your model will see is 24. In total, then, there are (n_images \* n_slices_per_image / sampler_batch_size) total batches in one epoch instead of (n_images / loader_batch_size) like there normally are.
+What happens is that we start with the ~190 images from the dataset, but 4 images will be read in from file at a time. Then, all possible 2D slices will be created from those 4 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 4 images) have been served, the loader will move on to the next 4 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
 
 <br />
 
-## Transforms
+### Transforms
 
-The philosophy of nitrain is to be as neuroimaging-native as possible. That means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to numpy arrays.
+The philosophy of nitrain is to be medical imaging-native. This means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to arrays / tensors for model consumption.
 
-The nitrain package supports an extensive amount of neuroimaging-based transforms:
+The nitrain package supports an extensive amount of medical imaging transforms:
 
 - Affine (Rotate, Translate, Shear, Zoom)
 - Flip, Pad, Crop, Slice
 - Noise
 - Motion
 - Intensity normalization
 
+You can create your own transform with the `CustomTransform` class:
+
+```python
+from nitrain import transforms as tx
+
+my_tx = tx.CustomTransform(lambda x: x * 2)
+```
+
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
 import ants
 import numpy as np
 from nitrain import transforms as tx
 
@@ -197,33 +206,17 @@
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
 ants.plot_grid(np.array(imgs).reshape(4,3))
 ```
 
-Writing your own transform is extremely easy! Just remember that the transform will operate on the `antsImage` type and that you should inherit from the `BaseTransform` class.
-
-```python
-from nitrain.transforms import BaseTransform
-
-class CoolTransform(BaseTransform):
-        def __init__(self, parameters):
-                self.parameters = parameters
-        def __call__(self, image):
-                image = my_function(image, self.parameters)
-                return image
-
-tx_fn = CoolTransform(parameters=123)
-img_transformed = tx_fn(img)
-```
-
 <br />
 
-## Architectures and pretrained models
+### Architectures and pretrained models
 
 The nitrain package provides an interface to an extensive amount of deep learning model architectures for all kinds of tasks - regression, classification, image-to-image generation, segmentation, autoencoders, etc.
 
 The available architectures can be listed and explored:
 
 ```python
 from nitrain import models
@@ -238,67 +231,48 @@
 vgg_fn = models.fetch_architecture('vgg', dim=3)
 vgg_model = vgg_fn((128, 128, 128, 1))
 
 autoencoder_fn = models.fetch_architecture('autoencoder')
 autoencoder_model = autoencoder_fn((784, 500, 500, 2000, 10))
 ```
 
-There is also a large collection of pretrained models available as a starting point for your training or simply to use for inference. If your dataset is small (<500 participants) than you may especially benefit from using pre-trained models.
-
-Similarly to architectures, you fetch a pretrained model based on its name. The result of fetching a pretrained model is the actual instantianed model with the pretrained weights loaded.
-
-```python
-from nitrain import models
-model = models.fetch_pretrained('basic-t1')
-```
-
-If you have trained an interested deep learning model on neuroimages and would like to share it with the community, it is possible to do so directly from nitrain. Any model you share will be hosted and available for use by anyone else through the `fetch_pretrained` function.
-
-```python
-from nitrain import models
-models.register_pretrained(model, 'my-cool-model')
-```
-
 <br />
 
-## Model trainers
+### Trainers
 
-After you have either fetched and created an architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
+After you have created a model from a nitrain architecture, fetched a pretrained model, or created a model yourself in your framework of choice, then it's time to actually train the model on the dataset / loader that you've created.
 
-To train with Pytorch, use the `nitrain.torch` module:
+Although you are free to train models on loaders using standard pytorch, keras, or tensorflow workflows, we also provide the `ModelTrainer` class to make training even easier. This class provides sensible defaults for key training parameters based on your task.
 
 ```python
-import nitrain
-```
-
-To train with Keras, use the `nitrain.keras` module:
+trainer = trainers.ModelTrainer(model=vgg_model, task='regression')
+trainer.fit(loader, epochs=10)
 
-```python
-import nitrain
+# access fitted model
+print(trainer.model)
 ```
 
-To train with Tensorflow, use the `nitrain.tensorflow` module:
+If you have signed up for an account at [nitrain.dev](https://www.nitrain.dev) then you can also train your model in the cloud using the `PlatformTrainer` class. All training takes place on HIPAA-compliant GPU servers with competitive pricing.
 
 ```python
-import nitrain
+trainer = trainers.PlatformTrainer(model=model, task='regression',
+                                name='brain-age', resource='gpu-small')
+trainer.fit(loader, epochs=10)
+
+# check job status
+print(trainer.status)
 ```
 
 <br />
 
-## Explainers
+### Explainers
 
 The idea that deep learning models are "black boxes" is out-dated, particularly when it comes to images. There are numerous techiques to help you understand which parts of the brain a trained model is weighing most when making predictions.
 
-One such technique is called the occlusion method, where you systematically "black out" different patches of an input image and see how the model prediction is affected. The idea is that when, when occluded, important areas result in a large change in model prediction compared to the original image.
-
 Nitrain provides tools to perform this techique - along with many others - and can help you visualize the results of such explainability experiments directly in brain space. Here is what that might look like:
 
-```python
-from nitrain import explain
-```
-
 <br />
 
 ## Contributing
 
 If you would like to contribute to nitrain, we would be extremely thankful. The best way to start is by posting an issue to discuss your proposed feature.
```

