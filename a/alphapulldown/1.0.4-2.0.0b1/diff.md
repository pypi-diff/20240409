# Comparing `tmp/alphapulldown-1.0.4.tar.gz` & `tmp/alphapulldown-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphapulldown-1.0.4.tar", last modified: Thu Jan  4 12:59:45 2024, max compression
+gzip compressed data, was "alphapulldown-2.0.0b1.tar", last modified: Tue Apr  9 14:04:56 2024, max compression
```

## Comparing `alphapulldown-1.0.4.tar` & `alphapulldown-2.0.0b1.tar`

### file list

```diff
@@ -1,215 +1,237 @@
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:44.000000 alphapulldown-1.0.4/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:26.000000 alphapulldown-1.0.4/AlphaLink2/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:36.000000 alphapulldown-1.0.4/AlphaLink2/unifold/
--rw-r--r--   0    24600      721       72 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/__init__.py
--rw-r--r--   0    24600      721    10969 2023-11-23 12:22:56.000000 alphapulldown-1.0.4/AlphaLink2/unifold/alphalink_inference.py
--rw-r--r--   0    24600      721    29224 2023-11-23 12:22:57.000000 alphapulldown-1.0.4/AlphaLink2/unifold/config.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:39.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/
--rw-r--r--   0    24600      721      633 2023-11-23 12:22:57.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/__init__.py
--rw-r--r--   0    24600      721    48256 2023-11-23 12:22:57.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/data_ops.py
--rw-r--r--   0    24600      721    19395 2023-11-23 12:22:57.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/msa_pairing.py
--rw-r--r--   0    24600      721     3169 2023-11-23 12:23:02.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/msa_subsampling.py
--rw-r--r--   0    24600      721     8898 2023-11-23 12:22:58.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/process.py
--rw-r--r--   0    24600      721    14694 2023-11-23 12:22:58.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/process_multimer.py
--rw-r--r--   0    24600      721    11218 2023-11-23 12:22:58.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/protein.py
--rw-r--r--   0    24600      721    40939 2023-11-23 12:22:58.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/residue_constants.py
--rw-r--r--   0    24600      721     4177 2023-11-23 12:22:58.000000 alphapulldown-1.0.4/AlphaLink2/unifold/data/utils.py
--rw-r--r--   0    24600      721    24147 2023-11-23 12:23:02.000000 alphapulldown-1.0.4/AlphaLink2/unifold/dataset.py
--rw-r--r--   0    24600      721    20784 2023-11-23 12:23:02.000000 alphapulldown-1.0.4/AlphaLink2/unifold/dataset_inference.py
--rw-r--r--   0    24600      721    10430 2023-11-23 12:23:02.000000 alphapulldown-1.0.4/AlphaLink2/unifold/homo_search.py
--rw-r--r--   0    24600      721     9126 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/inference.py
--rw-r--r--   0    24600      721     7587 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/inference_symmetry.py
--rw-r--r--   0    24600      721     9457 2023-11-23 12:23:07.000000 alphapulldown-1.0.4/AlphaLink2/unifold/loss.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:42.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/
--rw-r--r--   0    24600      721        0 2023-11-23 12:19:01.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/__init__.py
--rw-r--r--   0    24600      721     9122 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/auxillary.py
--rw-r--r--   0    24600      721     7332 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/chain_align.py
--rw-r--r--   0    24600      721     5179 2023-11-23 12:23:03.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/fape.py
--rw-r--r--   0    24600      721    13287 2023-11-23 12:23:04.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/geometry.py
--rw-r--r--   0    24600      721      723 2023-11-23 12:23:04.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/utils.py
--rw-r--r--   0    24600      721    17784 2023-11-23 12:23:04.000000 alphapulldown-1.0.4/AlphaLink2/unifold/losses/violation.py
--rw-r--r--   0    24600      721     1367 2023-11-23 12:23:07.000000 alphapulldown-1.0.4/AlphaLink2/unifold/model.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:47.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/
--rw-r--r--   0    24600      721      118 2023-11-23 12:23:07.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/__init__.py
--rw-r--r--   0    24600      721    16455 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/alphafold.py
--rw-r--r--   0    24600      721    12363 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/attentions.py
--rw-r--r--   0    24600      721     5316 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/auxillary_heads.py
--rw-r--r--   0    24600      721    10489 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/common.py
--rw-r--r--   0    24600      721     5573 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/confidence.py
--rw-r--r--   0    24600      721     8923 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/embedders.py
--rw-r--r--   0    24600      721    11196 2023-11-23 12:23:08.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/evoformer.py
--rw-r--r--   0    24600      721     6428 2023-11-23 12:23:09.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/featurization.py
--rw-r--r--   0    24600      721     1822 2023-11-23 12:23:14.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/flash_attention.py
--rw-r--r--   0    24600      721    17109 2023-11-23 12:23:09.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/frame.py
--rw-r--r--   0    24600      721    18180 2023-11-23 12:23:09.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/structure_module.py
--rw-r--r--   0    24600      721     9593 2023-11-23 12:23:09.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/template.py
--rw-r--r--   0    24600      721     5518 2023-11-23 12:23:09.000000 alphapulldown-1.0.4/AlphaLink2/unifold/modules/triangle_multiplication.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:50.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/
--rw-r--r--   0    24600      721       45 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/__init__.py
--rw-r--r--   0    24600      721    17687 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/mmcif.py
--rw-r--r--   0    24600      721     3130 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/msa_identifiers.py
--rw-r--r--   0    24600      721    23274 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/parsers.py
--rw-r--r--   0    24600      721    11235 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/pipeline.py
--rw-r--r--   0    24600      721    44767 2023-11-23 12:23:15.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/templates.py
--rw-r--r--   0    24600      721     2681 2023-11-23 12:23:17.000000 alphapulldown-1.0.4/AlphaLink2/unifold/msa/utils.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:53.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/
--rw-r--r--   0    24600      721      842 2023-11-23 12:23:20.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/__init__.py
--rw-r--r--   0    24600      721     4276 2023-11-23 12:23:21.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/assemble.py
--rw-r--r--   0    24600      721      910 2023-11-23 12:23:21.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/config.py
--rw-r--r--   0    24600      721     2065 2023-11-23 12:23:21.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/dataset.py
--rw-r--r--   0    24600      721     6782 2023-11-23 12:23:23.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/geometry_utils.py
--rw-r--r--   0    24600      721       23 2023-11-23 12:23:21.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/loss.py
--rw-r--r--   0    24600      721    10094 2023-11-23 12:23:21.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/model.py
--rw-r--r--   0    24600      721     7246 2023-11-23 12:23:22.000000 alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/modules.py
--rw-r--r--   0    24600      721     2523 2023-11-23 12:23:23.000000 alphapulldown-1.0.4/AlphaLink2/unifold/task.py
--rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-1.0.4/LICENSE
--rw-r--r--   0    24600      721       34 2023-11-15 13:03:52.000000 alphapulldown-1.0.4/MANIFEST.in
--rw-r--r--   0    24600      721     7242 2024-01-04 12:59:44.000000 alphapulldown-1.0.4/PKG-INFO
--rw-r--r--   0    24600      721     6235 2024-01-04 10:39:25.000000 alphapulldown-1.0.4/README.md
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:53.000000 alphapulldown-1.0.4/alphafold/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:55.000000 alphapulldown-1.0.4/alphafold/alphafold/
--rw-r--r--   0    24600      721      663 2023-05-16 14:00:32.000000 alphapulldown-1.0.4/alphafold/alphafold/__init__.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:58.000000 alphapulldown-1.0.4/alphafold/alphafold/common/
--rw-r--r--   0    24600      721      655 2023-05-16 14:00:32.000000 alphapulldown-1.0.4/alphafold/alphafold/common/__init__.py
--rw-r--r--   0    24600      721     7973 2023-12-21 15:30:41.000000 alphapulldown-1.0.4/alphafold/alphafold/common/confidence.py
--rw-r--r--   0    24600      721     1434 2023-12-21 15:30:41.000000 alphapulldown-1.0.4/alphafold/alphafold/common/confidence_test.py
--rw-r--r--   0    24600      721     7561 2023-12-21 15:30:41.000000 alphapulldown-1.0.4/alphafold/alphafold/common/mmcif_metadata.py
--rw-r--r--   0    24600      721    22147 2023-12-21 15:30:42.000000 alphapulldown-1.0.4/alphafold/alphafold/common/protein.py
--rw-r--r--   0    24600      721     5791 2023-12-21 15:30:42.000000 alphapulldown-1.0.4/alphafold/alphafold/common/protein_test.py
--rw-r--r--   0    24600      721    35625 2023-12-21 15:30:42.000000 alphapulldown-1.0.4/alphafold/alphafold/common/residue_constants.py
--rw-r--r--   0    24600      721     9256 2023-05-16 14:00:33.000000 alphapulldown-1.0.4/alphafold/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:01.000000 alphapulldown-1.0.4/alphafold/alphafold/data/
--rw-r--r--   0    24600      721      634 2023-05-16 14:00:34.000000 alphapulldown-1.0.4/alphafold/alphafold/data/__init__.py
--rw-r--r--   0    24600      721     8575 2023-05-16 14:00:35.000000 alphapulldown-1.0.4/alphafold/alphafold/data/feature_processing.py
--rw-r--r--   0    24600      721    14182 2023-05-16 14:00:35.000000 alphapulldown-1.0.4/alphafold/alphafold/data/mmcif_parsing.py
--rw-r--r--   0    24600      721     3122 2023-12-21 15:30:44.000000 alphapulldown-1.0.4/alphafold/alphafold/data/msa_identifiers.py
--rw-r--r--   0    24600      721    17220 2023-11-13 12:53:34.000000 alphapulldown-1.0.4/alphafold/alphafold/data/msa_pairing.py
--rw-r--r--   0    24600      721    21397 2023-05-16 14:00:35.000000 alphapulldown-1.0.4/alphafold/alphafold/data/parsers.py
--rw-r--r--   0    24600      721    10419 2024-01-04 10:24:26.000000 alphapulldown-1.0.4/alphafold/alphafold/data/pipeline.py
--rw-r--r--   0    24600      721    11126 2023-05-16 14:00:36.000000 alphapulldown-1.0.4/alphafold/alphafold/data/pipeline_multimer.py
--rw-r--r--   0    24600      721    40741 2023-12-21 15:30:45.000000 alphapulldown-1.0.4/alphafold/alphafold/data/templates.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:04.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/
--rw-r--r--   0    24600      721      639 2023-05-16 14:00:36.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/__init__.py
--rw-r--r--   0    24600      721     5504 2023-05-16 14:00:36.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/hhblits.py
--rw-r--r--   0    24600      721     3601 2023-05-16 14:00:36.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/hhsearch.py
--rw-r--r--   0    24600      721     4576 2023-12-19 15:12:27.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0    24600      721     4556 2023-05-16 14:00:37.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0    24600      721     8386 2023-05-16 14:00:37.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0    24600      721     3387 2023-05-16 14:00:37.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/kalign.py
--rw-r--r--   0    24600      721     1223 2023-05-16 14:00:37.000000 alphapulldown-1.0.4/alphafold/alphafold/data/tools/utils.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:14.000000 alphapulldown-1.0.4/alphafold/alphafold/model/
--rw-r--r--   0    24600      721      617 2023-05-16 14:00:37.000000 alphapulldown-1.0.4/alphafold/alphafold/model/__init__.py
--rw-r--r--   0    24600      721    47028 2023-05-16 14:00:38.000000 alphapulldown-1.0.4/alphafold/alphafold/model/all_atom.py
--rw-r--r--   0    24600      721    40145 2023-05-16 14:00:38.000000 alphapulldown-1.0.4/alphafold/alphafold/model/all_atom_multimer.py
--rw-r--r--   0    24600      721     4706 2023-05-16 14:00:38.000000 alphapulldown-1.0.4/alphafold/alphafold/model/all_atom_test.py
--rw-r--r--   0    24600      721     5957 2023-05-16 14:00:38.000000 alphapulldown-1.0.4/alphafold/alphafold/model/common_modules.py
--rw-r--r--   0    24600      721    26814 2023-05-16 14:00:38.000000 alphapulldown-1.0.4/alphafold/alphafold/model/config.py
--rw-r--r--   0    24600      721     1097 2023-05-16 14:00:39.000000 alphapulldown-1.0.4/alphafold/alphafold/model/data.py
--rw-r--r--   0    24600      721     3692 2023-05-16 14:00:39.000000 alphapulldown-1.0.4/alphafold/alphafold/model/features.py
--rw-r--r--   0    24600      721    37264 2023-05-16 14:00:39.000000 alphapulldown-1.0.4/alphafold/alphafold/model/folding.py
--rw-r--r--   0    24600      721    42498 2023-05-16 14:00:39.000000 alphapulldown-1.0.4/alphafold/alphafold/model/folding_multimer.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:17.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/
--rw-r--r--   0    24600      721     1172 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/__init__.py
--rw-r--r--   0    24600      721     4148 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0    24600      721     5751 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0    24600      721     7745 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0    24600      721     4166 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/test_utils.py
--rw-r--r--   0    24600      721      853 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/utils.py
--rw-r--r--   0    24600      721     6896 2023-05-16 14:00:40.000000 alphapulldown-1.0.4/alphafold/alphafold/model/geometry/vector.py
--rw-r--r--   0    24600      721     9134 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/layer_stack.py
--rw-r--r--   0    24600      721    10315 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/layer_stack_test.py
--rw-r--r--   0    24600      721     3505 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/lddt.py
--rw-r--r--   0    24600      721     2384 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/lddt_test.py
--rw-r--r--   0    24600      721     7963 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/mapping.py
--rw-r--r--   0    24600      721     6613 2023-05-16 14:00:41.000000 alphapulldown-1.0.4/alphafold/alphafold/model/model.py
--rw-r--r--   0    24600      721    74120 2023-05-16 14:00:42.000000 alphapulldown-1.0.4/alphafold/alphafold/model/modules.py
--rw-r--r--   0    24600      721    42351 2023-12-21 15:30:45.000000 alphapulldown-1.0.4/alphafold/alphafold/model/modules_multimer.py
--rw-r--r--   0    24600      721     1978 2023-05-16 14:00:42.000000 alphapulldown-1.0.4/alphafold/alphafold/model/prng.py
--rw-r--r--   0    24600      721     1202 2023-12-21 15:30:45.000000 alphapulldown-1.0.4/alphafold/alphafold/model/prng_test.py
--rw-r--r--   0    24600      721    17388 2023-05-16 14:00:42.000000 alphapulldown-1.0.4/alphafold/alphafold/model/quat_affine.py
--rw-r--r--   0    24600      721     5038 2023-05-16 14:00:42.000000 alphapulldown-1.0.4/alphafold/alphafold/model/quat_affine_test.py
--rw-r--r--   0    24600      721    10935 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/r3.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:21.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/
--rw-r--r--   0    24600      721      633 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/__init__.py
--rw-r--r--   0    24600      721    21428 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/data_transforms.py
--rw-r--r--   0    24600      721     5357 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0    24600      721     5051 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/protein_features.py
--rw-r--r--   0    24600      721     1822 2023-05-16 14:00:43.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0    24600      721     6344 2023-05-16 14:00:44.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0    24600      721     1415 2023-05-16 14:00:44.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0    24600      721     1318 2023-05-16 14:00:44.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0    24600      721      812 2023-05-16 14:00:44.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0    24600      721     1276 2023-05-16 14:00:44.000000 alphapulldown-1.0.4/alphafold/alphafold/model/tf/utils.py
--rw-r--r--   0    24600      721     5432 2023-12-21 15:30:46.000000 alphapulldown-1.0.4/alphafold/alphafold/model/utils.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:22.000000 alphapulldown-1.0.4/alphafold/alphafold/notebooks/
--rw-r--r--   0    24600      721      626 2023-05-16 14:00:45.000000 alphapulldown-1.0.4/alphafold/alphafold/notebooks/__init__.py
--rw-r--r--   0    24600      721     6628 2023-12-21 15:30:46.000000 alphapulldown-1.0.4/alphafold/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0    24600      721     9273 2023-12-21 15:30:46.000000 alphapulldown-1.0.4/alphafold/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:25.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/
--rw-r--r--   0    24600      721      618 2023-05-16 14:00:45.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/__init__.py
--rw-r--r--   0    24600      721    19096 2023-12-21 15:30:47.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/amber_minimize.py
--rw-r--r--   0    24600      721     4348 2023-05-16 14:00:46.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0    24600      721     4820 2023-12-21 15:30:47.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/cleanup.py
--rw-r--r--   0    24600      721     6164 2023-12-21 15:30:47.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/cleanup_test.py
--rw-r--r--   0    24600      721     3288 2023-05-16 14:00:46.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/relax.py
--rw-r--r--   0    24600      721     3827 2023-05-16 14:00:46.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/relax_test.py
--rw-r--r--   0    24600      721     2501 2023-10-26 14:36:43.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/utils.py
--rw-r--r--   0    24600      721     1996 2023-05-16 14:00:48.000000 alphapulldown-1.0.4/alphafold/alphafold/relax/utils_test.py
--rw-r--r--   0    24600      721    19606 2023-06-06 10:25:24.000000 alphapulldown-1.0.4/alphafold/alphafold/run_alphafold.py
--rw-r--r--   0    24600      721      674 2023-12-21 15:30:48.000000 alphapulldown-1.0.4/alphafold/alphafold/version.py
--rw-r--r--   0    24600      721    22575 2023-12-21 15:30:49.000000 alphapulldown-1.0.4/alphafold/run_alphafold.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:31.000000 alphapulldown-1.0.4/alphapulldown/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:29.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:34.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/
--rw-r--r--   0    24600      721        0 2023-05-16 09:15:18.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/__init__.py
--rw-r--r--   0    24600      721    81676 2023-11-14 14:21:50.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/batch.py
--rw-r--r--   0    24600      721     6493 2023-11-14 14:21:50.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/citations.py
--rw-r--r--   0    24600      721    28656 2023-11-14 14:21:50.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/colabfold.py
--rw-r--r--   0    24600      721     2240 2023-11-14 14:21:50.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/download.py
--rw-r--r--   0    24600      721     2120 2023-05-16 09:15:21.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/pdb.py
--rw-r--r--   0    24600      721     5392 2023-11-14 14:21:51.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/plot.py
--rw-r--r--   0    24600      721     3139 2023-11-14 14:21:51.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/relax.py
--rw-r--r--   0    24600      721    10396 2023-11-14 14:21:51.000000 alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/utils.py
--rw-r--r--   0    24600      721       21 2024-01-04 12:57:08.000000 alphapulldown-1.0.4/alphapulldown/__init__.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:37.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/
--rw-r--r--   0    24600      721     7268 2023-08-29 14:43:13.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2_3dmol.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:58:29.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:39.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/
--rw-r--r--   0    24600      721     3745 2023-08-29 10:45:59.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
--rw-r--r--   0    24600      721    11001 2023-08-29 10:45:59.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
--rw-r--r--   0    24600      721       21 2023-08-29 10:45:59.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
--rw-r--r--   0    24600      721     7544 2023-11-21 13:30:28.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/calculate_mpdockq.py
--rw-r--r--   0    24600      721     1821 2023-10-13 10:51:18.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/calculate_rmsd.py
--rw-r--r--   0    24600      721     6588 2024-01-04 12:15:22.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/create_notebook.py
--rw-r--r--   0    24600      721     6900 2023-12-19 14:56:42.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/get_good_inter_pae.py
--rw-r--r--   0    24600      721     3891 2024-01-04 12:01:24.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/test_create_notebook.py
--rw-r--r--   0    24600      721      962 2023-01-27 13:03:03.000000 alphapulldown-1.0.4/alphapulldown/analysis_pipeline/utils.py
--rw-r--r--   0    24600      721     7104 2024-01-04 10:36:01.000000 alphapulldown-1.0.4/alphapulldown/create_custom_template_db.py
--rwxr-xr-x   0    24600      721     9651 2023-12-19 15:01:35.000000 alphapulldown-1.0.4/alphapulldown/create_individual_features.py
--rwxr-xr-x   0    24600      721    11644 2023-12-19 15:01:35.000000 alphapulldown-1.0.4/alphapulldown/create_individual_features_with_templates.py
--rw-r--r--   0    24600      721     1276 2023-11-27 13:30:57.000000 alphapulldown-1.0.4/alphapulldown/generate_crosslink_pickle.py
--rw-r--r--   0    24600      721    25432 2023-12-19 15:01:35.000000 alphapulldown-1.0.4/alphapulldown/objects.py
--rw-r--r--   0    24600      721     2909 2023-11-20 10:48:19.000000 alphapulldown-1.0.4/alphapulldown/plot_pae.py
--rw-r--r--   0    24600      721    10786 2023-12-19 15:01:35.000000 alphapulldown-1.0.4/alphapulldown/predict_structure.py
--rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-1.0.4/alphapulldown/prepare_seq_names.py
--rwxr-xr-x   0    24600      721    14511 2023-12-19 15:01:35.000000 alphapulldown-1.0.4/alphapulldown/remove_clashes_low_plddt.py
--rwxr-xr-x   0    24600      721     1240 2023-11-15 13:03:55.000000 alphapulldown-1.0.4/alphapulldown/rename_colab_search_a3m.py
--rwxr-xr-x   0    24600      721    16790 2023-12-19 15:01:36.000000 alphapulldown-1.0.4/alphapulldown/run_multimer_jobs.py
--rw-r--r--   0    24600      721    22684 2023-12-19 15:01:36.000000 alphapulldown-1.0.4/alphapulldown/utils.py
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:41.000000 alphapulldown-1.0.4/alphapulldown.egg-info/
--rw-r--r--   0    24600      721     7242 2024-01-04 12:58:24.000000 alphapulldown-1.0.4/alphapulldown.egg-info/PKG-INFO
--rw-r--r--   0    24600      721     7833 2024-01-04 12:58:26.000000 alphapulldown-1.0.4/alphapulldown.egg-info/SOURCES.txt
--rw-r--r--   0    24600      721        1 2024-01-04 12:58:24.000000 alphapulldown-1.0.4/alphapulldown.egg-info/dependency_links.txt
--rw-r--r--   0    24600      721      271 2024-01-04 12:58:24.000000 alphapulldown-1.0.4/alphapulldown.egg-info/requires.txt
--rw-r--r--   0    24600      721       69 2024-01-04 12:58:25.000000 alphapulldown-1.0.4/alphapulldown.egg-info/top_level.txt
--rw-r--r--   0    24600      721     2113 2024-01-04 12:59:44.000000 alphapulldown-1.0.4/setup.cfg
--rwxr-xr-x   0    24600      721      124 2023-11-15 13:03:57.000000 alphapulldown-1.0.4/setup.py
--rw-r--r--   0    24600      721     9119 2023-08-29 14:43:16.000000 alphapulldown-1.0.4/stereo_chemical_props.txt
-drwxr-xr-x   0    24600      721        0 2024-01-04 12:59:44.000000 alphapulldown-1.0.4/test/
--rw-r--r--   0    24600      721     5802 2023-10-13 10:51:21.000000 alphapulldown-1.0.4/test/test_create_objects.py
--rw-r--r--   0    24600      721     2963 2023-11-14 10:55:56.000000 alphapulldown-1.0.4/test/test_crosslink_inference.py
--rw-r--r--   0    24600      721     2215 2023-11-14 10:55:56.000000 alphapulldown-1.0.4/test/test_crosslink_input.py
--rw-r--r--   0    24600      721     3081 2024-01-04 10:36:02.000000 alphapulldown-1.0.4/test/test_custom_db.py
--rw-r--r--   0    24600      721     8122 2023-12-19 15:01:43.000000 alphapulldown-1.0.4/test/test_features_with_templates.py
--rwxr-xr-x   0    24600      721      712 2023-11-15 13:06:08.000000 alphapulldown-1.0.4/test/test_predictions_slurm.py
--rwxr-xr-x   0    24600      721     1445 2023-11-15 13:06:09.000000 alphapulldown-1.0.4/test/test_remove_clashes_low_plddt.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.993713 alphapulldown-2.0.0b1/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.547797 alphapulldown-2.0.0b1/AlphaLink2/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.716786 alphapulldown-2.0.0b1/AlphaLink2/unifold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       72 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10975 2024-03-18 14:19:42.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/alphalink_inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    29224 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/config.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.809846 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    48256 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/data_ops.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19395 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_pairing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3169 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_subsampling.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8898 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14694 2024-03-07 11:29:35.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11218 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/protein.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40939 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/residue_constants.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4177 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    24281 2024-03-07 12:08:05.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    20784 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset_inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10430 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/homo_search.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9126 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7587 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/inference_symmetry.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9457 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/loss.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.864779 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2023-11-23 12:19:01.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9122 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/auxillary.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7332 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/chain_align.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5179 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/fape.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    13287 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/geometry.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      723 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17784 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/violation.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1367 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/model.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.945772 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      118 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    16455 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/alphafold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    12363 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/attentions.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5316 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/auxillary_heads.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10489 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/common.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5573 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/confidence.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8923 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/embedders.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11196 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/evoformer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6428 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/featurization.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-11-23 12:23:14.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/flash_attention.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17109 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/frame.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    18180 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/structure_module.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9593 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/template.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5518 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/triangle_multiplication.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.994772 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       45 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17687 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/mmcif.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3130 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/msa_identifiers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    23274 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/parsers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11235 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    44767 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/templates.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2681 2023-11-23 12:23:17.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.062766 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      842 2023-11-23 12:23:20.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4276 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/assemble.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      910 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/config.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2065 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6782 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/geometry_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       23 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/loss.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10094 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/model.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7246 2023-11-23 12:23:22.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2523 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/task.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.553800 alphapulldown-2.0.0b1/ColabFold/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.122766 alphapulldown-2.0.0b1/ColabFold/colabfold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-03-08 10:44:51.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    82218 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/batch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7301 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/citations.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28656 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/colabfold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5308 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/download.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2120 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/pdb.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5392 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/plot.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3139 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/relax.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10468 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35149 2022-08-09 10:02:13.000000 alphapulldown-2.0.0b1/LICENSE
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       34 2023-11-15 13:03:52.000000 alphapulldown-2.0.0b1/MANIFEST.in
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7244 2024-04-09 14:04:55.947719 alphapulldown-2.0.0b1/PKG-INFO
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6235 2024-04-05 14:09:33.000000 alphapulldown-2.0.0b1/README.md
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.844742 alphapulldown-2.0.0b1/alphafold/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.189763 alphapulldown-2.0.0b1/alphafold/alphafold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      663 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b1/alphafold/alphafold/__init__.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.227760 alphapulldown-2.0.0b1/alphafold/alphafold/common/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      655 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7973 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1434 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7561 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/mmcif_metadata.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22147 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/protein.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5791 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/protein_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35625 2024-03-01 11:31:47.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9256 2023-05-16 14:00:33.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.265762 alphapulldown-2.0.0b1/alphafold/alphafold/data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      634 2023-05-16 14:00:34.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8575 2024-04-02 11:51:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/feature_processing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14182 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3122 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_identifiers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17203 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_pairing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21397 2023-05-16 14:00:35.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/parsers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10419 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11126 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40791 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/templates.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.299756 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      639 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5504 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhblits.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3601 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4576 2023-12-19 15:12:27.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4556 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8386 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3387 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/kalign.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1223 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.428756 alphapulldown-2.0.0b1/alphafold/alphafold/model/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      617 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    47028 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40145 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4706 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5957 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/common_modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    26814 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/config.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1097 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/data.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3795 2024-03-27 11:08:31.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    37264 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/folding.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42494 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/folding_multimer.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.490743 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1172 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4148 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5751 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7745 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4166 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      853 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6896 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/vector.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9134 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10315 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3505 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2384 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7963 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/mapping.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6613 2024-03-29 15:44:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/model.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    74087 2024-03-01 11:33:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42351 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/modules_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1978 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/prng.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1202 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/prng_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17388 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5038 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10935 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/r3.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.553752 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21489 2024-03-27 11:00:48.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5357 2024-03-27 11:04:53.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5051 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6344 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1415 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1318 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      812 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5448 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.590739 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      626 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6628 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9273 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.641764 alphapulldown-2.0.0b1/alphafold/alphafold/relax/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      618 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19096 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4348 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4820 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6164 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3288 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3827 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2501 2023-10-26 14:36:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1996 2023-05-16 14:00:48.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19606 2023-06-06 10:25:24.000000 alphapulldown-2.0.0b1/alphafold/alphafold/run_alphafold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      674 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/version.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22575 2024-03-01 11:31:54.000000 alphapulldown-2.0.0b1/alphafold/run_alphafold.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.660742 alphapulldown-2.0.0b1/alphapulldown/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       24 2024-04-09 13:56:06.000000 alphapulldown-2.0.0b1/alphapulldown/__init__.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.686738 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2_3dmol.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.579793 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.700736 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3745 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11001 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       21 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7544 2023-11-21 13:30:28.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/calculate_mpdockq.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6588 2024-04-05 14:09:34.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/create_notebook.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7190 2024-04-09 14:01:52.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/get_good_inter_pae.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3891 2024-01-04 12:01:24.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/test_create_notebook.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1078 2024-04-05 14:09:35.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.738734 alphapulldown-2.0.0b1/alphapulldown/folding_backend/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2820 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    25303 2024-04-05 14:29:45.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphafold_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3320 2024-04-05 14:29:39.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphalink_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2302 2024-04-05 14:23:21.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/folding_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3570 2024-04-05 14:23:21.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/unifold_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28295 2024-04-09 14:01:53.000000 alphapulldown-2.0.0b1/alphapulldown/objects.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.890725 alphapulldown-2.0.0b1/alphapulldown/package_data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9119 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/package_data/stereo_chemical_props.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    12618 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/predict_structure.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.782763 alphapulldown-2.0.0b1/alphapulldown/scripts/
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    48825 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/convert_to_modelcif.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    15939 2024-04-09 14:01:54.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/create_individual_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/generate_crosslink_pickle.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1166 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/prepare_seq_names.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1240 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/rename_colab_search_a3m.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8881 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/run_multimer_jobs.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11865 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/run_structure_prediction.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3038 2024-03-12 10:27:02.000000 alphapulldown-2.0.0b1/alphapulldown/test_new_mmt.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.839764 alphapulldown-2.0.0b1/alphapulldown/utils/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b1/alphapulldown/utils/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4400 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b1/alphapulldown/utils/calculate_rmsd.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1838 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/create_combinations.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7919 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/create_custom_template_db.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4897 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/file_handling.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17488 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/modelling_setup.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7019 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/multimeric_template_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1100 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/plotting.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1447 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/post_modelling.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    15228 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/remove_clashes_low_plddt.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7884 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/save_meta_data.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.943731 alphapulldown-2.0.0b1/alphapulldown.egg-info/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7244 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/PKG-INFO
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8555 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/SOURCES.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        1 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/dependency_links.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      271 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/requires.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       69 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/top_level.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2357 2024-04-09 14:04:55.997715 alphapulldown-2.0.0b1/setup.cfg
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)      124 2023-11-15 13:03:57.000000 alphapulldown-2.0.0b1/setup.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.940720 alphapulldown-2.0.0b1/test/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1043 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_alphalink2_folding_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8545 2024-04-05 14:09:40.000000 alphapulldown-2.0.0b1/test/test_create_monomeric_objects.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1332 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_create_multimeric_objects.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2830 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_create_multimeric_template_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2845 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_crosslink_inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2215 2023-11-14 10:55:56.000000 alphapulldown-2.0.0b1/test/test_crosslink_input.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3071 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b1/test/test_custom_db.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3621 2024-04-05 14:09:46.000000 alphapulldown-2.0.0b1/test/test_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b1/test/test_features_with_templates.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)      712 2023-11-15 13:06:08.000000 alphapulldown-2.0.0b1/test/test_predictions_slurm.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1726 2024-04-05 14:23:34.000000 alphapulldown-2.0.0b1/test/test_python_imports.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1494 2024-04-05 14:23:34.000000 alphapulldown-2.0.0b1/test/test_remove_clashes_low_plddt.py
```

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/alphalink_inference.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/alphalink_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from unicore.utils import (
     tensor_tree_map,
 )
 from unifold.data.data_ops import get_pairwise_distances
 from unifold.data import residue_constants as rc
 import torch
 from alphafold.relax import relax
-from alphapulldown.plot_pae import plot_pae_from_matrix
+from alphapulldown.utils.plotting import plot_pae_from_matrix
 import math,time
 import numpy as np
 import pickle,gzip,os,json
 from unifold.dataset import process_ap
 # from https://github.com/deepmind/alphafold/blob/main/run_alphafold.py
 
 RELAX_MAX_ITERATIONS = 0
```

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/config.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/__init__.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/data_ops.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/data_ops.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/msa_pairing.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/msa_subsampling.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_subsampling.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/process.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/process_multimer.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/protein.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/residue_constants.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/data/utils.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/dataset.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from unifold.data import utils
 from unifold.data.data_ops import NumpyDict, TorchDict
 from unifold.data.process import process_features, process_labels
 from unifold.data.process_multimer import (
     pair_and_merge,
     add_assembly_features,
     convert_monomer_features,
-    merge_msas,
+    merge_msas,post_process
 )
 import gzip, pickle
 from unicore.data import UnicoreDataset, data_utils
 from unicore.distributed import utils as distributed_utils
 
 Rotation = Iterable[Iterable]
 Translation = Iterable
