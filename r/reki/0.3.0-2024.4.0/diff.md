# Comparing `tmp/reki-0.3.0.tar.gz` & `tmp/reki-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reki-0.3.0.tar", last modified: Wed Nov 24 02:42:04 2021, max compression
+gzip compressed data, was "reki-2024.4.0.tar", last modified: Tue Apr  9 08:16:21 2024, max compression
```

## Comparing `reki-0.3.0.tar` & `reki-2024.4.0.tar`

### file list

```diff
@@ -1,160 +1,248 @@
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:04.004217 reki-0.3.0/
--rw-rw-rw-   0        0        0    35587 2021-11-24 02:38:19.000000 reki-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0       41 2021-11-24 02:38:19.000000 reki-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11411 2021-11-24 02:42:04.003217 reki-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10325 2021-11-24 02:38:19.000000 reki-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.825956 reki-0.3.0/reki/
--rw-rw-rw-   0        0        0       23 2021-11-24 02:38:19.000000 reki-0.3.0/reki/__init__.py
--rw-rw-rw-   0        0        0      187 2021-11-24 02:38:19.000000 reki-0.3.0/reki/_util.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.844956 reki-0.3.0/reki/data_finder/
--rw-rw-rw-   0        0        0       54 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/__init__.py
--rw-rw-rw-   0        0        0     4945 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/__main__.py
--rw-rw-rw-   0        0        0      547 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/_config.py
--rw-rw-rw-   0        0        0     4399 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/_util.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.794956 reki-0.3.0/reki/data_finder/conf/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.767957 reki-0.3.0/reki/data_finder/conf/cm/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.846957 reki-0.3.0/reki/data_finder/conf/cm/glob/
--rw-rw-rw-   0        0        0      383 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/cm/glob/fnl.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.768959 reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.848956 reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/grib2/
--rw-rw-rw-   0        0        0      523 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/grib2/0p50.yaml
--rw-rw-rw-   0        0        0      523 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/grib2/1p00.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.769957 reki-0.3.0/reki/data_finder/conf/exp/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.769957 reki-0.3.0/reki/data_finder/conf/exp/grapes_gfs_gmf/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.853956 reki-0.3.0/reki/data_finder/conf/exp/grapes_gfs_gmf/grib2/
--rw-rw-rw-   0        0        0      410 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/exp/grapes_gfs_gmf/grib2/modelvar.yaml
--rw-rw-rw-   0        0        0      406 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/exp/grapes_gfs_gmf/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.782959 reki-0.3.0/reki/data_finder/conf/od/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.771959 reki-0.3.0/reki/data_finder/conf/od/grapes_geps/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.855957 reki-0.3.0/reki/data_finder/conf/od/grapes_geps/grib2/
--rw-rw-rw-   0        0        0     1020 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_geps/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.773958 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.861956 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/
--rw-rw-rw-   0        0        0      902 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/modelvar.yaml
--rw-rw-rw-   0        0        0      906 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/modelvar_ctl.yaml
--rw-rw-rw-   0        0        0      898 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/postvar.yaml
--rw-rw-rw-   0        0        0      904 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/postvar_ctl.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.866957 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/grib2/
--rw-rw-rw-   0        0        0     1836 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/grib2/modelvar.yaml
--rw-rw-rw-   0        0        0     1428 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/grib2/ne.yaml
--rw-rw-rw-   0        0        0     1991 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.874957 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/
--rw-rw-rw-   0        0        0      834 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/r2cwe.yaml
--rw-rw-rw-   0        0        0      834 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/rgwst.yaml
--rw-rw-rw-   0        0        0      834 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/rsing.yaml
--rw-rw-rw-   0        0        0      834 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/rsurf.yaml
--rw-rw-rw-   0        0        0      834 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/rtemp.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.775959 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.880988 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/
--rw-rw-rw-   0        0        0      787 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/modelvar.yaml
--rw-rw-rw-   0        0        0      793 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/modelvar_ctl.yaml
--rw-rw-rw-   0        0        0      785 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/postvar.yaml
--rw-rw-rw-   0        0        0      791 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/postvar_ctl.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.884957 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/grib2/
--rw-rw-rw-   0        0        0      819 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/grib2/modelvar.yaml
--rw-rw-rw-   0        0        0      803 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.779956 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.890956 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/
--rw-rw-rw-   0        0        0      783 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/modelvar.yaml
--rw-rw-rw-   0        0        0      789 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/modelvar_ctl.yaml
--rw-rw-rw-   0        0        0      781 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/postvar.yaml
--rw-rw-rw-   0        0        0      787 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/postvar_ctl.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.894959 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/
--rw-rw-rw-   0        0        0     1024 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/cloud.yaml
--rw-rw-rw-   0        0        0     1004 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/modelvar.yaml
--rw-rw-rw-   0        0        0      989 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.781959 reki-0.3.0/reki/data_finder/conf/od/grapes_reps/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.897960 reki-0.3.0/reki/data_finder/conf/od/grapes_reps/grib2/
--rw-rw-rw-   0        0        0      826 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_reps/grib2/orig.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.784956 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.901956 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/bin/
--rw-rw-rw-   0        0        0      761 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/bin/postvar.yaml
--rw-rw-rw-   0        0        0      741 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/bin/postvar_ctl.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.904958 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/grib2/
--rw-rw-rw-   0        0        0     1330 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/grib2/orig.yaml
--rw-rw-rw-   0        0        0      759 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/od/grapes_tym/grib2/sfc.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.785956 reki-0.3.0/reki/data_finder/conf/smart2022/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.789957 reki-0.3.0/reki/data_finder/conf/smart2022/obs/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.788956 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.788956 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.906960 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/chn/
--rw-rw-rw-   0        0        0      433 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/chn/1km.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.908959 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/RMAPS_IN/
--rw-rw-rw-   0        0        0      428 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/smart2022/obs/grid/RMAPS_IN/bth.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.793957 reki-0.3.0/reki/data_finder/conf/smart2022/obs/station/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.909959 reki-0.3.0/reki/data_finder/conf/smart2022/obs/station/cmadaas/
--rw-rw-rw-   0        0        0      286 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/smart2022/obs/station/cmadaas/olympics.yaml
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.795957 reki-0.3.0/reki/data_finder/conf/vfy/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.796958 reki-0.3.0/reki/data_finder/conf/vfy/muvos/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.913958 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.798960 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.925957 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/
--rw-rw-rw-   0        0        0      332 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_01.yaml
--rw-rw-rw-   0        0        0      332 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_03.yaml
--rw-rw-rw-   0        0        0      332 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_06.yaml
--rw-rw-rw-   0        0        0      332 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_24.yaml
--rw-rw-rw-   0        0        0      314 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/sfc.yaml
--rw-rw-rw-   0        0        0      306 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/conf/vfy/muvos/obs/gts.yaml
--rw-rw-rw-   0        0        0     5261 2021-11-24 02:38:19.000000 reki-0.3.0/reki/data_finder/local.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.930957 reki-0.3.0/reki/format/
--rw-rw-rw-   0        0        0        0 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.942958 reki-0.3.0/reki/format/grads/
--rw-rw-rw-   0        0        0       41 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grads/__init__.py
--rw-rw-rw-   0        0        0     5422 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grads/field.py
--rw-rw-rw-   0        0        0    13260 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grads/grads_ctl.py
--rw-rw-rw-   0        0        0     4194 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grads/grads_data_handler.py
--rw-rw-rw-   0        0        0     1499 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grads/grads_record_handler.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.949959 reki-0.3.0/reki/format/grib/
--rw-rw-rw-   0        0        0     1703 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/__init__.py
--rw-rw-rw-   0        0        0      981 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/_level.py
--rw-rw-rw-   0        0        0      620 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/_parameter.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.954956 reki-0.3.0/reki/format/grib/cfgrib/
--rw-rw-rw-   0        0        0       82 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/cfgrib/__init__.py
--rw-rw-rw-   0        0        0     2181 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/cfgrib/_util.py
--rw-rw-rw-   0        0        0     9600 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/cfgrib/field.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.958958 reki-0.3.0/reki/format/grib/config/
--rw-rw-rw-   0        0        0       42 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/config/__init__.py
--rw-rw-rw-   0        0        0     1394 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/config/short_name.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.976575 reki-0.3.0/reki/format/grib/eccodes/
--rw-rw-rw-   0        0        0      342 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/__init__.py
--rw-rw-rw-   0        0        0     1190 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/_level.py
--rw-rw-rw-   0        0        0     4567 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/_util.py
--rw-rw-rw-   0        0        0     7782 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/_xarray.py
--rw-rw-rw-   0        0        0     3767 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/bytes.py
--rw-rw-rw-   0        0        0    10027 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/field.py
--rw-rw-rw-   0        0        0     6424 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/message.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.977575 reki-0.3.0/reki/format/grib/eccodes/operator/
--rw-rw-rw-   0        0        0     3664 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/operator/__init__.py
--rw-rw-rw-   0        0        0      876 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/grib/eccodes/util.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.979578 reki-0.3.0/reki/format/netcdf/
--rw-rw-rw-   0        0        0     1096 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/netcdf/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.980575 reki-0.3.0/reki/format/table/
--rw-rw-rw-   0        0        0     4665 2021-11-24 02:38:19.000000 reki-0.3.0/reki/format/table/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.983576 reki-0.3.0/reki/grib/
--rw-rw-rw-   0        0        0        0 2021-11-24 02:38:19.000000 reki-0.3.0/reki/grib/__init__.py
--rw-rw-rw-   0        0        0      270 2021-11-24 02:38:19.000000 reki-0.3.0/reki/grib/eccodes.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.985576 reki-0.3.0/reki/operator/
--rw-rw-rw-   0        0        0       89 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.989221 reki-0.3.0/reki/operator/area/
--rw-rw-rw-   0        0        0      669 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/area/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.995217 reki-0.3.0/reki/operator/regrid/
--rw-rw-rw-   0        0        0     1369 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/regrid/__init__.py
--rw-rw-rw-   0        0        0     1726 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/regrid/_interpolator.py
--rw-rw-rw-   0        0        0     5019 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/regrid/_scipy.py
--rw-rw-rw-   0        0        0      924 2021-11-24 02:38:19.000000 reki-0.3.0/reki/operator/regrid/_xarray.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.996218 reki-0.3.0/reki/source/
--rw-rw-rw-   0        0        0        0 2021-11-24 02:38:19.000000 reki-0.3.0/reki/source/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.998216 reki-0.3.0/reki/source/gdata/
--rw-rw-rw-   0        0        0     2558 2021-11-24 02:38:19.000000 reki-0.3.0/reki/source/gdata/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:04.000218 reki-0.3.0/reki/source/gdata/transport/
--rw-rw-rw-   0        0        0      259 2021-11-24 02:38:19.000000 reki-0.3.0/reki/source/gdata/transport/__init__.py
--rw-rw-rw-   0        0        0     1868 2021-11-24 02:38:19.000000 reki-0.3.0/reki/source/gdata/transport/transport_pb2.py
-drwxrwxrwx   0        0        0        0 2021-11-24 02:42:03.836957 reki-0.3.0/reki.egg-info/
--rw-rw-rw-   0        0        0    11411 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4157 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      135 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-11-24 02:42:02.000000 reki-0.3.0/reki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-24 02:42:04.004217 reki-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1872 2021-11-24 02:38:19.000000 reki-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.328387 reki-2024.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.284387 reki-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.296387 reki-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 08:16:13.000000 reki-2024.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 08:16:13.000000 reki-2024.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-09 08:16:13.000000 reki-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 08:16:13.000000 reki-2024.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-09 08:16:13.000000 reki-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 08:16:13.000000 reki-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23108 2024-04-09 08:16:21.328387 reki-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-09 08:16:13.000000 reki-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.296387 reki-2024.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.296387 reki-2024.4.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/doc/source/develop/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.300387 reki-2024.4.0/doc/source/develop/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/develop/api/data_finder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/develop/api/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/develop/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.300387 reki-2024.4.0/doc/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/getting-started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/getting-started/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/getting-started/quick-overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.300387 reki-2024.4.0/doc/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/data_find.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/data_load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/data_process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/load_grads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/load_grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/load_netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/guide/load_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 08:16:13.000000 reki-2024.4.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-09 08:16:13.000000 reki-2024.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.300387 reki-2024.4.0/reki/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 08:16:21.000000 reki-2024.4.0/reki/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cm/glob/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cm/glob/fnl.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cm/glob/gfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cm/glob/gfs/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cm/glob/gfs/grib2/0p50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cm/glob/gfs/grib2/1p00.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_geps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_geps/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_geps/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_gfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_gfs/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_gfs/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_meso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_meso/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_meso/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_reps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_reps/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_reps/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_tym/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_tym/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/cmadaas/cma_tym/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/exp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/exp/cma_gfs_gmf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/exp/cma_gfs_gmf/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/exp/cma_gfs_gmf/grib2/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/exp/cma_gfs_gmf/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/od/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/od/cma_geps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.304387 reki-2024.4.0/reki/data_finder/conf/od/cma_geps/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_geps/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.288387 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/modelvar_ctl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/postvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/postvar_ctl.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/ne.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/r2cwe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rgwst.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rsing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rsurf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rtemp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/modelvar_ctl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/postvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/postvar_ctl.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/grib2/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/modelvar_ctl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/postvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/postvar_ctl.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.308387 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/cloud.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/modelvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/od/cma_reps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/od/cma_reps/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_reps/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/bin/postvar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/bin/postvar_ctl.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/grib2/orig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/od/cma_tym/grib2/sfc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/cma_meso_1km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/smart2022/cma_meso_1km/grib2/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/smart2022/cma_meso_1km/grib2/orig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/chn/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/HRCLDAS/chn/1km.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/RMAPS_IN/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/grid/RMAPS_IN/bth.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/station/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/station/cmadaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/smart2022/obs/station/cmadaas/olympics.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/vfy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.292387 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_01.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_03.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_06.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/rain_24.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/grid/ana/sfc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/conf/vfy/muvos/obs/gts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/data_finder/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/format/grads/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grads/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grads/grads_ctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grads/grads_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grads/grads_record_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.312387 reki-2024.4.0/reki/format/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/grib/cfgrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/cfgrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/cfgrib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/cfgrib/field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/grib/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/common/_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/common/_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/grib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/config/cemc-param-table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/config/cemc_param_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/config/wgrib2_short_name.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/config/wgrib2_short_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/grib/eccodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/grib/eccodes/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/grib/eccodes/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.316387 reki-2024.4.0/reki/format/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/netcdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/format/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/format/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/grib/eccodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/operator/area/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/area/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/operator/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/regrid/_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/regrid/_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/operator/regrid/_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/source/gdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/source/gdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/reki/source/gdata/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/source/gdata/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/source/gdata/transport/transport.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 08:16:13.000000 reki-2024.4.0/reki/source/gdata/transport/transport_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.324387 reki-2024.4.0/reki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23108 2024-04-09 08:16:21.000000 reki-2024.4.0/reki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-09 08:16:21.000000 reki-2024.4.0/reki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:16:21.000000 reki-2024.4.0/reki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 08:16:21.000000 reki-2024.4.0/reki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 08:16:21.000000 reki-2024.4.0/reki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:16:21.328387 reki-2024.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/tests/format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/tests/format/grads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grads/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grads/test_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grads/test_level_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grads/test_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.320387 reki-2024.4.0/tests/format/grib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.324387 reki-2024.4.0/tests/format/grib/eccodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.324387 reki-2024.4.0/tests/format/grib/eccodes/field/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/test_field_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/test_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/test_level_dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/test_level_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/field/test_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.324387 reki-2024.4.0/tests/format/grib/eccodes/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/message/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/message/test_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/message/test_level_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/message/test_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:21.324387 reki-2024.4.0/tests/format/grib/eccodes/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-09 08:16:13.000000 reki-2024.4.0/tests/format/grib/eccodes/system/test_load_field_meso.py
```

### Comparing `reki-0.3.0/README.md` & `reki-2024.4.0/reki/format/grib/cfgrib/field.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,249 +1,254 @@
-# reki
-
-A data tool for CEMC.
-
-Load GRIB2 data using [eccodes](https://github.com/ecmwf/eccodes-python)
-or [cfgrib](https://github.com/ecmwf/cfgrib).
-
-## Installation
-
-Download the latest source code from GitHub and install using `pip`.
-
-If you are using system python, such as `apps/python/3.6.3/gnu` on HPC CMA-PI,
-please use `--user` option to install on user directory.
-
-`reki` uses ecCodes to decode GRIB files
-(which is needed by [eccodes](https://github.com/ecmwf/eccodes-python) and [cfgrib](https://github.com/ecmwf/cfgrib)). 
-Please install ecCodes through conda or other package source.
-
-## Getting started
-
-`reki` has several functions to help users to find one filed from a local GRIB 2 file.
-
-`load_message_from_file` from `reki.format.grib.eccodes` returns a GRIB handler.
-Users can use it to get attrs or values with functions from [eccodes](https://github.com/ecmwf/eccodes-python) .
-
-For example, load 850hPa temperature from GRAPES GFS and get values from the returned message.
-
-```pycon
->>> from reki.format.grib.eccodes import load_message_from_file
->>> t = load_message_from_file(
-...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-...     parameter="t",
-...     level_type="isobaricInhPa",
-...     level=850,
-... )
->>> data = eccodes.codes_get_double_array(t, "values")
->>> data = data.reshape([720, 1440])
->>> data
-array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
-    249.19234375, 249.14234375],
-   [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
-    249.44234375, 249.44234375],
-   [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
-    249.67234375, 249.68234375],
-   ...,
-   [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
-    235.63234375, 235.48234375],
-   [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
-    235.72234375, 235.82234375],
-   [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
-    235.68234375, 235.70234375]])
-```
-
-**NOTE**: Please release the handler using `eccodes.codes_release` manually.
-
-`eccodes` engine also provides some functions to load array from GRIB2 file
-in which GRIB2 message is loaded by [eccodes-python](https://github.com/ecmwf/eccodes-python)
-and converted into `xarray.DataArray` by `nwpc-data`.
-
-**WARNING**: This feature is under construction.
-
-```pycon
->>> from reki.format.grib.eccodes import load_field_from_file
->>> load_field_from_file(
-...     file_path="/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-...     parameter="t",
-...     level_type="isobaricInhPa",
-...     level=850,
-... )
-<xarray.DataArray 't' (latitude: 720, longitude: 1440)>
-array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
-        249.19234375, 249.14234375],
-       [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
-        249.44234375, 249.44234375],
-       [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
-        249.67234375, 249.68234375],
-       ...,
-       [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
-        235.63234375, 235.48234375],
-       [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
-        235.72234375, 235.82234375],
-       [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
-        235.68234375, 235.70234375]])
-Coordinates:
-    time           datetime64[ns] 2020-03-18
-    step           timedelta64[ns] 4 days 09:00:00
-    valid_time     datetime64[ns] 2020-03-22T09:00:00
-    isobaricInhPa  int64 850
-  * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
-  * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
-Attributes:
-    GRIB_edition:                    2
-    GRIB_centre:                     babj
-    GRIB_subCentre:                  0
-    GRIB_tablesVersion:              4
-    GRIB_localTablesVersion:         1
-    GRIB_dataType:                   fc
-    GRIB_dataDate:                   20200318
-    GRIB_dataTime:                   0
-    GRIB_validityDate:               20200322
-    GRIB_validityTime:               900
-    GRIB_step:                       105
-    GRIB_stepType:                   instant
-    GRIB_stepUnits:                  1
-    GRIB_stepRange:                  105
-    GRIB_endStep:                    105
-    GRIB_name:                       Temperature
-    GRIB_shortName:                  t
-    GRIB_cfName:                     air_temperature
-    GRIB_discipline:                 0
-    GRIB_parameterCategory:          0
-    GRIB_parameterNumber:            0
-    GRIB_gridType:                   regular_ll
-    GRIB_gridDefinitionDescription:  Latitude/longitude 
-    GRIB_typeOfFirstFixedSurface:    pl
-    GRIB_typeOfLevel:                isobaricInhPa
-    GRIB_level:                      850
-    GRIB_numberOfPoints:             1036800
-    GRIB_missingValue:               9999
-    GRIB_units:                      K
-    long_name:                       Temperature
-    units:                           K
-```
-
-## Engines
-
-`reki` loads GRIB2 file using `eccodes` by default and also supports `cfgrib`.
-
-### cfgrib
-
-If you don't care about loading speed, please use [cfgrib](https://github.com/ecmwf/cfgrib) engine
-with option `engine="cfgrib"`.
-
-Please install cfgrib before using this engine.
-
-Read 850hPa temperature from a GRAEPS GFS grib2 file using `shortName` key `t`.
-( `shortName` is an ecCodes key. )
-
-```pycon
->>> load_field_from_file(
-...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-...     parameter="t",
-...     level_type="isobaricInhPa",
-...     level=850,
-...     engine="cfgrib",
-... )
-<xarray.DataArray 't' (latitude: 720, longitude: 1440)>
-[1036800 values with dtype=float32]
-Coordinates:
-    time           datetime64[ns] ...
-    step           timedelta64[ns] ...
-    isobaricInhPa  int64 ...
-  * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
-  * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
-    valid_time     datetime64[ns] ...
-Attributes:
-    GRIB_paramId:                             130
-    GRIB_shortName:                           t
-    GRIB_units:                               K
-    GRIB_name:                                Temperature
-    GRIB_cfName:                              air_temperature
-    GRIB_cfVarName:                           t
-    GRIB_dataType:                            fc
-    GRIB_missingValue:                        9999
-    GRIB_numberOfPoints:                      1036800
-    GRIB_typeOfLevel:                         isobaricInhPa
-    GRIB_NV:                                  0
-    GRIB_stepUnits:                           1
-    GRIB_stepType:                            instant
-    GRIB_gridType:                            regular_ll
-    GRIB_gridDefinitionDescription:           Latitude/longitude
-    GRIB_Nx:                                  1440
-    GRIB_iDirectionIncrementInDegrees:        0.25
-    GRIB_iScansNegatively:                    0
-    GRIB_longitudeOfFirstGridPointInDegrees:  0.0
-    GRIB_longitudeOfLastGridPointInDegrees:   359.75
-    GRIB_Ny:                                  720
-    GRIB_jDirectionIncrementInDegrees:        0.25
-    GRIB_jPointsAreConsecutive:               0
-    GRIB_jScansPositively:                    0
-    GRIB_latitudeOfFirstGridPointInDegrees:   89.875
-    GRIB_latitudeOfLastGridPointInDegrees:    -89.875
-    long_name:                                Temperature
-    units:                                    K
-    standard_name:                            air_temperature
-```
-
-If the field doesn't have a `shortName`, use `dict` for `parameter`.
-
-Load a filed without shortName.
-
-```pycon
->>> load_field_from_file(
-...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-...     parameter={
-...         "discipline": 0,
-...         "parameterCategory": 2,
-...         "parameterNumber": 225,
-...     },
-...     level_type="isobaricInhPa",
-...     level=850,
-... )
-<xarray.DataArray 'paramId_0' (latitude: 720, longitude: 1440)>
-[1036800 values with dtype=float32]
-Coordinates:
-    time           datetime64[ns] ...
-    step           timedelta64[ns] ...
-    isobaricInhPa  int64 ...
-  * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
-  * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
-    valid_time     datetime64[ns] ...
-Attributes:
-    GRIB_paramId:                             0
-    GRIB_dataType:                            fc
-    GRIB_missingValue:                        9999
-    GRIB_numberOfPoints:                      1036800
-    GRIB_typeOfLevel:                         isobaricInhPa
-    GRIB_NV:                                  0
-    GRIB_stepUnits:                           1
-    GRIB_stepType:                            instant
-    GRIB_gridType:                            regular_ll
-    GRIB_gridDefinitionDescription:           Latitude/longitude
-    GRIB_Nx:                                  1440
-    GRIB_iDirectionIncrementInDegrees:        0.25
-    GRIB_iScansNegatively:                    0
-    GRIB_longitudeOfFirstGridPointInDegrees:  0.0
-    GRIB_longitudeOfLastGridPointInDegrees:   359.75
-    GRIB_Ny:                                  720
-    GRIB_jDirectionIncrementInDegrees:        0.25
-    GRIB_jPointsAreConsecutive:               0
-    GRIB_jScansPositively:                    0
-    GRIB_latitudeOfFirstGridPointInDegrees:   89.875
-    GRIB_latitudeOfLastGridPointInDegrees:    -89.875
-    GRIB_discipline:                          0
-    GRIB_parameterCategory:                   2
-    GRIB_parameterNumber:                     225
-    long_name:                                original GRIB paramId: 0
-    units:                                    1
-```
-
-## Examples
-
-See `example` directory for more examples.
-
-## LICENSE
-
-Copyright &copy; 2020-2021, developers at cemc-oper.
-
-`reki` is licensed under [GPL v3.0](LICENSE.md)
+from typing import Dict, Union, Optional
+from pathlib import Path
+
+import xarray as xr
+
+from reki.format.grib.common import fix_level_type
+
+from ._util import (
+    _fill_parameter,
+    _fill_level,
+    _fill_level_type,
+    _fill_level_value,
+    _fill_index_path,
+)
+from reki._util import _load_first_variable
+
+
+def load_field_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict],
+        level_type: Union[str, Dict],
+        level: Union[int, float] = None,
+        with_index: Union[str, bool] = False,
+) -> Optional[xr.DataArray]:
+    """
+    Load **one** field from GRIB2 file using `ecmwf/cfgrib <https://github.com/ecmwf/cfgrib>`_.
+
+    This function loads the first data fitting searching conditions.
+
+    Parameters
+    ----------
+    file_path: str or Path
+        GRIB2 file path
+    parameter: str or Dict
+        parameter identifier. support two types:
+
+        * str: parameter name, see shortName key using grib_ls of ecCodes.
+        * Dict: parameter keys, including:
+
+            * discipline
+            * parameterCategory
+            * parameterNumber
+
+    level_type: str or Dict
+        level type, see typeOfLevel key using grib_ls of ecCodes.
+    level: int or float or None
+        level value. If none, all levels will be loaded.
+    with_index: str or bool
+        use index file generated by cfgrib.
+        if False, index file will not be used.
+        if True, cfgrib will generate index file.
+
+    Returns
+    -------
+    xr.DataArray or None:
+        `xr.DataArray` if found one data, or None if not.
+
+    Examples
+    --------
+    Read 850hPa temperature from a GRAEPS GFS grib2 file.
+    >>> load_field_from_file(
+   ...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
+   ...     parameter="t",
+   ...     level_type="isobaricInhPa",
+   ...     level=850,
+   ... )
+    <xarray.DataArray 't' (latitude: 720, longitude: 1440)>
+    [1036800 values with dtype=float32]
+    Coordinates:
+        time           datetime64[ns] ...
+        step           timedelta64[ns] ...
+        isobaricInhPa  int64 ...
+      * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
+      * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
+        valid_time     datetime64[ns] ...
+    Attributes:
+        GRIB_paramId:                             130
+        GRIB_shortName:                           t
+        GRIB_units:                               K
+        GRIB_name:                                Temperature
+        GRIB_cfName:                              air_temperature
+        GRIB_cfVarName:                           t
+        GRIB_dataType:                            fc
+        GRIB_missingValue:                        9999
+        GRIB_numberOfPoints:                      1036800
+        GRIB_typeOfLevel:                         isobaricInhPa
+        GRIB_NV:                                  0
+        GRIB_stepUnits:                           1
+        GRIB_stepType:                            instant
+        GRIB_gridType:                            regular_ll
+        GRIB_gridDefinitionDescription:           Latitude/longitude
+        GRIB_Nx:                                  1440
+        GRIB_iDirectionIncrementInDegrees:        0.25
+        GRIB_iScansNegatively:                    0
+        GRIB_longitudeOfFirstGridPointInDegrees:  0.0
+        GRIB_longitudeOfLastGridPointInDegrees:   359.75
+        GRIB_Ny:                                  720
+        GRIB_jDirectionIncrementInDegrees:        0.25
+        GRIB_jPointsAreConsecutive:               0
+        GRIB_jScansPositively:                    0
+        GRIB_latitudeOfFirstGridPointInDegrees:   89.875
+        GRIB_latitudeOfLastGridPointInDegrees:    -89.875
+        long_name:                                Temperature
+        units:                                    K
+        standard_name:                            air_temperature
+
+    Load a filed without shortName.
+    >>> load_field_from_file(
+    ...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
+    ...     parameter={
+    ...         "discipline": 0,
+    ...         "parameterCategory": 2,
+    ...         "parameterNumber": 225,
+    ...     },
+    ...     level_type="isobaricInhPa",
+    ...     level=850,
+    ... )
+    <xarray.DataArray 'paramId_0' (latitude: 720, longitude: 1440)>
+    [1036800 values with dtype=float32]
+    Coordinates:
+        time           datetime64[ns] ...
+        step           timedelta64[ns] ...
+        isobaricInhPa  int64 ...
+      * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
+      * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
+        valid_time     datetime64[ns] ...
+    Attributes:
+        GRIB_paramId:                             0
+        GRIB_dataType:                            fc
+        GRIB_missingValue:                        9999
+        GRIB_numberOfPoints:                      1036800
+        GRIB_typeOfLevel:                         isobaricInhPa
+        GRIB_NV:                                  0
+        GRIB_stepUnits:                           1
+        GRIB_stepType:                            instant
+        GRIB_gridType:                            regular_ll
+        GRIB_gridDefinitionDescription:           Latitude/longitude
+        GRIB_Nx:                                  1440
+        GRIB_iDirectionIncrementInDegrees:        0.25
+        GRIB_iScansNegatively:                    0
+        GRIB_longitudeOfFirstGridPointInDegrees:  0.0
+        GRIB_longitudeOfLastGridPointInDegrees:   359.75
+        GRIB_Ny:                                  720
+        GRIB_jDirectionIncrementInDegrees:        0.25
+        GRIB_jPointsAreConsecutive:               0
+        GRIB_jScansPositively:                    0
+        GRIB_latitudeOfFirstGridPointInDegrees:   89.875
+        GRIB_latitudeOfLastGridPointInDegrees:    -89.875
+        GRIB_discipline:                          0
+        GRIB_parameterCategory:                   2
+        GRIB_parameterNumber:                     225
+        long_name:                                original GRIB paramId: 0
+        units:                                    1
+
+
+    """
+    data_set = load_fields_from_file(
+        file_path=file_path,
+        parameter=parameter,
+        level_type=level_type,
+        level=level,
+        with_index=with_index
+    )
+
+    if data_set is None:
+        return None
+
+    return _load_first_variable(data_set)
+
+
+def load_fields_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict] = None,
+        level_type: str = None,
+        level: Union[int, float] = None,
+        with_index: Union[str, bool] = False,
+) -> Optional[xr.Dataset]:
+    """
+    Load fields from GRIB2 file using `ecmwf/cfgrib <https://github.com/ecmwf/cfgrib>`_.
+
+    Parameters
+    ----------
+    file_path: str or Path
+        GRIB2 data file path
+    parameter: str or Dict
+        see `load_message_from_file`
+    level_type: str
+        see `load_message_from_file`
+    level: int or float or None
+        see `load_message_from_file`
+    with_index: str or bool
+        see `load_message_from_file`
+
+    Returns
+    -------
+    xr.Dataset or None:
+        `xr.Dataset` if found, or None if not.
+
+    Examples
+    --------
+    >>> load_fields_from_file(
+    ...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
+    ...     parameter="t",
+    ...     level_type="isobaricInhPa",
+    ... )
+    <xarray.Dataset>
+    Dimensions:        (isobaricInhPa: 36, latitude: 720, longitude: 1440)
+    Coordinates:
+        time           datetime64[ns] ...
+        step           timedelta64[ns] ...
+      * isobaricInhPa  (isobaricInhPa) int64 1000 975 950 925 900 850 ... 5 4 3 2 1
+      * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
+      * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
+        valid_time     datetime64[ns] ...
+    Data variables:
+        t              (isobaricInhPa, latitude, longitude) float32 ...
+    Attributes:
+        GRIB_edition:            2
+        GRIB_centre:             babj
+        GRIB_centreDescription:  Beijing
+        GRIB_subCentre:          0
+        Conventions:             CF-1.7
+        institution:             Beijing
+        history:                 2020-03-20T08:15:39 GRIB to CDM+CF via cfgrib-0....
+
+    """
+    filter_by_keys = {}
+    read_keys = []
+
+    if parameter is not None:
+        _fill_parameter(parameter, filter_by_keys, read_keys)
+
+    if level_type is not None:
+        level_type = fix_level_type(level_type, engine="cfgrib")
+        _fill_level_type(level_type, filter_by_keys, read_keys)
+
+    if level is not None and level != "all":
+        _fill_level_value(level, filter_by_keys, read_keys)
+
+    backend_kwargs = {
+        "filter_by_keys": filter_by_keys
+    }
+    if len(read_keys) > 0:
+        backend_kwargs["read_keys"] = read_keys
+
+    _fill_index_path(with_index, backend_kwargs)
+
+    data_set = xr.open_dataset(
+        file_path,
+        engine="cfgrib",
+        backend_kwargs=backend_kwargs
+    )
+
+    return data_set
```

### Comparing `reki-0.3.0/reki/data_finder/__main__.py` & `reki-2024.4.0/reki/data_finder/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import argparse
-
-import click
-import pandas as pd
-
-from ._config import (
-    get_default_local_config_path,
-    find_config,
-    load_config,
-)
-from ._util import find_file
-
-
-def main():
-    cli()
-
-
-def print_local_help(ctx, param, value):
-    if value is False:
-        return
-    click.echo(ctx.get_help())
-
-    click.echo("\nDifferent steams use different additional options.\n")
-
-    oper_parser = create_oper_option_parser()
-    click.echo(oper_parser.format_help())
-
-    eps_parser = create_eps_option_parser()
-    click.echo(eps_parser.format_help())
-
-    ctx.exit()
-
-
-@click.group()
-def cli():
-    pass
-
-
-@cli.command("local", context_settings=dict(
-    ignore_unknown_options=True,
-))
-@click.option("--data-type", required=True, help="data type, such as grapes_gfs_gmf/grib2/orig")
-@click.option("--data-level", default="archive,storage", help="data level, split by comma, such as archive, storage")
-@click.option("--data-class", default="od", help="data class, od or cm")
-@click.option("--config-dir", default=None, help="config directory")
-@click.option(
-    "--help", "-h",
-    is_flag=True,
-    expose_value=False,
-    is_eager=True,
-    callback=print_local_help,
-    help="Show this message and exit.")
-@click.argument('query_args', nargs=-1, type=click.UNPROCESSED)
-@click.pass_context
-def find_local(ctx, data_type, data_level, data_class, config_dir, query_args):
-    if config_dir is None:
-        config_dir = get_default_local_config_path()
-
-    config_file_path = find_config(config_dir, data_type, data_class)
-    if config_file_path is None:
-        raise ValueError(f"data type is not found: {data_type}")
-
-    if data_level == "":
-        data_level = None
-    else:
-        data_level = data_level.split(",")
-
-    config = load_config(config_file_path)
-
-    stream = config["query"]["stream"]
-
-    if stream in ("oper", "cm"):
-        find_oper_file(config, data_level, query_args)
-    elif stream == "eps":
-        find_eps_file(config, data_level, query_args)
-    else:
-        raise ValueError(f"stream type is not supported: {stream}")
-
-
-def find_oper_file(config: dict, data_level: str, query_args: tuple):
-    parser = create_oper_option_parser()
-    args = parser.parse_args(query_args)
-
-    forecast_time = pd.to_timedelta(args.forecast_time)
-    start_time = pd.to_datetime(args.start_time, format="%Y%m%d%H")
-
-    file_path = find_file(config, data_level, start_time, forecast_time)
-    if file_path is None:
-        print("None")
-    else:
-        print(file_path)
-
-
-def find_eps_file(config: dict, data_level: str, query_args: tuple):
-    parser = create_eps_option_parser()
-    args = parser.parse_args(query_args)
-
-    forecast_time = pd.to_timedelta(args.forecast_time)
-    start_time = pd.to_datetime(args.start_time, format="%Y%m%d%H")
-
-    file_path = find_file(config, data_level, start_time, forecast_time, number=args.number)
-    if file_path is None:
-        print("None")
-    else:
-        print(file_path)
-
-
-def create_oper_option_parser():
-    parser = argparse.ArgumentParser(
-        description='Additional options for stream oper.',
-        usage=None,
-        add_help=False
-    )
-    parser.add_argument(
-        '--start-time',
-        dest="start_time",
-        help='start time, such as YYYMMDDHH'
-    )
-    parser.add_argument(
-        '--forecast-time',
-        dest='forecast_time',
-        default="0h",
-        help='forecast time, such as 3h'
-    )
-    return parser
-
-
-def create_eps_option_parser():
-    parser = argparse.ArgumentParser(
-        description='Additional options for stream eps.',
-        usage=None,
-        add_help=False
-    )
-    parser.add_argument(
-        '--start-time',
-        dest="start_time",
-        help='start time, such as YYYMMDDHH'
-    )
-    parser.add_argument(
-        '--forecast-time',
-        dest='forecast_time',
-        default="0h",
-        help='forecast time, such as 3h'
-    )
-    parser.add_argument(
-        '--number',
-        dest='number',
-        type=int,
-        help='member number')
-    return parser
-
-
-# copy from argparse module
-def _format_help(parser: argparse.ArgumentParser):
-    """
-    Notes
-    -----
-    This is an experimental function. Do not use it.
-    """
-    formatter = parser._get_formatter()
-
-    # description
-    formatter.add_text(parser.description)
-
-    # positionals, optionals and user-defined groups
-    for action_group in parser._action_groups:
-        formatter.start_section(action_group.title)
-        formatter.add_text(action_group.description)
-        formatter.add_arguments(action_group._group_actions)
-        formatter.end_section()
-
-    # epilog
-    # formatter.add_text(parser.epilog)
-
-    # determine help from format above
-    return formatter.format_help()
-
-
-if __name__ == "__main__":
-    cli()
+import argparse
+
+import click
+import pandas as pd
+
+from ._config import (
+    get_default_local_config_path,
+    find_config,
+    load_config,
+)
+from ._util import find_file
+
+
+def main():
+    cli()
+
+
+def print_local_help(ctx, param, value):
+    if value is False:
+        return
+    click.echo(ctx.get_help())
+
+    click.echo("\nDifferent steams use different additional options.\n")
+
+    oper_parser = create_oper_option_parser()
+    click.echo(oper_parser.format_help())
+
+    eps_parser = create_eps_option_parser()
+    click.echo(eps_parser.format_help())
+
+    ctx.exit()
+
+
+@click.group()
+def cli():
+    pass
+
+
+@cli.command("local", context_settings=dict(
+    ignore_unknown_options=True,
+))
+@click.option("--data-type", required=True, help="data type, such as cma_gfs_gmf/grib2/orig")
+@click.option("--data-level", default="archive,storage", help="data level, split by comma, such as archive, storage")
+@click.option("--data-class", default="od", help="data class, od or cm")
+@click.option("--config-dir", default=None, help="config directory")
+@click.option(
+    "--help", "-h",
+    is_flag=True,
+    expose_value=False,
+    is_eager=True,
+    callback=print_local_help,
+    help="Show this message and exit.")
+@click.argument('query_args', nargs=-1, type=click.UNPROCESSED)
+@click.pass_context
+def find_local(ctx, data_type, data_level, data_class, config_dir, query_args):
+    if config_dir is None:
+        config_dir = get_default_local_config_path()
+
+    config_file_path = find_config(config_dir, data_type, data_class)
+    if config_file_path is None:
+        raise ValueError(f"data type is not found: {data_type}")
+
+    if data_level == "":
+        data_level = None
+    else:
+        data_level = data_level.split(",")
+
+    config = load_config(config_file_path)
+
+    stream = config["query"]["stream"]
+
+    if stream in ("oper", "cm"):
+        find_oper_file(config, data_level, query_args)
+    elif stream == "eps":
+        find_eps_file(config, data_level, query_args)
+    else:
+        raise ValueError(f"stream type is not supported: {stream}")
+
+
+def find_oper_file(config: dict, data_level: str, query_args: tuple):
+    parser = create_oper_option_parser()
+    args = parser.parse_args(query_args)
+
+    forecast_time = pd.to_timedelta(args.forecast_time)
+    start_time = pd.to_datetime(args.start_time, format="%Y%m%d%H")
+
+    file_path = find_file(config, data_level, start_time, forecast_time)
+    if file_path is None:
+        print("None")
+    else:
+        print(file_path)
+
+
+def find_eps_file(config: dict, data_level: str, query_args: tuple):
+    parser = create_eps_option_parser()
+    args = parser.parse_args(query_args)
+
+    forecast_time = pd.to_timedelta(args.forecast_time)
+    start_time = pd.to_datetime(args.start_time, format="%Y%m%d%H")
+
+    file_path = find_file(config, data_level, start_time, forecast_time, number=args.number)
+    if file_path is None:
+        print("None")
+    else:
+        print(file_path)
+
+
+def create_oper_option_parser():
+    parser = argparse.ArgumentParser(
+        description='Additional options for stream oper.',
+        usage=None,
+        add_help=False
+    )
+    parser.add_argument(
+        '--start-time',
+        dest="start_time",
+        help='start time, such as YYYMMDDHH'
+    )
+    parser.add_argument(
+        '--forecast-time',
+        dest='forecast_time',
+        default="0h",
+        help='forecast time, such as 3h'
+    )
+    return parser
+
+
+def create_eps_option_parser():
+    parser = argparse.ArgumentParser(
+        description='Additional options for stream eps.',
+        usage=None,
+        add_help=False
+    )
+    parser.add_argument(
+        '--start-time',
+        dest="start_time",
+        help='start time, such as YYYMMDDHH'
+    )
+    parser.add_argument(
+        '--forecast-time',
+        dest='forecast_time',
+        default="0h",
+        help='forecast time, such as 3h'
+    )
+    parser.add_argument(
+        '--number',
+        dest='number',
+        type=int,
+        help='member number')
+    return parser
+
+
+# copy from argparse module
+def _format_help(parser: argparse.ArgumentParser):
+    """
+    Notes
+    -----
+    This is an experimental function. Do not use it.
+    """
+    formatter = parser._get_formatter()
+
+    # description
+    formatter.add_text(parser.description)
+
+    # positionals, optionals and user-defined groups
+    for action_group in parser._action_groups:
+        formatter.start_section(action_group.title)
+        formatter.add_text(action_group.description)
+        formatter.add_arguments(action_group._group_actions)
+        formatter.end_section()
+
+    # epilog
+    # formatter.add_text(parser.epilog)
+
+    # determine help from format above
+    return formatter.format_help()
+
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/grib2/0p50.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_reps/grib2/orig.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-query:
-  system: gfs
-  stream: cm
-  type: grib2
-  name: 0p50
-
-file_name: 'gfs.t{{ time_vars.Hour }}z.pgrb2.0p50.f{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/glob/gfs/{{ time_vars.Year }}/gfs.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/glob/gfs/{{ time_vars.Year }}/gfs.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_reps
+  stream: eps
+  type: grib2
+  name: orig
+
+file_name: "mef.gra.{{ '%.3d' | format(query_vars.number) }}.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2"
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CMA HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/cm/glob/gfs/grib2/1p00.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rsurf.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-query:
-  system: gfs
-  stream: cm
-  type: grib2
-  name: 1p00
-
-file_name: 'gfs.t{{ time_vars.Hour }}z.pgrb2.1p00.f{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/glob/gfs/{{ time_vars.Year }}/gfs.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/glob/gfs/{{ time_vars.Year }}/gfs.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: obs
+  name: rgwst
+
+file_name: 'rec_RSURF_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_geps/grib2/orig.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_geps/grib2/orig.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-query:
-  system: grapes_geps
-  stream: eps
-  type: grib2
-  name: orig
-
-file_name: "gef.gra.{{ '%.3d' | format(query_vars.number) }}.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2"
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp_qu/NWP_GEPS_DATA/GRAPES_GFS_2-1-2-2/GEPS/PRODS/GRIB2/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
-
-  - type: local
-    level: storage
+query:
+  system: cma_geps
+  stream: eps
+  type: grib2
+  name: orig
+
+file_name: "gef.gra.{{ '%.3d' | format(query_vars.number) }}.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2"
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CMA HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_GEPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/modelvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rsing.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: bin
-  name: modelvar
-
-file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp/GRAPES_GFS3.1/MODEL/data/NWP_GMFS/{{ time_vars.Hour }}/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: obs
+  name: rgwst
+
+file_name: 'rec_RSING_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/modelvar_ctl.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/postvar.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: bin
-  name: modelvar_ctl
-
-file_name: 'model.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp/GRAPES_GFS3.1/MODEL/data/NWP_GMFS/{{ time_vars.Hour }}/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
+query:
+  system: grapes_gfs_gmf
+  stream: oper
+  type: bin
+  name: postvar
+
+file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
+
+paths:
+  # CMA-PI
+#  - type: local
+#    level: runtime
+#    path: '/g0/nwp/CMA-GFS4.0_DATA/MODEL/NWP_GMFS/{{ time_vars.Hour }}/output'
+
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/postvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/bin/postvar_ctl.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: bin
-  name: postvar
-
-file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp/GRAPES_GFS3.1/MODEL/data/NWP_GMFS/{{ time_vars.Hour }}/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
+query:
+  system: grapes_gfs_gmf
+  stream: oper
+  type: bin
+  name: postvar_ctl
+
+file_name: 'post.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
+
+paths:
+  # CMA-PI
+#  - type: local
+#    level: runtime
+#    path: '/g0/nwp/CMA-GFS4.0_DATA/MODEL/NWP_GMFS/{{ time_vars.Hour }}/output'
+
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/bin/postvar_ctl.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/cloud.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: bin
-  name: postvar_ctl
-
-file_name: 'post.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}_{{ time_vars.Forecast }}'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp/GRAPES_GFS3.1/MODEL/data/NWP_GMFS/{{ time_vars.Hour }}/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Fcst-long/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: grib2
+  name: cloud
+
+file_name: 'Z_NAFP_C_BABJ_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}0000_P_NWPC-GRAPES-3KM-CN-{{ time_vars.Forecast }}00.grb2'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
+
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/grib2/ne.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rgwst.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: grib2
-  name: ne
-
-file_name: 'ne_gmf.gra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: runtime
-    path: "/g2/nwp_pd/NWP_GRAPES_GFS_GMF_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/togrib2/output/grib2_ne/"
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}/CMACAST'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}/CMACAST'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}/CMACAST'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: obs
+  name: rgwst
+
+file_name: 'rec_RGWST_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_gfs_gmf/obs/r2cwe.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/grib2/modelvar.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-query:
-  system: grapes_gfs_gmf
-  stream: oper
-  type: obs
-  name: rgwst
-
-file_name: 'rec_R2CWE_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_10km
+  stream: oper
+  type: grib2
+  name: modelvar
+
+file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/modelvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/orig.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_10km
-  stream: oper
-  type: bin
-  name: modelvar
-
-file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: grib2
+  name: orig
+
+file_name: 'rmf.hgra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/postvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/modelvar_ctl.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_10km
-  stream: oper
-  type: bin
-  name: postvar
-
-file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: bin
+  name: modelvar_ctl
+
+file_name: 'modelvar.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/bin/postvar_ctl.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_tym/bin/postvar.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_10km
-  stream: oper
-  type: bin
-  name: postvar_ctl
-
-file_name: 'post.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_tym
+  stream: oper
+  type: bin
+  name: postvar
+
+file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/grib2/modelvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/postvar_ctl.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-query:
-  system: grapes_meso_10km
-  stream: oper
-  type: grib2
-  name: modelvar
-
-file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+query:
+  system: cma_meso_10km
+  stream: oper
+  type: bin
+  name: postvar_ctl
+
+file_name: 'post.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_10km/grib2/orig.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/rtemp.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_10km
-  stream: oper
-  type: grib2
-  name: orig
-
-file_name: 'rmf.gra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: obs
+  name: rgwst
+
+file_name: 'rec_RTEMP_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/modelvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/modelvar.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: bin
-  name: modelvar
-
-file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: bin
+  name: modelvar
+
+file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/modelvar_ctl.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/postvar.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: bin
-  name: modelvar_ctl
-
-file_name: 'model.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: bin
+  name: postvar
+
+file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/postvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/bin/postvar_ctl.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: bin
-  name: postvar
-
-file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: bin
+  name: postvar_ctl
+
+file_name: 'postvar.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/bin/postvar_ctl.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/obs/r2cwe.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: bin
-  name: postvar_ctl
-
-file_name: 'post.ctl_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: obs
+  name: rgwst
+
+file_name: 'rec_R2CWE_{{ time_vars.Year4DV }}{{ time_vars.Month4DV }}{{ time_vars.Day4DV }}{{ time_vars.Hour4DV }}{{ query_vars.obs_time.Hour }}{{ query_vars.obs_time.Minute }}_g.dat'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Obs-prep/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/cloud.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/ne.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: grib2
-  name: cloud
-
-file_name: 'Z_NAFP_C_BABJ_{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}0000_P_NWPC-GRAPES-3KM-CN-{{ time_vars.Forecast }}00.grb2'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp_pd/NWP_GRAPES_MESO_3KM_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/togrib2/output_yun'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/YUN'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: grib2
+  name: ne
+
+file_name: 'ne_gmf.gra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  # CMA-PI
+#  - type: local
+#    level: runtime
+#    path: "/g0/nwp_pd/NWP_CMA_GFS_GMF_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/data/output/grib2_ne/"
+
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/CMACAST'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/modelvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_3km/grib2/modelvar.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: grib2
-  name: modelvar
-
-file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp_pd/NWP_GRAPES_MESO_3KM_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/togrib2/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
-
-  - type: local
-    level: storage
+query:
+  system: cma_meso_3km
+  stream: oper
+  type: grib2
+  name: modelvar
+
+file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  # CMA-PI
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  # CEMC Storage
+  - type: local
+    level: storage
     path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_meso_3km/grib2/orig.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/modelvar.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,40 @@
