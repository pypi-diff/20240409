# Comparing `tmp/sinabs-2.0.1.dev4.tar.gz` & `tmp/sinabs-2.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinabs-2.0.1.dev4.tar", last modified: Tue Apr  9 14:24:26 2024, max compression
+gzip compressed data, was "sinabs-2.0.1.dev5.tar", last modified: Tue Apr  9 14:25:52 2024, max compression
```

## Comparing `sinabs-2.0.1.dev4.tar` & `sinabs-2.0.1.dev5.tar`

### file list

```diff
@@ -1,334 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.172920 sinabs-2.0.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.120919 sinabs-2.0.1.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.124919 sinabs-2.0.1.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    61456 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 14:24:26.172920 sinabs-2.0.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.128919 sinabs-2.0.1.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.128919 sinabs-2.0.1.dev4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.128919 sinabs-2.0.1.dev4/docs/_static/Overview/
--rw-r--r--   0 runner    (1001) docker     (127)    41488 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/dataflow_layers.png
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/event_preprocessing_pipeline.png
--rw-r--r--   0 runner    (1001) docker     (127)    34971 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/memory_constraints.png
--rw-r--r--   0 runner    (1001) docker     (127)    56246 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/sinabs-dynapcnn-role.png
--rw-r--r--   0 runner    (1001) docker     (127)   114768 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/speck_dynapcnn.png
--rw-r--r--   0 runner    (1001) docker     (127)   345972 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/Overview/speck_top_level.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.128919 sinabs-2.0.1.dev4/docs/_static/devkits_images/
--rw-r--r--   0 runner    (1001) docker     (127)   188479 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/devkits_images/dynapcnn_devkit.png
--rw-r--r--   0 runner    (1001) docker     (127)    65675 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_devkit.png
--rw-r--r--   0 runner    (1001) docker     (127)    50505 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_module.png
--rw-r--r--   0 runner    (1001) docker     (127)   277714 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_module_devkit.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/
--rw-r--r--   0 runner    (1001) docker     (127)    48964 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/dvs_input_flow.png
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/dynapcnn_visualizer.png
--rw-r--r--   0 runner    (1001) docker     (127)    45601 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/spike_input_flow.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/power_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)    36805 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/power_monitoring/dynamic_power_samna_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/power_monitoring/idle_power_samna_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)    30647 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/power_monitoring/power_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/sinabs-logo-lowercase-whitebg.png
--rw-r--r--   0 runner    (1001) docker     (127)    80008 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/sinabs-logo-lowercase.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/tips_for_training/
--rw-r--r--   0 runner    (1001) docker     (127)    74980 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/tips_for_training/exceeding_bandwidth.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/using_readout_layer/
--rw-r--r--   0 runner    (1001) docker     (127)    80444 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/using_readout_layer/handcraft_weights.png
--rw-r--r--   0 runner    (1001) docker     (127)    28534 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/using_readout_layer/neuron_id_mismatch.png
--rw-r--r--   0 runner    (1001) docker     (127)    48829 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/using_readout_layer/readout_layer.png
--rw-r--r--   0 runner    (1001) docker     (127)    59701 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/using_readout_layer/samna_graph.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/visualize_speck_dvs/
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/visualize_speck_dvs/samna_graph.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_static/visualize_spike_count/
--rw-r--r--   0 runner    (1001) docker     (127)    53316 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/visualize_spike_count/samna_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_static/visualize_spike_count/spike_count.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_templates/class_activation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/_templates/class_layer.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.132919 sinabs-2.0.1.dev4/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/about/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/about/differences.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/about/info.md
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/about/release_notes.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.136919 sinabs-2.0.1.dev4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/activation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/from_torch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/layers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/network.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/nir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/synopcounter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/contact.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.136919 sinabs-2.0.1.dev4/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.136919 sinabs-2.0.1.dev4/docs/gallery/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/plot_alif.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/plot_exp_leaky.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/plot_iaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/plot_lif.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/layers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.136919 sinabs-2.0.1.dev4/docs/gallery/spike_fns/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/spike_fns/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/spike_fns/plot_maxspike.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/spike_fns/plot_multispike.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/spike_fns/plot_singlespike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.136919 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/plot_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/plot_heaviside.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/plot_multigaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/plot_periodicexponential.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/gallery/surrogate_grad_fns/plot_singleexponential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.140919 sinabs-2.0.1.dev4/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/fundamentals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/iaf_neuron_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/python_pyenv_pipenv.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/getting_started/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.140919 sinabs-2.0.1.dev4/docs/how_tos/
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/how_tos/activations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/how_tos/custom_hooks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/how_tos/how_tos.rst
--rw-r--r--   0 runner    (1001) docker     (127)    49760 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/how_tos/synops_loss_ann.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   107384 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/how_tos/synops_loss_snn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.140919 sinabs-2.0.1.dev4/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/plugins/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.140919 sinabs-2.0.1.dev4/docs/speck/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/advanced_concepts.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.120919 sinabs-2.0.1.dev4/docs/speck/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.144919 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/chip_factory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/config_builder.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/crop2d.rst
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/discretize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/dvs_layer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/dynapcnn.rst
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/dynapcnn_layer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/dynapcnn_network.rst
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/dynapcnn_visualizer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/flipdims.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/mapping.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/specksim.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/api/dynapcnn/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/dangers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.144919 sinabs-2.0.1.dev4/docs/speck/faqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/add_new_device.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/available_algorithmic_operation.md
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/available_network_arch.md
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/chip_errata.md
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/device_management.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/output_monitoring.md
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/save_hardware_config_as_binary.md
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/faqs/tips_for_training.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.144919 sinabs-2.0.1.dev4/docs/speck/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/leak_neuron.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    48347 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/nmnist_quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24137 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/play_with_speck_dvs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    65595 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/power_monitoring.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    89661 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/using_readout_layer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/visualize_speck_dvs_input.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    46024 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/notebooks/visualize_spike_count.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/overview.md
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/specksim.md
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/the_basics.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/speck/visualizer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.148919 sinabs-2.0.1.dev4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/LeNet_5_EngChinese.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/bptt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/nir_to_speck.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    48768 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/nmnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   273552 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/scnn_mnist.nir
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/weight_scaling.md
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/docs/tutorials/weight_transfer_mnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.120919 sinabs-2.0.1.dev4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.148919 sinabs-2.0.1.dev4/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/mnist/dynapcnn_network.py
--rw-r--r--   0 runner    (1001) docker     (127)   491676 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/mnist/mnist_params.pt
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/mnist/specksim_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.148919 sinabs-2.0.1.dev4/examples/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)   688196 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/dvs_gesture_params.pt
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/gesture_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.152919 sinabs-2.0.1.dev4/examples/visualizer/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/01_armroll.png
--rw-r--r--   0 runner    (1001) docker     (127)    31052 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/02_handclap.png
--rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/03_lefthandclockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)    58695 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/04_lefthandcounterclockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)    30701 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/05_lefthandwave.png
--rw-r--r--   0 runner    (1001) docker     (127)    36496 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/06_righthandwave.png
--rw-r--r--   0 runner    (1001) docker     (127)    58589 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/07_righthandclockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)    50175 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/08_righthandcounterclockwise.png
--rw-r--r--   0 runner    (1001) docker     (127)    33717 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/09_airdrums.png
--rw-r--r--   0 runner    (1001) docker     (127)    33211 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/10_airguitar.png
--rw-r--r--   0 runner    (1001) docker     (127)    69926 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/examples/visualizer/icons/11_other.png
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/jupyterlab-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 14:24:26.172920 sinabs-2.0.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.152919 sinabs-2.0.1.dev4/sinabs/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.156919 sinabs-2.0.1.dev4/sinabs/activation/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/activation/quantize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/activation/reset_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/activation/spike_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/activation/surrogate_gradient_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.156919 sinabs-2.0.1.dev4/sinabs/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.156919 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chip_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.156919 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/dynapcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2cmini.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2dmini.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2f.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/crop2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dvs_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    22858 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/flipdims.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/specksim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/cnnutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/from_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.160919 sinabs-2.0.1.dev4/sinabs/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/alif.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/crop2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/exp_leak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.160919 sinabs-2.0.1.dev4/sinabs/layers/functional/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/functional/alif.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/functional/lif.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/iaf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/lif.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/neuromorphic_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/pool2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/quantize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/stateful_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/layers/to_spike.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/nir.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/synopcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/sinabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.152919 sinabs-2.0.1.dev4/sinabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-09 14:24:26.000000 sinabs-2.0.1.dev4/sinabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 14:24:25.000000 sinabs-2.0.1.dev4/sinabs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.164919 sinabs-2.0.1.dev4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.124919 sinabs-2.0.1.dev4/tests/inputs_and_results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.164919 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/conv_input.pth
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/conv_layer_synops.pth
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/firing_rates.pth
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/firing_rates_per_neuron.pth
--rw-r--r--   0 runner    (1001) docker     (127)    41507 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/input_diffs.pth
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/model_synops.pth
--rw-r--r--   0 runner    (1001) docker     (127)   491676 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/mnist_params.pt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.164919 sinabs-2.0.1.dev4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/models/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44457 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/models/synop_hook_model.pth
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_batch_mismatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_batch_size_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.168919 sinabs-2.0.1.dev4/tests/test_dynapcnn/
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/hw_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_auto_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_compatible_layer_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_config_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_device_movement.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_device_name_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_discover_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_discretized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_doorbell.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_dvs_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_dvs_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_event_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_individual_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_large_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_neuron_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_single_neuron_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_speck2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_speckmini_config_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_dynapcnn/test_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_from_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.168919 sinabs-2.0.1.dev4/tests/test_layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_alif.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_channelshift.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_crop2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_exp_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_iaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_img2spk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_lif.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_maxpooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_neuromorphic_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_reshaping.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_sig2spk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_layers/test_stateful_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_network_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_nir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_normalize_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.168919 sinabs-2.0.1.dev4/tests/test_residual/
--rw-r--r--   0 runner    (1001) docker     (127)    60074 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_residual/NIR_graph_nonseq.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.172920 sinabs-2.0.1.dev4/tests/test_specksim/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_surrogate_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_synops_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:24:26.172920 sinabs-2.0.1.dev4/tests/weights/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 14:24:23.000000 sinabs-2.0.1.dev4/tests/weights/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.422800 sinabs-2.0.1.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.430800 sinabs-2.0.1.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    61456 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.430800 sinabs-2.0.1.dev5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.430800 sinabs-2.0.1.dev5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.430800 sinabs-2.0.1.dev5/docs/_static/Overview/
+-rw-r--r--   0 runner    (1001) docker     (127)    41488 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/dataflow_layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/event_preprocessing_pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34971 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/memory_constraints.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56246 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/sinabs-dynapcnn-role.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114768 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/speck_dynapcnn.png
+-rw-r--r--   0 runner    (1001) docker     (127)   345972 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/Overview/speck_top_level.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/devkits_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   188479 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/devkits_images/dynapcnn_devkit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65675 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_devkit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50505 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_module.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277714 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_module_devkit.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/
+-rw-r--r--   0 runner    (1001) docker     (127)    48964 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/dvs_input_flow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/dynapcnn_visualizer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45601 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/spike_input_flow.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/power_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)    36805 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/power_monitoring/dynamic_power_samna_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/power_monitoring/idle_power_samna_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30647 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/power_monitoring/power_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/sinabs-logo-lowercase-whitebg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80008 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/sinabs-logo-lowercase.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/tips_for_training/
+-rw-r--r--   0 runner    (1001) docker     (127)    74980 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/tips_for_training/exceeding_bandwidth.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/using_readout_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)    80444 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/using_readout_layer/handcraft_weights.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28534 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/using_readout_layer/neuron_id_mismatch.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48829 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/using_readout_layer/readout_layer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59701 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/using_readout_layer/samna_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.434800 sinabs-2.0.1.dev5/docs/_static/visualize_speck_dvs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/visualize_speck_dvs/samna_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/_static/visualize_spike_count/
+-rw-r--r--   0 runner    (1001) docker     (127)    53316 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/visualize_spike_count/samna_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_static/visualize_spike_count/spike_count.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_templates/class_activation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/_templates/class_layer.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/about/differences.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/about/info.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/about/release_notes.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/activation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/from_torch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/layers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/network.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/nir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/synopcounter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/contact.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.438800 sinabs-2.0.1.dev5/docs/gallery/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/plot_alif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/plot_exp_leaky.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/plot_iaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/plot_lif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/layers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.442800 sinabs-2.0.1.dev5/docs/gallery/spike_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/spike_fns/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/spike_fns/plot_maxspike.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/spike_fns/plot_multispike.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/spike_fns/plot_singlespike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.442800 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/plot_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/plot_heaviside.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/plot_multigaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/plot_periodicexponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/gallery/surrogate_grad_fns/plot_singleexponential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.442800 sinabs-2.0.1.dev5/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/fundamentals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/iaf_neuron_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/python_pyenv_pipenv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/getting_started/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.442800 sinabs-2.0.1.dev5/docs/how_tos/
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/how_tos/activations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/how_tos/custom_hooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/how_tos/how_tos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    49760 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/how_tos/synops_loss_ann.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   107384 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/how_tos/synops_loss_snn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.442800 sinabs-2.0.1.dev5/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/plugins/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.446800 sinabs-2.0.1.dev5/docs/speck/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/advanced_concepts.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.426800 sinabs-2.0.1.dev5/docs/speck/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.446800 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/chip_factory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/config_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/crop2d.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/discretize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/dvs_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/dynapcnn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/dynapcnn_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/dynapcnn_network.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/dynapcnn_visualizer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/flipdims.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/specksim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/api/dynapcnn/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/dangers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.446800 sinabs-2.0.1.dev5/docs/speck/faqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/add_new_device.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/available_algorithmic_operation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/available_network_arch.md
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/chip_errata.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/device_management.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/output_monitoring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/save_hardware_config_as_binary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/faqs/tips_for_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.450801 sinabs-2.0.1.dev5/docs/speck/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/leak_neuron.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    48347 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/nmnist_quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24137 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/play_with_speck_dvs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    65595 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/power_monitoring.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    89661 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/using_readout_layer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/visualize_speck_dvs_input.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    46024 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/notebooks/visualize_spike_count.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/overview.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/specksim.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/the_basics.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/speck/visualizer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.450801 sinabs-2.0.1.dev5/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/LeNet_5_EngChinese.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/bptt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/nir_to_speck.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    48768 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/nmnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   273552 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/scnn_mnist.nir
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/weight_scaling.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/docs/tutorials/weight_transfer_mnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.426800 sinabs-2.0.1.dev5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.450801 sinabs-2.0.1.dev5/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/mnist/dynapcnn_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   491676 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/mnist/mnist_params.pt
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/mnist/specksim_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.454800 sinabs-2.0.1.dev5/examples/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)   688196 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/dvs_gesture_params.pt
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/gesture_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.454800 sinabs-2.0.1.dev5/examples/visualizer/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/01_armroll.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31052 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/02_handclap.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/03_lefthandclockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58695 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/04_lefthandcounterclockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30701 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/05_lefthandwave.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36496 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/06_righthandwave.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58589 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/07_righthandclockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50175 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/08_righthandcounterclockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33717 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/09_airdrums.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33211 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/10_airguitar.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69926 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/examples/visualizer/icons/11_other.png
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/jupyterlab-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.458800 sinabs-2.0.1.dev5/sinabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.458800 sinabs-2.0.1.dev5/sinabs/activation/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/activation/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/activation/reset_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/activation/spike_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/activation/surrogate_gradient_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.458800 sinabs-2.0.1.dev5/sinabs/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.462801 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chip_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.462801 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/dynapcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2cmini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2dmini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/crop2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dvs_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22858 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/flipdims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/specksim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/cnnutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/from_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.462801 sinabs-2.0.1.dev5/sinabs/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/alif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/crop2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/exp_leak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.466801 sinabs-2.0.1.dev5/sinabs/layers/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/functional/alif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/functional/lif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/iaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15324 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/lif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/neuromorphic_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/pool2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/stateful_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/layers/to_spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/nir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/synopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/sinabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.458800 sinabs-2.0.1.dev5/sinabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 14:25:52.000000 sinabs-2.0.1.dev5/sinabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.466801 sinabs-2.0.1.dev5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.426800 sinabs-2.0.1.dev5/tests/inputs_and_results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.470800 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/conv_input.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/conv_layer_synops.pth
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/firing_rates.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/firing_rates_per_neuron.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    41507 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/input_diffs.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/model_synops.pth
+-rw-r--r--   0 runner    (1001) docker     (127)   491676 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/mnist_params.pt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.470800 sinabs-2.0.1.dev5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/models/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44457 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/models/synop_hook_model.pth
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_batch_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_batch_size_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.470800 sinabs-2.0.1.dev5/tests/test_dynapcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/hw_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_auto_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_compatible_layer_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_config_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_device_movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_device_name_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_discover_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_discretized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_doorbell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_dvs_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_dvs_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_event_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_individual_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_large_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_neuron_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_single_neuron_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_speck2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_speckmini_config_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_dynapcnn/test_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/tests/test_layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_alif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_channelshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_crop2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_exp_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_iaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_img2spk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_lif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_maxpooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_neuromorphic_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_sig2spk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_layers/test_stateful_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_network_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_nir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_normalize_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_quantize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/tests/test_specksim/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_surrogate_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_synops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:25:52.474801 sinabs-2.0.1.dev5/tests/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 14:25:48.000000 sinabs-2.0.1.dev5/tests/weights/README.txt
```

### Comparing `sinabs-2.0.1.dev4/.github/workflows/ci-pipeline.yml` & `sinabs-2.0.1.dev5/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/AUTHORS` & `sinabs-2.0.1.dev5/AUTHORS`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/CITATION.cff` & `sinabs-2.0.1.dev5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/ChangeLog` & `sinabs-2.0.1.dev5/ChangeLog`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/LICENSE` & `sinabs-2.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/PKG-INFO` & `sinabs-2.0.1.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinabs
-Version: 2.0.1.dev4
+Version: 2.0.1.dev5
 Summary: SynSense Spiking Neural Network simulator for deep neural networks (DNNs).
 Home-page: UNKNOWN
 Author: SynSense (formerly AiCTX)
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source code, https://github.com/synsense/sinabs
 Project-URL: Documentation, https://readthedocs.org/projects/sinabs/
