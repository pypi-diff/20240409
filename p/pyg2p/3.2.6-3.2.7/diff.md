# Comparing `tmp/pyg2p-3.2.6.tar.gz` & `tmp/pyg2p-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyg2p-3.2.6.tar", last modified: Fri Sep  1 10:03:46 2023, max compression
+gzip compressed data, was "dist/pyg2p-3.2.7.tar", last modified: Tue Apr  9 10:17:02 2024, max compression
```

## Comparing `pyg2p-3.2.6.tar` & `pyg2p-3.2.7.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-09-01 09:51:26.000000 pyg2p-3.2.6/LICENSE
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-09-01 09:51:26.000000 pyg2p-3.2.6/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    48250 2023-09-01 10:03:46.000000 pyg2p-3.2.6/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    47255 2023-09-01 09:51:26.000000 pyg2p-3.2.6/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/bin/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-09-01 09:51:26.000000 pyg2p-3.2.6/bin/pyg2p
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/configuration/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/geopotentials.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/configuration/global/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3225 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/geopotentials.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/global_conf.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    42231 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8250 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/global/test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-09-01 09:51:26.000000 pyg2p-3.2.6/configuration/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      201 2023-09-01 09:51:26.000000 pyg2p-3.2.6/requirements.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-09-01 10:03:46.000000 pyg2p-3.2.6/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7116 2023-09-01 09:55:43.000000 pyg2p-3.2.6/setup.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-09-01 09:55:55.000000 pyg2p-3.2.6/src/pyg2p/VERSION
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7672 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/exceptions.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/main/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    15783 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/config.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    23098 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/context.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/controller.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/main/interpolation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    21232 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/interpolation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/interpolation/grib_interpolation_lib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/interpolation/latlong.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    62427 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/main/manipulation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/manipulation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13758 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/manipulation/aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/manipulation/conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/manipulation/correction.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/main/readers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/readers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11905 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/readers/grib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3011 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/readers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/readers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/main/writers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/writers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/writers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2012 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/main/writers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/util/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/files.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/generics.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/numeric.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p/util/profiling/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/profiling/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/profiling/profilehooks.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p/util/strings.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    48250 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4423 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-09-01 09:56:56.000000 pyg2p-3.2.6/src/pyg2p.egg-info/not-zip-safe
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      162 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-09-01 10:03:46.000000 pyg2p-3.2.6/src/pyg2p.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-09-01 09:51:26.000000 pyg2p-3.2.6/src/pyg2p.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_cp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_lsp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_rg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_rn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_ta.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_td.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_wu.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/AFFS_wv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_15d.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_15d_glob.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_CV.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_CV_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy_inv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy_nn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_agg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_december.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/EUE_RainAnim_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/UKMO_t24_LA.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/UKMO_t24_LA_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/UKMO_t24_LA_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cin.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_e06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_r06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_t24_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/cosmo_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_e06_2.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_e06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_e06_3.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_r06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_r06_efas.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_r06_gmi.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_t24_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwd_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/dwdl_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/efas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eud_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_e24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_e24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24_15days.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24_15days_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24_15days_noagg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24_15days_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/eue_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/glofas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/glofas_sro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/glofas_ssro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/glofas_ssro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_scipy_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_scipy_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/octahedral_test_scipy_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/rn_false_mv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_r06_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_r06_scipy_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_t24_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-09-01 09:51:26.000000 pyg2p-3.2.6/templates/tigge_lam_t24_scipy_rotated.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-09-01 10:03:46.000000 pyg2p-3.2.6/tests/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4666 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8785 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      938 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2786 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_correction.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7610 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_interpolation.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2246 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_oracle_data.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1997 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_readers.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      669 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_strings.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       76 2023-09-01 09:51:26.000000 pyg2p-3.2.6/tests/test_writers.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-09-01 09:51:26.000000 pyg2p-3.2.7/LICENSE
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-09-01 09:51:26.000000 pyg2p-3.2.7/MANIFEST.in
+-rw-r--r--   0 carlo     (1000) carlo     (1000)    50175 2024-04-09 10:17:02.000000 pyg2p-3.2.7/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    48801 2024-04-09 10:12:33.000000 pyg2p-3.2.7/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/bin/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-09-01 09:51:26.000000 pyg2p-3.2.7/bin/pyg2p
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/configuration/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/geopotentials.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/configuration/global/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3225 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/geopotentials.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/global_conf.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    42231 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8250 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/global/test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-09-01 09:51:26.000000 pyg2p-3.2.7/configuration/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      223 2024-04-09 10:12:33.000000 pyg2p-3.2.7/requirements.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2024-04-09 10:17:02.000000 pyg2p-3.2.7/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7116 2023-09-01 09:55:43.000000 pyg2p-3.2.7/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/VERSION
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7672 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/exceptions.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/main/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    16153 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/main/api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/config.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    23464 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/main/context.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/controller.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/main/interpolation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    22812 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/main/interpolation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/interpolation/grib_interpolation_lib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/interpolation/latlong.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    83273 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/main/manipulation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/manipulation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13758 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/manipulation/aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/manipulation/conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/manipulation/correction.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/main/readers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/readers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11905 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/readers/grib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3468 2024-04-09 10:12:33.000000 pyg2p-3.2.7/src/pyg2p/main/readers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/readers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/main/writers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/writers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/writers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2012 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/main/writers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/util/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/files.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/generics.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/numeric.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p/util/profiling/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/profiling/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/profiling/profilehooks.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p/util/strings.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/
+-rw-r--r--   0 carlo     (1000) carlo     (1000)    50175 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4423 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-09-01 09:56:56.000000 pyg2p-3.2.7/src/pyg2p.egg-info/not-zip-safe
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      184 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2024-04-09 10:17:02.000000 pyg2p-3.2.7/src/pyg2p.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-09-01 09:51:26.000000 pyg2p-3.2.7/src/pyg2p.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_cp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_lsp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_rg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_rn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_ta.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_td.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_wu.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/AFFS_wv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_15d.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_15d_glob.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_CV.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_CV_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy_inv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy_nn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_agg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_december.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/EUE_RainAnim_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/UKMO_t24_LA.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/UKMO_t24_LA_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/UKMO_t24_LA_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cin.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_e06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_r06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_t24_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/cosmo_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_e06_2.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_e06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_e06_3.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_r06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_r06_efas.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_r06_gmi.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_t24_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwd_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/dwdl_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/efas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eud_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_e24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_e24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24_15days.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24_15days_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24_15days_noagg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24_15days_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/eue_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/glofas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/glofas_sro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/glofas_ssro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/glofas_ssro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_scipy_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_scipy_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/octahedral_test_scipy_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/rn_false_mv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_r06_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_r06_scipy_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_t24_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-09-01 09:51:26.000000 pyg2p-3.2.7/templates/tigge_lam_t24_scipy_rotated.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2024-04-09 10:17:02.000000 pyg2p-3.2.7/tests/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4666 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8785 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      938 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2786 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_correction.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8934 2024-04-09 10:12:33.000000 pyg2p-3.2.7/tests/test_interpolation.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2246 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_oracle_data.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1997 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_readers.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      669 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_strings.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       76 2023-09-01 09:51:26.000000 pyg2p-3.2.7/tests/test_writers.py
```

### Comparing `pyg2p-3.2.6/LICENSE` & `pyg2p-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/PKG-INFO` & `pyg2p-3.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pyg2p
-Version: 3.2.6
-Summary: Convert GRIB files to netCDF or PCRaster
-Author: Domenico Nappo
-Author-email: domenico.nappo@gmail.com
-License: EUPL 1.2
-Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Other Audience
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [ChangeLog](CHANGE_LOG.rst)
 
 
 # pyg2p
 pyg2p is a converter between GRIB and netCDF4/PCRaster files. 
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
 
@@ -691,24 +666,52 @@
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
 #### ADW
-It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
-If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+It's the Angular Distance Weighted (ADW) algorithm by Shepard et al. 1968, with scipy.kd_tree using 11 neighbours.
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
   "@lonMap": "/dataset/maps/europe5km/long.map",
   "@mode": "adw",
-  "@adw_broadcasting": false}
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
+}
+```
+
+#### CDD
+It's the Correlation Distance Decay (CDD) modified implementation of the Angular Distance Weighted algorithm, with scipy.kd_tree using 11 neighbours. It needs a map of CDD values for each point, to be specified in the field @cdd_map
+@cdd_mode can be one of the following values: "Hofstra", "NewEtAl" or "MixHofstraShepard"
+In case of mode "MixHofstraShepard", @cdd_options allows to customize the parameters of Hofstra and Shepard algorithm ("weights_mode": can be "All" or "OnlyTOP10" to take 10 higher values only in the interpolation of each point).
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "cdd",
+  "@cdd_map": "/dataset/maps/europe5km/cdd_map.nc",
+  "@cdd_mode": "MixHofstraShepard",
+  "@cdd_options": {
+    "m_const": 4,
+    "min_num_of_station": 4,
+    "radius_ratio": 0.3333333333333333,
+    "weights_mode": "All"
+  },
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
 }
 ```
 
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
```

### Comparing `pyg2p-3.2.6/README.md` & `pyg2p-3.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: pyg2p
+Version: 3.2.7
+Summary: Convert GRIB files to netCDF or PCRaster
+Author: Domenico Nappo
+Author-email: domenico.nappo@gmail.com
+License: EUPL 1.2
+Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: netCDF4<=1.6.4,>=1.5.3
+Requires-Dist: ujson>=5.4.0
+Requires-Dist: numpy>=1.18.2
+Requires-Dist: numba>=0.54.0
+Requires-Dist: scipy>=1.6.0
+Requires-Dist: numexpr>=2.7.1
+Requires-Dist: importlib-metadata<5.0.0
+Requires-Dist: dask[bag]
+Requires-Dist: dask[array]
+Requires-Dist: toolz
+Requires-Dist: eccodes
+Requires-Dist: lisflood-utilities
+Requires-Dist: GDAL==3.5.2
+
 [ChangeLog](CHANGE_LOG.rst)
 
 
 # pyg2p
 pyg2p is a converter between GRIB and netCDF4/PCRaster files. 
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
 
@@ -666,24 +704,52 @@
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
 #### ADW
-It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
-If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+It's the Angular Distance Weighted (ADW) algorithm by Shepard et al. 1968, with scipy.kd_tree using 11 neighbours.
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
   "@lonMap": "/dataset/maps/europe5km/long.map",
   "@mode": "adw",
-  "@adw_broadcasting": false}
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
+}
+```
+
+#### CDD
+It's the Correlation Distance Decay (CDD) modified implementation of the Angular Distance Weighted algorithm, with scipy.kd_tree using 11 neighbours. It needs a map of CDD values for each point, to be specified in the field @cdd_map
+@cdd_mode can be one of the following values: "Hofstra", "NewEtAl" or "MixHofstraShepard"
+In case of mode "MixHofstraShepard", @cdd_options allows to customize the parameters of Hofstra and Shepard algorithm ("weights_mode": can be "All" or "OnlyTOP10" to take 10 higher values only in the interpolation of each point).
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "cdd",
+  "@cdd_map": "/dataset/maps/europe5km/cdd_map.nc",
+  "@cdd_mode": "MixHofstraShepard",
+  "@cdd_options": {
+    "m_const": 4,
+    "min_num_of_station": 4,
+    "radius_ratio": 0.3333333333333333,
+    "weights_mode": "All"
+  },
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
 }
 ```
 
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
```

### Comparing `pyg2p-3.2.6/configuration/global/geopotentials.json` & `pyg2p-3.2.7/configuration/global/geopotentials.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/configuration/global/intertables.json` & `pyg2p-3.2.7/configuration/global/intertables.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/configuration/global/parameters.json` & `pyg2p-3.2.7/configuration/global/parameters.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/setup.py` & `pyg2p-3.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/__init__.py` & `pyg2p-3.2.7/src/pyg2p/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/exceptions.py` & `pyg2p-3.2.7/src/pyg2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/__init__.py` & `pyg2p-3.2.7/src/pyg2p/main/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/api.py` & `pyg2p-3.2.7/src/pyg2p/main/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,19 @@
             self._vars['correction.demMap'] = self.api_conf['Parameter']['demMap']
             if not self._vars['geopotential.dir'] and self.api_conf.get('geopotentialDir'):
                 self._vars['geopotential.dirs']['user'] = self.api_conf['geopotentialDir']
 
         self._vars['outMaps.clone'] = self.api_conf['OutMaps']['cloneMap']
         interpolation_conf = self.api_conf['OutMaps']['Interpolation']
         self._vars['interpolation.mode'] = interpolation_conf.get('mode', self.default_values['interpolation.mode'])
