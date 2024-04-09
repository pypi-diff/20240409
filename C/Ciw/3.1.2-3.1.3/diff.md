# Comparing `tmp/Ciw-3.1.2.tar.gz` & `tmp/Ciw-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ciw-3.1.2.tar", last modified: Mon Apr  8 14:23:19 2024, max compression
+gzip compressed data, was "Ciw-3.1.3.tar", last modified: Mon Apr  8 22:21:29 2024, max compression
```

## Comparing `Ciw-3.1.2.tar` & `Ciw-3.1.3.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:19.025698 Ciw-3.1.2/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       43 2019-10-02 14:24:32.000000 Ciw-3.1.2/.gitattributes
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.686376 Ciw-3.1.2/.github/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.708358 Ciw-3.1.2/.github/workflows/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1192 2023-08-22 13:40:54.000000 Ciw-3.1.2/.github/workflows/tests.yml
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      149 2023-08-22 13:40:54.000000 Ciw-3.1.2/.gitignore
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      733 2023-08-16 14:03:09.000000 Ciw-3.1.2/.readthedocs.yaml
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      984 2023-10-31 15:56:51.000000 Ciw-3.1.2/AUTHORS.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     9600 2024-04-08 14:14:49.000000 Ciw-3.1.2/CHANGES.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      597 2019-10-02 14:24:32.000000 Ciw-3.1.2/CITATION.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1514 2023-08-16 14:03:09.000000 Ciw-3.1.2/CONTRIBUTING.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:19.021882 Ciw-3.1.2/Ciw.egg-info/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14828 2024-04-08 14:23:18.000000 Ciw-3.1.2/Ciw.egg-info/PKG-INFO
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7189 2024-04-08 14:23:18.000000 Ciw-3.1.2/Ciw.egg-info/SOURCES.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        1 2024-04-08 14:23:18.000000 Ciw-3.1.2/Ciw.egg-info/dependency_links.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2024-04-08 14:23:18.000000 Ciw-3.1.2/Ciw.egg-info/requires.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        4 2024-04-08 14:23:18.000000 Ciw-3.1.2/Ciw.egg-info/top_level.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1080 2019-10-02 14:24:32.000000 Ciw-3.1.2/LICENSE.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       56 2019-10-02 14:24:32.000000 Ciw-3.1.2/MANIFEST.in
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14828 2024-04-08 14:23:19.024537 Ciw-3.1.2/PKG-INFO
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3854 2023-12-03 11:49:12.000000 Ciw-3.1.2/README.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.737197 Ciw-3.1.2/ciw/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      575 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     6681 2024-04-04 09:45:57.000000 Ciw-3.1.2/ciw/arrival_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1770 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/auxiliary.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      498 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/data_record.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.738880 Ciw-3.1.2/ciw/deadlock/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/deadlock/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4446 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/deadlock/deadlock_detector.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1361 2024-04-04 12:54:15.000000 Ciw-3.1.2/ciw/disciplines.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.740600 Ciw-3.1.2/ciw/dists/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.689608 Ciw-3.1.2/ciw/dists/.hypothesis/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.689333 Ciw-3.1.2/ciw/dists/.hypothesis/examples/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.774352 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/097e547b92b91adb
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/0af454191959d613
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/1189a64b3a63541c
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/12acac2df3df48b6
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/24d6e7fc3069832b
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/4da15fd7a09586c7
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/550f5aa3832b4fc3
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/628039b293dd5254
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/668938c233269c64
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/7db861381701d4e1
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/7fc1725f753ed55f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/9c29b872c797bf63
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       49 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/9d0de032dbc8ead3
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/b20d02d8f503a893
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/d08fa35e321f216d
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/d3be39602ef9c5c4
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/d8cccc4895f8a7c0
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/1a542554bc6caead/de3c78fe5b956e64
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.817033 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2823a3eaa9e3c5ba
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       28 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2a4930297c79ff33
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2cfb623d346ecd57
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2dbf20c932203d22
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/406bbe627cd1c44f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/4119c7a3257670d6
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/44f025d4566fcf0c
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/48d7a891c63260e5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5bde08a3480d1870
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5cbee9898702bbf5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      197 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5d8a93fd16b829b5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5e86df951ef52a16
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/601bbc65f8304262
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/7cd123fe7f4978f8
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/852cb323bed40f7d
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/b15db0ff5f98ebc2
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       37 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ba81a7b179458d39
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c3263c7fd9b5885f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c6327af1d657f71b
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c7d326df3641c9fe
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/d4a3e75cd97512cf
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/da68315e076fdb9e
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/df6ee214f7db1f01
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/dfd06dd224d1ba64
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ef3bdf5c7f89578a
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f4cb653a6cb0fe75
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f7823ac27f9552ef
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.689803 Ciw-3.1.2/ciw/dists/.hypothesis/unicodedata/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.818682 Ciw-3.1.2/ciw/dists/.hypothesis/unicodedata/8.0.0/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15457 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/dists/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    22936 2024-04-08 14:10:07.000000 Ciw-3.1.2/ciw/dists/distributions.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1896 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/exactnode.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1046 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/exit_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    16020 2024-04-03 14:32:52.000000 Ciw-3.1.2/ciw/import_params.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4108 2023-12-01 23:16:34.000000 Ciw-3.1.2/ciw/individual.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3663 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/network.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    42145 2024-04-04 12:54:15.000000 Ciw-3.1.2/ciw/node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4045 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/processor_sharing.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2024-04-03 14:32:52.000000 Ciw-3.1.2/ciw/schedules.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      851 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/server.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    11587 2023-12-03 01:41:53.000000 Ciw-3.1.2/ciw/simulation.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.846628 Ciw-3.1.2/ciw/tests/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        0 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/tests/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    21026 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/tests/test_arrival_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3536 2023-08-22 13:40:54.000000 Ciw-3.1.2/ciw/tests/test_auxiliary.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5651 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_data_record.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1584 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_exit_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5146 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_individual.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    43757 2024-04-03 14:32:52.000000 Ciw-3.1.2/ciw/tests/test_network.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    86319 2024-04-04 12:54:15.000000 Ciw-3.1.2/ciw/tests/test_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    10518 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_process_based.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    31330 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/tests/test_processor_sharing.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    67284 2024-04-03 14:32:52.000000 Ciw-3.1.2/ciw/tests/test_sampling.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    38735 2023-12-03 11:30:34.000000 Ciw-3.1.2/ciw/tests/test_scheduling.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5029 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_server.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    55060 2024-04-04 12:54:15.000000 Ciw-3.1.2/ciw/tests/test_simulation.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    70650 2023-08-22 13:40:55.000000 Ciw-3.1.2/ciw/tests/test_state_tracker.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      193 2023-08-17 16:01:41.000000 Ciw-3.1.2/ciw/tests/test_version.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.848664 Ciw-3.1.2/ciw/trackers/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.2/ciw/trackers/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14360 2024-04-03 14:32:52.000000 Ciw-3.1.2/ciw/trackers/state_tracker.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       22 2024-04-08 14:14:14.000000 Ciw-3.1.2/ciw/version.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.855248 Ciw-3.1.2/docs/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.866235 Ciw-3.1.2/docs/Background/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      482 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Background/codestructure.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      177 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Background/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2071 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Background/kendall.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3038 2023-11-14 12:21:00.000000 Ciw-3.1.2/docs/Background/mechanisms.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      910 2024-04-03 14:32:52.000000 Ciw-3.1.2/docs/Background/other.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      658 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Background/references.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3482 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Background/simulationpractice.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.929859 Ciw-3.1.2/docs/Guides/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3866 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/batching.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2991 2024-04-04 12:54:09.000000 Ciw-3.1.2/docs/Guides/baulking.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.939057 Ciw-3.1.2/docs/Guides/behaviour/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3160 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/behaviour/custom_arrivals.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3330 2023-12-03 11:30:34.000000 Ciw-3.1.2/docs/Guides/behaviour/custom_number_servers.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3932 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/behaviour/custom_routing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8332 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/behaviour/hybrid.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1606 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/behaviour/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3322 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/behaviour/ps_routing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4590 2023-08-17 09:42:42.000000 Ciw-3.1.2/docs/Guides/behaviour/server_dependent_dist.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2575 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/change-class-after-service.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4157 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/change-class-while-queueing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2377 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/deadlock.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      525 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/dynamic_customerclasses.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1707 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/exact.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      619 2023-12-03 11:30:34.000000 Ciw-3.1.2/docs/Guides/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2393 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/parallel_process.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2121 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/pause_restart.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7318 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/phasetype.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2023-12-03 11:30:34.000000 Ciw-3.1.2/docs/Guides/preemption.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2810 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/priority.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4600 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/process_based.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7125 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/processor-sharing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1144 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Guides/progressbar.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4376 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/reneging.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1524 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/seed.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5564 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/server_priority.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3251 2023-12-03 11:30:34.000000 Ciw-3.1.2/docs/Guides/server_schedule.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3504 2024-04-04 12:54:15.000000 Ciw-3.1.2/docs/Guides/service_disciplines.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8988 2024-04-03 14:32:52.000000 Ciw-3.1.2/docs/Guides/set_distributions.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2115 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/sim_numcusts.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3880 2023-12-03 11:30:34.000000 Ciw-3.1.2/docs/Guides/slotted.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3080 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Guides/state_trackers.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     9506 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Guides/time_dependent.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7413 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Makefile
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.947894 Ciw-3.1.2/docs/Reference/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       69 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Reference/authors.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       78 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Reference/changelog.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1494 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Reference/citation.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      109 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Reference/contributing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    10862 2024-04-03 14:32:52.000000 Ciw-3.1.2/docs/Reference/distributions.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3561 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Reference/glossary.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      225 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Reference/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     6083 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Reference/parameters.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3254 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Reference/results.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5378 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Reference/state_trackers.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.952367 Ciw-3.1.2/docs/Tutorial-I/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      237 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Tutorial-I/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3004 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Tutorial-I/tutorial_i.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2993 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/Tutorial-I/tutorial_ii.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3339 2023-11-14 12:21:00.000000 Ciw-3.1.2/docs/Tutorial-I/tutorial_iii.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4434 2023-11-14 12:22:13.000000 Ciw-3.1.2/docs/Tutorial-I/tutorial_iv.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:18.956017 Ciw-3.1.2/docs/Tutorial-II/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      320 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/Tutorial-II/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4708 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Tutorial-II/tutorial_v.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5637 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Tutorial-II/tutorial_vi.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5535 2023-08-22 13:40:55.000000 Ciw-3.1.2/docs/Tutorial-II/tutorial_vii.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:19.014498 Ciw-3.1.2/docs/_static/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    17655 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/2nodes.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)   116215 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/2nodesindeadlock.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14663 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/cafe.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    65346 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/codestructure.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4968 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/codestructure.tex
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    27837 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/coxian.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15838 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/custom_number_servers_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    16887 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/custom_number_servers_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    74719 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/custom_routing_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    71055 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/custom_routing_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    95903 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/des+sd_hybrid.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8422 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/erlang.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4286 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/favicon.ico
--rw-r--r--   0 geraintpalmer   (502) staff       (20)   207124 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/hybrid.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    46236 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/hypererlang.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15698 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/hyperexponential.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2603 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/logo.pdf
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8889 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/logo.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1561 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/logo.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7299 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/logo_small.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    20608 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/phasetype.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    21468 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/progress_bar_customers.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    22909 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/progress_bar_time.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    32489 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/ps_capacitated_verification.svg
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 14:23:19.018947 Ciw-3.1.2/docs/_static/script_for_parallel_processing/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      214 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/script_for_parallel_processing/README.md
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      823 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/script_for_parallel_processing/main.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    48896 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/server_dependent_dist_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    37013 2023-08-16 14:03:09.000000 Ciw-3.1.2/docs/_static/server_dependent_dist_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      194 2023-08-22 16:10:56.000000 Ciw-3.1.2/docs/_static/style.css
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14539 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/_static/tutorial_iii_waitshist.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    10027 2023-08-22 16:30:04.000000 Ciw-3.1.2/docs/conf.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      891 2023-12-03 11:38:09.000000 Ciw-3.1.2/docs/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      299 2019-10-02 14:24:32.000000 Ciw-3.1.2/docs/installation.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       20 2024-04-03 14:32:52.000000 Ciw-3.1.2/docs/requirements.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      492 2023-08-22 13:40:55.000000 Ciw-3.1.2/doctests.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      322 2023-08-16 14:03:09.000000 Ciw-3.1.2/new_release_checklist.md
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       40 2023-08-22 13:40:55.000000 Ciw-3.1.2/requirements.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       38 2024-04-08 14:23:19.025997 Ciw-3.1.2/setup.cfg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      956 2023-08-22 13:40:55.000000 Ciw-3.1.2/setup.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       55 2023-08-22 13:40:55.000000 Ciw-3.1.2/test_requirements.txt
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.232802 Ciw-3.1.3/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       43 2019-10-02 14:24:32.000000 Ciw-3.1.3/.gitattributes
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.937579 Ciw-3.1.3/.github/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.965257 Ciw-3.1.3/.github/workflows/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1192 2023-08-22 13:40:54.000000 Ciw-3.1.3/.github/workflows/tests.yml
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      149 2023-08-22 13:40:54.000000 Ciw-3.1.3/.gitignore
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      733 2023-08-16 14:03:09.000000 Ciw-3.1.3/.readthedocs.yaml
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      984 2023-10-31 15:56:51.000000 Ciw-3.1.3/AUTHORS.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     9705 2024-04-08 22:11:06.000000 Ciw-3.1.3/CHANGES.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      597 2019-10-02 14:24:32.000000 Ciw-3.1.3/CITATION.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1514 2023-08-16 14:03:09.000000 Ciw-3.1.3/CONTRIBUTING.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.230221 Ciw-3.1.3/Ciw.egg-info/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14933 2024-04-08 22:21:28.000000 Ciw-3.1.3/Ciw.egg-info/PKG-INFO
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7189 2024-04-08 22:21:28.000000 Ciw-3.1.3/Ciw.egg-info/SOURCES.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        1 2024-04-08 22:21:28.000000 Ciw-3.1.3/Ciw.egg-info/dependency_links.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2024-04-08 22:21:28.000000 Ciw-3.1.3/Ciw.egg-info/requires.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        4 2024-04-08 22:21:28.000000 Ciw-3.1.3/Ciw.egg-info/top_level.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1080 2019-10-02 14:24:32.000000 Ciw-3.1.3/LICENSE.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       56 2019-10-02 14:24:32.000000 Ciw-3.1.3/MANIFEST.in
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14933 2024-04-08 22:21:29.231591 Ciw-3.1.3/PKG-INFO
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3854 2023-12-03 11:49:12.000000 Ciw-3.1.3/README.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.982626 Ciw-3.1.3/ciw/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      575 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6681 2024-04-04 09:45:57.000000 Ciw-3.1.3/ciw/arrival_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1770 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/auxiliary.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      498 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/data_record.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.984329 Ciw-3.1.3/ciw/deadlock/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/deadlock/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4446 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/deadlock/deadlock_detector.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1361 2024-04-04 12:54:15.000000 Ciw-3.1.3/ciw/disciplines.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.986260 Ciw-3.1.3/ciw/dists/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.940182 Ciw-3.1.3/ciw/dists/.hypothesis/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.939898 Ciw-3.1.3/ciw/dists/.hypothesis/examples/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.013291 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/097e547b92b91adb
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/0af454191959d613
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/1189a64b3a63541c
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/12acac2df3df48b6
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/24d6e7fc3069832b
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/4da15fd7a09586c7
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/550f5aa3832b4fc3
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/628039b293dd5254
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/668938c233269c64
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/7db861381701d4e1
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/7fc1725f753ed55f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/9c29b872c797bf63
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       49 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/9d0de032dbc8ead3
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/b20d02d8f503a893
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/d08fa35e321f216d
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/d3be39602ef9c5c4
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/d8cccc4895f8a7c0
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/1a542554bc6caead/de3c78fe5b956e64
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.055021 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2823a3eaa9e3c5ba
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       28 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2a4930297c79ff33
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2cfb623d346ecd57
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2dbf20c932203d22
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/406bbe627cd1c44f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/4119c7a3257670d6
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/44f025d4566fcf0c
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/48d7a891c63260e5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5bde08a3480d1870
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5cbee9898702bbf5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      197 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5d8a93fd16b829b5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5e86df951ef52a16
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/601bbc65f8304262
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/7cd123fe7f4978f8
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/852cb323bed40f7d
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/b15db0ff5f98ebc2
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       37 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ba81a7b179458d39
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c3263c7fd9b5885f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c6327af1d657f71b
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c7d326df3641c9fe
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/d4a3e75cd97512cf
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/da68315e076fdb9e
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/df6ee214f7db1f01
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/dfd06dd224d1ba64
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ef3bdf5c7f89578a
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f4cb653a6cb0fe75
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f7823ac27f9552ef
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:28.940427 Ciw-3.1.3/ciw/dists/.hypothesis/unicodedata/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.057016 Ciw-3.1.3/ciw/dists/.hypothesis/unicodedata/8.0.0/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15457 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/dists/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    22936 2024-04-08 14:10:07.000000 Ciw-3.1.3/ciw/dists/distributions.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1896 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/exactnode.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1046 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/exit_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16230 2024-04-08 22:07:37.000000 Ciw-3.1.3/ciw/import_params.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4108 2023-12-01 23:16:34.000000 Ciw-3.1.3/ciw/individual.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3663 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/network.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    42145 2024-04-04 12:54:15.000000 Ciw-3.1.3/ciw/node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4045 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/processor_sharing.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2024-04-03 14:32:52.000000 Ciw-3.1.3/ciw/schedules.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      851 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/server.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    11587 2023-12-03 01:41:53.000000 Ciw-3.1.3/ciw/simulation.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.074251 Ciw-3.1.3/ciw/tests/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        0 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/tests/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    21026 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/tests/test_arrival_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3536 2023-08-22 13:40:54.000000 Ciw-3.1.3/ciw/tests/test_auxiliary.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5651 2023-08-22 13:40:55.000000 Ciw-3.1.3/ciw/tests/test_data_record.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1584 2023-08-22 13:40:55.000000 Ciw-3.1.3/ciw/tests/test_exit_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5146 2023-08-22 13:40:55.000000 Ciw-3.1.3/ciw/tests/test_individual.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    43757 2024-04-03 14:32:52.000000 Ciw-3.1.3/ciw/tests/test_network.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    86319 2024-04-04 12:54:15.000000 Ciw-3.1.3/ciw/tests/test_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    11284 2024-04-08 22:04:49.000000 Ciw-3.1.3/ciw/tests/test_process_based.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    31330 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/tests/test_processor_sharing.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    67284 2024-04-03 14:32:52.000000 Ciw-3.1.3/ciw/tests/test_sampling.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    38735 2023-12-03 11:30:34.000000 Ciw-3.1.3/ciw/tests/test_scheduling.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5029 2023-08-22 13:40:55.000000 Ciw-3.1.3/ciw/tests/test_server.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    55060 2024-04-04 12:54:15.000000 Ciw-3.1.3/ciw/tests/test_simulation.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    70650 2023-08-22 13:40:55.000000 Ciw-3.1.3/ciw/tests/test_state_tracker.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      193 2023-08-17 16:01:41.000000 Ciw-3.1.3/ciw/tests/test_version.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.076101 Ciw-3.1.3/ciw/trackers/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.3/ciw/trackers/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14360 2024-04-03 14:32:52.000000 Ciw-3.1.3/ciw/trackers/state_tracker.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       22 2024-04-08 22:10:08.000000 Ciw-3.1.3/ciw/version.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.084935 Ciw-3.1.3/docs/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.100981 Ciw-3.1.3/docs/Background/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      482 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Background/codestructure.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      177 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Background/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2071 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Background/kendall.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3038 2023-11-14 12:21:00.000000 Ciw-3.1.3/docs/Background/mechanisms.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      910 2024-04-03 14:32:52.000000 Ciw-3.1.3/docs/Background/other.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      658 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Background/references.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3482 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Background/simulationpractice.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.147976 Ciw-3.1.3/docs/Guides/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3866 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/batching.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2991 2024-04-04 12:54:09.000000 Ciw-3.1.3/docs/Guides/baulking.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.155345 Ciw-3.1.3/docs/Guides/behaviour/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3160 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/behaviour/custom_arrivals.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3330 2023-12-03 11:30:34.000000 Ciw-3.1.3/docs/Guides/behaviour/custom_number_servers.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3932 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/behaviour/custom_routing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8332 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/behaviour/hybrid.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1606 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/behaviour/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3322 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/behaviour/ps_routing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4590 2023-08-17 09:42:42.000000 Ciw-3.1.3/docs/Guides/behaviour/server_dependent_dist.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2575 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/change-class-after-service.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4157 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/change-class-while-queueing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2377 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/deadlock.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      525 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/dynamic_customerclasses.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1707 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/exact.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      619 2023-12-03 11:30:34.000000 Ciw-3.1.3/docs/Guides/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2393 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/parallel_process.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2121 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/pause_restart.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7318 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/phasetype.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2023-12-03 11:30:34.000000 Ciw-3.1.3/docs/Guides/preemption.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2810 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/priority.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4600 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/process_based.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7125 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/processor-sharing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1144 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Guides/progressbar.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4376 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/reneging.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1524 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/seed.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5564 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/server_priority.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3251 2023-12-03 11:30:34.000000 Ciw-3.1.3/docs/Guides/server_schedule.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3504 2024-04-04 12:54:15.000000 Ciw-3.1.3/docs/Guides/service_disciplines.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8988 2024-04-03 14:32:52.000000 Ciw-3.1.3/docs/Guides/set_distributions.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2115 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/sim_numcusts.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3880 2023-12-03 11:30:34.000000 Ciw-3.1.3/docs/Guides/slotted.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3080 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Guides/state_trackers.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     9506 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Guides/time_dependent.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7413 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Makefile
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.171528 Ciw-3.1.3/docs/Reference/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       69 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Reference/authors.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       78 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Reference/changelog.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1494 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Reference/citation.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      109 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Reference/contributing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10862 2024-04-03 14:32:52.000000 Ciw-3.1.3/docs/Reference/distributions.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3561 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Reference/glossary.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      225 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Reference/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6083 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Reference/parameters.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3254 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Reference/results.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5378 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Reference/state_trackers.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.177794 Ciw-3.1.3/docs/Tutorial-I/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      237 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Tutorial-I/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3004 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Tutorial-I/tutorial_i.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2993 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/Tutorial-I/tutorial_ii.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3339 2023-11-14 12:21:00.000000 Ciw-3.1.3/docs/Tutorial-I/tutorial_iii.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4434 2023-11-14 12:22:13.000000 Ciw-3.1.3/docs/Tutorial-I/tutorial_iv.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.182190 Ciw-3.1.3/docs/Tutorial-II/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      320 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/Tutorial-II/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4708 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Tutorial-II/tutorial_v.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5637 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Tutorial-II/tutorial_vi.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5535 2023-08-22 13:40:55.000000 Ciw-3.1.3/docs/Tutorial-II/tutorial_vii.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.226774 Ciw-3.1.3/docs/_static/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    17655 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/2nodes.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)   116215 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/2nodesindeadlock.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14663 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/cafe.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    65346 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/codestructure.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4968 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/codestructure.tex
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    27837 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/coxian.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15838 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/custom_number_servers_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16887 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/custom_number_servers_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    74719 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/custom_routing_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    71055 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/custom_routing_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    95903 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/des+sd_hybrid.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8422 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/erlang.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4286 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)   207124 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/hybrid.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    46236 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/hypererlang.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15698 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/hyperexponential.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2603 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/logo.pdf
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8889 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/logo.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1561 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/logo.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7299 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/logo_small.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    20608 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/phasetype.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    21468 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/progress_bar_customers.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    22909 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/progress_bar_time.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    32489 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/ps_capacitated_verification.svg
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-08 22:21:29.228941 Ciw-3.1.3/docs/_static/script_for_parallel_processing/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      214 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/script_for_parallel_processing/README.md
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      823 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/script_for_parallel_processing/main.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    48896 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/server_dependent_dist_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    37013 2023-08-16 14:03:09.000000 Ciw-3.1.3/docs/_static/server_dependent_dist_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      194 2023-08-22 16:10:56.000000 Ciw-3.1.3/docs/_static/style.css
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14539 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/_static/tutorial_iii_waitshist.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10027 2023-08-22 16:30:04.000000 Ciw-3.1.3/docs/conf.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      891 2023-12-03 11:38:09.000000 Ciw-3.1.3/docs/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      299 2019-10-02 14:24:32.000000 Ciw-3.1.3/docs/installation.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       20 2024-04-03 14:32:52.000000 Ciw-3.1.3/docs/requirements.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      492 2023-08-22 13:40:55.000000 Ciw-3.1.3/doctests.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      322 2023-08-16 14:03:09.000000 Ciw-3.1.3/new_release_checklist.md
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       40 2023-08-22 13:40:55.000000 Ciw-3.1.3/requirements.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       38 2024-04-08 22:21:29.233087 Ciw-3.1.3/setup.cfg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      956 2023-08-22 13:40:55.000000 Ciw-3.1.3/setup.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       55 2023-08-22 13:40:55.000000 Ciw-3.1.3/test_requirements.txt
```

### Comparing `Ciw-3.1.2/.github/workflows/tests.yml` & `Ciw-3.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/.readthedocs.yaml` & `Ciw-3.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/AUTHORS.rst` & `Ciw-3.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/CHANGES.rst` & `Ciw-3.1.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 History
 -------
 
