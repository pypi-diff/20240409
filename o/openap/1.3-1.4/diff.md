# Comparing `tmp/openap-1.3.tar.gz` & `tmp/openap-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openap-1.3.tar", last modified: Mon Jun 13 13:53:06 2022, max compression
+gzip compressed data, was "openap-1.4.tar", max compression
```

## Comparing `openap-1.3.tar` & `openap-1.4.tar`

### file list

```diff
@@ -1,137 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.914402 openap-1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-06-13 13:52:59.000000 openap-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-13 13:52:59.000000 openap-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-13 13:53:06.914402 openap-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-06-13 13:52:59.000000 openap-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.886402 openap-1.3/openap/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-13 13:52:59.000000 openap-1.3/openap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.886402 openap-1.3/openap/casadi/
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-06-13 13:52:59.000000 openap-1.3/openap/casadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8775 2022-06-13 13:52:59.000000 openap-1.3/openap/casadi/aero_override.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-13 13:52:59.000000 openap-1.3/openap/casadi/numpy_override.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.886402 openap-1.3/openap/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-06-13 13:52:59.000000 openap-1.3/openap/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-06-13 13:52:59.000000 openap-1.3/openap/data/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.894402 openap-1.3/openap/data/aircraft/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/_synonym.csv
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a19n.yml
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a20n.yml
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a21n.yml
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a319.yml
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a320.yml
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a321.yml
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a332.yml
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a333.yml
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a343.yml
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a359.yml
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/a388.yml
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b37m.yml
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b38m.yml
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b39m.yml
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b3xm.yml
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b734.yml
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b737.yml
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b738.yml
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b739.yml
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b744.yml
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b748.yml
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b752.yml
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b763.yml
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b772.yml
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b773.yml
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b77w.yml
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b788.yml
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/b789.yml
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/c550.yml
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/e145.yml
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/e170.yml
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/e190.yml
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/e195.yml
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-06-13 13:52:59.000000 openap-1.3/openap/data/aircraft/e75l.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.898402 openap-1.3/openap/data/dragpolar/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/_synonym.csv
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a20n.yml
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a319.yml
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a320.yml
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a321.yml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a332.yml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a333.yml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a343.yml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a359.yml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/a388.yml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b38m.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b734.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b737.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b738.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b739.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b744.yml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b748.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b752.yml
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b772.yml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b77w.yml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b788.yml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/b789.yml
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/c550.yml
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/e190.yml
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/e195.yml
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-13 13:52:59.000000 openap-1.3/openap/data/dragpolar/e75l.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.898402 openap-1.3/openap/data/engine/
--rw-r--r--   0 runner    (1001) docker     (121)    81420 2022-06-13 13:52:59.000000 openap-1.3/openap/data/engine/engines.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.902402 openap-1.3/openap/data/nav/
--rw-r--r--   0 runner    (1001) docker     (121)   762398 2022-06-13 13:52:59.000000 openap-1.3/openap/data/nav/airports.csv
--rw-r--r--   0 runner    (1001) docker     (121)  3591430 2022-06-13 13:52:59.000000 openap-1.3/openap/data/nav/fix.dat
--rw-r--r--   0 runner    (1001) docker     (121)  2043823 2022-06-13 13:52:59.000000 openap-1.3/openap/data/nav/nav.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.910402 openap-1.3/openap/data/wrap/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/_synonym.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a319.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a320.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a321.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a332.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4385 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a333.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4434 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a343.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/a388.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b737.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4323 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b738.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b739.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b744.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4363 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b752.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b763.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b77w.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b788.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/b789.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4340 2022-06-13 13:52:59.000000 openap-1.3/openap/data/wrap/e190.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-06-13 13:52:59.000000 openap-1.3/openap/drag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6174 2022-06-13 13:52:59.000000 openap-1.3/openap/emission.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.910402 openap-1.3/openap/extra/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-06-13 13:52:59.000000 openap-1.3/openap/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10406 2022-06-13 13:52:59.000000 openap-1.3/openap/extra/aero.py
--rw-r--r--   0 runner    (1001) docker     (121)     4906 2022-06-13 13:52:59.000000 openap-1.3/openap/extra/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-06-13 13:52:59.000000 openap-1.3/openap/extra/nav.py
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-06-13 13:52:59.000000 openap-1.3/openap/extra/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5809 2022-06-13 13:52:59.000000 openap-1.3/openap/fuel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2022-06-13 13:52:59.000000 openap-1.3/openap/kinematic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12961 2022-06-13 13:52:59.000000 openap-1.3/openap/phase.py
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2022-06-13 13:52:59.000000 openap-1.3/openap/prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-06-13 13:52:59.000000 openap-1.3/openap/thrust.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.914402 openap-1.3/openap/traj/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-13 13:52:59.000000 openap-1.3/openap/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17416 2022-06-13 13:52:59.000000 openap-1.3/openap/traj/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.886402 openap-1.3/openap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-13 13:53:06.000000 openap-1.3/openap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-06-13 13:53:06.000000 openap-1.3/openap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 13:53:06.000000 openap-1.3/openap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-13 13:53:06.000000 openap-1.3/openap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-13 13:53:06.000000 openap-1.3/openap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-13 13:53:06.914402 openap-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2022-06-13 13:52:59.000000 openap-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 13:53:06.914402 openap-1.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-06-13 13:52:59.000000 openap-1.3/test/test_actypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-13 13:52:59.000000 openap-1.3/test/test_drag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-06-13 13:52:59.000000 openap-1.3/test/test_emission.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-06-13 13:52:59.000000 openap-1.3/test/test_fuel.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-06-13 13:52:59.000000 openap-1.3/test/test_kinematic.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-06-13 13:52:59.000000 openap-1.3/test/test_nav.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-06-13 13:52:59.000000 openap-1.3/test/test_phase.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-13 13:52:59.000000 openap-1.3/test/test_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-06-13 13:52:59.000000 openap-1.3/test/test_thrust.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-06-13 13:52:59.000000 openap-1.3/test/test_trajectory.py
+-rw-r--r--   0        0        0     7652 2024-04-09 13:17:35.717328 openap-1.4/LICENSE
+-rw-r--r--   0        0        0     2685 2024-04-09 13:17:35.717328 openap-1.4/README.md
+-rw-r--r--   0        0        0      272 2024-04-09 13:17:35.717328 openap-1.4/openap/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/__init__.py
+-rw-r--r--   0        0        0     8774 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/aero_override.py
+-rw-r--r--   0        0        0      271 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/numpy_override.py
+-rw-r--r--   0        0        0     3044 2024-04-09 13:17:35.717328 openap-1.4/openap/contrail.py
+-rw-r--r--   0        0        0     1045 2024-04-09 13:17:35.717328 openap-1.4/openap/data/.gitignore
+-rw-r--r--   0        0        0    35141 2024-04-09 13:17:35.717328 openap-1.4/openap/data/LICENSE
+-rw-r--r--   0        0        0      239 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/_synonym.csv
+-rw-r--r--   0        0        0      626 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a19n.yml
+-rw-r--r--   0        0        0      702 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a20n.yml
+-rw-r--r--   0        0        0      676 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a21n.yml
+-rw-r--r--   0        0        0      735 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a319.yml
+-rw-r--r--   0        0        0      761 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a320.yml
+-rw-r--r--   0        0        0      734 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a321.yml
+-rw-r--r--   0        0        0      700 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a332.yml
+-rw-r--r--   0        0        0      768 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a333.yml
+-rw-r--r--   0        0        0      629 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a343.yml
+-rw-r--r--   0        0        0      585 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a359.yml
+-rw-r--r--   0        0        0      627 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a388.yml
+-rw-r--r--   0        0        0      563 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b37m.yml
+-rw-r--r--   0        0        0      565 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b38m.yml
+-rw-r--r--   0        0        0      564 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b39m.yml
+-rw-r--r--   0        0        0      565 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b3xm.yml
+-rw-r--r--   0        0        0      585 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b734.yml
+-rw-r--r--   0        0        0      635 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b737.yml
+-rw-r--r--   0        0        0      603 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b738.yml
+-rw-r--r--   0        0        0      602 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b739.yml
+-rw-r--r--   0        0        0      607 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b744.yml
+-rw-r--r--   0        0        0      568 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b748.yml
+-rw-r--r--   0        0        0      582 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b752.yml
+-rw-r--r--   0        0        0      602 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b763.yml
+-rw-r--r--   0        0        0      650 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b772.yml
+-rw-r--r--   0        0        0      604 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b773.yml
+-rw-r--r--   0        0        0      575 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b77w.yml
+-rw-r--r--   0        0        0      665 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b788.yml
+-rw-r--r--   0        0        0      649 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b789.yml
+-rw-r--r--   0        0        0      556 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/c550.yml
+-rw-r--r--   0        0        0      564 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e145.yml
+-rw-r--r--   0        0        0      573 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e170.yml
+-rw-r--r--   0        0        0      567 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e190.yml
+-rw-r--r--   0        0        0      567 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e195.yml
+-rw-r--r--   0        0        0      579 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e75l.yml
+-rw-r--r--   0        0        0      600 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/glf6.yml
+-rw-r--r--   0        0        0      328 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/_synonym.csv
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a20n.yml
+-rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a319.yml
+-rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a320.yml
+-rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a321.yml
+-rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a332.yml
+-rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a333.yml
+-rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a343.yml
+-rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a359.yml
+-rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a388.yml
+-rw-r--r--   0        0        0      191 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b38m.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b734.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b737.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b738.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b739.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b744.yml
+-rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b748.yml
+-rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b752.yml
+-rw-r--r--   0        0        0      195 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b772.yml
+-rw-r--r--   0        0        0      191 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b77w.yml
+-rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b788.yml
+-rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b789.yml
+-rw-r--r--   0        0        0      193 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/c550.yml
+-rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e190.yml
+-rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e195.yml
+-rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e75l.yml
+-rw-r--r--   0        0        0      198 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/glf6.yml
+-rw-r--r--   0        0        0    81420 2024-04-09 13:17:35.717328 openap-1.4/openap/data/engine/engines.csv
+-rw-r--r--   0        0        0   762442 2024-04-09 13:17:35.725328 openap-1.4/openap/data/nav/airports.csv
+-rw-r--r--   0        0        0  3591430 2024-04-09 13:17:35.741328 openap-1.4/openap/data/nav/fix.dat
+-rw-r--r--   0        0        0  2043823 2024-04-09 13:17:35.749328 openap-1.4/openap/data/nav/nav.dat
+-rw-r--r--   0        0        0      418 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/_synonym.csv
+-rw-r--r--   0        0        0     4391 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a319.txt
+-rw-r--r--   0        0        0     4386 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a320.txt
+-rw-r--r--   0        0        0     4337 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a321.txt
+-rw-r--r--   0        0        0     4371 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a332.txt
+-rw-r--r--   0        0        0     4385 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a333.txt
+-rw-r--r--   0        0        0     4434 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a343.txt
+-rw-r--r--   0        0        0     4381 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a388.txt
+-rw-r--r--   0        0        0     4396 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b737.txt
+-rw-r--r--   0        0        0     4323 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b738.txt
+-rw-r--r--   0        0        0     4370 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b739.txt
+-rw-r--r--   0        0        0     4378 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b744.txt
+-rw-r--r--   0        0        0     4363 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b752.txt
+-rw-r--r--   0        0        0     4386 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b763.txt
+-rw-r--r--   0        0        0     4359 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b77w.txt
+-rw-r--r--   0        0        0     4378 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b788.txt
+-rw-r--r--   0        0        0     4383 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b789.txt
+-rw-r--r--   0        0        0     4340 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/e190.txt
+-rw-r--r--   0        0        0     6063 2024-04-09 13:17:35.753328 openap-1.4/openap/drag.py
+-rw-r--r--   0        0        0     6174 2024-04-09 13:17:35.753328 openap-1.4/openap/emission.py
+-rw-r--r--   0        0        0      560 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/__init__.py
+-rw-r--r--   0        0        0    10408 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/aero.py
+-rw-r--r--   0        0        0     4971 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/filters.py
+-rw-r--r--   0        0        0     2873 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/nav.py
+-rw-r--r--   0        0        0     2486 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/statistics.py
+-rw-r--r--   0        0        0     5806 2024-04-09 13:17:35.753328 openap-1.4/openap/fuel.py
+-rw-r--r--   0        0        0     6076 2024-04-09 13:17:35.753328 openap-1.4/openap/kinematic.py
+-rw-r--r--   0        0        0    12961 2024-04-09 13:17:35.753328 openap-1.4/openap/phase.py
+-rw-r--r--   0        0        0     3681 2024-04-09 13:17:35.753328 openap-1.4/openap/prop.py
+-rw-r--r--   0        0        0     6371 2024-04-09 13:17:35.753328 openap-1.4/openap/thrust.py
+-rw-r--r--   0        0        0       27 2024-04-09 13:17:35.753328 openap-1.4/openap/traj/__init__.py
+-rw-r--r--   0        0        0    17416 2024-04-09 13:17:35.753328 openap-1.4/openap/traj/gen.py
+-rw-r--r--   0        0        0     1107 2024-04-09 13:17:35.753328 openap-1.4/pyproject.toml
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 openap-1.4/PKG-INFO
```

### Comparing `openap-1.3/LICENSE` & `openap-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openap-1.3/PKG-INFO` & `openap-1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: openap
-Version: 1.3
+Version: 1.4
 Summary: Open Aircraft Performance Model (OpenAP) in Python
 Home-page: https://openap.dev