@@ -276,14 +276,15 @@
     seed: int = 0,
     batch_idx: Optional[int] = None,
     is_distillation: bool = False,
     crosslinks: str = None,
     **kwargs
 ) -> TorchExample:
 
+    chain_id_map = kwargs['chain_id_map']
     if mode == "train":
         assert batch_idx is not None
         with data_utils.numpy_seed(seed, batch_idx, key="recycling"):
             num_iters = np.random.randint(0, config.common.max_recycling_iters + 1)
             use_clamped_fape = np.random.rand() < config[mode].use_clamped_fape_prob
     else:
         num_iters = config.common.max_recycling_iters
@@ -306,14 +307,15 @@
         features = utils.filter(features, desired_keys=feature_names)
         features = {k: torch.tensor(v) for k, v in features.items()}
         features["template_mask"] = torch.ones(
         features["template_aatype"].shape[-1], dtype=torch.float32
     ).reshape(1,-1)
         cfg.common.use_template = True
         with torch.no_grad():
+            features['assembly_num_chains'] = torch.tensor([len(chain_id_map)])
             features = process_features(features, cfg.common, cfg[mode])
 
     if labels is not None:
         labels = [{k: torch.tensor(v) for k, v in l.items()} for l in labels]
         with torch.no_grad():
             labels = process_labels(labels)
```

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/dataset_inference.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset_inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/homo_search.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/homo_search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/inference.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/inference_symmetry.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/inference_symmetry.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/loss.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/loss.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/auxillary.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/auxillary.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/chain_align.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/chain_align.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/fape.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/fape.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/geometry.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/geometry.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/utils.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/losses/violation.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/violation.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/model.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/alphafold.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/attentions.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/auxillary_heads.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/auxillary_heads.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/common.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/common.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/confidence.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/embedders.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/embedders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/evoformer.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/evoformer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/featurization.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/featurization.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/flash_attention.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/flash_attention.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/frame.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/frame.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/structure_module.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/structure_module.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/template.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/template.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/modules/triangle_multiplication.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/triangle_multiplication.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/mmcif.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/mmcif.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/msa_identifiers.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/parsers.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/pipeline.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/templates.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/msa/utils.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/__init__.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/assemble.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/assemble.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/config.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/dataset.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/geometry_utils.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/model.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/symmetry/modules.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/AlphaLink2/unifold/task.py` & `alphapulldown-2.0.0b1/AlphaLink2/unifold/task.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/LICENSE` & `alphapulldown-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/PKG-INFO` & `alphapulldown-2.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphapulldown
-Version: 1.0.4
+Version: 2.0.0b1
 Summary: Pipeline allows massive screening using alphafold
 Home-page: https://github.com/KosinskiLab/AlphaPulldown
 Author: Dingquan Yu
 Author-email: dingquan.yu@embl-hamburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: dm-haiku
 Requires-Dist: dm-tree>=0.1.6
 Requires-Dist: h5py>=3.1.0
 Requires-Dist: matplotlib>=3.3.3
 Requires-Dist: ml-collections>=0.1.0
 Requires-Dist: numpy
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: tensorflow>=2.14.0
+Requires-Dist: tensorflow==2.14.0
 Requires-Dist: importlib-resources>=6.1.0
 Requires-Dist: biopython==1.81
 Requires-Dist: nbformat>=5.9.2
 Requires-Dist: py3Dmol==2.0.4
 Requires-Dist: ipython==8.16.1
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: appdirs>=1.4.4
@@ -94,15 +94,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.3
+python3 -m pip install alphapulldown==1.0.4
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-1.0.4/README.md` & `alphapulldown-2.0.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.3
+python3 -m pip install alphapulldown==1.0.4
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/confidence.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/confidence_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/mmcif_metadata.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/mmcif_metadata.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/protein.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/protein_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/residue_constants.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/common/residue_constants_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/feature_processing.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/mmcif_parsing.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/msa_identifiers.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/msa_pairing.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_pairing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Pairing logic for multimer data pipeline."""
 
 import collections
-import functools
-import string
-from typing import Any, Dict, Iterable, List, Sequence
+from typing import cast, Dict, Iterable, List, Sequence
 
 from alphafold.common import residue_constants
 from alphafold.data import pipeline
 import numpy as np
 import pandas as pd
 import scipy.linalg
 
@@ -131,15 +129,15 @@
   return msa_df
 
 
 def _create_species_dict(msa_df: pd.DataFrame) -> Dict[bytes, pd.DataFrame]:
   """Creates mapping from species to msa dataframe of that species."""
   species_lookup = {}
   for species, species_df in msa_df.groupby('msa_species_identifiers'):
-    species_lookup[species] = species_df
+    species_lookup[cast(bytes, species)] = species_df
   return species_lookup
 
 
 def _match_rows_by_sequence_similarity(this_species_msa_dfs: List[pd.DataFrame]
                                        ) -> List[List[int]]:
   """Finds MSA sequence pairings across chains based on sequence similarity.
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/parsers.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/pipeline.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/pipeline_multimer.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/templates.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,14 +445,15 @@
   all_positions_mask = np.zeros([num_res, residue_constants.atom_type_num],
                                 dtype=np.int64)
   for res_index in range(num_res):
     pos = np.zeros([residue_constants.atom_type_num, 3], dtype=np.float32)
     mask = np.zeros([residue_constants.atom_type_num], dtype=np.float32)
     res_at_position = mmcif_object.seqres_to_structure[auth_chain_id][res_index]
     if not res_at_position.is_missing:
+      assert res_at_position.position is not None
       res = chain[(res_at_position.hetflag,
                    res_at_position.position.residue_number,
                    res_at_position.position.insertion_code)]
       for atom in res.get_atoms():
         atom_name = atom.get_name()
         x, y, z = atom.get_coord()
         if atom_name in residue_constants.atom_order.keys():
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/hhblits.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/hhsearch.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/hmmbuild.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/hmmsearch.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/jackhmmer.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/kalign.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/data/tools/utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/all_atom.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/all_atom_multimer.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/all_atom_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/common_modules.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/config.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/data.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/features.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,18 +73,21 @@
     features = sess.run(processed_batch)
 
   return {k: v for k, v in features.items() if v.dtype != 'O'}
 
 
 def np_example_to_features(np_example: FeatureDict,
                            config: ml_collections.ConfigDict,
-                           random_seed: int = 0) -> FeatureDict:
+                           random_seed: int = 0, desired_num_res: int = None) -> FeatureDict:
   """Preprocesses NumPy feature dict using TF pipeline."""
   np_example = dict(np_example)
-  num_res = int(np_example['seq_length'][0])
+  if desired_num_res is not None:
+    num_res = desired_num_res
+  else:
+    num_res = int(np_example['seq_length'][0])
   cfg, feature_names = make_data_config(config, num_res=num_res)
 
   if 'deletion_matrix_int' in np_example:
     np_example['deletion_matrix'] = (
         np_example.pop('deletion_matrix_int').astype(np.float32))
 
   tf_graph = tf.Graph()
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/folding.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/folding_multimer.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/folding_multimer.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,15 +771,15 @@
       pred_positions=pred_pos)
 
   use_alt = alt_naming_is_better[:, None]
 
   gt_mask = (1. - use_alt) * gt_mask + use_alt * alt_gt_mask
   gt_positions = (1. - use_alt) * gt_positions + use_alt * alt_gt_positions
 
-  return gt_positions, alt_gt_mask, alt_naming_is_better
+  return gt_positions, gt_mask, alt_naming_is_better
 
 
 def backbone_loss(gt_rigid: geometry.Rigid3Array,
                   gt_frames_mask: jnp.ndarray,
                   gt_positions_mask: jnp.ndarray,
                   target_rigid: geometry.Rigid3Array,
                   config: ml_collections.ConfigDict,
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/rigid_matrix_vector.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/rotation_matrix.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/struct_of_array.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/test_utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/geometry/vector.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/layer_stack.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/layer_stack_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/lddt.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/lddt_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/mapping.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/model.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/modules.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
       }
       return jax.tree_map(jax.lax.stop_gradient, new_prev)
 
     def do_call(prev,
                 recycle_idx,
                 compute_loss=compute_loss):
       if self.config.resample_msa_in_recycling:
-        num_ensemble = batch_size // (self.config.num_recycle + 1)
+        num_ensemble = batch_size
         def slice_recycle_idx(x):
           start = recycle_idx * num_ensemble
           size = num_ensemble
           return jax.lax.dynamic_slice_in_dim(x, start, size, axis=0)
         ensembled_batch = jax.tree_map(slice_recycle_idx, batch)
       else:
         num_ensemble = batch_size
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/modules_multimer.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/prng.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/prng_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/quat_affine.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/quat_affine_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/r3.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/data_transforms.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/data_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from alphafold.common import residue_constants
 from alphafold.model.tf import shape_helpers
 from alphafold.model.tf import shape_placeholders
 from alphafold.model.tf import utils
 import numpy as np
 import tensorflow.compat.v1 as tf
-
 # Pylint gets confused by the curry1 decorator because it changes the number
 #   of arguments to the function.
 # pylint:disable=no-value-for-parameter
 
 
 NUM_RES = shape_placeholders.NUM_RES
 NUM_MSA_SEQ = shape_placeholders.NUM_MSA_SEQ
@@ -409,27 +408,28 @@
   return protein
 
 
 @curry1
 def make_fixed_size(protein, shape_schema, msa_cluster_size, extra_msa_size,
                     num_res, num_templates=0):
   """Guess at the MSA and sequence dimensions to make fixed size."""
-
   pad_size_map = {
       NUM_RES: num_res,
       NUM_MSA_SEQ: msa_cluster_size,
       NUM_EXTRA_SEQ: extra_msa_size,
       NUM_TEMPLATES: num_templates,
   }
-
   for k, v in protein.items():
     # Don't transfer this to the accelerator.
     if k == 'extra_cluster_assignment':
       continue
-    shape = v.shape.as_list()
+    if type(v) ==np.ndarray:
+      shape = v.shape 
+    else:
+      shape = v.shape.as_list()
     schema = shape_schema[k]
     assert len(shape) == len(schema), (
         f'Rank mismatch between shape and shape schema for {k}: '
         f'{shape} vs {schema}')
     pad_size = [
         pad_size_map.get(s2, None) or s1 for (s1, s2) in zip(shape, schema)
     ]
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/input_pipeline.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/protein_features.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/protein_features_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/proteins_dataset.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_helpers.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_helpers_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/shape_placeholders.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/tf/utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/model/utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,16 @@
     new_keys = jax.vmap(functools.partial(jax.random.fold_in, key))(
         jnp.arange(shape[0]))
     return jax.vmap(functools.partial(grid_keys, shape=shape[1:]))(new_keys)
 
   def inner(key, shape, **kwargs):
     keys = grid_keys(key, shape)
     signature = (
-        '()->()' if isinstance(keys, jax.random.PRNGKeyArray) else '(2)->()'
+        '()->()'
+        if isinstance(keys, jax.random.PRNGKeyArray)
+        else '(2)->()'
     )
     return jnp.vectorize(
         functools.partial(f, shape=(), **kwargs), signature=signature
     )(keys)
 
   return inner
```

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/notebooks/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/notebooks/notebook_utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/notebooks/notebook_utils_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/__init__.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/amber_minimize.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/amber_minimize_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/cleanup.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/cleanup_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/relax.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/relax_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/utils.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/relax/utils_test.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/run_alphafold.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/alphafold/version.py` & `alphapulldown-2.0.0b1/alphafold/alphafold/version.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphafold/run_alphafold.py` & `alphapulldown-2.0.0b1/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/batch.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sys
 import time
 import zipfile
 import shutil
 import pickle
 import gzip
 
