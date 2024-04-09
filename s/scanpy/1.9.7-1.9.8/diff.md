# Comparing `tmp/scanpy-1.9.7.tar.gz` & `tmp/scanpy-1.9.8.tar.gz`

## Comparing `scanpy-1.9.7.tar` & `scanpy-1.9.8.tar`

### file list

```diff
@@ -1,229 +1,230 @@
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 scanpy-1.9.7/.azure-pipelines.yml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 scanpy-1.9.7/.codecov.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scanpy-1.9.7/.editorconfig
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scanpy-1.9.7/.flake8
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scanpy-1.9.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scanpy-1.9.7/.readthedocs.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scanpy-1.9.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/pull_request_template.md
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/ISSUE_TEMPLATE/enhancement-request.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/workflows/check-pr.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scanpy-1.9.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/Makefile
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_key_contributors.rst
--rw-r--r--   0        0        0     9884 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/api.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/basic_usage.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/community.md
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/conf.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/contributors.md
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/ecosystem.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/external.md
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/index.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/installation.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/matplotlibrc
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/news.md
--rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/references.rst
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/tutorials.md
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/usage-principles.md
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/Scanpy_Logo.svg
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/Scanpy_Logo_BrightFG.svg
--rw-r--r--   0        0        0    63218 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/Scanpy_Logo_RGB.png
--rw-r--r--   0        0        0   219512 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/ci_plot-view_attachment-tab.png
--rw-r--r--   0        0        0   100919 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/ci_plot-view_select-test.png
--rw-r--r--   0        0        0   241201 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/ci_plot-view_tests-tab.png
--rw-r--r--   0        0        0   540395 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/spatial-basic-analysis.png
--rw-r--r--   0        0        0    61708 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/stacked_violin_dotplot_matrixplot.png
--rw-r--r--   0        0        0   175602 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/paga_paul15.png
--rw-r--r--   0        0        0   330000 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/paga_planaria.png
--rwxr-xr-x   0        0        0   198469 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170430_krumsiek11/timeseries.png
--rwxr-xr-x   0        0        0    53008 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/NKG7.png
--rwxr-xr-x   0        0        0   216130 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/cell_types.png
--rwxr-xr-x   0        0        0    59760 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/filter_genes_dispersion.png
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/louvain.png
--rwxr-xr-x   0        0        0    84683 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/violin.png
--rwxr-xr-x   0        0        0   207532 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_static/img/tutorials/170522_visualizing_one_million_cells/tsne_1.3M.png
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/ci.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/code.md
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/documentation.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/external-tools.md
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/getting-set-up.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/index.md
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/release.md
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/testing.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/dev/versioning.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/debug_docstrings.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/function_images.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/github_links.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/has_attr_test.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/param_police.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.1.0.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.2.1.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.2.9.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.3.0.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.3.2.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.4.0.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.4.2.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.4.3.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/0.4.4.md
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.0.0.md
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.1.0.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.2.0.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.2.1.md
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.1.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.3.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.4.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.5.md
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.6.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.7.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.3.8.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.1.md
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.2.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.3.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.4.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.5.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.4.6.md
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.5.0.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.5.1.md
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.6.0.md
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.7.0.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.7.1.md
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.7.2.md
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.8.0.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.8.1.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.8.2.md
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.0.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.1.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.2.md
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.3.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.4.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.5.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.6.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/1.9.7.md
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/index.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 scanpy-1.9.7/docs/release-notes/release-latest.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/__main__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/_compat.py
--rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/_settings.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/_version.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/cli.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/logging.py
--rw-r--r--   0        0        0    33877 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/readwrite.py
--rw-r--r--   0        0        0    25286 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/_utils/__init__.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/_utils/compute/is_constant.py
--rw-r--r--   0        0        0  1772368 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/10x_pbmc68k_reduced.h5ad
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/__init__.py
--rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/_datasets.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/_ebi_expression_atlas.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/_utils.py
--rw-r--r--   0        0        0    59808 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/krumsiek11.txt
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/datasets/toggleswitch.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/__init__.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/_docs.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/pp/__init__.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/pp/_normalization.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/experimental/pp/_recipes.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/__init__.py
--rw-r--r--   0        0        0    21389 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/exporting.py
--rw-r--r--   0        0        0    12971 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pl.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/__init__.py
--rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_bbknn.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_dca.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_harmony_integrate.py
--rw-r--r--   0        0        0    15286 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_hashsolo.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_magic.py
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_mnn_correct.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_scanorama_integrate.py
--rw-r--r--   0        0        0    21747 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/pp/_scrublet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/__init__.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_harmony_timeseries.py
--rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_palantir.py
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_phate.py
--rw-r--r--   0        0        0     8553 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_phenograph.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_pypairs.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_sam.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_trimap.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/external/tl/_wishbone.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/get/__init__.py
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/get/get.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/metrics/__init__.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/metrics/_gearys_c.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/metrics/_metrics.py
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/metrics/_morans_i.py
--rw-r--r--   0        0        0    40591 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/neighbors/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/__init__.py
--rwxr-xr-x   0        0        0    87869 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_anndata.py
--rw-r--r--   0        0        0    38801 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_baseplot_class.py
--rw-r--r--   0        0        0    13507 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_docs.py
--rw-r--r--   0        0        0    38017 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_dotplot.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_matrixplot.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_preprocessing.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_qc.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_rcmod.py
--rw-r--r--   0        0        0    27060 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_stacked_violin.py
--rw-r--r--   0        0        0    38868 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_utils.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/palettes.py
--rw-r--r--   0        0        0    48883 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_tools/__init__.py
--rw-r--r--   0        0        0    47494 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_tools/paga.py
--rw-r--r--   0        0        0    43553 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/plotting/_tools/scatterplots.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/__init__.py
--rw-r--r--   0        0        0    11613 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_combat.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_distributed.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_docs.py
--rw-r--r--   0        0        0    22714 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_highly_variable_genes.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_normalization.py
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_pca.py
--rw-r--r--   0        0        0    14152 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_qc.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_recipes.py
--rw-r--r--   0        0        0    36555 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_simple.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_utils.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_deprecated/__init__.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/preprocessing/_deprecated/highly_variable_genes.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/queries/__init__.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/queries/_queries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/sim_models/__init__.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/sim_models/krumsiek11.txt
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/sim_models/krumsiek11_params.txt
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/sim_models/toggleswitch.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/sim_models/toggleswitch_params.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/__init__.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_helpers/__init__.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_helpers/data.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_pytest/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_pytest/marks.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_pytest/fixtures/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/testing/_pytest/fixtures/data.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/__init__.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_dendrogram.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_diffmap.py
--rw-r--r--   0        0        0    49576 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_dpt.py
--rw-r--r--   0        0        0     7003 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_draw_graph.py
--rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_embedding_density.py
--rw-r--r--   0        0        0    20102 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_ingest.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_leiden.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_louvain.py
--rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_marker_gene_overlap.py
--rw-r--r--   0        0        0    24674 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_paga.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_pca.py
--rw-r--r--   0        0        0    29307 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_rank_genes_groups.py
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_score_genes.py
--rw-r--r--   0        0        0    46842 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_sim.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_top_genes.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_tsne.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_umap.py
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_utils.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scanpy-1.9.7/scanpy/tools/_utils_clustering.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 scanpy-1.9.7/.gitignore
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scanpy-1.9.7/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scanpy-1.9.7/README.md
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 scanpy-1.9.7/pyproject.toml
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 scanpy-1.9.7/PKG-INFO
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 scanpy-1.9.8/.azure-pipelines.yml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 scanpy-1.9.8/.codecov.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scanpy-1.9.8/.editorconfig
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scanpy-1.9.8/.flake8
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scanpy-1.9.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scanpy-1.9.8/.readthedocs.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scanpy-1.9.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/ISSUE_TEMPLATE/enhancement-request.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/workflows/check-pr.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scanpy-1.9.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/Makefile
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_key_contributors.rst
+-rw-r--r--   0        0        0     9884 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/api.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/basic_usage.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/community.md
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/conf.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/contributors.md
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/ecosystem.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/external.md
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/index.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/installation.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/matplotlibrc
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/news.md
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/references.rst
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/tutorials.md
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/usage-principles.md
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/Scanpy_Logo.svg
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/Scanpy_Logo_BrightFG.svg
+-rw-r--r--   0        0        0    63218 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/Scanpy_Logo_RGB.png
+-rw-r--r--   0        0        0   219512 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/ci_plot-view_attachment-tab.png
+-rw-r--r--   0        0        0   100919 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/ci_plot-view_select-test.png
+-rw-r--r--   0        0        0   241201 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/ci_plot-view_tests-tab.png
+-rw-r--r--   0        0        0   540395 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/spatial-basic-analysis.png
+-rw-r--r--   0        0        0    61708 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/stacked_violin_dotplot_matrixplot.png
+-rw-r--r--   0        0        0   175602 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/paga_paul15.png
+-rw-r--r--   0        0        0   330000 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/paga_planaria.png
+-rwxr-xr-x   0        0        0   198469 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170430_krumsiek11/timeseries.png
+-rwxr-xr-x   0        0        0    53008 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/NKG7.png
+-rwxr-xr-x   0        0        0   216130 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/cell_types.png
+-rwxr-xr-x   0        0        0    59760 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/filter_genes_dispersion.png
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/louvain.png
+-rwxr-xr-x   0        0        0    84683 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/violin.png
+-rwxr-xr-x   0        0        0   207532 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_static/img/tutorials/170522_visualizing_one_million_cells/tsne_1.3M.png
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/ci.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/code.md
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/documentation.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/external-tools.md
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/getting-set-up.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/index.md
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/release.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/testing.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/dev/versioning.md
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/debug_docstrings.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/function_images.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/github_links.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/has_attr_test.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/param_police.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.1.0.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.2.1.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.2.9.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.3.0.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.3.2.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.4.0.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.4.2.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.4.3.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/0.4.4.md
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.0.0.md
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.1.0.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.2.0.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.2.1.md
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.1.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.3.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.4.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.5.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.6.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.7.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.3.8.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.1.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.2.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.3.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.4.md
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.5.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.4.6.md
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.5.0.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.5.1.md
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.6.0.md
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.7.0.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.7.1.md
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.7.2.md
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.8.0.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.8.1.md
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.8.2.md
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.0.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.1.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.2.md
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.3.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.4.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.5.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.6.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.7.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/1.9.8.md
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/index.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 scanpy-1.9.8/docs/release-notes/release-latest.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/__main__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/_compat.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/_settings.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/_version.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/cli.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/logging.py
+-rw-r--r--   0        0        0    33877 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/readwrite.py
+-rw-r--r--   0        0        0    25286 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/_utils/__init__.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/_utils/compute/is_constant.py
+-rw-r--r--   0        0        0  1772368 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/10x_pbmc68k_reduced.h5ad
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/__init__.py
+-rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/_datasets.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/_ebi_expression_atlas.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/_utils.py
+-rw-r--r--   0        0        0    59808 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/krumsiek11.txt
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/datasets/toggleswitch.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/__init__.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/_docs.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/pp/__init__.py
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/pp/_normalization.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/experimental/pp/_recipes.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/__init__.py
+-rw-r--r--   0        0        0    21389 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/exporting.py
+-rw-r--r--   0        0        0    12971 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pl.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/__init__.py
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_bbknn.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_dca.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_harmony_integrate.py
+-rw-r--r--   0        0        0    15286 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_hashsolo.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_magic.py
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_mnn_correct.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_scanorama_integrate.py
+-rw-r--r--   0        0        0    21747 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/pp/_scrublet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/__init__.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_harmony_timeseries.py
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_palantir.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_phate.py
+-rw-r--r--   0        0        0     8553 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_phenograph.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_pypairs.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_sam.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_trimap.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/external/tl/_wishbone.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/get/__init__.py
+-rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/get/get.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/metrics/__init__.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/metrics/_gearys_c.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/metrics/_metrics.py
+-rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/metrics/_morans_i.py
+-rw-r--r--   0        0        0    40591 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/neighbors/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/__init__.py
+-rwxr-xr-x   0        0        0    87869 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_anndata.py
+-rw-r--r--   0        0        0    38801 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_baseplot_class.py
+-rw-r--r--   0        0        0    13507 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_docs.py
+-rw-r--r--   0        0        0    38017 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_dotplot.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_matrixplot.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_preprocessing.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_qc.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_rcmod.py
+-rw-r--r--   0        0        0    27060 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_stacked_violin.py
+-rw-r--r--   0        0        0    38870 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_utils.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/palettes.py
+-rw-r--r--   0        0        0    48883 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_tools/__init__.py
+-rw-r--r--   0        0        0    47494 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_tools/paga.py
+-rw-r--r--   0        0        0    43553 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/plotting/_tools/scatterplots.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/__init__.py
+-rw-r--r--   0        0        0    11613 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_combat.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_distributed.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_docs.py
+-rw-r--r--   0        0        0    22714 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_highly_variable_genes.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_normalization.py
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_pca.py
+-rw-r--r--   0        0        0    14152 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_qc.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_recipes.py
+-rw-r--r--   0        0        0    36555 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_simple.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_utils.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_deprecated/__init__.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/preprocessing/_deprecated/highly_variable_genes.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/queries/__init__.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/queries/_queries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/sim_models/__init__.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/sim_models/krumsiek11.txt
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/sim_models/krumsiek11_params.txt
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/sim_models/toggleswitch.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/sim_models/toggleswitch_params.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/__init__.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_helpers/__init__.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_helpers/data.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_pytest/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_pytest/marks.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_pytest/fixtures/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/testing/_pytest/fixtures/data.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/__init__.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_dendrogram.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_diffmap.py
+-rw-r--r--   0        0        0    49576 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_dpt.py
+-rw-r--r--   0        0        0     7003 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_draw_graph.py
+-rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_embedding_density.py
+-rw-r--r--   0        0        0    20102 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_ingest.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_leiden.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_louvain.py
+-rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_marker_gene_overlap.py
+-rw-r--r--   0        0        0    24674 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_paga.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_pca.py
+-rw-r--r--   0        0        0    29307 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_rank_genes_groups.py
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_score_genes.py
+-rw-r--r--   0        0        0    46842 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_sim.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_top_genes.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_tsne.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_umap.py
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_utils.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scanpy-1.9.8/scanpy/tools/_utils_clustering.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 scanpy-1.9.8/.gitignore
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scanpy-1.9.8/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scanpy-1.9.8/README.md
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 scanpy-1.9.8/pyproject.toml
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 scanpy-1.9.8/PKG-INFO
```