++ **3.1.3** (2024-04-08)**
+    + Allows class methods as generator functions for process-based routing.
+
 + **3.1.2 (2024-04-08)**
     + Fix bug when using Mixture distribution.
 
 + **3.1.1 (2024-04-04)**
     + Add a MixtureDistrubution that probabilistically chooses from a number of other distributions to sample from.
     + Baulking functions now take the simulation, current node, and current individual.
     + Service disciplines now take the current time.
```

### Comparing `Ciw-3.1.2/CITATION.rst` & `Ciw-3.1.3/CITATION.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/CONTRIBUTING.rst` & `Ciw-3.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/Ciw.egg-info/PKG-INFO` & `Ciw-3.1.3/Ciw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ciw
-Version: 3.1.2
+Version: 3.1.3
 Summary: A discrete event simulation library for open queueing networks
 Home-page: https://github.com/CiwPython/Ciw
 Author: Geraint Palmer, Vincent Knight
 Author-email: palmer.geraint@googlemail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: networkx>=2.3
@@ -109,14 +109,17 @@
 + `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/deadlock.html>`_
 
 
 
 History
 -------
 
++ **3.1.3** (2024-04-08)**
+    + Allows class methods as generator functions for process-based routing.
+
 + **3.1.2 (2024-04-08)**
     + Fix bug when using Mixture distribution.
 
 + **3.1.1 (2024-04-04)**
     + Add a MixtureDistrubution that probabilistically chooses from a number of other distributions to sample from.
     + Baulking functions now take the simulation, current node, and current individual.
     + Service disciplines now take the current time.