-from argparse import ArgumentParser
+from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 from io import StringIO
 
 import importlib_metadata
 import numpy as np
 import pandas
@@ -71,15 +71,19 @@
 from Bio.PDB import MMCIFParser, PDBParser, MMCIF2Dict
 from Bio.PDB.PDBIO import Select
 
 # logging settings
 logger = logging.getLogger(__name__)
 import jax
 import jax.numpy as jnp
-logging.getLogger('jax._src.lib.xla_bridge').addFilter(lambda _: False)
+
+# from jax 0.4.6, jax._src.lib.xla_bridge moved to jax._src.xla_bridge
+# suppress warnings: Unable to initialize backend 'rocm' or 'tpu'
+logging.getLogger('jax._src.xla_bridge').addFilter(lambda _: False) # jax >=0.4.6
+logging.getLogger('jax._src.lib.xla_bridge').addFilter(lambda _: False) # jax < 0.4.5
 
 def mk_mock_template(
     query_sequence: Union[List[str], str], num_temp: int = 1
 ) -> Dict[str, Any]:
     ln = (
         len(query_sequence)
         if isinstance(query_sequence, str)
@@ -340,15 +344,14 @@
     use_gpu_relax: bool = False,
     save_all: bool = False,
     save_single_representations: bool = False,
     save_pair_representations: bool = False,
     save_recycles: bool = False,
 ):
     """Predicts structure using AlphaFold for the given sequence."""
-
     mean_scores = []
     conf = []
     unrelaxed_pdb_lines = []
     prediction_times = []
     model_names = []
     files = file_manager(prefix, result_dir)
     seq_len = sum(sequences_lengths)
@@ -645,15 +648,15 @@
     if sort_queries_by == "length":
         queries.sort(key=lambda t: len("".join(t[1])))
 
     elif sort_queries_by == "random":
         random.shuffle(queries)
 
     is_complex = False
-    for job_number, (raw_jobname, query_sequence, a3m_lines) in enumerate(queries):
+    for job_number, (_, query_sequence, a3m_lines) in enumerate(queries):
         if isinstance(query_sequence, list):
             is_complex = True
             break
         if a3m_lines is not None and a3m_lines[0].startswith("#"):
             a3m_line = a3m_lines[0].splitlines()[0]
             tab_sep_entries = a3m_line[1:].split("\t")
             if len(tab_sep_entries) == 2:
@@ -988,15 +991,15 @@
             [
                 template != b"none"
                 for i in template_features
                 for template in i["template_domain_names"]
             ]
         ):
             logger.warning(
-                "alphafold2_ptm complex does not consider templates. Chose multimer model-type for template support."
+                f"{model_type} complex does not consider templates. Chose multimer model-type for template support."
             )
 
     else:
         features_for_chain = {}
         chain_cnt = 0
         # for each unique sequence
         for sequence_index, sequence in enumerate(query_seqs_unique):
@@ -1110,19 +1113,19 @@
                 if seq[pos].islower():
                     continue
                 if seq[pos] != "-":
                     has_amino_acid[n] = True
                 curr_seq_len += 1
             seqs_line.append(paired_seq)
 
-        # is sequence is paired add them to output
+        # if sequence is paired add them to output
         if (
             not is_single_protein
             and not is_homooligomer
-            and sum(has_amino_acid) == len(query_seq_len)
+            and sum(has_amino_acid) > 1 # at least 2 sequences are paired
         ):
             header_no_faster = header.replace(">", "")
             header_no_faster_split = header_no_faster.split("\t")
             for j in range(0, len(seqs_line)):
                 paired_msa[j] += ">" + header_no_faster_split[j] + "\n"
                 paired_msa[j] += seqs_line[j] + "\n"
         else:
@@ -1243,14 +1246,15 @@
     random_seed: int = 0,
     num_seeds: int = 1,
     recompile_padding: Union[int, float] = 10,
     zip_results: bool = False,
     prediction_callback: Callable[[Any, Any, Any, Any, Any], Any] = None,
     save_single_representations: bool = False,
     save_pair_representations: bool = False,
+    jobname_prefix: Optional[str] = None,
     save_all: bool = False,
     save_recycles: bool = False,
     use_dropout: bool = False,
     use_gpu_relax: bool = False,
     stop_at_score: float = 100,
     dpi: int = 200,
     max_seq: Optional[int] = None,
@@ -1288,22 +1292,14 @@
     from colabfold.plot import plot_msa_v2
 
     data_dir = Path(data_dir)
     result_dir = Path(result_dir)
     result_dir.mkdir(exist_ok=True)
     model_type = set_model_type(is_complex, model_type)
 
-    # determine model extension
-    if   model_type == "alphafold2_multimer_v1": model_suffix = "_multimer"
-    elif model_type == "alphafold2_multimer_v2": model_suffix = "_multimer_v2"
-    elif model_type == "alphafold2_multimer_v3": model_suffix = "_multimer_v3"
-    elif model_type == "alphafold2_ptm":         model_suffix = "_ptm"
-    elif model_type == "alphafold2":             model_suffix = ""
-    else: raise ValueError(f"Unknown model_type {model_type}")
-
     # backward-compatibility with old options
     old_names = {"MMseqs2 (UniRef+Environmental)":"mmseqs2_uniref_env",
                  "MMseqs2 (UniRef only)":"mmseqs2_uniref",
                  "unpaired+paired":"unpaired_paired"}
     msa_mode   = old_names.get(msa_mode,msa_mode)
     pair_mode  = old_names.get(pair_mode,pair_mode)
     feature_dict_callback = kwargs.pop("input_features_callback", feature_dict_callback)
@@ -1414,16 +1410,23 @@
 
     if custom_template_path is not None:
         mk_hhsearch_db(custom_template_path)
 
     pad_len = 0
     ranks, metrics = [],[]
     first_job = True
+    job_number = 0
     for job_number, (raw_jobname, query_sequence, a3m_lines) in enumerate(queries):
-        jobname = safe_filename(raw_jobname)
+        if jobname_prefix is not None:
+            # pad job number based on number of queries
+            fill = len(str(len(queries)))
+            jobname = safe_filename(jobname_prefix) + "_" + str(job_number).zfill(fill)
+            job_number += 1
+        else:
+            jobname = safe_filename(raw_jobname)
 
         #######################################
         # check if job has already finished
         #######################################
         # In the colab version and with --zip we know we're done when a zip file has been written
         result_zip = result_dir.joinpath(jobname).with_suffix(".result.zip")
         if keep_existing_results and result_zip.is_file():
@@ -1548,15 +1551,15 @@
 
                     model_runner_and_params = load_models_and_params(
                         num_models=num_models,
                         use_templates=use_templates,
                         num_recycles=num_recycles,
                         num_ensemble=num_ensemble,
                         model_order=model_order,
-                        model_suffix=model_suffix,
+                        model_type=model_type,
                         data_dir=data_dir,
                         stop_at_score=stop_at_score,
                         rank_by=rank_by,
                         use_dropout=use_dropout,
                         max_seq=max_seq,
                         max_extra_seq=max_extra_seq,
                         use_cluster_profile=use_cluster_profile,
@@ -1617,21 +1620,21 @@
             if "pae" in scores[0]:
                 af_pae_file = result_dir.joinpath(f"{jobname}_predicted_aligned_error_v1.json")
                 af_pae_file.write_text(json.dumps({
                     "predicted_aligned_error":scores[0]["pae"],
                     "max_predicted_aligned_error":scores[0]["max_pae"]}))
                 result_files.append(af_pae_file)
 
-            # make pAE plots
-            paes_plot = plot_paes([np.asarray(x["pae"]) for x in scores],
-                Ls=query_sequence_len_array, dpi=dpi)
-            pae_png = result_dir.joinpath(f"{jobname}_pae.png")
-            paes_plot.savefig(str(pae_png), bbox_inches='tight')
-            paes_plot.close()
-            result_files.append(pae_png)
+                # make pAE plots
+                paes_plot = plot_paes([np.asarray(x["pae"]) for x in scores],
+                    Ls=query_sequence_len_array, dpi=dpi)
+                pae_png = result_dir.joinpath(f"{jobname}_pae.png")
+                paes_plot.savefig(str(pae_png), bbox_inches='tight')
+                paes_plot.close()
+                result_files.append(pae_png)
 
             # make pLDDT plot
             plddt_plot = plot_plddts([np.asarray(x["plddt"]) for x in scores],
                 Ls=query_sequence_len_array, dpi=dpi)
             plddt_png = result_dir.joinpath(f"{jobname}_plddt.png")
             plddt_plot.savefig(str(plddt_png), bbox_inches='tight')
             plddt_plot.close()
@@ -1651,29 +1654,32 @@
                 is_done_marker.touch()
 
     logger.info("Done")
     return {"rank":ranks,"metric":metrics}
 
 def set_model_type(is_complex: bool, model_type: str) -> str:
     # backward-compatibility with old options
-    old_names = {"AlphaFold2-multimer-v1":"alphafold2_multimer_v1",
-                 "AlphaFold2-multimer-v2":"alphafold2_multimer_v2",
-                 "AlphaFold2-multimer-v3":"alphafold2_multimer_v3",
-                 "AlphaFold2-ptm":        "alphafold2_ptm",
-                 "AlphaFold2":            "alphafold2"}
+    old_names = {
+        "AlphaFold2-multimer-v1":"alphafold2_multimer_v1",
+        "AlphaFold2-multimer-v2":"alphafold2_multimer_v2",
+        "AlphaFold2-multimer-v3":"alphafold2_multimer_v3",
+        "AlphaFold2-ptm":        "alphafold2_ptm",
+        "AlphaFold2":            "alphafold2",
+        "DeepFold":              "deepfold_v1",
+    }
     model_type = old_names.get(model_type, model_type)
     if model_type == "auto":
         if is_complex:
             model_type = "alphafold2_multimer_v3"
         else:
             model_type = "alphafold2_ptm"
     return model_type
 
 def main():
-    parser = ArgumentParser()
+    parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
     parser.add_argument(
         "input",
         default="input",
         help="One of: 1) directory with FASTA/A3M files, 2) CSV/TSV file, 3) FASTA file or 4) A3M file.",
     )
     parser.add_argument("results", help="Results output directory.")
 
@@ -1797,14 +1803,15 @@
         choices=[
             "auto",
             "alphafold2",
             "alphafold2_ptm",
             "alphafold2_multimer_v1",
             "alphafold2_multimer_v2",
             "alphafold2_multimer_v3",
+            "deepfold_v1",
         ],
     )
     pred_group.add_argument("--model-order", default="1,2,3,4,5", type=str)
     pred_group.add_argument(
         "--use-dropout",
         default=False,
         action="store_true",
@@ -1901,14 +1908,20 @@
         "--stop-at-score",
         help="Compute models until pLDDT (single chain) or pTM-score (multimer) > threshold is reached. "
         "This speeds up prediction by running less models for easier queries.",
         type=float,
         default=100,
     )
     output_group.add_argument(
+        "--jobname-prefix",
+        help="If set, the jobname will be prefixed with the given string and a running number, instead of the input headers/accession.",
+        type=str,
+        default=None,
+    )
+    output_group.add_argument(
         "--save-all",
         default=False,
         action="store_true",
         help="Save all raw outputs from model to a pickle file. "
         "Useful for downstream use in other models."
     )
     output_group.add_argument(
@@ -2055,13 +2068,14 @@
         max_seq=args.max_seq,
         max_extra_seq=args.max_extra_seq,
         max_msa=args.max_msa,
         pdb_hit_file=args.pdb_hit_file,
         local_pdb_path=args.local_pdb_path,
         use_cluster_profile=not args.disable_cluster_profile,
         use_gpu_relax = args.use_gpu_relax,
+        jobname_prefix=args.jobname_prefix,
         save_all=args.save_all,
         save_recycles=args.save_recycles,
     )
 
 if __name__ == "__main__":
     main()
```

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/citations.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/citations.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,44 +85,59 @@
 journal = {Nucleic Acids Res.},
 number = {D1},
 pages = {D170--D176},
 pmid = {27899574},
 title = {{Uniclust databases of clustered and deeply annotated protein sequences and alignments}},
 volume = {45},
 year = {2017},
-comment = {Uniclust30/UniRef30 database},
+comment = {Uniclust30/UniRef30 database}
 }""",
     "Berman2003": """@misc{Berman2003,
 author = {Berman, Helen and Henrick, Kim and Nakamura, Haruki},
 booktitle = {Nat. Struct. Biol.},
 doi = {10.1038/nsb1203-980},
 number = {12},
 pages = {980},
 pmid = {14634627},
 title = {{Announcing the worldwide Protein Data Bank}},
 volume = {10},
 year = {2003},
 comment = {templates downloaded from wwPDB server}
 }""",
+    "Lee2023": """@article{Lee2023,
+author = {Lee, Jae-Won and Won, Jong-Hyun and Jeon, Seonggwang and Choo, Yujin and Yeon, Yubin and Oh, Jin-Seon and Kim, Minsoo and Kim, SeonHwa and Joung, InSuk and Jang, Cheongjae and Lee, Sung Jong and Kim, Tae Hyun and Jin, Kyong Hwan and Song, Giltae and Kim, Eun-Sol and Yoo, Jejoong and Paek, Eunok and Noh, Yung-Kyun and Joo, Keehyoung},
+title = "{DeepFold: enhancing protein structure prediction through optimized loss functions, improved template features, and re-optimized energy function}",
+journal = {Bioinformatics},
+volume = {39},
+number = {12},
+pages = {btad712},
+year = {2023},
+month = {11},
+doi = {10.1093/bioinformatics/btad712},
+comment = {DeepFold-v1 Model}
+}
+""",
 }
 
 
 def write_bibtex(
     model: str,
     use_msa: bool,
     use_env: bool,
     use_templates: bool,
     use_amber: bool,
     result_dir: Path,
     bibtex_file: str = "cite.bibtex",
 ) -> Path:
     to_cite = ["Mirdita2021"]
-    if model == "AlphaFold2-ptm":
+    if model == "alphafold2_ptm" or model == "alphafold2":
         to_cite += ["Jumper2021"]
-    if model.startswith("AlphaFold2-multimer"):
+    if model == "deepfold_v1":
+        to_cite += ["Lee2023"]
+    if model.startswith("alphafold2_multimer"):
         to_cite += ["Evans2021"]
     if use_msa:
         to_cite += ["Mirdita2019"]
     if use_msa:
         to_cite += ["Mirdita2017"]
     if use_env:
         to_cite += ["Mitchell2019"]
```

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/colabfold.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/pdb.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/plot.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/relax.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/ColabFold/colabfold/utils.py` & `alphapulldown-2.0.0b1/ColabFold/colabfold/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,17 @@
 _struct_asym.id
 _struct_asym.entity_id
 #\n"""
             )
             chain_idx = 1
             for model in self.structure:
                 for chain in model:
-                    label_asym_id = asym_id_auth_to_label[chain.get_id()]
-                    out_file.write(f"{label_asym_id} {chain_idx}\n")
+                    if chain.get_id() in asym_id_auth_to_label:
+                        label_asym_id = asym_id_auth_to_label[chain.get_id()]
+                        out_file.write(f"{label_asym_id} {chain_idx}\n")
                     chain_idx += 1
             out_file.write("#\n")
 
         ### begin section copied from Bio.PDB
         for key, key_list in key_lists.items():
             # Pick a sample mmCIF value, which can be a list or a single value
             sample_val = self.dic[key + "." + key_list[0]]