+        self._vars['interpolation.cdd_map'] = interpolation_conf.get('cdd_map', '')
+        self._vars['interpolation.cdd_mode'] = interpolation_conf.get('cdd_mode', '')
+        self._vars['interpolation.cdd_options'] = interpolation_conf.get('cdd_options', None)
         self._vars['interpolation.use_broadcasting'] = interpolation_conf.get('use_broadcasting', False)
+        self._vars['interpolation.num_of_splits'] = interpolation_conf.get('num_of_splits', None)        
         self._vars['interpolation.rotated_target'] = interpolation_conf.get('rotated_target', False)
         if not self._vars['interpolation.dir'] and self.api_conf.get('intertableDir'):
             self._vars['interpolation.dirs']['user'] = self.api_conf['intertableDir']
 
         self._vars['interpolation.latMap'] = interpolation_conf['latMap']
         self._vars['interpolation.lonMap'] = interpolation_conf['lonMap']
         self._vars['outMaps.unitTime'] = self.api_conf['OutMaps'].get('unitTime')
```

### Comparing `pyg2p-3.2.6/src/pyg2p/main/config.py` & `pyg2p-3.2.7/src/pyg2p/main/config.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/context.py` & `pyg2p-3.2.7/src/pyg2p/main/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,19 @@
             self._vars['correction.formula'] = exec_conf['Parameter']['@correctionFormula']
             self._vars['correction.gemFormula'] = exec_conf['Parameter']['@gem']
             self._vars['correction.demMap'] = exec_conf['Parameter']['@demMap']
 
         self._vars['outMaps.clone'] = exec_conf['OutMaps']['@cloneMap']
         interpolation_conf = exec_conf['OutMaps']['Interpolation']
         self._vars['interpolation.mode'] = interpolation_conf.get('@mode', self.default_values['interpolation.mode'])
-        self._vars['interpolation.adw_broadcasting'] = interpolation_conf.get('@adw_broadcasting', False)
+        self._vars['interpolation.cdd_map'] = interpolation_conf.get('@cdd_map', '')
+        self._vars['interpolation.cdd_mode'] = interpolation_conf.get('@cdd_mode', '')
+        self._vars['interpolation.cdd_options'] = interpolation_conf.get('@cdd_options', None)
+        self._vars['interpolation.use_broadcasting'] = interpolation_conf.get('@use_broadcasting', False)
+        self._vars['interpolation.num_of_splits'] = interpolation_conf.get('@num_of_splits', None)
         self._vars['interpolation.rotated_target'] = interpolation_conf.get('@rotated_target', False)
         if not self._vars['interpolation.dir'] and interpolation_conf.get('@intertableDir'):
             # get from JSON
             self._vars['interpolation.dirs']['user'] = interpolation_conf['@intertableDir']
         if not self._vars['geopotential.dir'] and interpolation_conf.get('@geopotentialDir'):
             # get from JSON
             self._vars['geopotential.dirs']['user'] = interpolation_conf['@geopotentialDir']
```

### Comparing `pyg2p-3.2.6/src/pyg2p/main/controller.py` & `pyg2p-3.2.7/src/pyg2p/main/controller.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/interpolation/__init__.py` & `pyg2p-3.2.7/src/pyg2p/main/interpolation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 import pyg2p.util.files
 import pyg2p.util.numeric
 
 
 class Interpolator(Loggable):
     _LOADED_INTERTABLES = {}
     _prefix = 'I'
-    scipy_modes_nnear = {'nearest': 1, 'invdist': 4, 'adw': 4, 'cdd': 4, 'bilinear': 4, 'triangulation': 3, 'bilinear_delaunay': 4}
+    scipy_modes_nnear = {'nearest': 1, 'invdist': 4, 'adw': 11, 'cdd': 11, 'bilinear': 4, 'triangulation': 3, 'bilinear_delaunay': 4}
     suffixes = {'grib_nearest': 'grib_nearest', 'grib_invdist': 'grib_invdist',
                 'nearest': 'scipy_nearest', 'invdist': 'scipy_invdist', 'adw': 'scipy_adw', 'cdd': 'scipy_cdd',
                 'bilinear': 'scipy_bilinear', 'triangulation': 'scipy_triangulation', 'bilinear_delaunay': 'scipy_bilinear_delaunay'}
     _format_intertable = 'tbl{prognum}_{source_file}_{target_size}_{suffix}.npy.gz'.format
 
     def __init__(self, exec_ctx, mv_input):
         super().__init__()
         self._mv_grib = mv_input
         self.interpolate_with_grib = exec_ctx.is_with_grib_interpolation
         self._mode = exec_ctx.get('interpolation.mode')
-        self._adw_broadcasting = exec_ctx.get('interpolation.adw_broadcasting')
+        self._cdd_map = exec_ctx.get('interpolation.cdd_map')
+        self._cdd_mode = exec_ctx.get('interpolation.cdd_mode')
+        self._cdd_options = exec_ctx.get('interpolation.cdd_options')
+        self._use_broadcasting = exec_ctx.get('interpolation.use_broadcasting')
+        self._num_of_splits = exec_ctx.get('interpolation.num_of_splits')
         self._source_filename = pyg2p.util.files.filename(exec_ctx.get('input.file'))
         self._suffix = self.suffixes[self._mode]
         self._intertable_dirs = exec_ctx.get('interpolation.dirs')
         self._rotated_target_grid = exec_ctx.get('interpolation.rotated_target')
         self._target_coords = LatLong(exec_ctx.get('interpolation.latMap'), exec_ctx.get('interpolation.lonMap'))
         self.mv_out = self._target_coords.mv
         self.parallel = exec_ctx.get('interpolation.parallel')
@@ -163,14 +167,18 @@
         if DEBUG_BILINEAR_INTERPOLATION:
             # target_lats=target_lats[1800-(9*20):1800-(-16*20), 3600+(-15*20):3600+(16*20)]
             # target_lons=target_lons[1800-(9*20):1800-(-16*20), 3600+(-15*20):3600+(16*20)]
             if self._target_coords.lats.shape==(3600,7200):
                 # Global_3arcmin DEBUG
                 latefas=self._target_coords.lats[1800-int(DEBUG_MAX_LAT*20):1800-int(DEBUG_MIN_LAT*20), 3600+int(DEBUG_MIN_LON*20):3600+int(DEBUG_MAX_LON*20)]
                 lonefas=self._target_coords.lons[1800-int(DEBUG_MAX_LAT*20):1800-int(DEBUG_MIN_LAT*20), 3600+int(DEBUG_MIN_LON*20):3600+int(DEBUG_MAX_LON*20)]
+                #latefas-=0.008369999999992217
+                # lonefas-=0.00851999999999431
+                #lonefas-=0.024519999999977227   
+
             else:
                 # European_1arcmin DEBUG
                 selection_lats = np.logical_and(self._target_coords.lats[:,0]>=DEBUG_MIN_LAT,self._target_coords.lats[:,0]<=DEBUG_MAX_LAT)
                 selection_lons = np.logical_and(self._target_coords.lons[0,:]>=DEBUG_MIN_LON,self._target_coords.lons[0,:]<=DEBUG_MAX_LON)
                 latefas=self._target_coords.lats[selection_lats,:][:,selection_lons]
                 lonefas=self._target_coords.lons[selection_lats,:][:,selection_lons]
 
@@ -190,17 +198,26 @@
             # longrib = np.array([49.16690015, 48.11557968, 48.27217824, 49.70238655, 46.28414423,
             #     46.3485172, 46.08087359, 49.33047938, 49.112627, 49.48004859])
             # v = np.array([197.86183422, 179.91585642, 146.14793623, 178.05291763, 111.82744259, 
             #     163.99210213, 114.33532874, 194.4668917, 152.18483218, 141.466194  ])
             # latgrib = np.array([ 7.39050803,  8.72151493,  7.82210701,  7.35906546])
             # longrib = np.array([49.16690015, 48.11557968, 48.27217824, 49.70238655])
             # v = np.array([100, 133, 166, 200  ])
-            latgrib = np.array([ 8,  8,  8,  8])
-            longrib = np.array([45, 48.5, 49, 50])
-            v = np.array([200, 100, 100, 100  ])
+            # latgrib = np.array([ 8,  8,  8,  8])
+            # longrib = np.array([45, 48.5, 49, 50])
+            # v = np.array([200, 100, 100, 100  ])
+            
+            # OR load data points for the TEST from file
+            #data = np.genfromtxt('/media/sf_VMSharedFolder/pyg2p_adw_cdd_test/pr199106180600_idw.txt', delimiter='\t', skip_header=1)
+            #data = np.genfromtxt('/media/sf_VMSharedFolder/pyg2p_adw_cdd_test/pr199106170600_20230714101901.txt', delimiter='\t', skip_header=1)
+            data = np.genfromtxt('/media/sf_VMSharedFolder/test_split/tn202401010600_20240213140643.txt', delimiter='\t', skip_header=1)
+            longrib = data[:,0]
+            latgrib = data[:,1]
+            v = data[:,2]
+
             intertable_id, intertable_name = 'DEBUG_ADW','DEBUG_ADW.npy'
 
         nnear = self.scipy_modes_nnear[self._mode]
 
         if (not DEBUG_ADW_INTERPOLATION) and \
             (pyg2p.util.files.exists(intertable_name) or pyg2p.util.files.exists(intertable_name + '.gz')):
                 indexes, weights = self._read_intertable(intertable_name)
@@ -208,19 +225,30 @@
 
         elif self.create_if_missing:
             self.intertables_config.check_write()
             if latgrib is None:
                 self._log('Trying to interpolate without grib lat/lons. Probably a malformed grib!', 'ERROR')
                 raise ApplicationException.get_exc(5000)
 
+            # CR: to use float32 computations uncomment here:
+            # longrib=np.float32(longrib)
+            # latgrib=np.float32(latgrib)
+            # lonefas=np.float32(lonefas)
+            # latefas=np.float32(latefas)
+            # v=np.float32(v)
+            # self.mv_out=np.float32(self.mv_out)
+            
             self._log('\nInterpolating table not found\n Id: {}\nWill create file: {}'.format(intertable_id, intertable_name), 'WARN')
             scipy_interpolation = ScipyInterpolation(longrib, latgrib, grid_details, v.ravel(), nnear, self.mv_out,
                                           self._mv_grib, target_is_rotated=self._rotated_target_grid,
-                                          parallel=self.parallel, mode=self._mode, use_broadcasting=self._adw_broadcasting)
-            _, weights, indexes = scipy_interpolation.interpolate(lonefas, latefas)
+                                          parallel=self.parallel, mode=self._mode, 
+                                          cdd_map=self._cdd_map, cdd_mode=self._cdd_mode, cdd_options = self._cdd_options,
+                                          use_broadcasting=self._use_broadcasting,
+                                          num_of_splits=self._num_of_splits)
+            _, weights, indexes = scipy_interpolation.interpolate(lonefas, latefas)            
             result = self._interpolate_scipy_append_mv(v, weights, indexes, nnear)
 
             # saving interpolation lookup table
             intertable = np.rec.fromarrays((indexes, weights), names=('indexes', 'coeffs'))
             if intertable_name.endswith('.gz'):
                 f = gzip.GzipFile(intertable_name, 'w')
                 np.save(f, intertable)