```

### Comparing `Ciw-3.1.2/Ciw.egg-info/SOURCES.txt` & `Ciw-3.1.3/Ciw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/LICENSE.txt` & `Ciw-3.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/PKG-INFO` & `Ciw-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ciw
-Version: 3.1.2
+Version: 3.1.3
 Summary: A discrete event simulation library for open queueing networks
 Home-page: https://github.com/CiwPython/Ciw
 Author: Geraint Palmer, Vincent Knight
 Author-email: palmer.geraint@googlemail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: networkx>=2.3
@@ -109,14 +109,17 @@
 + `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/deadlock.html>`_
 
 
 
 History
 -------
 
++ **3.1.3** (2024-04-08)**
+    + Allows class methods as generator functions for process-based routing.
+
 + **3.1.2 (2024-04-08)**
     + Fix bug when using Mixture distribution.
 
 + **3.1.1 (2024-04-04)**
     + Add a MixtureDistrubution that probabilistically chooses from a number of other distributions to sample from.
     + Baulking functions now take the simulation, current node, and current individual.
     + Service disciplines now take the current time.
```

### Comparing `Ciw-3.1.2/README.rst` & `Ciw-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/__init__.py` & `Ciw-3.1.3/ciw/__init__.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/arrival_node.py` & `Ciw-3.1.3/ciw/arrival_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/auxiliary.py` & `Ciw-3.1.3/ciw/auxiliary.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/deadlock/deadlock_detector.py` & `Ciw-3.1.3/ciw/deadlock/deadlock_detector.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/disciplines.py` & `Ciw-3.1.3/ciw/disciplines.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz` & `Ciw-3.1.3/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/dists/distributions.py` & `Ciw-3.1.3/ciw/dists/distributions.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/exactnode.py` & `Ciw-3.1.3/ciw/exactnode.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/exit_node.py` & `Ciw-3.1.3/ciw/exit_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/import_params.py` & `Ciw-3.1.3/ciw/import_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 preempt_priorities[nd],
                 params["ps_thresholds"][nd],
                 params["server_priority_functions"][nd],
                 params["service_disciplines"][nd],
             )
         )
     for clss_name in params['customer_class_names']:
-        if all(isinstance(f, types.FunctionType) for f in params["routing"]):
+        if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
             classes[clss_name] = CustomerClass(
                 params['arrival_distributions'][clss_name],
                 params['service_distributions'][clss_name],
                 params['routing'],
                 params["priority_classes"][clss_name],
                 params["baulking_functions"][clss_name],
                 params["batching_distributions"][clss_name],
@@ -136,15 +136,15 @@
                 params["baulking_functions"][clss_name],
                 params["batching_distributions"][clss_name],
                 params["reneging_time_distributions"][clss_name],
                 params["reneging_destinations"][clss_name],
                 class_change_time_distributions[clss_name],
             )
     n = Network(nodes, classes)
-    if all(isinstance(f, types.FunctionType) for f in params["routing"]):
+    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
         n.process_based = True
     else:
         n.process_based = False
     return n
 
 
 def fill_out_dictionary(params):
@@ -216,15 +216,15 @@
 
 
 def validify_dictionary(params):
     """
     Raises errors if there is something wrong with the
     parameters dictionary.
     """
-    if all(isinstance(f, types.FunctionType) for f in params["routing"]):
+    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
         consistant_num_classes = (
             params["number_of_classes"]
             == len(params["arrival_distributions"])
             == len(params["service_distributions"])
             == len(params["batching_distributions"])
             == len(params["reneging_time_distributions"])
             == len(params["reneging_destinations"])
@@ -237,15 +237,15 @@
             == len(params["routing"])
             == len(params["batching_distributions"])
             == len(params["reneging_time_distributions"])
             == len(params["reneging_destinations"])
         )
     if not consistant_num_classes:
         raise ValueError("Ensure consistant number of classes is used throughout.")