### Comparing `scanpy-1.9.7/.azure-pipelines.yml` & `scanpy-1.9.8/.azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.flake8` & `scanpy-1.9.8/.flake8`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.pre-commit-config.yaml` & `scanpy-1.9.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/CONTRIBUTING.md` & `scanpy-1.9.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.github/ISSUE_TEMPLATE/bug-report.yml` & `scanpy-1.9.8/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.github/ISSUE_TEMPLATE/bug_report.md` & `scanpy-1.9.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.github/ISSUE_TEMPLATE/enhancement-request.md` & `scanpy-1.9.8/.github/ISSUE_TEMPLATE/enhancement-request.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.github/workflows/check-pr.yml` & `scanpy-1.9.8/.github/workflows/check-pr.yml`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/Makefile` & `scanpy-1.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_key_contributors.rst` & `scanpy-1.9.8/docs/_key_contributors.rst`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/api.md` & `scanpy-1.9.8/docs/api.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/community.md` & `scanpy-1.9.8/docs/community.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/conf.py` & `scanpy-1.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/ecosystem.md` & `scanpy-1.9.8/docs/ecosystem.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/external.md` & `scanpy-1.9.8/docs/external.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/index.md` & `scanpy-1.9.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/installation.md` & `scanpy-1.9.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/news.md` & `scanpy-1.9.8/docs/news.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/references.rst` & `scanpy-1.9.8/docs/references.rst`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/tutorials.md` & `scanpy-1.9.8/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/usage-principles.md` & `scanpy-1.9.8/docs/usage-principles.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/Scanpy_Logo.svg` & `scanpy-1.9.8/docs/_static/img/Scanpy_Logo.svg`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/Scanpy_Logo_BrightFG.svg` & `scanpy-1.9.8/docs/_static/img/Scanpy_Logo_BrightFG.svg`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/Scanpy_Logo_RGB.png` & `scanpy-1.9.8/docs/_static/img/Scanpy_Logo_RGB.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/ci_plot-view_attachment-tab.png` & `scanpy-1.9.8/docs/_static/img/ci_plot-view_attachment-tab.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/ci_plot-view_select-test.png` & `scanpy-1.9.8/docs/_static/img/ci_plot-view_select-test.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/ci_plot-view_tests-tab.png` & `scanpy-1.9.8/docs/_static/img/ci_plot-view_tests-tab.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/spatial-basic-analysis.png` & `scanpy-1.9.8/docs/_static/img/spatial-basic-analysis.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/stacked_violin_dotplot_matrixplot.png` & `scanpy-1.9.8/docs/_static/img/stacked_violin_dotplot_matrixplot.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/paga_paul15.png` & `scanpy-1.9.8/docs/_static/img/tutorials/paga_paul15.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/paga_planaria.png` & `scanpy-1.9.8/docs/_static/img/tutorials/paga_planaria.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170430_krumsiek11/timeseries.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170430_krumsiek11/timeseries.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/NKG7.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/NKG7.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/cell_types.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/cell_types.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/filter_genes_dispersion.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/filter_genes_dispersion.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/louvain.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/louvain.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170505_seurat/violin.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170505_seurat/violin.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_static/img/tutorials/170522_visualizing_one_million_cells/tsne_1.3M.png` & `scanpy-1.9.8/docs/_static/img/tutorials/170522_visualizing_one_million_cells/tsne_1.3M.png`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/_templates/autosummary/class.rst` & `scanpy-1.9.8/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/ci.md` & `scanpy-1.9.8/docs/dev/ci.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/code.md` & `scanpy-1.9.8/docs/dev/code.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/documentation.md` & `scanpy-1.9.8/docs/dev/documentation.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/external-tools.md` & `scanpy-1.9.8/docs/dev/external-tools.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/getting-set-up.md` & `scanpy-1.9.8/docs/dev/getting-set-up.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/index.md` & `scanpy-1.9.8/docs/dev/index.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/release.md` & `scanpy-1.9.8/docs/dev/release.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/testing.md` & `scanpy-1.9.8/docs/dev/testing.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/dev/versioning.md` & `scanpy-1.9.8/docs/dev/versioning.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/extensions/debug_docstrings.py` & `scanpy-1.9.8/docs/extensions/debug_docstrings.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/extensions/function_images.py` & `scanpy-1.9.8/docs/extensions/function_images.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/extensions/github_links.py` & `scanpy-1.9.8/docs/extensions/github_links.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/extensions/param_police.py` & `scanpy-1.9.8/docs/extensions/param_police.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/extensions/typed_returns.py` & `scanpy-1.9.8/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.0.0.md` & `scanpy-1.9.8/docs/release-notes/1.0.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.1.0.md` & `scanpy-1.9.8/docs/release-notes/1.1.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.3.1.md` & `scanpy-1.9.8/docs/release-notes/1.3.1.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.3.3.md` & `scanpy-1.9.8/docs/release-notes/1.3.3.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.3.6.md` & `scanpy-1.9.8/docs/release-notes/1.3.6.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.4.1.md` & `scanpy-1.9.8/docs/release-notes/1.4.1.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.4.2.md` & `scanpy-1.9.8/docs/release-notes/1.4.2.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.4.5.md` & `scanpy-1.9.8/docs/release-notes/1.4.5.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.4.6.md` & `scanpy-1.9.8/docs/release-notes/1.4.6.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.5.0.md` & `scanpy-1.9.8/docs/release-notes/1.5.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.6.0.md` & `scanpy-1.9.8/docs/release-notes/1.6.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.7.0.md` & `scanpy-1.9.8/docs/release-notes/1.7.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.7.1.md` & `scanpy-1.9.8/docs/release-notes/1.7.1.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.7.2.md` & `scanpy-1.9.8/docs/release-notes/1.7.2.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.8.0.md` & `scanpy-1.9.8/docs/release-notes/1.8.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.8.2.md` & `scanpy-1.9.8/docs/release-notes/1.8.2.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.9.0.md` & `scanpy-1.9.8/docs/release-notes/1.9.0.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.9.2.md` & `scanpy-1.9.8/docs/release-notes/1.9.2.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.9.4.md` & `scanpy-1.9.8/docs/release-notes/1.9.4.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.9.6.md` & `scanpy-1.9.8/docs/release-notes/1.9.6.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/1.9.7.md` & `scanpy-1.9.8/docs/release-notes/1.9.7.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/docs/release-notes/index.md` & `scanpy-1.9.8/docs/release-notes/index.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/__init__.py` & `scanpy-1.9.8/scanpy/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/_settings.py` & `scanpy-1.9.8/scanpy/_settings.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/cli.py` & `scanpy-1.9.8/scanpy/cli.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/logging.py` & `scanpy-1.9.8/scanpy/logging.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/readwrite.py` & `scanpy-1.9.8/scanpy/readwrite.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/_utils/__init__.py` & `scanpy-1.9.8/scanpy/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/_utils/compute/is_constant.py` & `scanpy-1.9.8/scanpy/_utils/compute/is_constant.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/10x_pbmc68k_reduced.h5ad` & `scanpy-1.9.8/scanpy/datasets/10x_pbmc68k_reduced.h5ad`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/_datasets.py` & `scanpy-1.9.8/scanpy/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/_ebi_expression_atlas.py` & `scanpy-1.9.8/scanpy/datasets/_ebi_expression_atlas.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/_utils.py` & `scanpy-1.9.8/scanpy/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/krumsiek11.txt` & `scanpy-1.9.8/scanpy/datasets/krumsiek11.txt`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/datasets/toggleswitch.txt` & `scanpy-1.9.8/scanpy/datasets/toggleswitch.txt`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/experimental/_docs.py` & `scanpy-1.9.8/scanpy/experimental/_docs.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/experimental/pp/_highly_variable_genes.py` & `scanpy-1.9.8/scanpy/experimental/pp/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/experimental/pp/_normalization.py` & `scanpy-1.9.8/scanpy/experimental/pp/_normalization.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/experimental/pp/_recipes.py` & `scanpy-1.9.8/scanpy/experimental/pp/_recipes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/exporting.py` & `scanpy-1.9.8/scanpy/external/exporting.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pl.py` & `scanpy-1.9.8/scanpy/external/pl.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_bbknn.py` & `scanpy-1.9.8/scanpy/external/pp/_bbknn.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_dca.py` & `scanpy-1.9.8/scanpy/external/pp/_dca.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_harmony_integrate.py` & `scanpy-1.9.8/scanpy/external/pp/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_hashsolo.py` & `scanpy-1.9.8/scanpy/external/pp/_hashsolo.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_magic.py` & `scanpy-1.9.8/scanpy/external/pp/_magic.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_mnn_correct.py` & `scanpy-1.9.8/scanpy/external/pp/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_scanorama_integrate.py` & `scanpy-1.9.8/scanpy/external/pp/_scanorama_integrate.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/pp/_scrublet.py` & `scanpy-1.9.8/scanpy/external/pp/_scrublet.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_harmony_timeseries.py` & `scanpy-1.9.8/scanpy/external/tl/_harmony_timeseries.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_palantir.py` & `scanpy-1.9.8/scanpy/external/tl/_palantir.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_phate.py` & `scanpy-1.9.8/scanpy/external/tl/_phate.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_phenograph.py` & `scanpy-1.9.8/scanpy/external/tl/_phenograph.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_pypairs.py` & `scanpy-1.9.8/scanpy/external/tl/_pypairs.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_sam.py` & `scanpy-1.9.8/scanpy/external/tl/_sam.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_trimap.py` & `scanpy-1.9.8/scanpy/external/tl/_trimap.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/external/tl/_wishbone.py` & `scanpy-1.9.8/scanpy/external/tl/_wishbone.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/get/get.py` & `scanpy-1.9.8/scanpy/get/get.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/metrics/_gearys_c.py` & `scanpy-1.9.8/scanpy/metrics/_gearys_c.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/metrics/_metrics.py` & `scanpy-1.9.8/scanpy/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/metrics/_morans_i.py` & `scanpy-1.9.8/scanpy/metrics/_morans_i.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/neighbors/__init__.py` & `scanpy-1.9.8/scanpy/neighbors/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/__init__.py` & `scanpy-1.9.8/scanpy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_anndata.py` & `scanpy-1.9.8/scanpy/plotting/_anndata.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_baseplot_class.py` & `scanpy-1.9.8/scanpy/plotting/_baseplot_class.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_docs.py` & `scanpy-1.9.8/scanpy/plotting/_docs.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_dotplot.py` & `scanpy-1.9.8/scanpy/plotting/_dotplot.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_matrixplot.py` & `scanpy-1.9.8/scanpy/plotting/_matrixplot.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_preprocessing.py` & `scanpy-1.9.8/scanpy/plotting/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_qc.py` & `scanpy-1.9.8/scanpy/plotting/_qc.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_rcmod.py` & `scanpy-1.9.8/scanpy/plotting/_rcmod.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_stacked_violin.py` & `scanpy-1.9.8/scanpy/plotting/_stacked_violin.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_utils.py` & `scanpy-1.9.8/scanpy/plotting/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,16 +349,16 @@
                     f"The following color value found in adata.uns['{key}_colors'] "
                     f"is not valid: '{color}'. Default colors will be used instead."
                 )
                 _set_default_colors_for_categorical_obs(adata, key)
                 _palette = None
                 break
         _palette.append(color)
