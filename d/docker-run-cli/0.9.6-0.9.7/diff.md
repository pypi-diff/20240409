# Comparing `tmp/docker-run-cli-0.9.6.tar.gz` & `tmp/docker-run-cli-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-run-cli-0.9.6.tar", last modified: Tue Nov 14 17:25:49 2023, max compression
+gzip compressed data, was "docker-run-cli-0.9.7.tar", last modified: Tue Apr  9 11:31:05 2024, max compression
```

## Comparing `docker-run-cli-0.9.6.tar` & `docker-run-cli-0.9.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.265443 docker-run-cli-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-11-14 17:25:49.265443 docker-run-cli-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.257443 docker-run-cli-0.9.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1620 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/scripts/activate-python-docker-run-shell-completion
--rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/scripts/docker-run
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 17:25:49.265443 docker-run-cli-0.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.253443 docker-run-cli-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.257443 docker-run-cli-0.9.6/src/docker_run/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.261443 docker-run-cli-0.9.6/src/docker_run/bash_completion.d/
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/bash_completion.d/docker-run
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.261443 docker-run-cli-0.9.6/src/docker_run/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-11-14 17:25:31.000000 docker-run-cli-0.9.6/src/docker_run/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 17:25:49.265443 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-11-14 17:25:49.000000 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-11-14 17:25:49.000000 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 17:25:49.000000 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-14 17:25:49.000000 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-14 17:25:49.000000 docker-run-cli-0.9.6/src/docker_run_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.317419 docker-run-cli-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-09 11:31:05.317419 docker-run-cli-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.313419 docker-run-cli-0.9.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1620 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/scripts/activate-python-docker-run-shell-completion
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1506 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/scripts/docker-run
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:31:05.317419 docker-run-cli-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.313419 docker-run-cli-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.313419 docker-run-cli-0.9.7/src/docker_run/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.313419 docker-run-cli-0.9.7/src/docker_run/bash_completion.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/bash_completion.d/docker-run
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.317419 docker-run-cli-0.9.7/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 11:30:59.000000 docker-run-cli-0.9.7/src/docker_run/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:05.317419 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-09 11:31:05.000000 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 11:31:05.000000 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:31:05.000000 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 11:31:05.000000 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:31:05.000000 docker-run-cli-0.9.7/src/docker_run_cli.egg-info/top_level.txt
```

### Comparing `docker-run-cli-0.9.6/LICENSE` & `docker-run-cli-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.6/PKG-INFO` & `docker-run-cli-0.9.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.6
+Version: 0.9.7
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -32,23 +32,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GPUtil~=1.4.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docker-ros
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "docker-ros"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "docker-ros"
 Provides-Extra: plugins
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "plugins"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "plugins"
 Provides-Extra: all
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "all"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "all"
 Requires-Dist: build; extra == "all"
 Requires-Dist: twine; extra == "all"
 
 <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png" height=130 align="right">
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
@@ -56,14 +57,22 @@
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+> [!IMPORTANT]  
+> This repository is open-sourced and maintained by the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**](https://www.ika.rwth-aachen.de/).  
+> **DevOps, Containerization and Orchestration of Software-Defined Vehicles** are some of many research topics within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-driving.html) domain.  
+> If you would like to learn more about how we can support your DevOps or automated driving efforts, feel free to reach out to us!  
+> &nbsp;&nbsp;&nbsp;&nbsp; *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated Driving*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *+49 241 80 23549*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *timo.woopen@ika.rwth-aachen.de*  
+
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
 
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
@@ -84,18 +93,19 @@
 
 In general, you can pass the same arguments to `docker-run` as you would pass to `docker run`, e.g.
 
 ```bash
 docker-run --volume $(pwd):/volume ubuntu ls /volume
 ```
 