```

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2_3dmol.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2_3dmol.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #
 # Author: Grzegorz Chojnowski @ EMBL-Hamburg
 #
 
 import os, sys, re
 import glob
 import iotbx
+import cctbx
 import iotbx.pdb
-
+import re
 import py3Dmol
 from scitbx import matrix
 from scitbx.math import superpose
+import numpy as np
+
+PLDDT_BANDS = [(50, '#FF7D45'), (70, '#FFDB13'), (90, '#65CBF3'), (100, '#0053D6')]
 
 def parse_pdbstring(pdb_string):
 
     # there may be issues with repeated BREAK lines, that we do not use here anyway
     pdb_string_lines = []
     for _line in pdb_string.splitlines():
         if re.match(r"^BREAK$", _line):
@@ -52,15 +56,18 @@
 def parse_results(output, color=None, models=5, multimer=False):
 
     if color is None:
         color = ["lDDT", "rainbow", "chain"][0]
 
     datadir = os.path.expanduser(output)
 
-    pdb_fnames = sorted(glob.glob("%s/ranked*.pdb" % datadir))
+    # now sorted numerically
+    pattern = r"ranked_(\d+)\.pdb"
+    pdb_fnames = sorted(glob.glob("%s/ranked*.pdb" % datadir),
+                        key=lambda x: int(re.search(pattern,x).group(1)))
 
     ph_array = []
     for idx, fn in enumerate(pdb_fnames[:models]):
         _ph, _symm = read_ph(fn)
         if len(ph_array) > 0:
             _s = superpose.least_squares_fit(
                 ph_array[0].atoms().extract_xyz(),
@@ -85,14 +92,17 @@
         view.addModel(ph_array[0].as_pdb_string(), "pdb", viewer=viewer)
         view.zoomTo(viewer=viewer)
         set_3dmol_styles(
             view, viewer, chain_ids=[_.id for _ in _ph.chains()], color="chain"
         )
 
         viewer = (0, 1)
+
+        set_b_to_plddtbands(ph_array[0])
+
         view.addModel(ph_array[0].as_pdb_string(), "pdb", viewer=viewer)
         view.zoomTo(viewer=viewer)
         set_3dmol_styles(
             view, viewer, chain_ids=[_.id for _ in _ph.chains()], color="lDDT"
         )
 
     else:
@@ -101,30 +111,36 @@
             width=400 * frames,
             height=400,
             viewergrid=(1, frames),
         )
 
         for idx, _ph in enumerate(ph_array):
             viewer = (0, idx)
+
+            if color=="lDDT": set_b_to_plddtbands(_ph)
+
             view.addModel(_ph.as_pdb_string(), "pdb", viewer=viewer)
             view.zoomTo(viewer=viewer)
 
             set_3dmol_styles(view, viewer, chain_ids=chain_ids, color=color)
 
     view.show()
 
 
 def parse_results_colour_chains(output, color=None, models=5, multimer=False):
 
     if color is None:
         color = ["chain"][0]
 
     datadir = os.path.expanduser(output)
-
-    pdb_fnames = sorted(glob.glob("%s/ranked*.pdb" % datadir))
+    
+    # now sorted numerically
+    pattern = r"ranked_(\d+)\.pdb"
+    pdb_fnames = sorted(glob.glob("%s/ranked*.pdb" % datadir),
+                        key=lambda x: int(re.search(pattern,x).group(1)))
 
     ph_array = []
     for idx, fn in enumerate(pdb_fnames[:models]):
         _ph, _symm = read_ph(fn)
         if len(ph_array) > 0:
             _s = superpose.least_squares_fit(
                 ph_array[0].atoms().extract_xyz(),
@@ -165,25 +181,36 @@
             width=400 * frames,
             height=400,
             viewergrid=(1, frames),
         )
 
         for idx, _ph in enumerate(ph_array):
             viewer = (0, idx)
+
+            if color=="lDDT": set_b_to_plddtbands(_ph)
+
             view.addModel(_ph.as_pdb_string(), "pdb", viewer=viewer)
             view.zoomTo(viewer=viewer)
 
             set_3dmol_styles(view, viewer, chain_ids=chain_ids, color=color)
 
     view.show()
 
 
 # ------------------------------------------------------
 
 
+def set_b_to_plddtbands(ph):
+
+    plddt_lims = np.array([_[0] for _ in PLDDT_BANDS])
+    for resi in ph.residue_groups():
+        resi.atoms().set_b(new_b=cctbx.array_family.flex.double(resi.atoms().size(), float(np.argmax(plddt_lims>resi.atoms()[0].b))))
+
+# ------------------------------------------------------
+
 def set_3dmol_styles(
     view,
     viewer,
     chain_ids=1,
     color=["lDDT", "rainbow", "chain"][0],
     show_sidechains=False,
     show_mainchains=False,
@@ -191,22 +218,23 @@
 
     """
     borrowed from colabfolds notebook at
     https://github.com/sokrypton/ColabFold/blob/main/colabfold/pdb.py
     """
 
     if color == "lDDT":
+
+        color_map = {i: band[1] for i, band in enumerate(PLDDT_BANDS)}
+
         view.setStyle(
             {
                 "cartoon": {
                     "colorscheme": {
                         "prop": "b",
-                        "gradient": "roygb",
-                        "min": 0,
-                        "max": 100,
+                        'map': color_map
                     }
                 }
             },
             viewer=viewer,
         )
     elif color == "rainbow":
         view.setStyle({"cartoon": {"color": "spectrum"}}, viewer=viewer)
```

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/calculate_mpdockq.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/calculate_mpdockq.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/create_notebook.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/get_good_inter_pae.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/get_good_inter_pae.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         mpDockq_or_pdockq = "None"
     return mpDockq_or_pdockq
 
 def run_and_summarise_pi_score(workd_dir,jobs,surface_thres):
 
     """A function to calculate all predicted models' pi_scores and make a pandas df of the results"""
     try:
-        os.remove(f"mkdir {workd_dir}/pi_score_outputs")
+        os.rmdir(f"{workd_dir}/pi_score_outputs")
     except:
         pass
     subprocess.run(f"mkdir {workd_dir}/pi_score_outputs",shell=True,executable='/bin/bash')
     pi_score_outputs = os.path.join(workd_dir,"pi_score_outputs")
     for job in jobs:
         subdir = os.path.join(workd_dir,job)
         if not os.path.isfile(os.path.join(subdir,"ranked_0.pdb")):
@@ -117,40 +117,43 @@
             best_model = json.load(open(os.path.join(result_subdir,"ranking_debug.json"),'rb'))['order'][0]
             data = json.load(open(os.path.join(result_subdir,"ranking_debug.json"),'rb'))
             if "iptm" in data.keys() or "iptm+ptm" in data.keys():
                 iptm_ptm_score = data['iptm+ptm'][best_model]
                 try:
                     check_dict = pickle.load(open(os.path.join(result_subdir,f"result_{best_model}.pkl"),'rb'))
                 except FileNotFoundError:
-                    print(os.path.join(result_subdir,f"result_{best_model}.pkl")+" does not exist. Will search for pkl.gz")
+                    logging.info(os.path.join(result_subdir,f"result_{best_model}.pkl")+" does not exist. Will search for pkl.gz")
                     check_dict = pickle.load(gzip.open(os.path.join(result_subdir,f"result_{best_model}.pkl.gz"),'rb'))
                 finally:
-                    print(f"finished reading result pickle for the best model.")
+                    logging.info(f"finished reading result pickle for the best model.")
                 seqs = check_dict['seqs']
                 iptm_score = check_dict['iptm']
                 pae_mtx = check_dict['predicted_aligned_error']
                 check = examine_inter_pae(pae_mtx,seqs,cutoff=FLAGS.cutoff)
                 mpDockq_score = obtain_mpdockq(os.path.join(FLAGS.output_dir,job))
                 if check:
                     good_jobs.append(str(job))
                     iptm_ptm.append(iptm_ptm_score)
                     iptm.append(iptm_score)
                     mpDockq_scores.append(mpDockq_score)
             logging.info(f"done for {job} {count} out of {len(jobs)} finished.")
-    other_measurements_df=pd.DataFrame.from_dict({
-        "jobs":good_jobs,
-        "iptm_ptm":iptm_ptm,
-        "iptm":iptm,
-        "mpDockQ/pDockQ":mpDockq_scores
-    })
-    pi_score_df = run_and_summarise_pi_score(FLAGS.output_dir,good_jobs,FLAGS.surface_thres)
-    pi_score_df=pd.merge(pi_score_df,other_measurements_df,on="jobs")
-    columns = list(pi_score_df.columns.values)
-    columns.pop(columns.index('jobs'))
-    pi_score_df = pi_score_df[['jobs'] + columns]
-    pi_score_df = pi_score_df.sort_values(by='iptm',ascending=False)
-    
-    pi_score_df.to_csv(os.path.join(FLAGS.output_dir,"predictions_with_good_interpae.csv"),index=False)
+    if len(good_jobs) > 0:
+        other_measurements_df=pd.DataFrame.from_dict({
+            "jobs":good_jobs,
+            "iptm_ptm":iptm_ptm,
+            "iptm":iptm,
+            "mpDockQ/pDockQ":mpDockq_scores
+        }) 
+        pi_score_df = run_and_summarise_pi_score(FLAGS.output_dir,good_jobs,FLAGS.surface_thres)
+        pi_score_df=pd.merge(pi_score_df,other_measurements_df,on="jobs")
+        columns = list(pi_score_df.columns.values)
+        columns.pop(columns.index('jobs'))
+        pi_score_df = pi_score_df[['jobs'] + columns]
+        pi_score_df = pi_score_df.sort_values(by='iptm',ascending=False)
+        
+        pi_score_df.to_csv(os.path.join(FLAGS.output_dir,"predictions_with_good_interpae.csv"),index=False)
     
+    else:
+        logging.info(f"Unfortunately, none of your protein models had at least one PAE on the interface below your cutoff value : {FLAGS.cutoff}.\n Please consider using a larger cutoff.")
 
 if __name__ =='__main__':
     app.run(main)
```

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/test_create_notebook.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/test_create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/analysis_pipeline/utils.py` & `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from configparser import Interpolation
 import IPython.display as display
 import ipywidgets as widgets
 import matplotlib.pyplot as plt
 import matplotlib.image as mpimg
 import os
+import re
 #from analysis_pipeline.af2hyde_mod import plot_predicted_alignment_error
 from af2plots.plotter import plotter
 
 
 def display_pae_plots(subdir,figsize=(50, 50)):
     """A function to display all the pae plots in the subdir"""
-    images = sorted([i for i in os.listdir(subdir) if ".png" in i])
+    pattern = r"ranked_(\d+)\.png"
+    images = sorted([i for i in os.listdir(subdir) if ".png" in i],
+                    key= lambda x: int(re.search(pattern,x).group(1)))
     if len(images) > 0:
         fig, axs = plt.subplots(1, len(images), figsize=figsize)
         for i in range(len(images)):
             img = plt.imread(os.path.join(subdir, images[i]))
             axs[i].imshow(img,interpolation="nearest")
             axs[i].axis("off")
         #plt.show()
```

### Comparing `alphapulldown-1.0.4/alphapulldown/create_custom_template_db.py` & `alphapulldown-2.0.0b1/alphapulldown/utils/create_custom_template_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 Removes steric clashes and low pLDDT regions from the template files.
 Duplicates one template 4 times to increase impact on AF.
 Can be used as a standalone script.
 
 """
 
 import os
-import shutil
-import random
+import hashlib
+import base64
 import string
 from pathlib import Path
 from absl import logging, flags, app
-from alphapulldown.remove_clashes_low_plddt import MmcifChainFiltered
+from alphapulldown.utils.remove_clashes_low_plddt import MmcifChainFiltered
 from colabfold.batch import validate_and_fix_mmcif
 from alphafold.common.protein import _from_bio_structure, to_mmcif
 
 FLAGS = flags.FLAGS
 
 
 def save_seqres(code, chain, s, path, duplicate):
@@ -46,25 +46,35 @@
             logging.info(f'Saving SEQRES for chain {chain} to {fn} with code {entry.split()[0][1:]}!')
             logging.debug(entry)
             f.write(entry)
 
     return fn
 
 
+def generate_code(filename):
+    # Create a hash of the filename
+    hash_object = hashlib.sha256(filename.encode())
+    # Convert the hash to a base64 encoded string
+    base64_hash = base64.urlsafe_b64encode(hash_object.digest())
+    # Take the first 4 characters of the base64 encoded hash
+    code = base64_hash[:4].decode('utf-8')
+    return code
+
+
 def parse_code(template):
     # Check that the code is 4 letters
     code = Path(template).stem
     with open(template, "r") as f:
         for line in f:
             if line.startswith("_entry.id"):
                 code = line.split()[1]
 
-    # Generate a random 4-character code if needed
+    # Generate a deterministic 4-character code if needed
     if len(code) != 4:
-        code = ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(4))
+        code = generate_code(code)
 
     return code.lower()
 
 
 def create_dir_and_remove_files(dir_path, files_to_remove=[]):
     try:
         Path(dir_path).mkdir(parents=True)
@@ -97,26 +107,39 @@
     # Create empty obsolete.dat file
     with open(pdb_mmcif_dir / 'obsolete.dat', 'a'):
         pass
 
     create_dir_and_remove_files(seqres_dir, ['pdb_seqres.txt'])
 
 
+def copy_file_exclude_lines(starting_with, src, dst):
+    """
+    Copy contents from src to dst excluding lines that start with `starting_with`.
+
+    o starting_with: A string that, if a line starts with it, the line will be excluded.
+    o src: Source file path.
+    o dst: Destination file path.
+    """
+    with open(src, 'r') as infile, open(dst, 'w') as outfile:
+        for line in infile:
+            if not line.startswith(starting_with):
+                outfile.write(line)
+
 def _prepare_template(template, code, chain_id, mmcif_dir, seqres_dir, templates_dir,
                       threshold_clashes, hb_allowance, plddt_threshold, number_of_templates):
     """
     Process and prepare each template.
     """
     duplicate = number_of_templates == 1
     new_template = templates_dir / Path(code + Path(template).suffix)
-    shutil.copyfile(template, new_template)
+    copy_file_exclude_lines('HETATM', template, new_template)
     logging.info(f"Processing template: {new_template}  Chain {chain_id}")
 
     # Convert to (our) mmcif object
-    mmcif_obj = MmcifChainFiltered(template, code, chain_id)
+    mmcif_obj = MmcifChainFiltered(new_template, code, chain_id)
     # Determine the full sequence
     seqres = mmcif_obj.sequence_seqres if mmcif_obj.sequence_seqres else mmcif_obj.sequence_atom
     sqrres_path = save_seqres(code, chain_id, seqres, seqres_dir, duplicate)
     logging.info(f"SEQRES saved to {sqrres_path}!")
 
     # Remove clashes and low pLDDT regions for each template
     mmcif_obj.remove_clashes(threshold_clashes, hb_allowance)
```

### Comparing `alphapulldown-1.0.4/alphapulldown/create_individual_features_with_templates.py` & `alphapulldown-2.0.0b1/alphapulldown/scripts/create_individual_features.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,261 +1,372 @@
 #!/usr/bin/env python3
+# coding: utf-8
+# Create features for AlphaFold from fasta file(s) or a csv file with descriptions for multimeric templates
+# #
 
-# create_individual_features using custom multimeric templates
-#
-
-from alphapulldown.objects import MonomericObject
-from alphapulldown.utils import create_uniprot_runner, get_run_alphafold, convert_fasta_description_to_protein_name
-from alphapulldown.create_custom_template_db import create_db
-from alphafold.data.pipeline import DataPipeline
-from alphafold.data.tools import hmmsearch
-from alphafold.data import templates
-from absl import logging, app
 import os
+import pickle
 import sys
-from pathlib import Path
 import tempfile
-import csv
-from create_individual_features import create_and_save_monomer_objects, iter_seqs
+from datetime import datetime
+from pathlib import Path
+
+from absl import logging, app
+from alphafold.data import templates
+from alphafold.data.pipeline import DataPipeline
+from alphafold.data.tools import hmmsearch, hhsearch
+from colabfold.utils import DEFAULT_API_SERVER
 
+from alphapulldown.utils.create_custom_template_db import create_db
+from alphapulldown.objects import MonomericObject
+from alphapulldown.utils.file_handling import iter_seqs,parse_csv_file
+from alphapulldown.utils.modelling_setup import get_run_alphafold,create_uniprot_runner
+from alphapulldown.utils import save_meta_data
 
+# Initialize and define flags
 run_af = get_run_alphafold()
 flags = run_af.flags
 
-flags.DEFINE_integer("job_index", None, "index of job in the description file, starting from 1")
+# All flags
+flags.DEFINE_bool("use_mmseqs2", False,
+                  "Use mmseqs2 remotely or not. 'true' or 'false', default is 'false'")
+flags.DEFINE_bool("save_msa_files", False, "Save MSA output or not")
+flags.DEFINE_bool("skip_existing", False,
+                  "Skip existing monomer feature pickles or not")
+flags.DEFINE_string("new_uniclust_dir", None,
+                    "Directory where new version of uniclust is stored")
+flags.DEFINE_integer(
+    "seq_index", None, "Index of sequence in the fasta file, starting from 1")
+
+flags.DEFINE_boolean("use_hhsearch", False,
+                     "Use hhsearch instead of hmmsearch when looking for structure template. Default is False")
+
+# Flags related to TrueMultimer
+flags.DEFINE_string("path_to_mmt", None,
+                    "Path to directory with multimeric template mmCIF files")
+flags.DEFINE_string("description_file", None,
+                    "Path to the text file with descriptions")
+flags.DEFINE_float("threshold_clashes", 1000,
+                   "Threshold for VDW overlap to identify clashes. The VDW overlap between two atoms is defined as "
+                   "the sum of their VDW radii minus the distance between their centers."
+                   "If the overlap exceeds this threshold, the two atoms are considered to be clashing."
+                   "A positive threshold is how far the VDW surfaces are allowed to interpenetrate before considering "
+                   "the atoms to be clashing."
+                   "(default: 1000, i.e. no threshold, for thresholding, use 0.6-0.9)")
+flags.DEFINE_float("hb_allowance", 0.4,
+                   "Additional allowance for hydrogen bonding (default: 0.4)")
+flags.DEFINE_float("plddt_threshold", 0,
+                   "Threshold for pLDDT score (default: 0)")
 
-flags.DEFINE_string("description_file", None, "Path to the text file with descriptions")
-
-flags.DEFINE_string("path_to_mmt", None, "Path to directory with multimeric template mmCIF files")
-
-flags.DEFINE_float("threshold_clashes", 1000, "Threshold for VDW overlap to identify clashes "
-                                             "(default: 1000, i.e. no threshold, for thresholding, use 0.9)")
+FLAGS = flags.FLAGS
 
-flags.DEFINE_float("hb_allowance", 0.4, "Allowance for hydrogen bonding (default: 0.4)")
+MAX_TEMPLATE_HITS = 20
 
-flags.DEFINE_float("plddt_threshold", 0, "Threshold for pLDDT score (default: 0)")
+flags_dict = FLAGS.flag_values_dict()
 
-FLAGS = flags.FLAGS
-MAX_TEMPLATE_HITS = 1000000  # make it large enough to get all templates
 
+def get_database_path(flag_value, default_subpath):
+    """
+    Retrieves the database path based on a flag value or a default subpath.
 
-def create_arguments(flags_dict, local_path_to_custom_template_db):
-    """Create arguments for alphafold.run()"""
-    global use_small_bfd
+    Args:
+    flag_value (str): The value of the flag specifying the database path.
+    default_subpath (str): The default subpath to use if the flag value is not set.
 
-    # Path to the Uniref30 database for use by HHblits.
-    FLAGS.uniref30_database_path = FLAGS.uniref30_database_path or os.path.join(
-        FLAGS.data_dir, "uniref30", "UniRef30_2021_03"
-    )
-    flags_dict.update({"uniref30_database_path": FLAGS.uniref30_database_path})
+    Returns:
+    str: The final path to the database.
+    """
+    return flag_value or os.path.join(FLAGS.data_dir, default_subpath)
 
-    # Path to the Uniref90 database for use by JackHMMER.
-    FLAGS.uniref90_database_path = FLAGS.uniref90_database_path or os.path.join(
-        FLAGS.data_dir, "uniref90", "uniref90.fasta"
-    )
-    flags_dict.update({"uniref90_database_path": FLAGS.uniref90_database_path})
 
-    # Path to the MGnify database for use by JackHMMER.
-    FLAGS.mgnify_database_path = FLAGS.mgnify_database_path or os.path.join(
-        FLAGS.data_dir, "mgnify", "mgy_clusters_2022_05.fa"
-    )
-    flags_dict.update({"mgnify_database_path": FLAGS.mgnify_database_path})
-
-    # Path to the BFD database for use by HHblits.
-    FLAGS.bfd_database_path = FLAGS.bfd_database_path or os.path.join(
-        FLAGS.data_dir,
-        "bfd",
-        "bfd_metaclust_clu_complete_id30_c90_final_seq.sorted_opt",
-    )
-    flags_dict.update({"bfd_database_path": FLAGS.bfd_database_path})
+def create_arguments(local_path_to_custom_template_db=None):
+    """
+    Updates the (global) flags dictionary with paths to various databases required for AlphaFold. If a local path to a
+    custom template database is provided, pdb-related paths are set to this local database.
 