```

### Comparing `sinabs-2.0.1.dev4/Pipfile.lock` & `sinabs-2.0.1.dev5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/README.md` & `sinabs-2.0.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/Makefile` & `sinabs-2.0.1.dev5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/dataflow_layers.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/dataflow_layers.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/event_preprocessing_pipeline.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/event_preprocessing_pipeline.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/memory_constraints.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/memory_constraints.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/sinabs-dynapcnn-role.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/sinabs-dynapcnn-role.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/speck_dynapcnn.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/speck_dynapcnn.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/Overview/speck_top_level.png` & `sinabs-2.0.1.dev5/docs/_static/Overview/speck_top_level.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/devkits_images/dynapcnn_devkit.png` & `sinabs-2.0.1.dev5/docs/_static/devkits_images/dynapcnn_devkit.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_devkit.png` & `sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_devkit.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_module.png` & `sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_module.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/devkits_images/speck_module_devkit.png` & `sinabs-2.0.1.dev5/docs/_static/devkits_images/speck_module_devkit.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/dvs_input_flow.png` & `sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/dvs_input_flow.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/dynapcnn_visualizer.png` & `sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/dynapcnn_visualizer.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/nmnist_quick_start/spike_input_flow.png` & `sinabs-2.0.1.dev5/docs/_static/nmnist_quick_start/spike_input_flow.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/power_monitoring/dynamic_power_samna_graph.png` & `sinabs-2.0.1.dev5/docs/_static/power_monitoring/dynamic_power_samna_graph.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/power_monitoring/idle_power_samna_graph.png` & `sinabs-2.0.1.dev5/docs/_static/power_monitoring/idle_power_samna_graph.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/power_monitoring/power_plot.png` & `sinabs-2.0.1.dev5/docs/_static/power_monitoring/power_plot.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/sinabs-logo-lowercase-whitebg.png` & `sinabs-2.0.1.dev5/docs/_static/sinabs-logo-lowercase-whitebg.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/sinabs-logo-lowercase.png` & `sinabs-2.0.1.dev5/docs/_static/sinabs-logo-lowercase.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/tips_for_training/exceeding_bandwidth.png` & `sinabs-2.0.1.dev5/docs/_static/tips_for_training/exceeding_bandwidth.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/using_readout_layer/handcraft_weights.png` & `sinabs-2.0.1.dev5/docs/_static/using_readout_layer/handcraft_weights.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/using_readout_layer/neuron_id_mismatch.png` & `sinabs-2.0.1.dev5/docs/_static/using_readout_layer/neuron_id_mismatch.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/using_readout_layer/readout_layer.png` & `sinabs-2.0.1.dev5/docs/_static/using_readout_layer/readout_layer.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/using_readout_layer/samna_graph.png` & `sinabs-2.0.1.dev5/docs/_static/using_readout_layer/samna_graph.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/visualize_speck_dvs/samna_graph.png` & `sinabs-2.0.1.dev5/docs/_static/visualize_speck_dvs/samna_graph.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/visualize_spike_count/samna_graph.png` & `sinabs-2.0.1.dev5/docs/_static/visualize_spike_count/samna_graph.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/_static/visualize_spike_count/spike_count.png` & `sinabs-2.0.1.dev5/docs/_static/visualize_spike_count/spike_count.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/about/contributing.md` & `sinabs-2.0.1.dev5/docs/about/contributing.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/about/differences.md` & `sinabs-2.0.1.dev5/docs/about/differences.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/about/release_notes.md` & `sinabs-2.0.1.dev5/docs/about/release_notes.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/api/activation.rst` & `sinabs-2.0.1.dev5/docs/api/activation.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/api/hooks.rst` & `sinabs-2.0.1.dev5/docs/api/hooks.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/api/layers.rst` & `sinabs-2.0.1.dev5/docs/api/layers.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/conf.py` & `sinabs-2.0.1.dev5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/gallery/layers/plot_lif.py` & `sinabs-2.0.1.dev5/docs/gallery/layers/plot_lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/gallery/layers/utils.py` & `sinabs-2.0.1.dev5/docs/gallery/layers/utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/getting_started/fundamentals.rst` & `sinabs-2.0.1.dev5/docs/getting_started/fundamentals.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/getting_started/iaf_neuron_model.ipynb` & `sinabs-2.0.1.dev5/docs/getting_started/iaf_neuron_model.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/getting_started/install.rst` & `sinabs-2.0.1.dev5/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/getting_started/python_pyenv_pipenv.rst` & `sinabs-2.0.1.dev5/docs/getting_started/python_pyenv_pipenv.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/getting_started/quickstart.ipynb` & `sinabs-2.0.1.dev5/docs/getting_started/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/how_tos/activations.ipynb` & `sinabs-2.0.1.dev5/docs/how_tos/activations.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/how_tos/custom_hooks.ipynb` & `sinabs-2.0.1.dev5/docs/how_tos/custom_hooks.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/how_tos/synops_loss_ann.ipynb` & `sinabs-2.0.1.dev5/docs/how_tos/synops_loss_ann.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/how_tos/synops_loss_snn.ipynb` & `sinabs-2.0.1.dev5/docs/how_tos/synops_loss_snn.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/index.md` & `sinabs-2.0.1.dev5/docs/index.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/make.bat` & `sinabs-2.0.1.dev5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/advanced_concepts.rst` & `sinabs-2.0.1.dev5/docs/speck/advanced_concepts.rst`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/dangers.md` & `sinabs-2.0.1.dev5/docs/speck/dangers.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/add_new_device.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/add_new_device.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/available_algorithmic_operation.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/available_algorithmic_operation.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/available_network_arch.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/available_network_arch.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/chip_errata.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/chip_errata.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/device_management.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/device_management.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/output_monitoring.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/output_monitoring.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/save_hardware_config_as_binary.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/save_hardware_config_as_binary.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/faqs/tips_for_training.md` & `sinabs-2.0.1.dev5/docs/speck/faqs/tips_for_training.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/leak_neuron.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/leak_neuron.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/nmnist_quick_start.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/nmnist_quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/play_with_speck_dvs.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/play_with_speck_dvs.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/power_monitoring.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/power_monitoring.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/using_readout_layer.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/using_readout_layer.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/visualize_speck_dvs_input.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/visualize_speck_dvs_input.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/notebooks/visualize_spike_count.ipynb` & `sinabs-2.0.1.dev5/docs/speck/notebooks/visualize_spike_count.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/overview.md` & `sinabs-2.0.1.dev5/docs/speck/overview.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/specksim.md` & `sinabs-2.0.1.dev5/docs/speck/specksim.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/the_basics.md` & `sinabs-2.0.1.dev5/docs/speck/the_basics.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/speck/visualizer.md` & `sinabs-2.0.1.dev5/docs/speck/visualizer.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/LeNet_5_EngChinese.ipynb` & `sinabs-2.0.1.dev5/docs/tutorials/LeNet_5_EngChinese.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/bptt.ipynb` & `sinabs-2.0.1.dev5/docs/tutorials/bptt.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/nir_to_speck.ipynb` & `sinabs-2.0.1.dev5/docs/tutorials/nir_to_speck.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/nmnist.ipynb` & `sinabs-2.0.1.dev5/docs/tutorials/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/scnn_mnist.nir` & `sinabs-2.0.1.dev5/docs/tutorials/scnn_mnist.nir`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/weight_scaling.md` & `sinabs-2.0.1.dev5/docs/tutorials/weight_scaling.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/docs/tutorials/weight_transfer_mnist.ipynb` & `sinabs-2.0.1.dev5/docs/tutorials/weight_transfer_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/mnist/dynapcnn_network.py` & `sinabs-2.0.1.dev5/examples/mnist/dynapcnn_network.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/mnist/mnist_params.pt` & `sinabs-2.0.1.dev5/examples/mnist/mnist_params.pt`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/mnist/specksim_network.py` & `sinabs-2.0.1.dev5/examples/mnist/specksim_network.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/dvs_gesture_params.pt` & `sinabs-2.0.1.dev5/examples/visualizer/dvs_gesture_params.pt`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/gesture_viz.py` & `sinabs-2.0.1.dev5/examples/visualizer/gesture_viz.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/01_armroll.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/01_armroll.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/02_handclap.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/02_handclap.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/03_lefthandclockwise.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/03_lefthandclockwise.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/04_lefthandcounterclockwise.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/04_lefthandcounterclockwise.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/05_lefthandwave.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/05_lefthandwave.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/06_righthandwave.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/06_righthandwave.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/07_righthandclockwise.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/07_righthandclockwise.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/08_righthandcounterclockwise.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/08_righthandcounterclockwise.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/09_airdrums.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/09_airdrums.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/10_airguitar.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/10_airguitar.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/examples/visualizer/icons/11_other.png` & `sinabs-2.0.1.dev5/examples/visualizer/icons/11_other.png`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/pull_request_template.md` & `sinabs-2.0.1.dev5/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/setup.cfg` & `sinabs-2.0.1.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/activation/quantize.py` & `sinabs-2.0.1.dev5/sinabs/activation/quantize.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/activation/reset_mechanism.py` & `sinabs-2.0.1.dev5/sinabs/activation/reset_mechanism.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/activation/spike_generation.py` & `sinabs-2.0.1.dev5/sinabs/activation/spike_generation.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/activation/surrogate_gradient_fn.py` & `sinabs-2.0.1.dev5/sinabs/activation/surrogate_gradient_fn.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chip_factory.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chip_factory.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/dynapcnn.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/dynapcnn.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2b.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2b.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2cmini.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2cmini.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2dmini.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2dmini.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2e.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2e.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/chips/speck2f.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/chips/speck2f.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/config_builder.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/config_builder.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/crop2d.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/crop2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/discretize.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/discretize.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dvs_layer.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dvs_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_layer.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_network.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_network.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/dynapcnn_visualizer.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/dynapcnn_visualizer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/flipdims.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/flipdims.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/io.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/io.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/mapping.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/mapping.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/specksim.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/specksim.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/backend/dynapcnn/utils.py` & `sinabs-2.0.1.dev5/sinabs/backend/dynapcnn/utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/cnnutils.py` & `sinabs-2.0.1.dev5/sinabs/cnnutils.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/conversion.py` & `sinabs-2.0.1.dev5/sinabs/conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/from_torch.py` & `sinabs-2.0.1.dev5/sinabs/from_torch.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/hooks.py` & `sinabs-2.0.1.dev5/sinabs/hooks.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/__init__.py` & `sinabs-2.0.1.dev5/sinabs/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/alif.py` & `sinabs-2.0.1.dev5/sinabs/layers/alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/channel_shift.py` & `sinabs-2.0.1.dev5/sinabs/layers/channel_shift.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/crop2d.py` & `sinabs-2.0.1.dev5/sinabs/layers/crop2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/exp_leak.py` & `sinabs-2.0.1.dev5/sinabs/layers/exp_leak.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/functional/alif.py` & `sinabs-2.0.1.dev5/sinabs/layers/functional/alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/functional/lif.py` & `sinabs-2.0.1.dev5/sinabs/layers/functional/lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/iaf.py` & `sinabs-2.0.1.dev5/sinabs/layers/iaf.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/lif.py` & `sinabs-2.0.1.dev5/sinabs/layers/lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/merge.py` & `sinabs-2.0.1.dev5/sinabs/layers/merge.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/neuromorphic_relu.py` & `sinabs-2.0.1.dev5/sinabs/layers/neuromorphic_relu.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/pool2d.py` & `sinabs-2.0.1.dev5/sinabs/layers/pool2d.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/reshape.py` & `sinabs-2.0.1.dev5/sinabs/layers/reshape.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/stateful_layer.py` & `sinabs-2.0.1.dev5/sinabs/layers/stateful_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/layers/to_spike.py` & `sinabs-2.0.1.dev5/sinabs/layers/to_spike.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/network.py` & `sinabs-2.0.1.dev5/sinabs/network.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/nir.py` & `sinabs-2.0.1.dev5/sinabs/nir.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/synopcounter.py` & `sinabs-2.0.1.dev5/sinabs/synopcounter.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs/utils.py` & `sinabs-2.0.1.dev5/sinabs/utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/sinabs.egg-info/PKG-INFO` & `sinabs-2.0.1.dev5/sinabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinabs
-Version: 2.0.1.dev4
+Version: 2.0.1.dev5
 Summary: SynSense Spiking Neural Network simulator for deep neural networks (DNNs).
 Home-page: UNKNOWN
 Author: SynSense (formerly AiCTX)
 Author-email: sinabs@synsense.ai
 License: GNU AGPLv3
 Project-URL: Source code, https://github.com/synsense/sinabs
 Project-URL: Documentation, https://readthedocs.org/projects/sinabs/
```