-In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Each of these default features can be disabled, see [Usage](#usage).
+In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Most of these default features can be disabled, see [Usage](#usage).
 - container removal after exit (`--rm`)
 - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`)
+- relative bind mounts (`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`)
 - GPU support (`--gpus all` / `--runtime nvidia`)
 - X11 GUI forwarding
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.6 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.7 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 rwth-aachen.de>, Jean-Pierre Busch
 rwth-aachen.de> Maintainer-email: Lennart Reiher
 rwth-aachen.de>, Jean-Pierre Busch
 rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -20,28 +20,38 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Repository, https://github.com/ika-rwth-
 aachen/docker-run Project-URL: Bug Tracker, https://github.com/ika-rwth-aachen/
 docker-run/issues Keywords: docker,container Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: POSIX ::
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE Provides-Extra: dev Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" Provides-Extra: docker-ros Requires-Dist:
-docker-run-docker-ros>=1.0.4; extra == "docker-ros" Provides-Extra: plugins
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "plugins" Provides-Extra:
-all Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "all" Requires-Dist:
-build; extra == "all" Requires-Dist: twine; extra == "all" [https://github.com/
-ika-rwth-aachen/docker-run/raw/main/assets/logo.png]# *docker-run* â ``docker
-run`` and ``docker exec`` with useful defaults
+File: LICENSE Requires-Dist: GPUtil~=1.4.0 Provides-Extra: dev Requires-Dist:
+build; extra == "dev" Requires-Dist: twine; extra == "dev" Provides-Extra:
+docker-ros Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "docker-ros"
+Provides-Extra: plugins Requires-Dist: docker-run-docker-ros>=1.0.5; extra ==
+"plugins" Provides-Extra: all Requires-Dist: docker-run-docker-ros>=1.0.5;
+extra == "all" Requires-Dist: build; extra == "all" Requires-Dist: twine; extra
+== "all" [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/
+logo.png]# *docker-run* â ``docker run`` and ``docker exec`` with useful
+defaults
   [https://img.shields.io/github/license/ika-rwth-aachen/docker-run]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
              _d_m_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_c_o_l_o_r_=_b_l_u_e_&_l_a_b_e_l_=_P_y_P_I_%_2_0_d_o_w_n_l_o_a_d_s_]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments.
+arguments. > [!IMPORTANT] > This repository is open-sourced and maintained by
+the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**]
+(https://www.ika.rwth-aachen.de/). > **DevOps, Containerization and
+Orchestration of Software-Defined Vehicles** are some of many research topics
+within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-
+aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-
+driving.html) domain. > If you would like to learn more about how we can
+support your DevOps or automated driving efforts, feel free to reach out to us!
+>      *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated
+Driving* >      *+49â¯241â¯80 23549* >      *timo.woopen@ika.rwth-aachen.de*
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_i_k_a_-_r_w_t_h_-
 _a_a_c_h_e_n_/_d_o_c_k_e_r_-_r_o_s_?_s_t_y_l_e_=_s_o_c_i_a_l_]- [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
@@ -53,20 +63,21 @@
 607qwq/xeyes ``` ## Functionality `docker-run` is designed to be used the same
 way as the official [`docker run`](https://docs.docker.com/engine/reference/
 commandline/run/) and [`docker exec`](https://docs.docker.com/engine/reference/
 commandline/exec/) commands. In general, you can pass the same arguments to
 `docker-run` as you would pass to `docker run`, e.g. ```bash docker-run --
 volume $(pwd):/volume ubuntu ls /volume ``` In addition to the arguments you
 are passing, `docker-run` however also enables the following features by
-default. Each of these default features can be disabled, see [Usage](#usage). -
+default. Most of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
-- current directory name as container name (`--name`) - GPU support (`--gpus
-all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
-name is already running, `docker-run` will execute a command in that container
-via `docker exec` instead. This lets you quickly attach to a running container
+- current directory name as container name (`--name`) - relative bind mounts
+(`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`) - GPU support (`--gpus all` / `--
+runtime nvidia`) - X11 GUI forwarding If a container with matching name is
+already running, `docker-run` will execute a command in that container via
+`docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
 container ``` Unlike with `docker run`, you can also set the Docker image via
 the `--image` arguments, see [Usage](#usage). This may be required for more
 complex use cases. ## Installation ```bash pip install docker-run-cli #
 (optional) shell auto-completion source $(activate-python-docker-run-shell-
 completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
 *pip* may default to a user-site installation of executables to `~/.local/bin`,
```

### Comparing `docker-run-cli-0.9.6/README.md` & `docker-run-cli-0.9.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,22 @@
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+> [!IMPORTANT]  
+> This repository is open-sourced and maintained by the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**](https://www.ika.rwth-aachen.de/).  
+> **DevOps, Containerization and Orchestration of Software-Defined Vehicles** are some of many research topics within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-driving.html) domain.  
+> If you would like to learn more about how we can support your DevOps or automated driving efforts, feel free to reach out to us!  
+> &nbsp;&nbsp;&nbsp;&nbsp; *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated Driving*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *+49 241 80 23549*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *timo.woopen@ika.rwth-aachen.de*  
+
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
 
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
@@ -34,18 +42,19 @@
 
 In general, you can pass the same arguments to `docker-run` as you would pass to `docker run`, e.g.
 
 ```bash
 docker-run --volume $(pwd):/volume ubuntu ls /volume
 ```
 
-In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Each of these default features can be disabled, see [Usage](#usage).
+In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Most of these default features can be disabled, see [Usage](#usage).
 - container removal after exit (`--rm`)
 - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`)
+- relative bind mounts (`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`)
 - GPU support (`--gpus all` / `--runtime nvidia`)
 - X11 GUI forwarding
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
```

#### html2text {}

```diff
@@ -1,15 +1,24 @@
 [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png]#
 *docker-run* â ``docker run`` and ``docker exec`` with useful defaults
   [https://img.shields.io/github/license/ika-rwth-aachen/docker-run]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
              _d_m_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_c_o_l_o_r_=_b_l_u_e_&_l_a_b_e_l_=_P_y_P_I_%_2_0_d_o_w_n_l_o_a_d_s_]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments.
+arguments. > [!IMPORTANT] > This repository is open-sourced and maintained by
+the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**]
+(https://www.ika.rwth-aachen.de/). > **DevOps, Containerization and
+Orchestration of Software-Defined Vehicles** are some of many research topics
+within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-
+aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-
+driving.html) domain. > If you would like to learn more about how we can
+support your DevOps or automated driving efforts, feel free to reach out to us!
+>      *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated
+Driving* >      *+49â¯241â¯80 23549* >      *timo.woopen@ika.rwth-aachen.de*
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_i_k_a_-_r_w_t_h_-
 _a_a_c_h_e_n_/_d_o_c_k_e_r_-_r_o_s_?_s_t_y_l_e_=_s_o_c_i_a_l_]- [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
@@ -21,20 +30,21 @@
 607qwq/xeyes ``` ## Functionality `docker-run` is designed to be used the same
 way as the official [`docker run`](https://docs.docker.com/engine/reference/
 commandline/run/) and [`docker exec`](https://docs.docker.com/engine/reference/
 commandline/exec/) commands. In general, you can pass the same arguments to
 `docker-run` as you would pass to `docker run`, e.g. ```bash docker-run --
 volume $(pwd):/volume ubuntu ls /volume ``` In addition to the arguments you
 are passing, `docker-run` however also enables the following features by
-default. Each of these default features can be disabled, see [Usage](#usage). -
+default. Most of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
-- current directory name as container name (`--name`) - GPU support (`--gpus
-all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
-name is already running, `docker-run` will execute a command in that container
-via `docker exec` instead. This lets you quickly attach to a running container
+- current directory name as container name (`--name`) - relative bind mounts
+(`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`) - GPU support (`--gpus all` / `--
+runtime nvidia`) - X11 GUI forwarding If a container with matching name is
+already running, `docker-run` will execute a command in that container via
+`docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
 container ``` Unlike with `docker run`, you can also set the Docker image via
 the `--image` arguments, see [Usage](#usage). This may be required for more
 complex use cases. ## Installation ```bash pip install docker-run-cli #
 (optional) shell auto-completion source $(activate-python-docker-run-shell-
 completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
 *pip* may default to a user-site installation of executables to `~/.local/bin`,
```

### Comparing `docker-run-cli-0.9.6/pyproject.toml` & `docker-run-cli-0.9.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-cli"
-version = "0.9.6"
+version = "0.9.7"
 description = "'docker run' and 'docker exec' with useful defaults"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
@@ -19,22 +19,22 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = ["docker", "container"]
-dependencies = []
+dependencies = ["GPUtil~=1.4.0"]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
-docker-ros = ["docker-run-docker-ros>=1.0.4"]
-plugins = ["docker-run-docker-ros>=1.0.4"]
-all = ["docker-run-docker-ros>=1.0.4", "build", "twine"]
+docker-ros = ["docker-run-docker-ros>=1.0.5"]
+plugins = ["docker-run-docker-ros>=1.0.5"]
+all = ["docker-run-docker-ros>=1.0.5", "build", "twine"]
 
 [project.urls]
 "Repository" = "https://github.com/ika-rwth-aachen/docker-run"
 "Bug Tracker" = "https://github.com/ika-rwth-aachen/docker-run/issues"
 
 [tool.setuptools]
 script-files = [
```

### Comparing `docker-run-cli-0.9.6/scripts/activate-python-docker-run-shell-completion` & `docker-run-cli-0.9.7/scripts/activate-python-docker-run-shell-completion`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.6/scripts/docker-run` & `docker-run-cli-0.9.7/scripts/docker-run`

 * *Files 26% similar despite different names*

```diff
@@ -22,12 +22,25 @@
 
 # generate docker run/exec command
 CMD_FILE=$(mktemp)
 python3 -m docker_run "${@}" 2>&1 >$CMD_FILE
 CMD=$(cat $CMD_FILE)
 rm $CMD_FILE
 
+# convert command string to array to allow for escaped characters, e.g. "docker run -v /path\ with\ spaces:/path\ with\ spaces ..."
+CMD_ARRAY=()
+  while IFS= read -r -d ' ' part; do
+    while [[ $part == *"\\" ]]; do
+      part+=" "
+      part="${part//\\/}"
+      IFS= read -r -d ' ' next_part
+      part+=$next_part
+    done
+    CMD_ARRAY+=("$part")
+  done <<< "$CMD"
+  CMD_ARRAY+=("${part%$'\n'}")
+
 # execute command
 if [[ ! -z "$CMD" ]]; then
   echo -e "================================================================================\n"
-  exec $CMD
+  exec "${CMD_ARRAY[@]}"
 fi
```

### Comparing `docker-run-cli-0.9.6/src/docker_run/bash_completion.d/docker-run` & `docker-run-cli-0.9.7/src/docker_run/bash_completion.d/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.6/src/docker_run/core.py` & `docker-run-cli-0.9.7/src/docker_run/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,18 @@
 
         # command
         if len(cmd_args) > 0:
             docker_cmd += cmd_args
         else:
             docker_cmd += ["bash"] # default exec command
 
+    # plugin modifications
+    for plugin in PLUGINS:
+        docker_cmd = plugin.modifyFinalCommand(docker_cmd, args, unknown_args)
+
     return " ".join(docker_cmd)
 
 
 def printDockerCommand(cmd: str):
     """Prints a docker command in human-readable way by line-breaking on each new argument.
 
     Args:
```

### Comparing `docker-run-cli-0.9.6/src/docker_run/plugins/core.py` & `docker-run-cli-0.9.7/src/docker_run/plugins/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 import os
 import platform
 import tempfile
 from typing import Any, Dict, List
 
+import GPUtil
+
 from docker_run.utils import log, runCommand
 from docker_run.plugins.plugin import Plugin
 
 
 class CorePlugin(Plugin):
 
     OS = platform.uname().system
@@ -52,14 +54,21 @@
     def getExecFlags(cls, args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
         flags = []
         if not args["no_it"]:
             flags += cls.interactiveFlags()
         return flags
 
     @classmethod
+    def modifyFinalCommand(cls, cmd: List[str], args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
+        if "-v" in cmd or "--volume" in cmd:
+            cmd = cls.resolveRelativeVolumeFlags(cmd)
+            cmd = cls.fixSpacesInVolumeFlags(cmd)
+        return cmd
+
+    @classmethod
     def removeFlags(cls) -> List[str]:
         return ["--rm"]
 
     @classmethod
     def interactiveFlags(cls) -> List[str]:
         return ["--interactive", "--tty"]
 
@@ -74,29 +83,33 @@
 
     @classmethod
     def localeFlags(cls) -> List[str]:
         return ["--env LANG", "--env LANGUAGE", "--env LC_ALL"]
 
     @classmethod
     def gpuSupportFlags(cls) -> List[str]:
-        if cls.ARCH == "x86_64":
-            return ["--gpus all"]
-        elif cls.ARCH == "aarch64" and cls.OS == "Linux":
-            return ["--runtime nvidia"]
+        if len(GPUtil.getGPUs()) > 0:
+            if cls.ARCH == "x86_64":
+                return ["--gpus all"]
+            elif cls.ARCH == "aarch64" and cls.OS == "Linux":
+                return ["--runtime nvidia"]
+            else:
+                log(f"GPU not supported by `docker-run` on {cls.OS} with {cls.ARCH} architecture")
+                return []
         else:
-            log(f"GPU not supported by `docker-run` on {cls.OS} with {cls.ARCH} architecture")
+            log(f"No GPU detected")
             return []
 
     @classmethod
     def x11GuiForwardingFlags(cls, docker_network: str = "bridge") -> List[str]:
 
         display = os.environ.get("DISPLAY")
         if display is None:
             return []
-        
+
         if cls.OS == "Darwin":
             runCommand(f"xhost +local:")
 
         xsock = "/tmp/.X11-unix"
         xauth = tempfile.NamedTemporaryFile(prefix='.docker.xauth.', delete=False).name
         xauth_display = display if cls.OS != "Darwin" else runCommand("ifconfig en0 | grep 'inet '")[0].split()[1] + ":0"
         xauth_output = "ffff" + runCommand(f"xauth nlist {xauth_display}")[0][4:]
@@ -115,8 +128,26 @@
         flags.append(f"--volume {xauth}:{xauth}")
         flags.append(f"--volume {xsock}:{xsock}")
 
         return flags
 
     @classmethod
     def currentDirMountFlags(cls) -> List[str]:
-        return [f"--volume {os.getcwd()}:{os.getcwd()}", f"--workdir {os.getcwd()}"]
+        cwd = os.getcwd().replace(" ", "\\ ")
+        return [f"--volume {cwd}:{cwd}", f"--workdir {cwd}"]
+
+    @classmethod
+    def resolveRelativeVolumeFlags(cls, cmd: List[str]) -> List[str]:
+        for i, arg in enumerate(cmd):
+            if arg in ["-v", "--volume"]:
+                mount_path = cmd[i + 1].split(":")[0]
+                if mount_path.startswith("."):
+                    absolute_mount_path = os.path.abspath(mount_path)
+                    cmd[i + 1] = absolute_mount_path + cmd[i + 1][len(mount_path):]
+        return cmd
+
+    @classmethod
+    def fixSpacesInVolumeFlags(cls, cmd: List[str]) -> List[str]:
+        for i, arg in enumerate(cmd):
+            if arg in ["-v", "--volume"]:
+                cmd[i + 1] = cmd[i + 1].replace(" ", "\\ ")
+        return cmd
```

### Comparing `docker-run-cli-0.9.6/src/docker_run/plugins/plugin.py` & `docker-run-cli-0.9.7/src/docker_run/plugins/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,7 +14,11 @@
     def getRunFlags(cls, args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
         raise NotImplementedError()
 
     @classmethod
     @abstractmethod
     def getExecFlags(cls, args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
         raise NotImplementedError()
+
+    @classmethod
+    def modifyFinalCommand(cls, cmd: List[str], args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
+        return cmd
```

### Comparing `docker-run-cli-0.9.6/src/docker_run/utils.py` & `docker-run-cli-0.9.7/src/docker_run/utils.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.6/src/docker_run_cli.egg-info/PKG-INFO` & `docker-run-cli-0.9.7/src/docker_run_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.6
+Version: 0.9.7
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -32,23 +32,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GPUtil~=1.4.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docker-ros
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "docker-ros"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "docker-ros"
 Provides-Extra: plugins
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "plugins"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "plugins"
 Provides-Extra: all
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "all"
+Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "all"
 Requires-Dist: build; extra == "all"
 Requires-Dist: twine; extra == "all"
 
 <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png" height=130 align="right">
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
@@ -56,14 +57,22 @@
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+> [!IMPORTANT]  
+> This repository is open-sourced and maintained by the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**](https://www.ika.rwth-aachen.de/).  
+> **DevOps, Containerization and Orchestration of Software-Defined Vehicles** are some of many research topics within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-driving.html) domain.  
+> If you would like to learn more about how we can support your DevOps or automated driving efforts, feel free to reach out to us!  
+> &nbsp;&nbsp;&nbsp;&nbsp; *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated Driving*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *+49 241 80 23549*  
+> &nbsp;&nbsp;&nbsp;&nbsp; *timo.woopen@ika.rwth-aachen.de*  
+
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
 
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
@@ -84,18 +93,19 @@
 
 In general, you can pass the same arguments to `docker-run` as you would pass to `docker run`, e.g.
 
 ```bash
 docker-run --volume $(pwd):/volume ubuntu ls /volume
 ```
 
-In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Each of these default features can be disabled, see [Usage](#usage).
+In addition to the arguments you are passing, `docker-run` however also enables the following features by default. Most of these default features can be disabled, see [Usage](#usage).
 - container removal after exit (`--rm`)
 - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`)
+- relative bind mounts (`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`)
 - GPU support (`--gpus all` / `--runtime nvidia`)
 - X11 GUI forwarding
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.6 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.7 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 rwth-aachen.de>, Jean-Pierre Busch
 rwth-aachen.de> Maintainer-email: Lennart Reiher
 rwth-aachen.de>, Jean-Pierre Busch
 rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -20,28 +20,38 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Repository, https://github.com/ika-rwth-
 aachen/docker-run Project-URL: Bug Tracker, https://github.com/ika-rwth-aachen/
 docker-run/issues Keywords: docker,container Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: POSIX ::
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
-File: LICENSE Provides-Extra: dev Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" Provides-Extra: docker-ros Requires-Dist:
-docker-run-docker-ros>=1.0.4; extra == "docker-ros" Provides-Extra: plugins
-Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "plugins" Provides-Extra:
-all Requires-Dist: docker-run-docker-ros>=1.0.4; extra == "all" Requires-Dist:
-build; extra == "all" Requires-Dist: twine; extra == "all" [https://github.com/
-ika-rwth-aachen/docker-run/raw/main/assets/logo.png]# *docker-run* â ``docker
-run`` and ``docker exec`` with useful defaults
+File: LICENSE Requires-Dist: GPUtil~=1.4.0 Provides-Extra: dev Requires-Dist:
+build; extra == "dev" Requires-Dist: twine; extra == "dev" Provides-Extra:
+docker-ros Requires-Dist: docker-run-docker-ros>=1.0.5; extra == "docker-ros"
+Provides-Extra: plugins Requires-Dist: docker-run-docker-ros>=1.0.5; extra ==
+"plugins" Provides-Extra: all Requires-Dist: docker-run-docker-ros>=1.0.5;
+extra == "all" Requires-Dist: build; extra == "all" Requires-Dist: twine; extra
+== "all" [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/
+logo.png]# *docker-run* â ``docker run`` and ``docker exec`` with useful
+defaults
   [https://img.shields.io/github/license/ika-rwth-aachen/docker-run]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
              _d_m_/_d_o_c_k_e_r_-_r_u_n_-_c_l_i_?_c_o_l_o_r_=_b_l_u_e_&_l_a_b_e_l_=_P_y_P_I_%_2_0_d_o_w_n_l_o_a_d_s_]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments.
+arguments. > [!IMPORTANT] > This repository is open-sourced and maintained by
+the [**Institute for Automotive Engineering (ika) at RWTH Aachen University**]
+(https://www.ika.rwth-aachen.de/). > **DevOps, Containerization and
+Orchestration of Software-Defined Vehicles** are some of many research topics
+within our [*Vehicle Intelligence & Automated Driving*](https://www.ika.rwth-
+aachen.de/en/competences/fields-of-research/vehicle-intelligence-automated-
+driving.html) domain. > If you would like to learn more about how we can
+support your DevOps or automated driving efforts, feel free to reach out to us!
+>      *Timo Woopen - Manager Research Area Vehicle Intelligence & Automated
+Driving* >      *+49â¯241â¯80 23549* >      *timo.woopen@ika.rwth-aachen.de*
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_i_k_a_-_r_w_t_h_-
 _a_a_c_h_e_n_/_d_o_c_k_e_r_-_r_o_s_?_s_t_y_l_e_=_s_o_c_i_a_l_]- [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
@@ -53,20 +63,21 @@
 607qwq/xeyes ``` ## Functionality `docker-run` is designed to be used the same
 way as the official [`docker run`](https://docs.docker.com/engine/reference/
 commandline/run/) and [`docker exec`](https://docs.docker.com/engine/reference/
 commandline/exec/) commands. In general, you can pass the same arguments to
 `docker-run` as you would pass to `docker run`, e.g. ```bash docker-run --
 volume $(pwd):/volume ubuntu ls /volume ``` In addition to the arguments you
 are passing, `docker-run` however also enables the following features by
-default. Each of these default features can be disabled, see [Usage](#usage). -
+default. Most of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
-- current directory name as container name (`--name`) - GPU support (`--gpus
-all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
-name is already running, `docker-run` will execute a command in that container
-via `docker exec` instead. This lets you quickly attach to a running container
+- current directory name as container name (`--name`) - relative bind mounts
+(`--volume [./RELATIVE_PATH>]:[TARGET_PATH]`) - GPU support (`--gpus all` / `--
+runtime nvidia`) - X11 GUI forwarding If a container with matching name is
+already running, `docker-run` will execute a command in that container via
+`docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
 container ``` Unlike with `docker run`, you can also set the Docker image via
 the `--image` arguments, see [Usage](#usage). This may be required for more
 complex use cases. ## Installation ```bash pip install docker-run-cli #
 (optional) shell auto-completion source $(activate-python-docker-run-shell-
 completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
 *pip* may default to a user-site installation of executables to `~/.local/bin`,
```

### Comparing `docker-run-cli-0.9.6/src/docker_run_cli.egg-info/SOURCES.txt` & `docker-run-cli-0.9.7/src/docker_run_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