```

### Comparing `pyg2p-3.2.6/src/pyg2p/main/interpolation/grib_interpolation_lib.py` & `pyg2p-3.2.7/src/pyg2p/main/interpolation/grib_interpolation_lib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/interpolation/latlong.py` & `pyg2p-3.2.7/src/pyg2p/main/interpolation/latlong.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/interpolation/scipy_interpolation_lib.py` & `pyg2p-3.2.7/src/pyg2p/main/interpolation/scipy_interpolation_lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 import eccodes
 import numexpr as ne
 import numpy as np
 import math 
 import scipy.optimize as opt  
 from scipy.spatial import cKDTree as KDTree, Delaunay
 
+from pyg2p.main.readers.netcdf import NetCDFReader
+from pyg2p.main.readers.pcr import PCRasterReader
+
 from ...exceptions import ApplicationException, WEIRD_STUFF, INVALID_INTERPOL_METHOD
 from pyg2p.util.numeric import mask_it, empty
 from pyg2p.util.generics import progress_step_and_backchar
 from pyg2p.util.strings import now_string
 
 #from matplotlib import pyplot as plt
 from scipy.integrate import quad
 
+from numba import njit
+
 
 DEBUG_BILINEAR_INTERPOLATION = False
 DEBUG_ADW_INTERPOLATION = False
 # DEBUG_MIN_LAT = 88
 # DEBUG_MIN_LON = -180
 # DEBUG_MAX_LAT = 90
 # DEBUG_MAX_LON = 180
@@ -32,18 +37,52 @@
 # DEBUG_MIN_LON = -24
 # DEBUG_MAX_LAT = 70
 # DEBUG_MAX_LON = -22
 # DEBUG_MIN_LAT = -10
 # DEBUG_MIN_LON = -100
 # DEBUG_MAX_LAT = 25
 # DEBUG_MAX_LON = -50
-DEBUG_MIN_LAT = 7
-DEBUG_MIN_LON = 45
-DEBUG_MAX_LAT = 9
-DEBUG_MAX_LON = 50
+# DEBUG_MIN_LAT = 7
+# DEBUG_MIN_LON = 45
+# DEBUG_MAX_LAT = 9
+# DEBUG_MAX_LON = 50
+# DEBUG_MIN_LAT = (45.31663-2)
+# DEBUG_MIN_LON = (0.46648-2) #0.50048
+# DEBUG_MAX_LAT = (45.31663+2)
+# DEBUG_MAX_LON = (0.46648+2) #0.50048
+# DEBUG_MIN_LAT = (45.31663-2)
+# DEBUG_MIN_LON = (0.50048-2) 
+# DEBUG_MAX_LAT = (45.31663+2)
+# DEBUG_MAX_LON = (0.50048+2) 
+# lat 45.28263, lon 0.45948
+# DEBUG_MIN_LAT = (45.28263-2)
+# DEBUG_MIN_LON = (0.45948-2) 
+# DEBUG_MAX_LAT = (45.28263+2)
+# DEBUG_MAX_LON = (0.45948+2) 
+# lat 45.28263 lon 0.5517
+
+# DEBUG_MIN_LAT = (45.28263-40)
+# DEBUG_MIN_LON = (0.5517-60) 
+# DEBUG_MAX_LAT = (45.28263+40)
+# DEBUG_MAX_LON = (0.5517+60) 
+
+# Full European 1arcmin, step 0.01666666666667993:
+# DEBUG_MIN_LAT = 22.758333333333333
+# DEBUG_MIN_LON = -25.241666666666667
+# DEBUG_MAX_LAT = 72.24166666666667
+# DEBUG_MAX_LON = 50.24166666666666
+DEBUG_MIN_LAT = 45-10
+DEBUG_MIN_LON = 8-10
+DEBUG_MAX_LAT = 45+10
+DEBUG_MAX_LON = 8+10
+# DEBUG_MIN_LAT = 57.95-0
+# DEBUG_MIN_LON = 16.80-0
+# DEBUG_MAX_LAT = 57.95+5
+# DEBUG_MAX_LON = 16.80+5
+
 #DEBUG_NN = 15410182
 
 
 ###########################################################################################
 ###### functions used to get correct quadrilateral points for the bilinear interpolation ####
 ###########################################################################################
 
@@ -275,35 +314,239 @@
     is_in_t2 = isPointInTriangle(pt, v1,v4,v3)
     return is_in_t1 or is_in_t2
 
 # used in triangulation for the evaluation of space between vertical grid in grib non regular grid files
 def integrand(x):
     return 1/np.cos(x)
 
