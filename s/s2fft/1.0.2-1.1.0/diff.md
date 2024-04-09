# Comparing `tmp/s2fft-1.0.2.tar.gz` & `tmp/s2fft-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2fft-1.0.2.tar", last modified: Tue Mar  5 12:27:04 2024, max compression
+gzip compressed data, was "s2fft-1.1.0.tar", last modified: Tue Apr  9 07:56:03 2024, max compression
```

## Comparing `s2fft-1.0.2.tar` & `s2fft-1.1.0.tar`

### file list

```diff
@@ -1,173 +1,179 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.878355 s2fft-1.0.2/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3890 2024-03-04 10:08:08.000000 s2fft-1.0.2/.pip_readme.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1079 2023-12-07 10:38:57.000000 s2fft-1.0.2/LICENCE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      351 2023-12-07 10:38:57.000000 s2fft-1.0.2/MANIFEST.in
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4768 2024-03-05 12:27:04.877892 s2fft-1.0.2/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)    14818 2024-03-05 12:25:33.000000 s2fft-1.0.2/README.md
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.825323 s2fft-1.0.2/benchmarks/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.0.2/benchmarks/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10453 2023-12-07 10:38:57.000000 s2fft-1.0.2/benchmarks/benchmarking.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3183 2023-12-07 10:38:57.000000 s2fft-1.0.2/benchmarks/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3007 2023-12-07 10:38:57.000000 s2fft-1.0.2/benchmarks/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.826018 s2fft-1.0.2/docs/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      616 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/Makefile
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.826887 s2fft-1.0.2/docs/_static/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2099 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/MIT_Licence.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)      768 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/arxiv-logomark-small.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7906 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/codecov.png
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.827549 s2fft-1.0.2/docs/_static/css/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2801 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/css/custom.css
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1116 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/css/custom_tabs.css
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7676 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/_static/pypi.png
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.827892 s2fft-1.0.2/docs/api/
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.828482 s2fft-1.0.2/docs/api/base_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1000 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/base_transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      183 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/base_transforms/spin_spherical_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/base_transforms/wigner_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      558 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.829172 s2fft-1.0.2/docs/api/precompute_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      172 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/precompute_transforms/construct.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3063 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/api/precompute_transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      189 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/precompute_transforms/spin_spherical.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      174 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/precompute_transforms/wigner.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.830721 s2fft-1.0.2/docs/api/recursions/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6080 2024-02-20 10:53:24.000000 s2fft-1.0.2/docs/api/recursions/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      167 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/recursions/price_mcewen.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      151 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/recursions/risbo.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      159 2024-02-20 10:53:24.000000 s2fft-1.0.2/docs/api/recursions/risbo_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      155 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/recursions/trapani.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      160 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/recursions/turok.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/recursions/turok_jax.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.831268 s2fft-1.0.2/docs/api/sampling/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4419 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/sampling/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/sampling/spherical_samples.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/sampling/wigner_samples.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.831983 s2fft-1.0.2/docs/api/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2475 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/transforms/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/transforms/on_the_fly_recursions.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/transforms/spin_spherical_transform.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      163 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/transforms/wigner.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.834254 s2fft-1.0.2/docs/api/utility/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      165 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/healpix_ffts.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7400 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/api/utility/index.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      139 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/logs.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/quadrature.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/quadrature_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/api/utility/quadrature_torch.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/resampling.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/resampling_jax.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/api/utility/resampling_torch.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      153 2024-02-20 10:53:24.000000 s2fft-1.0.2/docs/api/utility/rotation.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/signal_generator.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      140 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/api/utility/utils.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.836375 s2fft-1.0.2/docs/assets/
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.841543 s2fft-1.0.2/docs/assets/authors/
--rw-r--r--   0 cosmomatt   (503) staff       (20)    17823 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/authors/gopinathan.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    76930 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/authors/graham.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    16624 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/authors/mcewen.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    40335 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/authors/minano.jpeg
--rw-r--r--   0 cosmomatt   (503) staff       (20)    20411 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/authors/price.jpeg
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.859155 s2fft-1.0.2/docs/assets/figures/
--rw-r--r--   0 cosmomatt   (503) staff       (20)   818639 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/Wigner_recursion_github_docs.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   818295 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/Wigner_recursion_legend_darkmode.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)  1397896 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/sax_schematic_github_docs.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)  1386068 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/sax_schematic_legend_darkmode.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   552260 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/schematic.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   232599 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/software_overview.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   205989 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/spherical_sampling.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   285599 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/spin_spherical_mw.pdf
--rw-r--r--   0 cosmomatt   (503) staff       (20)   372503 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/spin_spherical_mw.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   339446 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/wigner_mw.pdf
--rw-r--r--   0 cosmomatt   (503) staff       (20)   537199 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/figures/wigner_mw.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   698556 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/sax_logo.png
--rw-r--r--   0 cosmomatt   (503) staff       (20)   198825 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/assets/sax_logo.svg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6397 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/conf.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10782 2024-03-05 12:25:33.000000 s2fft-1.0.2/docs/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.861409 s2fft-1.0.2/docs/tutorials/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4574 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/tutorials/index.rst
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.861717 s2fft-1.0.2/docs/tutorials/rotation/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       61 2024-02-20 10:53:24.000000 s2fft-1.0.2/docs/tutorials/rotation/rotation.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.862015 s2fft-1.0.2/docs/tutorials/spherical_harmonic/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       71 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/tutorials/spherical_harmonic/spherical_harmonic_transform.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.862302 s2fft-1.0.2/docs/tutorials/torch_frontend/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       57 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/tutorials/torch_frontend/torch_frontend.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.862579 s2fft-1.0.2/docs/tutorials/wigner/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       59 2023-12-07 10:38:57.000000 s2fft-1.0.2/docs/tutorials/wigner/wigner_transform.nblink
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.862804 s2fft-1.0.2/docs/user_guide/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3011 2024-03-04 10:08:08.000000 s2fft-1.0.2/docs/user_guide/install.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      116 2023-12-07 11:29:29.000000 s2fft-1.0.2/pytest.ini
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.865182 s2fft-1.0.2/requirements/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      147 2024-03-05 12:25:33.000000 s2fft-1.0.2/requirements/requirements-core.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)      290 2024-01-30 16:57:46.000000 s2fft-1.0.2/requirements/requirements-docs.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       81 2023-12-07 10:38:57.000000 s2fft-1.0.2/requirements/requirements-plotting.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       75 2023-12-07 10:38:57.000000 s2fft-1.0.2/requirements/requirements-tests.txt
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.866288 s2fft-1.0.2/s2fft/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2404 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/README.rst
--rw-r--r--   0 cosmomatt   (503) staff       (20)      570 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)      426 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/_version.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.867607 s2fft-1.0.2/s2fft/base_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       45 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/base_transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    31229 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/base_transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5570 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/base_transforms/wigner.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1513 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/default-logging-config.yaml
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2297 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/logs.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.868346 s2fft-1.0.2/s2fft/precompute_transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       69 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/precompute_transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11236 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/precompute_transforms/construct.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    16458 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/precompute_transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    20375 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/precompute_transforms/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.870082 s2fft-1.0.2/s2fft/recursions/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-02-20 10:53:24.000000 s2fft-1.0.2/s2fft/recursions/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    22422 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/recursions/price_mcewen.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3821 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/recursions/risbo.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3745 2024-02-20 10:53:24.000000 s2fft-1.0.2/s2fft/recursions/risbo_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    23578 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/recursions/trapani.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    13852 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/recursions/turok.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9333 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/recursions/turok_jax.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.870658 s2fft-1.0.2/s2fft/sampling/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       51 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/sampling/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    25532 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/sampling/s2_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     7720 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/sampling/so3_samples.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.871660 s2fft-1.0.2/s2fft/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)       74 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    32077 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/transforms/otf_recursions.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    23364 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/transforms/spherical.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24895 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/transforms/wigner.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.874313 s2fft-1.0.2/s2fft/utils/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      251 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/utils/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    21892 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/utils/healpix_ffts.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     8678 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/utils/quadrature.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9883 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/utils/quadrature_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9211 2024-03-05 12:25:33.000000 s2fft-1.0.2/s2fft/utils/quadrature_torch.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11542 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/utils/resampling.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    12362 2023-12-07 10:38:57.000000 s2fft-1.0.2/s2fft/utils/resampling_jax.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11759 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/utils/resampling_torch.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2924 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/utils/rotation.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3415 2024-03-04 10:08:08.000000 s2fft-1.0.2/s2fft/utils/signal_generator.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.877487 s2fft-1.0.2/s2fft.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4768 2024-03-05 12:27:04.000000 s2fft-1.0.2/s2fft.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4391 2024-03-05 12:27:04.000000 s2fft-1.0.2/s2fft.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-03-05 12:27:04.000000 s2fft-1.0.2/s2fft.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       68 2024-03-05 12:27:04.000000 s2fft-1.0.2/s2fft.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       23 2024-03-05 12:27:04.000000 s2fft-1.0.2/s2fft.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-03-05 12:27:04.878439 s2fft-1.0.2/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1229 2024-03-04 10:08:08.000000 s2fft-1.0.2/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-03-05 12:27:04.877161 s2fft-1.0.2/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.0.2/tests/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1909 2023-12-07 10:38:57.000000 s2fft-1.0.2/tests/conftest.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1489 2024-03-04 10:08:08.000000 s2fft-1.0.2/tests/test_healpix_ffts.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)      497 2023-12-07 10:38:57.000000 s2fft-1.0.2/tests/test_logs.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1468 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_quadrature.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3487 2023-12-07 10:38:57.000000 s2fft-1.0.2/tests/test_resampling.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3758 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4838 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_spherical_base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5897 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_spherical_custom_grads.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6697 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_spherical_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     5024 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_spherical_transform.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     3770 2024-03-04 10:08:08.000000 s2fft-1.0.2/tests/test_utils.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2955 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_wigner_base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2465 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_wigner_custom_grads.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6643 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_wigner_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     8248 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_wigner_recursions.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2435 2023-12-07 10:38:57.000000 s2fft-1.0.2/tests/test_wigner_samples.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     2999 2024-03-05 12:25:33.000000 s2fft-1.0.2/tests/test_wigner_transform.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.398958 s2fft-1.1.0/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4271 2024-04-09 07:43:48.000000 s2fft-1.1.0/.pip_readme.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1079 2023-12-07 10:38:57.000000 s2fft-1.1.0/LICENCE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      351 2023-12-07 10:38:57.000000 s2fft-1.1.0/MANIFEST.in
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-09 07:56:03.398647 s2fft-1.1.0/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    16828 2024-04-09 07:43:48.000000 s2fft-1.1.0/README.md
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.345249 s2fft-1.1.0/benchmarks/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10453 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/benchmarking.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3183 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3007 2023-12-07 10:38:57.000000 s2fft-1.1.0/benchmarks/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.346021 s2fft-1.1.0/docs/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      616 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/Makefile
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347142 s2fft-1.1.0/docs/_static/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2099 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/MIT_Licence.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      768 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/arxiv-logomark-small.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7906 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/codecov.png
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347602 s2fft-1.1.0/docs/_static/css/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2801 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1116 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/css/custom_tabs.css
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7676 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/_static/pypi.png
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.347778 s2fft-1.1.0/docs/api/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.348369 s2fft-1.1.0/docs/api/base_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1000 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      183 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/spin_spherical_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/base_transforms/wigner_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      558 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.349224 s2fft-1.1.0/docs/api/precompute_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      172 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/construct.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3063 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/precompute_transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      189 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/spin_spherical.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      174 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/precompute_transforms/wigner.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.350908 s2fft-1.1.0/docs/api/recursions/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6080 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/recursions/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      167 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/price_mcewen.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      151 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/risbo.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      159 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/recursions/risbo_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      155 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/trapani.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      160 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/turok.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/recursions/turok_jax.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.351380 s2fft-1.1.0/docs/api/sampling/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4419 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/spherical_samples.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/sampling/wigner_samples.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.352705 s2fft-1.1.0/docs/api/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/api/transforms/c_backend_spherical.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3458 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/api/transforms/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      184 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/transforms/on_the_fly_recursions.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      178 2024-04-07 08:49:16.000000 s2fft-1.1.0/docs/api/transforms/spin_spherical_transform.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      163 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/transforms/wigner.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.355016 s2fft-1.1.0/docs/api/utility/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      165 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/healpix_ffts.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7400 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/index.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      139 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/logs.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/quadrature.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/quadrature_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/quadrature_torch.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      156 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/resampling.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      164 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/resampling_jax.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/api/utility/resampling_torch.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      153 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/api/utility/rotation.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      168 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/signal_generator.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      140 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/api/utility/utils.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.356707 s2fft-1.1.0/docs/assets/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.358733 s2fft-1.1.0/docs/assets/authors/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    17823 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/gopinathan.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    76930 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/graham.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    16624 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/mcewen.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    40335 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/minano.jpeg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    20411 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/authors/price.jpeg
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.378533 s2fft-1.1.0/docs/assets/figures/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   818639 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/Wigner_recursion_github_docs.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   818295 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/Wigner_recursion_legend_darkmode.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)  1397896 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/sax_schematic_github_docs.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)  1386068 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/sax_schematic_legend_darkmode.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   552260 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/schematic.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   232599 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/software_overview.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   336240 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/assets/figures/spherical_sampling.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   285599 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.pdf
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   372503 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   339446 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/wigner_mw.pdf
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   537199 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/figures/wigner_mw.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   698556 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/sax_logo.png
+-rw-r--r--   0 cosmomatt   (503) staff       (20)   198825 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/assets/sax_logo.svg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6425 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/conf.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11384 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.379732 s2fft-1.1.0/docs/tutorials/
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380006 s2fft-1.1.0/docs/tutorials/JAX_HEALPix/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       63 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/JAX_HEALPix/JAX_HEALPix_frontend.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380407 s2fft-1.1.0/docs/tutorials/JAX_SSHT/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       60 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/JAX_SSHT/JAX_SSHT_frontend.nblink
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3340 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/tutorials/index.rst
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380643 s2fft-1.1.0/docs/tutorials/rotation/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       61 2024-02-20 10:53:24.000000 s2fft-1.1.0/docs/tutorials/rotation/rotation.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.380935 s2fft-1.1.0/docs/tutorials/spherical_harmonic/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       71 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/tutorials/spherical_harmonic/spherical_harmonic_transform.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381340 s2fft-1.1.0/docs/tutorials/torch_frontend/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       57 2024-03-04 10:08:08.000000 s2fft-1.1.0/docs/tutorials/torch_frontend/torch_frontend.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381685 s2fft-1.1.0/docs/tutorials/wigner/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       59 2023-12-07 10:38:57.000000 s2fft-1.1.0/docs/tutorials/wigner/wigner_transform.nblink
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.381964 s2fft-1.1.0/docs/user_guide/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2960 2024-04-09 07:43:48.000000 s2fft-1.1.0/docs/user_guide/install.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      116 2023-12-07 11:29:29.000000 s2fft-1.1.0/pytest.ini
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.382946 s2fft-1.1.0/requirements/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      166 2024-04-09 07:43:48.000000 s2fft-1.1.0/requirements/requirements-core.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      290 2024-01-30 16:57:46.000000 s2fft-1.1.0/requirements/requirements-docs.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       81 2023-12-07 10:38:57.000000 s2fft-1.1.0/requirements/requirements-plotting.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       79 2024-04-09 07:43:48.000000 s2fft-1.1.0/requirements/requirements-tests.txt
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.384197 s2fft-1.1.0/s2fft/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2404 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/README.rst
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      570 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      412 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/_version.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.385897 s2fft-1.1.0/s2fft/base_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       45 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/base_transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    31229 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/base_transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5570 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/base_transforms/wigner.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1513 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/default-logging-config.yaml
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2297 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/logs.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.386621 s2fft-1.1.0/s2fft/precompute_transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       69 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/precompute_transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11236 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/construct.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    16458 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    20375 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/precompute_transforms/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.388174 s2fft-1.1.0/s2fft/recursions/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-02-20 10:53:24.000000 s2fft-1.1.0/s2fft/recursions/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    22422 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/price_mcewen.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3821 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/recursions/risbo.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3745 2024-02-20 10:53:24.000000 s2fft-1.1.0/s2fft/recursions/risbo_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    23578 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/trapani.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    13852 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/turok.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9333 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/recursions/turok_jax.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.389048 s2fft-1.1.0/s2fft/sampling/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       51 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/sampling/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    25532 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/sampling/s2_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     7720 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/sampling/so3_samples.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.390435 s2fft-1.1.0/s2fft/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      108 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11670 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/c_backend_spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    32077 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/transforms/otf_recursions.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24969 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/spherical.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    32303 2024-04-09 07:43:48.000000 s2fft-1.1.0/s2fft/transforms/wigner.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.392844 s2fft-1.1.0/s2fft/utils/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      251 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    21892 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/healpix_ffts.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     8678 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9883 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9211 2024-03-05 12:25:33.000000 s2fft-1.1.0/s2fft/utils/quadrature_torch.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11542 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/utils/resampling.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    12362 2023-12-07 10:38:57.000000 s2fft-1.1.0/s2fft/utils/resampling_jax.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11759 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/resampling_torch.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2924 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/rotation.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3415 2024-03-04 10:08:08.000000 s2fft-1.1.0/s2fft/utils/signal_generator.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.398173 s2fft-1.1.0/s2fft.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5153 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4579 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       73 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       23 2024-04-09 07:56:03.000000 s2fft-1.1.0/s2fft.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-09 07:56:03.399009 s2fft-1.1.0/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1188 2024-04-09 07:43:48.000000 s2fft-1.1.0/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 07:56:03.397926 s2fft-1.1.0/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1909 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/conftest.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1489 2024-03-04 10:08:08.000000 s2fft-1.1.0/tests/test_healpix_ffts.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      497 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_logs.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1468 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_quadrature.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3487 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_resampling.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3758 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4838 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_spherical_base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10252 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_spherical_custom_grads.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6697 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_spherical_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6590 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_spherical_transform.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     3770 2024-03-04 10:08:08.000000 s2fft-1.1.0/tests/test_utils.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2955 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5075 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_wigner_custom_grads.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6643 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     8248 2024-03-05 12:25:33.000000 s2fft-1.1.0/tests/test_wigner_recursions.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     2435 2023-12-07 10:38:57.000000 s2fft-1.1.0/tests/test_wigner_samples.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     5183 2024-04-09 07:43:48.000000 s2fft-1.1.0/tests/test_wigner_transform.py
```

### Comparing `s2fft-1.0.2/.pip_readme.rst` & `s2fft-1.1.0/.pip_readme.rst`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
     :target: https://opensource.org/licenses/MIT
 .. image:: http://img.shields.io/badge/arXiv-2311.14670-orange.svg?style=flat
     :target: https://arxiv.org/abs/2311.14670
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
-    :target: https://colab.research.google.com/drive/1YmJ2ljsF8HBvhPmD4hrYPlyAKc4WPUgq?usp=sharing
+    :target: https://colab.research.google.com/github/astro-informatics/s2fft/blob/main/notebooksspherical_harmonic_transform.ipynb
 
 Differentiable and accelerated spherical transforms
 =================================================================================================================
 
 `S2FFT` is a Python package for computing Fourier transforms on the sphere
 and rotation group using JAX and PyTorch. It leverages autodiff to provide differentiable
 transforms, which are also deployable on hardware accelerators
@@ -27,14 +27,20 @@
 optimisations (precompute or not) that one may select depending on
 available resources and desired angular resolution $L$.
 
 As of version 1.0.2 `S2FFT` also provides PyTorch implementations of underlying 
 precompute transforms. In future releases this support will be extended to our 
 on-the-fly algorithms.
 
+As of version 1.1.0 `S2FFT` also provides JAX support for existing C/C++ packages, 
+specifically `HEALPix` and `SSHT`. This works by wrapping python bindings with custom 
+JAX frontends. Note that currently this C/C++ to JAX interoperability is currently 
+limited to CPU, however for many applications this is desirable due to memory 
+constraints.
+
 Documentation
 =============
 Read the full documentation `here <https://astro-informatics.github.io/s2fft/>`_.
 
 Attribution
 ===========
 Should this code be used in any way, we kindly request that the following article is