-Author: Junzi Sun
-Author-email: junzisun@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
-Keywords: OpenAP,Aircraft Performance,Open Data
-Platform: UNKNOWN
+Author: Junzi Sun
+Author-email: j.sun-1@tudelft.nl
+Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: matplotlib (>=3.1)
+Requires-Dist: numpy (>=1.24)
+Requires-Dist: pandas (>=1.2)
+Requires-Dist: pyyaml (>=5.1)
+Requires-Dist: scikit-fuzzy (>=0.4)
+Requires-Dist: scipy (>=1.7)
+Project-URL: Repository, https://github.com/junzis/openap
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Open Aircraft Performance Model (OpenAP) and Toolkit
 
 This repository contains the OpenAP model data and Python packages for aircraft performance and emission calculations.
 
 More information on user guide and related articles at: [OpenAP.dev](https://openap.dev/)
 
@@ -40,15 +49,15 @@
 
 Install the latest stable release from pypi:
 
 ```sh
 pip install --upgrade openap
 ```
 
-Install the latest stable release on conda-froge:
+Install the latest stable release on conda-forge:
 
 ```sh
 conda install openap
 ```
 
 ## Content
 
@@ -95,8 +104,7 @@
   number={8},
   pages={104},
   year={2020},
   publisher={Multidisciplinary Digital Publishing Institute}
 }
 ```
 
-
```

### Comparing `openap-1.3/README.md` & `openap-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Install the latest stable release from pypi:
 
 ```sh
 pip install --upgrade openap
 ```
 
-Install the latest stable release on conda-froge:
+Install the latest stable release on conda-forge:
 
 ```sh
 conda install openap
 ```
 
 ## Content
```

### Comparing `openap-1.3/openap/casadi/__init__.py` & `openap-1.4/openap/casadi/__init__.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/casadi/aero_override.py` & `openap-1.4/openap/casadi/aero_override.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 gamma = 1.40  # cp/cv for air
 gamma1 = 0.2  # (gamma-1)/2 for air
 gamma2 = 3.5  # gamma/(gamma-1) for air
 beta = -0.0065  # [K/m] ISA temp gradient below tropopause
 r_earth = 6371000.0  # m, average earth radius
 a0 = 340.293988  # m/s, sea level speed of sound ISA, sqrt(gamma*R*T0)
 
+deg = 180 / 3.14159  # radians -> degrees
+rad = 3.14159 / 180  # degrees -> radians
+
 
 def atmos(h):
     """Compute press, density and temperature at a given altitude.
 
     Args:
         h (SX or MX): Altitude (in meters).
 
@@ -112,18 +115,18 @@
         h (SX or MX): Altitude (in meters). Defaults to 0.
 
     Returns:
         SX or MX: Distance (in meters).
 
     """
     # convert decimal degrees to radians
-    lat1 = np.radians(lat1)
-    lon1 = np.radians(lon1)
-    lat2 = np.radians(lat2)
-    lon2 = np.radians(lon2)
+    lat1 = lat1 * rad
+    lon1 = lon1 * rad
+    lat2 = lat2 * rad
+    lon2 = lon2 * rad
 
     # haversine formula
     dlon = lon2 - lon1
     dlat = lat2 - lat1
     a = np.sin(dlat / 2) ** 2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2) ** 2
     c = 2 * np.arcsin(np.sqrt(a))
     dist = c * (r_earth + h)  # meters, radius of earth