+
+@njit(parallel=True, fastmath=False, cache=True)
+def adw_compute_weights_from_cutoff_distances(distances, s, ref_radius):
+    # get "s" vector as the inverse distance with power = 1 (in "w" we have the invdist power 2)
+    # actually s(d) should be 
+    #   1/d                     when 0 < d <= r'/3
+    #   (27/4r')*[(d/r'-1)^2]   when r'/3 < d <= r'
+    #   0                       when r' < d
+    # The orginal method consider a range of 4 to 10 data points e removes distant point using the rule:
+    # pi*r= 7(N/A)  where N id the number of points and A is the area of the largest poligon enclosed by data points
+    # r'(C^n) = di(n+1) where di is the Point having the minimum distance major than the first n Points
+    # so that
+    #   r' = r' C^4 = di(5)     when n(C) <= 4
+    #   r' = r                  when 4 < n(C) <= 10
+    #   r' = r' C^10 = di(11)   when 10 < n(C)
+    #
+    # evaluate r from pi*r= 7(N/A):
+    # A = area of the polygon containing all points
+    # N = number of points
+    # trick: I can evaluate r from the KD Tree of distances: r should be the radius that contains 7 points as an average
+    # so I can set it as the value that contains 70% of the whole distance dataset.
+    # Given the ordered distances struct, the quickest way to do it is to evaluate the average of all distances of the 7th 
+    # element of the distance arrays
+    
+    if ref_radius==None:
+        r_ref = np.mean(distances[:, 6])
+    else:
+        r_ref = ref_radius 
+    
+    # prepare r, initialize with di(11):                 
+    r = distances[:, 10].copy()
+    # evaluate r' for each point. to do that, 
+    # 1) chech if the distance in the fourth position is higher that r_ref, if so, we are in case r' C^4 (that is = di(5))
+    
+    r_1_flag = distances[:, 3] > r_ref
+    # copy the corresponding fifth distance di(5) as the radius
+    r[r_1_flag] = distances[r_1_flag, 4]
+    # 2) check if n(C)>4 and n(C)<=10
+    r_2_flag = np.logical_and(~r_1_flag, distances[:, 9] > r_ref)
+    # copy r as the radius
+    r[r_2_flag] = r_ref
+    # 3) all the other case, n(C)>10, will be equal to di(11) (already set at the initialization, so do nothing here)
+    
+    # apply the distance rule based on the radiuses
+    r_broadcasted = r.reshape(-1,1)
+    
+    #   1/d                     when 0 < d <= r'/3
+    dist_leq_r3 = distances <= r_broadcasted / 3
+    s.ravel()[dist_leq_r3.ravel()] = 1. / distances.ravel()[dist_leq_r3.ravel()]
+    
+    #   (27/4r')*(d/r'-1)       when r'/3 < d <= r'
+    dist_g_r3_leq_r = np.logical_and(~dist_leq_r3, distances <= r_broadcasted)
+    s.ravel()[dist_g_r3_leq_r.ravel()] = ((27 / (4 * r_broadcasted)) * ((distances / r_broadcasted - 1) ** 2)).ravel()[dist_g_r3_leq_r.ravel()]
+    
+    #   0                       when r' < d  (keep the default zero value)
+
+    # in case of Shepard we use the square of the coeafficient stored later in variable "s"
+    w = s ** 2
+    return w, s
+
+@njit(parallel=True, fastmath=False, cache=True)
+def cdd_hofstra_compute_weights_from_cutoff_distances(distances, CDD_map, s):
+    # Hofstra et al. 2008 
+    # CDD is the correlation distance decay to get the serach radius
+
+    # formula for weights:
+    # where m is fixed to 4 and x is the distance between the station i and the point 
+    m_const = 4.0 # constant
+    # wi = [e^(−x/CDD)]^m       when 0  < d <= CDD
+    #   0                       when CDD < d
+    # The orginal method consider a range of 3 to 10 data points e removes distant points
+    #
+
+    # 1) chech if the distance in the third position is higher that CDD, if so, we should store a missing value
+    # because it means we don't have a minimum of 3 points within the CDD radius
+    missingval_flag = distances[:, 2] > CDD_map
+    
+    # apply the distance rule based on the radiuses
+    CDD_broadcasted = CDD_map.reshape(-1,1)
+    
+    #   [e^(−x/CDD)]^m       when 0  < d <= CDD
+    dist_leq_CDD = distances <= CDD_broadcasted
+    s.ravel()[dist_leq_CDD.ravel()] = np.exp(-distances*m_const/CDD_broadcasted).ravel()[dist_leq_CDD.ravel()]
+        
+    #   0                       when CDD < d  (keep the default zero value)
+
+    s[missingval_flag] = 0
+    return s
+
+@njit(parallel=True, fastmath=False, cache=True)
+def cdd_hofstra_shepard_compute_weights_from_cutoff_distances(distances, CDD_map, nnear, s, m_const = 4, min_num_of_station = 4, radius_ratio=1/3):
+    # mix Hofstra and Shepard methods 
+    # uses Shepard approach to smooth borders:
+    #   wi = [e^(−x/CDD)]^m                                             when 0  < d <= CDD*radius_ratio  e^(-radius_ratio)^m
+    #   [1/(radius_ratio-1)^2]*{[e^(-radius_ratio)]^m}*[(d/CDD-1)^2]    when CDD*radius_ratio < d <= CDD  
+    #   0                                                               when CDD < d
+    # furthermore, as in Shepard, increases adjust radius value in these cases:
+    #   having n(C) number of points having distance < CDD
+    #   r' = r' C^min_num_of_station = di(min_num_of_station+1)     when n(C) <= min_num_of_station
+    #   r' = CDD                when min_num_of_station < n(C) <= 10    n.b: 10 = [nnear-1]
+    #   r' = r' C^10 = di(11)   when 10 < n(C)                          n.b: 10 = [nnear-1]
+
+    r_ref = CDD_map
+    # prepare r, initialize with di(11) [nnear]:
+    #r = distances[:, 10].copy()
+    r = distances[:, nnear-1].copy()
+    # evaluate r' for each point. to do that, 
+    # 1) chech if the distance in the fourth position is higher that r_ref, if so, we are in case r' C^min_num_of_station (that is = di(min_num_of_station+1))
+    r_1_flag = distances[:, min_num_of_station-1] > r_ref
+    # copy the corresponding fifth distance di(min_num_of_station+1) as the radius
+    r[r_1_flag] = distances[r_1_flag, min_num_of_station]
+    # 2) check if n(C)>min_num_of_station and n(C)<=10 [nnear-1]
+    #r_2_flag = np.logical_and(~r_1_flag, distances[:, 9] > r_ref)
+    r_2_flag = np.logical_and(~r_1_flag, distances[:, nnear-2] > r_ref)
+    # copy CDD as the radius
+    r[r_2_flag] = r_ref[r_2_flag]
+    # 3) all the other case, n(C)>10 [nnear-1], will be equal to di(11) (already set at the initialization, so do nothing here)
+    
+    # apply the distance rule based on the radiuses
+    r_broadcasted = r.reshape(-1,1)
+    
+    #   wi = [e^(−x/CDD)]^m     when 0 < d <= CDD*radius_ratio  e^(-radius_ratio)^m
+    dist_leq_r3 = distances <= r_broadcasted * radius_ratio
+    s.ravel()[dist_leq_r3.ravel()] = np.exp(-distances*m_const/r_broadcasted).ravel()[dist_leq_r3.ravel()]
+    
+    #   [1/(radius_ratio-1)^2]*{[e^(-radius_ratio)]^m}*[(d/CDD-1)^2]   when CDD*radius_ratio < d <= CDD
+    dist_g_r3_leq_r = np.logical_and(~dist_leq_r3, distances <= r_broadcasted)
+    s.ravel()[dist_g_r3_leq_r.ravel()] = (( (1/(radius_ratio-1)**2) * np.exp(-m_const*radius_ratio)) * ((distances / r_broadcasted - 1) ** 2)).ravel()[dist_g_r3_leq_r.ravel()]
+    
+    #   0                       when r' < d  (keep the default zero value)
+    return s
+
+
+@njit(parallel=True, fastmath=False, cache=True)
+def cdd_newetal_compute_weights_from_cutoff_distances(distances, CDD_map, indexes, longrib, latgrib, TargetLonRes, TargetLatRes, LonOrigin, LatOrigin, s):
+    # New et al. 2000 
+    # no search radius applied
+    # consider all the available nearest station, and use their respective CDD to compute the weights
+
+    # formula for weights:
+    # where m is fixed to 4 and x is the distance between the station i and the point 
+    m_const = 4.0 # constant
+    # wi = [e^(−x/CDD)]^m       
+        
+    #   [e^(−x/CDD)]^m       when 0  < d <= CDD
+
+    CDD_values = CDD_map[np.clip(((LatOrigin-latgrib[indexes])/TargetLatRes).astype(int),0,CDD_map.shape[0]-1), \
+                                        np.clip(((LonOrigin-longrib[indexes])/TargetLonRes).astype(int),0,CDD_map.shape[1]-1)]
+    dist_leq_CDD = distances <= CDD_values
+    s.ravel()[dist_leq_CDD.ravel()] = np.exp(-distances*m_const/CDD_values).ravel()[dist_leq_CDD.ravel()]
+        
+    return s
+
+@njit(parallel=True, fastmath=False, cache=True)
+def adw_and_cdd_compute_weights_directional_in_broadcasting(
+    s,latgrib,longrib,indexes,lat_inALL,lon_inALL):
+    # All in broadcasting: 
+    # this algorithm uses huge amount of memory and deas not speed up much on standard Virtual Machine
+    if DEBUG_ADW_INTERPOLATION:
+        print("\nUsing full broadcasting")
+    # Compute xi and yi for all elements
+    k=indexes.shape[1]
+    xi = latgrib.ravel()[indexes.ravel()]
+    yi = longrib.ravel()[indexes.ravel()]
+    # Compute xi_diff and yi_diff for all elements
+    xi_diff = lat_inALL.reshape(-1,1) - xi.reshape(-1,k)
+    yi_diff = lon_inALL.reshape(-1,1) - yi.reshape(-1,k)
+    # Compute Di for all elements
+    Di = np.sqrt(xi_diff**2 + yi_diff**2)
+    # Compute cos_theta for all elements
+    cos_theta = (xi_diff.reshape(-1,k,1)* xi_diff.reshape(-1,1,k) + yi_diff.reshape(-1,k,1) * yi_diff.reshape(-1,1,k)) / (Di.reshape(-1,k,1) * Di.reshape(-1,1,k))
+    # skip when i==j, so that directional weight of i is evaluated on all points j where j!=i 
+    # TODO: tip: since cos_theta = 1 for i==j, to speed up we can skip this passage and apply i!=j only on denominator
+    # Delete the diagonal elements from cos_theta
+    # Reshape cos_theta to (n, nnear, nnear-1)
+    n = cos_theta.shape[0]
+    m = cos_theta.shape[1]
+    strided = np.lib.stride_tricks.as_strided
+    s0,s1,s2 = cos_theta[:].strides
+    cos_theta = strided(cos_theta.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).copy().reshape(n,m,-1)
+    sj = s.T.repeat(k).reshape(k,-1,k).transpose(1,2,0).copy()
+    s0,s1,s2 = sj[:].strides
+    sj = strided(sj.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).copy().reshape(n,m,-1)
+    # sj = np.tile(s[:, np.newaxis, :], (1, m, 1))
+    # s0,s1,s2 = sj[:].strides
+    # sj = strided(sj.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).reshape(n,m,-1)
+
+    numerator = np.sum((1 - cos_theta) * sj, axis=2)
+    denominator = np.sum(sj, axis=2)
+    # Compute weight_directional for all elements
+    weight_directional = numerator / denominator
+    
+    return weight_directional
+
+
 class ScipyInterpolation(object):
     """
     http://docs.scipy.org/doc/scipy/reference/spatial.html
     """
     gribapi_version = list(map(int, eccodes.codes_get_api_version().split('.')))
     rotated_bugfix_gribapi = gribapi_version[0] > 1 or (gribapi_version[0] == 1 and gribapi_version[1] > 14) or (gribapi_version[0] == 1 and gribapi_version[1] == 14 and gribapi_version[2] >= 3)
 
     def __init__(self, longrib, latgrib, grid_details, source_values, nnear, 
                     mv_target, mv_source, target_is_rotated=False, parallel=False,
-                    mode='nearest', use_broadcasting = False):
+                    mode='nearest', cdd_map='', cdd_mode='', cdd_options = None, use_broadcasting = False,
+                    num_of_splits = None):
         stdout.write('Start scipy interpolation: {}\n'.format(now_string()))
         self.geodetic_info = grid_details
         self.source_grid_is_rotated = 'rotated' in grid_details.get('gridType')
         self.target_grid_is_rotated = target_is_rotated
         self.njobs = 1 if not parallel else -1
         
         self.longrib = longrib
         self.latgrib = latgrib
         self.nnear = nnear
         self.mode = mode
+        self.cdd_map = cdd_map
+        self.cdd_mode = cdd_mode
+        self.cdd_options = cdd_options
         self.use_broadcasting = use_broadcasting
+        self.num_of_splits = num_of_splits
+        
+        if DEBUG_ADW_INTERPOLATION:
+            self.use_broadcasting = True
+
         self._mv_target = mv_target
         self._mv_source = mv_source
         self.z = source_values
         
         # we receive rotated coords from GRIB_API iterator before 1.14.3
         x, y, zz = self.to_3d(longrib, latgrib, to_regular=not self.rotated_bugfix_gribapi)
         source_locations = np.vstack((x.ravel(), y.ravel(), zz.ravel())).T
@@ -311,47 +554,98 @@
             assert len(source_locations) == len(source_values), "len(coordinates) {} != len(values) {}".format(len(source_locations), len(source_values))
         except AssertionError as e:
             ApplicationException.get_exc(WEIRD_STUFF, details=str(e))
 
         stdout.write('Building KDTree...\n')
         self.tree = KDTree(source_locations, leafsize=30)  # build the tree
 
-        # we can calculate resolution in KM as described here:
-        # http://math.boisestate.edu/~wright/montestigliano/NearestNeighborSearches.pdf
-        # sphdist = R*acos(1-maxdist^2/2);
-        # Finding actual resolution of source GRID
-        distances, indexes = self.tree.query(source_locations, k=2, n_jobs=self.njobs)
-        # set max of distances as min upper bound and add an empirical correction value
-        self.min_upper_bound = np.max(distances) + np.max(distances) * 4 / self.geodetic_info.get('Nj')
+        if self.mode == "adw":
+            self.min_upper_bound = None # not used in adw (Shepard) algorithm
+        else:
+            # we can calculate resolution in KM as described here:
+            # http://math.boisestate.edu/~wright/montestigliano/NearestNeighborSearches.pdf
+            # sphdist = R*acos(1-maxdist^2/2);
+            # Finding actual resolution of source GRID
+            distances, indexes = self.tree.query(source_locations, k=2, workers=self.njobs)
+            # set max of distances as min upper bound and add an empirical correction value
+            self.min_upper_bound = np.max(distances) + np.max(distances) * 4 / self.geodetic_info.get('Nj')
+
+    def interpolate(self, lonefas, latefas):        
+        if (self.num_of_splits is not None):
+            ref_radius = None
+            if self.mode == 'adw' and self.nnear == 11:
+                start = time.time()
+                stdout.write('Finding global reference radius {} interpolation k=7\n'.format(self.mode))
+                x, y, z = self.to_3d(lonefas, latefas, to_regular=self.target_grid_is_rotated)
+                efas_locations = np.vstack((x.ravel(), y.ravel(), z.ravel())).T
+                distances, indexes = self.tree.query(efas_locations, k=7, workers=self.njobs) 
+                if efas_locations.dtype==np.dtype('float32'):
+                    distances=np.float32(distances)
+
+                ref_radius=np.mean(distances[:, 6])
+                checktime = time.time()
+                stdout.write('KDtree find radius time (sec): {}\n'.format(checktime - start))
+
+            # Define the size of the subsets, only in lonm
+            subset_size = lonefas.shape[0]//self.num_of_splits
+
+            # Initialize empty arrays to store the results
+            weights = np.empty((lonefas.shape[0]*lonefas.shape[1],self.nnear),dtype=lonefas.dtype)
+            indexes = np.empty((lonefas.shape[0]*lonefas.shape[1],self.nnear),dtype=int)
+            result = np.empty((lonefas.shape[0]*lonefas.shape[1]),dtype=lonefas.dtype)
+
+            # Iterate over the subsets of the arrays
+            for i in range(0, lonefas.shape[0], subset_size):
+                subset_lonefas = lonefas[i:i+subset_size, :]
+                subset_latefas = latefas[i:i+subset_size, :]
+
+                # Call the interpolate function for the subset
+                subset_result, subset_weights, subset_indexes = self.interpolate_split(subset_lonefas, subset_latefas, ref_radius)
+
+                # Collect the results back into the weights and indexes arrays
+                weights[i*lonefas.shape[1]:(i+subset_size)*lonefas.shape[1],:] = subset_weights
+                indexes[i*lonefas.shape[1]:(i+subset_size)*lonefas.shape[1],:] = subset_indexes
+                result[i*lonefas.shape[1]:(i+subset_size)*lonefas.shape[1]] = subset_result
+        
+        else:
+            result, weights, indexes = self.interpolate_split(lonefas, latefas)
 
-    def interpolate(self, target_lons, target_lats):
+        return result, weights, indexes
+
+
+    def interpolate_split(self, target_lons, target_lats, ref_radius=None):        
         # Target coordinates  HAVE to be rotated coords in case GRIB grid is rotated
         # Example of target rotated coords are COSMO lat/lon/dem PCRASTER maps
         self.target_latsOR=target_lats
         self.target_lonsOR=target_lons
 
         start = time.time()
         if self.mode != 'triangulation' and self.mode != 'bilinear_delaunay':
             stdout.write('Finding indexes for {} interpolation k={}\n'.format(self.mode, self.nnear))
             x, y, z = self.to_3d(target_lons, target_lats, to_regular=self.target_grid_is_rotated)
             efas_locations = np.vstack((x.ravel(), y.ravel(), z.ravel())).T