```

### Comparing `s2fft-1.0.2/LICENCE.txt` & `s2fft-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/PKG-INFO` & `s2fft-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2fft
-Version: 1.0.2
+Version: 1.1.0
 Summary: Differentiable and accelerated spherical transforms with JAX
 Home-page: https://github.com/astro-informatics/s2fft
 Author: Matthew A. Price, Jason D. McEwen & Contributors
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,31 +17,32 @@
 License-File: LICENCE.txt
 Requires-Dist: numpy>=1.20
 Requires-Dist: colorlog
 Requires-Dist: pyyaml
 Requires-Dist: jax>=0.3.13
 Requires-Dist: jaxlib
 Requires-Dist: torch
-Provides-Extra: torch
-Requires-Dist: torch; extra == "torch"
+Requires-Dist: pyssht
+Requires-Dist: healpy
+Requires-Dist: ducc0
 
 .. image:: https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml
 .. image:: https://img.shields.io/badge/GitHub-s2fft-brightgreen.svg?style=flat
     :target: https://github.com/astro-informatics/s2fft
 .. image:: https://codecov.io/gh/astro-informatics/s2fft/branch/main/graph/badge.svg?token=7QYAFAAWLE
     :target: https://codecov.io/gh/astro-informatics/s2fft
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
     :target: https://opensource.org/licenses/MIT
 .. image:: http://img.shields.io/badge/arXiv-2311.14670-orange.svg?style=flat
     :target: https://arxiv.org/abs/2311.14670
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
-    :target: https://colab.research.google.com/drive/1YmJ2ljsF8HBvhPmD4hrYPlyAKc4WPUgq?usp=sharing
+    :target: https://colab.research.google.com/github/astro-informatics/s2fft/blob/main/notebooksspherical_harmonic_transform.ipynb
 
 Differentiable and accelerated spherical transforms
 =================================================================================================================
 
 `S2FFT` is a Python package for computing Fourier transforms on the sphere
 and rotation group using JAX and PyTorch. It leverages autodiff to provide differentiable
 transforms, which are also deployable on hardware accelerators