-    if all(isinstance(f, types.FunctionType) for f in params["routing"]):
+    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
         consistant_class_names = (
             set(params["arrival_distributions"])
             == set(params["service_distributions"])
             == set(params["batching_distributions"])
             == set(params["reneging_time_distributions"])
             == set(params["reneging_destinations"])
         )
@@ -262,15 +262,15 @@
             == len(params["service_distributions"])
             == len(params["batching_distributions"])
             == len(params["reneging_time_distributions"])
             == len(params["reneging_destinations"])
         )
     if not consistant_class_names:
         raise ValueError("Ensure consistant names for customer classes.")
-    if all(isinstance(f, types.FunctionType) for f in params["routing"]):
+    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
         num_nodes_count = (
             [params["number_of_nodes"]]
             + [len(obs) for obs in params["arrival_distributions"].values()]
             + [len(obs) for obs in params["service_distributions"].values()]
             + [len(obs) for obs in params["batching_distributions"].values()]
             + [len(obs) for obs in params["reneging_time_distributions"].values()]
             + [len(obs) for obs in params["reneging_destinations"].values()]
@@ -292,15 +292,15 @@
             + [len(params["number_of_servers"])]
             + [len(params["server_priority_functions"])]
             + [len(params["queue_capacities"])]
             + [len(params["service_disciplines"])]
         )
     if len(set(num_nodes_count)) != 1:
         raise ValueError("Ensure consistant number of nodes is used throughout.")