-            distances, indexes = self.tree.query(efas_locations, k=self.nnear, n_jobs=self.njobs) 
+            distances, indexes = self.tree.query(efas_locations, k=self.nnear, workers=self.njobs) 
+            if efas_locations.dtype==np.dtype('float32'):
+                distances=np.float32(distances)
+            checktime = time.time()
+            stdout.write('KDtree time (sec): {}\n'.format(checktime - start))
         
         if self.mode == 'nearest' and self.nnear == 1:
             # return results, indexes
             result, indexes = self._build_nn(distances, indexes)
             weights = distances
         else:
             if self.mode == 'invdist': 
                 # return results, distances, indexes
                 result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear)
-            elif self.mode == 'adw':
-                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='Shepard', use_broadcasting=self.use_broadcasting)             
+            elif self.mode == 'adw' and self.nnear == 11:
+                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='Shepard', use_broadcasting=self.use_broadcasting, ref_radius=ref_radius)             
             elif self.mode == 'cdd':
-                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='CDD', use_broadcasting=self.use_broadcasting)
+                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='CDD', use_broadcasting=self.use_broadcasting, ref_radius=None,
+                                                                       cdd_map=self.cdd_map, cdd_mode=self.cdd_mode, cdd_options=self.cdd_options)
             elif self.mode == 'bilinear' and self.nnear == 4: # bilinear interpolation only supported with nnear = 4
                 # BILINEAR INTERPOLATION
                 result, weights, indexes = self._build_weights_bilinear(distances, indexes, efas_locations, self.nnear) 
             elif self.mode == 'triangulation':
                 # linear barycentric interpolation on Delaunay triangulation
                 result, weights, indexes = self._build_weights_triangulation(use_bilinear=False) 
             elif self.mode == 'bilinear_delaunay':
@@ -389,14 +683,20 @@
             y = ne.evaluate('(-sin(fi) * ({x})) + (cos(fi) * ({y}))'.format(x=x_formula, y=y_formula))
             z = ne.evaluate('(-sin(teta) * cos(fi) * ({x})) - (sin(teta) * sin(fi) * ({y})) + (cos(teta) * ({z}))'.format(x=x_formula, y=y_formula, z=z_formula))
         else:
             r = self.geodetic_info.get('radius')
             x = ne.evaluate('r * {x}'.format(x=x_formula))
             y = ne.evaluate('r * {y}'.format(y=y_formula))
             z = ne.evaluate('r * {z}'.format(z=z_formula))
+
+        if lons.dtype==np.dtype('float32'):
+            x=np.float32(x)
+            y=np.float32(y)
+            z=np.float32(z)
+
         return x, y, z
 
     def _build_nn(self, distances, indexes):
         z = self.z
         result = mask_it(np.empty((len(distances),) + np.shape(z[0])), self._mv_target, 1)
         jinterpol = 0
         num_cells = result.size
@@ -467,197 +767,323 @@
     #     stdout.write('{}Building coeffs: {}/{} (100%)\n'.format(back_char, 5, 5))
     #     stdout.flush()
     #     return result, weights, idxs
 
     # Inverse distance weights (IDW) interpolation, with optional Angular distance weighting (ADW) factor
     # if adw_type == None -> simple IDW 
     # if adw_type == Shepard -> Shepard 1968 original formulation
-    def _build_weights_invdist(self, distances, indexes, nnear, adw_type = None, use_broadcasting = False):
+    def _build_weights_invdist(self, distances, indexes, nnear, adw_type = None, use_broadcasting = False, ref_radius = None, 
+                               cdd_map='', cdd_mode='', cdd_options=None):
         if DEBUG_ADW_INTERPOLATION:
-            self.min_upper_bound = 1000000000
+            if adw_type != "Shepard":
+                self.min_upper_bound = 1000000000
             if DEBUG_BILINEAR_INTERPOLATION:
-                n_debug=1940
+                #n_debug=1940
+                #n_debug=3120
+                n_debug=1120
             else:
                 n_debug=11805340
         z = self.z
-        result = mask_it(np.empty((len(distances),) + np.shape(z[0])), self._mv_target, 1)
-        weights = empty((len(distances),) + (nnear,))
+        result = mask_it(np.empty((len(distances),) + np.shape(z[0]),dtype=z.dtype), self._mv_target, 1)
+        weights = empty((len(distances),) + (nnear,),dtype=z.dtype)
         idxs = empty((len(indexes),) + (nnear,), fill_value=z.size, dtype=int)
         num_cells = result.size
         back_char, _ = progress_step_and_backchar(num_cells)
 
         stdout.write('Skipping neighbors at distance > {}\n'.format(self.min_upper_bound))
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 0, 5, 0, 0))
         stdout.flush()
 
-        dist_leq_1e_10 = distances[:, 0] <= 1e-10
-        dist_leq_min_upper_bound = np.logical_and(~dist_leq_1e_10, distances[:, 0] <= self.min_upper_bound)
+        if (adw_type is None):
+            dist_leq_1e_10 = distances[:, 0] <= 1e-10
+            dist_leq_min_upper_bound = np.logical_and(~dist_leq_1e_10, distances[:, 0] <= self.min_upper_bound)
         
-        # distances <= 1e-10 : take exactly the point, weight = 1
-        onlyfirst_array = np.zeros(nnear)
-        onlyfirst_array[0] = 1
-        weights[dist_leq_1e_10] = onlyfirst_array
-        idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
-        result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
+            # distances <= 1e-10 : take exactly the point, weight = 1
+            onlyfirst_array = np.zeros(nnear)
+            onlyfirst_array[0] = 1
+            weights[dist_leq_1e_10] = onlyfirst_array
+            idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
+            result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
+
+            w = np.zeros_like(distances)
+
+            # in case of normal IDW we use inverse squared distances
+            # while in case of Shepard we use the square of the coeafficient stored later in variable "s"
+            # while in case of CDD we use the same Wi coeafficient stored later in variable "s"
+            w[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound] ** 2
 
-        w = np.zeros_like(distances)
-        w[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound] ** 2
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 1, 5, 100/5))
         stdout.flush()
 
-        if (adw_type=='Shepard'):
-            # initialize weights
-            weight_directional = np.zeros_like(distances)
-
-            # get "s" vector as the inverse distance with power = 1 (in "w" we have the invdist power 2)
-            # actually s(d) should be 
-            #   1/d                     when 0 < d < r'/3
-            #   (27/4r')*(d/r'-1)       when r'/3 < d < r'
-            #   0                       when r' < d
-            # The orginal method consider a range of 4 to 10 data points e removes distant point using the rule:
-            # pi*r= 7(N/A)  where N id the number of points and A is the area of the largest poligon enclosed by data points
-            # r'(C^n) = di(n+1) where di is the Point having the minimum distance major than the first n Points
-            # so that
-            #   r' = r' C^4 = di(5)     when n(C) <= 4
-            #   r' = r                  when 4 < n(C) <= 10
-            #   r' = r' C^10 = di(11)   when 10 < n(C)
-            #
-            # TODO: check if the implementation needs to be updated accordingly
-            # here we take only the inverse of the distance in "s"
-            s = np.zeros_like(distances)       
-            s[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound]
-
+        if (adw_type=='Shepard') or (adw_type=='CDD'):
             self.lat_inALL = self.target_latsOR.ravel()
             self.lon_inALL = self.target_lonsOR.ravel()
 
+            if (adw_type=='Shepard'): 
+                # this implementation is based on the manuscript by Shepard et al. 1968 
+                # now it applies the selection of station, too. k=11 stations are need to perform the full elavaluation
+
+                # initialize weights
+                if (use_broadcasting == False):
+                    weight_directional = np.zeros_like(distances)
+                start = time.time()
+                s = np.zeros_like(distances)
+                w, s = adw_compute_weights_from_cutoff_distances(distances, s, ref_radius)
+                checktime = time.time()
+                stdout.write('adw_compute_weights_from_cutoff_distances time (sec): {}\n'.format(checktime - start))
+
+            elif (adw_type=='CDD'):
+                # this implementation is based on the manuscript by Hofstra et al. 2008 and New et al. 2000 
+
+                #read CDD map or txt file
+                CDD_map = None
+                stdout.write(f'Reading CDD values from: {cdd_map}')
+                if cdd_map.endswith('.nc'):
+                    reader = NetCDFReader(cdd_map)
+                else:
+                    reader = PCRasterReader(cdd_map)
+                # CDD map values are in km, so convert to meters to compare with distances
+                CDD_map = reader.values * 1000
+
+                if DEBUG_BILINEAR_INTERPOLATION:
+                    # target_lats=target_lats[1800-(9*20):1800-(-16*20), 3600+(-15*20):3600+(16*20)]
+                    # target_lons=target_lons[1800-(9*20):1800-(-16*20), 3600+(-15*20):3600+(16*20)]
+                    if CDD_map.shape==(3600,7200):
+                        # Global_3arcmin DEBUG
+                        CDD_map=CDD_map[1800-int(DEBUG_MAX_LAT*20):1800-int(DEBUG_MIN_LAT*20), 3600+int(DEBUG_MIN_LON*20):3600+int(DEBUG_MAX_LON*20)]
+                        #latefas-=0.008369999999992217
+                        # lonefas-=0.00851999999999431
+                        #lonefas-=0.024519999999977227   
+
+                    else:
+                        # European_1arcmin DEBUG
+                        CDD_map=CDD_map[round((72.24166666666667-DEBUG_MAX_LAT)/0.01666666666667993):round((72.24166666666667-DEBUG_MIN_LAT)/0.01666666666667993), \
+                            round((-25.241666666666667-DEBUG_MIN_LON)/-0.01666666666667993):round((-25.241666666666667-DEBUG_MAX_LON)/-0.01666666666667993)]
+
+                #CDDmode = 'NewEtAl'
+                #CDDmode = 'Hofstra'
+                #CDDmode = 'MixHofstraShepard'       #uses Shepard approach to smooth borders
+                CDDmode = cdd_mode
+                
+                weights_mode = 'All'
+                #weights_mode = 'OnlyTOP10'
+                if (CDDmode == 'Hofstra'):
+                    CDD_map = CDD_map.ravel()
+                    try:
+                        assert(len(CDD_map)==len(self.lat_inALL)) 
+                    except AssertionError as e:
+                        ApplicationException.get_exc(WEIRD_STUFF, details=str(e) + "\nCDD map should have the same resolution of target map. CDD map len={}, target map len={}".format(len(CDD_map), len(self.lat_inALL)))
+
+                    stdout.write('\nEvaluating cutoffs...')
+                    
+                    s = np.zeros_like(distances)       
+                    s = cdd_hofstra_compute_weights_from_cutoff_distances(distances, CDD_map, s)
+                elif CDDmode == 'MixHofstraShepard':
+                    CDD_map = CDD_map.ravel()
+                    try:
+                        assert(len(CDD_map)==len(self.lat_inALL)) 
+                    except AssertionError as e:
+                        ApplicationException.get_exc(WEIRD_STUFF, details=str(e) + "\nCDD map should have the same resolution of target map. CDD map len={}, target map len={}".format(len(CDD_map), len(self.lat_inALL)))
+
+                    if DEBUG_ADW_INTERPOLATION:
+                        stdout.write('\nEvaluating cutoffs...')
+                    
+                    s = np.zeros_like(distances)      
+                    if cdd_options is None:
+                        # Hofstra standard values
+                        m_const = 4
+                        min_num_of_station = 4
+                        radius_ratio = 1/3
+                        weights_mode = "All"
+                    else:
+                        # Custom values
+                        m_const, min_num_of_station, radius_ratio, weights_mode = cdd_options.values()
+                    cdd_hofstra_shepard_compute_weights_from_cutoff_distances(distances, CDD_map, nnear, s, m_const, min_num_of_station, radius_ratio)
+                elif CDDmode == 'NewEtAl':
+                    s = np.zeros_like(distances)  
+                    TargetLonRes=self.target_lonsOR[0,0]-self.target_lonsOR[0,1]
+                    TargetLatRes=self.target_latsOR[0,0]-self.target_latsOR[1,0]
+                    LonOrigin=self.target_lonsOR[0,0]
+                    LatOrigin=self.target_latsOR[0,0]
+                    s = cdd_newetal_compute_weights_from_cutoff_distances(distances, CDD_map, indexes, self.longrib, self.latgrib, 
+                                                                        TargetLonRes, TargetLatRes, LonOrigin, LatOrigin, s)
+                else:
+                    ApplicationException.get_exc(WEIRD_STUFF, "\nCDD mode unknown={}".format(CDDmode))
+
+                # consider only TOP 10 weights instead of all:
+                if weights_mode == "OnlyTOP10":
+                    # indices of top 10 values in each row
+                    #   idx = np.argpartition(s, 10, axis=1)  # get indices of top 10 values
+                    #   rows = np.arange(s.shape[0])[:, None]
+                    #   s[rows, idx[:, :-10]] = 0
+                    # all in one row:
+                    s[np.arange(s.shape[0])[:, None], np.argpartition(s, 10, axis=1)[:, :-10]] = 0
+
+
+                
+                # ####### Old version: 
+                # CDD should be the correlation distance decay to get the search radius
+                # # in this implementation we take always k station, regardless of the radius
+                # # thus we can use CDD=max(distances)
+                # CDD = np.empty((len(distances),) + np.shape(z[0]))
+                # CDD[dist_leq_min_upper_bound] = np.max(distances[dist_leq_min_upper_bound],axis=1)
+                # # formula for weights:
+                # # wi = [e^(−x/CDD)]^m 
+                # # where m is fixed to 4 and x is the distance between the station i and the point 
+                # m_const = 4.0 # constant
+                # # initialize weights
+                # weight_directional = np.zeros_like(distances)
+                # # get distance weights            
+                # s = np.zeros_like(distances)       
+                # s[dist_leq_min_upper_bound] = np.exp(-distances[dist_leq_min_upper_bound]*m_const/CDD[dist_leq_min_upper_bound,np.newaxis])
+    
+
             # start_time = time.time()
             if not use_broadcasting:
+                weight_directional = np.zeros_like(distances)
                 for i in range(nnear):
                     xj_diff = self.lat_inALL[:, np.newaxis] - self.latgrib[indexes]
                     yj_diff = self.lon_inALL[:, np.newaxis] - self.longrib[indexes]
                     
                     Dj = np.sqrt(xj_diff**2 + yj_diff**2)
-                    # TODO: check here: we could use "distances", but we are actually evaluating the cos funcion on lat and lon values, that 
+                    # we could use "distances", but we are actually evaluating the cos funcion on lat and lon values, that 
                     # approximates the real angle... to use "distances" we need to operate in 3d version of the points
                     # in theory it should be OK to use the solution above, otherwise we can change it to 
                     # Di = distances[i]
                     # Dj = distances
                     # and formula cos_theta = [(x-xi)*(x-xj) + (y-yi)*(y-yj) + (z-zi)*(z-zj)] / di*dj
-                    
-                    # cos_theta = [(x-xi)*(x-xj) + (y-yi)*(y-yj)] / di*dj. 
-                    #cos_theta = (xi_diff[:,np.newaxis] * xj_diff + yi_diff[:,np.newaxis] * yj_diff) / (Di[:,np.newaxis] * Dj)
-                    # cos_theta = (xj_diff[:,i,np.newaxis] * xj_diff + yj_diff[:,i,np.newaxis] * yj_diff) / (Dj[:,i,np.newaxis] * Dj)
-                    # numerator = np.sum((1 - cos_theta) * s, axis=1)
-                    # denominator = np.sum(s, axis=1)
-                    
+                                        
                     cos_theta = (xj_diff[:,i,np.newaxis] * xj_diff + yj_diff[:,i,np.newaxis] * yj_diff) / (Dj[:,i,np.newaxis] * Dj)
                     # skip when i==j, so that directional weight of i is evaluated on all points j where j!=i 
                     # TODO: tip: since cos_theta = 1 for i==j, to speed up we can skip this passage and apply i!=j only on denominator
                     cos_theta = cos_theta[:,np.concatenate([np.arange(i), np.arange(i+1, cos_theta.shape[1])])]
                     sj = s[:,np.concatenate([np.arange(i), np.arange(i+1, s.shape[1])])]            
                     numerator = np.sum((1 - cos_theta) * sj, axis=1)
                     denominator = np.sum(sj, axis=1)
-                                        
-                    weight_directional[dist_leq_min_upper_bound, i] = numerator[dist_leq_min_upper_bound] / denominator[dist_leq_min_upper_bound]
+                    weight_directional[:,i] = numerator / denominator
 
                     # DEBUG: test the point at n_debug 11805340=lat 8.025 lon 47.0249999
                     if DEBUG_ADW_INTERPOLATION:
                         print("i: {}".format(i))
                         print("cos_theta: {}".format(cos_theta[n_debug]))
                         print("s: {}".format(s[n_debug]))
                         print("numerator: {}".format(numerator[n_debug]))
                         print("denominator: {}".format(denominator[n_debug]))
             else:
-                # All in broadcasting:            
-                # this algorithm uses huge amount of memory and deas not speed up much on standard Virtual Machine
-                # TODO: check if it is worth to use it on HPC 
-                # Compute xi and yi for all elements
-                xi = self.latgrib[indexes]
-                yi = self.longrib[indexes]
-                # Compute xi_diff and yi_diff for all elements
-                xi_diff = self.lat_inALL[:, np.newaxis] - xi
-                yi_diff = self.lon_inALL[:, np.newaxis] - yi
-                # Compute Di for all elements
-                Di = np.sqrt(xi_diff**2 + yi_diff**2)
-                # Compute cos_theta for all elements
-                cos_theta = (xi_diff[:, :, np.newaxis] * xi_diff[:, np.newaxis, :] + yi_diff[:, :, np.newaxis] * yi_diff[:, np.newaxis, :]) / (Di[:, :, np.newaxis] * Di[:, np.newaxis, :])
-                # skip when i==j, so that directional weight of i is evaluated on all points j where j!=i 
-                # TODO: tip: since cos_theta = 1 for i==j, to speed up we can skip this passage and apply i!=j only on denominator
-                # Delete the diagonal elements from cos_theta
-                # Reshape cos_theta to (n, nnear, nnear-1)
-                n = cos_theta.shape[0]
-                m = cos_theta.shape[1]
-                strided = np.lib.stride_tricks.as_strided
-                s0,s1,s2 = cos_theta[:].strides
-                cos_theta = strided(cos_theta.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).reshape(n,m,-1)
-                sj = np.tile(s[:, np.newaxis, :], (1, 4, 1))
-                s0,s1,s2 = sj[:].strides
-                sj = strided(sj.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).reshape(n,m,-1)
-
-                numerator = np.sum((1 - cos_theta) * sj, axis=2)
-                denominator = np.sum(sj, axis=2)
-                # Compute weight_directional for all elements
-                weight_directional[dist_leq_min_upper_bound, :] = numerator[dist_leq_min_upper_bound, :] / denominator[dist_leq_min_upper_bound, :]
-    
+                # All in broadcasting:     
+                start = time.time()
+                weight_directional = adw_and_cdd_compute_weights_directional_in_broadcasting(
+                    s, self.latgrib, self.longrib, indexes,
+                    self.lat_inALL, self.lon_inALL)
+                checktime = time.time()
+                stdout.write('adw_and_cdd_compute_weights_directional_in_broadcasting time (sec): {}\n'.format(checktime - start))
+
+            # replace all the nan values with "1"
+            # this is because we have NaNs when denominator is zero, that happens when only one station is considered 
+            # in the angular evaluation, thus no agle is present
+            weight_directional = np.nan_to_num(weight_directional, nan=1)
+
             # end_time = time.time()
             # elapsed_time = end_time - start_time
             # print(f"Elapsed time for computation: {elapsed_time:.6f} seconds")
-    
+            if (adw_type=='CDD'):
+                w=s
+                # in CDD the weight_directional should be normalized before multiply by 1+...
+                # normalize weight_directional
+                sums_weight_directional = np.sum(weight_directional, axis=1, keepdims=True)
+                weight_directional = weight_directional / sums_weight_directional
+                
             # update weights with directional ones
             if DEBUG_ADW_INTERPOLATION:
                 print("weight_directional: {}".format(weight_directional[n_debug]))
                 print("w (before adding angular weights): {}".format(w[n_debug]))
             w = np.multiply(w,1+weight_directional)
             if DEBUG_ADW_INTERPOLATION:
                 print("w (after adding angular weights): {}".format(w[n_debug]))
-        elif (adw_type=='CDD'):
-            raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
-                        f"interpolation method not implemented yet (mode = {self.mode}, nnear = {self.nnear}, adw_type = {adw_type})")
+
+            # if (adw_type=='Shepard'):
+            #     # TODO: Add Gradient
+            #     # for each D included in C', evaluate A and B
+            #     # A = Sum{wj[(zj-zi)(xj-xi)/d(Dj,Di)^2]}/Sum(wj)
+            #     # B = Sum{wj[(zj-zi)(yj-yi)/d(Dj,Di)^2]}/Sum(wj)
+            #     # v = O.1[max{zi} - min{zi}] / [max{(A^2+B^2)}]^(1/2). 
+            #     # Dzi = [Ai(x-xi) + Bi(y-yi)][v/(v+di)]
+            #     # final results:
+            #     # value = Sum[wi(zi+Dzi)] / Sum(wi) when d!=0, else zi
+
+
         elif (adw_type!=None):
             raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
                         f"interpolation method not supported (mode = {self.mode}, nnear = {self.nnear}, adw_type = {adw_type})")
 
-        #normalize weights
-        sums = np.sum(w[dist_leq_min_upper_bound], axis=1, keepdims=True)
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 2, 5, 2*100/5))
         stdout.flush()
-        weights[dist_leq_min_upper_bound] = w[dist_leq_min_upper_bound] / sums
+        #normalize weights
+        if (adw_type=='Shepard') or (adw_type=='CDD'):
+            sums = np.sum(w, axis=1, keepdims=True)
+            weights = w / sums
+        else:
+            sums = np.sum(w[dist_leq_min_upper_bound], axis=1, keepdims=True)
+            weights[dist_leq_min_upper_bound] = w[dist_leq_min_upper_bound] / sums
         if DEBUG_ADW_INTERPOLATION:
-            dist_smalltest = distances[:, 0] <= 10000
-            onlyfirst_array_test = np.zeros(nnear)
-            onlyfirst_array_test[0] = 1000
-            weights[dist_smalltest]=onlyfirst_array_test
+            # dist_smalltest = distances[:, 0] <= 10000
+            # onlyfirst_array_test = np.zeros(nnear)
+            # onlyfirst_array_test[0] = 1000
+            # weights[dist_smalltest]=onlyfirst_array_test
             print("weights (after normalization): {}".format(weights[n_debug]))
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 3, 5, 3*100/5))
         stdout.flush()
 
         wz = np.einsum('ij,ij->i', weights, z[indexes])
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 4, 5, 4*100/5))
         stdout.flush()