-    # Don't modify if nothing changed
-    if _palette is None or np.equal(_palette, adata.uns[color_key]).all():
+    # Don’t modify if nothing changed
+    if _palette is None or np.array_equal(_palette, adata.uns[color_key]):
         return
     adata.uns[color_key] = _palette
 
 
 def _set_colors_for_categorical_obs(
     adata, value_to_plot, palette: Union[str, Sequence[str], Cycler]
 ):
```

### Comparing `scanpy-1.9.7/scanpy/plotting/palettes.py` & `scanpy-1.9.8/scanpy/plotting/palettes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_tools/__init__.py` & `scanpy-1.9.8/scanpy/plotting/_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_tools/paga.py` & `scanpy-1.9.8/scanpy/plotting/_tools/paga.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/plotting/_tools/scatterplots.py` & `scanpy-1.9.8/scanpy/plotting/_tools/scatterplots.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/__init__.py` & `scanpy-1.9.8/scanpy/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_combat.py` & `scanpy-1.9.8/scanpy/preprocessing/_combat.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_docs.py` & `scanpy-1.9.8/scanpy/preprocessing/_docs.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_highly_variable_genes.py` & `scanpy-1.9.8/scanpy/preprocessing/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_normalization.py` & `scanpy-1.9.8/scanpy/preprocessing/_normalization.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_pca.py` & `scanpy-1.9.8/scanpy/preprocessing/_pca.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_qc.py` & `scanpy-1.9.8/scanpy/preprocessing/_qc.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_recipes.py` & `scanpy-1.9.8/scanpy/preprocessing/_recipes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_simple.py` & `scanpy-1.9.8/scanpy/preprocessing/_simple.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_utils.py` & `scanpy-1.9.8/scanpy/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_deprecated/__init__.py` & `scanpy-1.9.8/scanpy/preprocessing/_deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/preprocessing/_deprecated/highly_variable_genes.py` & `scanpy-1.9.8/scanpy/preprocessing/_deprecated/highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/queries/_queries.py` & `scanpy-1.9.8/scanpy/queries/_queries.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/sim_models/krumsiek11.txt` & `scanpy-1.9.8/scanpy/sim_models/krumsiek11.txt`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_helpers/__init__.py` & `scanpy-1.9.8/scanpy/testing/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_helpers/data.py` & `scanpy-1.9.8/scanpy/testing/_helpers/data.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_pytest/__init__.py` & `scanpy-1.9.8/scanpy/testing/_pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_pytest/marks.py` & `scanpy-1.9.8/scanpy/testing/_pytest/marks.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_pytest/fixtures/__init__.py` & `scanpy-1.9.8/scanpy/testing/_pytest/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/testing/_pytest/fixtures/data.py` & `scanpy-1.9.8/scanpy/testing/_pytest/fixtures/data.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/__init__.py` & `scanpy-1.9.8/scanpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_dendrogram.py` & `scanpy-1.9.8/scanpy/tools/_dendrogram.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_diffmap.py` & `scanpy-1.9.8/scanpy/tools/_diffmap.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_dpt.py` & `scanpy-1.9.8/scanpy/tools/_dpt.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_draw_graph.py` & `scanpy-1.9.8/scanpy/tools/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_embedding_density.py` & `scanpy-1.9.8/scanpy/tools/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_ingest.py` & `scanpy-1.9.8/scanpy/tools/_ingest.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_leiden.py` & `scanpy-1.9.8/scanpy/tools/_leiden.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_louvain.py` & `scanpy-1.9.8/scanpy/tools/_louvain.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_marker_gene_overlap.py` & `scanpy-1.9.8/scanpy/tools/_marker_gene_overlap.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_paga.py` & `scanpy-1.9.8/scanpy/tools/_paga.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_rank_genes_groups.py` & `scanpy-1.9.8/scanpy/tools/_rank_genes_groups.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_score_genes.py` & `scanpy-1.9.8/scanpy/tools/_score_genes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_sim.py` & `scanpy-1.9.8/scanpy/tools/_sim.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_top_genes.py` & `scanpy-1.9.8/scanpy/tools/_top_genes.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_tsne.py` & `scanpy-1.9.8/scanpy/tools/_tsne.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_umap.py` & `scanpy-1.9.8/scanpy/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_utils.py` & `scanpy-1.9.8/scanpy/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/scanpy/tools/_utils_clustering.py` & `scanpy-1.9.8/scanpy/tools/_utils_clustering.py`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/.gitignore` & `scanpy-1.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/LICENSE` & `scanpy-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/README.md` & `scanpy-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/pyproject.toml` & `scanpy-1.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scanpy-1.9.7/PKG-INFO` & `scanpy-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpy
-Version: 1.9.7
+Version: 1.9.8
 Summary: Single-Cell Analysis in Python.
 Project-URL: Documentation, https://scanpy.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/scanpy
 Project-URL: Home-page, https://scanpy.org
 Author: Alex Wolf, Philipp Angerer, Fidel Ramirez, Isaac Virshup, Sergei Rybakov, Gokcen Eraslan, Tom White, Malte Luecken, Davide Cittaro, Tobias Callies, Marius Lange, Andrés R. Muñoz-Rojas
 Maintainer-email: Isaac Virshup <ivirshup@gmail.com>, Philipp Angerer <phil.angerer@gmail.com>, Alex Wolf <f.alex.wolf@gmx.de>
 License-Expression: BSD-3-Clause
```