-    # Path to the Small BFD database for use by JackHMMER.
-    FLAGS.small_bfd_database_path = FLAGS.small_bfd_database_path or os.path.join(
-        FLAGS.data_dir, "small_bfd", "bfd-first_non_consensus_sequences.fasta"
-    )
-    flags_dict.update({"small_bfd_database_path": FLAGS.small_bfd_database_path})
+    Args:
+    local_path_to_custom_template_db (str, optional): Path to a local custom template database. Defaults to None.
+    """
+    global use_small_bfd
 
-    # Path to pdb70 database
-    FLAGS.pdb70_database_path = FLAGS.pdb70_database_path or os.path.join(FLAGS.data_dir, "pdb70", "pdb70")
-    flags_dict.update({"pdb70_database_path": FLAGS.pdb70_database_path})
+    FLAGS.uniref30_database_path = get_database_path(FLAGS.uniref30_database_path,
+                                                     "uniref30/UniRef30_2023_02")
+    FLAGS.uniref90_database_path = get_database_path(FLAGS.uniref90_database_path,
+                                                     "uniref90/uniref90.fasta")
+    FLAGS.mgnify_database_path = get_database_path(FLAGS.mgnify_database_path,
+                                                   "mgnify/mgy_clusters_2022_05.fa")
+    FLAGS.bfd_database_path = get_database_path(FLAGS.bfd_database_path,
+                                                "bfd/bfd_metaclust_clu_complete_id30_c90_final_seq.sorted_opt")
+    FLAGS.small_bfd_database_path = get_database_path(FLAGS.small_bfd_database_path,
+                                                      "small_bfd/bfd-first_non_consensus_sequences.fasta")
+    FLAGS.pdb70_database_path = get_database_path(
+        FLAGS.pdb70_database_path, "pdb70/pdb70")
 
-    use_small_bfd= FLAGS.db_preset == "reduced_dbs"
+    use_small_bfd = FLAGS.db_preset == "reduced_dbs"
     flags_dict.update({"use_small_bfd": use_small_bfd})
 
     # Update pdb related flags
-    FLAGS.pdb_seqres_database_path = os.path.join(local_path_to_custom_template_db, "pdb_seqres", "pdb_seqres.txt")
-    flags_dict.update({"pdb_seqres_database_path": FLAGS.pdb_seqres_database_path})
-    FLAGS.template_mmcif_dir = os.path.join(local_path_to_custom_template_db, "pdb_mmcif", "mmcif_files")
-    flags_dict.update({"template_mmcif_dir": FLAGS.template_mmcif_dir})
-    FLAGS.obsolete_pdbs_path = os.path.join(local_path_to_custom_template_db, "pdb_mmcif", "obsolete.dat")
-    flags_dict.update({"obsolete_pdbs_path": FLAGS.obsolete_pdbs_path})
+    if local_path_to_custom_template_db:
+        FLAGS.pdb_seqres_database_path = os.path.join(
+            local_path_to_custom_template_db, "pdb_seqres", "pdb_seqres.txt")
+        flags_dict.update(
+            {"pdb_seqres_database_path": FLAGS.pdb_seqres_database_path})
+        FLAGS.template_mmcif_dir = os.path.join(
+            local_path_to_custom_template_db, "pdb_mmcif", "mmcif_files")
+        flags_dict.update({"template_mmcif_dir": FLAGS.template_mmcif_dir})
+        FLAGS.obsolete_pdbs_path = os.path.join(
+            local_path_to_custom_template_db, "pdb_mmcif", "obsolete.dat")
+        flags_dict.update({"obsolete_pdbs_path": FLAGS.obsolete_pdbs_path})
+    else:
+        FLAGS.pdb_seqres_database_path = get_database_path(
+            FLAGS.pdb_seqres_database_path, "pdb_seqres/pdb_seqres.txt")
+        flags_dict.update(
+            {"pdb_seqres_database_path": FLAGS.pdb_seqres_database_path})
+        FLAGS.template_mmcif_dir = get_database_path(
+            FLAGS.template_mmcif_dir, "pdb_mmcif/mmcif_files")
+        flags_dict.update({"template_mmcif_dir": FLAGS.template_mmcif_dir})
+        FLAGS.obsolete_pdbs_path = get_database_path(
+            FLAGS.obsolete_pdbs_path, "pdb_mmcif/obsolete.dat")
+        flags_dict.update({"obsolete_pdbs_path": FLAGS.obsolete_pdbs_path})
 
 
-def create_custom_db(temp_dir, protein, templates, chains):
-    # Create custom template database
+def create_custom_db(temp_dir, protein, template_paths, chains):
+    """
+    Creates a custom template database for a specific protein using given templates and chains.
+
+    Args:
+    temp_dir (str): The temporary directory to store the custom database.
+    protein (str): The name of the protein for which the database is created.
+    templates (list): A list of template file paths.
+    chains (list): A list of chain identifiers corresponding to the templates.
+
+    Returns:
+    Path: The path to the created custom template database.
+    """
     threashold_clashes = FLAGS.threshold_clashes
     hb_allowance = FLAGS.hb_allowance
     plddt_threshold = FLAGS.plddt_threshold
-    #local_path_to_custom_template_db = Path(".") / "custom_template_db" / protein # DEBUG
-    local_path_to_custom_template_db = Path(temp_dir) / "custom_template_db" / protein
+    # local_path_to_custom_template_db = Path(".") / "custom_template_db" / protein # DEBUG
+    local_path_to_custom_template_db = Path(
+        temp_dir) / "custom_template_db" / protein
     logging.info(f"Path to local database: {local_path_to_custom_template_db}")
-    create_db(local_path_to_custom_template_db, templates, chains, threashold_clashes, hb_allowance, plddt_threshold)
+    create_db(
+        local_path_to_custom_template_db, template_paths, chains, threashold_clashes, hb_allowance, plddt_threshold
+    )
 
     return local_path_to_custom_template_db
 
 
-
-def parse_csv_file(csv_path, fasta_paths, mmt_dir):
+def create_pipeline():
     """
-    o csv_path: Path to the text file with descriptions
-        features.csv: A coma-separated file with three columns: PROTEIN name, PDB/CIF template, chain ID.
-    o fasta_paths: path to fasta file(s)
-    o mmt_dir: Path to directory with multimeric template mmCIF files
+    Creates and returns a data pipeline for AlphaFold, configured with necessary binary paths and database paths.
 
     Returns:
-        a list of dictionaries with the following structure:
-    [{"protein": protein_name, "sequence" :sequence", templates": [pdb_files], "chains": [chain_id]}, ...]}]
+    DataPipeline: An instance of the AlphaFold DataPipeline configured with necessary paths.
     """
-    protein_names = {}
-    # Check that fasta files exist
-    for fasta_path in fasta_paths:
-        logging.info(f"Parsing {fasta_path}...")
-        if not os.path.isfile(fasta_path):
-            raise FileNotFoundError(f"Fasta file {fasta_path} does not exist. Please check your input file.")
-    # Parse all protein names from fasta files
-    for curr_seq, curr_desc in iter_seqs(fasta_paths):
-        if curr_desc in protein_names.keys():
-            continue
-        protein_names[curr_desc] = curr_seq
-
-    # Parse csv file
-    parsed_dict = {}
-    with open(csv_path, newline="") as csvfile:
-        csvreader = csv.reader(csvfile)
-        for row in csvreader:
-            # skip empty lines
-            if not row:
-                continue
-            if len(row) == 3:
-                protein, template, chain = [item.strip() for item in row]
-                # Remove special symbols from protein name
-                protein = convert_fasta_description_to_protein_name(protein)
-                if protein not in protein_names:
-                    raise Exception(f"Protein {protein} from description.csv is not found in the fasta file(s)."
-                                    f"List of proteins in fasta file(s): {protein_names}")
-                if protein not in parsed_dict:
-                    parsed_dict[protein] = {
-                        "protein": protein,
-                        "templates": [],
-                        "chains": [],
-                        "sequence": None,
-                    }
-                parsed_dict[protein]["sequence"] = protein_names[protein]
-                parsed_dict[protein]["templates"].append(os.path.join(mmt_dir, template))
-                parsed_dict[protein]["chains"].append(chain)
-            else:
-                logging.error(f"Invalid line found in the file {csv_path}: {row}")
-                sys.exit()
-
-    return list(parsed_dict.values())
-
-
-def create_pipeline():
+    if FLAGS.use_hhsearch:
+        logging.info("Will use hhsearch looking for templates")
+        template_searcher = hhsearch.HHSearch(
+        binary_path=FLAGS.hhsearch_binary_path,
+        databases=[FLAGS.pdb70_database_path]
+        )
+        template_featuriser = templates.HhsearchHitFeaturizer(
+        mmcif_dir=FLAGS.template_mmcif_dir,
+        max_template_date=FLAGS.max_template_date,
+        max_hits=MAX_TEMPLATE_HITS,
+        kalign_binary_path=FLAGS.kalign_binary_path,
+        release_dates_path=None,
+        obsolete_pdbs_path=FLAGS.obsolete_pdbs_path
+        )
+    else:
+        logging.info("Will use hmmsearch looking for templates")
+        template_featuriser = templates.HmmsearchHitFeaturizer(
+            mmcif_dir=FLAGS.template_mmcif_dir,
+            max_template_date=FLAGS.max_template_date,
+            max_hits=MAX_TEMPLATE_HITS,
+            kalign_binary_path=FLAGS.kalign_binary_path,
+            obsolete_pdbs_path=FLAGS.obsolete_pdbs_path,
+            release_dates_path=None,
+        )
+        template_searcher = hmmsearch.Hmmsearch(
+            binary_path=FLAGS.hmmsearch_binary_path,
+            hmmbuild_binary_path=FLAGS.hmmbuild_binary_path,
+            database_path=FLAGS.pdb_seqres_database_path,
+        )
     monomer_data_pipeline = DataPipeline(
         jackhmmer_binary_path=FLAGS.jackhmmer_binary_path,
         hhblits_binary_path=FLAGS.hhblits_binary_path,
         uniref90_database_path=FLAGS.uniref90_database_path,
         mgnify_database_path=FLAGS.mgnify_database_path,
         bfd_database_path=FLAGS.bfd_database_path,
         uniref30_database_path=FLAGS.uniref30_database_path,
         small_bfd_database_path=FLAGS.small_bfd_database_path,
         use_small_bfd=use_small_bfd,
         use_precomputed_msas=FLAGS.use_precomputed_msas,
-        template_searcher=hmmsearch.Hmmsearch(
-            binary_path=FLAGS.hmmsearch_binary_path,
-            hmmbuild_binary_path=FLAGS.hmmbuild_binary_path,
-            database_path=FLAGS.pdb_seqres_database_path,
-        ),
-        template_featurizer=templates.HmmsearchHitFeaturizer(
-            mmcif_dir=FLAGS.template_mmcif_dir,
-            max_template_date=FLAGS.max_template_date,
-            max_hits=MAX_TEMPLATE_HITS,
-            kalign_binary_path=FLAGS.kalign_binary_path,
-            obsolete_pdbs_path=FLAGS.obsolete_pdbs_path,
-            release_dates_path=None,
-        ),
+        template_searcher=template_searcher,
+        template_featurizer=template_featuriser
     )
     return monomer_data_pipeline
 
 
+def create_and_save_monomer_objects(monomer, pipeline):
+    """
+    Processes a MonomericObject to create and save its features. Skips processing if the feature file already exists
+    and skipping is enabled.
+
+    Args:
+    monomer (MonomericObject): The monomeric object to process.
+    pipeline (DataPipeline): The data pipeline object for feature creation.
+    """
+    pickle_path = os.path.join(FLAGS.output_dir, f"{monomer.description}.pkl")
+
+    # Check if we should skip existing files
+    if FLAGS.skip_existing and os.path.exists(pickle_path):
+        logging.info(
+            f"Feature file for {monomer.description} already exists. Skipping...")
+        return
+
+    # Save metadata
+    metadata_output_path = os.path.join(FLAGS.output_dir,
+                                        f"{monomer.description}_feature_metadata_{datetime.date(datetime.now())}.json")
+    with save_meta_data.output_meta_file(metadata_output_path) as meta_data_outfile:
+        save_meta_data.save_meta_data(flags_dict, meta_data_outfile)
+
+    # Create features
+    if FLAGS.use_mmseqs2:
+        logging.info("Running MMseqs2 for feature generation...")
+        monomer.make_mmseq_features(
+            DEFAULT_API_SERVER=DEFAULT_API_SERVER,
+            output_dir=FLAGS.output_dir
+        )
+    else:
+        monomer.make_features(
+            pipeline=pipeline,
+            output_dir=FLAGS.output_dir,
+            use_precomputed_msa=FLAGS.use_precomputed_msas,
+            save_msa=FLAGS.save_msa_files,
+        )
+
+    # Save the processed monomer object
+    with open(pickle_path, "wb") as pickle_file:
+        pickle.dump(monomer, pickle_file)
+
+    # Optional: Clear monomer from memory if necessary
+    del monomer
+
+
+def check_template_date_and_uniprot():
+    """
+    Checks if the max_template_date is provided and updates the flags dictionary with the path to the Uniprot database.
+    Exits the script if max_template_date is not provided or if the Uniprot database file is not found.
+    """
+    if not FLAGS.max_template_date:
+        logging.info(
+            "You have not provided a max_template_date. Please specify a date and run again.")
+        sys.exit()
+    uniprot_database_path = os.path.join(
+        FLAGS.data_dir, "uniprot/uniprot.fasta")
+    flags_dict.update({"uniprot_database_path": uniprot_database_path})
+    if not os.path.isfile(uniprot_database_path):
+        logging.info(
+            f"Failed to find uniprot.fasta under {uniprot_database_path}."
+            f" Please make sure your data_dir has been configured correctly.")
+        sys.exit()
+
+
+def process_sequences_individual_mode():
+    """
+    Processes individual sequences specified in the fasta files. For each sequence, it creates a MonomericObject,
+    processes it, and saves its features. Skips processing if the sequence index does not match the seq_index flag.
+
+    """
+    create_arguments()
+    uniprot_runner = None if FLAGS.use_mmseqs2 else create_uniprot_runner(FLAGS.jackhmmer_binary_path,
+                                                                          FLAGS.uniref90_database_path)
+    pipeline = None if FLAGS.use_mmseqs2 else create_pipeline()
+    seq_idx = 0
+    for curr_seq, curr_desc in iter_seqs(FLAGS.fasta_paths):
+        seq_idx += 1
+        if FLAGS.seq_index is None or (FLAGS.seq_index == seq_idx):
+            if curr_desc and not curr_desc.isspace():
+                curr_monomer = MonomericObject(curr_desc, curr_seq)
+                curr_monomer.uniprot_runner = uniprot_runner
+                create_and_save_monomer_objects(curr_monomer, pipeline)
+
+
+def process_sequences_multimeric_mode():
+    """
+    Processes sequences in multimeric mode using descriptions from a CSV file. For each entry in the CSV file,
+    it processes the corresponding sequence if it matches the seq_index flag.
+    """
+    fasta_paths = FLAGS.fasta_paths
+    feats = parse_csv_file(FLAGS.description_file,
+                           fasta_paths, FLAGS.path_to_mmt)
+    logging.info(f"seq_index: {FLAGS.seq_index}, feats: {feats}")
+
+    for idx, feat in enumerate(feats, 1):
+        if FLAGS.seq_index is None or (FLAGS.seq_index == idx):
+            process_multimeric_features(feat, idx)
+
+
+def process_multimeric_features(feat, idx):
+    """
+    Processes a multimeric feature from a provided feature dictionary. It checks for the existence of template files
+    and creates a custom database for the specified protein. It then processes the protein and saves its features.
+
+    Args:
+    feat (dict): A dictionary containing protein information and its corresponding templates and chains.
+    idx (int): The index of the current protein being processed.
+    """
+    for temp_path in feat["templates"]:
+        if not os.path.isfile(temp_path):
+            logging.error(f"Template file {temp_path} does not exist.")
+            raise FileNotFoundError(
+                f"Template file {temp_path} does not exist.")
+
+    protein = feat["protein"]
+    chains = feat["chains"]
+    template_paths = feat["templates"]
+    logging.info(
+        f"Processing {protein}: templates: {templates}, chains: {chains}")
+
+    with tempfile.TemporaryDirectory() as temp_dir:
+        local_path_to_custom_db = create_custom_db(
+            temp_dir, protein, template_paths, chains)
+        create_arguments(local_path_to_custom_db)
+
+        flags_dict.update({f"protein_{idx}": feat['protein'], f"multimeric_templates_{idx}": template_paths,
+                           f"multimeric_chains_{idx}": feat['chains']})
+
+        if not FLAGS.use_mmseqs2:
+            uniprot_runner = create_uniprot_runner(
+                FLAGS.jackhmmer_binary_path, FLAGS.uniref90_database_path)
+        else:
+            uniprot_runner = None
+        pipeline = create_pipeline()
+        curr_monomer = MonomericObject(feat['protein'], feat['sequence'])
+        curr_monomer.uniprot_runner = uniprot_runner
+        create_and_save_monomer_objects(curr_monomer, pipeline)
+
+
 def main(argv):
+    del argv  # Unused.
     try:
         Path(FLAGS.output_dir).mkdir(parents=True, exist_ok=True)
     except FileExistsError:
-        logging.info("Multiple processes are trying to create the same folder now.")
-
-    flags_dict = FLAGS.flag_values_dict()
-    fasta_paths = flags_dict["fasta_paths"]
-    feats = parse_csv_file(FLAGS.description_file, fasta_paths, FLAGS.path_to_mmt)
-    logging.info(f"job_index: {FLAGS.job_index} feats: {feats}")
-    for idx, feat in enumerate(feats, 1):
-        if (FLAGS.job_index is None) or (FLAGS.job_index == idx):
-            for temp in feat["templates"]:
-                if not os.path.isfile:
-                    logging.error(f"Template file {temp} does not exist. Please check your input file.")
-                    sys.exit()
-            protein = feat["protein"]
-            chains = feat["chains"]
-            templates = feat["templates"]
-            logging.info(f"Processing {protein}: templates: {templates} chains: {chains}")
-            # For each protein, create a temp dir
-            with tempfile.TemporaryDirectory() as temp_dir:
-                local_path_to_custom_db = create_custom_db(temp_dir, protein, templates, chains)
-                create_arguments(flags_dict, local_path_to_custom_db)
-
-                # Update flags_dict to store data about templates
-                flags_dict.update({f"protein_{idx}": feat['protein']})
-                flags_dict.update({f"multimeric_templates_{idx}": feat['templates']})
-                flags_dict.update({f"multimeric_chains_{idx}": feat['chains']})
-
-                if not FLAGS.use_mmseqs2:
-                    if not FLAGS.max_template_date:
-                        logging.info("You have not provided a max_template_date. Please specify a date and run again.")
-                        sys.exit()
-                    else:
-                        pipeline = create_pipeline()
-                        uniprot_database_path = os.path.join(FLAGS.data_dir, "uniprot/uniprot.fasta")
-                        flags_dict.update({"uniprot_database_path": uniprot_database_path})
-                        if os.path.isfile(uniprot_database_path):
-                            uniprot_runner = create_uniprot_runner(FLAGS.jackhmmer_binary_path, uniprot_database_path)
-                        else:
-                            logging.info(
-                                f"Failed to find uniprot.fasta under {uniprot_database_path}."
-                                "Please make sure your data_dir has been configured correctly."
-                            )
-                            sys.exit()
-                else:
-                    pipeline = create_pipeline()
-                    uniprot_runner = None
-                    flags_dict = FLAGS.flag_values_dict()
-                curr_monomer = MonomericObject(feat['protein'], feat['sequence'])
-                curr_monomer.uniprot_runner = uniprot_runner
-                create_and_save_monomer_objects(
-                    curr_monomer,
-                    pipeline,
-                    flags_dict,
-                    use_mmseqs2=FLAGS.use_mmseqs2,
-                )
+        logging.error(
+            "Multiple processes are trying to create the same folder now.")
+        pass
+    if not FLAGS.use_mmseqs2:
+        check_template_date_and_uniprot()
+
+    if not FLAGS.path_to_mmt:
+        process_sequences_individual_mode()
+    else:
+        process_sequences_multimeric_mode()
 
 
 if __name__ == "__main__":
     flags.mark_flags_as_required(
-        [
-            "description_file",
-            "fasta_paths",
-            "path_to_mmt",
-            "output_dir",
-            "max_template_date",
-            "data_dir",
-        ]
+        ["fasta_paths", "output_dir", "max_template_date", "data_dir"]
     )
     app.run(main)
```

### Comparing `alphapulldown-1.0.4/alphapulldown/generate_crosslink_pickle.py` & `alphapulldown-2.0.0b1/alphapulldown/scripts/generate_crosslink_pickle.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/objects.py` & `alphapulldown-2.0.0b1/alphapulldown/objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-# Author Dingquan Yu
-# scripts to create objects (e.g. monomeric object, multimeric objects)
-#
-# #
-import logging
+""" Create monomeric or multimeric objects with corresponding import features for the modelling backends
+
+    Copyright (c) 2024 European Molecular Biology Laboratory
+
+    Author: Dingquan Yu <dingquan.yu@embl-hamburg.de>
+"""
+from absl import logging
+logging.set_verbosity(logging.INFO)
 import tempfile
 import os
-import contextlib
+import subprocess
 import numpy as np
+from alphafold.data.tools import jackhmmer
 from alphafold.data import parsers
 from alphafold.data import pipeline_multimer
 from alphafold.data import pipeline
 from alphafold.data import msa_pairing
 from alphafold.data import feature_processing
-from alphafold.data import templates
 from pathlib import Path as plPath
-from alphafold.data.tools import hhsearch
+from typing import List, Dict
 from colabfold.batch import unserialize_msa, get_msa_and_templates, msa_to_str, build_monomer_feature
-
-
-@contextlib.contextmanager
-def temp_fasta_file(sequence_str):
-    """function that create temp file"""
-    with tempfile.NamedTemporaryFile("w", suffix=".fasta") as fasta_file:
-        fasta_file.write(sequence_str)
-        fasta_file.seek(0)
-        yield fasta_file.name
-
+from alphapulldown.utils.multimeric_template_utils import (extract_multimeric_template_features_for_single_chain,
+                                                     prepare_multimeric_template_meta_info)
+from alphapulldown.utils.file_handling import temp_fasta_file
 
 class MonomericObject:
     """
     monomeric objects
 
     Args
     description: description of the protein. By default is everything after the ">" symbol
