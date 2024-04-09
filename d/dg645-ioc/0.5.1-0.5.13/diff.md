# Comparing `tmp/dg645-ioc-0.5.1.tar.gz` & `tmp/dg645-ioc-0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg645-ioc-0.5.1.tar", last modified: Wed Apr  3 13:47:59 2024, max compression
+gzip compressed data, was "dg645-ioc-0.5.13.tar", last modified: Tue Apr  9 12:25:46 2024, max compression
```

## Comparing `dg645-ioc-0.5.1.tar` & `dg645-ioc-0.5.13.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/
--rw-r--r--   0 florin    (1000) florin    (1000)      143 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3752 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      604 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/Dockerfile
--rw-r--r--   0 florin    (1000) florin    (1000)    35147 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     6654 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     5543 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/README.md
--rw-r--r--   0 florin    (1000) florin    (1000)     1551 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)       38 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.225640 dg645-ioc-0.5.1/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     6654 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      558 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       47 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/entry_points.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       88 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        7 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/src/kronos/
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/kronos/_version.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2559 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/application.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1221 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/application.py~
--rw-r--r--   0 florin    (1000) florin    (1000)    11290 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/channel.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4806 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/flags.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5386 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/flags.py~
--rw-r--r--   0 florin    (1000) florin    (1000)     3105 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19510 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/ioc.py~
--rw-r--r--   0 florin    (1000) florin    (1000)     1051 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/main.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/test/
--rw-r--r--   0 florin    (1000) florin    (1000)     1345 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/test_dg645.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2000 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/test_ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7630 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/visa-sim-dg645.yml
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:25:46.095544 dg645-ioc-0.5.13/
+-rw-r--r--   0 florin    (1000) florin    (1000)      143 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     4121 2024-04-03 20:51:56.000000 dg645-ioc-0.5.13/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      604 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/Dockerfile
+-rw-r--r--   0 florin    (1000) florin    (1000)    35147 2024-03-30 22:30:28.000000 dg645-ioc-0.5.13/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     6816 2024-04-09 12:25:46.095544 dg645-ioc-0.5.13/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     5704 2024-04-03 19:44:42.000000 dg645-ioc-0.5.13/README.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     1551 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)       38 2024-04-09 12:25:46.095544 dg645-ioc-0.5.13/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:25:46.090544 dg645-ioc-0.5.13/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:25:46.094544 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     6816 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      491 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       47 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/entry_points.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       88 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        7 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/dg645_ioc.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:25:46.094544 dg645-ioc-0.5.13/src/kronos/
+-rw-r--r--   0 florin    (1000) florin    (1000)      413 2024-04-09 12:25:46.000000 dg645-ioc-0.5.13/src/kronos/_version.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2559 2024-03-30 22:30:28.000000 dg645-ioc-0.5.13/src/kronos/application.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11290 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/src/kronos/channel.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4806 2024-03-30 22:30:28.000000 dg645-ioc-0.5.13/src/kronos/flags.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     3105 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/src/kronos/ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1051 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/src/kronos/main.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 12:25:46.094544 dg645-ioc-0.5.13/test/
+-rw-r--r--   0 florin    (1000) florin    (1000)     1345 2024-03-30 22:30:28.000000 dg645-ioc-0.5.13/test/test_dg645.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2000 2024-04-03 18:49:13.000000 dg645-ioc-0.5.13/test/test_ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7630 2024-03-30 22:30:28.000000 dg645-ioc-0.5.13/test/visa-sim-dg645.yml
```

### Comparing `dg645-ioc-0.5.1/.gitlab-ci.yml` & `dg645-ioc-0.5.13/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     KRONOS_SIM: "yes"
   script:
     - export
     - id
     - pwd
     - ls -l /home
     - git config --global --add safe.directory /builds/kmc3-xpp/kronos-ioc