-    if not all(isinstance(f, types.FunctionType) for f in params["routing"]):
+    if not all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
         for clss in params["routing"].values():
             for row in clss:
                 if sum(row) > 1.0 or min(row) < 0.0 or max(row) > 1.0:
                     raise ValueError("Ensure that routing matrix is valid.")
     neg_numservers = any(
         [(isinstance(obs, int) and obs < 0) for obs in params["number_of_servers"]]
     )
```

### Comparing `Ciw-3.1.2/ciw/individual.py` & `Ciw-3.1.3/ciw/individual.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/network.py` & `Ciw-3.1.3/ciw/network.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/node.py` & `Ciw-3.1.3/ciw/node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/processor_sharing.py` & `Ciw-3.1.3/ciw/processor_sharing.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/schedules.py` & `Ciw-3.1.3/ciw/schedules.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/server.py` & `Ciw-3.1.3/ciw/server.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/simulation.py` & `Ciw-3.1.3/ciw/simulation.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_arrival_node.py` & `Ciw-3.1.3/ciw/tests/test_arrival_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_auxiliary.py` & `Ciw-3.1.3/ciw/tests/test_auxiliary.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_data_record.py` & `Ciw-3.1.3/ciw/tests/test_data_record.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_exit_node.py` & `Ciw-3.1.3/ciw/tests/test_exit_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_individual.py` & `Ciw-3.1.3/ciw/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_network.py` & `Ciw-3.1.3/ciw/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_node.py` & `Ciw-3.1.3/ciw/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_process_based.py` & `Ciw-3.1.3/ciw/tests/test_process_based.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
 
 def generator_function_8(ind):
     if ind.customer_class == 'Class 0':
         return [1]
     return [1, 1, 1]
 