-        idxs[dist_leq_min_upper_bound] = indexes[dist_leq_min_upper_bound]
-        result[dist_leq_min_upper_bound] = wz[dist_leq_min_upper_bound]
+        if (adw_type=='Shepard') or (adw_type=='CDD'):
+            idxs = indexes
+            result = wz
+            
+            if (adw_type=='Shepard'):
+                # in Shepard, we still have NaN values because of the denominator when the distance is equal to 0
+                # so we just take the exact value when the point is exacly on the station coordinates
+                dist_leq_1e_10 = distances[:, 0] <= 1e-10
+            
+                # distances <= 1e-10 : take exactly the point, weight = 1
+                onlyfirst_array = np.zeros(nnear, dtype=weights.dtype)
+                onlyfirst_array[0] = 1
+                weights[dist_leq_1e_10] = onlyfirst_array
+                idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
+                result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
+        else:
+            idxs[dist_leq_min_upper_bound] = indexes[dist_leq_min_upper_bound]
+            result[dist_leq_min_upper_bound] = wz[dist_leq_min_upper_bound]
         if DEBUG_ADW_INTERPOLATION:
             print("result: {}".format(result[n_debug]))
+            if adw_type is None:
+                self.lat_inALL = self.target_latsOR.ravel()
+                self.lon_inALL = self.target_lonsOR.ravel()
+
             print("lat: {}".format(self.lat_inALL[n_debug]))
             print("lon: {}".format(self.lon_inALL[n_debug]))
+            # Lon 0.46648 Lat 45.31663
+            # Lon 0.50048 Lat 45.31663
+
             print("idxs: {}".format(idxs[n_debug]))
             print("distances: {}".format(distances[n_debug]))
             print("latgrib: {}".format(self.latgrib[idxs[n_debug]]))
             print("longrib: {}".format(self.longrib[idxs[n_debug]]))
             print("value: {}".format(self.z[idxs[n_debug]]))
         stdout.write('{}Building coeffs: {}/{} (100%)\n'.format(back_char, 5, 5))
         stdout.flush()
 
         return result, weights, idxs
 
     # take additional points from the KDTree close to the current point and replace the wrong ones with a new ones
     def replaceIndex(self, indexes_to_replace, indexes, nn, additional_points):
         additional_points += len(indexes_to_replace)
         # replace the unwanted index with next one:
-        _, replacement_indexes = self.tree.query(self.target_location, k=self.nnear+additional_points, n_jobs=self.njobs) 
+        _, replacement_indexes = self.tree.query(self.target_location, k=self.nnear+additional_points, workers=self.njobs) 
         # print("replacement_indexes: {}".format(replacement_indexes))
 
         # delete all the current indexes from the replaceent_indexes 
         # this is to fix an issue with the query, that do not give always the same
         # order when the distance is the same for some of the points
         for i in indexes[nn, 0:4]:
             replacement_indexes = np.delete(replacement_indexes, np.where(replacement_indexes == i))
@@ -676,15 +1102,15 @@
 
     # take additional points from the KDTree close to the another specific point
     # and replace the wrong ones with new ones
     def replaceIndexCloseToPoint(self, indexes_to_replace, new_lat, new_lon, indexes, nn):
         # replace up to 2 unwanted indexes with next ones:
         x, y, z = self.to_3d(new_lon, new_lat, to_regular=self.target_grid_is_rotated)
         new_target_location = [x,y,z]
-        _, replacement_indexes = self.tree.query(new_target_location, k=len(indexes_to_replace), n_jobs=self.njobs) 
+        _, replacement_indexes = self.tree.query(new_target_location, k=len(indexes_to_replace), workers=self.njobs) 
         # print("replacement_indexes: {}".format(replacement_indexes))
         
         # get rid of the wrong points and add the farthest among the new selected points
         if len(indexes_to_replace)>1:
             for n,i in enumerate(indexes_to_replace):
                 indexes[nn, indexes[nn, 0:4] == i] = replacement_indexes[-(n+1)]
         else:
@@ -951,15 +1377,15 @@
             normalized_longrib = padded_longrib
             normalized_latgrib = padded_latgrib
             z=padded_z
         else:
             stdout.write('Finding nearest neighbor to exclude outside triangles\n')
             x_tmp, y_tmp, z_tmp = self.to_3d(self.target_lonsOR[:,:], self.target_latsOR[:,:], to_regular=self.target_grid_is_rotated)
             efas_locations = np.vstack((x_tmp.ravel(), y_tmp.ravel(), z_tmp.ravel())).T
-            distances, _ = self.tree.query(efas_locations, k=1, n_jobs=self.njobs) 
+            distances, _ = self.tree.query(efas_locations, k=1, workers=self.njobs) 
 
         gribpoints = np.stack((normalized_latgrib,normalized_longrib),axis=-1)
         gribpoints_scaled = gribpoints.copy()
         # In case of non rotated grib files, the grid has variable number of points according to the latitude, 
         # so adjust the grid spaces for an effective triangulation
         # In case of rotated grid, instead, use the original grid points, that is fine for the spece even if it is rotaded
         if self.source_grid_is_rotated == False:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyg2p-3.2.6/src/pyg2p/main/manipulation/aggregator.py` & `pyg2p-3.2.7/src/pyg2p/main/manipulation/aggregator.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/manipulation/conversion.py` & `pyg2p-3.2.7/src/pyg2p/main/manipulation/conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/manipulation/correction.py` & `pyg2p-3.2.7/src/pyg2p/main/manipulation/correction.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/readers/grib.py` & `pyg2p-3.2.7/src/pyg2p/main/readers/grib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/readers/netcdf.py` & `pyg2p-3.2.7/src/pyg2p/main/readers/netcdf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import numpy as np
 
 from pyg2p import Loggable
 import netCDF4 as nc
-from netCDF4 import Dataset 
+from netCDF4 import Dataset, default_fillvals
 import warnings
 
 class NetCDFReader(Loggable):
 
     def __init__(self, nc_map):
         super().__init__()
         self._log(f'Reading {nc_map}')
@@ -28,15 +28,22 @@
         self._origY = self._dataset.variables[self.label_lat][:].min()
         self._pxlW = self._dataset.variables[self.label_lon][1]-self._dataset.variables[self.label_lon][0]
         self._pxlH = self._dataset.variables[self.label_lat][1]-self._dataset.variables[self.label_lat][0]       
         self.lat_min = self._dataset.variables[self.label_lat][:].min()
         self.lon_min = self._dataset.variables[self.label_lon][:].min()
         self.lat_max = self._dataset.variables[self.label_lat][:].max()
         self.lon_max = self._dataset.variables[self.label_lon][:].max()
-        self.mv = self._dataset.variables[self.var_name].missing_value
+        if hasattr(self._dataset.variables[self.var_name],'missing_value'):
+            self.mv = self._dataset.variables[self.var_name].missing_value
+        else:
+            if hasattr(self._dataset.variables[self.var_name],'_FillValue'):
+                self.mv = self._dataset.variables[self.var_name]._FillValue
+            else:
+                dtype = self._dataset.variables[self.var_name].dtype
+                self.mv = default_fillvals[dtype.str[1:]] if np.issubdtype(dtype, np.integer) else np.nan
 
     def find_main_var(self, path):
         variable_names = [k for k in self._dataset.variables if len(self._dataset.variables[k].dimensions) >= 2]
         if len(variable_names) > 1:
             warnings.warn('More than one variable in dataset {}'.format(path), RuntimeWarning)
         elif len(variable_names) == 0:
             warnings.warn('Could not find a valid variable in dataset {}'.format(path), RuntimeWarning)
```

### Comparing `pyg2p-3.2.6/src/pyg2p/main/readers/pcr.py` & `pyg2p-3.2.7/src/pyg2p/main/readers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/writers/__init__.py` & `pyg2p-3.2.7/src/pyg2p/main/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/writers/netcdf.py` & `pyg2p-3.2.7/src/pyg2p/main/writers/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/main/writers/pcr.py` & `pyg2p-3.2.7/src/pyg2p/main/writers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/util/files.py` & `pyg2p-3.2.7/src/pyg2p/util/files.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/util/generics.py` & `pyg2p-3.2.7/src/pyg2p/util/generics.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/util/numeric.py` & `pyg2p-3.2.7/src/pyg2p/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/util/profiling/profilehooks.py` & `pyg2p-3.2.7/src/pyg2p/util/profiling/profilehooks.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p/util/strings.py` & `pyg2p-3.2.7/src/pyg2p/util/strings.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/src/pyg2p.egg-info/PKG-INFO` & `pyg2p-3.2.7/src/pyg2p.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.6
+Version: 3.2.7
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,27 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: netCDF4<=1.6.4,>=1.5.3
+Requires-Dist: ujson>=5.4.0
+Requires-Dist: numpy>=1.18.2
+Requires-Dist: numba>=0.54.0
+Requires-Dist: scipy>=1.6.0
+Requires-Dist: numexpr>=2.7.1
+Requires-Dist: importlib-metadata<5.0.0
+Requires-Dist: dask[bag]
+Requires-Dist: dask[array]
+Requires-Dist: toolz
+Requires-Dist: eccodes
+Requires-Dist: lisflood-utilities
+Requires-Dist: GDAL==3.5.2
 
 [ChangeLog](CHANGE_LOG.rst)
 
 
 # pyg2p
 pyg2p is a converter between GRIB and netCDF4/PCRaster files. 
 It can also manipulates GRIB messages (performing aggregation or simple unit conversion) before to apply format conversion.
@@ -691,24 +704,52 @@
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
 #### ADW
-It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
-If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+It's the Angular Distance Weighted (ADW) algorithm by Shepard et al. 1968, with scipy.kd_tree using 11 neighbours.
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
   "@lonMap": "/dataset/maps/europe5km/long.map",
   "@mode": "adw",