@@ -139,22 +142,22 @@
         lat2 (SX or MX): Ending latitude (in degrees).
         lon2 (SX or MX): Ending longitude (in degrees).
 
     Returns:
         SX or MX: Bearing (in degrees). Between 0 and 360.
 
     """
-    lat1 = np.radians(lat1)
-    lon1 = np.radians(lon1)
-    lat2 = np.radians(lat2)
-    lon2 = np.radians(lon2)
+    lat1 = lat1 * rad
+    lon1 = lon1 * rad
+    lat2 = lat2 * rad
+    lon2 = lon2 * rad
     x = np.sin(lon2 - lon1) * np.cos(lat2)
     y = np.cos(lat1) * np.sin(lat2) - np.sin(lat1) * np.cos(lat2) * np.cos(lon2 - lon1)
     initial_bearing = np.arctan2(x, y)
-    initial_bearing = np.degrees(initial_bearing)
+    initial_bearing = initial_bearing * deg
     bearing = (initial_bearing + 360) % 360
     return bearing
 
 
 def h_isa(p):
     """Compute ISA altitude for a given pressure.
 
@@ -191,29 +194,29 @@
 
     Returns:
         lat2: Point latitude.
         lon2: Point longitude
 
     """
     # convert decimal degrees to radians
-    lat1 = np.radians(lat1)
-    lon1 = np.radians(lon1)
-    brg = np.radians(brg)
+    lat1 = lat1 * rad
+    lon1 = lon1 * rad
+    brg = brg * rad
 
     # haversine formula
     lat2 = np.arcsin(
         np.sin(lat1) * np.cos(d / (r_earth + h))
         + np.cos(lat1) * np.sin(d / (r_earth + h)) * np.cos(brg)
     )
     lon2 = lon1 + np.arctan2(
         np.sin(brg) * np.sin(d / (r_earth + h)) * np.cos(lat1),
         np.cos(d / (r_earth + h)) - np.sin(lat1) * np.sin(lat2),
     )
-    lat2 = np.degrees(lat2)
-    lon2 = np.degrees(lon2)
+    lat2 = lat2 * deg
+    lon2 = lon2 * deg
     return lat2, lon2
 
 
 def tas2mach(v_tas, h):
     """Convert true airspeed to mach number at a given altitude.
 
     Args:
@@ -352,11 +355,11 @@
 
     Returns:
         SX or MX: Altitude (m).
 
     """
     mach = 1e-4 if mach < 1e-4 else mach
     delta = ((0.2 * (v_cas / a0) ** 2 + 1) ** 3.5 - 1) / (
-        (0.2 * mach ** 2 + 1) ** 3.5 - 1
+        (0.2 * mach**2 + 1) ** 3.5 - 1
     )
     h = T0 / beta * (delta ** (-1 * R * beta / g0) - 1)
     return h
```

### Comparing `openap-1.3/openap/data/.gitignore` & `openap-1.4/openap/data/.gitignore`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/LICENSE` & `openap-1.4/openap/data/LICENSE`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/aircraft/a19n.yml` & `openap-1.4/openap/data/aircraft/b37m.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-aircraft: Airbus A319neo
+aircraft: Boeing 737 MAX 7
+
+pax: 
+  max: 172
+  low: 138
+  high: 153
+
 
 fuselage:
-  length:   33.84
-  height:   4.14
-  width:    3.95
+  length:   33.6
+  height:   3.73
+  width:    3.73
 
 wing:
-  area:     124
-  span:     35.8
-  mac:      4.29
+  area:     124.6
+  span:     34.32
+  mac:      4.17
   sweep:    25
   t/c:      null
 
 flaps:
-  type:     single-slotted
-  area:     21.1
-  bf/b:     0.780
+  type:     double-slotted
+  area:     null
+  bf/b:     0.60
 
 limits:
-  MTOW:     75500
-  MLW:      62500
-  OEW:      42600
-  MFC:      29700
-  VMO:      350
+  MTOW:     80000
+  MLW:      60000
+  OEW:      45000
+  MFC:      26000
+  VMO:      340
   MMO:      0.82
   ceiling:  12500
 
 cruise:
   height:   11000
   mach:     0.78
 
 engine:
   type: turbofan
   mount: wing
   number: 2
-  default: PW1124G1-JM
+  default: LEAP-1B
   options:
-    A319-171N: PW1124G1-JM
-    A319-151N: LEAP-1A24
-    A319-153N: LEAP-1A26
+    - LEAP-1B
```

### Comparing `openap-1.3/openap/data/aircraft/a20n.yml` & `openap-1.4/openap/data/aircraft/a20n.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A320neo
 
+pax: 
+  max: 194
+  low: 150
+  high: 180
+
 fuselage:
   length:   37.57
   height:   4.14
   width:    3.95
 
 wing:
   area:     124
```

### Comparing `openap-1.3/openap/data/aircraft/a21n.yml` & `openap-1.4/openap/data/aircraft/a21n.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A321neo
 
+pax: 
+  max: 244
+  low: 180
+  high: 220
+
 fuselage:
   length:   44.51
   height:   4.14
   width:    3.95
 
 wing:
   area:     128
```

### Comparing `openap-1.3/openap/data/aircraft/a319.yml` & `openap-1.4/openap/data/aircraft/a319.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A319
 
+pax: 
+  max: 156
+  low: 110
+  high: 140
+
 fuselage:
   length:   33.84
   height:   4.14
   width:    3.95
 
 wing:
   area:     124
```

### Comparing `openap-1.3/openap/data/aircraft/a320.yml` & `openap-1.4/openap/data/aircraft/a320.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A320
 
+pax: 
+  max: 180
+  low: 140
+  high: 170
+
 fuselage:
   length:   37.57
   height:   4.14
   width:    3.95
 
 wing:
   area:     124
```

### Comparing `openap-1.3/openap/data/aircraft/a332.yml` & `openap-1.4/openap/data/aircraft/a332.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A330-200
 
+pax: 
+  max: 406
+  low: 220
+  high: 260
+
 fuselage:
   length:   58.82
   height:   5.64
   width:    5.64
 
 wing:
   area:     361.6
```

### Comparing `openap-1.3/openap/data/aircraft/a333.yml` & `openap-1.4/openap/data/aircraft/a333.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A330-300
 
+pax: 
+  max: 440
+  low: 250
+  high: 290
+
 fuselage:
   length:   63.67
   height:   5.64
   width:    5.64
 
 wing:
   area:     361.6
```

### Comparing `openap-1.3/openap/data/aircraft/a343.yml` & `openap-1.4/openap/data/aircraft/b773.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-aircraft: Airbus A340-300
+aircraft: Boeing 777-300
+
+pax: 
+  max: 550
+  low: 360
+  high: 400
 
 fuselage:
-  length:   63.69
-  height:   5.64
-  width:    5.64
+  length:   73.86
+  height:   6.20
+  width:    6.20
 
 wing:
-  area:     363.1
-  span:     60.3
-  mac:      7.26
-  sweep:    29.7
-  t/c:      0.11
+  area:     427.8
+  span:     60.93
+  mac:      8.75
+  sweep:    31.6
+  t/c:      null
 
 flaps:
   type:     double-slotted
-  area:     null
-  bf/b:     0.665
+  area:     67.13
+  bf/b:     0.758
 
 limits:
-  MTOW:     276000
-  MLW:      190000
-  OEW:      130000
-  MFC:      147850
+  MTOW:     299300
+  MLW:      237600
+  OEW:      160500
+  MFC:      171200
   VMO:      330
-  MMO:      0.86
-  ceiling:  12500
+  MMO:      0.89
+  ceiling:  13100
 
 cruise:
   height:   11000
-  mach:     0.82
+  mach:     0.84
 
 engine:
   type: turbofan
   mount: wing
-  number: 4
-  default: CFM56-5C3
+  number: 2
+  default: Trent 892
   options:
-    A340-311: CFM56-5C2
-    A340-312: CFM56-5C3
-    A340-313: CFM56-5C4
+    - GE90-110B1
+    - PW4090
+    - Trent 892
```

### Comparing `openap-1.3/openap/data/aircraft/a359.yml` & `openap-1.4/openap/data/aircraft/a359.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 aircraft: Airbus A350-900
 
+pax: 
+  max: 440
+  low: 300
+  high: 350
+
+
 fuselage:
   length:   66.8
   height:   6.09
   width:    5.96
 
 wing:
   area:     442
```

### Comparing `openap-1.3/openap/data/aircraft/a388.yml` & `openap-1.4/openap/data/aircraft/a388.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Airbus A380-800
 
+pax: 
+  max: 853
+  low: 410
+  high: 620
+
 fuselage:
   length:   72.72
   height:   8.41
   width:    7.14
 
 wing:
   area:     845
```

### Comparing `openap-1.3/openap/data/aircraft/b37m.yml` & `openap-1.4/openap/data/aircraft/b38m.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-aircraft: Boeing 737 MAX 7
+aircraft: Boeing 737 MAX 8
+
+pax: 
+  max: 210
+  low: 162
+  high: 178
 
 fuselage:
-  length:   33.6
+  length:   39.47
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
   span:     34.32
   mac:      4.17
@@ -14,26 +19,27 @@
 
 flaps:
   type:     double-slotted
   area:     null
   bf/b:     0.60
 
 limits:
-  MTOW:     80000
-  MLW:      60000
+  MTOW:     82000
+  MLW:      66300
   OEW:      45000
   MFC:      26000
   VMO:      340
   MMO:      0.82
   ceiling:  12500
 
 cruise:
   height:   11000
-  mach:     0.78
+  mach:     0.79
 
 engine:
   type: turbofan
   mount: wing
   number: 2
   default: LEAP-1B
   options:
-    - LEAP-1B
+    - LEAP-1B
+
```

### Comparing `openap-1.3/openap/data/aircraft/b38m.yml` & `openap-1.4/openap/data/aircraft/b3xm.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-aircraft: Boeing 737 MAX 8
+aircraft: Boeing 737 MAX 10
+
+pax: 
+  max: 230
+  low: 188
+  high: 204
+
 
 fuselage:
-  length:   39.47
+  length:   43.8
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
   span:     34.32
   mac:      4.17
@@ -14,16 +20,16 @@
 
 flaps:
   type:     double-slotted
   area:     null
   bf/b:     0.60
 
 limits:
-  MTOW:     82000
-  MLW:      66300
+  MTOW:     90000
+  MLW:      70000
   OEW:      45000
   MFC:      26000
   VMO:      340
   MMO:      0.82
   ceiling:  12500
 
 cruise:
@@ -33,8 +39,7 @@
 engine:
   type: turbofan
   mount: wing
   number: 2
   default: LEAP-1B
   options:
     - LEAP-1B
-
```

### Comparing `openap-1.3/openap/data/aircraft/b39m.yml` & `openap-1.4/openap/data/aircraft/b39m.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 737 MAX 9
 
+pax: 
+  max: 220
+  low: 178
+  high: 193
+
 fuselage:
   length:   42.11
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
```

### Comparing `openap-1.3/openap/data/aircraft/b3xm.yml` & `openap-1.4/openap/data/aircraft/b739.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-aircraft: Boeing 737 MAX 10
+aircraft: Boeing 737-900
+
+pax: 
+  max: 215
+  low: 170
+  high: 190
 
 fuselage:
-  length:   43.8
+  length:   42.11
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
   span:     34.32
   mac:      4.17
@@ -14,26 +19,28 @@
 
 flaps:
   type:     double-slotted
   area:     null
   bf/b:     0.60
 
 limits:
-  MTOW:     90000
-  MLW:      70000
-  OEW:      45000
+  MTOW:     85100
+  MLW:      71300
+  OEW:      44600
   MFC:      26000
   VMO:      340
   MMO:      0.82
   ceiling:  12500
 
 cruise:
   height:   11000
   mach:     0.79
 
 engine:
   type: turbofan
   mount: wing
   number: 2
-  default: LEAP-1B
+  default: CFM56-7B26
   options:
-    - LEAP-1B
+    - CFM56-7B24
+    - CFM56-7B26
+    - CFM56-7B27
```

### Comparing `openap-1.3/openap/data/aircraft/b734.yml` & `openap-1.4/openap/data/aircraft/c550.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-aircraft: Boeing 737-400
+aircraft: Cessna Citation II
+
+pax: 
+  max: 10
+  low: 5
+  high: 10
 
 fuselage:
-  length:   33.4
-  height:   3.73
-  width:    3.73
+  length:   14.39
+  height:   1.46
+  width:    1.46
 
 wing:
-  area:     91.04
-  span:     28.88
-  mac:      3.73
-  sweep:    25
-  t/c:      0.129
+  area:     31.83
+  span:     15.90
+  mac:      2.05
+  sweep:    0
+  t/c:      0.13
 
 flaps:
-  type:     triple-slotted
+  type:     single-slotted
   area:     null
-  bf/b:     0.72
+  bf/b:     null
 
 limits:
-  MTOW:     68000
-  MLW:      56200
-  OEW:      33700
-  MFC:      20000
-  VMO:      340
-  MMO:      0.82
-  ceiling:  12500
+  MTOW:     6849
+  MLW:      6804
+  OEW:      3655
+  MFC:      2204
+  VMO:      270
+  MMO:      0.7
+  ceiling:  13100
 
 cruise:
   height:   11000
-  mach:     0.78
+  mach:     0.67
 
 engine:
   type: turbofan
-  mount: wing
+  mount: rear
   number: 2
-  default: CFM56-3B-2
+  default: JT15D-4
   options:
-    - CFM56-3B-2
-    - CFM56-3C-1
+    - JT15D-4
```

### Comparing `openap-1.3/openap/data/aircraft/b737.yml` & `openap-1.4/openap/data/aircraft/b737.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 737-700
 
+pax: 
+  max: 149
+  low: 130
+  high: 149
+
 fuselage:
   length:   33.6
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
```

### Comparing `openap-1.3/openap/data/aircraft/b739.yml` & `openap-1.4/openap/data/aircraft/b738.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-aircraft: Boeing 737-900
+aircraft: Boeing 737-800
+
+pax: 
+  max: 189
+  low: 162
+  high: 189
 
 fuselage:
-  length:   42.11
+  length:   39.47
   height:   3.73
   width:    3.73
 
 wing:
   area:     124.6
   span:     34.32
   mac:      4.17
@@ -14,25 +19,25 @@
 
 flaps:
   type:     double-slotted
   area:     null
   bf/b:     0.60
 
 limits:
-  MTOW:     85100
-  MLW:      71300
-  OEW:      44600
+  MTOW:     79000
+  MLW:      66300
+  OEW:      41400
   MFC:      26000
   VMO:      340
   MMO:      0.82
   ceiling:  12500
 
 cruise:
   height:   11000
-  mach:     0.79
+  mach:     0.789
 
 engine:
   type: turbofan
   mount: wing
   number: 2
   default: CFM56-7B26
   options:
```

### Comparing `openap-1.3/openap/data/aircraft/b744.yml` & `openap-1.4/openap/data/aircraft/e145.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-aircraft: Boeing 747-400
+aircraft: Embraer ERJ145 (LR)
+
+pax: 
+  max: 50
+  low: 50
+  high: 50
 
 fuselage:
-  length:   70.66
-  height:   8.10
-  width:    6.50
+  length:   29.87
+  height:   2.28
+  width:    2.28
 
 wing:
-  area:     525.6
-  span:     64.4
-  mac:      9.68
-  sweep:    37.5
-  t/c:      0.094
+  area:     51.2
+  span:     20.04
+  mac:      3.19
+  sweep:    23
+  t/c:      null
 
 flaps:
-  type:     triple-slotted
-  area:     78.7
-  bf/b:     0.639
+  type:     double-slotted
+  area:     null
+  bf/b:     null
 
 limits:
-  MTOW:     396800
-  MLW:      260300
-  OEW:      182400
-  MFC:      203500
-  VMO:      365
-  MMO:      0.92
-  ceiling:  13700
+  MTOW:     22000
+  MLW:      19300
+  OEW:      12110
+  MFC:      5136
+  VMO:      320
+  MMO:      0.78
+  ceiling:  11300
 
 cruise:
   height:   11000
-  mach:     0.85
+  mach:     0.72
 
 engine:
   type: turbofan
   mount: wing
-  number: 4
-  default: CF6-80C2B1F
+  number: 2
+  default: AE3007A1
   options:
-    - PW4062
-    - CF6-80C2B1F
-    - RB211-524G
+    - AE3007A1
```

### Comparing `openap-1.3/openap/data/aircraft/b748.yml` & `openap-1.4/openap/data/aircraft/b748.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 747-8
 
+pax: 
+  max: 605
+  low: 460
+  high: 480
+
 fuselage:
   length:   76.3
   height:   7.10
   width:    6.50
 
 wing:
   area:     554
```

### Comparing `openap-1.3/openap/data/aircraft/b752.yml` & `openap-1.4/openap/data/aircraft/e75l.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-aircraft: Boeing 757-200
+aircraft: Embraer E175 (LR)
+
+pax: 
+  max: 88
+  low: 64
+  high: 78
 
 fuselage:
-  length:   47.3
-  height:   4.10
-  width:    4.10
+  length:   29.90
+  height:   3.35
+  width:    3.01
 
 wing:
-  area:     182.3
-  span:     38.0
-  mac:      5.64
-  sweep:    25
+  area:     72.72
+  span:     26.00
+  mac:      3.19
+  sweep:    23
   t/c:      null
 
 flaps:
   type:     double-slotted
-  area:     30.4
-  bf/b:     0.757
+  area:     null
+  bf/b:     null
 
 limits:
-  MTOW:     115600
-  MLW:      92200
-  OEW:      58400
-  MFC:      43500
-  VMO:      350
-  MMO:      0.86
-  ceiling:  12800
+  MTOW:     38790
+  MLW:      34000
+  OEW:      21890
+  MFC:      11625
+  VMO:      320
+  MMO:      0.82
+  ceiling:  12500
 
 cruise:
   height:   11000
-  mach:     0.8
+  mach:     0.75
 
 engine:
   type: turbofan
   mount: wing
   number: 2
-  default: RB211-535E4
+  default: CF34-8E6
   options:
-    - PW2037
-    - RB211-535E4
+    - CF34-8E5
+    - CF34-8E6
```

### Comparing `openap-1.3/openap/data/aircraft/b763.yml` & `openap-1.4/openap/data/aircraft/b763.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 767-300
 
+pax: 
+  max: 350
+  low: 210
+  high: 290
+
 fuselage:
   length:   54.94
   height:   5.03
   width:    5.03
 
 wing:
   area:     283.3
```

### Comparing `openap-1.3/openap/data/aircraft/b772.yml` & `openap-1.4/openap/data/aircraft/b772.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 777-200/200ER 
 
+pax: 
+  max: 440
+  low: 300
+  high: 320
+
 fuselage:
   length:   63.73
   height:   6.20
   width:    6.20
 
 wing:
   area:     427.8
```

### Comparing `openap-1.3/openap/data/aircraft/b773.yml` & `openap-1.4/openap/data/aircraft/b789.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,48 @@
-aircraft: Boeing 777-300
+aircraft: Boeing 787-9
+
+pax: 
+  max: 420
+  low: 260
+  high: 290
 
 fuselage:
-  length:   73.86
-  height:   6.20
-  width:    6.20
+  length:   62.81
+  height:   5.94
+  width:    5.77
 
 wing:
-  area:     427.8
-  span:     60.93
-  mac:      8.75
-  sweep:    31.6
-  t/c:      null
+  area:     377
+  span:     60.12
+  mac:      6.27
+  sweep:    32.2
+  t/c:      0.094
 
 flaps:
-  type:     double-slotted
-  area:     67.13
-  bf/b:     0.758
+  type:     single-slotted
+  area:     null
+  bf/b:     null
 
 limits:
-  MTOW:     299300
-  MLW:      237600
-  OEW:      160500
-  MFC:      171200
-  VMO:      330
-  MMO:      0.89
+  MTOW:     254000
+  MLW:      193000
+  OEW:      128000
+  MFC:      126400
+  VMO:      515
+  MMO:      0.90
   ceiling:  13100
 
 cruise:
   height:   11000
-  mach:     0.84
+  mach:     0.85
 
 engine:
   type: turbofan
   mount: wing
   number: 2
-  default: Trent 892
+  default: Trent 1000-K2
   options:
-    - GE90-110B1
-    - PW4090
-    - Trent 892
+    - GEnx-1B75
+    - GEnx-1B74
+    - Trent 1000-K2
+    - Trent 1000-J2
+    - Trent 1000-A2
```

### Comparing `openap-1.3/openap/data/aircraft/b77w.yml` & `openap-1.4/openap/data/aircraft/b77w.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 777-300ER
 
+pax: 
+  max: 550
+  low: 365
+  high: 451
+
 fuselage:
   length:   73.86
   height:   6.20
   width:    6.20
 
 wing:
   area:     436.8
```

### Comparing `openap-1.3/openap/data/aircraft/b788.yml` & `openap-1.4/openap/data/aircraft/b788.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Boeing 787-8
 
+pax: 
+  max: 380
+  low: 220
+  high: 250
+
 fuselage:
   length:   56.72
   height:   5.94
   width:    5.77
 
 wing:
   area:     377
```

### Comparing `openap-1.3/openap/data/aircraft/c550.yml` & `openap-1.4/openap/data/aircraft/glf6.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-aircraft: Cessna Citation II
+aircraft: Gulfstream G650 / 650ER
+
+pax: 
+  max: 18
+  low: 8
+  high: 18
 
 fuselage:
-  length:   14.39
-  height:   1.46
-  width:    1.46
+  length:   30.41
+  height:   7.82
+  width:    2.49
 
 wing:
-  area:     31.83
-  span:     15.90
-  mac:      2.05
-  sweep:    0
-  t/c:      0.13
+  area:     119.2
+  span:     30.36
+  mac:      4.76
+  sweep:    36
+  t/c:      0.1
 
 flaps:
   type:     single-slotted
   area:     null
   bf/b:     null
 
 limits:
-  MTOW:     6849
-  MLW:      6804
-  OEW:      3655
-  MFC:      2204
-  VMO:      270
-  MMO:      0.7
-  ceiling:  13100
+  MTOW:     45200
+  MLW:      37900
+  OEW:      24000
+  MFC:      21000
+  VMO:      null
+  MMO:      0.925
+  ceiling:  16000
+  range:    13000
 
 cruise:
-  height:   11000
-  mach:     0.67
+  height:   12000
+  mach:     0.85
 
 engine:
   type: turbofan
   mount: rear
   number: 2
-  default: JT15D-4
+  default: BR700-725A1-12
   options:
-    - JT15D-4
+    - BR700-725A1-12
```

### Comparing `openap-1.3/openap/data/aircraft/e145.yml` & `openap-1.4/openap/data/aircraft/b752.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-aircraft: Embraer ERJ145 (LR)
+aircraft: Boeing 757-200
+
+pax: 
+  max: 239
+  low: 200
+  high: 225
 
 fuselage:
-  length:   29.87
-  height:   2.28
-  width:    2.28
+  length:   47.3
+  height:   4.10
+  width:    4.10
 
 wing:
-  area:     51.2
-  span:     20.04
-  mac:      3.19
-  sweep:    23
+  area:     182.3
+  span:     38.0
+  mac:      5.64
+  sweep:    25
   t/c:      null
 
 flaps:
   type:     double-slotted
-  area:     null
-  bf/b:     null
+  area:     30.4
+  bf/b:     0.757
 
 limits:
-  MTOW:     22000
-  MLW:      19300
-  OEW:      12110
-  MFC:      5136
-  VMO:      320
-  MMO:      0.78
-  ceiling:  11300
+  MTOW:     115600
+  MLW:      92200
+  OEW:      58400
+  MFC:      43500
+  VMO:      350
+  MMO:      0.86
+  ceiling:  12800
 
 cruise:
   height:   11000
-  mach:     0.72
+  mach:     0.8
 
 engine:
   type: turbofan
   mount: wing
   number: 2
-  default: AE3007A1
+  default: RB211-535E4
   options:
-    - AE3007A1
+    - PW2037
+    - RB211-535E4
```

### Comparing `openap-1.3/openap/data/aircraft/e170.yml` & `openap-1.4/openap/data/aircraft/e170.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Embraer E170
 
+pax: 
+  max: 78
+  low: 60
+  high: 72
+
 fuselage:
   length:   29.90
   height:   3.35
   width:    3.01
 
 wing:
   area:     72.72
```

### Comparing `openap-1.3/openap/data/aircraft/e195.yml` & `openap-1.4/openap/data/aircraft/e195.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 aircraft: Embraer E195 (LR)
 
+pax: 
+  max: 124
+  low: 88
+  high: 116
+
 fuselage:
   length:   38.65
   height:   3.35
   width:    3.01
 
 wing:
   area:     92.5
```

### Comparing `openap-1.3/openap/data/engine/engines.csv` & `openap-1.4/openap/data/engine/engines.csv`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/nav/airports.csv` & `openap-1.4/openap/data/nav/airports.csv`

 * *Files 0% similar despite different names*

```diff
@@ -6468,14 +6468,15 @@
 OSDZ,35.2866,40.15288,700,SY,Deir Zzor,Deir ez-Zor
 OSKL,37.00795,41.17864,1480,SY,Kamishly,Al Qamishli
 OSLK,35.41388,35.94753,157,SY,Bassel Al Assad Intl,Jablah
 OSPR,34.55599,38.30125,1322,SY,Palmyra,Tadmur
 OTBD,25.28022,51.55653,35,QA,Doha Intl,Doha
 OTBH,25.13301,51.30804,130,QA,Al Udeid Ab,Ar Rayyan
 OTBK,25.63514,51.50162,10,QA,Al Khor,Al Khawr
+OTHH,25.25980,51.61430,13,QA,Doha Intl,Doha
 OYAA,12.82642,45.01475,7,YE,Aden Intl,Khawr Maksar
 OYAT,14.56044,46.81683,3735,YE,Ataq,Ataq
 OYBA,18.71225,50.82457,908,YE,Al Badie,Rumah
 OYBN,14.78947,45.71914,3800,YE,Beihan,Bayhan
 OYGD,16.19155,52.16074,134,YE,Al Ghaidah Intl,Al Ghayzah
 OYHD,14.74083,42.97014,41,YE,Hodeidah Intl,Al Hudaydah
 OYRN,14.65627,49.36273,54,YE,Mukalla Intl,Ghayl Ba Wazir
```

### Comparing `openap-1.3/openap/data/nav/fix.dat` & `openap-1.4/openap/data/nav/fix.dat`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/nav/nav.dat` & `openap-1.4/openap/data/nav/nav.dat`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a319.txt` & `openap-1.4/openap/data/wrap/a319.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a320.txt` & `openap-1.4/openap/data/wrap/a320.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a321.txt` & `openap-1.4/openap/data/wrap/a321.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a332.txt` & `openap-1.4/openap/data/wrap/a332.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a333.txt` & `openap-1.4/openap/data/wrap/a333.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a343.txt` & `openap-1.4/openap/data/wrap/a343.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/a388.txt` & `openap-1.4/openap/data/wrap/a388.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b737.txt` & `openap-1.4/openap/data/wrap/b737.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b738.txt` & `openap-1.4/openap/data/wrap/b738.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b739.txt` & `openap-1.4/openap/data/wrap/b739.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b744.txt` & `openap-1.4/openap/data/wrap/b744.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b752.txt` & `openap-1.4/openap/data/wrap/b752.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b763.txt` & `openap-1.4/openap/data/wrap/b763.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b77w.txt` & `openap-1.4/openap/data/wrap/b77w.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b788.txt` & `openap-1.4/openap/data/wrap/b788.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/b789.txt` & `openap-1.4/openap/data/wrap/b789.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/data/wrap/e190.txt` & `openap-1.4/openap/data/wrap/e190.txt`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/drag.py` & `openap-1.4/openap/drag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """OpenAP drag model."""
 
-import os
+import glob
 import importlib
+import os
+import warnings
+
 import pandas as pd
-import glob
 import yaml
-import math
-import warnings
+
 from . import prop
 from .extra import ndarrayconvert
 
-
 curr_path = os.path.dirname(os.path.realpath(__file__))
 dir_dragpolar = curr_path + "/data/dragpolar/"
 file_synonym = curr_path + "/data/dragpolar/_synonym.csv"
 
 polar_synonym = pd.read_csv(file_synonym)
 
 
@@ -65,42 +65,41 @@
                 raise RuntimeError(f"Drag polar for {self.ac} not avaiable in OpenAP.")
 
         f = dir_dragpolar + ac + ".yml"
         dragpolar = yaml.safe_load(open(f))
         return dragpolar
 
     @ndarrayconvert
-    def _cl(self, mass, tas, alt, path_angle):
+    def _cl(self, mass, tas, alt):
         v = tas * self.aero.kts
         h = alt * self.aero.ft
-        gamma = path_angle * self.np.pi / 180
 
         S = self.aircraft["wing"]["area"]
 
         rho = self.aero.density(h)
-        qS = 0.5 * rho * v ** 2 * S
-        L = mass * self.aero.g0 * self.np.cos(gamma)
+        qS = 0.5 * rho * v**2 * S
+        L = mass * self.aero.g0
         qS = self.np.where(qS < 1e-3, 1e-3, qS)
         cl = L / qS
         return cl
 
     @ndarrayconvert
     def _calc_drag(self, mass, tas, alt, cd0, k, path_angle):
         v = tas * self.aero.kts
         h = alt * self.aero.ft
         gamma = path_angle * self.np.pi / 180
 
         S = self.aircraft["wing"]["area"]
 
         rho = self.aero.density(h)
-        qS = 0.5 * rho * v ** 2 * S
+        qS = 0.5 * rho * v**2 * S
         L = mass * self.aero.g0 * self.np.cos(gamma)
         qS = self.np.where(qS < 1e-3, 1e-3, qS)
         cl = L / qS
-        cd = cd0 + k * cl ** 2
+        cd = cd0 + k * cl**2
         D = cd * qS
         return D
 
     @ndarrayconvert
     def clean(self, mass, tas, alt, path_angle=0):
         """Compute drag at clean configuration (considering compressibility).
 