-query:
-  system: grapes_meso_3km
-  stream: oper
-  type: grib2
-  name: orig
-
-file_name: 'rmf.hgra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: runtime
-    path: '/g2/nwp_pd/NWP_GRAPES_MESO_3KM_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/togrib2/output'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_MESO_3KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: grib2
+  name: modelvar
+
+file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  # CMA-PI
+#  - type: local
+#    level: runtime
+#    path: "/g0/nwp_pd/NWP_CMA_GFS_GMF_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/data/output/grib2_orig/"
+
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/MODELVAR'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_reps/grib2/orig.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/postvar.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-query:
-  system: grapes_reps
-  stream: eps
-  type: grib2
-  name: orig
-
-file_name: "mef.gra.{{ '%.3d' | format(query_vars.number) }}.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2"
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_REPS/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/grib2'
+query:
+  system: cma_meso_10km
+  stream: oper
+  type: bin
+  name: postvar
+
+file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_tym/bin/postvar.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/bin/modelvar.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-query:
-  system: grapes_tym
-  stream: oper
-  type: bin
-  name: postvar
-
-file_name: 'postvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_TYM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_10km
+  stream: oper
+  type: bin
+  name: modelvar
+
+file_name: 'modelvar{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}00'
+
+paths:
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Fcst-main/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_tym/grib2/orig.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_gfs_gmf/grib2/orig.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-query:
-  system: grapes_tym
-  stream: oper
-  type: grib2
-  name: orig
-
-file_name: 'rmf.tcgra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_gfs_gmf
+  stream: oper
+  type: grib2
+  name: orig
+
+file_name: 'gmf.gra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  # CMA-PI
+#  - type: local
+#    level: runtime
+#    path: "/g0/nwp_pd/NWP_CMA_GFS_GMF_POST_DATA/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/data/output/grib2_orig/"
+
+  - type: local
+    level: archive
+    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  # HPC2023
+  - type: local
+    level: archive
+    path: '/g3/COMMONDATA/OPER/CEMC/GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  # CMA Storage
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+
+  # CEMC Storage
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_GFS_GMF/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
```

### Comparing `reki-0.3.0/reki/data_finder/conf/od/grapes_tym/grib2/sfc.yaml` & `reki-2024.4.0/reki/data_finder/conf/od/cma_meso_10km/grib2/orig.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-query:
-  system: grapes_tym
-  stream: oper
-  type: grib2
-  name: sfc
-
-file_name: 'TYM.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
-
-paths:
-  - type: local
-    level: archive
-    path: '/g1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
-
-  - type: local
-    level: storage
-    path: '{{ query_vars.storage_base }}/GRAPES_TYM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}'
+query:
+  system: cma_meso_10km
+  stream: oper
+  type: grib2
+  name: orig
+
+file_name: 'rmf.gra.{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}{{ time_vars.Forecast }}.grb2'
+
+paths:
+  - type: local
+    level: storage
+    path: '/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
+
+  - type: local
+    level: storage
+    path: '{{ query_vars.storage_base }}/GRAPES_MESO_10KM/Prod-grib/{{ time_vars.Year }}{{ time_vars.Month }}{{ time_vars.Day }}{{ time_vars.Hour }}/ORIG'
```

### Comparing `reki-0.3.0/reki/data_finder/local.py` & `reki-2024.4.0/reki/data_finder/local.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,149 +1,201 @@
-import datetime
-from typing import Union, Optional, Iterable
-from pathlib import Path
-
-import pandas as pd
-
-from reki.data_finder._config import (
-    find_config, load_config, get_default_local_config_path,
-)
-from reki.data_finder._util import find_file, find_files
-
-
-def find_local_file(
-        data_type: str,
-        start_time: Union[str, pd.Timestamp, datetime.datetime],
-        forecast_time: Union[str, pd.Timedelta] = "0",
-        data_level: Optional[Union[str, Iterable]] = ("archive", "storage"),
-        path_type: str = "local",
-        data_class: str = "od",
-        config_dir: Union[str, Path] = None,
-        obs_time: Union[str, pd.Timestamp] = None,
-        **kwargs,
-) -> Optional[Path]:
-    """Find local data path using config files in config dir.
-
-    Parameters
-    ----------
-    data_type
-        data type, relative path of config file to `config_dir` without suffix.
-        For example `grapes_gfs_gmf/grib2/orig` means using config file `{config_dir}/grapes_gfs_gmf/grib2/orig.yaml`.
-    start_time
-        start time of production. YYYYMMDDHH if str.
-    forecast_time
-        forecast time of production. A string (such as `3h`) will be parsed by ``pd.to_timedelta``.
-    data_level
-        data storage level, ["archive", "runtime", "storage", ... ], default is ``("archive", "storage")``.
-    path_type
-        path type, ["local", "storage", ...], for future usage.
-    data_class
-        data class, ``od`` means operation systems.
-    config_dir
-        config root directory. If None, use embedded config files in `conf` directory.
-    obs_time
-        time for observation data.
-    **kwargs
-        other options needed by path template. All of them will be added into `query_vars`.
-
-    Returns
-    -------
-    Path or None
-        file path if found or None if not.
-
-    Examples
-    --------
-    Find an existing orig grib2 file of GRAPES GFS.
-
-    >>> find_local_file(
-    ...     "grapes_gfs_gmf/grib2/orig",
-    ...     start_time="2020032100",
-    ...     forecast_time="3h",
-    ... )
-    /g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020032021/ORIG/gmf.gra.2020032100003.grb2
-
-    Find a non-existing orig grib2 file of GRAPES GFS.
-    >>> find_local_file(
-    ...     "grapes_gfs_gmf/grib2/orig",
-    ...     start_time="2020032100",
-    ...     forecast_time="1h",
-    ... )
-    None
-
-    Find a grib2 file in storage for GRAPES MESO 3km.
-    >>> find_local_file(
-    ...     "grapes_meso_3km/grib2/orig",
-    ...     start_time="2020032100",
-    ...     forecast_time="1h",
-    ...     data_level="storage",
-    ... )
-    /sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/2020032021/ORIG/rmf.hgra.2020032100001.grb2
-
-    Find a grib2 file in storage for GRAPES GEPS.
-    >>> find_local_file(
-    ...     "grapes_geps/grib2/orig",
-    ...     start_time="2020032100",
-    ...     forecast_time="3h",
-    ...     data_level="storage",
-    ...     number=1,
-    ... )
-    /sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/2020032100/grib2/gef.gra.001.2020032100003.grb2
-
-    Find GRAPES TYM postvar ctl file in Windows mount storage.
-    >>> find_local_file("grapes_tym/bin/postvar_ctl", start_time="2021080200", storage_base="Y:")
-    WindowsPath('Y:/GRAPES_TYM/Fcst-main/2021080200/post.ctl_2021080200')
-
-    """
-    if config_dir is None:
-        config_dir = get_default_local_config_path()
-
-    config_file_path = find_config(config_dir, data_type, data_class)
-    if config_file_path is None:
-        raise ValueError(f"data type is not found: {data_type}")
-
-    if isinstance(forecast_time, str):
-        forecast_time = pd.to_timedelta(forecast_time)
-    if isinstance(start_time, str):
-        start_time = pd.to_datetime(start_time, format="%Y%m%d%H")
-    if isinstance(obs_time, str):
-        obs_time = pd.to_datetime(obs_time)
-    elif obs_time is None:
-        obs_time = start_time
-
-    config = load_config(config_file_path)
-    file_path = find_file(
-        config,
-        data_level,
-        start_time,
-        forecast_time,
-        obs_time=obs_time,
-        **kwargs
-    )
-    return file_path
-
-
-def find_local_files(
-        data_type: str,
-        start_time: Union[str, pd.Timestamp, datetime.datetime],
-        forecast_time: Union[str, pd.Timedelta] = "0",
-        data_level: Optional[Union[str, Iterable]] = ("archive", "storage"),
-        path_type: str = "local",
-        data_class: str = "od",
-        config_dir: Union[str, Path] = None,
-        glob: bool = True,
-        **kwargs,
-) -> Optional[Path]:
-    if config_dir is None:
-        config_dir = get_default_local_config_path()
-
-    config_file_path = find_config(config_dir, data_type, data_class)
-    if config_file_path is None:
-        raise ValueError(f"data type is not found: {data_type}")
-
-    if isinstance(forecast_time, str):
-        forecast_time = pd.to_timedelta(forecast_time)
-    if isinstance(start_time, str):
-        start_time = pd.to_datetime(start_time, format="%Y%m%d%H")
-
-    config = load_config(config_file_path)
-    file_path = find_files(config, data_level, start_time, forecast_time, glob, **kwargs)
-    return file_path
+import datetime
+from typing import Union, Optional, Iterable
+from pathlib import Path
+
+import pandas as pd
+
+from reki.data_finder._config import (
+    find_config, load_config, get_default_local_config_path,
+)
+from reki.data_finder._util import find_file, find_files, render_file_name
+
+
+def find_local_file(
+        data_type: str,
+        start_time: Union[str, pd.Timestamp, datetime.datetime],
+        forecast_time: Union[str, pd.Timedelta] = "0",
+        data_level: Optional[Union[str, Iterable]] = ("archive", "storage"),
+        path_type: str = "local",
+        data_class: str = "od",
+        config_dir: Union[str, Path] = None,
+        obs_time: Union[str, pd.Timestamp] = None,
+        debug: bool = False,
+        **kwargs,
+) -> Optional[Path]:
+    """
+    Find local data path using config files in config dir.
+
+    Parameters
+    ----------
+    data_type
+        data type, relative path of config file to `config_dir` without suffix.
+        For example `grapes_gfs_gmf/grib2/orig` means using config file `{config_dir}/grapes_gfs_gmf/grib2/orig.yaml`.
+    start_time
+        start time of production. YYYYMMDDHH if str.
+    forecast_time
+        forecast time of production. A string (such as `3h`) will be parsed by ``pd.to_timedelta``.
+    data_level
+        data storage level, ["archive", "runtime", "storage", ... ], default is ``("archive", "storage")``.
+    path_type
+        path type, ["local", "storage", ...], for future usage.
+    data_class
+        data class, ``od`` means operation systems.
+    config_dir
+        config root directory. If None, use embedded config files in `conf` directory.
+    obs_time
+        time for observation data.
+    debug
+        show debug info.
+    **kwargs
+        other options needed by path template. All of them will be added into `query_vars`.
+
+    Returns
+    -------
+    Path or None
+        file path if found or None if not.
+
+    Examples
+    --------
+    Find an existing orig grib2 file of CMA-GFS in CMA-PAI HPC.
+
+    >>> find_local_file(
+    ...     "cma_gfs_gmf/grib2/orig",
+    ...     start_time="2023122000",
+    ...     forecast_time="3h",
+    ... )
+    PosixPath('/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2023122000/ORIG/gmf.gra.2023122000003.grb2')
+
+    Find a non-existing orig grib2 file of CMA-GFS.
+
+    >>> find_local_file(
+    ...     "cma_gfs_gmf/grib2/orig",
+    ...     start_time="2020032100",
+    ...     forecast_time="1h",
+    ... )
+    None
+
+    Find a grib2 file in storage for CMA-MESO 3km.
+
+    >>> find_local_file(
+    ...     "cma_meso_3km/grib2/orig",
+    ...     start_time="2020032100",
+    ...     forecast_time="1h",
+    ...     data_level="storage",
+    ... )
+    PosixPath('/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_MESO_3KM/Prod-grib/2020032100/ORIG/rmf.hgra.2020032100001.grb2')
+
+    Find a grib2 file in storage for CMA-GEPS.
+
+    >>> find_local_file(
+    ...     "cma_geps/grib2/orig",
+    ...     start_time="2023032100",
+    ...     forecast_time="3h",
+    ...     data_level="storage",
+    ...     number=1,
+    ... )
+    PosixPath('/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GEPS/Prod-grib/2023032100/grib2/gef.gra.001.2023032100003.grb2')
+
+    Find postvar ctl file for CMA-TYM in Windows mount storage.
+
+    .. code-block:: pycon
+
+        >>> find_local_file(
+        ...     "cma_tym/bin/postvar_ctl",
+        ...     start_time="2021080200",
+        ...     storage_base="M:"
+        ... )
+        WindowsPath('M:/GRAPES_TYM/Fcst-main/2021080200/post.ctl_2021080200')
+
+    """
+    if config_dir is None:
+        config_dir = get_default_local_config_path()
+
+    config_file_path = find_config(config_dir, data_type, data_class)
+    if config_file_path is None:
+        raise ValueError(f"data type is not found: {data_type}")
+
+    if isinstance(forecast_time, str):
+        forecast_time = pd.to_timedelta(forecast_time)
+    if isinstance(start_time, str):
+        start_time = pd.to_datetime(start_time, format="%Y%m%d%H")
+    if isinstance(obs_time, str):
+        obs_time = pd.to_datetime(obs_time)
+    elif obs_time is None:
+        obs_time = start_time
+
+    config = load_config(config_file_path)
+    file_path = find_file(
+        config,
+        data_level,
+        start_time,
+        forecast_time,
+        obs_time=obs_time,
+        debug=debug,
+        **kwargs
+    )
+    return file_path
+
+
+def get_local_file_name(
+        data_type: str,
+        start_time: Union[str, pd.Timestamp, datetime.datetime],
+        forecast_time: Union[str, pd.Timedelta] = pd.Timedelta(hours=1),
+        data_class: str = "od",
+        config_dir: Union[str, Path] = None,
+        obs_time: Union[str, pd.Timestamp] = None,
+        **kwargs,
+) -> str:
+    if config_dir is None:
+        config_dir = get_default_local_config_path()
+
+    config_file_path = find_config(config_dir, data_type, data_class)
+    if config_file_path is None:
+        raise ValueError(f"data type is not found: {data_type}")
+
+    # if isinstance(forecast_time, str):
+    #     forecast_time = pd.to_timedelta(forecast_time)
+
+    if isinstance(start_time, str):
+        start_time = pd.to_datetime(start_time, format="%Y%m%d%H")
+    if isinstance(obs_time, str):
+        obs_time = pd.to_datetime(obs_time)
+    elif obs_time is None:
+        obs_time = start_time
+
+    config = load_config(config_file_path)
+    file_name = render_file_name(
+        config,
+        start_time,
+        forecast_time,
+        obs_time=obs_time,
+        **kwargs
+    )
+    return file_name
+
+
+def find_local_files(
+        data_type: str,
+        start_time: Union[str, pd.Timestamp, datetime.datetime],
+        forecast_time: Union[str, pd.Timedelta] = "0",
+        data_level: Optional[Union[str, Iterable]] = ("archive", "storage"),
+        path_type: str = "local",
+        data_class: str = "od",
+        config_dir: Union[str, Path] = None,
+        glob: bool = True,
+        **kwargs,
+) -> Optional[Path]:
+    if config_dir is None:
+        config_dir = get_default_local_config_path()
+
+    config_file_path = find_config(config_dir, data_type, data_class)
+    if config_file_path is None:
+        raise ValueError(f"data type is not found: {data_type}")
+
+    if isinstance(forecast_time, str):
+        forecast_time = pd.to_timedelta(forecast_time)
+    if isinstance(start_time, str):
+        start_time = pd.to_datetime(start_time, format="%Y%m%d%H")
+
+    config = load_config(config_file_path)
+    file_path = find_files(config, data_level, start_time, forecast_time, glob, **kwargs)
+    return file_path
```

### Comparing `reki-0.3.0/reki/format/grads/field.py` & `reki-2024.4.0/reki/format/grads/field.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,200 +1,244 @@
-from typing import Union, Dict, List, Optional
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-import xarray as xr
-
-
-from .grads_ctl import GradsCtlParser
-from .grads_data_handler import GradsDataHandler, GradsRecordHandler
-
-
-def load_field_from_file(
-        file_path: Union[str, Path],
-        parameter: Union[str, Dict] = None,
-        level_type: str = None,
-        level: Union[int, float, List] = None,
-        level_dim: Optional[str] = None,
-        latitude_direction: str = "degree_north",
-        forecast_time: Union[str, pd.Timedelta] = None,
-        **kwargs
-) -> Optional[xr.DataArray]:
-    """
-    Load one field or fields of one parameter from GrADS binary file.
-
-    Parameters
-    ----------
-    file_path
-    parameter
-    level_type
-        * pl / ml
-        * index
-        * single
-        * None
-    level
-    level_dim
-    latitude_direction
-        * degree_north
-        * degree_south
-    forecast_time
-    kwargs
-
-    Returns
-    -------
-    xr.DataArray
-        Xarray DataArray if found, or None if not.
-
-    Examples
-    --------
-    Load GRAPES GFS GMF postvar data:
-
-    >>> from reki.data_finder import find_local_file
-    >>> from reki.format.grads import load_field_from_file
-    >>> postvar_file_path = find_local_file(
-    ...     "grapes_gfs_gmf/bin/postvar_ctl",
-    ...     start_time="2021080200",
-    ...     forecast_time="36h"
-    ... )
-    >>> field = load_field_from_file(
-    ...     postvar_file_path,
-    ...     parameter="t",
-    ...     level_type="pl",
-    ...     level=850
-    ... )
-
-    Load GRAPES TYM postvar data. Set ``forecast_time`` option because all data files of one cycle use one CTL file.
-
-    >>> postvar_file_path = find_local_file(
-    ...     "grapes_tym/bin/postvar_ctl",
-    ...     start_time="2021080200",
-    ... )
-    >>> field = load_field_from_file(
-    ...     postvar_file_path,
-    ...     parameter="t",
-    ...     level_type="pl",
-    ...     forecast_time="24h",
-    ...     level=850
-    ... )
-    """
-    if isinstance(forecast_time, str):
-        forecast_time = pd.to_timedelta(forecast_time)
-
-    ctl_parser = GradsCtlParser()
-    ctl_parser.parse(file_path)
-    grads_ctl = ctl_parser.grads_ctl
-
-    # level_type: pl, index, single
-    grads_level_type = "multi"
-    level_dim_name = "level"
-    if not isinstance(level, List):
-        level = [level]
-    if level_type == "single":
-        level = np.zeros(len(level))
-        grads_level_type = "single"
-    elif level_type == "index":
-        level = [grads_ctl.zdef["values"][cur_level] for cur_level in level]
-    elif level_type in ("pl", "ml"):
-        level_dim_name = level_type
-    if level_dim is not None:
-        level_dim_name = level_dim
-
-    data_handler = GradsDataHandler(grads_ctl)
-
-    xarray_records = []
-    for cur_level in level:
-        record = data_handler.find_record(
-            name=parameter,
-            level=cur_level,
-            level_type=grads_level_type,
-            forecast_time=forecast_time,
-        )
-        if record is None:
-            continue
-
-        xarray_record = create_data_array_from_record(
-            record=record,
-            parameter=parameter,
-            level=cur_level,
-            level_dim_name=level_dim_name,
-            latitude_direction=latitude_direction,
-        )
-        xarray_records.append(xarray_record)
-
-    record_count = len(xarray_records)
-    if record_count == 0:
-        return None
-    elif record_count == 1:
-        return xarray_records[0]
-    else:
-        data = xr.concat(xarray_records, level_dim_name)
-
-    return data
-
-
-def create_data_array_from_record(
-        record: GradsRecordHandler,
-        parameter,
-        level,
-        level_dim_name=None,
-        latitude_direction="degree_north",
-) -> Optional[xr.DataArray]:
-    grads_ctl = record.grads_ctl
-
-    # values
-    file_path = grads_ctl.get_data_file_path(record.record_info)
-    with open(file_path, "rb") as f:
-        values = record.load_data(f)
-
-    # coords
-    lons = grads_ctl.xdef["values"]
-    lats = grads_ctl.ydef["values"]
-
-    if latitude_direction == "degree_north":
-        values = np.flip(values, 0)
-        lats = lats[::-1]
-
-    coords = {}
-    coords["latitude"] = xr.Variable(
-        "latitude",
-        lats,
-        attrs={
-            "units": latitude_direction,
-            "standard_name": "latitude",
-            "long_name": "latitude"
-        },
-    )
-    coords["longitude"] = xr.Variable(
-        "longitude",
-        lons,
-        attrs={
-            "units": "degrees_east",
-            "standard_name": "longitude",
-            "long_name": "longitude"
-        }
-    )
-
-    coords[level_dim_name] = level
-    coords["valid_time"] = record.record_info["valid_time"]
-
-    if grads_ctl.start_time is not None and grads_ctl.forecast_time is not None:
-        coords["start_time"] = grads_ctl.start_time
-        coords["forecast_time"] = grads_ctl.forecast_time
-
-    # dims
-    dims = ("latitude", "longitude")
-
-    # attrs
-    data_attrs = {
-        "description": record.record_info["description"]
-    }
-
-    data = xr.DataArray(
-        values,
-        dims=dims,
-        coords=coords,
-        attrs=data_attrs,
-        name=parameter,
-    )
-
-    return data
+from typing import Union, Dict, List, Optional
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+import xarray as xr
+
+
+from .grads_ctl import GradsCtlParser
+from .grads_data_handler import GradsDataHandler, GradsRecordHandler
+
+
+def load_field_from_file(
+        file_path: Union[str, Path],
+        parameter: str,
+        level_type: str = None,
+        level: Union[int, float, List] = None,
+        level_dim: Optional[str] = None,
+        latitude_direction: str = "degree_north",
+        forecast_time: Union[str, pd.Timedelta] = None,
+        **kwargs
+) -> Optional[xr.DataArray]:
+    """
+    Load one field or fields of one parameter from GrADS binary file.
+
+    Parameters
+    ----------
+    file_path
+    parameter
+    level_type
+        * pl / ml
+        * index
+        * single
+        * None
+    level
+    level_dim
+    latitude_direction
+        * degree_north
+        * degree_south
+    forecast_time
+    kwargs
+
+    Returns
+    -------
+    xr.DataArray
+        Xarray DataArray if found, or None if not.
+
+    Examples
+    --------
+    Load GRAPES GFS GMF postvar data:
+
+    >>> from reki.data_finder import find_local_file
+    >>> from reki.format.grads import load_field_from_file
+    >>> postvar_file_path = find_local_file(
+    ...     "grapes_gfs_gmf/bin/postvar_ctl",
+    ...     start_time="2021080200",
+    ...     forecast_time="36h"
+    ... )
+    >>> field = load_field_from_file(
+    ...     postvar_file_path,
+    ...     parameter="t",
+    ...     level_type="pl",
+    ...     level=850
+    ... )
+
+    Load GRAPES TYM postvar data. Set ``forecast_time`` option because all data files of one cycle use one CTL file.
+
+    >>> postvar_file_path = find_local_file(
+    ...     "grapes_tym/bin/postvar_ctl",
+    ...     start_time="2021080200",
+    ... )
+    >>> field = load_field_from_file(
+    ...     postvar_file_path,
+    ...     parameter="t",
+    ...     level_type="pl",
+    ...     forecast_time="24h",
+    ...     level=850
+    ... )
+    """
+    if isinstance(forecast_time, str):
+        forecast_time = pd.to_timedelta(forecast_time)
+    if isinstance(file_path, str):
+        file_path = Path(file_path)
+
+    ctl_parser = GradsCtlParser()
+    ctl_parser.parse(file_path)
+    grads_ctl = ctl_parser.grads_ctl
+
+    # level_type: pl, index, single
+    grads_level_type = "multi"
+    level_dim_name = "level"
+
+    if not isinstance(level, List) and level is not None:
+        level = [level]
+
+    if level_type == "single":
+        level = [0]
+        grads_level_type = "single"
+    elif level_type == "index":
+        level = [grads_ctl.zdef["values"][cur_level] for cur_level in level]
+    elif level_type in ("pl", "ml"):
+        level_dim_name = level_type
+        if level is None:
+            level = grads_ctl.zdef["values"]
+    elif level_type is None:
+        grads_level_type = None
+        # level = None
+
+    if level_dim is not None:
+        level_dim_name = level_dim
+
+    data_handler = GradsDataHandler(grads_ctl)
+
+    xarray_records = []
+    for index, record in enumerate(grads_ctl.record):
+        if not check_record(
+            record,
+            parameter=parameter,
+            level=level,
+            level_type=grads_level_type,
+            forecast_time=forecast_time,
+        ):
+            continue
+
+        offset = data_handler.get_offset_by_record_index(record["record_index"])
+        record_handler = GradsRecordHandler(grads_ctl, index, offset)
+
+        xarray_record = create_data_array_from_record(
+            record=record_handler,
+            parameter=parameter,
+            level=record["level"],
+            level_dim_name=level_dim_name,
+            latitude_direction=latitude_direction,
+        )
+        xarray_records.append(xarray_record)
+
+    record_count = len(xarray_records)
+    if record_count == 0:
+        return None
+    elif record_count == 1:
+        return xarray_records[0]
+    else:
+        data = xr.concat(xarray_records, level_dim_name)
+
+    return data
+
+
+def check_record(
+        record: Dict,
+        parameter: str,
+        level_type: str = None,
+        level: Union[int, float, List] = None,
+        valid_time: pd.Timestamp = None,
+        forecast_time: pd.Timedelta = None
+) -> bool:
+    if parameter != record["name"]:
+        return False
+
+    if level_type is not None and level_type != record["level_type"]:
+        return False
+
+    if level is not None:
+        if isinstance(level, List):
+            if record["level"] not in level:
+                return False
+        else:
+            if level != record["level"]:
+                return False
+
+    if valid_time is not None and valid_time != record["valid_time"]:
+        return False
+
+    if forecast_time is not None and forecast_time != record["forecast_time"]:
+        return False
+
+    return True
+
+
+def create_data_array_from_record(
+        record: GradsRecordHandler,
+        parameter,
+        level,
+        level_dim_name=None,
+        latitude_direction="degree_north",
+) -> Optional[xr.DataArray]:
+    grads_ctl = record.grads_ctl
+
+    # values
+    file_path = grads_ctl.get_data_file_path(record.record_info)
+    with open(file_path, "rb") as f:
+        values = record.load_data(f)
+
+    # coords
+    lons = grads_ctl.xdef["values"]
+    lats = grads_ctl.ydef["values"]
+
+    if latitude_direction == "degree_north":
+        values = np.flip(values, 0)
+        lats = lats[::-1]
+
+    coords = {}
+    coords["latitude"] = xr.Variable(
+        "latitude",
+        lats,
+        attrs={
+            "units": latitude_direction,
+            "standard_name": "latitude",
+            "long_name": "latitude"
+        },
+    )
+    coords["longitude"] = xr.Variable(
+        "longitude",
+        lons,
+        attrs={
+            "units": "degrees_east",
+            "standard_name": "longitude",
+            "long_name": "longitude"
+        }
+    )
+
+    coords[level_dim_name] = level
+    coords["valid_time"] = record.record_info["valid_time"]
+
+    if grads_ctl.start_time is not None and grads_ctl.forecast_time is not None:
+        coords["start_time"] = grads_ctl.start_time
+        coords["forecast_time"] = grads_ctl.forecast_time
+
+    # dims
+    dims = ("latitude", "longitude")
+
+    # attrs
+    data_attrs = {
+        "description": record.record_info["description"]
+    }
+
+    data = xr.DataArray(
+        values,
+        dims=dims,
+        coords=coords,
+        attrs=data_attrs,
+        name=parameter,
+    )
+
+    return data
```

### Comparing `reki-0.3.0/reki/format/grads/grads_ctl.py` & `reki-2024.4.0/reki/format/grads/grads_ctl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,387 +1,396 @@
-import sys
-import re
-from pathlib import Path
-import logging
-from typing import Optional, Union
-
-import pandas as pd
-
-
-logger = logging.getLogger(__name__)
-
-
-class GradsCtl(object):
-    def __init__(self):
-        self.dset = None  # data file path
-        self.dset_template = False
-
-        self.title = ''
-        self.options = list()
-        self.data_endian = 'little'
-        self.local_endian = sys.byteorder
-        self.yrev = 0
-        self.undef = None
-
-        self.start_time = None
-        self.forecast_time = None
-
-        # dimension
-        self.xdef = None
-        self.ydef = None
-        self.zdef = None
-        self.tdef = None
-
-        self.vars = []
-        self.record = []
-
-    def get_data_file_path(self, record):
-        return GradsCtlParser.get_data_file_path(self, record)
-
-
-class GradsCtlParser(object):
-    def __init__(self, grads_ctl: Optional[GradsCtl] = None):
-        self.ctl_file_path = None
-
-        if grads_ctl is None:
-            grads_ctl = GradsCtl()
-        self.grads_ctl = grads_ctl
-
-        self.ctl_file_lines = list()
-        self.cur_no = -1
-
-        self.parser_mapper = {
-            'ctl_file_name': self._parse_ctl_file_name,
-            'dset': self._parse_dset,
-            'options': self._parse_options,
-            'title': self._parse_title,
-            'undef': self._parse_undef,
-            'xdef': self._parse_dimension,
-            'ydef': self._parse_dimension,
-            'zdef': self._parse_dimension,
-            'tdef': self._parse_tdef,
-            'vars': self._parse_vars,
-        }
-
-    def set_ctl_file_path(self, ctl_file_path: Union[Path, str]):
-        self.ctl_file_path = Path(ctl_file_path)
-        with open(ctl_file_path) as f:
-            lines = f.readlines()
-            self.ctl_file_lines = [l.strip() for l in lines]
-            self.cur_no = 0
-
-    def parse(self, ctl_file_path: Union[Path, str]):
-        self.set_ctl_file_path(ctl_file_path)
-        total_lines = len(self.ctl_file_lines)
-        while self.cur_no < total_lines:
-            cur_line = self.ctl_file_lines[self.cur_no]
-            first_word = cur_line[0:cur_line.find(' ')]
-            if first_word.lower() in self.parser_mapper:
-                self.parser_mapper[first_word]()
-            self.cur_no += 1
-
-        self._parse_ctl_file_name()
-
-        return self.grads_ctl
-
-    def _parse_ctl_file_name(self):
-        ctl_file_name = Path(self.ctl_file_path).name
-
-        if (
-                self.grads_ctl.start_time is None
-                and self.grads_ctl.forecast_time is None
-        ):
-            logger.debug("guess start time and forecast time")
-
-            if ctl_file_name.startswith("post.ctl_") or ctl_file_name.startswith("model.ctl_"):
-                file_name = ctl_file_name[ctl_file_name.index("_")+1:]
-                # check for GRAPES MESO:
-                #   post.ctl_201408111202900
-                if re.match(r"[0-9]{15}", file_name):
-                    self.grads_ctl.start_time = pd.to_datetime(file_name[:10], format="%Y%m%d%H")
-                    self.grads_ctl.forecast_time = pd.Timedelta(hours=int(file_name[11:14]))
-                # check for GRAPES GFS:
-                #   post.ctl_2014081112_001
-                elif re.match(r"[0-9]{10}_[0-9]{3}", file_name):
-                    self.grads_ctl.start_time = pd.to_datetime(file_name[:10], format="%Y%m%d%H")
-                    self.grads_ctl.forecast_time = pd.Timedelta(hours=int(file_name[12:]))
-                else:
-                    logger.warning("We can't recognize ctl file name. ")
-
-    def _parse_dset(self):
-        """
-        parse data file path:
-
-            dset ^postvar2021080200_024
-            dset ^postvar2021092700%f3%n2
-
-        """
-        cur_line = self.ctl_file_lines[self.cur_no]
-        file_path = cur_line[4:].strip()
-        if "%" in file_path:
-            self.grads_ctl.dset_template = True
-        if file_path[0] == '^':
-            file_dir = Path(self.ctl_file_path).parent
-            file_path = Path(file_dir, file_path[1:])
-
-        self.grads_ctl.dset = file_path
-
-    def _parse_options(self):
-        cur_line = self.ctl_file_lines[self.cur_no]
-        options = cur_line[7:].strip().split(' ')
-        self.grads_ctl.options.extend(options)
-        for an_option in options:
-            if an_option == 'big_endian':
-                self.grads_ctl.data_endian = 'big'
-            elif an_option == 'little_endian':
-                self.grads_ctl.data_endian = 'little'
-            elif an_option == 'yrev':
-                self.grads_ctl.yrev = True
-
-    def _parse_title(self):
-        cur_line = self.ctl_file_lines[self.cur_no]
-        title = cur_line[5:].strip()
-        self.grads_ctl.title = title
-
-    def _parse_undef(self):
-        cur_line = self.ctl_file_lines[self.cur_no]
-        undef = cur_line[5:].strip()
-        self.grads_ctl.undef = float(undef)
-
-    def _parse_dimension(self):
-        """
-        parser for keywords xdef, ydef and zdef
-        """
-        cur_line = self.ctl_file_lines[self.cur_no].lower()
-        tokens = cur_line.split()
-        dim_name = tokens[0]  # xdef, ydef, zdef
-        dimension_type = tokens[2]
-
-        dimension_parser_map = {
-            'linear': self._parse_linear_dimension,
-            'levels': self._parse_levels_dimension
-        }
-
-        if dimension_type in dimension_parser_map:
-            dimension_parser_map[dimension_type](dim_name, tokens)
-        else:
-            raise NotImplemented(f'dimension_type is not supported: {dimension_type}')
-
-    def _parse_linear_dimension(self, dim_name, tokens):
-        """
-        Parse linear dimension
-
-            xdef 1440 linear    0.0000    0.2500
-
-        """
-        if len(tokens) < 4:
-            raise Exception("%s parser error" % dim_name)
-        count = int(tokens[1])
-        start = float(tokens[3])
-        step = float(tokens[4])
-        levels = [start + step * n for n in range(count)]
-        setattr(self.grads_ctl, dim_name, {
-            'type': 'linear',
-            'count': count,
-            'start': start,
-            'step': step,
-            'values': levels
-        })
-
-    def _parse_levels_dimension(self, dim_name, tokens):
-        """
-        Parse levels dimension
-
-            zdef   27 levels
-                 1000.000
-                 925.0000
-                 850.0000
-                 700.0000
-                 ...
-
-        """
-        levels = list()
-        count = int(tokens[1])
-        if len(tokens) > 2:
-            levels = [float(l) for l in tokens[3:]]
-        i = len(levels)
-        while i < count:
-            self.cur_no += 1
-            cur_line = self.ctl_file_lines[self.cur_no]
-            levels.append(float(cur_line))
-            i += 1
-
-        setattr(self.grads_ctl, dim_name, {
-            'type': 'levels',
-            'count': count,
-            'values': levels
-        })
-
-    def _parse_tdef(self):
-        """
-        Parse time dimension
-
-            tdef    1 linear 00z03AUG2021   360mn
-
-        """
-        cur_line = self.ctl_file_lines[self.cur_no]
-        parts = cur_line.strip().split()
-        assert parts[2] == "linear"
-        assert len(parts) == 5
-
-        count = int(parts[1])
-        start_string = parts[3]
-        increment_string = parts[4]
-
-        start_date = GradsCtlParser._parse_start_time(start_string)
-        time_step = GradsCtlParser._parse_increment_time(increment_string)
-
-        values = [start_date + time_step * i for i in range(count)]
-
-        self.grads_ctl.tdef = {
-            'type': 'linear',
-            'count': count,
-            'start': start_date,
-            'step': time_step,
-            'values': values
-        }
-
-    @classmethod
-    def _parse_start_time(cls, start_string) -> pd.Timestamp:
-        """
-        parse start time
-        format:
-            hh:mmZddmmmyyyy
-        where:
-            hh	=	hour (two digit integer)
-            mm	=	minute (two digit integer)
-            dd	=	day (one or two digit integer)
-            mmm	=	3-character month
-            yyyy	=	year (may be a two or four digit integer;
-                              2 digits implies a year between 1950 and 2049)
-        """
-        start_date = pd.Timestamp.now()
-        if start_string[3] == ':':
-            raise NotImplemented('Not supported time with hh')
-        elif len(start_string) == 12:
-            start_date = pd.to_datetime(start_string.lower(), format='%Hz%d%b%Y')
-        else:
-            raise NotImplemented(f'start time not supported: {start_string}')
-        return start_date
-
-    @classmethod
-    def _parse_increment_time(cls, increment_string) -> pd.Timedelta:
-        """
-        parse increment time
-        format:
-            vvkk
-        where:
-            vv	=	an integer number, 1 or 2 digits
-            kk	=	mn (minute)
-                    hr (hour)
-                    dy (day)
-                    mo (month)
-                    yr (year)
-        """
-        vv = int(increment_string[:-2])
-        kk = increment_string[-2:]
-
-        kk_map = {
-            'mn': (lambda v: pd.Timedelta(minutes=v)),
-            'hr': (lambda v: pd.Timedelta(hours=v)),
-            'dy': (lambda v: pd.Timedelta(days=v))
-        }
-        if kk in kk_map:
-            return kk_map[kk](vv)
-        else:
-            raise NotImplemented('{kk} is not supported'.format(kk=kk))
-
-    def _parse_vars(self):
-        self._parse_variables()
-        self._generate_records()
-
-    def _parse_variables(self):
-        var_list = list()
-
-        parts = self.ctl_file_lines[self.cur_no].strip().split()
-        assert len(parts) == 2
-        count = int(parts[1])
-        for _ in range(count):
-            # parse one var line
-            self.cur_no += 1
-            cur_line = self.ctl_file_lines[self.cur_no].strip()
-            parts = cur_line.split()
-            # we currently use old style of var record.
-            # TODO: check for new type of record from GrADS v2.0.2
-
-            var_name = parts[0]
-            levels = int(parts[1])
-            units = parts[2]
-            description = " ".join(parts[3:])
-
-            cur_var = {
-                'name': var_name,
-                'levels': levels,
-                'units': units,
-                'description': description
-            }
-            var_list.append(cur_var)
-
-        self.grads_ctl.vars = var_list
-
-    def _generate_records(self):
-        record_list = list()
-        record_index = 0
-        for time_step_index, valid_time in enumerate(self.grads_ctl.tdef["values"]):
-            forecast_time = self.grads_ctl.tdef["step"] * time_step_index
-            if self.grads_ctl.dset_template:
-                record_index = 0
-            for a_var_record in self.grads_ctl.vars:
-                if a_var_record['levels'] == 0:
-                    record_list.append({
-                        'name': a_var_record['name'],
-                        'level_type': 'single',
-                        'level': 0,
-                        'level_index': 0,
-                        'valid_time': valid_time,
-                        'forecast_time': forecast_time,
-                        'units': a_var_record['units'],
-                        'description': a_var_record['description'],
-                        'record_index': record_index
-                    })
-                    record_index += 1
-                else:
-                    for level_index in range(0, a_var_record["levels"]):
-                        a_level = self.grads_ctl.zdef["values"][level_index]
-                        record_list.append({
-                            'name': a_var_record['name'],
-                            'level_type': 'multi',
-                            'level': a_level,
-                            'level_index': level_index,
-                            'units': a_var_record['units'],
-                            'valid_time': valid_time,
-                            'forecast_time': forecast_time,
-                            'description': a_var_record['description'],
-                            'record_index': record_index
-                        })
-                        record_index += 1
-
-        self.grads_ctl.record = record_list
-
-    @classmethod
-    def get_data_file_path(cls, grads_ctl, record) -> Path:
-        if not grads_ctl.dset_template:
-            return grads_ctl.dset
-
-        tokens = str(grads_ctl.dset).split("%")
-        token_mapper = {
-            "f3": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(hours=1)):03d}",
-            "n2": lambda x: f"{x['forecast_time'].seconds // 60 % 60:02d}",
-            "fhn": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(hours=1)):02d}00"   # TODO: change
-        }
-
-        parts = tokens[:1]
-        for token in tokens[1:]:
-            m = token_mapper.get(token, lambda x: x)
-            parts.append(m(record))
-
-        return Path("".join(parts))
+import sys
+import re
+from pathlib import Path
+import logging
+from typing import Optional, Union
+
+import pandas as pd
+
+
+logger = logging.getLogger(__name__)
+
+
+class GradsCtl(object):
+    def __init__(self):
+        self.dset = None  # data file path
+        self.dset_template = False
+
+        self.title = ''
+        self.options = list()
+        self.data_endian = 'little'
+        self.local_endian = sys.byteorder
+        self.yrev = 0
+        self.undef = None
+
+        self.start_time = None
+        self.forecast_time = None
+
+        # dimension
+        self.xdef = None
+        self.ydef = None
+        self.zdef = None
+        self.tdef = None
+
+        self.vars = []
+        self.record = []
+
+    def get_data_file_path(self, record):
+        return GradsCtlParser.get_data_file_path(self, record)
+
+
+class GradsCtlParser(object):
+    def __init__(self, grads_ctl: Optional[GradsCtl] = None):
+        self.ctl_file_path = None
+
+        if grads_ctl is None:
+            grads_ctl = GradsCtl()
+        self.grads_ctl = grads_ctl
+
+        self.ctl_file_lines = list()
+        self.cur_no = -1
+
+        self.parser_mapper = {
+            'ctl_file_name': self._parse_ctl_file_name,
+            'dset': self._parse_dset,
+            'options': self._parse_options,
+            'title': self._parse_title,
+            'undef': self._parse_undef,
+            'xdef': self._parse_dimension,
+            'ydef': self._parse_dimension,
+            'zdef': self._parse_dimension,
+            'tdef': self._parse_tdef,
+            'vars': self._parse_vars,
+        }
+
+    def set_ctl_file_path(self, ctl_file_path: Union[Path, str]):
+        self.ctl_file_path = Path(ctl_file_path)
+        with open(ctl_file_path) as f:
+            lines = f.readlines()
+            self.ctl_file_lines = [l.strip() for l in lines]
+            self.cur_no = 0
+
+    def parse(self, ctl_file_path: Union[Path, str]):
+        self.set_ctl_file_path(ctl_file_path)
+        total_lines = len(self.ctl_file_lines)
+        while self.cur_no < total_lines:
+            cur_line = self.ctl_file_lines[self.cur_no]
+            first_word = cur_line[0:cur_line.find(' ')]
+            if first_word.lower() in self.parser_mapper:
+                self.parser_mapper[first_word]()
+            self.cur_no += 1
+
+        self._parse_ctl_file_name()
+
+        return self.grads_ctl
+
+    def _parse_ctl_file_name(self):
+        ctl_file_name = Path(self.ctl_file_path).name
+
+        if (
+                self.grads_ctl.start_time is None
+                and self.grads_ctl.forecast_time is None
+        ):
+            logger.debug("guess start time and forecast time")
+
+            if ctl_file_name.startswith("post.ctl_") or ctl_file_name.startswith("model.ctl_"):
+                file_name = ctl_file_name[ctl_file_name.index("_")+1:]
+                # check for GRAPES MESO:
+                #   post.ctl_201408111202900
+                if re.match(r"[0-9]{15}", file_name):
+                    self.grads_ctl.start_time = pd.to_datetime(file_name[:10], format="%Y%m%d%H")
+                    self.grads_ctl.forecast_time = pd.Timedelta(hours=int(file_name[11:14]))
+                # check for GRAPES GFS:
+                #   post.ctl_2014081112_001
+                elif re.match(r"[0-9]{10}_[0-9]{3}", file_name):
+                    self.grads_ctl.start_time = pd.to_datetime(file_name[:10], format="%Y%m%d%H")
+                    self.grads_ctl.forecast_time = pd.Timedelta(hours=int(file_name[12:]))
+                else:
+                    logger.warning("We can't recognize ctl file name. ")
+
+    def _parse_dset(self):
+        """
+        parse data file path:
+
+            dset ^postvar2021080200_024
+            dset ^postvar2021092700%f3%n2
+
+        """
+        cur_line = self.ctl_file_lines[self.cur_no]
+        file_path = cur_line[4:].strip()
+        if "%" in file_path:
+            self.grads_ctl.dset_template = True
+        if file_path[0] == '^':
+            file_dir = Path(self.ctl_file_path).parent
+            file_path = Path(file_dir, file_path[1:])
+
+        self.grads_ctl.dset = file_path
+
+    def _parse_options(self):
+        cur_line = self.ctl_file_lines[self.cur_no]
+        options = cur_line[7:].strip().split(' ')
+        self.grads_ctl.options.extend(options)
+        for an_option in options:
+            if an_option == 'big_endian':
+                self.grads_ctl.data_endian = 'big'
+            elif an_option == 'little_endian':
+                self.grads_ctl.data_endian = 'little'
+            elif an_option == 'yrev':
+                self.grads_ctl.yrev = True
+
+    def _parse_title(self):
+        cur_line = self.ctl_file_lines[self.cur_no]
+        title = cur_line[5:].strip()
+        self.grads_ctl.title = title
+
+    def _parse_undef(self):
+        cur_line = self.ctl_file_lines[self.cur_no]
+        undef = cur_line[5:].strip()
+        self.grads_ctl.undef = float(undef)
+
+    def _parse_dimension(self):
+        """
+        parser for keywords xdef, ydef and zdef
+        """
+        cur_line = self.ctl_file_lines[self.cur_no].lower()
+        tokens = cur_line.split()
+        dim_name = tokens[0]  # xdef, ydef, zdef
+        dimension_type = tokens[2]
+
+        dimension_parser_map = {
+            'linear': self._parse_linear_dimension,
+            'levels': self._parse_levels_dimension
+        }
+
+        if dimension_type in dimension_parser_map:
+            dimension_parser_map[dimension_type](dim_name, tokens)
+        else:
+            raise NotImplemented(f'dimension_type is not supported: {dimension_type}')
+
+    def _parse_linear_dimension(self, dim_name, tokens):
+        """
+        Parse linear dimension
+
+            xdef 1440 linear    0.0000    0.2500
+
+        """
+        if len(tokens) < 4:
+            raise Exception("%s parser error" % dim_name)
+        count = int(tokens[1])
+        start = float(tokens[3])
+        step = float(tokens[4])
+        levels = [start + step * n for n in range(count)]
+        setattr(self.grads_ctl, dim_name, {
+            'type': 'linear',
+            'count': count,
+            'start': start,
+            'step': step,
+            'values': levels
+        })
+
+    def _parse_levels_dimension(self, dim_name, tokens):
+        """
+        Parse levels dimension
+
+            zdef   27 levels
+                 1000.000
+                 925.0000
+                 850.0000
+                 700.0000
+                 ...
+
+        """
+        levels = list()
+        count = int(tokens[1])
+        if len(tokens) > 2:
+            levels = [float(l) for l in tokens[3:]]
+        i = len(levels)
+        while i < count:
+            self.cur_no += 1
+            cur_line = self.ctl_file_lines[self.cur_no]
+            levels.append(float(cur_line))
+            i += 1
+
+        setattr(self.grads_ctl, dim_name, {
+            'type': 'levels',
+            'count': count,
+            'values': levels
+        })
+
+    def _parse_tdef(self):
+        """
+        Parse time dimension
+
+            tdef    1 linear 00z03AUG2021   360mn
+
+        """
+        cur_line = self.ctl_file_lines[self.cur_no]
+        parts = cur_line.strip().split()
+        assert parts[2] == "linear"
+        assert len(parts) == 5
+
+        count = int(parts[1])
+        start_string = parts[3]
+        increment_string = parts[4]
+
+        start_date = GradsCtlParser._parse_start_time(start_string)
+        time_step = GradsCtlParser._parse_increment_time(increment_string)
+
+        values = [start_date + time_step * i for i in range(count)]
+
+        self.grads_ctl.tdef = {
+            'type': 'linear',
+            'count': count,
+            'start': start_date,
+            'step': time_step,
+            'values': values
+        }
+
+    @classmethod
+    def _parse_start_time(cls, start_string) -> pd.Timestamp:
+        """
+        parse start time
+        format:
+            hh:mmZddmmmyyyy
+        where:
+            hh	=	hour (two digit integer)
+            mm	=	minute (two digit integer)
+            dd	=	day (one or two digit integer)
+            mmm	=	3-character month
+            yyyy	=	year (may be a two or four digit integer;
+                              2 digits implies a year between 1950 and 2049)
+        """
+        start_date = pd.Timestamp.now()
+        if start_string[3] == ':':
+            raise NotImplemented('Not supported time with hh')
+        elif len(start_string) == 12:
+            start_date = pd.to_datetime(start_string.lower(), format='%Hz%d%b%Y')
+        else:
+            raise NotImplemented(f'start time not supported: {start_string}')
+        return start_date
+
+    @classmethod
+    def _parse_increment_time(cls, increment_string) -> pd.Timedelta:
+        """
+        parse increment time
+        format:
+            vvkk
+        where:
+            vv	=	an integer number, 1 or 2 digits
+            kk	=	mn (minute)
+                    hr (hour)
+                    dy (day)
+                    mo (month)
+                    yr (year)
+        """
+        vv = int(increment_string[:-2])
+        kk = increment_string[-2:]
+
+        kk_map = {
+            'mn': (lambda v: pd.Timedelta(minutes=v)),
+            'hr': (lambda v: pd.Timedelta(hours=v)),
+            'dy': (lambda v: pd.Timedelta(days=v))
+        }
+        if kk in kk_map:
+            return kk_map[kk](vv)
+        else:
+            raise NotImplemented('{kk} is not supported'.format(kk=kk))
+
+    def _parse_vars(self):
+        self._parse_variables()
+        self._generate_records()
+
+    def _parse_variables(self):
+        var_list = list()
+
+        parts = self.ctl_file_lines[self.cur_no].strip().split()
+        assert len(parts) == 2
+        count = int(parts[1])
+        for _ in range(count):
+            # parse one var line
+            self.cur_no += 1
+            cur_line = self.ctl_file_lines[self.cur_no].strip()
+            parts = cur_line.split()
+            # we currently use old style of var record.
+            # TODO: check for new type of record from GrADS v2.0.2
+
+            var_name = parts[0]
+            levels = int(parts[1])
+            units = parts[2]
+            description = " ".join(parts[3:])
+
+            cur_var = {
+                'name': var_name,
+                'levels': levels,
+                'units': units,
+                'description': description
+            }
+            var_list.append(cur_var)
+
+        self.grads_ctl.vars = var_list
+
+    def _generate_records(self):
+        record_list = list()
+        record_index = 0
+        for time_step_index, valid_time in enumerate(self.grads_ctl.tdef["values"]):
+            forecast_time = self.grads_ctl.tdef["step"] * time_step_index
+            if self.grads_ctl.dset_template:
+                record_index = 0
+            for a_var_record in self.grads_ctl.vars:
+                if a_var_record['levels'] == 0:
+                    record_list.append({
+                        'name': a_var_record['name'],
+                        'level_type': 'single',
+                        'level': 0,
+                        'level_index': 0,
+                        'valid_time': valid_time,
+                        'forecast_time': forecast_time,
+                        'units': a_var_record['units'],
+                        'description': a_var_record['description'],
+                        'record_index': record_index
+                    })
+                    record_index += 1
+                else:
+                    for level_index in range(0, a_var_record["levels"]):
+                        a_level = self.grads_ctl.zdef["values"][level_index]
+                        record_list.append({
+                            'name': a_var_record['name'],
+                            'level_type': 'multi',
+                            'level': a_level,
+                            'level_index': level_index,
+                            'units': a_var_record['units'],
+                            'valid_time': valid_time,
+                            'forecast_time': forecast_time,
+                            'description': a_var_record['description'],
+                            'record_index': record_index
+                        })
+                        record_index += 1
+
+        self.grads_ctl.record = record_list
+
+    @classmethod
+    def get_data_file_path(cls, grads_ctl, record) -> Path:
+        if not grads_ctl.dset_template:
+            return grads_ctl.dset
+
+        tokens = str(grads_ctl.dset).split("%")
+        token_mapper = {
+            "n2": lambda x: f"{x['forecast_time'].seconds // 60 % 60:02d}",
+            "f2": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(hours=1)):02d}",
+            "f3": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(hours=1)):03d}",
+            "fn2": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(minutes=1)):02d}",
+            "fhn": lambda x: f"{int(x['forecast_time'] / pd.Timedelta(hours=1)):02d}{int(x['forecast_time'].total_seconds() % (60*60) / 60):02d}"
+        }
+
+        def parse_file_template_token(token: str) -> str:
+            for key in token_mapper:
+                if token.startswith(key):
+                    result = token_mapper[key](record) + token[len(key):]
+                    return result
+            return token
+
+        parts = tokens[:1]
+        for token in tokens[1:]:
+            parsed_part = parse_file_template_token(token)
+            parts.append(parsed_part)
+
+        return Path("".join(parts))
```

### Comparing `reki-0.3.0/reki/format/grads/grads_record_handler.py` & `reki-2024.4.0/reki/format/grads/grads_record_handler.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import BinaryIO
-
-import numpy as np
-
-from .grads_ctl import GradsCtl
-
-
-class GradsRecordHandler(object):
-    """
-    Load record data from binary file.
-    """
-    def __init__(self, grads_ctl: GradsCtl, record_index: int, offset: int, var_index: int = -1, level_index: int = -1):
-        self.grads_ctl = grads_ctl
-        self.record_index = record_index
-        self.record_info = grads_ctl.record[record_index]
-        self.offset = offset
-
-        self.var_index = var_index
-        self.level_index = level_index
-
-        self.data = None
-
-    def load_data(self, data_file: BinaryIO) -> np.ndarray:
-        if 'sequential' in self.grads_ctl.options:
-            self.offset += 4
-        x_count = self.grads_ctl.xdef['count']
-        y_count = self.grads_ctl.ydef['count']
-
-        if self.grads_ctl.data_endian == 'big':
-            data_format = '>f'
-        elif self.grads_ctl.data_endian == 'little':
-            data_format = '<f'
-        else:
-            # print("Data endian is not found. Use local endian to unpack values.")
-            data_format = 'f'
-
-        # load data from file
-        data_file.seek(self.offset)
-
-        var_yrev = self.grads_ctl.yrev
-
-        values = np.fromfile(data_file, dtype=np.dtype(data_format), count=x_count * y_count)
-        values = values.reshape((y_count, x_count))
-
-        if var_yrev:
-            values = np.flip(values, 0)
-
-        self.data = values
-        return values
+from typing import BinaryIO
+
+import numpy as np
+
+from .grads_ctl import GradsCtl
+
+
+class GradsRecordHandler(object):
+    """
+    Load record data from binary file.
+    """
+    def __init__(self, grads_ctl: GradsCtl, record_index: int, offset: int, var_index: int = -1, level_index: int = -1):
+        self.grads_ctl = grads_ctl
+        self.record_index = record_index
+        self.record_info = grads_ctl.record[record_index]
+        self.offset = offset
+
+        self.var_index = var_index
+        self.level_index = level_index
+
+        self.data = None
+
+    def load_data(self, data_file: BinaryIO) -> np.ndarray:
+        if 'sequential' in self.grads_ctl.options:
+            self.offset += 4
+        x_count = self.grads_ctl.xdef['count']
+        y_count = self.grads_ctl.ydef['count']
+
+        if self.grads_ctl.data_endian == 'big':
+            data_format = '>f'
+        elif self.grads_ctl.data_endian == 'little':
+            data_format = '<f'
+        else:
+            # print("Data endian is not found. Use local endian to unpack values.")
+            data_format = 'f'
+
+        # load data from file
+        data_file.seek(self.offset)
+
+        var_yrev = self.grads_ctl.yrev
+
+        values = np.fromfile(data_file, dtype=np.dtype(data_format), count=x_count * y_count)
+        values = values.reshape((y_count, x_count))
+
+        if var_yrev:
+            values = np.flip(values, 0)
+
+        self.data = values
+        return values
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/_level.py` & `reki-2024.4.0/reki/format/grib/eccodes/_level.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Dict, List, Union, Optional, Tuple
-
-
-def _fix_level(
-        level_type: Optional[Union[str, Dict, List]],
-        level_dim: Optional[str],
-) -> Tuple[str or dict, str]:
-    if level_type is None:
-        return level_type, level_dim
-
-    if isinstance(level_type, dict):
-        return level_type, level_dim
-
-    if isinstance(level_type, List):
-        _, level_dim = _fix_level(level_type[0], level_dim)
-        level_type = [_fix_level(cur_level, level_dim)[0] for cur_level in level_type]
-        return level_type, level_dim
-
-    if level_type == "pl":
-        if level_dim is None:
-            level_dim = level_type
-        return {
-            "typeOfFirstFixedSurface": 100,
-        }, level_dim
-    elif level_type == "sfc":
-        if level_dim is None:
-            level_dim = level_type
-        return {
-            "typeOfLevel": "surface"
-        }, level_dim
-    elif level_type == "ml":
-        if level_dim is None:
-            level_dim = level_type
-        return {
-            "typeOfFirstFixedSurface": 131,
-            # "typeOfSecondFixedSurface": 255,
-        }, level_dim
-    return level_type, level_dim
+from typing import Dict, List, Union, Optional, Tuple
+
+
+def _fix_level(
+        level_type: Optional[Union[str, Dict, List]],
+        level_dim: Optional[str],
+) -> Tuple[str or dict, str]:
+    if level_type is None:
+        return level_type, level_dim
+
+    if isinstance(level_type, dict):
+        return level_type, level_dim
+
+    if isinstance(level_type, List):
+        _, level_dim = _fix_level(level_type[0], level_dim)
+        level_type = [_fix_level(cur_level, level_dim)[0] for cur_level in level_type]
+        return level_type, level_dim
+
+    if level_type == "pl":
+        if level_dim is None:
+            level_dim = level_type
+        return {
+            "typeOfFirstFixedSurface": 100,
+        }, level_dim
+    elif level_type == "sfc":
+        if level_dim is None:
+            level_dim = level_type
+        return {
+            "typeOfLevel": "surface"
+        }, level_dim
+    elif level_type == "ml":
+        if level_dim is None:
+            level_dim = level_type
+        return {
+            "typeOfFirstFixedSurface": 131,
+            # "typeOfSecondFixedSurface": 255,
+        }, level_dim
+    return level_type, level_dim
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/_util.py` & `reki-2024.4.0/reki/format/grib/eccodes/_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-from typing import Union, Dict, List, Optional
-import math
-
-import eccodes
-
-from reki.format.grib._parameter import _convert_parameter
-
-
-def _check_message(
-        message_id,
-        parameter: Optional[Union[str, Dict]],
-        level_type: Optional[Union[str, List[str]]],
-        level: Optional[Union[int, List[int], Dict]],
-        **kwargs,
-) -> bool:
-    """
-    Check whether GRIB message (`message_id`) fits conditions.
-
-    Currently, conditions are:
-        - parameter
-        - level_Type
-        - level
-        - other GRIB keys
-
-    Parameters
-    ----------
-    message_id
-    parameter
-    level_type
-    level
-    kwargs
-
-    Returns
-    -------
-
-    """
-    if not _check_parameter(message_id, parameter):
-        return False
-    if not _check_level_type(message_id, level_type):
-        return False
-    if not _check_level_value(message_id, level, level_type):
-        return False
-    if not _check_keys(message_id, **kwargs):
-        return False
-    return True
-
-
-def _check_parameter(message_id, parameter: Optional[Union[str, Dict]]) -> bool:
-    if parameter is None:
-        return True
-    parameter = _convert_parameter(parameter)
-    if isinstance(parameter, str):
-        short_name = eccodes.codes_get(message_id, "shortName")
-        return short_name == parameter
-    elif isinstance(parameter, Dict):
-        for key, value in parameter.items():
-            if eccodes.codes_get(message_id, key) != value:
-                return False
-        return True
-    else:
-        raise ValueError(f"parameter is not supported: {parameter}")
-
-
-def _check_level_type(
-        message_id,
-        level_type: Optional[Union[str, List, Dict]],
-) -> bool:
-    if level_type is None:
-        return True
-    message_type = eccodes.codes_get(message_id, "typeOfLevel", ktype=str)
-    if isinstance(level_type, str):
-        return message_type == level_type
-    elif isinstance(level_type, List):
-        for cur_level_type in level_type:
-            if _check_level_type(message_id, cur_level_type):
-                return True
-        return False
-    elif isinstance(level_type, Dict):
-        for key in level_type:
-            requested_value = level_type[key]
-            value = eccodes.codes_get(message_id, key, ktype=type(requested_value))
-            if requested_value != value:
-                return False
-        return True
-    else:
-        raise ValueError(f"level_type is not supported: {level_type}")
-
-
-def _check_level_value(
-        message_id,
-        level: Optional[Union[int, float, List[int], Dict]],
-        level_type: Union[str, Dict] = None
-) -> bool:
-    if level is None:
-        return True
-
-    message_level = eccodes.codes_get(message_id, "level", ktype=float)
-
-    # check for `pl` using unit hPa.
-    # WARNING: This may be changed.
-    if isinstance(level_type, Dict):
-        if "typeOfFirstFixedSurface" in level_type and level_type["typeOfFirstFixedSurface"] == 100:
-            level_in_pa = _get_level_value(message_id, "First")
-            message_level = level_in_pa / 100.0
-
-    if isinstance(level, int) or isinstance(level, float):
-        return message_level == level
-    elif isinstance(level, List):
-        return message_level in level
-    elif isinstance(level, Dict):
-        current_level_dict = level.copy()
-        if "first_level" in current_level_dict:
-            required_first_level = current_level_dict.pop("first_level")
-            first_level = _get_level_value(message_id, "First")
-            if first_level != float(required_first_level):
-                return False
-        if "second_level" in current_level_dict:
-            required_second_level = current_level_dict.pop("second_level")
-            second_level = _get_level_value(message_id, "Second")
-            if second_level != float(required_second_level):
-                return False
-        return _check_keys(message_id, **current_level_dict)
-    else:
-        raise ValueError(f"level is not supported: {level}")
-
-
-def _check_keys(message_id, **kwargs):
-    for key, value in kwargs.items():
-        v = eccodes.codes_get(message_id, key)
-        if value != v:
-            return False
-    return True
-
-
-def _get_level_value(message_id, name: str = "First"):
-    f = eccodes.codes_get(message_id, f"scaleFactorOf{name}FixedSurface")
-    v = eccodes.codes_get(message_id, f"scaledValueOf{name}FixedSurface")
-    level = math.pow(10, -1 * f) * v
-    return level
+from typing import Union, Dict, List, Optional
+import math
+
+import eccodes
+
+
+def _check_message(
+        message_id,
+        parameter: Optional[Union[str, Dict]],
+        level_type: Optional[Union[str, List[str]]],
+        level: Optional[Union[int, List[int], Dict]],
+        **kwargs,
+) -> bool:
+    """
+    Check whether GRIB message (`message_id`) fits conditions.
+
+    Currently, conditions are:
+        - parameter
+        - level_Type
+        - level
+        - other GRIB keys
+
+    Parameters
+    ----------
+    message_id
+    parameter
+    level_type
+    level
+    kwargs
+
+    Returns
+    -------
+
+    """
+    if not _check_parameter(message_id, parameter):
+        return False
+    if not _check_level_type(message_id, level_type):
+        return False
+    if not _check_level_value(message_id, level, level_type):
+        return False
+    if not _check_keys(message_id, **kwargs):
+        return False
+    return True
+
+
+def _check_parameter(message_id, parameter: Optional[Union[str, Dict]]) -> bool:
+    if parameter is None:
+        return True
+    # parameter = _convert_parameter(parameter)
+    if isinstance(parameter, str):
+        short_name = eccodes.codes_get(message_id, "shortName")
+        return short_name == parameter
+    elif isinstance(parameter, Dict):
+        for key, value in parameter.items():
+            if eccodes.codes_get(message_id, key) != value:
+                return False
+        return True
+    else:
+        raise ValueError(f"parameter is not supported: {parameter}")
+
+
+def _check_level_type(
+        message_id,
+        level_type: Optional[Union[str, List, Dict]],
+) -> bool:
+    if level_type is None:
+        return True
+    message_type = eccodes.codes_get(message_id, "typeOfLevel", ktype=str)
+    if isinstance(level_type, str):
+        return message_type == level_type
+    elif isinstance(level_type, List):
+        for cur_level_type in level_type:
+            if _check_level_type(message_id, cur_level_type):
+                return True
+        return False
+    elif isinstance(level_type, Dict):
+        for key in level_type:
+            requested_value = level_type[key]
+            value = eccodes.codes_get(message_id, key, ktype=type(requested_value))
+            if requested_value != value:
+                return False
+        return True
+    else:
+        raise ValueError(f"level_type is not supported: {level_type}")
+
+
+def _check_level_value(
+        message_id,
+        level: Optional[Union[int, float, List[int], Dict]],
+        level_type: Union[str, Dict] = None
+) -> bool:
+    if level is None:
+        return True
+
+    message_level = eccodes.codes_get(message_id, "level", ktype=float)
+
+    # check for `pl` using unit hPa.
+    # WARNING: This may be changed.
+    if isinstance(level_type, Dict):
+        if "typeOfFirstFixedSurface" in level_type and level_type["typeOfFirstFixedSurface"] == 100:
+            level_in_pa = _get_level_value(message_id, "First")
+            message_level = level_in_pa / 100.0
+
+    if isinstance(level, int) or isinstance(level, float):
+        return message_level == level
+    elif isinstance(level, List):
+        return message_level in level
+    elif isinstance(level, Dict):
+        current_level_dict = level.copy()
+        if "first_level" in current_level_dict:
+            required_first_level = current_level_dict.pop("first_level")
+            first_level = _get_level_value(message_id, "First")
+            if first_level != float(required_first_level):
+                return False
+        if "second_level" in current_level_dict:
+            required_second_level = current_level_dict.pop("second_level")
+            second_level = _get_level_value(message_id, "Second")
+            if second_level != float(required_second_level):
+                return False
+        return _check_keys(message_id, **current_level_dict)
+    elif level == "all":
+        return True
+    else:
+        raise ValueError(f"level is not supported: {level}")
+
+
+def _check_keys(message_id, **kwargs):
+    for key, value in kwargs.items():
+        v = eccodes.codes_get(message_id, key)
+        if value != v:
+            return False
+    return True
+
+
+def _get_level_value(message_id, name: str = "First"):
+    f = eccodes.codes_get(message_id, f"scaleFactorOf{name}FixedSurface")
+    v = eccodes.codes_get(message_id, f"scaledValueOf{name}FixedSurface")
+    level = math.pow(10, -1 * f) * v
+    return level
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/bytes.py` & `reki-2024.4.0/reki/format/grib/eccodes/bytes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,136 @@
-from pathlib import Path
-from typing import List, Dict, Union, Optional
-
-import eccodes
-
-from reki.format.grib._level import fix_level_type
-from ._util import (
-    _check_message,
-)
-
-
-def load_bytes_from_file(
-        file_path: Union[str, Path],
-        parameter: Union[str, Dict],
-        level_type: str = None,
-        level: int = None,
-) -> Optional[bytes]:
-    """
-    Load one message from grib file and return message's original bytes.
-
-    Parameters
-    ----------
-    file_path
-    parameter
-    level_type
-    level
-
-    Returns
-    -------
-    bytes or None
-
-    Examples
-    --------
-    Load bytes of 850hPa temperature from GRAPES GFS GMF and create GRIB message using `eccodes.codes_new_from_message`.
-
-    >>> file_path = "/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2"
-    >>> message_bytes = load_bytes_from_file(
-    ...     file_path=file_path,
-    ...     parameter="t",
-    ...     level_type="pl",
-    ...     level=850,
-    ... )
-    >>> message = eccodes.codes_new_from_message(message_bytes)
-    >>> values = eccodes.codes_get_double_array(message, "values")
-    >>> print(len(values))
-    1036800
-
-    """
-    offset = 0
-    fixed_level_type = fix_level_type(level_type)
-    with open(file_path, "rb") as f:
-        while True:
-            message_id = eccodes.codes_grib_new_from_file(f)
-            length = eccodes.codes_get(message_id, "totalLength")
-            if message_id is None:
-                return None
-            if not _check_message(message_id, parameter, fixed_level_type, level):
-                eccodes.codes_release(message_id)
-                offset += length
-                continue
-            return eccodes.codes_get_message(message_id)
-
-
-def create_message_from_bytes(raw_message: bytes) -> Optional[int]:
-    """
-    Create **the first** message from raw bytes.
-
-    The returned message should be released using ``eccodes.codes_release`` manually.
-
-    Parameters
-    ----------
-    raw_message
-
-    Returns
-    -------
-    int or None
-    """
-    return eccodes.codes_new_from_message(raw_message)
-
-
-def create_messages_from_bytes(raw_message: bytes) -> List[int]:
-    """
-    Create all messages from raw bytes.
-
-    The returned messages should be released using ``eccodes.codes_release`` manually.
-
-    Parameters
-    ----------
-    raw_message
-
-    Returns
-    -------
-    int or None
-
-    Examples
-    --------
-    Load raw bytes of temperature at 500hPa and 850hPa and reload them from raw bytes.
-    Print level value of all returned messages.
-
-    >>> file_path = "/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2"
-    >>> message_bytes_t850 = load_bytes_from_file(
-    ...     file_path=file_path,
-    ...     parameter="t",
-    ...     level_type="pl",
-    ...     level=850,
-    ... )
-    >>> message_bytes_t500 = load_bytes_from_file(
-    ...     file_path=file_path,
-    ...     parameter="t",
-    ...     level_type="pl",
-    ...     level=500,
-    ... )
-    >>> message_bytes = message_bytes_t500 + message_bytes_t850
-    >>> messages = create_messages_from_bytes(message_bytes)
-    >>> for message in messages:
-    ...     print(eccodes.codes_get(message, "level"))
-    500
-    850
-
-    """
-    messages = []
-    message_bytes = raw_message
-
-    while len(message_bytes) > 0:
-        message = create_message_from_bytes(message_bytes)
-        if message is None:
-            break
-        message_size = eccodes.codes_get_message_size(message)
-        messages.append(message)
-        message_bytes = message_bytes[message_size:]
-    return messages
+from pathlib import Path
+from typing import List, Dict, Union, Optional
+
+import eccodes
+
+from reki.format.grib.common._level import fix_level_type
+from reki.format.grib.common._parameter import convert_parameter
+from ._util import (
+    _check_message,
+)
+
+
+def load_bytes_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict],
+        level_type: str = None,
+        level: int = None,
+) -> Optional[bytes]:
+    """
+    Load one message from grib file and return message's original bytes.
+
+    Parameters
+    ----------
+    file_path
+    parameter
+    level_type
+    level
+
+    Returns
+    -------
+    bytes or None
+
+    Examples
+    --------
+    Load bytes of 850hPa temperature from GRAPES GFS GMF and create GRIB message using `eccodes.codes_new_from_message`.
+
+    >>> file_path = "/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2"
+    >>> message_bytes = load_bytes_from_file(
+    ...     file_path=file_path,
+    ...     parameter="t",
+    ...     level_type="pl",
+    ...     level=850,
+    ... )
+    >>> message = eccodes.codes_new_from_message(message_bytes)
+    >>> values = eccodes.codes_get_double_array(message, "values")
+    >>> print(len(values))
+    1036800
+
+    """
+    offset = 0
+
+    fixed_level_type = fix_level_type(level_type)
+
+    parameter = convert_parameter(parameter)
+
+    with open(file_path, "rb") as f:
+        while True:
+            message_id = eccodes.codes_grib_new_from_file(f)
+            length = eccodes.codes_get(message_id, "totalLength")
+            if message_id is None:
+                return None
+            if not _check_message(message_id, parameter, fixed_level_type, level):
+                eccodes.codes_release(message_id)
+                offset += length
+                continue
+            return eccodes.codes_get_message(message_id)
+
+
+def create_message_from_bytes(raw_message: bytes) -> Optional[int]:
+    """
+    Create **the first** message from raw bytes.
+
+    The returned message should be released using ``eccodes.codes_release`` manually.
+
+    Parameters
+    ----------
+    raw_message
+
+    Returns
+    -------
+    int or None
+    """
+    return eccodes.codes_new_from_message(raw_message)
+
+
+def create_messages_from_bytes(raw_message: bytes) -> List[int]:
+    """
+    Create all messages from raw bytes.
+
+    The returned messages should be released using ``eccodes.codes_release`` manually.
+
+    Parameters
+    ----------
+    raw_message
+
+    Returns
+    -------
+    int or None
+
+    Examples
+    --------
+    Load raw bytes of temperature at 500hPa and 850hPa and reload them from raw bytes.
+    Print level value of all returned messages.
+
+    >>> file_path = "/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2"
+    >>> message_bytes_t850 = load_bytes_from_file(
+    ...     file_path=file_path,
+    ...     parameter="t",
+    ...     level_type="pl",
+    ...     level=850,
+    ... )
+    >>> message_bytes_t500 = load_bytes_from_file(
+    ...     file_path=file_path,
+    ...     parameter="t",
+    ...     level_type="pl",
+    ...     level=500,
+    ... )
+    >>> message_bytes = message_bytes_t500 + message_bytes_t850
+    >>> messages = create_messages_from_bytes(message_bytes)
+    >>> for message in messages:
+    ...     print(eccodes.codes_get(message, "level"))
+    500
+    850
+
+    """
+    messages = []
+    message_bytes = raw_message
+
+    while len(message_bytes) > 0:
+        message = create_message_from_bytes(message_bytes)
+        if message is None:
+            break
+        message_size = eccodes.codes_get_message_size(message)
+        messages.append(message)
+        message_bytes = message_bytes[message_size:]
+    return messages
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/field.py` & `reki-2024.4.0/reki/format/grib/eccodes/field.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,281 +1,318 @@
-import typing
-from typing import Union, List, Dict, Optional
-from pathlib import Path
-
-import eccodes
-import xarray as xr
-from tqdm import tqdm
-
-from ._level import _fix_level
-from ._util import _check_message
-from ._xarray import create_data_array_from_message, get_level_coordinate_name
-from reki._util import _load_first_variable
-
-
-def load_field_from_file(
-        file_path: Union[str, Path],
-        parameter: Union[str, Dict] = None,
-        level_type: Union[str, Dict] = None,
-        level: Union[int, float, List, Dict] = None,
-        level_dim: Optional[str] = None,
-        show_progress: bool = False,
-        **kwargs
-) -> Optional[xr.DataArray]:
-    """
-    Load **one** field from local GRIB2 file using eccodes-python.
-    Or load multi levels into one field.
-
-    Parameters
-    ----------
-    file_path: str or Path
-    parameter: str or typing.Dict
-        parameter name.
-        Use GRIB key `shortName` or a dict of filter conditions such as:
-            {
-                "discipline": 0,
-                "parameterCategory": 2,
-                "parameterNumber": 225,
-            }
-
-    level_type: str or typing.Dict or None
-        level type.
-
-        - Use "pl", "ml" or "sfc". They will be converted into dict.
-        - Use GRIB key `typeOfLevel`, such as
-            - "isobaricInhPa"
-            - "isobaricInPa"
-            - "surface"
-            - "heightAboveGround"
-            - ...
-          See https://apps.ecmwf.int/codes/grib/format/edition-independent/3/ for more values.
-        - If `typeOfLevel` is not available, use dict to specify filter conditions.
-          For example, to get one filed from GRAPES GFS modelvar GRIB2 file, use:
-            {
-                "typeOfFirstFixedSurface": 131
-            }
-
-    level: int or float or typing.List or typing.Dict or None
-        level value(s).
-
-        - If use a scalar, level will be a non-dimension coordinate.
-        - If your want to extract multi levels, use a list and level will be a dimension (level, lat, lon).
-        - If use a dict, message will be filtered by dict keys. Support custom calculate keys:
-            - ``first_level``
-            - ``second_level``
-        - If use `"all"`, all levels of level_type will be packed in the result field.
-        - If use `None`, only the first field will be returned.
-
-    level_dim: str or None
-        name of level dimension.
-        If none, function will generate a name for level dim.
-        If `level_type="pl"`, some values can be used:
-
-            - `None` or `pl` or `isobaricInhPa`: level_dim is a float number with unit hPa.
-            - `isobaricInPa`: level_dim is a float number with unit Pa.
-
-    show_progress: bool
-        show progress bar.
-
-    Returns
-    -------
-    DataArray or None:
-        DataArray if found, or None if not.
-
-    Examples
-    --------
-    Load 850hPa temperature field from a GRIB2 file generated by GRAPES GFS.
-
-    >>> load_field_from_file(
-    ...     file_path="/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-    ...     parameter="t",
-    ...     level_type="isobaricInhPa",
-    ...     level=850,
-    ... )
-    <xarray.DataArray 't' (latitude: 720, longitude: 1440)>
-    array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
-            249.19234375, 249.14234375],
-           [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
-            249.44234375, 249.44234375],
-           [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
-            249.67234375, 249.68234375],
-           ...,
-           [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
-            235.63234375, 235.48234375],
-           [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
-            235.72234375, 235.82234375],
-           [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
-            235.68234375, 235.70234375]])
-    Coordinates:
-        time           datetime64[ns] 2020-03-18
-        step           timedelta64[ns] 4 days 09:00:00
-        valid_time     datetime64[ns] 2020-03-22T09:00:00
-        isobaricInhPa  int64 850
-      * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
-      * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
-    Attributes:
-        GRIB_edition:                    2
-        GRIB_centre:                     babj
-        GRIB_subCentre:                  0
-        GRIB_tablesVersion:              4
-        GRIB_localTablesVersion:         1
-        GRIB_dataType:                   fc
-        GRIB_dataDate:                   20200318
-        GRIB_dataTime:                   0
-        GRIB_validityDate:               20200322
-        GRIB_validityTime:               900
-        GRIB_step:                       105
-        GRIB_stepType:                   instant
-        GRIB_stepUnits:                  1
-        GRIB_stepRange:                  105
-        GRIB_endStep:                    105
-        GRIB_name:                       Temperature
-        GRIB_shortName:                  t
-        GRIB_cfName:                     air_temperature
-        GRIB_discipline:                 0
-        GRIB_parameterCategory:          0
-        GRIB_parameterNumber:            0
-        GRIB_gridType:                   regular_ll
-        GRIB_gridDefinitionDescription:  Latitude/longitude
-        GRIB_typeOfFirstFixedSurface:    pl
-        GRIB_typeOfLevel:                isobaricInhPa
-        GRIB_level:                      850
-        GRIB_numberOfPoints:             1036800
-        GRIB_missingValue:               9999
-        GRIB_units:                      K
-        long_name:                       Temperature
-        units:                           K
-
-    """
-    messages = []
-
-    fixed_level_type, fixed_level_dim = _fix_level(level_type, level_dim)
-
-    if show_progress:
-        with open(file_path, "rb") as f:
-            total_count = eccodes.codes_count_in_file(f)
-
-    with open(file_path, "rb") as f:
-        if show_progress:
-            pbar = tqdm(
-                total=total_count,
-                desc="Filtering",
-            )
-        while True:
-            message_id = eccodes.codes_grib_new_from_file(f)
-            if message_id is None:
-                break
-            if show_progress:
-                pbar.update(1)
-            if not _check_message(message_id, parameter, fixed_level_type, level, **kwargs):
-                eccodes.codes_release(message_id)
-                continue
-            messages.append(message_id)
-            if isinstance(level, typing.List) or level == "all":
-                continue
-            else:
-                break
-        if show_progress:
-            pbar.close()
-
-    if len(messages) == 0:
-        return None
-
-    if len(messages) == 1:
-        message_id = messages[0]
-        data = create_data_array_from_message(message_id, level_dim_name=fixed_level_dim)
-        eccodes.codes_release(message_id)
-        return data
-
-    if len(messages) > 1:
-        if show_progress:
-            pbar = tqdm(
-                total=len(messages),
-                desc="Decoding",
-            )
-
-        def creat_array(message):
-            array = create_data_array_from_message(message, level_dim_name=fixed_level_dim)
-            if show_progress:
-                pbar.update(1)
-            return array
-
-        xarray_messages = [creat_array(message) for message in messages]
-        for m in messages:
-            eccodes.codes_release(m)
-        if show_progress:
-            pbar.close()
-
-        if level_dim is None:
-            if isinstance(level_type, str):
-                level_dim_name = level_type
-            elif isinstance(level_type, typing.Dict):
-                level_dim_name = get_level_coordinate_name(xarray_messages[0])
-            else:
-                raise ValueError(f"level_type is not supported: {level_type}")
-        elif isinstance(level_dim, str):
-            level_dim_name = level_dim
-        else:
-            raise ValueError(f"level_type is not supported: {level_type}")
-
-        if show_progress:
-            print("Packing...")
-
-        data = xr.concat(xarray_messages, level_dim_name)
-        return data
-
-    return None
-
-
-def load_field_from_files(
-        file_list: List,
-        parameter: Union[str, Dict],
-        level_type: Union[str, Dict],
-        level: Optional[Union[int, float, List, Dict]],
-        level_dim: Optional[str] = None,
-        show_progress: bool = False,
-        **kwargs
-) -> Optional[xr.DataArray]:
-    """
-    Load one field from multiply files.
-
-    Parameters
-    ----------
-    file_list: typing.List
-        file list.
-    parameter: str or typing.Dict
-        see ``load_field_from_file``
-    level_type: str or typing.Dict
-        see ``load_field_from_file``
-    level: int or float or typing.List or None
-        see ``load_field_from_file``
-    level_dim: str or None
-        level dimension name.
-    show_progress: bool
-        see ``load_field_from_file``
-
-    Returns
-    -------
-    xr.DataArray or None:
-        xr.DataArray if found, or None if not.
-
-    """
-    field_list = []
-    for file_path in file_list:
-        print(file_path)
-        field = load_field_from_file(
-            file_path,
-            parameter=parameter,
-            level_type=level_type,
-            level=level,
-            level_dim=level_dim,
-            show_progress=show_progress,
-            **kwargs
-        )
-        field_list.append(field)
-
-    data_set = xr.combine_by_coords(
-        [f.expand_dims(["time", "step"]).to_dataset() for f in field_list]
-    )
-    data = _load_first_variable(data_set)
-    data = data.transpose("time", "step", ...)
-    return data
+import typing
+from typing import Union, List, Dict, Optional
+from pathlib import Path
+
+import eccodes
+import xarray as xr
+from tqdm import tqdm
+
+from ._level import _fix_level
+from ._util import _check_message
+from ._xarray import create_data_array_from_message, get_level_coordinate_name
+from reki._util import _load_first_variable
+from reki.format.grib.common._parameter import convert_parameter
+
+
+def load_field_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict] = None,
+        level_type: Union[str, Dict] = None,
+        level: Union[int, float, List, Dict, str] = None,
+        level_dim: Optional[str] = None,
+        field_name: Optional[str] = None,
+        show_progress: bool = False,
+        **kwargs
+) -> Optional[xr.DataArray]:
+    """
+    Load **one** field from local GRIB2 file using eccodes-python.
+    Or load multi levels into one field.
+
+    Parameters
+    ----------
+    file_path : str or Path
+    parameter : str or typing.Dict
+        parameter name.
+
+        Use GRIB key `shortName` or a dict of filter conditions such as:
+
+        .. code-block::
+
+            {
+                "discipline": 0,
+                "parameterCategory": 2,
+                "parameterNumber": 225,
+            }
+
+    level_type : str or typing.Dict or None
+        level type.
+
+        - Use "pl", "ml" or "sfc". They will be converted into dict.
+        - Use GRIB key `typeOfLevel`, such as
+            - "isobaricInhPa"
+            - "isobaricInPa"
+            - "surface"
+            - "heightAboveGround"
+            - "nominalTop"
+            - "atmosphere"
+            - "meanSea"
+            - "depthBelowLandLayer"
+            - ...
+          See https://apps.ecmwf.int/codes/grib/format/edition-independent/3/ for more values.
+        - If `typeOfLevel` is not available, use dict to specify filter conditions.
+          For example, to get one filed from GRAPES GFS modelvar GRIB2 file, use:
+
+          .. code-block::
+
+            {
+                "typeOfFirstFixedSurface": 131
+            }
+
+    level : int or float or typing.List or typing.Dict or None
+        level value(s).
+
+        - If use a scalar, level will be a non-dimension coordinate.
+        - If your want to extract multi levels, use a list and level will be a dimension (level, lat, lon).
+        - If use a dict, message will be filtered by dict keys. Support custom calculate keys:
+            - ``first_level``
+            - ``second_level``
+        - If use `"all"`, all levels of level_type will be packed in the result field.
+        - If use `None`, only the first field will be returned.
+
+    level_dim : str or None
+        name of level dimension.
+        If none, function will generate a name for level dim.
+        If `level_type="pl"`, some values can be used:
+
+            - `None` or `pl` or `isobaricInhPa`: level_dim is a float number with unit hPa.
+            - `isobaricInPa`: level_dim is a float number with unit Pa.
+
+    field_name :
+        name of field.
+
+        * If ``None``, generate field name automatically.
+            * use ``parameter`` if it's a string
+            * use GRIB Key shortName if it's not `unknown`
+            * use GRIB Keys to combine a name: `discipline_parameterCategory_parameterNumber`
+        * If string, set the field's name with it.
+
+    show_progress : bool
+        show progress bar.
+
+    Returns
+    -------
+    DataArray or None:
+        DataArray if found, or None if not.
+
+    Examples
+    --------
+    Load 850hPa temperature field from a GRIB2 file generated by GRAPES GFS.
+
+    .. code-block:: pycon
+
+        >>> load_field_from_file(
+        ...     file_path="/sstorage1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
+        ...     parameter="t",
+        ...     level_type="isobaricInhPa",
+        ...     level=850,
+        ... )
+        <xarray.DataArray 't' (latitude: 720, longitude: 1440)>
+        array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
+                249.19234375, 249.14234375],
+               [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
+                249.44234375, 249.44234375],
+               [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
+                249.67234375, 249.68234375],
+               ...,
+               [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
+                235.63234375, 235.48234375],
+               [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
+                235.72234375, 235.82234375],
+               [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
+                235.68234375, 235.70234375]])
+        Coordinates:
+            time           datetime64[ns] 2020-03-18
+            step           timedelta64[ns] 4 days 09:00:00
+            valid_time     datetime64[ns] 2020-03-22T09:00:00
+            isobaricInhPa  int64 850
+          * latitude       (latitude) float64 89.88 89.62 89.38 ... -89.38 -89.62 -89.88
+          * longitude      (longitude) float64 0.0 0.25 0.5 0.75 ... 359.2 359.5 359.8
+        Attributes:
+            GRIB_edition:                    2
+            GRIB_centre:                     babj
+            GRIB_subCentre:                  0
+            GRIB_tablesVersion:              4
+            GRIB_localTablesVersion:         1
+            GRIB_dataType:                   fc
+            GRIB_dataDate:                   20200318
+            GRIB_dataTime:                   0
+            GRIB_validityDate:               20200322
+            GRIB_validityTime:               900
+            GRIB_step:                       105
+            GRIB_stepType:                   instant
+            GRIB_stepUnits:                  1
+            GRIB_stepRange:                  105
+            GRIB_endStep:                    105
+            GRIB_name:                       Temperature
+            GRIB_shortName:                  t
+            GRIB_cfName:                     air_temperature
+            GRIB_discipline:                 0
+            GRIB_parameterCategory:          0
+            GRIB_parameterNumber:            0
+            GRIB_gridType:                   regular_ll
+            GRIB_gridDefinitionDescription:  Latitude/longitude
+            GRIB_typeOfFirstFixedSurface:    pl
+            GRIB_typeOfLevel:                isobaricInhPa
+            GRIB_level:                      850
+            GRIB_numberOfPoints:             1036800
+            GRIB_missingValue:               9999
+            GRIB_units:                      K
+            long_name:                       Temperature
+            units:                           K
+
+    """
+    messages = []
+
+    fixed_level_type, fixed_level_dim = _fix_level(level_type, level_dim)
+
+    if field_name is None and isinstance(parameter, str):
+        field_name = parameter
+
+    parameter = convert_parameter(parameter)
+
+    if show_progress:
+        with open(file_path, "rb") as f:
+            total_count = eccodes.codes_count_in_file(f)
+
+    with open(file_path, "rb") as f:
+        if show_progress:
+            pbar = tqdm(
+                total=total_count,
+                desc="Filtering",
+            )
+        while True:
+            message_id = eccodes.codes_grib_new_from_file(f)
+            if message_id is None:
+                break
+            if show_progress:
+                pbar.update(1)
+            if not _check_message(message_id, parameter, fixed_level_type, level, **kwargs):
+                eccodes.codes_release(message_id)
+                continue
+            messages.append(message_id)
+            if isinstance(level, typing.List) or level == "all":
+                continue
+            else:
+                break
+        if show_progress:
+            pbar.close()
+
+    if len(messages) == 0:
+        return None
+
+    if len(messages) == 1:
+        message_id = messages[0]
+        data = create_data_array_from_message(
+            message_id,
+            level_dim_name=fixed_level_dim,
+            field_name=field_name,
+        )
+        eccodes.codes_release(message_id)
+        return data
+
+    if len(messages) > 1:
+        if show_progress:
+            pbar = tqdm(
+                total=len(messages),
+                desc="Decoding",
+            )
+
+        def creat_array(message):
+            array = create_data_array_from_message(
+                message,
+                level_dim_name=fixed_level_dim,
+                field_name=field_name
+            )
+            if show_progress:
+                pbar.update(1)
+            return array
+
+        xarray_messages = [creat_array(message) for message in messages]
+        for m in messages:
+            eccodes.codes_release(m)
+        if show_progress:
+            pbar.close()
+
+        if level_dim is None:
+            if isinstance(level_type, str):
+                level_dim_name = level_type
+            elif isinstance(level_type, typing.Dict):
+                level_dim_name = get_level_coordinate_name(xarray_messages[0])
+            else:
+                raise ValueError(f"level_type is not supported: {level_type}")
+        elif isinstance(level_dim, str):
+            level_dim_name = level_dim
+        else:
+            raise ValueError(f"level_type is not supported: {level_type}")
+
+        if show_progress:
+            print("Packing...")
+
+        data = xr.concat(xarray_messages, level_dim_name)
+        return data
+
+    return None
+
+
+def load_field_from_files(
+        file_list: List,
+        parameter: Union[str, Dict],
+        level_type: Union[str, Dict],
+        level: Optional[Union[int, float, List, Dict]],
+        level_dim: Optional[str] = None,
+        show_progress: bool = False,
+        **kwargs
+) -> Optional[xr.DataArray]:
+    """
+    Load one field from multiply files.
+
+    Parameters
+    ----------
+    file_list: typing.List
+        file list.
+    parameter: str or typing.Dict
+        see ``load_field_from_file``
+    level_type: str or typing.Dict
+        see ``load_field_from_file``
+    level: int or float or typing.List or None
+        see ``load_field_from_file``
+    level_dim: str or None
+        level dimension name.
+    show_progress: bool
+        see ``load_field_from_file``
+
+    Returns
+    -------
+    xr.DataArray or None:
+        xr.DataArray if found, or None if not.
+
+    """
+    field_list = []
+    for file_path in file_list:
+        print(file_path)
+        field = load_field_from_file(
+            file_path,
+            parameter=parameter,
+            level_type=level_type,
+            level=level,
+            level_dim=level_dim,
+            show_progress=show_progress,
+            **kwargs
+        )
+        field_list.append(field)
+
+    data_set = xr.combine_by_coords(
+        [f.expand_dims(["time", "step"]).to_dataset() for f in field_list]
+    )
+    data = _load_first_variable(data_set)
+    data = data.transpose("time", "step", ...)
+    return data
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/message.py` & `reki-2024.4.0/reki/format/grib/eccodes/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,205 @@
-import typing
-from typing import Union, List, Dict, Optional
-from pathlib import Path
-
-import eccodes
-# from tqdm import tqdm
-
-from ._level import _fix_level
-from ._util import (
-    _check_parameter,
-    _check_level_type,
-    _check_level_value,
-    _check_keys,
-    _check_message,
-)
-
-
-def load_message_from_file(
-        file_path: Union[str, Path],
-        parameter: Union[str, Dict] = None,
-        level_type: Union[str, Dict] = None,
-        level: Union[int, float, Dict] = None,
-        count: int = None,
-        **kwargs,
-) -> Optional[int]:
-    """
-    Load the **first** message from GRIB 2 file using eccodes-python library.
-
-    Returned message is a copied one of original message and file is closed before return.
-    And the returned message should be released by user using `eccodes.codes_release()`.
-
-    Parameters
-    ----------
-    file_path
-        GRIB 2 file path.
-    parameter
-        short name of the field or a dictionary including some GRIB keys:
-
-        - discipline
-        - parameterCategory
-        - parameterNumber
-
-    level_type
-        level type.
-    level
-        level value.
-    kwargs
-        other grib key used to filter.
-    count
-        grib message index in grib file, starting with 1
-    Returns
-    -------
-    int or None
-        GRIB handler (int) if found or None if not found.
-
-    Examples
-    --------
-    Load 850hPa temperature from GRAPES GFS and get values from GRIB message.
-
-    >>> t = load_message_from_file(
-    ...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
-    ...     parameter="t",
-    ...     level_type="isobaricInhPa",
-    ...     level=850,
-    ... )
-    >>> data = eccodes.codes_get_double_array(t, "values")
-    >>> data = data.reshape([720, 1440])
-    >>> data
-    array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
-        249.19234375, 249.14234375],
-       [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
-        249.44234375, 249.44234375],
-       [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
-        249.67234375, 249.68234375],
-       ...,
-       [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
-        235.63234375, 235.48234375],
-       [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
-        235.72234375, 235.82234375],
-       [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
-        235.68234375, 235.70234375]])
-
-    """
-    if count is not None:
-        return _load_message_from_file_by_count(file_path, count)
-
-    fixed_level_type, _ = _fix_level(level_type, None)
-    with open(file_path, "rb") as f:
-        while True:
-            message_id = eccodes.codes_grib_new_from_file(f)
-            if message_id is None:
-                return None
-            if not _check_message(message_id, parameter, fixed_level_type, level, **kwargs):
-                eccodes.codes_release(message_id)
-                continue
-            return message_id
-
-            # # clone message
-            # new_message_id = eccodes.codes_clone(message_id)
-            # eccodes.codes_release(message_id)
-            # return new_message_id
-        return None
-
-
-def load_messages_from_file(
-        file_path: Union[str, Path],
-        parameter: Union[str, Dict],
-        level_type: Union[str, Dict, List] = None,
-        level: Union[int, float, List, Dict] = None,
-        **kwargs,
-) -> Optional[List]:
-    """
-    Load multiply messages from file.
-
-    This function will scan all messages in GRIB 2 file and return all messages which fit conditions.
-
-    Parameters
-    ----------
-    file_path: str or Path
-    parameter: str or typing.Dict
-        see ``load_message_from_file``, required option.
-    level_type: str or typing.List or None
-        level type.
-        - string, same as ``load_message_from_file``
-        - typing.List, level type should be in the list.
-        - None, don't check level type.
-    level: int or float or typing.Dict or typing.List or None
-        level value.
-        - string, same as ``load_message_from_file``
-        - typing.Dict, same as ``load_message_from_file``
-        - typing.List, level value should be in the list.
-        - None, don't check level value. For example, load all messages of some typeOfLevel.
-    kwargs: dict
-        other grib key used to filter.
-
-    Returns
-    -------
-    typing.List or None:
-        a list of message number or None if no message is found.
-    """
-    fixed_level_type, _ = _fix_level(level_type, None)
-
-    messages = []
-
-    # print("count...")
-    # with open(file_path, "rb") as f:
-    #     total_count = eccodes.codes_count_in_file(f)
-    #     print(total_count)
-    # print("count..done")
-
-    with open(file_path, "rb") as f:
-        # pbar = tqdm(total=total_count)
-        while True:
-            message_id = eccodes.codes_grib_new_from_file(f)
-            if message_id is None:
-                break
-            # pbar.update(1)
-            if not _check_parameter(message_id, parameter):
-                eccodes.codes_release(message_id)
-                continue
-            if not _check_level_type(message_id, fixed_level_type):
-                eccodes.codes_release(message_id)
-                continue
-            if not _check_level_value(message_id, level):
-                eccodes.codes_release(message_id)
-                continue
-            if not _check_keys(message_id, **kwargs):
-                eccodes.codes_release(message_id)
-                continue
-
-            # clone message
-            new_message_id = eccodes.codes_clone(message_id)
-            eccodes.codes_release(message_id)
-            messages.append(new_message_id)
-        # pbar.close()
-        if len(messages) == 0:
-            return None
-        return messages
-
-
-def _load_message_from_file_by_count(file_path, count):
-    current_index = 0
-    with open(file_path, "rb") as f:
-        while True:
-            message_id = eccodes.codes_grib_new_from_file(f)
-            if message_id is None:
-                return None
-            current_index += 1
-            if current_index == count:
-                return message_id
-            else:
-                eccodes.codes_release(message_id)
+import typing
+from typing import Union, List, Dict, Optional
+from pathlib import Path
+
+import eccodes
+# from tqdm import tqdm
+
+from ._level import _fix_level
+from ._util import (
+    _check_parameter,
+    _check_level_type,
+    _check_level_value,
+    _check_keys,
+    _check_message,
+)
+
+from reki.format.grib.common._parameter import convert_parameter
+
+
+def load_message_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict] = None,
+        level_type: Union[str, Dict] = None,
+        level: Union[int, float, Dict] = None,
+        count: int = None,
+        look_parameter: bool = True,
+        **kwargs,
+) -> Optional[int]:
+    """
+    Load the **first** message from GRIB 2 file using eccodes-python library.
+
+    Returned message is a copied one of original message and file is closed before return.
+    And the returned message should be released by user using `eccodes.codes_release()`.
+
+    Parameters
+    ----------
+    file_path
+        GRIB 2 file path.
+    parameter
+        short name of the field, or a dict of GRIB keys:
+
+        * discipline
+        * parameterCategory
+        * parameterNumber
+
+    level_type
+        level type.
+    level
+        level value.
+    kwargs
+        other grib key used to filter.
+    count
+        grib message index in grib file, starting with 1.
+
+        This option will make all others options ignored.
+
+    Returns
+    -------
+    Union[int]
+        GRIB handler (int) if found or None if not found.
+
+    Examples
+    --------
+    Load 850hPa temperature from GRAPES GFS and get values from GRIB message.
+
+    >>> t = load_message_from_file(
+    ...     file_path="/g1/COMMONDATA/OPER/NWPC/GRAPES_GFS_GMF/Prod-grib/2020031721/ORIG/gmf.gra.2020031800105.grb2",
+    ...     parameter="t",
+    ...     level_type="isobaricInhPa",
+    ...     level=850,
+    ... )
+    >>> data = eccodes.codes_get_double_array(t, "values")
+    >>> data = data.reshape([720, 1440])
+    >>> data
+    array([[249.19234375, 249.16234375, 249.16234375, ..., 249.15234375,
+        249.19234375, 249.14234375],
+       [249.45234375, 249.45234375, 249.42234375, ..., 249.45234375,
+        249.44234375, 249.44234375],
+       [249.69234375, 249.68234375, 249.68234375, ..., 249.70234375,
+        249.67234375, 249.68234375],
+       ...,
+       [235.33234375, 235.45234375, 235.62234375, ..., 235.47234375,
+        235.63234375, 235.48234375],
+       [235.78234375, 235.91234375, 235.64234375, ..., 235.80234375,
+        235.72234375, 235.82234375],
+       [235.66234375, 235.86234375, 235.82234375, ..., 235.85234375,
+        235.68234375, 235.70234375]])
+    >>> eccodes.codes_release(t)
+
+    """
+    if count is not None:
+        return _load_message_from_file_by_count(file_path, count)
+
+    fixed_level_type, _ = _fix_level(level_type, None)
+
+    if look_parameter:
+        parameter = convert_parameter(parameter)
+
+    with open(file_path, "rb") as f:
+        while True:
+            message_id = eccodes.codes_grib_new_from_file(f)
+            if message_id is None:
+                return None
+            if not _check_message(message_id, parameter, fixed_level_type, level, **kwargs):
+                eccodes.codes_release(message_id)
+                continue
+            return message_id
+
+            # # clone message
+            # new_message_id = eccodes.codes_clone(message_id)
+            # eccodes.codes_release(message_id)
+            # return new_message_id
+        return None
+
+
+def load_messages_from_file(
+        file_path: Union[str, Path],
+        parameter: Union[str, Dict],
+        level_type: Union[str, Dict, List] = None,
+        level: Union[int, float, List, Dict] = None,
+        **kwargs,
+) -> Optional[List]:
+    """
+    Load multiply messages from file.
+
+    This function will scan all messages in GRIB 2 file and return all messages which fit conditions.
+
+    Parameters
+    ----------
+    file_path: str or Path
+    parameter: str or typing.Dict
+        see ``load_message_from_file``, required option.
+    level_type: str or typing.List or None
+        level type.
+        - string, same as ``load_message_from_file``
+        - typing.List, level type should be in the list.
+        - None, don't check level type.
+    level: int or float or typing.Dict or typing.List or None
+        level value.
+        - string, same as ``load_message_from_file``
+        - typing.Dict, same as ``load_message_from_file``
+        - typing.List, level value should be in the list.
+        - None, don't check level value. For example, load all messages of some typeOfLevel.
+    kwargs: dict
+        other grib key used to filter.
+
+    Returns
+    -------
+    typing.List or None:
+        a list of message number or None if no message is found.
+    """
+    fixed_level_type, _ = _fix_level(level_type, None)
+
+    parameter = convert_parameter(parameter)
+
+    messages = []
+
+    # print("count...")
+    # with open(file_path, "rb") as f:
+    #     total_count = eccodes.codes_count_in_file(f)
+    #     print(total_count)
+    # print("count..done")
+
+    with open(file_path, "rb") as f:
+        # pbar = tqdm(total=total_count)
+        while True:
+            message_id = eccodes.codes_grib_new_from_file(f)
+            if message_id is None:
+                break
+            # pbar.update(1)
+            if not _check_parameter(message_id, parameter):
+                eccodes.codes_release(message_id)
+                continue
+            if not _check_level_type(message_id, fixed_level_type):
+                eccodes.codes_release(message_id)
+                continue
+            if not _check_level_value(message_id, level):
+                eccodes.codes_release(message_id)
+                continue
+            if not _check_keys(message_id, **kwargs):
+                eccodes.codes_release(message_id)
+                continue
+
+            # clone message
+            new_message_id = eccodes.codes_clone(message_id)
+            eccodes.codes_release(message_id)
+            messages.append(new_message_id)
+        # pbar.close()
+        if len(messages) == 0:
+            return None
+        return messages
+
+
+def _load_message_from_file_by_count(file_path, count):
+    current_index = 0
+    with open(file_path, "rb") as f:
+        while True:
+            message_id = eccodes.codes_grib_new_from_file(f)
+            if message_id is None:
+                return None
+            current_index += 1
+            if current_index == count:
+                return message_id
+            else:
+                eccodes.codes_release(message_id)
```

### Comparing `reki-0.3.0/reki/format/grib/eccodes/util.py` & `reki-2024.4.0/reki/format/grib/eccodes/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Optional, Union, List, Dict
-
-from ._util import _check_message
-from ._level import _fix_level
-from reki.format.grib._parameter import _convert_parameter
-
-
-def check_message(
-        message_id,
-        parameter: Optional[Union[str, Dict]],
-        level_type: Optional[Union[str, List[str]]],
-        level: Optional[Union[int, List[int], Dict]],
-        **kwargs,
-) -> bool:
-    """
-    Check whether GRIB message fits conditions.
-
-    Parameters
-    ----------
-    message_id
-    parameter
-    level_type
-    level
-    kwargs
-
-    Returns
-    -------
-    bool
-    """
-    parameter = _convert_parameter(parameter)
-    level_type, _ = _fix_level(level_type, None)
-
-    return _check_message(
-        message_id,
-        parameter=parameter,
-        level_type=level_type,
-        level=level,
-        **kwargs
-    )
+from typing import Optional, Union, List, Dict
+
+from ._util import _check_message
+from ._level import _fix_level
+from reki.format.grib.common import convert_parameter
+
+
+def check_message(
+        message_id,
+        parameter: Optional[Union[str, Dict]],
+        level_type: Optional[Union[str, List[str]]],
+        level: Optional[Union[int, List[int], Dict]],
+        **kwargs,
+) -> bool:
+    """
+    Check whether GRIB message fits conditions.
+
+    Parameters
+    ----------
+    message_id
+    parameter
+    level_type
+    level
+    kwargs
+
+    Returns
+    -------
+    bool
+    """
+    # parameter = _convert_parameter(parameter)
+    level_type, _ = _fix_level(level_type, None)
+
+    return _check_message(
+        message_id,
+        parameter=parameter,
+        level_type=level_type,
+        level=level,
+        **kwargs
+    )
```

### Comparing `reki-0.3.0/reki/format/netcdf/__init__.py` & `reki-2024.4.0/reki/format/netcdf/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from pathlib import Path
-import typing
-from typing import Union, Dict, Optional
-
-import xarray as xr
-
-from reki._util import _load_first_variable
-
-
-def load_field_from_file(
-        file_path: str or Path,
-        parameter: Union[str, Dict] = None,
-        level_type: Union[str, Dict] = None,
-        level: Optional[Union[int, float]] = None,
-        **kwargs
-) -> Optional[xr.DataArray]:
-    """
-    Load **one** field from NetCDF file.
-
-    Parameters
-    ----------
-    file_path
-    parameter
-    level_type
-        level type, default is level.
-    level
-    **kwargs
-        other parameters used by engine.
-
-    Returns
-    -------
-    DataArray or None:
-        DataArray if found one field, or None if not.
-    """
-    ds = xr.open_dataset(file_path)
-    if parameter is None:
-        field = _load_first_variable(ds)
-    else:
-        field = ds[parameter]
-
-    if level is not None:
-        if level_type is None:
-            level_type = "level"
-        field = field.loc[{
-            level_type: level
-        }]
-
-    return field
+from pathlib import Path
+import typing
+from typing import Union, Dict, Optional
+
+import xarray as xr
+
+from reki._util import _load_first_variable
+
+
+def load_field_from_file(
+        file_path: str or Path,
+        parameter: Union[str, Dict] = None,
+        level_type: Union[str, Dict] = None,
+        level: Optional[Union[int, float]] = None,
+        **kwargs
+) -> Optional[xr.DataArray]:
+    """
+    Load **one** field from NetCDF file.
+
+    Parameters
+    ----------
+    file_path
+    parameter
+    level_type
+        level type, default is level.
+    level
+    **kwargs
+        other parameters used by engine.
+
+    Returns
+    -------
+    DataArray or None:
+        DataArray if found one field, or None if not.
+    """
+    ds = xr.open_dataset(file_path)
+    if parameter is None:
+        field = _load_first_variable(ds)
+    else:
+        field = ds[parameter]
+
+    if level is not None:
+        if level_type is None:
+            level_type = "level"
+        field = field.loc[{
+            level_type: level
+        }]
+
+    return field
```

### Comparing `reki-0.3.0/reki/operator/regrid/__init__.py` & `reki-2024.4.0/reki/operator/regrid/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import Dict, Union
-
-import xarray as xr
-
-from ._interpolator import _get_interpolator
-
-
-def interpolate_grid(
-        data: xr.DataArray,
-        target: xr.DataArray,
-        scheme: str = "linear",
-        engine: str = "scipy",
-        **kwargs: Dict,
-) -> xr.DataArray:
-    """
-
-    Parameters
-    ----------
-    data
-    target
-    scheme: str
-        interpolate method.
-    engine: str
-        interpolate engine, `scipy` or `xarray`
-    kwargs
-
-    Returns
-    -------
-    xr.DataArray
-    """
-    interpolator = _get_interpolator(scheme, engine, **kwargs)
-
-    target_field = interpolator.interpolate_grid(
-        data=data,
-        target=target,
-    )
-
-    return target_field
-
-
-def extract_point(
-        data: xr.DataArray,
-        latitude: Union[float, int],
-        longitude: Union[float, int],
-        scheme: str = "linear",
-        engine: str = "xarray",
-        **kwargs
-) -> xr.DataArray:
-    """
-    Extract a point from 2D field with interpolation.
-
-    Parameters
-    ----------
-    data
-    latitude
-    longitude
-    scheme
-    engine
-    kwargs
-
-    Returns
-    -------
-    xr.DataArray
-    """
-    interpolator = _get_interpolator(scheme, engine, **kwargs)
-    value = interpolator.extract_point(data, latitude=latitude, longitude=longitude)
-    return value
+from typing import Dict, Union
+
+import xarray as xr
+
+from ._interpolator import _get_interpolator
+
+
+def interpolate_grid(
+        data: xr.DataArray,
+        target: xr.DataArray,
+        scheme: str = "linear",
+        engine: str = "scipy",
+        **kwargs: Dict,
+) -> xr.DataArray:
+    """
+
+    Parameters
+    ----------
+    data
+    target
+    scheme: str
+        interpolate method.
+    engine: str
+        interpolate engine, `scipy` or `xarray`
+    kwargs
+
+    Returns
+    -------
+    xr.DataArray
+    """
+    interpolator = _get_interpolator(scheme, engine, **kwargs)
+
+    target_field = interpolator.interpolate_grid(
+        data=data,
+        target=target,
+    )
+
+    return target_field
+
+
+def extract_point(
+        data: xr.DataArray,
+        latitude: Union[float, int],
+        longitude: Union[float, int],
+        scheme: str = "linear",
+        engine: str = "xarray",
+        **kwargs
+) -> xr.DataArray:
+    """
+    Extract a point from 2D field with interpolation.
+
+    Parameters
+    ----------
+    data
+    latitude
+    longitude
+    scheme
+    engine
+    kwargs
+
+    Returns
+    -------
+    xr.DataArray
+    """
+    interpolator = _get_interpolator(scheme, engine, **kwargs)
+    value = interpolator.extract_point(data, latitude=latitude, longitude=longitude)
+    return value
```

### Comparing `reki-0.3.0/reki/operator/regrid/_interpolator.py` & `reki-2024.4.0/reki/operator/regrid/_interpolator.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import abc
-from typing import Union
-
-import numpy as np
-import xarray as xr
-
-
-class BaseInterpolator(abc.ABC):
-    @abc.abstractmethod
-    def interpolate_grid(
-            self,
-            data: xr.DataArray,
-            target: xr.DataArray,
-    ) -> xr.DataArray:
-        pass
-
-    @abc.abstractmethod
-    def extract_point(
-            self,
-            data: xr.DataArray,
-            latitude: Union[int, float],
-            longitude: Union[int, float],
-    ) -> xr.DataArray:
-        pass
-
-
-def _get_interpolator(
-        scheme: str,
-        engine: str,
-        **kwargs
-) -> BaseInterpolator:
-    if engine == "scipy":
-        from ._scipy import ScipyInterpnInterpolator, ScipyRectBivariateSplineInterpolator
-        if scheme in ["linear", "nearest", "splinef2d"]:
-            return ScipyInterpnInterpolator(scheme, **kwargs)
-        elif scheme in ["rect_bivariate_spline"]:
-            return ScipyRectBivariateSplineInterpolator(scheme, **kwargs)
-        else:
-            raise ValueError(f"{scheme} is not supported for engine {engine}")
-    elif engine == "xarray":
-        from ._xarray import XarrayInterpolator
-        return XarrayInterpolator(scheme, **kwargs)
-    else:
-        raise ValueError(f"engine {engine} is not supported")
-
-
-def _create_data_array(
-        data: xr.DataArray,
-        target: xr.DataArray,
-        target_values: np.ndarray,
-) -> xr.DataArray:
-    coords = data.coords.to_dataset()
-    coords["longitude"] = target["longitude"]
-    coords["latitude"] = target["latitude"]
-
-    target_field = xr.DataArray(
-        target_values,
-        coords=coords.coords,
-        dims=data.dims
-    )
-    return target_field
+import abc
+from typing import Union
+
+import numpy as np
+import xarray as xr
+
+
+class BaseInterpolator(abc.ABC):
+    @abc.abstractmethod
+    def interpolate_grid(
+            self,
+            data: xr.DataArray,
+            target: xr.DataArray,
+    ) -> xr.DataArray:
+        pass
+
+    @abc.abstractmethod
+    def extract_point(
+            self,
+            data: xr.DataArray,
+            latitude: Union[int, float],
+            longitude: Union[int, float],
+    ) -> xr.DataArray:
+        pass
+
+
+def _get_interpolator(
+        scheme: str,
+        engine: str,
+        **kwargs
+) -> BaseInterpolator:
+    if engine == "scipy":
+        from ._scipy import ScipyInterpnInterpolator, ScipyRectBivariateSplineInterpolator
+        if scheme in ["linear", "nearest", "splinef2d"]:
+            return ScipyInterpnInterpolator(scheme, **kwargs)
+        elif scheme in ["rect_bivariate_spline"]:
+            return ScipyRectBivariateSplineInterpolator(scheme, **kwargs)
+        else:
+            raise ValueError(f"{scheme} is not supported for engine {engine}")
+    elif engine == "xarray":
+        from ._xarray import XarrayInterpolator
+        return XarrayInterpolator(scheme, **kwargs)
+    else:
+        raise ValueError(f"engine {engine} is not supported")
+
+
+def _create_data_array(
+        data: xr.DataArray,
+        target: xr.DataArray,
+        target_values: np.ndarray,
+) -> xr.DataArray:
+    coords = data.coords.to_dataset()
+    coords["longitude"] = target["longitude"]
+    coords["latitude"] = target["latitude"]
+
+    target_field = xr.DataArray(
+        target_values,
+        coords=coords.coords,
+        dims=data.dims
+    )
+    return target_field
```

### Comparing `reki-0.3.0/reki/source/gdata/transport/transport_pb2.py` & `reki-2024.4.0/reki/source/gdata/transport/transport_pb2.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: transport.proto
-
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='transport.proto',
-  package='transport',
-  syntax='proto2',
-  serialized_options=None,
-  serialized_pb=b'\n\x0ftransport.proto\x12\ttransport\"\x1d\n\x08RawField\x12\x11\n\traw_bytes\x18\x01 \x02(\x0c'
-)
-
-
-
-
-_RAWFIELD = _descriptor.Descriptor(
-  name='RawField',
-  full_name='transport.RawField',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='raw_bytes', full_name='transport.RawField.raw_bytes', index=0,
-      number=1, type=12, cpp_type=9, label=2,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=30,
-  serialized_end=59,
-)
-
-DESCRIPTOR.message_types_by_name['RawField'] = _RAWFIELD
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-RawField = _reflection.GeneratedProtocolMessageType('RawField', (_message.Message,), {
-  'DESCRIPTOR' : _RAWFIELD,
-  '__module__' : 'transport_pb2'
-  # @@protoc_insertion_point(class_scope:transport.RawField)
-  })
-_sym_db.RegisterMessage(RawField)
-
-
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: transport.proto
+
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='transport.proto',
+  package='transport',
+  syntax='proto2',
+  serialized_options=None,
+  serialized_pb=b'\n\x0ftransport.proto\x12\ttransport\"\x1d\n\x08RawField\x12\x11\n\traw_bytes\x18\x01 \x02(\x0c'
+)
+
+
+
+
+_RAWFIELD = _descriptor.Descriptor(
+  name='RawField',
+  full_name='transport.RawField',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='raw_bytes', full_name='transport.RawField.raw_bytes', index=0,
+      number=1, type=12, cpp_type=9, label=2,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=30,
+  serialized_end=59,
+)
+
+DESCRIPTOR.message_types_by_name['RawField'] = _RAWFIELD
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
+RawField = _reflection.GeneratedProtocolMessageType('RawField', (_message.Message,), {
+  'DESCRIPTOR' : _RAWFIELD,
+  '__module__' : 'transport_pb2'
+  # @@protoc_insertion_point(class_scope:transport.RawField)
+  })
+_sym_db.RegisterMessage(RawField)
+
+
+# @@protoc_insertion_point(module_scope)
```