-  "@adw_broadcasting": false}
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
+}
+```
+
+#### CDD
+It's the Correlation Distance Decay (CDD) modified implementation of the Angular Distance Weighted algorithm, with scipy.kd_tree using 11 neighbours. It needs a map of CDD values for each point, to be specified in the field @cdd_map
+@cdd_mode can be one of the following values: "Hofstra", "NewEtAl" or "MixHofstraShepard"
+In case of mode "MixHofstraShepard", @cdd_options allows to customize the parameters of Hofstra and Shepard algorithm ("weights_mode": can be "All" or "OnlyTOP10" to take 10 higher values only in the interpolation of each point).
+If @use_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+If @num_of_splits is set to any number, computations will be split on subset and then recollected into the final map, to save mamory (do not set it if you have enought memory to run interpolation)
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "cdd",
+  "@cdd_map": "/dataset/maps/europe5km/cdd_map.nc",
+  "@cdd_mode": "MixHofstraShepard",
+  "@cdd_options": {
+    "m_const": 4,
+    "min_num_of_station": 4,
+    "radius_ratio": 0.3333333333333333,
+    "weights_mode": "All"
+  },
+  "@use_broadcasting": false,
+  "@num_of_splits": 10}
 }
 ```
 
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
```

### Comparing `pyg2p-3.2.6/src/pyg2p.egg-info/SOURCES.txt` & `pyg2p-3.2.7/src/pyg2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_cp.json` & `pyg2p-3.2.7/templates/AFFS_cp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_lsp.json` & `pyg2p-3.2.7/templates/AFFS_lsp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_rg.json` & `pyg2p-3.2.7/templates/AFFS_rg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_rn.json` & `pyg2p-3.2.7/templates/AFFS_rn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_ta.json` & `pyg2p-3.2.7/templates/AFFS_ta.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_td.json` & `pyg2p-3.2.7/templates/AFFS_td.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_wu.json` & `pyg2p-3.2.7/templates/AFFS_wu.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/AFFS_wv.json` & `pyg2p-3.2.7/templates/AFFS_wv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_15d.json` & `pyg2p-3.2.7/templates/EUE_15d.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_15d_glob.json` & `pyg2p-3.2.7/templates/EUE_15d_glob.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim.json` & `pyg2p-3.2.7/templates/EUE_RainAnim.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_CV.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_CV.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_CV_g.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_CV_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy_inv.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy_inv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_CV_scipy_nn.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_CV_scipy_nn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_agg.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_agg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_december.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_december.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_g.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/EUE_RainAnim_scipy.json` & `pyg2p-3.2.7/templates/EUE_RainAnim_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/UKMO_t24_LA.json` & `pyg2p-3.2.7/templates/UKMO_t24_LA.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/UKMO_t24_LA_g.json` & `pyg2p-3.2.7/templates/UKMO_t24_LA_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/UKMO_t24_LA_scipy.json` & `pyg2p-3.2.7/templates/UKMO_t24_LA_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cin.json` & `pyg2p-3.2.7/templates/cin.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_e06.json` & `pyg2p-3.2.7/templates/cosmo_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_e06_newmaps.json` & `pyg2p-3.2.7/templates/cosmo_e06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_e06_scipy.json` & `pyg2p-3.2.7/templates/cosmo_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_r06.json` & `pyg2p-3.2.7/templates/cosmo_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_r06_newmaps.json` & `pyg2p-3.2.7/templates/cosmo_r06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_r06_scipy.json` & `pyg2p-3.2.7/templates/cosmo_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_t24.json` & `pyg2p-3.2.7/templates/cosmo_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_t24_newmaps.json` & `pyg2p-3.2.7/templates/cosmo_t24_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/cosmo_t24_scipy.json` & `pyg2p-3.2.7/templates/cosmo_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_e06.json` & `pyg2p-3.2.7/templates/dwd_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_e06_2.json` & `pyg2p-3.2.7/templates/dwd_e06_2.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_e06_2nd.json` & `pyg2p-3.2.7/templates/dwd_e06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_e06_3.json` & `pyg2p-3.2.7/templates/dwd_e06_3.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_e06_scipy.json` & `pyg2p-3.2.7/templates/dwd_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_r06.json` & `pyg2p-3.2.7/templates/dwd_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_r06_2nd.json` & `pyg2p-3.2.7/templates/dwd_r06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_r06_efas.json` & `pyg2p-3.2.7/templates/dwd_r06_efas.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_r06_gmi.json` & `pyg2p-3.2.7/templates/dwd_r06_gmi.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_r06_scipy.json` & `pyg2p-3.2.7/templates/dwd_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_t24.json` & `pyg2p-3.2.7/templates/dwd_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_t24_2nd.json` & `pyg2p-3.2.7/templates/dwd_t24_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwd_t24_scipy.json` & `pyg2p-3.2.7/templates/dwd_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/dwdl_r06.json` & `pyg2p-3.2.7/templates/dwdl_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/efas_sro.json` & `pyg2p-3.2.7/templates/efas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_e06.json` & `pyg2p-3.2.7/templates/eud_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_e06_scipy.json` & `pyg2p-3.2.7/templates/eud_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_r06.json` & `pyg2p-3.2.7/templates/eud_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_r06_scipy.json` & `pyg2p-3.2.7/templates/eud_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_r24.json` & `pyg2p-3.2.7/templates/eud_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_r24_scipy.json` & `pyg2p-3.2.7/templates/eud_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_t24.json` & `pyg2p-3.2.7/templates/eud_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eud_t24_scipy.json` & `pyg2p-3.2.7/templates/eud_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_e24.json` & `pyg2p-3.2.7/templates/eue_e24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_e24_scipy.json` & `pyg2p-3.2.7/templates/eue_e24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24.json` & `pyg2p-3.2.7/templates/eue_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24_15days.json` & `pyg2p-3.2.7/templates/eue_r24_15days.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24_15days_g.json` & `pyg2p-3.2.7/templates/eue_r24_15days_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24_15days_noagg.json` & `pyg2p-3.2.7/templates/eue_r24_15days_noagg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24_15days_scipy.json` & `pyg2p-3.2.7/templates/eue_r24_15days_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_r24_scipy.json` & `pyg2p-3.2.7/templates/eue_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_t24.json` & `pyg2p-3.2.7/templates/eue_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/eue_t24_scipy.json` & `pyg2p-3.2.7/templates/eue_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/glofas_sro.json` & `pyg2p-3.2.7/templates/glofas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/glofas_sro_scipy.json` & `pyg2p-3.2.7/templates/glofas_sro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/glofas_ssro.json` & `pyg2p-3.2.7/templates/glofas_ssro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/glofas_ssro_scipy.json` & `pyg2p-3.2.7/templates/glofas_ssro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test.json` & `pyg2p-3.2.7/templates/octahedral_test.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_global.json` & `pyg2p-3.2.7/templates/octahedral_test_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_global_invdist.json` & `pyg2p-3.2.7/templates/octahedral_test_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_invdist.json` & `pyg2p-3.2.7/templates/octahedral_test_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_scipy.json` & `pyg2p-3.2.7/templates/octahedral_test_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_scipy_global.json` & `pyg2p-3.2.7/templates/octahedral_test_scipy_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_scipy_global_invdist.json` & `pyg2p-3.2.7/templates/octahedral_test_scipy_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/octahedral_test_scipy_invdist.json` & `pyg2p-3.2.7/templates/octahedral_test_scipy_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/rn_false_mv.json` & `pyg2p-3.2.7/templates/rn_false_mv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_r06.json` & `pyg2p-3.2.7/templates/tigge_lam_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_r06_rotated.json` & `pyg2p-3.2.7/templates/tigge_lam_r06_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_r06_scipy.json` & `pyg2p-3.2.7/templates/tigge_lam_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_r06_scipy_rotated.json` & `pyg2p-3.2.7/templates/tigge_lam_r06_scipy_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_t24.json` & `pyg2p-3.2.7/templates/tigge_lam_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_t24_rotated.json` & `pyg2p-3.2.7/templates/tigge_lam_t24_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_t24_scipy.json` & `pyg2p-3.2.7/templates/tigge_lam_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/templates/tigge_lam_t24_scipy_rotated.json` & `pyg2p-3.2.7/templates/tigge_lam_t24_scipy_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_aggregator.py` & `pyg2p-3.2.7/tests/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_api.py` & `pyg2p-3.2.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_conversion.py` & `pyg2p-3.2.7/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_correction.py` & `pyg2p-3.2.7/tests/test_correction.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_interpolation.py` & `pyg2p-3.2.7/tests/test_interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         interpolator = Interpolator(ctx, missing)
         values_in = messages.values_first_or_single_res[messages.first_step_range]
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(config_dict['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
 
-    @pytest.mark.slow
+    #@pytest.mark.slow
     def test_interpolation_create_scipy_invdist(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'invdist'
         file = d['input.file']
         reader = GRIBReader(file)
@@ -41,21 +41,21 @@
         values_in = messages.values_first_or_single_res[messages.first_step_range]
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
         os.unlink('tests/data/tbl_pf10tp_550800_scipy_invdist.npy.gz')
 
-    @pytest.mark.slow
+    #@pytest.mark.slow
     def test_interpolation_create_scipy_adw(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'adw'
-        d['interpolation.adw_broadcasting'] = True
+        d['interpolation.use_broadcasting'] = True
         file = d['input.file']
         reader = GRIBReader(file)
         messages = reader.select_messages(shortName='2t')
         grid_id = messages.grid_id
         missing = messages.missing_value
         ctx = MockedExecutionContext(d, False)
         interpolator = Interpolator(ctx, missing)
@@ -63,14 +63,40 @@
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
         os.unlink('tests/data/tbl_pf10tp_550800_scipy_adw.npy.gz')
 
     @pytest.mark.slow
+    def test_interpolation_create_scipy_cdd(self):
+        d = deepcopy(config_dict)
+        d['interpolation.create'] = True
+        d['interpolation.parallel'] = True
+        d['interpolation.mode'] = 'cdd'
+        d['interpolation.lonMap'] = 'tests/data/template_test.nc'
+        d['interpolation.latMap'] = 'tests/data/template_test.nc'
+        d['interpolation.cdd_map'] = 'tests/data/cdd_temp_map.nc'
+        d['interpolation.cdd_options'] = None
+        d['interpolation.cdd_mode'] = 'MixHofstraShepard'
+        d['interpolation.use_broadcasting'] = True
+        file = d['input.file']
+        reader = GRIBReader(file)
+        messages = reader.select_messages(shortName='2t')
+        grid_id = messages.grid_id
+        missing = messages.missing_value
+        ctx = MockedExecutionContext(d, False)
+        interpolator = Interpolator(ctx, missing)
+        values_in = messages.values_first_or_single_res[messages.first_step_range]
+        lats, lons = messages.latlons
+        values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
+        shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
+        assert shape_target == values_resampled.shape
+        os.unlink('tests/data/tbl_input_360000_scipy_cdd.npy.gz')
+
+    @pytest.mark.slow
     def test_interpolation_create_scipy_bilinear(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'bilinear'
         # # Test on era5 grib map in NetCDF format
         d['interpolation.lonMap'] = 'tests/data/template_test.nc'
@@ -85,15 +111,15 @@
         ctx = MockedExecutionContext(d, False)
         interpolator = Interpolator(ctx, missing)
         values_in = messages.values_first_or_single_res[messages.first_step_range]
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
-        os.unlink('tests/data/tbl_era5t2avg_441_scipy_bilinear.npy.gz')
+        os.unlink('tests/data/tbl_era5t2avg_360000_scipy_bilinear.npy.gz')
 
     @pytest.mark.slow
     def test_interpolation_create_scipy_triangulation(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'triangulation'
@@ -110,15 +136,15 @@
         ctx = MockedExecutionContext(d, False)
         interpolator = Interpolator(ctx, missing)
         values_in = messages.values_first_or_single_res[messages.first_step_range]
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
-        os.unlink('tests/data/tbl_era5t2avg_441_scipy_triangulation.npy.gz')
+        os.unlink('tests/data/tbl_era5t2avg_360000_scipy_triangulation.npy.gz')
 
     @pytest.mark.slow
     def test_interpolation_create_scipy_bilinear_delaunay(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'bilinear_delaunay'
@@ -135,15 +161,15 @@
         ctx = MockedExecutionContext(d, False)
         interpolator = Interpolator(ctx, missing)
         values_in = messages.values_first_or_single_res[messages.first_step_range]
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
-        os.unlink('tests/data/tbl_era5t2avg_441_scipy_bilinear_delaunay.npy.gz')
+        os.unlink('tests/data/tbl_era5t2avg_360000_scipy_bilinear_delaunay.npy.gz')
 
     @pytest.mark.slow
     def test_interpolation_create_eccodes_nearest(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = False
         d['interpolation.mode'] = 'grib_nearest'
```

### Comparing `pyg2p-3.2.6/tests/test_oracle_data.py` & `pyg2p-3.2.7/tests/test_oracle_data.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_readers.py` & `pyg2p-3.2.7/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.6/tests/test_strings.py` & `pyg2p-3.2.7/tests/test_strings.py`

 * *Files identical despite different names*