@@ -116,29 +115,32 @@
         """
 
         cd0 = self.polar["clean"]["cd0"]
         k = self.polar["clean"]["k"]
 
         if self.wave_drag:
             mach = self.aero.tas2mach(tas * self.aero.kts, alt * self.aero.ft)
-            cl = self._cl(mass, tas, alt, path_angle)
+            cl = self._cl(mass, tas, alt)
 
-            sweep = math.radians(self.aircraft["wing"]["sweep"])
+            sweep = self.np.radians(self.aircraft["wing"]["sweep"])
             tc = self.aircraft["wing"]["t/c"]
             if tc is None:
-                tc = 0.11
+                tc = 0.12
+
+            cos_sweep = self.np.cos(sweep)
+
+            kappa = 0.95  # assume supercritical airfoils
 
-            cos_sweep = math.cos(sweep)
             mach_crit = (
-                0.87 - 0.108 / cos_sweep - 0.1 * cl / (cos_sweep ** 2) - tc / cos_sweep
-            ) / cos_sweep
+                kappa / cos_sweep - tc / cos_sweep**2 - 0.1 * cl / cos_sweep**3 - 0.108
+            )
 
-            dmach = self.np.where(mach - mach_crit <= 0, 0, mach - mach_crit)
+            dmach = mach - mach_crit
 
-            dCdw = self.np.where(dmach, 20 * dmach ** 4, 0)
+            dCdw = self.np.where(dmach > 0, 20 * dmach**4, 0)
 
         else:
             dCdw = 0
 
         cd0 = cd0 + dCdw
 
         D = self._calc_drag(mass, tas, alt, cd0, k, path_angle)
```

### Comparing `openap-1.3/openap/emission.py` & `openap-1.4/openap/emission.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/extra/__init__.py` & `openap-1.4/openap/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/extra/aero.py` & `openap-1.4/openap/extra/aero.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,13 +370,13 @@
         v_cas (float or ndarray): Calibrated airspeed (m/s).
         mach (float or ndarray): Mach number.
 
     Returns:
         float or ndarray: Altitude (m).
 
     """