-    - if git describe --tags --exact-match --match v[0-9]\*; then 
+    - if git describe --tags --exact-match --match v[0-9]\*; then
     -   git describe --tags --exact-match --match v[0-9]\*
     -   export KRONOS_DESCRIBE=`git describe --tags --exact-match --match v[0-9]\*`
     -   echo -n "" > kronos.env
     -   export KRONOS_VERSION=${KRONOS_DESCRIBE##v}
     -   echo "KRONOS_VERSION=$KRONOS_VERSION" >> kronos.env
     -   echo "KRONOS_FAMILY=${KRONOS_VERSION%.*}" >> kronos.env
     -   echo "KRONOS_COMMIT=$CI_COMMIT_SHA" >> kronos.env
@@ -80,15 +80,15 @@
     -   export RELEASE_VERSION=$KRONOS_VERSION
     -   export RELEASE_FAMILY=$KRONOS_FAMILY
     -   export RELEASE_COMMIT=$KRONOS_COMMIT
     - elif [ ! -z "$CI_COMMIT_TAG" ]; then
     -   export RELEASE_VERSION=${CI_COMMIT_TAG##v}
     -   export RELEASE_FAMILY=${RELEASE_VERSION%.*}
     -   export RELAASE_COMMIT=$CI_COMMIT_SHA
-    - fi    
+    - fi
     - echo Kronos release version is $RELEASE_VERSION from commit $CI_COMMIT_SHA
     - if [ ! -z "$RELEASE_VERSION" ]; then
     -   echo "FROM $CI_REGISTRY_IMAGE:$CI_COMMIT_BRANCH" | /kaniko/executor --dockerfile /dev/stdin --destination "$CI_REGISTRY_IMAGE:latest" --destination "$CI_REGISTRY_IMAGE:$RELEASE_VERSION" --destination "$CI_REGISTRY_IMAGE:$RELEASE_FAMILY"
     - else
     -   echo "Cannot determine release tag."
     - fi
 
@@ -104,12 +104,21 @@
     -   export RELEASE_VERSION=$KRONOS_VERSION
     -   export RELEASE_FAMILY=$KRONOS_FAMILY
     - elif [ ! -z "$CI_COMMIT_TAG" ]; then
     -   export RELEASE_VERSION="${CI_COMMIT_TAG##v}"
     -   export RELEASE_FAMILY="${RELEASE_VERSION%.*}"
     - fi
     - echo Kronos release version is "$RELEASE_VERSION"
-    - if [ ! -z "$KRONOS_VERSION" ]; then
-    -   release-cli create --name "v$RELEASE_VERSION" --tag-name "v$RELEASE_VERSION" --description "v$RELEASE_VERSION, $RELEASE_FAMILY family -- $CI_COMMIT_DESCRIPTION"
-    - else
+    - if [ -z "$RELEASE_VERSION" ]; then
     -   echo "Cannot determine release tag, no release created."
+    -   "/bin/false"
     - fi
+    - echo "Releasing version $RELEASE_VERSION"
+    - echo -e "Description follows\n$CI_COMMIT_TITLE\n$CI_COMMIT_DESCRIPTION"
+    - |
+      release-cli create \
+          --name "Release v$RELEASE_VERSION" \
+          --tag-name "v$RELEASE_VERSION" \
+          --tag-message "t.m. $CI_COMMIT_TITLE" \
+          --description "$CI_COMMIT_TITLE" \
+          --ref "$CI_COMMIT_SHA" \
+          --assets-link "{\"name\":\"Source code tarball\",\"url\":\"$CI_PROJECT_URL/-/archive/v$RELEASE_VERSION/kronos-ioc-v$RELEASE_VERSION.tar.gz\"}"
```

### Comparing `dg645-ioc-0.5.1/Dockerfile` & `dg645-ioc-0.5.13/Dockerfile`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/LICENSE` & `dg645-ioc-0.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/PKG-INFO` & `dg645-ioc-0.5.13/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dg645-ioc
-Version: 0.5.1
+Version: 0.5.13
 Summary: CAproto-based pure-Python EPICS IOC for the Stanford Research Systems DG645 delay generator.
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source, https://gitlab.com/kmc3-xpp/kronos-ioc
 Project-URL: Issues, https://gitlab.com/kmc3-xpp/kronos-ioc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
@@ -32,52 +32,56 @@
 ![pipeline](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/pipeline.svg)
 ![coverage](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/coverage.svg)
 
 
 Quickstart
 ----------
 
-### Obtaining
+### In a System Shell
+
+#### Obtaining
 
 Download via PyPI: `pip install dg645-ioc` or via GitLab:
 
    ```
    git clone https://gitlab.com/kmc3-xpp/kronos-ioc
    ```
 
-### Running from the command line
+#### Running from the command line
 
 Configure at least the IP address and the EPICS prefix and start via shell:
 
    ```
    $ export DG645_EPICS_PREFIX="BEAMLINE:DG645:"
    $ export DG645_HOST="10.0.0.17"
    $ dg645-ioc
    INFO:kronos.ioc:Stanford Research Systems,DG645,s/n001776,ver1.14.10E
    INFO:root:Starting IOC, PV list following
    [...]
    INFO:caproto.ctx:Server startup complete.
    ```
-   
-### Obtaining a Container
+
+### In a Container
+
+#### Obtaining a Container
 
 
 You can download the automatically generated container:
 
    ```
    podman pull registry.gitlab.com/kmc3-xpp/kronos-ioc:latest
    ```
 
 ...or create your own, assuming  you've downloaded the sources into `./kronos-ioc`:
 
    ```
    $ podman build -t kronos-ioc -f kronos-ioc/Dockerfile -v $PWD/kronos-ioc:/kronos_src:z
    ```
 
-### Running in Podman / Docker
+#### Running in Podman / Docker
 
 Start as a Podman container (Docker should work the same, just replace thed
 `podman` command by `docker`):
 
    ```
    $ podman run -ti --rm \
        --env DG645_EPICS_PREFIX="BEAMLINE:DG645:" \
@@ -100,101 +104,102 @@
    ```
 
 Configuration
 -------------
 
  Here's a list of environment variables that might help:
  
-  - `DG645_HOST`: host name or IP of the DG645 controller
+- `DG645_HOST`: host name or IP of the DG645 controller
   
-  - `DG645_PORT`: this is better left blank (the default). In that
-    case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
-	name. If the port is specified, it will create a
-	"`TCPIP::<host>::<ip>::SOCKET`" device name instead.
+- `DG645_PORT`: this is better left blank (the default). In that
+  case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
+  name. If the port is specified, it will create a
+  "`TCPIP::<host>::<ip>::SOCKET`" device name instead.
   
-  - `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
-    TCP/IP device. If set, overrides host/port.
+- `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
+  TCP/IP device. If set, overrides host/port.
 	
-  - `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
-    If you've got this far, you know what this is good for ;-)
+- `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
+  If you've got this far, you know what this is good for ;-)
 	
-  - `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
-    (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
+- `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
+  (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
 	
-  - `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
-    to `info`.
-	
-  - `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
-    (about once per second) log the
-    current status of all variables it observes to the `info` logging
-	facility. The default is not to do that.
+- `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
+  to `info`.
+	
+- `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
+  (about once per second) log the
+  current status of all variables it observes to the `info` logging
+  acility. The default is not to do that.
 	
 
 EPICS Variables
 ---------------
 
 The IOC exports the following variables. To all of these the
 desginated prefix (`$DG645_EPICS_PREFIX`) needs to be prepended.
 
 Main IOC control and flow variables:
 
-  - `main_state`: used to drive the main query loop. Do not use.
-  
-  
+- `update`: used to drive the main query loop. When read, returns
+  an integer value which is being continuously increased on
+  every device readout (all readback values are read out regularly,
+  quasi-simultaneously, typically 1 up to 4 times per second).
+
 The presets device module:
 
-  - `pres:load`: when a string is written to this, the corresponding
-    preset is loaded. This is typically an instrument-specific feature.
-	On the DG645, `0` is loading instrument defaults, and `1` to `9`
-	are user-addressable slots.
-  - `pres:save`: when a string is written to this, current settings are
-    saved to the corresponding slot.
+- `pres:load`: when a string is written to this, the corresponding
+   preset is loaded. This is typically an instrument-specific feature.
+   on the DG645, `0` is loading instrument defaults, and `1` to `9`
+   are user-addressable slots.
+
+- `pres:save`: when a string is written to this, current settings are
+  saved to the corresponding slot.
 	
 	
 The error device module (for error handling)
 
-  - `err:last_RBV`: string representation of the latest device error.
-  - `err:clear`: when 1 is written here, the errors are cleared
-    (typically using a `*CLS` SCPI command)
+- `err:last_RBV`: string representation of the latest device error.
+- `err:clear`: when 1 is written here, the errors are cleared
+  (typically using a `*CLS` SCPI command)
 	
 	
 Trigger device module variables:
 
-  - `trig:lvl`: set the trigger channel level.
-  - `trig:lvl_RBV`: readback value for trigger channel level
-  - `src`: trigger source. Currently `"RISING"` and `"FALLING"`
-    are supported for the corresponding edges of the external
-	trigger pulse, and `"INTERNAL"` (on DG645) for an automated
-	internal trigger
-  - `src_RBV`: trigger source readback.
-  - `intrate`: trigger rate for internal trigger (in Hz)
-  - `intrate_RBV`: readback for the internal trigger frequency.
-  
+- `trig:lvl`: set the trigger channel level.
+- `trig:lvl_RBV`: readback value for trigger channel level
+- `src`: trigger source. Currently `"RISING"` and `"FALLING"`
+  are supported for the corresponding edges of the external
+  trigger pulse, and `"INTERNAL"` (on DG645) for an automated
+  internal trigger
+- `src_RBV`: trigger source readback.
+- `intrate`: trigger rate for internal trigger (in Hz)
+- `intrate_RBV`: readback for the internal trigger frequency.
+
 
 Channel specific variables: the DG645 has 4 channels, labeled
 `1`, `2`, `3` and `4`, respectively. Other devices may have
 different labels (when and if supported). For every channel,
 the following set of variables is exported. `{label}` designates
 the channel label, e.g. `ch{label}...` for channel 4 would be
 `ch4...`:
 
-  - `ch{label}:dly`: start of the delay, in seconds, from the
-    trigger pulse
-  - `ch{label}:dur`: pulse duration in seconds
-  - `ch{label}:div`: pulse divider (i.e. which N-th pulse to
-    trigger for)
-  - `ch{label}:ampl`: pulse amplitude in V
-  - `ch{label}:offs`: pulse offset in V
-  - `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
-  - `ch{label}:..._RBV`: each of the variables above publishes
-    its readback value in the corresponding `_RBV` PV.
+- `ch{label}:dly`: start of the delay, in seconds, from the
+  trigger pulse
+- `ch{label}:dur`: pulse duration in seconds
+- `ch{label}:div`: pulse divider (i.e. which N-th pulse to
+  trigger for)
+- `ch{label}:ampl`: pulse amplitude in V
+- `ch{label}:offs`: pulse offset in V
+- `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
+- `ch{label}:..._RBV`: each of the variables above publishes
+  its readback value in the corresponding `_RBV` PV.
 
 
 Caveats & Bugs
 --------------
 
 Might kick your dog, empty your fridge, and run off with your
 girlfriend.
 
 Otherwise enjoy! :-D
-
-
```

### Comparing `dg645-ioc-0.5.1/README.md` & `dg645-ioc-0.5.13/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,56 @@
 ![pipeline](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/pipeline.svg)
 ![coverage](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/coverage.svg)
 
 
 Quickstart
 ----------
 
-### Obtaining
+### In a System Shell
+
+#### Obtaining
 
 Download via PyPI: `pip install dg645-ioc` or via GitLab:
 
    ```
    git clone https://gitlab.com/kmc3-xpp/kronos-ioc
    ```
 
-### Running from the command line
+#### Running from the command line
 
 Configure at least the IP address and the EPICS prefix and start via shell:
 
    ```
    $ export DG645_EPICS_PREFIX="BEAMLINE:DG645:"
    $ export DG645_HOST="10.0.0.17"
    $ dg645-ioc
    INFO:kronos.ioc:Stanford Research Systems,DG645,s/n001776,ver1.14.10E
    INFO:root:Starting IOC, PV list following
    [...]
    INFO:caproto.ctx:Server startup complete.
    ```
-   
-### Obtaining a Container
+
+### In a Container
+
+#### Obtaining a Container
 
 
 You can download the automatically generated container:
 
    ```
    podman pull registry.gitlab.com/kmc3-xpp/kronos-ioc:latest
    ```
 
 ...or create your own, assuming  you've downloaded the sources into `./kronos-ioc`:
 
    ```
    $ podman build -t kronos-ioc -f kronos-ioc/Dockerfile -v $PWD/kronos-ioc:/kronos_src:z
    ```
 
-### Running in Podman / Docker
+#### Running in Podman / Docker
 
 Start as a Podman container (Docker should work the same, just replace thed
 `podman` command by `docker`):
 
    ```
    $ podman run -ti --rm \
        --env DG645_EPICS_PREFIX="BEAMLINE:DG645:" \
@@ -73,101 +77,102 @@
    ```
 
 Configuration
 -------------
 
  Here's a list of environment variables that might help:
  
-  - `DG645_HOST`: host name or IP of the DG645 controller
+- `DG645_HOST`: host name or IP of the DG645 controller
   
-  - `DG645_PORT`: this is better left blank (the default). In that
-    case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
-	name. If the port is specified, it will create a
-	"`TCPIP::<host>::<ip>::SOCKET`" device name instead.
+- `DG645_PORT`: this is better left blank (the default). In that
+  case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
+  name. If the port is specified, it will create a
+  "`TCPIP::<host>::<ip>::SOCKET`" device name instead.
   
-  - `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
-    TCP/IP device. If set, overrides host/port.
+- `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
+  TCP/IP device. If set, overrides host/port.
 	
-  - `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
-    If you've got this far, you know what this is good for ;-)
+- `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
+  If you've got this far, you know what this is good for ;-)
 	
-  - `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
-    (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
+- `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
+  (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
 	
-  - `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
-    to `info`.
-	
-  - `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
-    (about once per second) log the
-    current status of all variables it observes to the `info` logging
-	facility. The default is not to do that.
+- `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
+  to `info`.
+	
+- `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
+  (about once per second) log the
+  current status of all variables it observes to the `info` logging
+  acility. The default is not to do that.
 	
 
 EPICS Variables
 ---------------
 
 The IOC exports the following variables. To all of these the
 desginated prefix (`$DG645_EPICS_PREFIX`) needs to be prepended.
 
 Main IOC control and flow variables:
 
-  - `main_state`: used to drive the main query loop. Do not use.
-  
-  
+- `update`: used to drive the main query loop. When read, returns
+  an integer value which is being continuously increased on
+  every device readout (all readback values are read out regularly,
+  quasi-simultaneously, typically 1 up to 4 times per second).
+
 The presets device module:
 
-  - `pres:load`: when a string is written to this, the corresponding
-    preset is loaded. This is typically an instrument-specific feature.
-	On the DG645, `0` is loading instrument defaults, and `1` to `9`
-	are user-addressable slots.
-  - `pres:save`: when a string is written to this, current settings are
-    saved to the corresponding slot.
+- `pres:load`: when a string is written to this, the corresponding
+   preset is loaded. This is typically an instrument-specific feature.
+   on the DG645, `0` is loading instrument defaults, and `1` to `9`
+   are user-addressable slots.
+
+- `pres:save`: when a string is written to this, current settings are
+  saved to the corresponding slot.
 	
 	
 The error device module (for error handling)
 
-  - `err:last_RBV`: string representation of the latest device error.
-  - `err:clear`: when 1 is written here, the errors are cleared
-    (typically using a `*CLS` SCPI command)
+- `err:last_RBV`: string representation of the latest device error.
+- `err:clear`: when 1 is written here, the errors are cleared
+  (typically using a `*CLS` SCPI command)
 	
 	
 Trigger device module variables:
 
-  - `trig:lvl`: set the trigger channel level.
-  - `trig:lvl_RBV`: readback value for trigger channel level
-  - `src`: trigger source. Currently `"RISING"` and `"FALLING"`
-    are supported for the corresponding edges of the external
-	trigger pulse, and `"INTERNAL"` (on DG645) for an automated
-	internal trigger
-  - `src_RBV`: trigger source readback.
-  - `intrate`: trigger rate for internal trigger (in Hz)
-  - `intrate_RBV`: readback for the internal trigger frequency.
-  
+- `trig:lvl`: set the trigger channel level.
+- `trig:lvl_RBV`: readback value for trigger channel level
+- `src`: trigger source. Currently `"RISING"` and `"FALLING"`
+  are supported for the corresponding edges of the external
+  trigger pulse, and `"INTERNAL"` (on DG645) for an automated
+  internal trigger
+- `src_RBV`: trigger source readback.
+- `intrate`: trigger rate for internal trigger (in Hz)
+- `intrate_RBV`: readback for the internal trigger frequency.
+
 
 Channel specific variables: the DG645 has 4 channels, labeled
 `1`, `2`, `3` and `4`, respectively. Other devices may have
 different labels (when and if supported). For every channel,
 the following set of variables is exported. `{label}` designates
 the channel label, e.g. `ch{label}...` for channel 4 would be
 `ch4...`:
 
-  - `ch{label}:dly`: start of the delay, in seconds, from the
-    trigger pulse
-  - `ch{label}:dur`: pulse duration in seconds
-  - `ch{label}:div`: pulse divider (i.e. which N-th pulse to
-    trigger for)
-  - `ch{label}:ampl`: pulse amplitude in V
-  - `ch{label}:offs`: pulse offset in V
-  - `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
-  - `ch{label}:..._RBV`: each of the variables above publishes
-    its readback value in the corresponding `_RBV` PV.
+- `ch{label}:dly`: start of the delay, in seconds, from the
+  trigger pulse
+- `ch{label}:dur`: pulse duration in seconds
+- `ch{label}:div`: pulse divider (i.e. which N-th pulse to
+  trigger for)
+- `ch{label}:ampl`: pulse amplitude in V
+- `ch{label}:offs`: pulse offset in V
+- `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
+- `ch{label}:..._RBV`: each of the variables above publishes
+  its readback value in the corresponding `_RBV` PV.
 
 
 Caveats & Bugs
 --------------
 
 Might kick your dog, empty your fridge, and run off with your
 girlfriend.
 
 Otherwise enjoy! :-D
-
-
```

### Comparing `dg645-ioc-0.5.1/pyproject.toml` & `dg645-ioc-0.5.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/src/dg645_ioc.egg-info/PKG-INFO` & `dg645-ioc-0.5.13/src/dg645_ioc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dg645-ioc
-Version: 0.5.1
+Version: 0.5.13
 Summary: CAproto-based pure-Python EPICS IOC for the Stanford Research Systems DG645 delay generator.
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source, https://gitlab.com/kmc3-xpp/kronos-ioc
 Project-URL: Issues, https://gitlab.com/kmc3-xpp/kronos-ioc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
@@ -32,52 +32,56 @@
 ![pipeline](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/pipeline.svg)
 ![coverage](https://gitlab.com/kmc3-xpp/kronos-ioc/badges/release/coverage.svg)
 
 
 Quickstart
 ----------
 
-### Obtaining
+### In a System Shell
+
+#### Obtaining
 
 Download via PyPI: `pip install dg645-ioc` or via GitLab:
 
    ```
    git clone https://gitlab.com/kmc3-xpp/kronos-ioc
    ```
 
-### Running from the command line
+#### Running from the command line
 
 Configure at least the IP address and the EPICS prefix and start via shell:
 
    ```
    $ export DG645_EPICS_PREFIX="BEAMLINE:DG645:"
    $ export DG645_HOST="10.0.0.17"
    $ dg645-ioc
    INFO:kronos.ioc:Stanford Research Systems,DG645,s/n001776,ver1.14.10E
    INFO:root:Starting IOC, PV list following
    [...]
    INFO:caproto.ctx:Server startup complete.
    ```
-   
-### Obtaining a Container
+
+### In a Container
+
+#### Obtaining a Container
 
 
 You can download the automatically generated container:
 
    ```
    podman pull registry.gitlab.com/kmc3-xpp/kronos-ioc:latest
    ```
 
 ...or create your own, assuming  you've downloaded the sources into `./kronos-ioc`:
 
    ```
    $ podman build -t kronos-ioc -f kronos-ioc/Dockerfile -v $PWD/kronos-ioc:/kronos_src:z
    ```
 
-### Running in Podman / Docker
+#### Running in Podman / Docker
 
 Start as a Podman container (Docker should work the same, just replace thed
 `podman` command by `docker`):
 
    ```
    $ podman run -ti --rm \
        --env DG645_EPICS_PREFIX="BEAMLINE:DG645:" \
@@ -100,101 +104,102 @@
    ```
 
 Configuration
 -------------
 
  Here's a list of environment variables that might help:
  
-  - `DG645_HOST`: host name or IP of the DG645 controller
+- `DG645_HOST`: host name or IP of the DG645 controller
   
-  - `DG645_PORT`: this is better left blank (the default). In that
-    case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
-	name. If the port is specified, it will create a
-	"`TCPIP::<host>::<ip>::SOCKET`" device name instead.
+- `DG645_PORT`: this is better left blank (the default). In that
+  case, the IOC will create a "`TCPIP::<host>::INSTR`" PyVISA device
+  name. If the port is specified, it will create a
+  "`TCPIP::<host>::<ip>::SOCKET`" device name instead.
   
-  - `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
-    TCP/IP device. If set, overrides host/port.
+- `DG645_VISA_DEV`: PyVISA device to connecto to, instead of the
+  TCP/IP device. If set, overrides host/port.
 	
-  - `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
-    If you've got this far, you know what this is good for ;-)
+- `DG645_VISA_RMAN`: PyVISA resource manager. Defaults to `"@py"`.
+  If you've got this far, you know what this is good for ;-)
 	
-  - `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
-    (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
+- `DG645_EPICS_PREFIX`: EPICS PV prefix to use. Include trailing column
+  (`:`) if you need one. Defaults to `KMC3:XPP:DG645:`.
 	
-  - `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
-    to `info`.
-	
-  - `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
-    (about once per second) log the
-    current status of all variables it observes to the `info` logging
-	facility. The default is not to do that.
+- `DG645_LOGGING`: one of `error`, `warn`, `info` or `debug`. Defaults
+  to `info`.
+	
+- `DG645_LOG_STATUS`: if set to `yes`, the IOC will periodically
+  (about once per second) log the
+  current status of all variables it observes to the `info` logging
+  acility. The default is not to do that.
 	
 
 EPICS Variables
 ---------------
 
 The IOC exports the following variables. To all of these the
 desginated prefix (`$DG645_EPICS_PREFIX`) needs to be prepended.
 
 Main IOC control and flow variables:
 
-  - `main_state`: used to drive the main query loop. Do not use.
-  
-  
+- `update`: used to drive the main query loop. When read, returns
+  an integer value which is being continuously increased on
+  every device readout (all readback values are read out regularly,
+  quasi-simultaneously, typically 1 up to 4 times per second).
+
 The presets device module:
 
-  - `pres:load`: when a string is written to this, the corresponding
-    preset is loaded. This is typically an instrument-specific feature.
-	On the DG645, `0` is loading instrument defaults, and `1` to `9`
-	are user-addressable slots.
-  - `pres:save`: when a string is written to this, current settings are
-    saved to the corresponding slot.
+- `pres:load`: when a string is written to this, the corresponding
+   preset is loaded. This is typically an instrument-specific feature.
+   on the DG645, `0` is loading instrument defaults, and `1` to `9`
+   are user-addressable slots.
+
+- `pres:save`: when a string is written to this, current settings are
+  saved to the corresponding slot.
 	
 	
 The error device module (for error handling)
 
-  - `err:last_RBV`: string representation of the latest device error.
-  - `err:clear`: when 1 is written here, the errors are cleared
-    (typically using a `*CLS` SCPI command)
+- `err:last_RBV`: string representation of the latest device error.
+- `err:clear`: when 1 is written here, the errors are cleared
+  (typically using a `*CLS` SCPI command)
 	
 	
 Trigger device module variables:
 
-  - `trig:lvl`: set the trigger channel level.
-  - `trig:lvl_RBV`: readback value for trigger channel level
-  - `src`: trigger source. Currently `"RISING"` and `"FALLING"`
-    are supported for the corresponding edges of the external
-	trigger pulse, and `"INTERNAL"` (on DG645) for an automated
-	internal trigger
-  - `src_RBV`: trigger source readback.
-  - `intrate`: trigger rate for internal trigger (in Hz)
-  - `intrate_RBV`: readback for the internal trigger frequency.
-  
+- `trig:lvl`: set the trigger channel level.
+- `trig:lvl_RBV`: readback value for trigger channel level
+- `src`: trigger source. Currently `"RISING"` and `"FALLING"`
+  are supported for the corresponding edges of the external
+  trigger pulse, and `"INTERNAL"` (on DG645) for an automated
+  internal trigger
+- `src_RBV`: trigger source readback.
+- `intrate`: trigger rate for internal trigger (in Hz)
+- `intrate_RBV`: readback for the internal trigger frequency.
+
 
 Channel specific variables: the DG645 has 4 channels, labeled
 `1`, `2`, `3` and `4`, respectively. Other devices may have
 different labels (when and if supported). For every channel,
 the following set of variables is exported. `{label}` designates
 the channel label, e.g. `ch{label}...` for channel 4 would be
 `ch4...`:
 
-  - `ch{label}:dly`: start of the delay, in seconds, from the
-    trigger pulse
-  - `ch{label}:dur`: pulse duration in seconds
-  - `ch{label}:div`: pulse divider (i.e. which N-th pulse to
-    trigger for)
-  - `ch{label}:ampl`: pulse amplitude in V
-  - `ch{label}:offs`: pulse offset in V
-  - `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
-  - `ch{label}:..._RBV`: each of the variables above publishes
-    its readback value in the corresponding `_RBV` PV.
+- `ch{label}:dly`: start of the delay, in seconds, from the
+  trigger pulse
+- `ch{label}:dur`: pulse duration in seconds
+- `ch{label}:div`: pulse divider (i.e. which N-th pulse to
+  trigger for)
+- `ch{label}:ampl`: pulse amplitude in V
+- `ch{label}:offs`: pulse offset in V
+- `ch{label}:pol`: pulse polarity, can be one of `"POS"` or `"NEG"`.
+- `ch{label}:..._RBV`: each of the variables above publishes
+  its readback value in the corresponding `_RBV` PV.
 
 
 Caveats & Bugs
 --------------
 
 Might kick your dog, empty your fridge, and run off with your
 girlfriend.
 
 Otherwise enjoy! :-D
-
-
```

### Comparing `dg645-ioc-0.5.1/src/kronos/application.py` & `dg645-ioc-0.5.13/src/kronos/application.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/src/kronos/channel.py` & `dg645-ioc-0.5.13/src/kronos/channel.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/src/kronos/flags.py` & `dg645-ioc-0.5.13/src/kronos/flags.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/src/kronos/ioc.py` & `dg645-ioc-0.5.13/src/kronos/ioc.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/src/kronos/main.py` & `dg645-ioc-0.5.13/src/kronos/main.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/test/test_dg645.py` & `dg645-ioc-0.5.13/test/test_dg645.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/test/test_ioc.py` & `dg645-ioc-0.5.13/test/test_ioc.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.5.1/test/visa-sim-dg645.yml` & `dg645-ioc-0.5.13/test/visa-sim-dg645.yml`

 * *Files identical despite different names*