@@ -48,218 +44,208 @@
     def uniprot_runner(self):
         return self._uniprot_runner
 
     @uniprot_runner.setter
     def uniprot_runner(self, uniprot_runner):
         self._uniprot_runner = uniprot_runner
 
+    @staticmethod
+    def zip_msa_files(msa_output_path: str):
+        """
+        A static method that zip individual msa files within the given msa_output_path folder
+        """
+        def zip_individual_file(msa_file: plPath):
+            assert os.path.exists(msa_file)
+            cmd = f"gzip {msa_file}"
+            _ = subprocess.run(cmd, shell=True, capture_output=True, text=True)
+
+        msa_file_endings = ['.a3m', '.fasta', '.sto', '.hmm']
+        msa_files = [i for i in plPath(
+            msa_output_path).iterdir() if i.suffix in msa_file_endings]
+        if len(msa_files) > 0:
+            for msa_file in msa_files:
+                zip_individual_file(msa_file)
+
+    @staticmethod
+    def unzip_msa_files(msa_output_path: str):
+        """
+        A static method that unzip msa files in a folder if they exist
+        """
+        def unzip_individual_file(msa_file: plPath):
+            assert os.path.exists(msa_file)
+            cmd = f"gunzip {msa_file}"
+            _ = subprocess.run(cmd, shell=True, capture_output=True, text=True)
+
+        zipped_files = [i for i in plPath(
+            msa_output_path).iterdir() if i.suffix == '.gz']
+        if len(zipped_files) > 0:
+            for zipped_file in zipped_files:
+                unzip_individual_file(zipped_file)
+            return True  # means it has used zipped msa files
+        else:
+            return False
+
+    @staticmethod
+    def remove_msa_files(msa_output_path: str):
+        """A method that remove msa files is save_msa is set to False"""
+        msa_file_endings = ['.a3m', '.fasta', '.sto', '.hmm']
+        msa_files = [i for i in plPath(
+            msa_output_path).iterdir() if i.suffix in msa_file_endings]
+        if len(msa_files) > 0:
+            for msa_file in msa_files:
+                os.remove(msa_file)
+
     def all_seq_msa_features(
             self,
-            input_fasta_path,
-            uniprot_msa_runner,
-            save_msa,
-            output_dir=None,
-            use_precomuted_msa=False,
-    ):
+            input_fasta_path: str,
+            uniprot_msa_runner: jackhmmer.Jackhmmer,
+            output_dir: str = None,
+            use_precomputed_msa: bool = False
+    ) -> None:
         """Get MSA features for unclustered uniprot, for pairing later on."""
-        if not use_precomuted_msa:
-            if not save_msa:
-                with tempfile.TemporaryDirectory() as tempdir:
-                    logging.info("now going to run uniprot runner")
-                    result = pipeline.run_msa_tool(
-                        uniprot_msa_runner,
-                        input_fasta_path,
-                        f"{tempdir}/uniprot.sto",
-                        "sto",
-                        use_precomuted_msa,
-                    )
-            elif save_msa and (output_dir is not None):
-                logging.info(
-                    f"now going to run uniprot runner and save uniprot alignment in {output_dir}"
-                )
-                result = pipeline.run_msa_tool(
-                    uniprot_msa_runner,
-                    input_fasta_path,
-                    f"{output_dir}/uniprot.sto",
-                    "sto",
-                    use_precomuted_msa,
-                )
-        else:
-            result = pipeline.run_msa_tool(
-                uniprot_msa_runner,
-                input_fasta_path,
-                f"{output_dir}/uniprot.sto",
-                "sto",
-                use_precomuted_msa,
-            )
+
+        logging.info(
+            f"now going to run uniprot runner and save uniprot alignment in {output_dir}"
+        )
+        result = pipeline.run_msa_tool(
+            uniprot_msa_runner,
+            input_fasta_path,
+            f"{output_dir}/uniprot.sto",
+            "sto",
+            use_precomputed_msa,
+        )
+
         msa = parsers.parse_stockholm(result["sto"])
         msa = msa.truncate(max_seqs=50000)
         all_seq_features = pipeline.make_msa_features([msa])
         valid_feats = msa_pairing.MSA_FEATURES + (
             "msa_species_identifiers",
             "msa_uniprot_accession_identifiers",
         )
         feats = {
             f"{k}_all_seq": v for k, v in all_seq_features.items() if k in valid_feats
         }
         return feats
 
     def make_features(
-            self, pipeline, output_dir=None, use_precomputed_msa=False, save_msa=True
+            self, pipeline, output_dir: str,
+            use_precomputed_msa: bool = False,
+            save_msa: bool = True, compress_msa_files: bool = False
     ):
         """a method that make msa and template features"""
-        if not use_precomputed_msa:
-            if not save_msa:
-                """this means no msa files are going to be saved"""
-                logging.info("You have chosen not to save msa output files")
-                sequence_str = f">{self.description}\n{self.sequence}"
-                with temp_fasta_file(
-                        sequence_str
-                ) as fasta_file, tempfile.TemporaryDirectory() as tmpdirname:
-                    self.feature_dict = pipeline.process(
-                        input_fasta_path=fasta_file, msa_output_dir=tmpdirname
-                    )
-                    pairing_results = self.all_seq_msa_features(
-                        fasta_file, self._uniprot_runner, save_msa
-                    )
-                    self.feature_dict.update(pairing_results)
+        os.makedirs(os.path.join(output_dir, self.description), exist_ok=True)
 