-    mach = 1e-4 if mach < 1e-4 else mach
+    mach = np.where(mach < 1e-4, 1e-4, mach)
     delta = ((0.2 * (v_cas / a0) ** 2 + 1) ** 3.5 - 1) / (
-        (0.2 * mach ** 2 + 1) ** 3.5 - 1
+        (0.2 * mach**2 + 1) ** 3.5 - 1
     )
     h = T0 / beta * (delta ** (-1 * R * beta / g0) - 1)
     return h
```

### Comparing `openap-1.3/openap/extra/filters.py` & `openap-1.4/openap/extra/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from matplotlib import pyplot as plt
 import numpy as np
-from scipy.signal import gaussian
-from scipy.ndimage import filters
+from matplotlib import pyplot as plt
 from scipy.interpolate import UnivariateSpline
+from scipy.ndimage import filters
+from scipy.signal.windows import gaussian
 
 
 class BaseFilter(object):
     def __init__(self, i=False):
         self.interpolate = i
 
     def sortxy(self, X, Y):
         XY = list(zip(X, Y))
         XY.sort(key=lambda t: t[0])
         X1, Y1 = list(zip(*XY))
         return np.array(X1), np.array(Y1)
 
     def simplefill(self, X, Y):
-        ''' Fill the missing data with closest previous data each second '''
+        """Fill the missing data with closest previous data each second"""
 
         X, Y = self.sortxy(X, Y)
 
         X = np.array(X)
         Y = np.array(Y)
 
