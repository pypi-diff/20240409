# Comparing `tmp/nef_pipelines-0.1.62.tar.gz` & `tmp/nef_pipelines-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.62.tar", last modified: Tue Apr  9 11:16:22 2024, max compression
+gzip compressed data, was "nef_pipelines-0.1.63.tar", last modified: Tue Apr  9 11:41:15 2024, max compression
```

## Comparing `nef_pipelines-0.1.62.tar` & `nef_pipelines-0.1.63.tar`

### file list

```diff
@@ -1,491 +1,491 @@
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.952124 nef_pipelines-0.1.62/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.797474 nef_pipelines-0.1.62/.github/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.860494 nef_pipelines-0.1.62/.github/workflows/
--rw-r--r--   0 garyt      (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.62/.github/workflows/ci.yml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.868369 nef_pipelines-0.1.62/.idea/
--rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.62/.idea/.gitignore
--rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.62/.idea/.name
--rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.62/.idea/NFC.iml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.871741 nef_pipelines-0.1.62/.idea/inspectionProfiles/
--rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.62/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.62/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.62/.idea/modules.xml
--rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.62/.idea/vcs.xml
--rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.62/.pre-commit-config.yaml
--rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.62/.readthedocs.yml
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.62/AUTHORS.md
--rw-r--r--   0 garyt      (501) staff       (20)     7058 2024-04-09 11:15:06.000000 nef_pipelines-0.1.62/CHANGELOG.md
--rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.62/CONTRIBUTING.md
--rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.62/LICENSE.txt
--rw-r--r--   0 garyt      (501) staff       (20)     9641 2024-04-09 11:16:22.951542 nef_pipelines-0.1.62/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)     8212 2024-03-04 22:23:39.000000 nef_pipelines-0.1.62/README.md
--rw-r--r--   0 garyt      (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.62/TODO.md
--rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.62/pyproject.toml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.881580 nef_pipelines-0.1.62/references/
--rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.62/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.62/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.62/references/kosol idps molecules-18-10802.pdf
--rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.62/release_to_pypi.sh
--rw-r--r--   0 garyt      (501) staff       (20)      387 2024-04-09 11:14:15.000000 nef_pipelines-0.1.62/requirements.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1733 2024-04-09 11:16:22.953535 nef_pipelines-0.1.62/setup.cfg
--rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.62/setup.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.798528 nef_pipelines-0.1.62/src/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.893063 nef_pipelines-0.1.62/src/nef_pipelines/
--rw-r--r--   0 garyt      (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.62/src/nef_pipelines/VERSION
--rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.906787 nef_pipelines-0.1.62/src/nef_pipelines/data/
--rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/ambiguity_translations.json
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.069289 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/
--rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
--rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
--rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
--rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
--rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
--rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
--rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.111630 nef_pipelines-0.1.62/src/nef_pipelines/lib/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    20383 2024-04-09 10:57:52.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-04-08 08:38:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    25699 2024-04-06 13:43:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     6334 2024-03-19 22:25:46.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    14093 2024-04-09 11:03:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garyt      (501) staff       (20)    10315 2024-03-04 21:14:19.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.119263 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/chem_comp.py
--rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/io.py
--rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/object_iter.py
--rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/translator.py
--rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garyt      (501) staff       (20)    27949 2024-03-19 22:43:06.000000 nef_pipelines-0.1.62/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     5431 2024-03-04 22:07:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/main.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.120368 nef_pipelines-0.1.62/src/nef_pipelines/nef_app/
--rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.129026 nef_pipelines-0.1.62/src/nef_pipelines/tests/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.142987 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.148999 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garyt      (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garyt      (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.151141 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.155714 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
--rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.157343 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.159978 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)     3621 2024-04-07 09:20:05.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.161742 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.227761 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr--r--   0 garyt      (501) staff       (20)     3405 2024-04-07 09:19:50.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.292504 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.296147 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_delete.py
--rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_filter.py
--rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_tabulate.py
--rwxr--r--   0 garyt      (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_unassign.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.301365 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.311267 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sparky_all.out
--rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     6221 2024-04-07 09:31:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.318793 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.362176 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garyt      (501) staff       (20)      840 2024-03-04 21:16:11.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4093 2024-02-10 20:35:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:21.801988 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.367827 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
--rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.383234 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.413826 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     2742 2024-02-10 18:10:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr--r--   0 garyt      (501) staff       (20)     3881 2023-08-24 07:58:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     3847 2024-02-10 20:35:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.416287 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.419696 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr--r--   0 garyt      (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.423608 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.440523 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
--rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     7860 2023-12-20 18:35:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
--rwxr--r--   0 garyt      (501) staff       (20)     4316 2023-12-20 18:23:05.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.464220 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7234 2024-04-08 08:37:44.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.466028 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.473719 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.496536 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     4314 2024-04-07 09:31:37.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.502456 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.515059 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
--rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
--rw-r--r--   0 garyt      (501) staff       (20)     5638 2023-11-05 11:38:38.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     1877 2023-11-01 22:08:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_import_order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)     5825 2023-12-08 21:08:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_import_restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3282 2023-12-07 10:10:58.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_secondary_structure.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.617333 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/header.nef
--rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_header.py
--rwxr--r--   0 garyt      (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     7636 2024-04-06 13:42:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.621593 nef_pipelines-0.1.62/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.627550 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.633692 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
--rw-r--r--   0 garyt      (501) staff       (20)     3392 2024-04-07 09:31:44.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8984 2024-03-27 21:18:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.643691 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.665871 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garyt      (501) staff       (20)     8138 2023-10-30 22:33:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     6577 2023-10-30 08:28:29.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    11089 2023-07-12 13:14:21.000000 nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.699375 nef_pipelines-0.1.62/src/nef_pipelines/tools/
--rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.704967 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-03-04 21:23:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.707526 nef_pipelines-0.1.62/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.721262 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garyt      (501) staff       (20)     8838 2023-12-21 14:29:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/filter.py
--rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-02-10 20:35:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     7774 2024-02-12 15:11:26.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garyt      (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/unassign.py
--rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.725633 nef_pipelines-0.1.62/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/peaks/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.729173 nef_pipelines-0.1.62/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    12051 2024-04-09 11:02:16.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.730591 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.735698 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.741031 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.742884 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.744680 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.746248 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.748584 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.751470 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     6680 2024-04-06 13:44:59.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.773318 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garyt      (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.779138 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garyt      (501) staff       (20)      826 2024-04-06 13:45:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     5998 2024-04-06 13:45:32.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.782440 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    11631 2024-04-06 16:51:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.785990 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.792496 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.795156 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/
--rw-r--r--   0 garyt      (501) staff       (20)      682 2024-03-19 07:46:08.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.800827 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7952 2024-04-09 11:01:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/project.py
--rw-r--r--   0 garyt      (501) staff       (20)     5993 2024-03-19 07:42:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    24119 2024-03-15 17:31:35.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.804087 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.809874 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.815588 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16945 2023-11-21 22:15:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2313 2024-02-10 20:35:20.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     5749 2023-12-20 19:52:03.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.817275 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.819747 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.848728 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.851980 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     4829 2023-12-20 18:35:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.853908 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.856339 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.858100 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.860957 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.864731 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.866813 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.872708 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     9018 2024-03-27 21:44:50.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.875607 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/
--rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.894805 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8157 2023-12-07 22:13:01.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.900782 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5134 2024-03-19 07:42:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
--rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/talos_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.902269 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.904226 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.907453 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.914633 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     2923 2024-03-27 21:18:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2852 2023-05-21 10:57:07.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.918184 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.943077 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.948974 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:16:22.949955 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/
--rw-r--r--   0 garyt      (501) staff       (20)     9641 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)    21038 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garyt      (501) staff       (20)       48 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garyt      (501) staff       (20)      460 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garyt      (501) staff       (20)       19 2024-04-09 11:16:21.000000 nef_pipelines-0.1.62/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.62/tox.ini
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.236254 nef_pipelines-0.1.63/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.061859 nef_pipelines-0.1.63/.github/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.135360 nef_pipelines-0.1.63/.github/workflows/
+-rw-r--r--   0 garyt      (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.63/.github/workflows/ci.yml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.144050 nef_pipelines-0.1.63/.idea/
+-rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.63/.idea/.gitignore
+-rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.63/.idea/.name
+-rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.63/.idea/NFC.iml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.147115 nef_pipelines-0.1.63/.idea/inspectionProfiles/
+-rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.63/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.63/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.63/.idea/modules.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.63/.idea/vcs.xml
+-rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.63/.pre-commit-config.yaml
+-rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.63/.readthedocs.yml
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.63/AUTHORS.md
+-rw-r--r--   0 garyt      (501) staff       (20)     7150 2024-04-09 11:40:52.000000 nef_pipelines-0.1.63/CHANGELOG.md
+-rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.63/CONTRIBUTING.md
+-rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.63/LICENSE.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     9606 2024-04-09 11:41:15.235664 nef_pipelines-0.1.63/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)     8212 2024-03-04 22:23:39.000000 nef_pipelines-0.1.63/README.md
+-rw-r--r--   0 garyt      (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.63/TODO.md
+-rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.63/pyproject.toml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.155993 nef_pipelines-0.1.63/references/
+-rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.63/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.63/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.63/references/kosol idps molecules-18-10802.pdf
+-rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.63/release_to_pypi.sh
+-rw-r--r--   0 garyt      (501) staff       (20)      367 2024-04-09 11:38:51.000000 nef_pipelines-0.1.63/requirements.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1712 2024-04-09 11:41:15.238175 nef_pipelines-0.1.63/setup.cfg
+-rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.63/setup.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.062884 nef_pipelines-0.1.63/src/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.168676 nef_pipelines-0.1.63/src/nef_pipelines/
+-rw-r--r--   0 garyt      (501) staff       (20)        6 2024-04-09 11:38:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/VERSION
+-rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.203643 nef_pipelines-0.1.63/src/nef_pipelines/data/
+-rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/ambiguity_translations.json
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.348867 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/
+-rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
+-rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
+-rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
+-rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
+-rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.391808 nef_pipelines-0.1.63/src/nef_pipelines/lib/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20383 2024-04-09 10:57:52.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-04-08 08:38:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    25699 2024-04-06 13:43:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6334 2024-03-19 22:25:46.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14093 2024-04-09 11:03:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10315 2024-03-04 21:14:19.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.398999 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/chem_comp.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/io.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/object_iter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/translator.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garyt      (501) staff       (20)    27949 2024-03-19 22:43:06.000000 nef_pipelines-0.1.63/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5431 2024-03-04 22:07:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/main.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.400174 nef_pipelines-0.1.63/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.422691 nef_pipelines-0.1.63/src/nef_pipelines/tests/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.464794 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.469297 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garyt      (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.472011 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.476999 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.478610 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.480853 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     3621 2024-04-07 09:20:05.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.481830 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.484450 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)     3405 2024-04-07 09:19:50.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.516218 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.518617 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_filter.py
+-rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr--r--   0 garyt      (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.522678 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.530526 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6221 2024-04-07 09:31:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.536613 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.601622 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garyt      (501) staff       (20)      840 2024-03-04 21:16:11.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4093 2024-02-10 20:35:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.066205 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.605535 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
+-rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.614314 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.650839 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2742 2024-02-10 18:10:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr--r--   0 garyt      (501) staff       (20)     3881 2023-08-24 07:58:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3847 2024-02-10 20:35:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.653952 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.657070 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.659373 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.712958 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
+-rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)     7860 2023-12-20 18:35:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4316 2023-12-20 18:23:05.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.714621 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7234 2024-04-08 08:37:44.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.716577 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.722403 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.774288 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4314 2024-04-07 09:31:37.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.780593 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.796020 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     5638 2023-11-05 11:38:38.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1877 2023-11-01 22:08:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_import_order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5825 2023-12-08 21:08:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_import_restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3282 2023-12-07 10:10:58.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_secondary_structure.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.803546 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/header.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_header.py
+-rwxr--r--   0 garyt      (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     7636 2024-04-06 13:42:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.804655 nef_pipelines-0.1.63/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.842418 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.845805 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
+-rw-r--r--   0 garyt      (501) staff       (20)     3392 2024-04-07 09:31:44.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8984 2024-03-27 21:18:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.852699 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.868984 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)     8138 2023-10-30 22:33:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6577 2023-10-30 08:28:29.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11089 2023-07-12 13:14:21.000000 nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.922281 nef_pipelines-0.1.63/src/nef_pipelines/tools/
+-rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.930211 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-03-04 21:23:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.933957 nef_pipelines-0.1.63/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.945927 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8838 2023-12-21 14:29:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/filter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-02-10 20:35:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8044 2024-04-09 11:39:47.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garyt      (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.950866 nef_pipelines-0.1.63/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/peaks/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.955217 nef_pipelines-0.1.63/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    12051 2024-04-09 11:02:16.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.956141 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:14.956774 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.019474 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.040416 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.042438 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.043300 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.046048 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.048581 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6680 2024-04-06 13:44:59.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.049660 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.055509 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garyt      (501) staff       (20)      826 2024-04-06 13:45:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5998 2024-04-06 13:45:32.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.058627 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11631 2024-04-06 16:51:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.062380 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.068592 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.072277 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)      682 2024-03-19 07:46:08.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.077438 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7952 2024-04-09 11:01:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/project.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5993 2024-03-19 07:42:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    24119 2024-03-15 17:31:35.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.080767 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.083959 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.117359 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16945 2023-11-21 22:15:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2313 2024-02-10 20:35:20.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5749 2023-12-20 19:52:03.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.119851 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.122863 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.127085 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.130590 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     4829 2023-12-20 18:35:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.131447 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.134266 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.136136 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.138852 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.142639 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.145404 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.150878 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9018 2024-03-27 21:44:50.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.153616 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.179797 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8157 2023-12-07 22:13:01.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.184902 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5134 2024-03-19 07:42:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/talos_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.186179 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.188762 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.193400 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.220780 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     2923 2024-03-27 21:18:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2852 2023-05-21 10:57:07.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.225937 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.227201 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.232220 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-09 11:41:15.233678 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garyt      (501) staff       (20)     9606 2024-04-09 11:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)    21038 2024-04-09 11:41:14.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2024-04-09 11:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       48 2024-04-09 11:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garyt      (501) staff       (20)      440 2024-04-09 11:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       19 2024-04-09 11:41:13.000000 nef_pipelines-0.1.63/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.63/tox.ini
```

### Comparing `nef_pipelines-0.1.62/.github/workflows/ci.yml` & `nef_pipelines-0.1.63/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.63/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/.pre-commit-config.yaml` & `nef_pipelines-0.1.63/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/CHANGELOG.md` & `nef_pipelines-0.1.63/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -257,8 +257,11 @@
 ## version 0.1.60
 - add support for c detect spectra for idps in peak simulation code
 
 ## version 0.1.61
 - use requests to download bmrb files from the web
 
 ## version 0.1.62
--use urllib3 <= / == 1.26.15 to avoid a security warning
+- use urllib3 <= / == 1.26.15 to avoid a security warning
+
+## version 0.1.63
+- remove dependance on Levenshtein which was causing compilation errors
```

### Comparing `nef_pipelines-0.1.62/CONTRIBUTING.md` & `nef_pipelines-0.1.63/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/LICENSE.txt` & `nef_pipelines-0.1.63/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/PKG-INFO` & `nef_pipelines-0.1.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.62
+Version: 0.1.63
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -17,15 +17,14 @@
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: click==8.1.3
 Requires-Dist: f-yeah==0.3.0
 Requires-Dist: fastaparser==1.1.1
 Requires-Dist: freezegun==1.1.0
 Requires-Dist: frozendict==2.3.7
 Requires-Dist: hjson==3.1.0
-Requires-Dist: Levenshtein==0.20.9
 Requires-Dist: mmcif-pdbx==2.0.1
 Requires-Dist: ordered-set==4.1.0
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: pynmrstar==3.3.2
 Requires-Dist: pyparsing==3.0.8
 Requires-Dist: pytest==7.1.3
 Requires-Dist: pytest-mock==3.12.0
```

### Comparing `nef_pipelines-0.1.62/README.md` & `nef_pipelines-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/TODO.md` & `nef_pipelines-0.1.63/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.63/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.63/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/references/kosol idps molecules-18-10802.pdf` & `nef_pipelines-0.1.63/references/kosol idps molecules-18-10802.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/release_to_pypi.sh` & `nef_pipelines-0.1.63/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/setup.cfg` & `nef_pipelines-0.1.63/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 	cachetools==5.3.3
 	click==8.1.3
 	f-yeah==0.3.0
 	fastaparser==1.1.1
 	freezegun==1.1.0
 	frozendict==2.3.7
 	hjson==3.1.0
-	Levenshtein==0.20.9
 	mmcif-pdbx==2.0.1
 	ordered-set==4.1.0
 	pydantic==2.6.3
 	pynmrstar==3.3.2
 	pyparsing==3.0.8
 	pytest==7.1.3
 	pytest-mock==3.12.0
```

### Comparing `nef_pipelines-0.1.62/setup.py` & `nef_pipelines-0.1.63/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/ambiguity_translations.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/ambiguity_translations.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json` & `nef_pipelines-0.1.63/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.63/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/chem_comp.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/chem_comp.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/io.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/io.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/object_iter.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/object_iter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/translation/translator.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/translation/translator.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.63/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/main.py` & `nef_pipelines-0.1.63/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/frames/test_unassign.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/frames/test_unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/rcsb/test_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/rcsb/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/predSS_4.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/predSS_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/protonated_his.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/protonated_his.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/ubi_4.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/ubi_4.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_export_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_import_order_parameters.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_import_order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_import_restraints.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_import_restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/talos/test_secondary_structure.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/talos/test_secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/filter.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/filter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/rename.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
+from difflib import SequenceMatcher
 from fnmatch import fnmatch
 from pathlib import Path
 from textwrap import dedent, indent
 from typing import List
 
 import typer
 from fyeah import f
-from Levenshtein import distance
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
 from nef_pipelines.lib.util import (
@@ -197,21 +197,27 @@
             there were no frames in the entry to rename
         """
     else:
         category_msg = (
             "" if target_category == "*" else f" with category {target_category}"
         )
         category_msg = category_msg
-        distances = [
-            (
-                distance(name, target_name) + distance(target_category, category),
-                (name, category),
-            )
-            for name, category in all_names_and_categories
-        ]
+        matcher = SequenceMatcher()
+        distances = []
+        for name, category in all_names_and_categories:
+            matcher.set_seq1(name)
+            matcher.set_seq2(target_name)
+            distance_name = 1.0 - matcher.ratio()
+
+            matcher.set_seq1(target_category)
+            matcher.set_seq2(category)
+            distance_category = 1.0 - matcher.ratio()
+            distance = (distance_name + distance_category) / 2.0
+        distances.append((distance, (name, category)))
+
         distances.sort()
 
         all_names = [name for name, _ in all_names_and_categories]
         table = strings_to_table_terminal_sensitive(all_names)
         table = tabulate(table, tablefmt="plain")
         table = indent(dedent(table), FOUR_SPACES)
```

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/frames/unassign.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/frames/unassign.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.63/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/project.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/project.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/order_parameters.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/order_parameters.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/restraints.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/talos/talos_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/talos/talos_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.63/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.63/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.62
+Version: 0.1.63
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -17,15 +17,14 @@
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: click==8.1.3
 Requires-Dist: f-yeah==0.3.0
 Requires-Dist: fastaparser==1.1.1
 Requires-Dist: freezegun==1.1.0
 Requires-Dist: frozendict==2.3.7
 Requires-Dist: hjson==3.1.0
-Requires-Dist: Levenshtein==0.20.9
 Requires-Dist: mmcif-pdbx==2.0.1
 Requires-Dist: ordered-set==4.1.0
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: pynmrstar==3.3.2
 Requires-Dist: pyparsing==3.0.8
 Requires-Dist: pytest==7.1.3
 Requires-Dist: pytest-mock==3.12.0
```

### Comparing `nef_pipelines-0.1.62/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.63/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.62/tox.ini` & `nef_pipelines-0.1.63/tox.ini`

 * *Files identical despite different names*