@@ -53,14 +54,20 @@
 optimisations (precompute or not) that one may select depending on
 available resources and desired angular resolution $L$.
 
 As of version 1.0.2 `S2FFT` also provides PyTorch implementations of underlying 
 precompute transforms. In future releases this support will be extended to our 
 on-the-fly algorithms.
 
+As of version 1.1.0 `S2FFT` also provides JAX support for existing C/C++ packages, 
+specifically `HEALPix` and `SSHT`. This works by wrapping python bindings with custom 
+JAX frontends. Note that currently this C/C++ to JAX interoperability is currently 
+limited to CPU, however for many applications this is desirable due to memory 
+constraints.
+
 Documentation
 =============
 Read the full documentation `here <https://astro-informatics.github.io/s2fft/>`_.
 
 Attribution
 ===========
 Should this code be used in any way, we kindly request that the following article is
```

### Comparing `s2fft-1.0.2/README.md` & `s2fft-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![image](https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml)
 [![image](https://codecov.io/gh/astro-informatics/s2fft/branch/main/graph/badge.svg?token=7QYAFAAWLE)](https://codecov.io/gh/astro-informatics/s2fft)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![image](https://badge.fury.io/py/s2fft.svg)](https://badge.fury.io/py/s2fft)
 [![image](http://img.shields.io/badge/arXiv-2311.14670-orange.svg?style=flat)](https://arxiv.org/abs/2311.14670)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors-)<!-- ALL-CONTRIBUTORS-BADGE:END --> 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YmJ2ljsF8HBvhPmD4hrYPlyAKc4WPUgq?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/astro-informatics/s2fft/blob/main/notebooks/spherical_harmonic_transform.ipynb)
 <!-- [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) -->
 
 <img align="left" height="85" width="98" src="./docs/assets/sax_logo.png">
 
 # Differentiable and accelerated spherical transforms
 
 `S2FFT` is a Python package for computing Fourier transforms on the sphere
@@ -18,18 +18,28 @@
 
 More specifically, `S2FFT` provides support for spin spherical harmonic
 and Wigner transforms (for both real and complex signals), with support
 for adjoint transformations where needed, and comes with different
 optimisations (precompute or not) that one may select depending on
 available resources and desired angular resolution $L$.
 
+> [!IMPORTANT]
+> HEALPix long JIT compile time fixed for CPU!  Fix for GPU coming soon.
+
+> [!TIP]
 As of version 1.0.2 `S2FFT` also provides PyTorch implementations of underlying 
 precompute transforms. In future releases this support will be extended to our 
 on-the-fly algorithms.
 
+> [!TIP]
+As of version 1.1.0 `S2FFT` also provides JAX support for existing C/C++ packages, 
+specifically `HEALPix` and `SSHT`. This works by wrapping python bindings with custom 
+JAX frontends. Note that currently this C/C++ to JAX interoperability is currently 
+limited to CPU.
+
 ## Algorithms :zap:
 
 `S2FFT` leverages new algorithmic structures that can he highly
 parallelised and distributed, and so map very well onto the architecture
 of hardware accelerators (i.e. GPUs and TPUs). In particular, these
 algorithms are based on new Wigner-d recursions that are stable to high
 angular resolution $L$. The diagram below illustrates the recursions
@@ -49,15 +59,15 @@
 (for further details see Price & McEwen, in prep.).
 
 ![image](./docs/assets/figures/sax_schematic_legend_darkmode.png)
 
 ## Sampling :earth_africa:
 
 The structure of the algorithms implemented in `S2FFT` can support any
-isolattitude sampling scheme. A number of sampling schemes are currently
+isolatitude sampling scheme. A number of sampling schemes are currently
 supported.
 
 The equiangular sampling schemes of [McEwen & Wiaux
 (2012)](https://arxiv.org/abs/1110.6298), [Driscoll & Healy
 (1995)](https://www.sciencedirect.com/science/article/pii/S0196885884710086) 
 and [Gauss-Legendre (1986)](https://link.springer.com/article/10.1007/BF02519350)
 are supported, which exhibit associated sampling theorems and so
@@ -69,52 +79,53 @@
 The popular [HEALPix](https://healpix.jpl.nasa.gov) sampling scheme
 ([Gorski et al. 2005](https://arxiv.org/abs/astro-ph/0409513)) is also
 supported. The HEALPix sampling does not exhibit a sampling theorem and
 so the corresponding harmonic transforms do not achieve machine
 precision but exhibit some error. However, the HEALPix sampling provides
 pixels of equal areas, which has many practical advantages.
 
-<p align="center"><img src="./docs/assets/figures/spherical_sampling.png" width="500"></p>
+<p align="center"><img src="./docs/assets/figures/spherical_sampling.png" width="700"></p>
 
 > [!NOTE]  
-> For algorithmic reasons JIT compilation of HEALPix transforms can become slow at high bandlimits, due to XLA unfolding of loops which currently cannot be avoided. After compiling HEALPix transforms should execute with the efficiency outlined in the associated paper, therefore this additional time overhead need only be incurred once. We are aware of this issue and will work to improve this in subsequent versions.
+> For algorithmic reasons JIT compilation of HEALPix transforms can become slow at high bandlimits, due to XLA unfolding of loops which currently cannot be avoided. After compiling HEALPix transforms should execute with the efficiency outlined in the associated paper, therefore this additional time overhead need only be incurred once. We are aware of this issue and are working to fix it.  A fix for CPU execution has now been implemented (see example [notebook](https://astro-informatics.github.io/s2fft/tutorials/spherical_harmonic/JAX_HEALPix_backend.html)).  Fix for GPU execution is coming soon.
 
 ## Installation :computer:
 
 The Python dependencies for the `S2FFT` package are listed in the file
 `requirements/requirements-core.txt` and will be automatically installed
 into the active python environment by [pip](https://pypi.org) when running
 
 ``` bash
 pip install s2fft
 ```
-This will install all core functionality which includes JAX support. To install `S2FFT` 
-with PyTorch support run 
-
-``` bash
-pip install s2fft[torch]
-```
+This will install all core functionality which includes JAX support (including PyTorch support).
 
 Alternatively, the `S2FFT` package may be installed directly from GitHub by cloning this 
 repository and then running 
 
 ``` bash
 pip install .        
 ```
 
-from the root directory of the repository. To enable PyTorch support you will need to run 
+from the root directory of the repository. 
+
+Unit tests can then be executed to ensure the installation was successful by first installing the test requirements and then running pytest
 
 ``` bash
-pip install .[torch]     
+pip install -r requirements/requirements-tests.txt
+pytest tests/  
 ```
 
-Unit tests can then be executed to ensure the installation was successful by running
+Documentation for the released version is available [here](https://astro-informatics.github.io/s2fft/).  To build the documentation locally run
 
 ``` bash
-pytest tests/  
+pip install -r requirements/requirements-docs.txt
+cd docs 
+make html
+open _build/html/index.html
 ```
 
 > [!NOTE]  
 > For plotting functionality which can be found throughout our various notebooks, one must install the requirements which can be found in `requirements/requirements-plotting.txt`.
 
 ## Usage :rocket:
 
@@ -139,15 +150,37 @@
 ```
 
 For further details on usage see the [documentation](https://astro-informatics.github.io/s2fft/) and associated [notebooks](https://astro-informatics.github.io/s2fft/tutorials/spherical_harmonic/spherical_harmonic_transform.html).
 
 > [!NOTE]  
 > We also provide PyTorch support for the precompute version of our transforms. These are called through forward/inverse_torch(). Full PyTorch support will be provided in future releases.
 
-## Benchmarking :hourglass_flowing_sand:
+## C/C++ JAX Frontends for SSHT/HEALPix :bulb:
+
+`S2FFT` also provides JAX support for existing C/C++ packages, specifically [`HEALPix`](https://healpix.jpl.nasa.gov) and [`SSHT`](https://github.com/astro-informatics/ssht). This works 
+by wrapping python bindings with custom JAX frontends. Note that this C/C++ to JAX interoperability is currently limited to CPU.
+
+For example, one may call these alternate backends for the spherical harmonic transform by:
+
+``` python
+# Forward SSHT spherical harmonic transform
+flm = s2fft.forward(f, L, sampling=["mw"], method="jax_ssht")  
+
+# Forward HEALPix spherical harmonic transform
+flm = s2fft.forward(f, L, nside=nside, sampling="healpix", method="jax_healpy")  
+```
+
+All of these JAX frontends supports out of the box reverse mode automatic differentiation, 
+and under the hood is simply linking to the C/C++ packages you are familiar with. In this 
+way `S2fft` enhances existing packages with gradient functionality for modern scientific computing or machine learning 
+applications!
+
+For further details on usage see the associated [notebooks](https://astro-informatics.github.io/s2fft/tutorials/spherical_harmonic/JAX_SSHT_backend.html).
+
+<!-- ## Benchmarking :hourglass_flowing_sand:
 
 We benchmarked the spherical harmonic and Wigner transforms implemented
 in `S2FFT` against the C implementations in the
 [SSHT](https://github.com/astro-informatics/ssht) package.
 
 A brief summary is shown in the table below for the recursion (left) and
 precompute (right) algorithms, with `S2FFT` running on GPUs (for further
@@ -163,15 +196,15 @@
 | 512  | 58.3 ms   | 11.4     | 1.43E-14 | 3.6 ms    | 184      | 1.37E-14 | 2.14 GB |
 | 1024 | 194 ms    | 32.9     | 2.69E-14 | 32.6 ms   | 195      | 2.47E-14 | 17.1 GB |
 | 2048 | 1.44 s    | 49.7     | 5.17E-14 | N/A       | N/A      | N/A      | N/A     |
 | 4096 | 8.48 s    | 133.9    | 1.06E-13 | N/A       | N/A      | N/A      | N/A     |
 | 8192 | 82 s      | 110.8    | 2.14E-13 | N/A       | N/A      | N/A      | N/A     |
 
 where the left hand results are for the recursive based algorithm and the right hand side are 
-our precompute implementation.
+our precompute implementation. -->
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji
 key](https://allcontributors.org/docs/en/emoji-key)):
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

### Comparing `s2fft-1.0.2/benchmarks/benchmarking.py` & `s2fft-1.1.0/benchmarks/benchmarking.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/benchmarks/spherical.py` & `s2fft-1.1.0/benchmarks/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/benchmarks/wigner.py` & `s2fft-1.1.0/benchmarks/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/Makefile` & `s2fft-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/MIT_Licence.png` & `s2fft-1.1.0/docs/_static/MIT_Licence.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/arxiv-logomark-small.png` & `s2fft-1.1.0/docs/_static/arxiv-logomark-small.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/codecov.png` & `s2fft-1.1.0/docs/_static/codecov.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/css/custom.css` & `s2fft-1.1.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/css/custom_tabs.css` & `s2fft-1.1.0/docs/_static/css/custom_tabs.css`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/_static/pypi.png` & `s2fft-1.1.0/docs/_static/pypi.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/base_transforms/index.rst` & `s2fft-1.1.0/docs/api/base_transforms/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/index.rst` & `s2fft-1.1.0/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/precompute_transforms/index.rst` & `s2fft-1.1.0/docs/api/precompute_transforms/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/recursions/index.rst` & `s2fft-1.1.0/docs/api/recursions/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/sampling/index.rst` & `s2fft-1.1.0/docs/api/sampling/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/api/transforms/index.rst` & `s2fft-1.1.0/docs/api/transforms/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,33 @@
    * - :func:`~s2fft.transforms.wigner.forward`
      - Wrapper function around NumPy/JAX forward methods
    * - :func:`~s2fft.transforms.wigner.forward_numpy`
      - Forward Wigner transform (NumPy)
    * - :func:`~s2fft.transforms.wigner.forward_jax`
      - Forward Wigner transform (JAX)
 
+.. list-table:: C/C++ backend gradient support
+   :widths: 25 25
+   :header-rows: 1
+
+   * - Function Name
+     - Description
+   * - :func:`~s2fft.transforms.c_backend_spherical.ssht_inverse`
+     - Custom JAX frontend for inverse SSHT C spherical harmonic library.
+   * - :func:`~s2fft.transforms.c_backend_spherical.ssht_forward`
+     - Custom JAX frontend for forward SSHT C spherical harmonic library.
+   * - :func:`~s2fft.transforms.c_backend_spherical.healpy_inverse`
+     - Custom JAX frontend for inverse HEALPix C++ spherical harmonic library.
+   * - :func:`~s2fft.transforms.c_backend_spherical.healpy_forward`
+     - Custom JAX frontend for forwardHEALPix C++ spherical harmonic library.
+   * - :func:`~s2fft.transforms.wigner.inverse_jax_ssht`
+     - Custom JAX frontend for hybrid inverse SSHT C Wigner transforms.
+   * - :func:`~s2fft.transforms.wigner.forward_jax_ssht`
+     - Custom JAX frontend for hybrid forward SSHT C Wigner transforms.
+
 .. list-table:: On-the-fly Price-McEwen recursions.
    :widths: 25 25
    :header-rows: 1
 
    * - Function Name
      - Description
    * - :func:`~s2fft.transforms.otf_recursions.inverse_latitudinal_step`
@@ -60,8 +79,9 @@
    :hidden:
    :maxdepth: 3
    :caption: Transforms
 
    on_the_fly_recursions
    spin_spherical_transform
    wigner
+  ..  c_backend_spherical
```

### Comparing `s2fft-1.0.2/docs/api/utility/index.rst` & `s2fft-1.1.0/docs/api/utility/index.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/authors/gopinathan.jpeg` & `s2fft-1.1.0/docs/assets/authors/gopinathan.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/authors/graham.jpeg` & `s2fft-1.1.0/docs/assets/authors/graham.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/authors/mcewen.jpeg` & `s2fft-1.1.0/docs/assets/authors/mcewen.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/authors/minano.jpeg` & `s2fft-1.1.0/docs/assets/authors/minano.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/authors/price.jpeg` & `s2fft-1.1.0/docs/assets/authors/price.jpeg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/Wigner_recursion_github_docs.png` & `s2fft-1.1.0/docs/assets/figures/Wigner_recursion_github_docs.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/Wigner_recursion_legend_darkmode.png` & `s2fft-1.1.0/docs/assets/figures/Wigner_recursion_legend_darkmode.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/sax_schematic_github_docs.png` & `s2fft-1.1.0/docs/assets/figures/sax_schematic_github_docs.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/sax_schematic_legend_darkmode.png` & `s2fft-1.1.0/docs/assets/figures/sax_schematic_legend_darkmode.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/schematic.png` & `s2fft-1.1.0/docs/assets/figures/schematic.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/software_overview.png` & `s2fft-1.1.0/docs/assets/figures/software_overview.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/spin_spherical_mw.pdf` & `s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.pdf`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/spin_spherical_mw.png` & `s2fft-1.1.0/docs/assets/figures/spin_spherical_mw.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/wigner_mw.pdf` & `s2fft-1.1.0/docs/assets/figures/wigner_mw.pdf`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/figures/wigner_mw.png` & `s2fft-1.1.0/docs/assets/figures/wigner_mw.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/sax_logo.png` & `s2fft-1.1.0/docs/assets/sax_logo.png`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/assets/sax_logo.svg` & `s2fft-1.1.0/docs/assets/sax_logo.svg`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/docs/conf.py` & `s2fft-1.1.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # -- Project information -----------------------------------------------------
 
 project = "S2FFT"
 copyright = "2023, Matthew Price and Jason McEwen"
 author = "Matthew Price, Jason McEwen, Matthew Graham, Sofia Miñano, Devaraj Gopinathan"
 
 # The short X.Y version
-version = "1.0.2"
+version = "1.1.0"
 # The full version, including alpha/beta/rc tags
-release = "1.0.2"
+release = "1.1.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
@@ -102,20 +102,20 @@
     "icon_links": [
         {
             "name": "ArXiv",
             "url": "https://arxiv.org/abs/2311.14670",
             "icon": "_static/arxiv-logomark-small.png",
             "type": "local",
         },
-        # {
-        #     "name": "YouTube",
-        #     "url": "https://www.youtube.com/channel/UCrCOQsyQOJhOUaIYzmbkKQQ",
-        #     "icon": "fa-brands fa-youtube fa-2x",
-        #     "type": "fontawesome",
-        # },
+        {
+            "name": "Medium",
+            "url": "https://towardsdatascience.com/differentiable-and-accelerated-spherical-harmonic-transforms-c269393d08f1",
+            "icon": "fa-brands fa-medium",
+            "type": "fontawesome",
+        },
         {
             "name": "PyPi",
             "url": "https://pypi.org/project/s2fft/",
             "icon": "_static/pypi.png",
             "type": "local",
         },
         {
```

### Comparing `s2fft-1.0.2/docs/index.rst` & `s2fft-1.1.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,27 @@
 deployable on modern hardware accelerators (e.g. GPUs and TPUs).
 
 More specifically, ``S2FFT`` provides support for spin spherical harmonic and Wigner
 transforms (for both real and complex signals), with support for adjoint transformations
 where needed, and comes with different optimisations (precompute or not) that one
 may select depending on available resources and desired angular resolution :math:`L`.
 
-As of version 1.0.2 ``S2FFT`` also provides PyTorch implementations of underlying 
-precompute transforms. In future releases this support will be extended to our 
-on-the-fly algorithms.
+.. important::
+    HEALPix long JIT compile time fixed for CPU!  Fix for GPU coming soon.
+
+.. tip::
+    As of version 1.0.2 ``S2FFT`` also provides PyTorch implementations of underlying 
+    precompute transforms. In future releases this support will be extended to our 
+    on-the-fly algorithms.
+
+.. tip::
+    As of version 1.1.0 ``S2FFT`` also provides JAX support for existing C/C++ packages, 
+    specifically ``HEALPix`` and ``SSHT``. This works by wrapping python bindings with custom 
+    JAX frontends. Note that currently this C/C++ to JAX interoperability is currently 
+    limited to CPU.
 
 Algorithms |:zap:|
 -------------------
 
 ``S2FFT`` leverages new algorithmic structures that can he highly parallelised and
 distributed, and so map very well onto the architecture of hardware accelerators (i.e.
 GPUs and TPUs).  In particular, these algorithms are based on new Wigner-d recursions
@@ -36,28 +46,28 @@
 computing only a portion of the projection at a time, hence incurring 
 negligible memory overhead at the cost of slightly slower execution. The 
 diagram below illustrates the separable spherical harmonic transform.
 
 .. image:: ./assets/figures/sax_schematic_github_docs.png
 
 .. note::
-    For algorithmic reasons JIT compilation of HEALPix transforms can become slow at high bandlimits, due to XLA unfolding of loops which currently cannot be avoided. After compiling HEALPix transforms should execute with the efficiency outlined in the associated paper, therefore this additional time overhead need only be incurred once. We are aware of this issue and will work to improve this in subsequent versions.
+    For algorithmic reasons JIT compilation of HEALPix transforms can become slow at high bandlimits, due to XLA unfolding of loops which currently cannot be avoided. After compiling HEALPix transforms should execute with the efficiency outlined in the associated paper, therefore this additional time overhead need only be incurred once. We are aware of this issue and are working to fix it.  A fix for CPU execution has now been implemented (see example `notebook <https://astro-informatics.github.io/s2fft/tutorials/spherical_harmonic/JAX_HEALPix_backend.html>`_).  Fix for GPU execution is coming soon.
 
 Sampling |:earth_africa:|
 -----------------------------------
 
 The structure of the algorithms implemented in ``S2FFT`` can support any isolattitude sampling scheme.  A number of sampling schemes are currently supported.
 
 The equiangular sampling schemes of `McEwen & Wiaux (2012) <https://arxiv.org/abs/1110.6298>`_, 
 `Driscoll & Healy (1995) <https://www.sciencedirect.com/science/article/pii/S0196885884710086>`_, and `Gauss-Legendre (1986) <https://link.springer.com/article/10.1007/BF02519350>`_ are supported, which exhibit associated sampling theorems and so harmonic transforms can be computed to machine precision.  Note that the McEwen & Wiaux sampling theorem reduces the Nyquist rate on the sphere by a factor of two compared to the Driscoll & Healy approach, halving the number of spherical samples required. 
 
 The popular `HEALPix <https://healpix.jpl.nasa.gov>`_ sampling scheme (`Gorski et al. 2005 <https://arxiv.org/abs/astro-ph/0409513>`_) is also supported.  The HEALPix sampling does not exhibit a sampling theorem and so the corresponding harmonic transforms do not achieve machine precision but exhibit some error.  However, the HEALPix sampling provides pixels of equal areas, which has many practical advantages.
     
 .. image:: ./assets/figures/spherical_sampling.png
-   :width: 700
+   :width: 900
    :align: center
 
 Contributors ✨
 -----------------------------------
 
 Thanks goes to these wonderful people (`emoji
 key <https://allcontributors.org/docs/en/emoji-key>`_):
```

### Comparing `s2fft-1.0.2/docs/user_guide/install.rst` & `s2fft-1.1.0/docs/user_guide/install.rst`

 * *Files 23% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 from PyPi by running 
 
 .. code-block:: bash
     
     pip install s2fft 
 
 after which ``S2FFT`` may be imported and run as outlined in the associated notebooks and collab tutorials.
-To install the PyTorch functionality you will need to install the subpackage by running 
-
-.. code-block:: bash
-    
-    pip install s2fft[torch]
+This will include PyTorch functionality.
 
 Install from source (GitHub)
 ----------------------------
 
 When installing from source we recommend working within an existing conda environment, or creating a fresh conda environment to avoid any dependency conflicts,
 
 .. code-block:: bash
@@ -40,34 +36,33 @@
 
 .. code-block:: bash
 
     git clone https://github.com/astro-informatics/s2fft
     cd s2fft
     pip install .
 
-from the root directory of the repository. To install the Pytorch support you will need to 
-install the subpackage by running 
+from the root directory of the repository. This will include PyTorch functionality.
 
-.. code-block:: bash
-
-    pip install .[torch]
+Unit tests can then be executed to ensure the installation was successful by first installing the test requirements and then running pytest
 
-which, depending on operating system, can sometimes be 
+.. code-block:: bash 
 
-.. code-block:: bash
+    pip install -r requirements/requirements-tests.txt
+    pytest tests/ 
 
-    pip install .\[torch\]
-    
-Unit tests can then be executed to ensure the installation was successful by running 
+Documentation for the released version is available `here <https://astro-informatics.github.io/s2fft/>`_.  To build the documentation locally run
 
 .. code-block:: bash 
 
-    pytest tests/ 
+    pip install -r requirements/requirements-docs.txt
+    cd docs 
+    make html
+    open _build/html/index.html
+
 
-In the very near future one will be able to install ``S2FFT`` directly from `PyPi` by ``pip install s2fft`` but this is not yet supported.
 
 Installing JAX for NVIDIA GPUs
 ------------------------------
 We include both ``jax`` and ``jaxlib`` as dependencies in ``requirements/requirements-core.txt`` 
 however to get things running on GPUs can be a bit more involved. We strongly recommend 
 this installation `guide <https://github.com/google/jax#installation>`_ provided by 
 Google. To summarise you will first need to install NVIDIA drivers for
```

### Comparing `s2fft-1.0.2/s2fft/README.rst` & `s2fft-1.1.0/s2fft/README.rst`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/__init__.py` & `s2fft-1.1.0/s2fft/__init__.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/base_transforms/spherical.py` & `s2fft-1.1.0/s2fft/base_transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/base_transforms/wigner.py` & `s2fft-1.1.0/s2fft/base_transforms/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/default-logging-config.yaml` & `s2fft-1.1.0/s2fft/default-logging-config.yaml`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/logs.py` & `s2fft-1.1.0/s2fft/logs.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/precompute_transforms/construct.py` & `s2fft-1.1.0/s2fft/precompute_transforms/construct.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/precompute_transforms/spherical.py` & `s2fft-1.1.0/s2fft/precompute_transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/precompute_transforms/wigner.py` & `s2fft-1.1.0/s2fft/precompute_transforms/wigner.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/price_mcewen.py` & `s2fft-1.1.0/s2fft/recursions/price_mcewen.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/risbo.py` & `s2fft-1.1.0/s2fft/recursions/risbo.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/risbo_jax.py` & `s2fft-1.1.0/s2fft/recursions/risbo_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/trapani.py` & `s2fft-1.1.0/s2fft/recursions/trapani.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/turok.py` & `s2fft-1.1.0/s2fft/recursions/turok.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/recursions/turok_jax.py` & `s2fft-1.1.0/s2fft/recursions/turok_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/sampling/s2_samples.py` & `s2fft-1.1.0/s2fft/sampling/s2_samples.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/sampling/so3_samples.py` & `s2fft-1.1.0/s2fft/sampling/so3_samples.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/transforms/otf_recursions.py` & `s2fft-1.1.0/s2fft/transforms/otf_recursions.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/transforms/spherical.py` & `s2fft-1.1.0/s2fft/transforms/spherical.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,29 @@
     resampling,
     quadrature,
     resampling_jax,
     quadrature_jax,
 )
 from s2fft.utils import healpix_ffts as hp
 from s2fft.transforms import otf_recursions as otf
+from s2fft.transforms import c_backend_spherical as c_sph
 
 
 def inverse(
     flm: np.ndarray,
     L: int,
     spin: int = 0,
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
     spmd: bool = False,
     L_lower: int = 0,
+    _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the inverse spin-spherical harmonic transform.
 
     Args:
         flm (np.ndarray): Spherical harmonic coefficients.
 
         L (int): Harmonic band-limit.
@@ -38,15 +40,16 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
+        method (str, optional): Execution mode in {"numpy", "jax", "jax_ssht", "jax_healpy"}.
+            Defaults to "numpy".
 
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
@@ -54,35 +57,50 @@
         spmd (bool, optional): Whether to map compute over multiple devices. Currently this
             only maps over all available devices, and is only valid for JAX implementations.
             Defaults to False.
 
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
     Raises:
         ValueError: Transform method not recognised.
 
     Returns:
         np.ndarray: Signal on the sphere.
 
     Note:
         The single-program multiple-data (SPMD) optional variable determines whether
         the transform is run over a single device or all available devices. For very low
         harmonic bandlimits L this is inefficient as the I/O overhead for communication
         between devices is noticable, however as L increases one will asymptotically
         recover acceleration by the number of devices.
     """
-    if spin >= 8:
+
+    if spin >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond spin ~ 8")
+
     if method == "numpy":
         return inverse_numpy(flm, L, spin, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
         return inverse_jax(
             flm, L, spin, nside, sampling, reality, precomps, spmd, L_lower
         )
+    elif method == "jax_ssht":
+        if sampling.lower() == "healpix":
+            raise ValueError("SSHT does not support healpix sampling.")
+        ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+        return c_sph.ssht_inverse(flm, L, spin, reality, ssht_sampling, _ssht_backend)
+    elif method == "jax_healpy":
+        if sampling.lower() != "healpix":
+            raise ValueError("Healpy only supports healpix sampling.")
+        return c_sph.healpy_inverse(flm, L, nside)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
         )
 
 
 def inverse_numpy(
@@ -110,16 +128,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -209,16 +225,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -316,14 +330,16 @@
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
     spmd: bool = False,
     L_lower: int = 0,
+    iter: int = 3,
+    _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the forward spin-spherical harmonic transform.
 
     Args:
         f (np.ndarray): Signal on the sphere.
 
         L (int): Harmonic band-limit.
@@ -332,15 +348,16 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
+        method (str, optional): Execution mode in {"numpy", "jax", "jax_ssht", "jax_healpy"}.
+            Defaults to "numpy".
 
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
@@ -348,35 +365,54 @@
         spmd (bool, optional): Whether to map compute over multiple devices. Currently this
             only maps over all available devices, and is only valid for JAX implementations.
             Defaults to False.
 
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
+        iter (int, optional): Number of subiterations for healpy. Note that iterations
+            increase the precision of the forward transform, but reduce the accuracy of
+            the gradient pass. Between 2 and 3 iterations is a good compromise.
+
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
     Raises:
         ValueError: Transform method not recognised.
 
     Returns:
         np.ndarray: Spherical harmonic coefficients.
 
     Note:
         The single-program multiple-data (SPMD) optional variable determines whether
         the transform is run over a single device or all available devices. For very low
         harmonic bandlimits L this is inefficient as the I/O overhead for communication
         between devices is noticable, however as L increases one will asymptotically
         recover acceleration by the number of devices.
     """
-    if spin >= 8:
+
+    if spin >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond spin ~ 8")
+
     if method == "numpy":
         return forward_numpy(f, L, spin, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
         return forward_jax(
             f, L, spin, nside, sampling, reality, precomps, spmd, L_lower
         )
+    elif method == "jax_ssht":
+        if sampling.lower() == "healpix":
+            raise ValueError("SSHT does not support healpix sampling.")
+        ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+        return c_sph.ssht_forward(f, L, spin, reality, ssht_sampling, _ssht_backend)
+    elif method == "jax_healpy":
+        if sampling.lower() != "healpix":
+            raise ValueError("Healpy only supports healpix sampling.")
+        return c_sph.healpy_forward(f, L, nside, iter)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
         )
 
 
 def forward_numpy(
@@ -404,16 +440,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -531,16 +565,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
```

### Comparing `s2fft-1.0.2/s2fft/transforms/wigner.py` & `s2fft-1.1.0/s2fft/transforms/wigner.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,52 +4,59 @@
 import numpy as np
 import jax.numpy as jnp
 import jax.lax as lax
 from functools import partial
 from typing import List
 import s2fft
 from s2fft.sampling import so3_samples as samples
+from s2fft.transforms import c_backend_spherical as c_sph
 
 
 def inverse(
     flmn: np.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
     spmd: bool = False,
     L_lower: int = 0,
+    _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the inverse Wigner transform, i.e. inverse Fourier transform on
     :math:`SO(3)`.
 
     Importantly, the convention adopted for storage of f is :math:`[\gamma, \beta,
     \alpha]`, for Euler angles :math:`(\alpha, \beta, \gamma)` following the
     :math:`zyz` Euler convention, in order to simplify indexing for internal use.
     For a given :math:`\gamma` we thus recover a signal on the sphere indexed by
     :math:`[\theta, \phi]`, i.e. we associate :math:`\beta` with :math:`\theta` and
     :math:`\alpha` with :math:`\phi`.
 
+    Should the user select method = "jax_ssht" they will be restricted to deployment on
+    CPU using our custom JAX frontend for the SSHT C library [1]. In many
+    cases this approach may be desirable to mitigate e.g. memory i/o cost.
+
     Args:
         flmn (np.ndarray): Wigner coefficients with shape :math:`[2N-1, L, 2L-1]`.
 
         L (int): Harmonic band-limit.
 
         N (int): Azimuthal band-limit.
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
+        method (str, optional): Execution mode in {"numpy", "jax", "jax_ssht"}.
+            Defaults to "numpy".
 
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
@@ -57,37 +64,50 @@
         spmd (bool, optional): Whether to map compute over multiple devices. Currently this
             only maps over all available devices, and is only valid for JAX implementations.
             Defaults to False.
 
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
     Raises:
         ValueError: Transform method not recognised.
 
     Returns:
         np.ndarray:  Signal on the on :math:`SO(3)` with shape :math:`[n_{\gamma},
         n_{\beta}, n_{\alpha}]`, where :math:`n_\xi` denotes the number of samples for
         angle :math:`\xi`.
 
     Note:
         The single-program multiple-data (SPMD) optional variable determines whether
         the transform is run over a single device or all available devices. For very low
         harmonic bandlimits L this is inefficient as the I/O overhead for communication
         between devices is noticable, however as L increases one will asymptotically
         recover acceleration by the number of devices.
+
+        [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
+            IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
-    if N >= 8:
+
+    if N >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond N ~ 8")
+
     if method == "numpy":
         return inverse_numpy(flmn, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
         return inverse_jax(
             flmn, L, N, nside, sampling, reality, precomps, spmd, L_lower
         )
+    elif method == "jax_ssht":
+        if sampling.lower() == "healpix":
+            raise ValueError("SSHT does not support healpix sampling.")
+        return inverse_jax_ssht(flmn, L, N, L_lower, sampling, reality, _ssht_backend)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
         )
 
 
 def inverse_numpy(
@@ -122,16 +142,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -173,52 +191,50 @@
         f = np.fft.ifft(np.fft.ifftshift(fban, axes=ax), axis=ax, norm="forward")
 
     return f
 
 
 @partial(jit, static_argnums=(1, 2, 3, 4, 5, 7, 8))
 def inverse_jax(
-    flmn: np.ndarray,
+    flmn: jnp.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     reality: bool = False,
     precomps: List = None,
     spmd: bool = False,
     L_lower: int = 0,
 ) -> jnp.ndarray:
-    r"""Compute the inverse Wigner transform (numpy).
+    r"""Compute the inverse Wigner transform (JAX).
 
     Uses separation of variables and exploits the Price & McEwen recursion for accelerated
     and numerically stable Wiger-d on-the-fly recursions. The memory overhead for this
     function is theoretically :math:`\mathcal{O}(NL^2)`.
 
     Importantly, the convention adopted for storage of f is :math:`[\gamma, \beta,
     \alpha]`, for Euler angles :math:`(\alpha, \beta, \gamma)` following the
     :math:`zyz` Euler convention, in order to simplify indexing for internal use.
     For a given :math:`\gamma` we thus recover a signal on the sphere indexed by
     :math:`[\theta, \phi]`, i.e. we associate :math:`\beta` with :math:`\theta` and
     :math:`\alpha` with :math:`\phi`.
 
     Args:
-        flmn (np.ndarray): Wigner coefficients with shape :math:`[2N-1, L, 2L-1]`.
+        flmn (jnp.ndarray): Wigner coefficients with shape :math:`[2N-1, L, 2L-1]`.
 
         L (int): Harmonic band-limit.
 
         N (int): Azimuthal band-limit.
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -327,36 +343,120 @@
         fban = fban.at[: N - 1].set(jnp.flip(jnp.conj(fban[N:]), axis=0))
     fban = jnp.conj(jnp.fft.ifftshift(fban, axes=0))
     f = jnp.conj(jnp.fft.fft(fban, axis=0, norm="backward"))
 
     return f
 
 
+def inverse_jax_ssht(
+    flmn: jnp.ndarray,
+    L: int,
+    N: int,
+    L_lower: int = 0,
+    sampling: str = "mw",
+    reality: bool = False,
+    _ssht_backend: int = 1,
+) -> jnp.ndarray:
+    r"""Compute the inverse Wigner transform (SSHT JAX).
+
+    SSHT is a C library which implements the spin-spherical harmonic transform outlined
+    in McEwen & Wiaux 2011 [1]. We make use of their python bindings for which we
+    provide custom JAX frontends, hence providing support for automatic differentiation.
+    Currently these transforms can only be deployed on CPU, which is a limitation of the
+    SSHT C package.
+
+    Args:
+        flmn (jnp.ndarray): Wigner coefficients with shape :math:`[2N-1, L, 2L-1]`.
+
+        L (int): Harmonic band-limit.
+
+        N (int): Azimuthal band-limit.
+
+        L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
+            for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
+
+        sampling (str, optional): Sampling scheme.  Supported sampling schemes include
+            {"mw", "mwss", "dh", "gl"}.  Defaults to "mw".
+
+        reality (bool, optional): Whether the signal on the sphere is real.  If so,
+            conjugate symmetry is exploited to reduce computational costs.  Defaults to
+            False.
+
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
+    Returns:
+        np.ndarray: Signal on the sphere.
+
+    Note:
+        [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
+            IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
+    """
+    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+    fban = jnp.zeros(samples.f_shape(L, N, sampling), dtype=jnp.complex128)
+
+    flmn = flmn.at[:, L_lower:].set(
+        jnp.einsum(
+            "...nlm,...l->...nlm",
+            flmn[:, L_lower:],
+            jnp.sqrt((2 * jnp.arange(L_lower, L) + 1) / (16 * jnp.pi**3)),
+            optimize=True,
+        )
+    )
+
+    n_start_ind = 0 if reality else -N + 1
+    for n in range(n_start_ind, N):
+        fban = fban.at[N - 1 + n].add(
+            (-1) ** jnp.abs(n)
+            * c_sph.ssht_inverse(
+                flmn[N - 1 + n],
+                L,
+                -n,
+                reality if n == 0 else False,
+                ssht_sampling,
+                _ssht_backend,
+            )
+        )
+
+    if reality:
+        f = jnp.fft.irfft(fban[N - 1 :], 2 * N - 1, axis=-3, norm="forward")
+    else:
+        f = jnp.fft.ifft(jnp.fft.ifftshift(fban, axes=-3), axis=-3, norm="forward")
+
+    return f
+
+
 def forward(
     f: np.ndarray,
     L: int,
     N: int,
     nside: int = None,
     sampling: str = "mw",
     method: str = "numpy",
     reality: bool = False,
     precomps: List = None,
     spmd: bool = False,
     L_lower: int = 0,
+    _ssht_backend: int = 1,
 ) -> np.ndarray:
     r"""Wrapper for the forward Wigner transform, i.e. Fourier transform on
     :math:`SO(3)`.
 
     Importantly, the convention adopted for storage of f is :math:`[\gamma, \beta,
     \alpha]`, for Euler angles :math:`(\alpha, \beta, \gamma)` following the
     :math:`zyz` Euler convention, in order to simplify indexing for internal use.
     For a given :math:`\gamma` we thus recover a signal on the sphere indexed by
     :math:`[\theta, \phi]`, i.e. we associate :math:`\beta` with :math:`\theta` and
     :math:`\alpha` with :math:`\phi`.
 
+    Should the user select method = "jax_ssht" they will be restricted to deployment on
+    CPU using our custom JAX frontend for the SSHT C library [1]. In many cases this
+    approach may be desirable to mitigate e.g. memory i/o cost.
+
     Args:
         f (np.ndarray): Signal on the on :math:`SO(3)` with shape
             :math:`[n_{\gamma}, n_{\beta}, n_{\alpha}]`, where :math:`n_\xi` denotes the
             number of samples for angle :math:`\xi`.
 
         L (int): Harmonic band-limit.
 
@@ -364,15 +464,16 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
+        method (str, optional): Execution mode in {"numpy", "jax", "jax_ssht"}.
+            Defaults to "numpy".
 
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
@@ -380,33 +481,46 @@
         spmd (bool, optional): Whether to map compute over multiple devices. Currently this
             only maps over all available devices, and is only valid for JAX implementations.
             Defaults to False.
 
         L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
             for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
 
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
     Raises:
         ValueError: Transform method not recognised.
 
     Returns:
         np.ndarray: Wigner coefficients `flmn` with shape :math:`[2N-1, L, 2L-1]`.
 
     Note:
         The single-program multiple-data (SPMD) optional variable determines whether
         the transform is run over a single device or all available devices. For very low
         harmonic bandlimits L this is inefficient as the I/O overhead for communication
         between devices is noticable, however as L increases one will asymptotically
         recover acceleration by the number of devices.
+
+        [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
+            IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
     """
-    if N >= 8:
+
+    if N >= 8 and method in ["numpy", "jax"]:
         raise Warning("Recursive transform may provide lower precision beyond N ~ 8")
+
     if method == "numpy":
         return forward_numpy(f, L, N, nside, sampling, reality, precomps, L_lower)
     elif method == "jax":
         return forward_jax(f, L, N, nside, sampling, reality, precomps, spmd, L_lower)
+    elif method == "jax_ssht":
+        if sampling.lower() == "healpix":
+            raise ValueError("SSHT does not support healpix sampling.")
+        return forward_jax_ssht(f, L, N, L_lower, sampling, reality, _ssht_backend)
     else:
         raise ValueError(
             f"Implementation {method} not recognised. Should be either numpy or jax."
         )
 
 
 def forward_numpy(
@@ -443,16 +557,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[np.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -539,16 +651,14 @@
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required
             if sampling="healpix".  Defaults to None.
 
         sampling (str, optional): Sampling scheme.  Supported sampling schemes include
             {"mw", "mwss", "dh", "gl", "healpix"}.  Defaults to "mw".
 
-        method (str, optional): Execution mode in {"numpy", "jax"}. Defaults to "numpy".
-
         reality (bool, optional): Whether the signal on the sphere is real.  If so,
             conjugate symmetry is exploited to reduce computational costs.  Defaults to
             False.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
 
@@ -654,13 +764,100 @@
             flmn = flmn.at[N - 1 - n].set(
                 jnp.conj(jnp.flip(flmn[N - 1 + n] * sgn * (-1) ** n, axis=-1))
             )
 
     flmn = flmn.at[:, L_lower:].set(
         jnp.einsum(
             "...nlm,...l->...nlm",
+            flmn[:, L_lower:],
+            jnp.sqrt(4 * jnp.pi / (2 * jnp.arange(L_lower, L) + 1)),
+            optimize=True,
+        )
+    )
+    return flmn
+
+
+def forward_jax_ssht(
+    f: jnp.ndarray,
+    L: int,
+    N: int,
+    L_lower: int = 0,
+    sampling: str = "mw",
+    reality: bool = False,
+    _ssht_backend: int = 1,
+) -> jnp.ndarray:
+    r"""Compute the forward Wigner transform (SSHT JAX).
+
+    SSHT is a C library which implements the spin-spherical harmonic transform outlined
+    in McEwen & Wiaux 2011 [1]. We make use of their python bindings for which we
+    provide custom JAX frontends, hence providing support for automatic differentiation.
+    Currently these transforms can only be deployed on CPU, which is a limitation of the
+    SSHT C package.
+
+    Args:
+        f (jnp.ndarray): Signal on the on :math:`SO(3)` with shape
+            :math:`[n_{\gamma}, n_{\beta}, n_{\alpha}]`, where :math:`n_\xi` denotes the
+            number of samples for angle :math:`\xi`.
+
+        L (int): Harmonic band-limit.
+
+        N (int): Azimuthal band-limit.
+
+        L_lower (int, optional): Harmonic lower-bound. Transform will only be computed
+            for :math:`\texttt{L_lower} \leq \ell < \texttt{L}`. Defaults to 0.
+
+        sampling (str, optional): Sampling scheme.  Supported sampling schemes include
+            {"mw", "mwss", "dh", "gl"}.  Defaults to "mw".
+
+        reality (bool, optional): Whether the signal on the sphere is real.  If so,
+            conjugate symmetry is exploited to reduce computational costs.  Defaults to
+            False.
+
+        _ssht_backend (int, optional, experimental): Whether to default to SSHT core
+            (set to 0) recursions or pick up ducc0 (set to 1) accelerated experimental
+            backend. Use with caution.
+
+    Returns:
+        jnp.ndarray: Wigner coefficients `flmn` with shape :math:`[2N-1, L, 2L-1]`.
+
+    Note:
+        [1] McEwen, Jason D. and Yves Wiaux. “A Novel Sampling Theorem on the Sphere.”
+            IEEE Transactions on Signal Processing 59 (2011): 5876-5887.
+    """
+    ssht_sampling = ["mw", "mwss", "dh", "gl"].index(sampling.lower())
+    flmn = jnp.zeros(samples.flmn_shape(L, N), dtype=jnp.complex128)
+
+    if reality:
+        fban = jnp.fft.rfft(jnp.real(f), axis=0, norm="backward")
+    else:
+        fban = jnp.fft.fftshift(jnp.fft.fft(f, axis=0, norm="backward"), axes=0)
+
+    fban *= 2 * jnp.pi / (2 * N - 1)
+
+    n_start_ind = 0 if reality else -N + 1
+    for n in range(n_start_ind, N):
+        flmn = flmn.at[N - 1 + n].set(
+            (-1) ** jnp.abs(n)
+            * c_sph.ssht_forward(
+                fban[jnp.int64(n - n_start_ind)],
+                L,
+                -n,
+                False,
+                ssht_sampling,
+                _ssht_backend,
+            )
+        )
+        if reality and n != 0:
+            sgn = (-1) ** abs(jnp.arange(-L + 1, L))
+            flmn = flmn.at[N - 1 - n].set(
+                jnp.conj(jnp.flip(flmn[N - 1 + n] * sgn * (-1) ** n, axis=-1))
+            )
+
+    flmn = flmn.at[:, L_lower:].set(
+        jnp.einsum(
+            "...nlm,...l->...nlm",
             flmn[:, L_lower:],
             jnp.sqrt(4 * jnp.pi / (2 * jnp.arange(L_lower, L) + 1)),
             optimize=True,
         )
     )
     return flmn
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `s2fft-1.0.2/s2fft/utils/healpix_ffts.py` & `s2fft-1.1.0/s2fft/utils/healpix_ffts.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/quadrature.py` & `s2fft-1.1.0/s2fft/utils/quadrature.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/quadrature_jax.py` & `s2fft-1.1.0/s2fft/utils/quadrature_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/quadrature_torch.py` & `s2fft-1.1.0/s2fft/utils/quadrature_torch.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/resampling.py` & `s2fft-1.1.0/s2fft/utils/resampling.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/resampling_jax.py` & `s2fft-1.1.0/s2fft/utils/resampling_jax.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/resampling_torch.py` & `s2fft-1.1.0/s2fft/utils/resampling_torch.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/rotation.py` & `s2fft-1.1.0/s2fft/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft/utils/signal_generator.py` & `s2fft-1.1.0/s2fft/utils/signal_generator.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/s2fft.egg-info/PKG-INFO` & `s2fft-1.1.0/s2fft.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2fft
-Version: 1.0.2
+Version: 1.1.0
 Summary: Differentiable and accelerated spherical transforms with JAX
 Home-page: https://github.com/astro-informatics/s2fft
 Author: Matthew A. Price, Jason D. McEwen & Contributors
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,31 +17,32 @@
 License-File: LICENCE.txt
 Requires-Dist: numpy>=1.20
 Requires-Dist: colorlog
 Requires-Dist: pyyaml
 Requires-Dist: jax>=0.3.13
 Requires-Dist: jaxlib
 Requires-Dist: torch
-Provides-Extra: torch
-Requires-Dist: torch; extra == "torch"
+Requires-Dist: pyssht
+Requires-Dist: healpy
+Requires-Dist: ducc0
 
 .. image:: https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/astro-informatics/s2fft/actions/workflows/tests.yml
 .. image:: https://img.shields.io/badge/GitHub-s2fft-brightgreen.svg?style=flat
     :target: https://github.com/astro-informatics/s2fft
 .. image:: https://codecov.io/gh/astro-informatics/s2fft/branch/main/graph/badge.svg?token=7QYAFAAWLE
     :target: https://codecov.io/gh/astro-informatics/s2fft
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
     :target: https://opensource.org/licenses/MIT
 .. image:: http://img.shields.io/badge/arXiv-2311.14670-orange.svg?style=flat
     :target: https://arxiv.org/abs/2311.14670
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
-    :target: https://colab.research.google.com/drive/1YmJ2ljsF8HBvhPmD4hrYPlyAKc4WPUgq?usp=sharing
+    :target: https://colab.research.google.com/github/astro-informatics/s2fft/blob/main/notebooksspherical_harmonic_transform.ipynb
 
 Differentiable and accelerated spherical transforms
 =================================================================================================================
 
 `S2FFT` is a Python package for computing Fourier transforms on the sphere
 and rotation group using JAX and PyTorch. It leverages autodiff to provide differentiable
 transforms, which are also deployable on hardware accelerators
@@ -53,14 +54,20 @@
 optimisations (precompute or not) that one may select depending on
 available resources and desired angular resolution $L$.
 
 As of version 1.0.2 `S2FFT` also provides PyTorch implementations of underlying 
 precompute transforms. In future releases this support will be extended to our 
 on-the-fly algorithms.
 
+As of version 1.1.0 `S2FFT` also provides JAX support for existing C/C++ packages, 
+specifically `HEALPix` and `SSHT`. This works by wrapping python bindings with custom 
+JAX frontends. Note that currently this C/C++ to JAX interoperability is currently 
+limited to CPU, however for many applications this is desirable due to memory 
+constraints.
+
 Documentation
 =============
 Read the full documentation `here <https://astro-informatics.github.io/s2fft/>`_.
 
 Attribution
 ===========
 Should this code be used in any way, we kindly request that the following article is
```

### Comparing `s2fft-1.0.2/s2fft.egg-info/SOURCES.txt` & `s2fft-1.1.0/s2fft.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 docs/api/recursions/risbo_jax.rst
 docs/api/recursions/trapani.rst
 docs/api/recursions/turok.rst
 docs/api/recursions/turok_jax.rst
 docs/api/sampling/index.rst
 docs/api/sampling/spherical_samples.rst
 docs/api/sampling/wigner_samples.rst
+docs/api/transforms/c_backend_spherical.rst
 docs/api/transforms/index.rst
 docs/api/transforms/on_the_fly_recursions.rst
 docs/api/transforms/spin_spherical_transform.rst
 docs/api/transforms/wigner.rst
 docs/api/utility/healpix_ffts.rst
 docs/api/utility/index.rst
 docs/api/utility/logs.rst
@@ -66,14 +67,16 @@
 docs/assets/figures/software_overview.png
 docs/assets/figures/spherical_sampling.png
 docs/assets/figures/spin_spherical_mw.pdf
 docs/assets/figures/spin_spherical_mw.png
 docs/assets/figures/wigner_mw.pdf
 docs/assets/figures/wigner_mw.png
 docs/tutorials/index.rst
+docs/tutorials/JAX_HEALPix/JAX_HEALPix_frontend.nblink
+docs/tutorials/JAX_SSHT/JAX_SSHT_frontend.nblink
 docs/tutorials/rotation/rotation.nblink
 docs/tutorials/spherical_harmonic/spherical_harmonic_transform.nblink
 docs/tutorials/torch_frontend/torch_frontend.nblink
 docs/tutorials/wigner/wigner_transform.nblink
 docs/user_guide/install.rst
 requirements/requirements-core.txt
 requirements/requirements-docs.txt
@@ -103,14 +106,15 @@
 s2fft/recursions/trapani.py
 s2fft/recursions/turok.py
 s2fft/recursions/turok_jax.py
 s2fft/sampling/__init__.py
 s2fft/sampling/s2_samples.py
 s2fft/sampling/so3_samples.py
 s2fft/transforms/__init__.py
+s2fft/transforms/c_backend_spherical.py
 s2fft/transforms/otf_recursions.py
 s2fft/transforms/spherical.py
 s2fft/transforms/wigner.py
 s2fft/utils/__init__.py
 s2fft/utils/healpix_ffts.py
 s2fft/utils/quadrature.py
 s2fft/utils/quadrature_jax.py
```

### Comparing `s2fft-1.0.2/setup.py` & `s2fft-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,20 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="s2fft",
-    version="1.0.2",
+    version="1.1.0",
     url="https://github.com/astro-informatics/s2fft",
     author="Matthew A. Price, Jason D. McEwen & Contributors",
     license="MIT",
     python_requires=">=3.8",
     install_requires=requirements,
     description=("Differentiable and accelerated spherical transforms with JAX"),
     long_description_content_type="text/x-rst",
     long_description=long_description,
     packages=find_packages(),
     include_package_data=True,
     pacakge_data={"s2fft": ["default-logging-config.yaml"]},
-    extras_require={"torch": ["torch"]},
 )
```

### Comparing `s2fft-1.0.2/tests/conftest.py` & `s2fft-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_healpix_ffts.py` & `s2fft-1.1.0/tests/test_healpix_ffts.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_quadrature.py` & `s2fft-1.1.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_resampling.py` & `s2fft-1.1.0/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_samples.py` & `s2fft-1.1.0/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_spherical_base.py` & `s2fft-1.1.0/tests/test_spherical_base.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_spherical_custom_grads.py` & `s2fft-1.1.0/tests/test_wigner_custom_grads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,210 +1,163 @@
 import jax
 
 jax.config.update("jax_enable_x64", True)
 import pytest
 import jax.numpy as jnp
 from jax.test_util import check_grads
 
-from s2fft.transforms import spherical
-from s2fft.recursions.price_mcewen import generate_precomputes_jax
+from s2fft.transforms import wigner
+from s2fft.recursions.price_mcewen import generate_precomputes_wigner_jax
 
-L_to_test = [16]
-L_lower_to_test = [2]
-spin_to_test = [-2, 0, 1]
-nside_to_test = [8]
+L_to_test = [6]
+N_to_test = [3]
+L_lower_to_test = [1]
 sampling_to_test = ["mw", "mwss", "dh", "gl"]
 reality_to_test = [False, True]
 
 
 @pytest.mark.parametrize("L", L_to_test)
+@pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
-@pytest.mark.parametrize("spin", spin_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
-def test_inverse_custom_gradients(
-    flm_generator,
+def test_inverse_wigner_custom_gradients(
+    flmn_generator,
     L: int,
+    N: int,
     L_lower: int,
-    spin: int,
     sampling: str,
     reality: bool,
 ):
-    if reality and spin != 0:
-        pytest.skip("Reality only valid for scalar fields (spin=0).")
-
-    flm = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    flm_target = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    f_target = spherical.inverse_jax(
-        flm_target,
-        L,
-        L_lower=L_lower,
-        spin=spin,
-        sampling=sampling,
-        reality=reality,
+    precomps = generate_precomputes_wigner_jax(
+        L, N, sampling, None, False, reality, L_lower
     )
-    precomps = generate_precomputes_jax(
-        L, spin, sampling, forward=False, L_lower=L_lower
+
+    flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    f_target = wigner.inverse_jax(
+        flmn_target, L, N, None, sampling, reality, precomps, False, L_lower
     )
 
-    def func(flm):
-        f = spherical.inverse_jax(
-            flm,
-            L,
-            spin=spin,
-            L_lower=L_lower,
-            reality=reality,
-            precomps=precomps,
-            sampling=sampling,
+    def func(flmn):
+        f = wigner.inverse_jax(
+            flmn, L, N, None, sampling, reality, precomps, False, L_lower
         )
         return jnp.sum(jnp.abs(f - f_target) ** 2)
 
-    check_grads(func, (flm,), order=1, modes=("rev"))
+    check_grads(func, (flmn,), order=1, modes=("rev"))
 
 
 @pytest.mark.parametrize("L", L_to_test)
+@pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
-@pytest.mark.parametrize("spin", spin_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
-def test_forward_custom_gradients(
-    flm_generator,
+def test_forward_wigner_custom_gradients(
+    flmn_generator,
     L: int,
+    N: int,
     L_lower: int,
-    spin: int,
     sampling: str,
     reality: bool,
 ):
-    if reality and spin != 0:
-        pytest.skip("Reality only valid for scalar fields (spin=0).")
-
-    flm_target = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    flm = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    f = spherical.inverse_jax(
-        flm,
-        L,
-        L_lower=L_lower,
-        spin=spin,
-        sampling=sampling,
-        reality=reality,
-    )
-    precomps = generate_precomputes_jax(
-        L, spin, sampling, forward=True, L_lower=L_lower
+    precomps = generate_precomputes_wigner_jax(
+        L, N, sampling, None, True, reality, L_lower
     )
 
+    flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, False, L_lower)
+
     def func(f):
-        flm = spherical.forward_jax(
-            f,
-            L,
-            spin=spin,
-            L_lower=L_lower,
-            reality=reality,
-            precomps=precomps,
-            sampling=sampling,
+        flmn = wigner.forward_jax(
+            f, L, N, None, sampling, reality, precomps, False, L_lower
         )
-        return jnp.sum(jnp.abs(flm - flm_target) ** 2)
+        return jnp.sum(jnp.abs(flmn - flmn_target) ** 2)
 
     check_grads(func, (f,), order=1, modes=("rev"))
 
 
-@pytest.mark.parametrize("nside", nside_to_test)
+@pytest.mark.parametrize("L", L_to_test)
+@pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
-@pytest.mark.parametrize("spin", spin_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
+@pytest.mark.parametrize("_ssht_backend", [0, 1])
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
-def test_healpix_inverse_custom_gradients(
-    flm_generator,
-    nside: int,
+def test_ssht_c_backend_inverse_wigner_custom_gradients(
+    flmn_generator,
+    L: int,
+    N: int,
     L_lower: int,
-    spin: int,
     sampling: str,
     reality: bool,
+    _ssht_backend: int,
 ):
-    sampling = "healpix"
-    L = 2 * nside
 
-    if reality and spin != 0:
-        pytest.skip("Reality only valid for scalar fields (spin=0).")
+    if sampling.lower() == "dh" and _ssht_backend == 1:
+        pytest.skip("Driscoll Healy ducc0 backend gradient calculation tempremental.")
 
-    flm = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    flm_target = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    f_target = spherical.inverse_jax(
-        flm_target,
-        L,
-        L_lower=L_lower,
-        spin=spin,
-        nside=nside,
-        sampling=sampling,
-        reality=reality,
-    )
-    precomps = generate_precomputes_jax(
-        L, spin, sampling, nside, forward=False, L_lower=L_lower
+    flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    f_target = wigner.inverse_jax(
+        flmn_target, L, N, None, sampling, reality, None, False, L_lower
     )
 
-    def func(flm):
-        f = spherical.inverse_jax(
-            flm,
+    def func(flmn):
+        f = wigner.inverse(
+            jnp.array(flmn),
             L,
-            spin=spin,
-            nside=nside,
+            N,
+            None,
+            sampling,
+            "jax_ssht",
+            reality,
             L_lower=L_lower,
-            reality=reality,
-            precomps=precomps,
-            sampling=sampling,
+            _ssht_backend=_ssht_backend,
         )
         return jnp.sum(jnp.abs(f - f_target) ** 2)
 
-    check_grads(func, (flm,), order=1, modes=("rev"))
+    check_grads(func, (flmn,), order=1, modes=("rev"))
 
 
-@pytest.mark.parametrize("nside", nside_to_test)
+@pytest.mark.parametrize("L", L_to_test)
+@pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("L_lower", L_lower_to_test)
-@pytest.mark.parametrize("spin", spin_to_test)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("reality", reality_to_test)
+@pytest.mark.parametrize("_ssht_backend", [0, 1])
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
-def test_healpix_forward_custom_gradients(
-    flm_generator,
-    nside: int,
+def test_ssht_c_backend_forward_wigner_custom_gradients(
+    flmn_generator,
+    L: int,
+    N: int,
     L_lower: int,
-    spin: int,
     sampling: str,
     reality: bool,
+    _ssht_backend: int,
 ):
-    sampling = "healpix"
-    L = 2 * nside
 
-    if reality and spin != 0:
-        pytest.skip("Reality only valid for scalar fields (spin=0).")
+    if sampling.lower() == "dh" and _ssht_backend == 1:
+        pytest.skip("Driscoll Healy ducc0 backend gradient calculation tempremental.")
 
-    flm_target = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    flm = flm_generator(L=L, L_lower=L_lower, spin=spin, reality=reality)
-    f = spherical.inverse_jax(
-        flm,
-        L,
-        L_lower=L_lower,
-        spin=spin,
-        nside=nside,
-        sampling=sampling,
-        reality=reality,
-    )
-    precomps = generate_precomputes_jax(
-        L, spin, sampling, nside, forward=True, L_lower=L_lower
-    )
+    flmn_target = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    flmn = flmn_generator(L=L, N=N, L_lower=L_lower, reality=reality)
+    f = wigner.inverse_jax(flmn, L, N, None, sampling, reality, None, False, L_lower)
 
     def func(f):
-        flm = spherical.forward_jax(
+        flmn = wigner.forward(
             f,
             L,
-            spin=spin,
-            nside=nside,
+            N,
+            None,
+            sampling,
+            "jax_ssht",
+            reality,
             L_lower=L_lower,
-            reality=reality,
-            precomps=precomps,
-            sampling=sampling,
+            _ssht_backend=_ssht_backend,
         )
-        return jnp.sum(jnp.abs(flm - flm_target) ** 2)
+        return jnp.sum(jnp.abs(flmn - flmn_target) ** 2)
 
-    check_grads(func, (f,), order=1, modes=("rev"))
+    check_grads(func, (jnp.array(f),), order=1, modes=("rev"))
```

### Comparing `s2fft-1.0.2/tests/test_spherical_precompute.py` & `s2fft-1.1.0/tests/test_spherical_precompute.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_spherical_transform.py` & `s2fft-1.1.0/tests/test_spherical_transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -176,7 +176,59 @@
         spmd=spmd,
     )
     flm_check = samples.flm_2d_to_hp(flm_check, L)
 
     flm = hp.sphtfunc.map2alm(f, lmax=L - 1, iter=0)
 
     np.testing.assert_allclose(flm, flm_check, atol=1e-14)
+
+
+def test_spin_exceptions(flm_generator):
+    spin = 10
+    L = 16
+    sampling = "mw"
+
+    flm = flm_generator(L=L, reality=False)
+    f = spherical.inverse(flm, L, spin=0, sampling=sampling, method="jax_ssht")
+
+    with pytest.raises(Warning) as e:
+        spherical.inverse(flm, L, spin=spin, sampling=sampling, method="jax")
+
+    with pytest.raises(Warning) as e:
+        spherical.forward(f, L, spin=spin, sampling=sampling, method="jax")
+
+
+def test_sampling_ssht_backend_exceptions(flm_generator):
+    sampling = "healpix"
+    nside = 6
+    L = 2 * nside
+
+    flm = flm_generator(L=L, reality=False)
+    f = spherical.inverse(flm, L, 0, nside, sampling, "jax_healpy")
+
+    with pytest.raises(ValueError) as e:
+        spherical.inverse(flm, L, 0, nside, sampling, "jax_ssht")
+
+    with pytest.raises(ValueError) as e:
+        spherical.forward(f, L, 0, nside, sampling, "jax_ssht")
+
+
+def test_sampling_healpy_backend_exceptions(flm_generator):
+    sampling = "mw"
+    L = 12
+
+    flm = flm_generator(L=L, reality=False)
+    f = spherical.inverse(flm, L, 0, None, sampling, "jax_ssht")
+
+    with pytest.raises(ValueError) as e:
+        spherical.inverse(flm, L, 0, None, sampling, "jax_healpy")
+
+    with pytest.raises(ValueError) as e:
+        spherical.forward(f, L, 0, None, sampling, "jax_healpy")
+
+
+def test_sampling_exceptions(flm_generator):
+    with pytest.raises(ValueError) as e:
+        spherical.inverse(None, 0, 0, None, method="incorrect")
+
+    with pytest.raises(ValueError) as e:
+        spherical.forward(None, 0, 0, None, method="incorrect")
```

### Comparing `s2fft-1.0.2/tests/test_utils.py` & `s2fft-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_wigner_base.py` & `s2fft-1.1.0/tests/test_wigner_base.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_wigner_precompute.py` & `s2fft-1.1.0/tests/test_wigner_precompute.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_wigner_recursions.py` & `s2fft-1.1.0/tests/test_wigner_recursions.py`

 * *Files identical despite different names*

### Comparing `s2fft-1.0.2/tests/test_wigner_samples.py` & `s2fft-1.1.0/tests/test_wigner_samples.py`

 * *Files identical despite different names*