-        Xfull = list(range(int(X[0]), int(X[-1]+1)))
+        Xfull = list(range(int(X[0]), int(X[-1] + 1)))
         Yfull = []
 
         y = 0
         for x in Xfull:
             try:
                 i = np.where(X == x)[0][0]
                 y = Y[i]
@@ -35,17 +35,16 @@
                 pass
 
             Yfull.append(y)
 
         return np.array(Xfull), np.array(Yfull)
 
     def filterplot(self, x, y, xf, yf):
-        plt.plot(x, y, '.', color='blue', alpha=0.5)
-        plt.plot(xf, yf, '-', color='red')
-
+        plt.plot(x, y, ".", color="blue", alpha=0.5)
+        plt.plot(xf, yf, "-", color="red")
 
 
 class SavitzkyGolay(BaseFilter):
     """
     SavitzkyGolay Filter
 
     Parameters
@@ -56,14 +55,15 @@
         the order of the polynomial used in the filtering.
         Must be less then `window_size` - 1.
     deriv: int
         the order of the derivative to compute (default = 0
         means only smoothing)
 
     """
+
     def __init__(self, window_size=11, order=2, deriv=0, i=False):
         super(SavitzkyGolay, self).__init__(i=i)
 
         try:
             window_size = np.abs(np.int(window_size))
             order = np.abs(np.int(order))
         except ValueError:
@@ -79,56 +79,58 @@
 
     def filter(self, X, Y):
         if self.interpolate:
             X, Y = self.simplefill(X, Y)
         else:
             X, Y = self.sortxy(X, Y)
 
-        order_range = list(range(self.order+1))
+        order_range = list(range(self.order + 1))
         half_window = (self.window_size - 1) // 2
         # precompute coefficients
-        b = np.mat([[k**i for i in order_range]
-                    for k in range(-half_window, half_window+1)])
+        b = np.mat(
+            [[k**i for i in order_range] for k in range(-half_window, half_window + 1)]
+        )
         m = np.linalg.pinv(b).A[self.deriv]
         # pad the signal at the extremes with
         # values taken from the signal itself
-        firstvals = Y[0] - np.abs(Y[1:half_window+1][::-1] - Y[0])
-        lastvals = Y[-1] + np.abs(Y[-half_window-1:-1][::-1] - Y[-1])
+        firstvals = Y[0] - np.abs(Y[1 : half_window + 1][::-1] - Y[0])
+        lastvals = Y[-1] + np.abs(Y[-half_window - 1 : -1][::-1] - Y[-1])
         Y1 = np.concatenate((firstvals, Y, lastvals))
-        Y2 = np.convolve(m, Y1, mode='valid')
+        Y2 = np.convolve(m, Y1, mode="valid")
 
         return X, Y2
 
 
 class Spline(BaseFilter):
     """
     Spline smoothing
 
     """
+
     def __init__(self, k=1, i=False):
         super(Spline, self).__init__(i=i)
         self.k = k
 
     def kernel(self, series, sigma=3):
         # fix the weight of data
         # http://www.nehalemlabs.net/prototype/blog/2014/04/12/
         #    how-to-fix-scipys-interpolating-spline-default-behavior/
         series = np.asarray(series)
         b = gaussian(25, sigma)
-        averages = filters.convolve1d(series, b/b.sum())
-        variances = filters.convolve1d(np.power(series-averages, 2), b/b.sum())
+        averages = filters.convolve1d(series, b / b.sum())
+        variances = filters.convolve1d(np.power(series - averages, 2), b / b.sum())
         variances[variances == 0] = 1
         return averages, variances
 
     def filter(self, X, Y):
         X, Y = self.sortxy(X, Y)
 
         # using gaussian kernel to get a better variances
         avg, var = self.kernel(Y)
-        spl = UnivariateSpline(X, Y, k=self.k, w=1/np.sqrt(var))
+        spl = UnivariateSpline(X, Y, k=self.k, w=1 / np.sqrt(var))
 
         if self.interpolate:
             xmax = X[-1]
             Xfull = np.arange(xmax)
             Yfull = spl(Xfull)
             return Xfull, Yfull
         else:
@@ -137,30 +139,32 @@
 
 
 class TWF(BaseFilter):
     """
     Time-based weighted filter
     input X is the time stamps of Y
     """
+
     def __init__(self, window_size=10):
         super(TWF, self).__init__()
         self.window_size = window_size
 
     def filter(self, X, Y):
         X, Y = self.sortxy(X, Y)
 
         YF = np.zeros(Y.shape)
         YF[0] = Y[0]
         YF[1] = Y[1]
 
         for i in range(2, len(X)):
             if i < self.window_size:
-                y = (np.average(YF[:i-1]) + Y[i]) / 2.0
+                y = (np.average(YF[: i - 1]) + Y[i]) / 2.0
             else:
-                Xwin = X[i-self.window_size: i-1][::-1]
-                Ywin = YF[i-self.window_size: i-1][::-1]
+                Xwin = X[i - self.window_size : i - 1][::-1]
+                Ywin = YF[i - self.window_size : i - 1][::-1]
                 dXwin = Xwin[1:] - Xwin[:-1]
-                yw = (Ywin[0] + np.sum(1./dXwin * Ywin[1:])) / \
-                     (1 + np.sum(1.0/dXwin))
+                yw = (Ywin[0] + np.sum(1.0 / dXwin * Ywin[1:])) / (
+                    1 + np.sum(1.0 / dXwin)
+                )
                 y = (yw + Y[i]) / 2.0
             YF[i] = y
         return X, np.array(YF)
```

### Comparing `openap-1.3/openap/extra/nav.py` & `openap-1.4/openap/extra/nav.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 from openap.extra import aero
 
 fixes = None
 airports = None
 
 curr_path = os.path.dirname(os.path.realpath(__file__))
 db_airport = curr_path + "/../data/nav/airports.csv"
-db_fix = curr_path + '/../data/nav/fix.dat'
+db_fix = curr_path + "/../data/nav/fix.dat"
 
 
 def _read_fix():
     return pd.read_csv(
-        db_fix, skiprows=3, skipfooter=1,
-        engine='python',
-        sep=r'\s+',
-        names=('lat', 'lon', 'fix')
+        db_fix,
+        skiprows=3,
+        skipfooter=1,
+        engine="python",
+        sep=r"\s+",
+        names=("lat", "lon", "fix"),
+        encoding="unicode_escape",
     )
 
 
 def _read_airport():
     return pd.read_csv(db_airport)
 
 
@@ -38,15 +41,15 @@
 
     """
     NAME = str(name).upper()
 
     if not isinstance(airport, pd.DataFrame):
         airports = _read_airport()
 
-    df = airports[airports['icao']==NAME]
+    df = airports[airports["icao"] == NAME]
     if df.shape[0] == 0:
         return None
     else:
         return df.iloc[0, :].to_dict()
 
 
 def closest_airport(lat, lon):
@@ -61,21 +64,24 @@
 
     """
     global airports
 
     if not isinstance(airport, pd.DataFrame):
         airports = _read_airport()
 
-    df = airports[airports['lat'].between(lat-2, lat+2) & airports['lon'].between(lon-2, lon+2)]
+    df = airports[
+        airports["lat"].between(lat - 2, lat + 2)
+        & airports["lon"].between(lon - 2, lon + 2)
+    ]
 
     if df.shape[0] == 0:
         return None
 
-    coords = np.array(df[['lat', 'lon']])
-    dist2 = np.sum((coords - [lat, lon])**2, axis=1)
+    coords = np.array(df[["lat", "lon"]])
+    dist2 = np.sum((coords - [lat, lon]) ** 2, axis=1)
     idx = np.argmin(dist2)
 
     ap = df.iloc[idx, :]
 
     return ap.icao
 
 