### Comparing `sinabs-2.0.1.dev4/sinabs.egg-info/SOURCES.txt` & `sinabs-2.0.1.dev5/sinabs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -272,12 +272,11 @@
 tests/test_layers/test_lif.py
 tests/test_layers/test_maxpooling.py
 tests/test_layers/test_merge.py
 tests/test_layers/test_neuromorphic_relu.py
 tests/test_layers/test_reshaping.py
 tests/test_layers/test_sig2spk.py
 tests/test_layers/test_stateful_layer.py
-tests/test_residual/NIR_graph_nonseq.ipynb
 tests/test_specksim/test_specksim_bindings.py
 tests/test_specksim/test_specksim_conversion.py
 tests/test_specksim/test_specksim_network.py
 tests/weights/README.txt
```

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/conv_input.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/conv_input.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/conv_layer_synops.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/conv_layer_synops.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/firing_rates.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/firing_rates.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/firing_rates_per_neuron.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/firing_rates_per_neuron.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/input_diffs.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/input_diffs.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/inputs_and_results/hooks/model_synops.pth` & `sinabs-2.0.1.dev5/tests/inputs_and_results/hooks/model_synops.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/mnist_params.pt` & `sinabs-2.0.1.dev5/tests/mnist_params.pt`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/models/synop_hook_model.pth` & `sinabs-2.0.1.dev5/tests/models/synop_hook_model.pth`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_activations.py` & `sinabs-2.0.1.dev5/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_batch_mismatch.py` & `sinabs-2.0.1.dev5/tests/test_batch_mismatch.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_batch_size_update.py` & `sinabs-2.0.1.dev5/tests/test_batch_size_update.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_conversion.py` & `sinabs-2.0.1.dev5/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_copy.py` & `sinabs-2.0.1.dev5/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/hw_utils.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/hw_utils.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_auto_mapping.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_auto_mapping.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_compatible_layer_build.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_compatible_layer_build.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_config_making.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_config_making.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_device_movement.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_device_movement.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_discover_device.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_discover_device.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_discretized.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_discretized.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_doorbell.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_doorbell.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_dvs_input.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_dvs_input.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_dvs_layer.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_dvs_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_event_conversion.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_event_conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_individual_cases.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_individual_cases.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_large_net.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_large_net.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_learning.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_learning.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_monitoring.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_neuron_leak.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_neuron_leak.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_single_neuron_hardware.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_single_neuron_hardware.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_speck2e.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_speck2e.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_speckmini_config_making.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_speckmini_config_making.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_dynapcnn/test_visualizer.py` & `sinabs-2.0.1.dev5/tests/test_dynapcnn/test_visualizer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_from_model.py` & `sinabs-2.0.1.dev5/tests/test_from_model.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_hooks.py` & `sinabs-2.0.1.dev5/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_alif.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_alif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_exp_leak.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_exp_leak.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_iaf.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_iaf.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_img2spk.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_img2spk.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_lif.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_lif.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_maxpooling.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_maxpooling.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_merge.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_merge.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_neuromorphic_relu.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_neuromorphic_relu.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_reshaping.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_reshaping.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_layers/test_stateful_layer.py` & `sinabs-2.0.1.dev5/tests/test_layers/test_stateful_layer.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_network_class.py` & `sinabs-2.0.1.dev5/tests/test_network_class.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_nir.py` & `sinabs-2.0.1.dev5/tests/test_nir.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_normalize_weights.py` & `sinabs-2.0.1.dev5/tests/test_normalize_weights.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_onnx.py` & `sinabs-2.0.1.dev5/tests/test_onnx.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_quantize.py` & `sinabs-2.0.1.dev5/tests/test_quantize.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_bindings.py` & `sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_bindings.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_conversion.py` & `sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_conversion.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_specksim/test_specksim_network.py` & `sinabs-2.0.1.dev5/tests/test_specksim/test_specksim_network.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_surrogate_gradients.py` & `sinabs-2.0.1.dev5/tests/test_surrogate_gradients.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_synops_counter.py` & `sinabs-2.0.1.dev5/tests/test_synops_counter.py`

 * *Files identical despite different names*

### Comparing `sinabs-2.0.1.dev4/tests/test_utils.py` & `sinabs-2.0.1.dev5/tests/test_utils.py`

 * *Files identical despite different names*