+class ClassForProcessBasedMethod:
+    def __init__(self, n):
+        self.n = n
+    def generator_method(self, ind):
+        return [1, 1, 1]
+
 
 class TestProcessBased(unittest.TestCase):
     def test_network_takes_routing_function(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(1)],
             service_distributions=[ciw.dists.Exponential(2)],
             number_of_servers=[1],
@@ -290,7 +296,23 @@
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
         Q.simulate_until_max_customers(500, method="Finish")
         inds = Q.nodes[-1].all_individuals
         routes_counter = set([tuple([ind.customer_class, tuple(dr.node for dr in ind.data_records)]) for ind in inds])
         self.assertEqual(routes_counter, {('Class 1', (1, 1, 1)), ('Class 0', (1,))})
+
+    def test_process_based_takes_methods(self):
+        import types
+        G = ClassForProcessBasedMethod(5)
+        self.assertTrue(isinstance(G.generator_method, types.MethodType))
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Deterministic(1)],
+            service_distributions=[ciw.dists.Deterministic(1000)],
+            number_of_servers=[1],
+            routing=[G.generator_method],
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(4.5)
+        inds = Q.nodes[1].all_individuals
+        for ind in inds:
+            self.assertEqual(ind.route, [1, 1, 1])
```

### Comparing `Ciw-3.1.2/ciw/tests/test_processor_sharing.py` & `Ciw-3.1.3/ciw/tests/test_processor_sharing.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_sampling.py` & `Ciw-3.1.3/ciw/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_scheduling.py` & `Ciw-3.1.3/ciw/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_server.py` & `Ciw-3.1.3/ciw/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_simulation.py` & `Ciw-3.1.3/ciw/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/tests/test_state_tracker.py` & `Ciw-3.1.3/ciw/tests/test_state_tracker.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/ciw/trackers/state_tracker.py` & `Ciw-3.1.3/ciw/trackers/state_tracker.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Background/kendall.rst` & `Ciw-3.1.3/docs/Background/kendall.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Background/mechanisms.rst` & `Ciw-3.1.3/docs/Background/mechanisms.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Background/other.rst` & `Ciw-3.1.3/docs/Background/other.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Background/references.rst` & `Ciw-3.1.3/docs/Background/references.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Background/simulationpractice.rst` & `Ciw-3.1.3/docs/Background/simulationpractice.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/batching.rst` & `Ciw-3.1.3/docs/Guides/batching.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/baulking.rst` & `Ciw-3.1.3/docs/Guides/baulking.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/custom_arrivals.rst` & `Ciw-3.1.3/docs/Guides/behaviour/custom_arrivals.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/custom_number_servers.rst` & `Ciw-3.1.3/docs/Guides/behaviour/custom_number_servers.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/custom_routing.rst` & `Ciw-3.1.3/docs/Guides/behaviour/custom_routing.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/hybrid.rst` & `Ciw-3.1.3/docs/Guides/behaviour/hybrid.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/index.rst` & `Ciw-3.1.3/docs/Guides/behaviour/index.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/ps_routing.rst` & `Ciw-3.1.3/docs/Guides/behaviour/ps_routing.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/behaviour/server_dependent_dist.rst` & `Ciw-3.1.3/docs/Guides/behaviour/server_dependent_dist.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/change-class-after-service.rst` & `Ciw-3.1.3/docs/Guides/change-class-after-service.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/change-class-while-queueing.rst` & `Ciw-3.1.3/docs/Guides/change-class-while-queueing.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/deadlock.rst` & `Ciw-3.1.3/docs/Guides/deadlock.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/dynamic_customerclasses.rst` & `Ciw-3.1.3/docs/Guides/dynamic_customerclasses.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/exact.rst` & `Ciw-3.1.3/docs/Guides/exact.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/index.rst` & `Ciw-3.1.3/docs/Guides/index.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/parallel_process.rst` & `Ciw-3.1.3/docs/Guides/parallel_process.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/pause_restart.rst` & `Ciw-3.1.3/docs/Guides/pause_restart.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/phasetype.rst` & `Ciw-3.1.3/docs/Guides/phasetype.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/preemption.rst` & `Ciw-3.1.3/docs/Guides/preemption.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/priority.rst` & `Ciw-3.1.3/docs/Guides/priority.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/process_based.rst` & `Ciw-3.1.3/docs/Guides/process_based.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/processor-sharing.rst` & `Ciw-3.1.3/docs/Guides/processor-sharing.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/progressbar.rst` & `Ciw-3.1.3/docs/Guides/progressbar.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/reneging.rst` & `Ciw-3.1.3/docs/Guides/reneging.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/seed.rst` & `Ciw-3.1.3/docs/Guides/seed.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/server_priority.rst` & `Ciw-3.1.3/docs/Guides/server_priority.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/server_schedule.rst` & `Ciw-3.1.3/docs/Guides/server_schedule.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/service_disciplines.rst` & `Ciw-3.1.3/docs/Guides/service_disciplines.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/set_distributions.rst` & `Ciw-3.1.3/docs/Guides/set_distributions.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/sim_numcusts.rst` & `Ciw-3.1.3/docs/Guides/sim_numcusts.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/slotted.rst` & `Ciw-3.1.3/docs/Guides/slotted.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/state_trackers.rst` & `Ciw-3.1.3/docs/Guides/state_trackers.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Guides/time_dependent.rst` & `Ciw-3.1.3/docs/Guides/time_dependent.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Makefile` & `Ciw-3.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/citation.rst` & `Ciw-3.1.3/docs/Reference/citation.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/distributions.rst` & `Ciw-3.1.3/docs/Reference/distributions.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/glossary.rst` & `Ciw-3.1.3/docs/Reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/parameters.rst` & `Ciw-3.1.3/docs/Reference/parameters.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/results.rst` & `Ciw-3.1.3/docs/Reference/results.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Reference/state_trackers.rst` & `Ciw-3.1.3/docs/Reference/state_trackers.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-I/tutorial_i.rst` & `Ciw-3.1.3/docs/Tutorial-I/tutorial_i.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-I/tutorial_ii.rst` & `Ciw-3.1.3/docs/Tutorial-I/tutorial_ii.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-I/tutorial_iii.rst` & `Ciw-3.1.3/docs/Tutorial-I/tutorial_iii.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-I/tutorial_iv.rst` & `Ciw-3.1.3/docs/Tutorial-I/tutorial_iv.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-II/tutorial_v.rst` & `Ciw-3.1.3/docs/Tutorial-II/tutorial_v.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-II/tutorial_vi.rst` & `Ciw-3.1.3/docs/Tutorial-II/tutorial_vi.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/Tutorial-II/tutorial_vii.rst` & `Ciw-3.1.3/docs/Tutorial-II/tutorial_vii.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/2nodes.svg` & `Ciw-3.1.3/docs/_static/2nodes.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/2nodesindeadlock.svg` & `Ciw-3.1.3/docs/_static/2nodesindeadlock.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/cafe.svg` & `Ciw-3.1.3/docs/_static/cafe.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/codestructure.svg` & `Ciw-3.1.3/docs/_static/codestructure.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/codestructure.tex` & `Ciw-3.1.3/docs/_static/codestructure.tex`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/coxian.svg` & `Ciw-3.1.3/docs/_static/coxian.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/custom_number_servers_with.svg` & `Ciw-3.1.3/docs/_static/custom_number_servers_with.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/custom_number_servers_without.svg` & `Ciw-3.1.3/docs/_static/custom_number_servers_without.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/custom_routing_with.svg` & `Ciw-3.1.3/docs/_static/custom_routing_with.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/custom_routing_without.svg` & `Ciw-3.1.3/docs/_static/custom_routing_without.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/des+sd_hybrid.svg` & `Ciw-3.1.3/docs/_static/des+sd_hybrid.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/erlang.svg` & `Ciw-3.1.3/docs/_static/erlang.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/favicon.ico` & `Ciw-3.1.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/hybrid.png` & `Ciw-3.1.3/docs/_static/hybrid.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/hypererlang.svg` & `Ciw-3.1.3/docs/_static/hypererlang.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/hyperexponential.svg` & `Ciw-3.1.3/docs/_static/hyperexponential.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/logo.pdf` & `Ciw-3.1.3/docs/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/logo.png` & `Ciw-3.1.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/logo.svg` & `Ciw-3.1.3/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/logo_small.png` & `Ciw-3.1.3/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/phasetype.svg` & `Ciw-3.1.3/docs/_static/phasetype.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/progress_bar_customers.png` & `Ciw-3.1.3/docs/_static/progress_bar_customers.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/progress_bar_time.png` & `Ciw-3.1.3/docs/_static/progress_bar_time.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/ps_capacitated_verification.svg` & `Ciw-3.1.3/docs/_static/ps_capacitated_verification.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/script_for_parallel_processing/main.py` & `Ciw-3.1.3/docs/_static/script_for_parallel_processing/main.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/server_dependent_dist_with.svg` & `Ciw-3.1.3/docs/_static/server_dependent_dist_with.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/server_dependent_dist_without.svg` & `Ciw-3.1.3/docs/_static/server_dependent_dist_without.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/_static/tutorial_iii_waitshist.svg` & `Ciw-3.1.3/docs/_static/tutorial_iii_waitshist.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/conf.py` & `Ciw-3.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/docs/index.rst` & `Ciw-3.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.2/setup.py` & `Ciw-3.1.3/setup.py`

 * *Files identical despite different names*