-            else:
-                """this means no precomputed msa available and will save output msa files"""
-                msa_output_dir = os.path.join(output_dir, self.description)
-                sequence_str = f">{self.description}\n{self.sequence}"
-                logging.info("will save msa files in :{}".format(msa_output_dir))
-                plPath(msa_output_dir).mkdir(parents=True, exist_ok=True)
-                with temp_fasta_file(sequence_str) as fasta_file:
-                    self.feature_dict = pipeline.process(fasta_file, msa_output_dir)
-                    pairing_results = self.all_seq_msa_features(
-                        fasta_file, self._uniprot_runner, save_msa, msa_output_dir
-                    )
-                    self.feature_dict.update(pairing_results)
-        else:
-            """This means precomputed msa files are available"""
-            msa_output_dir = os.path.join(output_dir, self.description)
-            plPath(msa_output_dir).mkdir(parents=True, exist_ok=True)
-            logging.info(
-                "use precomputed msa. Searching for msa files in :{}".format(
-                    msa_output_dir
-                )
+        # firstly check if there are zipped msa files. unzip it if there is zipped msa files
+        using_zipped_msa_files = MonomericObject.unzip_msa_files(
+            os.path.join(output_dir, self.description))
+
+        # Then start creating msa features
+        msa_output_dir = os.path.join(output_dir, self.description)
+        sequence_str = f">{self.description}\n{self.sequence}"
+        logging.info(
+            "will save msa files in :{}".format(msa_output_dir))
+        plPath(msa_output_dir).mkdir(parents=True, exist_ok=True)
+        with temp_fasta_file(sequence_str) as fasta_file:
+            self.feature_dict = pipeline.process(
+                fasta_file, msa_output_dir)
+            pairing_results = self.all_seq_msa_features(
+                fasta_file, self._uniprot_runner, msa_output_dir, use_precomputed_msa
             )
-            sequence_str = f">{self.description}\n{self.sequence}"
-            with temp_fasta_file(sequence_str) as fasta_file:
-                self.feature_dict = pipeline.process(fasta_file, msa_output_dir)
-                pairing_results = self.all_seq_msa_features(
-                    fasta_file,
-                    self._uniprot_runner,
-                    save_msa,
-                    msa_output_dir,
-                    use_precomuted_msa=True,
-                )
-                self.feature_dict.update(pairing_results)
-
-    def mk_template(self, a3m_lines, 
-                    pipeline, query_sequence):
-        """
-        Overwrite ColabFold's original mk_template to incorporate max_template data argument
-        from the command line input. Use Hmmsearch instead of hhsearch to stay in lign 
-        withe AlphaPulldown's convention and new TrueMultimer updates
-        Modified from ColabFold: https://github.com/sokrypton/ColabFold
-
-        Args
-        template_path should be the same as FLAG.data_dir
-        """
-        template_featuriser = pipeline.template_featurizer
-        hmm_build_runner = pipeline.template_searcher.hmmbuild_runner
-        hmm_profile = hmm_build_runner.build_profile_from_a3m(a3m_lines)
-        query_result = pipeline.template_searcher.query_with_hmm(hmm_profile)
-        template_hits = pipeline.template_searcher.get_template_hits(query_result,query_sequence)
-        templates_result = template_featuriser.get_templates(
-            query_sequence=query_sequence, hits=template_hits
-        )
-        return dict(templates_result.features)
+            self.feature_dict.update(pairing_results)
 
+        # post processing
+        if (not save_msa) and (not use_precomputed_msa):
+            MonomericObject.remove_msa_files(msa_output_path=msa_output_dir)
+        elif (not save_msa) and use_precomputed_msa:
+            logging.warning("You chose not to save MSA files but still want to use precomputed MSA files thus the precomputed MSA files will NOT be removed.")     
+        if compress_msa_files:
+            MonomericObject.zip_msa_files(msa_output_dir)
+        if using_zipped_msa_files:
+            MonomericObject.zip_msa_files(
+                os.path.join(output_dir, self.description))
+            
     def make_mmseq_features(
-            self, DEFAULT_API_SERVER, 
-            pipeline=None, output_dir=None,
+            self, DEFAULT_API_SERVER,
+            output_dir=None,
+            compress_msa_files=False
     ):
         """
         A method to use mmseq_remote to calculate msa
         Modified from ColabFold: https://github.com/sokrypton/ColabFold
         """
-
+        # first check if there are zipped a3m files
+        os.makedirs(output_dir, exist_ok=True)
+        using_zipped_msa_files = MonomericObject.unzip_msa_files(
+            output_dir)
         logging.info("You chose to calculate MSA with mmseq2.\nPlease also cite: Mirdita M, Schütze K, Moriwaki Y, Heo L, Ovchinnikov S and Steinegger M. ColabFold: Making protein folding accessible to all. Nature Methods (2022) doi: 10.1038/s41592-022-01488-1")
-        msa_mode = "MMseqs2 (UniRef+Environmental)"
+        
+        msa_mode = "mmseqs2_uniref_env"
         keep_existing_results = True
         result_dir = output_dir
-        use_templates = False
+        use_templates = True
         result_zip = os.path.join(result_dir, self.description, ".result.zip")
         if keep_existing_results and plPath(result_zip).is_file():
             logging.info(f"Skipping {self.description} (result.zip)")
-
-        logging.info(f"looking for possible precomputed a3m at {os.path.join(result_dir, self.description + '.a3m')}")
-        try:
-            logging.info(f"input is {os.path.join(result_dir, self.description + '.a3m')}")
-            input_path = os.path.join(result_dir, self.description + '.a3m')
-            a3m_lines = [plPath(input_path).read_text()]
-            logging.info(f"Finished parsing the precalculated a3m_file\nNow will search for template")
-        except:
-            a3m_lines = None
-
-        if a3m_lines is not None:
-            (
-                unpaired_msa,
-                paired_msa,
-                query_seqs_unique,
-                query_seqs_cardinality,
-                template_features,
-            ) = unserialize_msa(a3m_lines, self.sequence)
-
-        else:
-            (
-                unpaired_msa,
-                paired_msa,
-                query_seqs_unique,
-                query_seqs_cardinality,
-                template_features,
-            ) = get_msa_and_templates(
-                jobname = '',
-                query_sequences=self.sequence,
-                a3m_lines = None,
-                result_dir=plPath(result_dir),
-                msa_mode=msa_mode,
-                use_templates=use_templates,
-                custom_template_path=None,
-                pair_mode="none",
-                host_url=DEFAULT_API_SERVER,
-                user_agent='alphapulldown'
-            )
-            msa = msa_to_str(
-                unpaired_msa, paired_msa, query_seqs_unique, query_seqs_cardinality
-            )
-            plPath(os.path.join(result_dir, self.description + ".a3m")).write_text(msa)
-            a3m_lines = [plPath(os.path.join(result_dir, self.description + ".a3m")).read_text()]
+        
+        (
+            unpaired_msa,
+            paired_msa,
+            query_seqs_unique,
+            query_seqs_cardinality,
+            template_features,
+        ) = get_msa_and_templates(
+            jobname=self.description,
+            query_sequences=self.sequence,
+            a3m_lines=None,
+            result_dir=plPath(result_dir),
+            msa_mode=msa_mode,
+            use_templates=use_templates,
+            custom_template_path=None,
+            pair_mode="none",
+            host_url=DEFAULT_API_SERVER,
+            user_agent='alphapulldown'
+        )
+        msa = msa_to_str(
+            unpaired_msa, paired_msa, query_seqs_unique, query_seqs_cardinality
+        )
+        plPath(os.path.join(result_dir, self.description + ".a3m")
+                ).write_text(msa)
+        a3m_lines = [
+            plPath(os.path.join(result_dir, self.description + ".a3m")).read_text()]
+
+        if compress_msa_files:
+            MonomericObject.zip_msa_files(
+                os.path.join(result_dir, self.description))
         # unserialize_msa was from colabfold.batch and originally will only create mock template features
-        # below will search against pdb70 database using hhsearch and create real template features
-        logging.info("will search for templates in local template database")
-        a3m_lines[0] = "\n".join([line for line in a3m_lines[0].splitlines() if not line.startswith("#")])
-        template_features = self.mk_template(a3m_lines[0],
-                                              pipeline, query_sequence=self.sequence)
-        self.feature_dict = build_monomer_feature(self.sequence, unpaired_msa[0], 
-                                                  template_features)
+        a3m_lines[0] = "\n".join(
+            [line for line in a3m_lines[0].splitlines() if not line.startswith("#")])
+        self.feature_dict = build_monomer_feature(self.sequence, unpaired_msa[0],
+                                                  template_features[0])
 
         # update feature_dict with
         valid_feats = msa_pairing.MSA_FEATURES + (
             "msa_species_identifiers",
             "msa_uniprot_accession_identifiers",
         )
         feats = {
             f"{k}_all_seq": v for k, v in self.feature_dict.items() if k in valid_feats
         }
+
+        # add template_confidence_scores if it does not exist 
+        template_confidence_scores = self.feature_dict.get('template_confidence_scores', None)
+        if template_confidence_scores is None:
+            self.feature_dict.update(
+                {'template_confidence_scores': np.array([[1] * len(self.sequence)])}
+            )
         self.feature_dict.update(feats)
 
+        if using_zipped_msa_files:
+            MonomericObject.zip_msa_files(
+                output_dir)
+
 
 class ChoppedObject(MonomericObject):
     """chopped monomeric objects"""
 
     def __init__(self, description, sequence, feature_dict, regions) -> None:
         super().__init__(description, sequence)
         self.feature_dict = feature_dict
@@ -282,23 +268,25 @@
         msa_feature is actually the full feature_dict
         """
         start_point = start_point - 1
         length = end_point - start_point
         new_seq_length = np.array([length] * length)
         new_aa_type = msa_feature["aatype"][start_point:end_point, :]
         new_between_segment_residue = msa_feature["between_segment_residues"][
-                                      start_point:end_point
-                                      ]
+            start_point:end_point
+        ]
         new_domain_name = msa_feature["domain_name"]
         new_residue_index = msa_feature["residue_index"][start_point:end_point]
-        new_sequence = np.array([msa_feature["sequence"][0][start_point:end_point]])
-        new_deletion_mtx = msa_feature["deletion_matrix_int"][:, start_point:end_point]
+        new_sequence = np.array(
+            [msa_feature["sequence"][0][start_point:end_point]])
+        new_deletion_mtx = msa_feature["deletion_matrix_int"][:,
+                                                              start_point:end_point]
         new_deletion_mtx_all_seq = msa_feature["deletion_matrix_int_all_seq"][
-                                   :, start_point:end_point
-                                   ]
+            :, start_point:end_point
+        ]
         new_msa = msa_feature["msa"][:, start_point:end_point]
         new_msa_all_seq = msa_feature["msa_all_seq"][:, start_point:end_point]
         new_num_alignments = np.array([msa_feature["msa"].shape[0]] * length)
         new_uniprot_species = msa_feature["msa_species_identifiers"]
         new_uniprot_species_all_seq = msa_feature["msa_species_identifiers_all_seq"]
 
         new_msa_feature = {
@@ -326,22 +314,22 @@
         prepare template  features
 
         Args:
         template_feature is actually the full feature_dict
         """
         start_point = start_point - 1
         new_template_aatype = template_feature["template_aatype"][
-                              :, start_point:end_point, :
-                              ]
+            :, start_point:end_point, :
+        ]
         new_template_all_atom_masks = template_feature["template_all_atom_masks"][
-                                      :, start_point:end_point, :
-                                      ]
+            :, start_point:end_point, :
+        ]
         new_template_all_atom_positions = template_feature[
-                                              "template_all_atom_positions"
-                                          ][:, start_point:end_point, :, :]
+            "template_all_atom_positions"
+        ][:, start_point:end_point, :, :]
         new_template_domain_names = template_feature["template_domain_names"]
         new_template_sequence = template_feature["template_sequence"]
         new_template_sum_probs = template_feature["template_sum_probs"]
 
         new_template_feature = {
             "template_aatype": new_template_aatype,
             "template_all_atom_masks": new_template_all_atom_masks,
@@ -435,51 +423,65 @@
 class MultimericObject:
     """
     multimeric objects with features for multimer
 
     Args
     index: assign a unique index ranging from 0 just to identify different multimer jobs
     interactors: individual interactors that are to be concatenated
+    pair_msa: boolean, tells the programme whether to pair MSA or not
+    multimeric_mode: boolean, tells the programme whether use multimeric templates or not
+    multimeric_template_meta_data: a csv with the format {"monomer_A":{"xxx.cif":"chainID"},"monomer_B":{"yyy.cif":"chainID"}}
+    multimeric_template_dir: a directory where all the multimeric templates mmcifs files are stored
     """
 
-    def __init__(self, interactors: list, pair_msa: bool = True, multimeric_mode: bool = False) -> None:
+    def __init__(self, interactors: list, pair_msa: bool = True, 
+                 multimeric_mode: bool = False, 
+                 multimeric_template_meta_data: str = None,
+                 multimeric_template_dir:str = None) -> None:
         self.description = ""
         self.interactors = interactors
+        self.build_description_monomer_mapping()
         self.pair_msa = pair_msa
         self.multimeric_mode = multimeric_mode
         self.chain_id_map = dict()
         self.input_seqs = []
+        self.multimeric_template_dir = multimeric_template_dir
         self.create_output_name()
+
+        if multimeric_template_meta_data is not None:
+            self.multimeric_template_meta_data = prepare_multimeric_template_meta_info(multimeric_template_meta_data,
+                                                                                       self.multimeric_template_dir)
+            
+        if self.multimeric_mode:
+            self.create_multimeric_template_features()
         self.create_all_chain_features()
         pass
-
-    def get_all_residue_index(self):
-        """get all residue indexes from subunits"""
-        self.res_indexes = []
-        for i in self.interactors:
-            curr_res_idx = i.feature_dict['residue_index']
-            self.res_indexes.append([curr_res_idx[0], curr_res_idx[-1]])
+    
+    def build_description_monomer_mapping(self):
+        """This method constructs a dictionary {description: monomer}"""
+        self.monomers_mapping = {m.description: m for m in self.interactors}
 
     def create_output_name(self):
         """a method to create output name"""
         for i in range(len(self.interactors)):
             if i == 0:
                 self.description += f"{self.interactors[i].description}"
             else:
                 self.description += f"_and_{self.interactors[i].description}"
 
     def create_chain_id_map(self):
         """a method to create chain id"""
         multimer_sequence_str = ""
         for interactor in self.interactors:
             multimer_sequence_str = (
-                    multimer_sequence_str
-                    + f">{interactor.description}\n{interactor.sequence}\n"
+                multimer_sequence_str
+                + f">{interactor.description}\n{interactor.sequence}\n"
             )
-        self.input_seqs, input_descs = parsers.parse_fasta(multimer_sequence_str)
+        self.input_seqs, input_descs = parsers.parse_fasta(
+            multimer_sequence_str)
         self.chain_id_map = pipeline_multimer._make_chain_id_map(
             sequences=self.input_seqs, descriptions=input_descs
         )
 
     def save_binary_matrix(self, matrix, file_path):
         from PIL import Image, ImageDraw, ImageFont
         height, width = matrix.shape
@@ -498,51 +500,106 @@
             font = ImageFont.load_default()
         for col in range(width - 1):
             if matrix[:, col].any() != matrix[:, col + 1].any():
                 text = str(col + 1)
                 text_width, text_height = draw.textsize(text, font=font)
                 x = (col + 0.5) * image.width / width - text_width / 2
                 y = image.height - text_height
-                draw.text((x, y), text, font=font, fill=(0, 0, 0))  # Set text fill color to black
+                # Set text fill color to black
+                draw.text((x, y), text, font=font, fill=(0, 0, 0))
 
         image.save(file_path)
 
     def create_multichain_mask(self):
         """a method to create pdb_map for further multitemplate modeling"""
         pdb_map = []
         no_gap_map = []
         for interactor in self.interactors:
             temp_length = len(interactor.sequence)
-            pdb_map.extend([interactor.feature_dict['template_domain_names'][0]] * temp_length)
+            pdb_map.extend(
+                [interactor.feature_dict['template_domain_names'][0]] * temp_length)
             has_no_gaps = [True] * temp_length
             # for each template in the interactor, check for gaps in sequence
             for template_sequence in interactor.feature_dict['template_sequence']:
-                is_not_gap = [s != '-' for s in template_sequence.decode("utf-8").strip()]
+                is_not_gap = [
+                    s != '-' for s in template_sequence.decode("utf-8").strip()]
                 # False if any of the templates has a gap in this position
-                has_no_gaps = [a and b for a, b in zip(has_no_gaps, is_not_gap)]
+                has_no_gaps = [a and b for a,
+                               b in zip(has_no_gaps, is_not_gap)]
             no_gap_map.extend(has_no_gaps)
         multichain_mask = np.zeros((len(pdb_map), len(pdb_map)), dtype=int)
         for index1, id1 in enumerate(pdb_map):
             for index2, id2 in enumerate(pdb_map):
-                if (id1[:4] == id2[:4]):  # and (no_gap_map[index1] and no_gap_map[index2]):
+                # and (no_gap_map[index1] and no_gap_map[index2]):
+                if (id1[:4] == id2[:4]):
                     multichain_mask[index1, index2] = 1
         # DEBUG
-        # self.save_binary_matrix(multichain_mask, "multichain_mask.png")
+        self.save_binary_matrix(multichain_mask, "multichain_mask.png")
         return multichain_mask
+    
+    def create_multimeric_template_features(self):
+        """A method of creating multimeric template features"""
+        if self.multimeric_template_dir is None or not hasattr(self,"multimeric_template_meta_data"):
+            logging.warning(f"""
+You chose to use multimeric template modelling 
+but did not give path to multimeric_template_dir or the descrption File. 
+This suggests you have already created template features from your desired multimeric models when runnign 
+create_individual_features.py 
+                            """)
+            pass
+        else:
+            for monomer_name in self.multimeric_template_meta_data:
+                for k,v in self.multimeric_template_meta_data[monomer_name].items():
+                    curr_monomer = self.monomers_mapping[monomer_name]
+                    assert k.endswith(".cif"), "The multimeric template file you provided does not seem to be a mmcif file. Please check your format and make sure it ends with .cif"
+                    assert os.path.exists(os.path.join(self.multimeric_template_dir,k)), f"Your provided {k} cannot be found in: {self.multimeric_template_dir}. Abort"
+                    pdb_id = k.split('.cif')[0]
+                    multimeric_template_features = extract_multimeric_template_features_for_single_chain(query_seq=curr_monomer.sequence,
+                                                                                                        pdb_id=pdb_id,chain_id=v,
+                                                                                                        mmcif_file=os.path.join(self.multimeric_template_dir,k))
+                    curr_monomer.feature_dict.update(multimeric_template_features.features)
+            
+
+    @staticmethod
+    def remove_all_seq_features(np_chain_list: List[Dict]) -> List[Dict]:
+        """
+        Because AlphaPulldown will calculate Uniprot MSA during the feature creating step automatically,
+        thus, if the user wants to model multimeric structures without paired MSAs, this method will be called 
+        within the pair_and_merge method 
+
+        Args:
+        np_chain_list: A list of dictionary that corresponds to individual chain's feature matrices
+
+
+        Return:
+        A new list of chain features without all these xxx_all_seq features
+        """
+        output_list = []
+        for feat_dict in np_chain_list:
+            new_chain = {k: v for k, v in feat_dict.items()
+                         if '_all_seq' not in k}
+            output_list.append(new_chain)
+        return output_list
 
     def pair_and_merge(self, all_chain_features):
         """merge all chain features"""
+        feature_processing.process_unmerged_features(all_chain_features)
         MAX_TEMPLATES = 4
         MSA_CROP_SIZE = 2048
-        feature_processing.process_unmerged_features(all_chain_features)
         np_chains_list = list(all_chain_features.values())
-        pair_msa_sequences = self.pair_msa and not feature_processing._is_homomer_or_monomer(np_chains_list)
+        pair_msa_sequences = self.pair_msa and not feature_processing._is_homomer_or_monomer(
+            np_chains_list)
         if pair_msa_sequences:
-            np_chains_list = msa_pairing.create_paired_features(chains=np_chains_list)
-            np_chains_list = msa_pairing.deduplicate_unpaired_sequences(np_chains_list)
+            np_chains_list = msa_pairing.create_paired_features(
+                chains=np_chains_list)
+            np_chains_list = msa_pairing.deduplicate_unpaired_sequences(
+                np_chains_list)
+        else:
+            np_chains_list = MultimericObject.remove_all_seq_features(
+                np_chains_list)
         np_chains_list = feature_processing.crop_chains(
             np_chains_list,
             msa_crop_size=MSA_CROP_SIZE,
             pair_msa_sequences=pair_msa_sequences,
             max_templates=MAX_TEMPLATES,
         )
         np_example = msa_pairing.merge_chain_features(
@@ -560,15 +617,14 @@
         Args
         uniprot_runner: a jackhammer runner with path to the uniprot database
         msa_pairing: boolean pairs msas or not
         """
         if self.multimeric_mode:
             logging.info("Running in TrueMultimer mode")
             self.multichain_mask = self.create_multichain_mask()
-        self.get_all_residue_index()
         self.create_chain_id_map()
         all_chain_features = {}
         sequence_features = {}
         count = 0  # keep the index of input_seqs
         for chain_id, fasta_chain in self.chain_id_map.items():
             chain_features = self.interactors[count].feature_dict
             chain_features = pipeline_multimer.convert_monomer_features(
@@ -576,13 +632,24 @@
             )
             all_chain_features[chain_id] = chain_features
             sequence_features[fasta_chain.sequence] = chain_features
             count += 1
         self.all_chain_features = pipeline_multimer.add_assembly_features(
             all_chain_features
         )
+
         self.feature_dict = self.pair_and_merge(
             all_chain_features=self.all_chain_features
         )
         self.feature_dict = pipeline_multimer.pad_msa(self.feature_dict, 512)
+
+        # make integer to np.array
+        for k in ['num_alignments']:
+            self.feature_dict[k] = np.array([self.feature_dict[k]])
         if self.multimeric_mode:
+            self.feature_dict['template_sequence'] = []
             self.feature_dict['multichain_mask'] = self.multichain_mask
+            # save used templates
+            for i in self.interactors:
+                logging.info(
+                    "Used multimeric templates for protein {}".format(i.description))
+                logging.info(i.feature_dict['template_domain_names'])
```

### Comparing `alphapulldown-1.0.4/alphapulldown/predict_structure.py` & `alphapulldown-2.0.0b1/alphapulldown/predict_structure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-#
-# This script is
-# based on run_alphafold.py by DeepMind from https://github.com/deepmind/alphafold
-# and contains code copied from the script run_alphafold.py.
-# #
+""" Predict protein structures with input features from objects.py
+
+    This script is based on run_alphafold.py by DeepMind from https://github.com/deepmind/alphafold
+    and contains code copied from the script run_alphafold.py.
+
+    Author: Dingquan Yu <dingquan.yu@embl-hamburg.de>
+"""
+
 import json
 import os
 import pickle,gzip
 import time
 from absl import logging
 from alphafold.common import protein
 from alphafold.common import residue_constants
 from alphafold.relax import relax
 import numpy as np
-from alphapulldown.utils import get_run_alphafold
 import jax.numpy as jnp
 
+from alphapulldown.utils.modelling_setup import get_run_alphafold
 
 run_af = get_run_alphafold()
 RELAX_MAX_ITERATIONS = run_af.RELAX_MAX_ITERATIONS
 RELAX_ENERGY_TOLERANCE = run_af.RELAX_ENERGY_TOLERANCE
 RELAX_STIFFNESS = run_af.RELAX_STIFFNESS
 RELAX_EXCLUDE_RESIDUES = run_af.RELAX_EXCLUDE_RESIDUES
 RELAX_MAX_OUTER_ITERATIONS = run_af.RELAX_MAX_OUTER_ITERATIONS
 
 ModelsToRelax = run_af.ModelsToRelax
 
-def _jnp_to_np(output):
-  """Recursively changes jax arrays to numpy arrays."""
-  for k, v in output.items():
-    if isinstance(v, dict):
-      output[k] = _jnp_to_np(v)
-    elif isinstance(v, jnp.ndarray):
-      output[k] = np.array(v)
-  return output
-
 def get_score_from_result_pkl(pkl_path):
     """Get the score from the model result pkl file"""
 
     with open(pkl_path, "rb") as f:
         result = pickle.load(f)
     if "iptm" in result:
         score_type = "iptm+ptm"
@@ -106,14 +100,18 @@
     benchmark,
     models_to_relax: ModelsToRelax,
     fasta_name,
     allow_resume=True,
     seqs=[],
     use_gpu_relax=True
 ):
+    """
+    The actual function that predicts protein structures
+    Modified from https://github.com/google-deepmind/alphafold/blob/032e2f26732d1473ec5db7ff5b8572754576e459/run_alphafold.py#L232
+    """
     timings = {}
     unrelaxed_pdbs = {}
     relaxed_pdbs = {}
     relax_metrics = {}
     ranking_confidences = {}
     unrelaxed_proteins = {}
     prediction_result = {}
@@ -183,15 +181,15 @@
                 t_diff,
             )
 
         plddt = prediction_result["plddt"]
         ranking_confidences[model_name] = prediction_result["ranking_confidence"]
 
         # Remove jax dependency from results.
-        np_prediction_result = _jnp_to_np(dict(prediction_result))
+        np_prediction_result = run_af._jnp_to_np(dict(prediction_result))
 
         result_output_path = os.path.join(output_dir, f"result_{model_name}.pkl")
         with open(result_output_path, "wb") as f:
             pickle.dump(np_prediction_result, f, protocol=4)
 
         plddt_b_factors = np.repeat(
             plddt[:, None], residue_constants.atom_type_num, axis=-1
@@ -252,17 +250,51 @@
             f.write(relaxed_pdb_str)
 
     # Write out relaxed PDBs in rank order.
     for idx, model_name in enumerate(ranked_order):
         ranked_output_path = os.path.join(output_dir, f'ranked_{idx}.pdb')
         with open(ranked_output_path, 'w') as f:
             if model_name in relaxed_pdbs:
-                f.write(relaxed_pdbs[model_name])
+                model = relaxed_pdbs[model_name]
             else:
-                f.write(unrelaxed_pdbs[model_name])
+                model = unrelaxed_pdbs[model_name]
+            f.write(model)
+        # Calculate and report RMSD if multimeric templates were used.
+        if run_af.flags.FLAGS.multimeric_mode:
+            # Calculate RMSD
+            from alphapulldown.utils.calculate_rmsd import calculate_rmsd_and_superpose
+            import tempfile
+            template_positions = feature_dict['template_all_atom_positions'][0]
+            template_mask = feature_dict['template_all_atom_mask'][0]
+            template_aatype = feature_dict['template_aatype'][0]
+            template_residue_index = feature_dict.get('residue_index', None)
+            chain_index = feature_dict['asym_id']
+            b_factors = np.zeros(template_mask.shape, dtype=float)  # stub
+            #template_sequence = feature_dict['template_sequence'] # doesn't work because we can't store b-strings there
+
+            # Create the Protein object
+            template_protein = protein.Protein(
+                atom_positions=template_positions,
+                atom_mask=template_mask,
+                aatype=template_aatype,
+                residue_index=template_residue_index,
+                chain_index=chain_index,
+                b_factors=b_factors
+            )
+
+            # Convert to PDB format
+            pdb_string = protein.to_pdb(template_protein)
+
+            with tempfile.TemporaryDirectory() as temp_dir:
+                # TODO: do not geenrate a new template each time
+                template_file_path = f"{temp_dir}/template.pdb"
+                with open(template_file_path, 'w') as file:
+                    file.write(pdb_string)
+                # TODO: use template_sequence for alignment
+                calculate_rmsd_and_superpose(template_file_path, ranked_output_path, temp_dir)
 
     if not os.path.exists(ranking_output_path):  # already exists if restored.
         with open(ranking_output_path, "w") as f:
             label = "iptm+ptm" if "iptm" in prediction_result else "plddts"
             f.write(
                 json.dumps(
                     {label: ranking_confidences, "order": ranked_order}, indent=4
```

### Comparing `alphapulldown-1.0.4/alphapulldown/prepare_seq_names.py` & `alphapulldown-2.0.0b1/alphapulldown/scripts/prepare_seq_names.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown/remove_clashes_low_plddt.py` & `alphapulldown-2.0.0b1/alphapulldown/utils/remove_clashes_low_plddt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections import defaultdict
-from absl import app, flags
-import logging
+from absl import app, flags,logging
 import copy
 from alphafold.data.mmcif_parsing import parse
 from alphafold.common.residue_constants import residue_atoms, atom_types
 from Bio.PDB import NeighborSearch, PDBIO, MMCIFIO
 from Bio.PDB.Polypeptide import protein_letters_3to1
 from Bio import SeqIO
 from colabfold.batch import convert_pdb_to_mmcif
 from Bio.PDB import Structure, Model, Chain, Residue
 from Bio.PDB.MMCIF2Dict import MMCIF2Dict
+from pathlib import Path
 
 STANDARD_AMINO_ACIDS = residue_atoms.keys()
 
 
 def extract_seqs(template, chain_id):
     """
     Extract sequences from PDB/CIF file using Bio.SeqIO.
@@ -91,41 +91,45 @@
 
 
     def __init__(self, input_file_path, code, chain_id=None):
         self.atom_site_label_seq_id = None
         self.atom_to_label_id = None
         self.atom_site_label_seq_ids = None
         self.input_file_path = input_file_path
-        self.chain_id = chain_id
+        if chain_id is not None:
+            self.chain_id = chain_id 
+        else:
+            raise ValueError(f"You have to specify a chain id when using multimeric template modelling")
         logging.info("Parsing SEQRES...")
         sequence_atom, sequence_seqres = extract_seqs(input_file_path, chain_id)
         if not sequence_seqres:
             logging.warning(f"No SEQRES was found in {input_file_path}! Parsing from atoms...")
         file_type = input_file_path.suffix.lower()
         if file_type == ".pdb":
             logging.info(f"Converting to mmCIF: {input_file_path}")
             convert_pdb_to_mmcif(input_file_path)
             self.input_file_path = input_file_path.with_suffix(".cif")
         with open(self.input_file_path) as f:
             mmcif = f.read()
-        parsing_result = parse(file_id=code, mmcif_string=mmcif)
-        if parsing_result.errors:
-            raise Exception(f"Can't parse mmcif file {self.input_file_path}: {parsing_result.errors}")
-        mmcif_object = parsing_result.mmcif_object
+        self.parsing_result = parse(file_id=code, mmcif_string=mmcif)
+        if self.parsing_result.errors:
+            raise Exception(f"Can't parse mmcif file {self.input_file_path}: {self.parsing_result.errors}")
+        mmcif_object = self.parsing_result.mmcif_object
         self.seqres_to_structure = mmcif_object.seqres_to_structure[chain_id]
         structure, sequence_atom = self.extract_chain(mmcif_object.structure, chain_id)
         self.sequence_atom = sequence_atom
         self.sequence_seqres = mmcif_object.chain_to_seqres[chain_id]
         if self.sequence_seqres is None:
             self.sequence_seqres = sequence_seqres
         if self.sequence_atom is None:
             self.sequence_atom = sequence_atom
         self.structure = remove_hydrogens_and_irregularities(structure)
         self.map_atoms_to_label_seq_id()
         self.extract_atom_site_label_seq_id()
+        self.all_chains_structure = mmcif_object.structure  # for removing intra-chain clashes
         self.structure_modified = False
 
 
     def __eq__(self, other):
         return self.structure == other.structure
 
 
@@ -242,31 +246,34 @@
 
     def remove_clashes(self, threshold=0.9, hb_allowance=0.4):
         """
         Remove residues that are clashing with other residues in the structure.
         o threshold - threshold for VDW overlap to identify clashes (default: 0.9)
         o hb_allowance - correction to threshold for hydrogen bonding (default: 0.4)
         """
-        model = self.structure[0]
-        ns = NeighborSearch(list(model.get_atoms()))
+        model = self.structure
+        ns = NeighborSearch(list(self.all_chains_structure.get_atoms()))
         clashing_atoms = set()
 
-        for residue in model.get_residues():
+        for residue in self.structure.get_residues():
             for atom in residue:
-                neighbors = ns.search(atom.get_coord(), self.VDW_RADII[atom.element] + max(self.VDW_RADII.values()))
+                neighbors = ns.search(center=atom.get_coord(),
+                                      radius=self.VDW_RADII[atom.element] + max(self.VDW_RADII.values()),
+                                      level='A')
                 for neighbor in neighbors:
-                    if neighbor.get_parent() == atom.get_parent() or \
-                            abs(neighbor.get_parent().id[1] - atom.get_parent().id[1]) <= 1:
-                        continue
+                    if neighbor.get_parent() == atom.get_parent():
+                        continue  # Same residue
+                    if abs(neighbor.get_parent().id[1] - residue.id[1]) <= 1 and \
+                            neighbor.get_parent().get_parent() == residue.get_parent():
+                        continue  # Neighboring residues in the same chain
                     overlap = (self.VDW_RADII[atom.element] + self.VDW_RADII[neighbor.element]) - (atom - neighbor)
                     if self.is_potential_hbond(atom, neighbor):
                         overlap -= hb_allowance
                     if overlap >= threshold:
                         clashing_atoms.add(atom)
-                        clashing_atoms.add(neighbor)
                         break
 
         # Remove residues if at least one atom is clashing
         clashing_residues = set(atom.get_parent() for atom in clashing_atoms)
         logging.info(f"Unique clashing atoms: {len(clashing_atoms)} out of {len(list(model.get_atoms()))}")
         logging.info(f"Unique clashing residues: {len(clashing_residues)} out of {len(list(model.get_residues()))}")
         # remove from structure and seqres_to_structure
@@ -311,38 +318,42 @@
         self.extract_atom_site_label_seq_id()
 
 
     def save_structure(self, output_file_path):
         """
         Save structure to a file.
         """
+        output_file_path = str(output_file_path)
         if output_file_path.endswith(".pdb"):
             io = PDBIO()
         elif output_file_path.endswith(".cif"):
             io = MMCIFIO()
+        #io.set_structure(self.all_chains_structure[self.chain_id])
         io.set_structure(self.structure)
         io.save(output_file_path)
 
 
 def main(argv):
-    input_file_path = flags.FLAGS.input_file_path
-    output_file_path = flags.FLAGS.output_file_path
+    input_file_path = Path(flags.FLAGS.input_file_path)
+    output_file_path = Path(flags.FLAGS.output_file_path)
+    chain = flags.FLAGS.chain
     threshold = flags.FLAGS.threshold
     hb_allowance = flags.FLAGS.hb_allowance
     plddt_threshold = flags.FLAGS.plddt_threshold
 
-    bio_struct = MmcifChainFiltered(input_file_path, "TEST")
+    bio_struct = MmcifChainFiltered(input_file_path, "TEST", chain)
     bio_struct.remove_clashes(threshold, hb_allowance)
     bio_struct.remove_low_plddt(plddt_threshold)
 
     if output_file_path:
         bio_struct.save_structure(output_file_path)
 
 
 if __name__ == '__main__':
     flags.DEFINE_string("input_file_path", None, "Path to the input PDB or CIF file")
-    flags.DEFINE_string("output_file_path", None, "Path to save the output file. Optional if --save is False")
-    flags.DEFINE_float("threshold", 0.9, "Threshold for VDW overlap to identify clashes")
+    flags.DEFINE_string("output_file_path", None, "Path to save the output file.")
+    flags.DEFINE_string("chain", "A", "Chain ID")
+    flags.DEFINE_float("threshold", 1.0, "Threshold for VDW overlap to identify clashes")
     flags.DEFINE_float("hb_allowance", 0.4, "Allowance for hydrogen bonding (default: 0.0)")
     flags.DEFINE_float("plddt_threshold", 50, "Threshold for pLDDT score (default: 50)")
     flags.mark_flags_as_required(["input_file_path"])
     app.run(main)
```

### Comparing `alphapulldown-1.0.4/alphapulldown/rename_colab_search_a3m.py` & `alphapulldown-2.0.0b1/alphapulldown/scripts/rename_colab_search_a3m.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/alphapulldown.egg-info/PKG-INFO` & `alphapulldown-2.0.0b1/alphapulldown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphapulldown
-Version: 1.0.4
+Version: 2.0.0b1
 Summary: Pipeline allows massive screening using alphafold
 Home-page: https://github.com/KosinskiLab/AlphaPulldown
 Author: Dingquan Yu
 Author-email: dingquan.yu@embl-hamburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: dm-haiku
 Requires-Dist: dm-tree>=0.1.6
 Requires-Dist: h5py>=3.1.0
 Requires-Dist: matplotlib>=3.3.3
 Requires-Dist: ml-collections>=0.1.0
 Requires-Dist: numpy
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: tensorflow>=2.14.0
+Requires-Dist: tensorflow==2.14.0
 Requires-Dist: importlib-resources>=6.1.0
 Requires-Dist: biopython==1.81
 Requires-Dist: nbformat>=5.9.2
 Requires-Dist: py3Dmol==2.0.4
 Requires-Dist: ipython==8.16.1
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: appdirs>=1.4.4
@@ -94,15 +94,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.3
+python3 -m pip install alphapulldown==1.0.4
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-1.0.4/alphapulldown.egg-info/SOURCES.txt` & `alphapulldown-2.0.0b1/alphapulldown.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-stereo_chemical_props.txt
 ./AlphaLink2/unifold/__init__.py
 ./AlphaLink2/unifold/alphalink_inference.py
 ./AlphaLink2/unifold/config.py
 ./AlphaLink2/unifold/dataset.py
 ./AlphaLink2/unifold/dataset_inference.py
 ./AlphaLink2/unifold/homo_search.py
 ./AlphaLink2/unifold/inference.py
@@ -56,14 +55,23 @@
 ./AlphaLink2/unifold/symmetry/assemble.py
 ./AlphaLink2/unifold/symmetry/config.py
 ./AlphaLink2/unifold/symmetry/dataset.py
 ./AlphaLink2/unifold/symmetry/geometry_utils.py
 ./AlphaLink2/unifold/symmetry/loss.py
 ./AlphaLink2/unifold/symmetry/model.py
 ./AlphaLink2/unifold/symmetry/modules.py
+./ColabFold/colabfold/__init__.py
+./ColabFold/colabfold/batch.py
+./ColabFold/colabfold/citations.py
+./ColabFold/colabfold/colabfold.py
+./ColabFold/colabfold/download.py
+./ColabFold/colabfold/pdb.py
+./ColabFold/colabfold/plot.py
+./ColabFold/colabfold/relax.py
+./ColabFold/colabfold/utils.py
 ./alphafold/run_alphafold.py
 ./alphafold/alphafold/__init__.py
 ./alphafold/alphafold/run_alphafold.py
 ./alphafold/alphafold/version.py
 ./alphafold/alphafold/common/__init__.py
 ./alphafold/alphafold/common/confidence.py
 ./alphafold/alphafold/common/confidence_test.py
@@ -139,51 +147,61 @@
 ./alphafold/alphafold/relax/cleanup.py
 ./alphafold/alphafold/relax/cleanup_test.py
 ./alphafold/alphafold/relax/relax.py
 ./alphafold/alphafold/relax/relax_test.py
 ./alphafold/alphafold/relax/utils.py
 ./alphafold/alphafold/relax/utils_test.py
 ./alphapulldown/__init__.py
-./alphapulldown/create_custom_template_db.py
-./alphapulldown/create_individual_features.py
-./alphapulldown/create_individual_features_with_templates.py
-./alphapulldown/generate_crosslink_pickle.py
 ./alphapulldown/objects.py
-./alphapulldown/plot_pae.py
 ./alphapulldown/predict_structure.py
-./alphapulldown/prepare_seq_names.py
-./alphapulldown/remove_clashes_low_plddt.py
-./alphapulldown/rename_colab_search_a3m.py
-./alphapulldown/run_multimer_jobs.py
-./alphapulldown/utils.py
-./alphapulldown/ColabFold/colabfold/__init__.py
-./alphapulldown/ColabFold/colabfold/batch.py
-./alphapulldown/ColabFold/colabfold/citations.py
-./alphapulldown/ColabFold/colabfold/colabfold.py
-./alphapulldown/ColabFold/colabfold/download.py
-./alphapulldown/ColabFold/colabfold/pdb.py
-./alphapulldown/ColabFold/colabfold/plot.py
-./alphapulldown/ColabFold/colabfold/relax.py
-./alphapulldown/ColabFold/colabfold/utils.py
+./alphapulldown/test_new_mmt.py
 ./alphapulldown/analysis_pipeline/af2_3dmol.py
 ./alphapulldown/analysis_pipeline/calculate_mpdockq.py
-./alphapulldown/analysis_pipeline/calculate_rmsd.py
 ./alphapulldown/analysis_pipeline/create_notebook.py
 ./alphapulldown/analysis_pipeline/get_good_inter_pae.py
 ./alphapulldown/analysis_pipeline/test_create_notebook.py
 ./alphapulldown/analysis_pipeline/utils.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
+./alphapulldown/folding_backend/__init__.py
+./alphapulldown/folding_backend/alphafold_backend.py
+./alphapulldown/folding_backend/alphalink_backend.py
+./alphapulldown/folding_backend/folding_backend.py
+./alphapulldown/folding_backend/unifold_backend.py
+./alphapulldown/scripts/convert_to_modelcif.py
+./alphapulldown/scripts/create_individual_features.py
+./alphapulldown/scripts/generate_crosslink_pickle.py
+./alphapulldown/scripts/prepare_seq_names.py
+./alphapulldown/scripts/rename_colab_search_a3m.py
+./alphapulldown/scripts/run_multimer_jobs.py
+./alphapulldown/scripts/run_structure_prediction.py
+./alphapulldown/utils/__init__.py
+./alphapulldown/utils/calculate_rmsd.py
+./alphapulldown/utils/create_combinations.py
+./alphapulldown/utils/create_custom_template_db.py
+./alphapulldown/utils/file_handling.py
+./alphapulldown/utils/modelling_setup.py
+./alphapulldown/utils/multimeric_template_utils.py
+./alphapulldown/utils/plotting.py
+./alphapulldown/utils/post_modelling.py
+./alphapulldown/utils/remove_clashes_low_plddt.py
+./alphapulldown/utils/save_meta_data.py
 alphafold/run_alphafold.py
 alphapulldown.egg-info/PKG-INFO
 alphapulldown.egg-info/SOURCES.txt
 alphapulldown.egg-info/dependency_links.txt
 alphapulldown.egg-info/requires.txt
 alphapulldown.egg-info/top_level.txt
-test/test_create_objects.py
+alphapulldown/package_data/stereo_chemical_props.txt
+test/test_alphalink2_folding_backend.py
+test/test_create_monomeric_objects.py
+test/test_create_multimeric_objects.py
+test/test_create_multimeric_template_features.py
 test/test_crosslink_inference.py
 test/test_crosslink_input.py
 test/test_custom_db.py
+test/test_features.py
 test/test_features_with_templates.py
 test/test_predictions_slurm.py
+test/test_python_imports.py
 test/test_remove_clashes_low_plddt.py
```

### Comparing `alphapulldown-1.0.4/setup.cfg` & `alphapulldown-2.0.0b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = 
 	alphapulldown
+	alphapulldown.utils
+	alphapulldown.folding_backend
+	alphapulldown.analysis_pipeline
 	alphafold
 	alphafold.data
 	alphafold.data.tools
 	alphafold.common
 	alphafold.relax
 	alphafold.model
 	alphafold.model.geometry
@@ -30,16 +33,17 @@
 	unifold.data
 	unifold.modules
 	unifold.msa
 	unifold.losses
 	unifold.symmetry
 package_dir = 
 	alphapulldown = ./alphapulldown
+	alphapulldown.folding_backend = ./alphapulldown/folding_backend
 	alphafold = ./alphafold/alphafold
-	colabfold = ./alphapulldown/ColabFold/colabfold
+	colabfold = ./ColabFold/colabfold
 	analysis_pipeline = ./alphapulldown/analysis_pipeline
 	af2plots = ./alphapulldown/analysis_pipeline/af2plots/af2plots
 	unifold = ./AlphaLink2/unifold/
 	unifold.data = ./AlphaLink2/unifold/data
 	unifold.losses = ./AlphaLink2/unifold/losses
 	unifold.symmetry = ./AlphaLink2/unifold/symmetry
 include_package_data = True
@@ -49,27 +53,35 @@
 	dm-haiku
 	dm-tree>=0.1.6
 	h5py>=3.1.0
 	matplotlib>=3.3.3
 	ml-collections>=0.1.0
 	numpy
 	pandas>=1.5.3
-	tensorflow>=2.14.0
+	tensorflow==2.14.0
 	importlib-resources>=6.1.0
 	biopython==1.81
 	nbformat>=5.9.2
 	py3Dmol==2.0.4
 	ipython==8.16.1
 	tqdm>=4.66.1
 	appdirs>=1.4.4
 	jupyterlab
 	ipywidgets
-scripts = ./alphafold/run_alphafold.py, ./alphapulldown/create_individual_features.py, ./alphapulldown/create_individual_features_with_templates.py, ./alphapulldown/run_multimer_jobs.py, ./alphapulldown/analysis_pipeline/create_notebook.py, ./alphapulldown/rename_colab_search_a3m.py, ./alphapulldown/prepare_seq_names.py, ./alphapulldown/generate_crosslink_pickle.py
+scripts = ./alphafold/run_alphafold.py
+	./alphapulldown/scripts/create_individual_features.py
+	./alphapulldown/scripts/run_multimer_jobs.py
+	./alphapulldown/analysis_pipeline/create_notebook.py
+	./alphapulldown/scripts/rename_colab_search_a3m.py
+	./alphapulldown/scripts/prepare_seq_names.py
+	./alphapulldown/scripts/generate_crosslink_pickle.py
+	./alphapulldown/scripts/convert_to_modelcif.py
+	./alphapulldown/scripts/run_structure_prediction.py
 
 [options.data_files]
-lib/python3.10/site-packages/alphafold/common/ = stereo_chemical_props.txt
+lib/python3.10/site-packages/alphafold/common/ = ./alphapulldown/package_data/stereo_chemical_props.txt
 lib/python3.10/site-packages/alphafold/ = ./alphafold/run_alphafold.py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `alphapulldown-1.0.4/stereo_chemical_props.txt` & `alphapulldown-2.0.0b1/alphapulldown/package_data/stereo_chemical_props.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/test/test_crosslink_inference.py` & `alphapulldown-2.0.0b1/test/test_crosslink_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import tempfile
 import unittest
 import sys
 import os
 import torch
 from unifold.modules.alphafold import AlphaFold
 from unifold.alphalink_inference import prepare_model_runner
-from unifold.alphalink_inference import alphalink_prediction
 from unifold.dataset import process_ap
 from unifold.config import model_config
 from alphapulldown.utils import create
-from alphapulldown.run_multimer_jobs import predict_individual_jobs,create_custom_jobs
 
 class _TestBase(unittest.TestCase):
     def setUp(self) -> None:
         self.crosslink_file_path = os.path.join(os.path.dirname(__file__),"test_data/example_crosslink.pkl.gz")
         self.config_data_model_name = 'model_5_ptm_af2'
         self.config_alphafold_model_name = 'multimer_af2_crop'
 
@@ -22,41 +20,41 @@
     def setUp(self) -> None:
         super().setUp()
         self.output_dir = tempfile.mkdtemp()
         self.monomer_object_path = os.path.join(os.path.dirname(__file__),"test_data/")
         self.protein_list = os.path.join(os.path.dirname(__file__),"test_data/example_crosslinked_pair.txt")
         self.alphalink_weight = '/g/alphafold/alphalink_weights/AlphaLink-Multimer_SDA_v3.pt'
         self.multimerobject = create_custom_jobs(self.protein_list,self.monomer_object_path,job_index=1,pair_msa=True)[0]
-        
+    @unittest.skip
     def test1_process_features(self):
         """Test whether the PyTorch model of AlphaLink can be initiated successfully"""
         configs = model_config(self.config_data_model_name)
         processed_features,_ = process_ap(config=configs.data,
                                           features=self.multimerobject.feature_dict,
                                           mode="predict",labels=None,
                                           seed=42,batch_idx=None,
                                           data_idx=None,is_distillation=False,
                                           chain_id_map = self.multimerobject.chain_id_map,
                                           crosslinks = self.crosslink_file_path
                                           )
-                
+    @unittest.skip
     def test2_load_AlphaLink_weights(self):
         """This is testing weither loading the PyTorch checkpoint is sucessfull"""
         if torch.cuda.is_available():
             model_device = 'cuda:0'
         else:
             model_device = 'cpu'
 
         config = model_config(self.config_alphafold_model_name)
         model = AlphaFold(config)
         state_dict = torch.load(self.alphalink_weight)["ema"]["params"]
         state_dict = {".".join(k.split(".")[1:]): v for k, v in state_dict.items()}
         model.load_state_dict(state_dict)
         model.to(model_device)
-
+    @unittest.skip
     def test3_test_inference(self):
         if torch.cuda.is_available():
             model_device = 'cuda:0'
         else:
             model_device = 'cpu'
         model = prepare_model_runner(self.alphalink_weight,model_device=model_device)
```

### Comparing `alphapulldown-1.0.4/test/test_crosslink_input.py` & `alphapulldown-2.0.0b1/test/test_crosslink_input.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/test/test_custom_db.py` & `alphapulldown-2.0.0b1/test/test_custom_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import pytest
-from alphapulldown.create_custom_template_db import create_db
+from alphapulldown.utils.create_custom_template_db import create_db
 import tempfile
 import os
 from alphafold.data import mmcif_parsing
 from pathlib import Path
 from Bio.PDB import MMCIF2Dict
 from alphafold.data.mmcif_parsing import _get_atom_site_list, _get_protein_chains
 
@@ -65,11 +64,11 @@
 def test_from_pdb(capfd):
     run_test(["./test/test_data/true_multimer/3L4Q.pdb"], ["C"])
 
 def test_from_cif(capfd):
     run_test(["./test/test_data/true_multimer/3L4Q.cif"], ["A"])
 
 def test_from_af_output_pdb(capfd):
-    run_test(["./test/test_data/true_multimer/cage_BC_AF.pdb"], ["B"])
+    run_test(["./test/test_data/true_multimer/ranked_0.pdb"], ["B"])
 
 def test_from_minimal_pdb(capfd):
     run_test(["./test/test_data/true_multimer/RANdom_name1_.7-1_0.pdb"], ["B"])
```

### Comparing `alphapulldown-1.0.4/test/test_features_with_templates.py` & `alphapulldown-2.0.0b1/test/test_features_with_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+import shutil
+import pickle
+import tempfile
 import subprocess
 from pathlib import Path
+
+import numpy as np
 from absl.testing import absltest
-import alphapulldown.create_individual_features_with_templates as run_features_generation
-import pickle
-import  numpy as np
-from alphapulldown.remove_clashes_low_plddt import extract_seqs
-import tempfile
-import shutil
-import glob
 
+from alphapulldown.utils.remove_clashes_low_plddt import extract_seqs
 
 class TestCreateIndividualFeaturesWithTemplates(absltest.TestCase):
 
     def setUp(self):
         super().setUp()
         self.temp_dir = tempfile.TemporaryDirectory()  # Create a temporary directory
         self.TEST_DATA_DIR = Path(self.temp_dir.name)  # Use the temporary directory as the test data directory
@@ -57,14 +56,15 @@
 
         # Mock databases
         create_mock_file(root_dir / 'uniref90/uniref90.fasta')
         create_mock_file(root_dir / 'mgnify/mgy_clusters_2022_05.fa')
         create_mock_file(root_dir / 'uniprot/uniprot.fasta')
         create_mock_file(root_dir / 'bfd/bfd_metaclust_clu_complete_id30_c90_final_seq.sorted_opt_hhm.ffindex')
         create_mock_file(root_dir / 'uniref30/UniRef30_2021_03_hhm.ffindex')
+        create_mock_file(root_dir / 'uniref30/UniRef30_2023_02_hhm.ffindex')
         create_mock_file(root_dir / 'pdb70/pdb70_hhm.ffindex')
 
         # Mock hhblits files
         hhblits_root = root_dir / 'bfd/bfd_metaclust_clu_complete_id30_c90_final_seq.sorted_opt'
         hhblits_files = ['_a3m.ffdata', '_a3m.ffindex', '_cs219.ffdata', '_cs219.ffindex', '_hhmm.ffdata',
                          '_hhmm.ffindex']
         for file in hhblits_files:
@@ -74,23 +74,23 @@
         uniclust_db_root = root_dir / 'uniclust30/uniclust30_2018_08/uniclust30_2018_08'
         uniclust_db_files = ['_a3m_db', '_a3m.ffdata', '_a3m.ffindex', '.cs219', '_cs219.ffdata', '_cs219.ffindex',
                              '_hhm_db', '_hhm.ffdata', '_hhm.ffindex']
         for suffix in uniclust_db_files:
             create_mock_file(f"{uniclust_db_root}{suffix}")
 
         # Mock uniref30 files - Adjusted for the correct naming convention
-        uniref_db_root = root_dir / 'uniref30/UniRef30_2021_03'
+        #uniref_db_root = root_dir / 'uniref30/UniRef30_2021_03'
+        uniref_db_root = root_dir / 'uniref30/UniRef30_2023_02'
         uniref_db_files = ['_a3m.ffdata', '_a3m.ffindex', '_hmm.ffdata', '_hmm.ffindex', '_cs.ffdata', '_cs.ffindex']
         for suffix in uniref_db_files:
             create_mock_file(f"{uniref_db_root}{suffix}")
 
         # Prepare the command and arguments
         cmd = [
-            'python',
-            run_features_generation.__file__,
+            'create_individual_features.py',
             '--use_precomputed_msas', 'True',
             '--save_msa_files', 'True',
             '--skip_existing', 'True',
             '--data_dir', f"{self.TEST_DATA_DIR}",
             '--max_template_date', '3021-01-01',
             '--threshold_clashes', '1000',
             '--hb_allowance', '0.4',
```

### Comparing `alphapulldown-1.0.4/test/test_predictions_slurm.py` & `alphapulldown-2.0.0b1/test/test_predictions_slurm.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-1.0.4/test/test_remove_clashes_low_plddt.py` & `alphapulldown-2.0.0b1/test/test_remove_clashes_low_plddt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import pytest
 import os
 import alphapulldown
-from alphapulldown.remove_clashes_low_plddt import MmcifChainFiltered
+from alphapulldown.utils.remove_clashes_low_plddt import MmcifChainFiltered
 from pathlib import Path
 
 alphapulldown_dir = os.path.dirname(alphapulldown.__file__)
 alphapulldown_dir = Path(alphapulldown_dir)
-cif_file = alphapulldown_dir / '..' / 'test' / 'test_data' / 'true_multimer' / 'cage_BC_AF.cif'
+pdb_file = alphapulldown_dir / '..' / 'test' / 'test_data' / 'true_multimer' / 'ranked_0.pdb'
 
 
 def test_init():
     for chain in ['B', 'C']:
-        mmcif_chain = MmcifChainFiltered(cif_file, "TEST", chain)
-        assert mmcif_chain.input_file_path == cif_file
+        mmcif_chain = MmcifChainFiltered(pdb_file, "TEST", chain)
+        assert mmcif_chain.input_file_path == pdb_file.with_suffix('.cif')
         assert mmcif_chain.chain_id == chain
 
 
 def test_eq():
-    mmcif_chain1 = MmcifChainFiltered(cif_file, "TEST", "B")
-    mmcif_chain2 = MmcifChainFiltered(cif_file, "TEST", "B")
+    mmcif_chain1 = MmcifChainFiltered(pdb_file, "TEST", "B")
+    mmcif_chain2 = MmcifChainFiltered(pdb_file, "TEST", "B")
     assert mmcif_chain1 == mmcif_chain2
 
 
 def test_remove_clashes():
     for chain in ['B', 'C']:
-        mmcif_chain = MmcifChainFiltered(cif_file, "TEST", chain)
+        mmcif_chain = MmcifChainFiltered(pdb_file, "TEST", chain)
         initial_atoms = list(mmcif_chain.structure.get_atoms())
 
         mmcif_chain.remove_clashes()
+        mmcif_chain.remove_low_plddt()
         final_atoms = list(mmcif_chain.structure.get_atoms())
 
         assert len(final_atoms) < len(initial_atoms)
 
 
 def test_remove_low_plddt():
     for chain in ['B', 'C']:
-        mmcif_chain = MmcifChainFiltered(cif_file, "TEST", chain)
+        mmcif_chain = MmcifChainFiltered(pdb_file, "TEST", chain)
         initial_atoms = list(mmcif_chain.structure.get_atoms())
 
         mmcif_chain.remove_low_plddt()
         final_atoms = list(mmcif_chain.structure.get_atoms())
 
         assert len(final_atoms) < len(initial_atoms)
```