@@ -91,15 +97,15 @@
     """
     global fixes
 
     if not isinstance(fixes, pd.DataFrame):
         fixes = _read_fix()
 
     NAME = str(name).upper()
-    fix = fixes[fixes['fix']==NAME].iloc[0].tolist()
+    fix = fixes[fixes["fix"] == NAME].iloc[0].tolist()
     return fix
 
 
 def closest_fix(lat, lon):
     """Get the closest fix of a location.
 
     Args:
@@ -112,19 +118,21 @@
 
     """
     global fixes
 
     if not isinstance(fixes, pd.DataFrame):
         fixes = _read_fix()
 
-    mask = (fixes['lat'].between(lat-1, lat+1)) & (fixes['lon'].between(lon-1, lon+1))
+    mask = (fixes["lat"].between(lat - 1, lat + 1)) & (
+        fixes["lon"].between(lon - 1, lon + 1)
+    )
     chunk = fixes[mask]
 
-    lats = np.asarray(chunk['lat'])
-    lons = np.asarray(chunk['lon'])
+    lats = np.asarray(chunk["lat"])
+    lons = np.asarray(chunk["lon"])
 
     distances = aero.distance(lat, lon, lats, lons)
     idx = distances.argmin()
 
     fix = chunk.iloc[idx].tolist()
     dist = distances[idx]
```

### Comparing `openap-1.3/openap/extra/statistics.py` & `openap-1.4/openap/extra/statistics.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/fuel.py` & `openap-1.4/openap/fuel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """OpenAP FuelFlow model."""
 
 import importlib
+
 from openap import prop
 from openap.extra import ndarrayconvert
 
 
 def func_fuel2(a, b):
     return lambda x: a * (x + b) ** 2
 
 
 def func_fuel3(c3, c2, c1):
-    return lambda x: c3 * x ** 3 + c2 * x ** 2 + c1 * x
+    return lambda x: c3 * x**3 + c2 * x**2 + c1 * x
 
 
 class FuelFlow(object):
     """Fuel flow model based on ICAO emission databank."""
 
     def __init__(self, ac, eng=None, **kwargs):
         """Initialize FuelFlow object.
```

### Comparing `openap-1.3/openap/kinematic.py` & `openap-1.4/openap/kinematic.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/phase.py` & `openap-1.4/openap/phase.py`

 * *Files identical despite different names*

### Comparing `openap-1.3/openap/prop.py` & `openap-1.4/openap/prop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Retrive properties of aircraft and engines."""
 
 import os
 import glob
 import yaml
 import numpy as np
 import pandas as pd
+from functools import lru_cache
 
 curr_path = os.path.dirname(os.path.realpath(__file__))
 dir_aircraft = curr_path + "/data/aircraft/"
 file_engine = curr_path + "/data/engine/engines.csv"
 file_synonym = curr_path + "/data/aircraft/_synonym.csv"
 
 aircraft_synonym = pd.read_csv(file_synonym)
 
 
+@lru_cache()
 def available_aircraft(use_synonym=False):
     """Get available aircraft types in OpenAP model.
 
     Returns:
         list of string: aircraft types.
 
     """
@@ -55,14 +57,15 @@
 
     f = files[0]
     acdict = yaml.safe_load(open(f))
 
     return acdict
 
 
+@lru_cache()
 def aircraft_engine_options(ac):
     """Get engine options of an aircraft type.
 
     Args:
         ac (string): ICAO aircraft type (for example: A320).
 
     Returns:
@@ -75,14 +78,15 @@
         eng_options = list(acdict["engine"]["options"].values())
     elif type(acdict["engine"]["options"]) == list:
         eng_options = list(acdict["engine"]["options"])
 
     return eng_options
 
 
+@lru_cache()
 def search_engine(eng):
     """Search engine by the starting characters.
 
     Args:
         eng (string): Engine type (for example: CFM56-5).
 
     Returns:
@@ -101,14 +105,15 @@
         print("Engines found:")
         result = available_engines.name.tolist()
         print(result)
 
     return result
 
 
+@lru_cache()
 def engine(eng):
     """Get engine parameters.
 
     Args:
         eng (string): Engine type (for example: CFM56-5B6).
 
     Returns:
```

### Comparing `openap-1.3/openap/thrust.py` & `openap-1.4/openap/thrust.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Models for Modern Two-Shaft Turbonfan Engines
 
     - C. Svoboda, Turbofan engine database as a preliminary desgin (cruise thrust)
 
 """
 
 import importlib
+
 from openap import prop
 from openap.extra import ndarrayconvert
 
 
 class Thrust(object):
     """Simplified two-shaft turbonfan model."""
 
@@ -28,25 +29,27 @@
         if not hasattr(self, "np"):
             self.np = importlib.import_module("numpy")
 
         if not hasattr(self, "aero"):
             self.aero = importlib.import_module("openap").aero
 
         aircraft = prop.aircraft(ac, **kwargs)
+        force_engine = kwargs.get("force_engine", False)
 
         if eng is None:
             eng = aircraft["engine"]["default"]
 
         engine = prop.engine(eng)
 
-        if type(aircraft["engine"]["options"]) == dict:
+        eng_options = aircraft["engine"]["options"]
+
+        if isinstance(eng_options, dict):
             eng_options = list(aircraft["engine"]["options"].values())
-        elif type(aircraft["engine"]["options"]) == list:
-            eng_options = list(aircraft["engine"]["options"])
-        if engine["name"] not in eng_options:
+
+        if (not force_engine) and (engine["name"] not in eng_options):
             raise RuntimeError(
                 f"Engine {eng} and aircraft {ac} mismatch. Available engines for {ac} are {eng_options}"
             )
 
         self.cruise_alt = aircraft["cruise"]["height"] / self.aero.ft
         # self.cruise_alt = 30000
         self.eng_bpr = engine["bpr"]
@@ -66,15 +69,15 @@
 
     def _nfunc(self, roc):
         # n = self.np.where(roc<1500, 0.89, self.np.where(roc<2500, 0.93, 0.97))
         n = 2.667e-05 * roc + 0.8633
         return n
 
     def _mfunc(self, vratio, roc):
-        m = -1.2043e-1 * vratio - 8.8889e-9 * roc ** 2 + 2.4444e-5 * roc + 4.7379e-1
+        m = -1.2043e-1 * vratio - 8.8889e-9 * roc**2 + 2.4444e-5 * roc + 4.7379e-1
         return m
 
     @ndarrayconvert
     def takeoff(self, tas, alt=None):
         """Calculate thrust at takeoff condition.
 
         Args:
@@ -91,34 +94,34 @@
         G0 = 0.0606 * self.eng_bpr + 0.6337
 
         if alt is None:
             # at sea level
             ratio = (
                 1
                 - 0.377 * (1 + eng_bpr) / self.np.sqrt((1 + 0.82 * eng_bpr) * G0) * mach
-                + (0.23 + 0.19 * self.np.sqrt(eng_bpr)) * mach ** 2
+                + (0.23 + 0.19 * self.np.sqrt(eng_bpr)) * mach**2
             )
 
         else:
             # at certain altitude
             P = self.aero.pressure(alt * self.aero.ft)
             dP = P / self.aero.p0
 
-            A = -0.4327 * dP ** 2 + 1.3855 * dP + 0.0472
-            Z = 0.9106 * dP ** 3 - 1.7736 * dP ** 2 + 1.8697 * dP
-            X = 0.1377 * dP ** 3 - 0.4374 * dP ** 2 + 1.3003 * dP
+            A = -0.4327 * dP**2 + 1.3855 * dP + 0.0472
+            Z = 0.9106 * dP**3 - 1.7736 * dP**2 + 1.8697 * dP
+            X = 0.1377 * dP**3 - 0.4374 * dP**2 + 1.3003 * dP
 
             ratio = (
                 A
                 - 0.377
                 * (1 + eng_bpr)
                 / self.np.sqrt((1 + 0.82 * eng_bpr) * G0)
                 * Z
                 * mach
-                + (0.23 + 0.19 * self.np.sqrt(eng_bpr)) * X * mach ** 2
+                + (0.23 + 0.19 * self.np.sqrt(eng_bpr)) * X * mach**2
             )
 
         F = ratio * self.eng_max_thrust * self.eng_number
         return F
 
     @ndarrayconvert
     def cruise(self, tas, alt):
```

### Comparing `openap-1.3/openap/traj/gen.py` & `openap-1.4/openap/traj/gen.py`

 * *Files identical despite different names*

