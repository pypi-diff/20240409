# Comparing `tmp/ALLCools-1.0.8.tar.gz` & `tmp/allcools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALLCools-1.0.8.tar", last modified: Fri Sep 23 06:50:55 2022, max compression
+gzip compressed data, was "allcools-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ALLCools-1.0.8.tar` & `allcools-1.1.0.tar`

### file list

```diff
@@ -1,104 +1,107 @@
--rw-r--r--   0        0        0      154 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/__init__.py
--rw-r--r--   0        0        0    27909 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/__main__.py
--rw-r--r--   0        0        0     8723 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_allc_to_bigwig.py
--rw-r--r--   0        0        0    14129 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_allc_to_region_count.py
--rw-r--r--   0        0        0    18951 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_bam_to_allc.py
--rw-r--r--   0        0        0     9228 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_doc.py
--rw-r--r--   0        0        0    14869 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_extract_allc.py
--rw-r--r--   0        0        0    19061 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_merge_allc.py
--rw-r--r--   0        0        0    15305 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_open.py
--rw-r--r--   0        0        0       32 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/abc/__init__.py
--rw-r--r--   0        0        0    13031 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/abc/abc_score.py
--rw-r--r--   0        0        0      624 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/api.py
--rw-r--r--   0        0        0     5835 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/ClusterMerging.py
--rw-r--r--   0        0        0    29849 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/ConsensusClustering.py
--rw-r--r--   0        0        0      638 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/__init__.py
--rw-r--r--   0        0        0     6057 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/art_of_tsne.py
--rw-r--r--   0        0        0    12785 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/balanced_pca.py
--rw-r--r--   0        0        0      910 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/chromatin_conformation.py
--rw-r--r--   0        0        0    17669 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/dmg.py
--rw-r--r--   0        0        0       86 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/__init__.py
--rw-r--r--   0        0        0     6700 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/coverage_doublets.py
--rw-r--r--   0        0        0    10214 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/scrublet.py
--rw-r--r--   0        0        0      113 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/__init__.py
--rw-r--r--   0        0        0    10574 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/feature_enrichment.py
--rw-r--r--   0        0        0     3393 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/gene_panel_design.py
--rw-r--r--   0        0        0     7821 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/incremental_pca.py
--rw-r--r--   0        0        0     5944 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/lsi.py
--rw-r--r--   0        0        0     3696 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/mcad.py
--rw-r--r--   0        0        0     5578 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/clustering/pvclust.py
--rw-r--r--   0        0        0      643 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/clustering/rutilities.py
--rw-r--r--   0        0        0       66 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/__init__.py
--rw-r--r--   0        0        0      114 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/atac.py
--rw-r--r--   0        0        0    23961 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/base_ds.py
--rw-r--r--   0        0        0    14453 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/dataset.py
--rw-r--r--   0        0        0    10291 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/h5ad.py
--rw-r--r--   0        0        0     5839 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/mcad.py
--rw-r--r--   0        0        0    18533 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/mcds.py
--rw-r--r--   0        0        0     4562 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/snap.py
--rw-r--r--   0        0        0     1873 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/zarr.py
--rw-r--r--   0        0        0       41 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/__init__.py
--rw-r--r--   0        0        0      168 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/dataset.yaml
--rw-r--r--   0        0        0     2041 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/directory_structure.py
--rw-r--r--   0        0        0      181 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/entry_point.py
--rw-r--r--   0        0        0      133 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/__init__.py
--rw-r--r--   0        0        0     8795 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dmr.py
--rw-r--r--   0        0        0     6644 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dmr_baseds.py
--rw-r--r--   0        0        0     7321 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dms.py
--rw-r--r--   0        0        0     8561 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dms_baseds.py
--rw-r--r--   0        0        0     2461 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/parse_methylpy.py
--rw-r--r--   0        0        0     4503 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/rms_test.py
--rw-r--r--   0        0        0        0 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/genomic/__init__.py
--rw-r--r--   0        0        0     5639 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/Gtf.py
--rw-r--r--   0        0        0       80 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/__init__.py
--rw-r--r--   0        0        0     1164 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/utilities.py
--rw-r--r--   0        0        0      195 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/__init__.py
--rw-r--r--   0        0        0    12276 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/cca.py
--rw-r--r--   0        0        0     6554 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/confusion.py
--rw-r--r--   0        0        0     9912 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/metric.py
--rw-r--r--   0        0        0    32816 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/seurat_class.py
--rw-r--r--   0        0        0     4794 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/jbrowse/__init__.py
--rw-r--r--   0        0        0      124 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/__init__.py
--rw-r--r--   0        0        0    25737 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/base_ds.py
--rw-r--r--   0        0        0    11587 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/correlation.py
--rw-r--r--   0        0        0    57790 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/mcds.py
--rw-r--r--   0        0        0    39343 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/region_ds.py
--rw-r--r--   0        0        0    19345 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/utilities.py
--rw-r--r--   0        0        0       75 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/motif/__init__.py
--rw-r--r--   0        0        0  1614001 2022-09-23 06:50:34.767006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme
--rw-r--r--   0        0        0   172054 2022-09-23 06:50:34.767006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv
--rw-r--r--   0        0        0    77918 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv
--rw-r--r--   0        0        0        0 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/__init__.py
--rw-r--r--   0        0        0     8709 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/motifs.py
--rw-r--r--   0        0        0     4260 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/parse_meme.py
--rw-r--r--   0        0        0     4864 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/snakemake.py
--rw-r--r--   0        0        0      306 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/__init__.py
--rw-r--r--   0        0        0     9026 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/categorical_scatter.py
--rw-r--r--   0        0        0     4512 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/color.py
--rw-r--r--   0        0        0     7704 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/continuous_scatter.py
--rw-r--r--   0        0        0     1429 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/contour.py
--rw-r--r--   0        0        0     2645 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/decomposition.py
--rw-r--r--   0        0        0     7940 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/dendro.py
--rw-r--r--   0        0        0    12573 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/GtfTrack.py
--rw-r--r--   0        0        0    10256 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py
--rw-r--r--   0        0        0       55 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/__init__.py
--rw-r--r--   0        0        0    37598 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/_pygenometrack.py
--rw-r--r--   0        0        0     1026 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/interactive_scatter.py
--rw-r--r--   0        0        0     7382 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/qc_plots.py
--rw-r--r--   0        0        0      833 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/size.py
--rw-r--r--   0        0        0     7469 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/sunburst.py
--rw-r--r--   0        0        0     2083 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/text_anno_scatter.py
--rw-r--r--   0        0        0     7410 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/utilities.py
--rw-r--r--   0        0        0      166 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/__init__.py
--rw-r--r--   0        0        0     6211 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_kmeans.py
--rw-r--r--   0        0        0    10950 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_knn.py
--rw-r--r--   0        0        0       29 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/reptile/__init__.py
--rw-r--r--   0        0        0    31804 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/reptile/reptile.py
--rw-r--r--   0        0        0        0 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/schema/__init__.py
--rw-r--r--   0        0        0      894 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/schema/mcds_schema.py
--rw-r--r--   0        0        0    11318 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/table_to_allc.py
--rw-r--r--   0        0        0    18046 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/utilities.py
--rw-r--r--   0        0        0     1073 2022-09-23 06:50:34.771006 ALLCools-1.0.8/LICENSE
--rw-r--r--   0        0        0      339 2022-09-23 06:50:34.771006 ALLCools-1.0.8/README.md
--rw-r--r--   0        0        0     2018 2022-09-23 06:50:35.059016 ALLCools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2127 1970-01-01 00:00:00.000000 ALLCools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      154 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/__init__.py
+-rw-r--r--   0        0        0    27909 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/__main__.py
+-rw-r--r--   0        0        0     8723 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_allc_to_bigwig.py
+-rw-r--r--   0        0        0    14233 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_allc_to_region_count.py
+-rw-r--r--   0        0        0    18951 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_bam_to_allc.py
+-rw-r--r--   0        0        0     9228 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_doc.py
+-rw-r--r--   0        0        0    14905 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_extract_allc.py
+-rw-r--r--   0        0        0    19061 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_merge_allc.py
+-rw-r--r--   0        0        0    18063 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/_open.py
+-rw-r--r--   0        0        0       32 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/abc/__init__.py
+-rw-r--r--   0        0        0    13031 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/abc/abc_score.py
+-rw-r--r--   0        0        0      624 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/api.py
+-rw-r--r--   0        0        0     5834 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/ClusterMerging.py
+-rw-r--r--   0        0        0    29959 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/ConsensusClustering.py
+-rw-r--r--   0        0        0      638 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/__init__.py
+-rw-r--r--   0        0        0     6057 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/art_of_tsne.py
+-rw-r--r--   0        0        0    12836 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/balanced_pca.py
+-rw-r--r--   0        0        0      910 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/chromatin_conformation.py
+-rw-r--r--   0        0        0    17639 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/dmg.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/doublets/__init__.py
+-rw-r--r--   0        0        0     6699 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/doublets/coverage_doublets.py
+-rw-r--r--   0        0        0    10214 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/doublets/scrublet.py
+-rw-r--r--   0        0        0      113 2024-04-09 16:13:03.320026 allcools-1.1.0/ALLCools/clustering/feature_selection/__init__.py
+-rw-r--r--   0        0        0    10574 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/feature_selection/feature_enrichment.py
+-rw-r--r--   0        0        0     3393 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/feature_selection/gene_panel_design.py
+-rw-r--r--   0        0        0     7821 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/incremental_pca.py
+-rw-r--r--   0        0        0     5945 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/lsi.py
+-rw-r--r--   0        0        0     4128 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/mcad.py
+-rw-r--r--   0        0        0     5578 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/pvclust.py
+-rw-r--r--   0        0        0      643 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/clustering/rutilities.py
+-rw-r--r--   0        0        0       66 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/atac.py
+-rw-r--r--   0        0        0    23961 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/base_ds.py
+-rw-r--r--   0        0        0    14453 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/dataset.py
+-rw-r--r--   0        0        0    10291 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/h5ad.py
+-rw-r--r--   0        0        0     5839 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/mcad.py
+-rw-r--r--   0        0        0    18713 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/mcds.py
+-rw-r--r--   0        0        0     4562 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/snap.py
+-rw-r--r--   0        0        0     1873 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/count_matrix/zarr.py
+-rw-r--r--   0        0        0       41 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dataset/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dataset/dataset.yaml
+-rw-r--r--   0        0        0     2041 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dataset/directory_structure.py
+-rw-r--r--   0        0        0      181 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dataset/entry_point.py
+-rw-r--r--   0        0        0      133 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/__init__.py
+-rw-r--r--   0        0        0     8795 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/call_dmr.py
+-rw-r--r--   0        0        0     7010 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/call_dmr_baseds.py
+-rw-r--r--   0        0        0     7321 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/call_dms.py
+-rw-r--r--   0        0        0     9459 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/call_dms_baseds.py
+-rw-r--r--   0        0        0     2461 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/parse_methylpy.py
+-rw-r--r--   0        0        0     4503 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/dmr/rms_test.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/genomic/__init__.py
+-rw-r--r--   0        0        0     5639 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/gtf/Gtf.py
+-rw-r--r--   0        0        0       80 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/gtf/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/gtf/utilities.py
+-rw-r--r--   0        0        0      195 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/integration/__init__.py
+-rw-r--r--   0        0        0    12569 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/integration/cca.py
+-rw-r--r--   0        0        0     7943 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/integration/confusion.py
+-rw-r--r--   0        0        0     9912 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/integration/metric.py
+-rw-r--r--   0        0        0    31959 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/integration/seurat_class.py
+-rw-r--r--   0        0        0     4794 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/jbrowse/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/__init__.py
+-rw-r--r--   0        0        0    27019 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/base_ds.py
+-rw-r--r--   0        0        0    13557 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/cool_ds.py
+-rw-r--r--   0        0        0    14383 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/correlation.py
+-rw-r--r--   0        0        0    57795 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/mcds.py
+-rw-r--r--   0        0        0    39474 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/region_ds.py
+-rw-r--r--   0        0        0    19429 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/mcds/utilities.py
+-rw-r--r--   0        0        0      163 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/motif/__init__.py
+-rw-r--r--   0        0        0     4074 2024-04-09 16:13:03.324026 allcools-1.1.0/ALLCools/motif/cistarget.py
+-rw-r--r--   0        0        0  1614001 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme
+-rw-r--r--   0        0        0   172054 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv
+-rw-r--r--   0        0        0    77918 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv
+-rw-r--r--   0        0        0        0 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/default_motif_set/__init__.py
+-rw-r--r--   0        0        0     3478 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/dem.py
+-rw-r--r--   0        0        0     8709 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/motifs.py
+-rw-r--r--   0        0        0     4260 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/parse_meme.py
+-rw-r--r--   0        0        0     4864 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/motif/snakemake.py
+-rw-r--r--   0        0        0      324 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/__init__.py
+-rw-r--r--   0        0        0     9026 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/categorical_scatter.py
+-rw-r--r--   0        0        0     4512 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/color.py
+-rw-r--r--   0        0        0     7704 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/continuous_scatter.py
+-rw-r--r--   0        0        0     1429 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/contour.py
+-rw-r--r--   0        0        0     2645 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/decomposition.py
+-rw-r--r--   0        0        0     7940 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/dendro.py
+-rw-r--r--   0        0        0    12573 2024-04-09 16:13:03.332026 allcools-1.1.0/ALLCools/plot/genome_track/GtfTrack.py
+-rw-r--r--   0        0        0    10256 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py
+-rw-r--r--   0        0        0       55 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/genome_track/__init__.py
+-rw-r--r--   0        0        0    37598 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/genome_track/_pygenometrack.py
+-rw-r--r--   0        0        0     1956 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/interactive_scatter.py
+-rw-r--r--   0        0        0     7382 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/qc_plots.py
+-rw-r--r--   0        0        0      833 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/size.py
+-rw-r--r--   0        0        0     7469 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/sunburst.py
+-rw-r--r--   0        0        0     2083 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/text_anno_scatter.py
+-rw-r--r--   0        0        0     7852 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/plot/utilities.py
+-rw-r--r--   0        0        0      166 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/pseudo_cell/__init__.py
+-rw-r--r--   0        0        0     6211 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/pseudo_cell/pseudo_cell_kmeans.py
+-rw-r--r--   0        0        0    10949 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/pseudo_cell/pseudo_cell_knn.py
+-rw-r--r--   0        0        0       29 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/reptile/__init__.py
+-rw-r--r--   0        0        0    31804 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/reptile/reptile.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/schema/__init__.py
+-rw-r--r--   0        0        0      894 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/schema/mcds_schema.py
+-rw-r--r--   0        0        0    11318 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/table_to_allc.py
+-rw-r--r--   0        0        0    18046 2024-04-09 16:13:03.336026 allcools-1.1.0/ALLCools/utilities.py
+-rw-r--r--   0        0        0     1073 2024-04-09 16:13:03.336026 allcools-1.1.0/LICENSE
+-rw-r--r--   0        0        0      339 2024-04-09 16:13:03.336026 allcools-1.1.0/README.md
+-rw-r--r--   0        0        0     2004 2024-04-09 16:13:03.592026 allcools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 allcools-1.1.0/PKG-INFO
```

### Comparing `ALLCools-1.0.8/ALLCools/__main__.py` & `allcools-1.1.0/ALLCools/__main__.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/_allc_to_bigwig.py` & `allcools-1.1.0/ALLCools/_allc_to_bigwig.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/_allc_to_region_count.py` & `allcools-1.1.0/ALLCools/_allc_to_region_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     bin_sizes_doc=bin_sizes_doc,
     region_bed_paths_doc=region_bed_paths_doc,
     region_bed_names_doc=region_bed_names_doc,
     binarize_doc=binarize_doc,
 )
 def allc_to_region_count(
     allc_path: str,
+    cmeta_path: str,
     output_prefix: str,
     chrom_size_path: str,
     mc_contexts: List[str],
     split_strand: bool = False,
     region_bed_paths: List[str] = None,
     region_bed_names: List[str] = None,
     bin_sizes: List[int] = None,
@@ -211,14 +212,15 @@
                 )
 
     # print('Extract ALLC context')
     output_prefix = output_prefix.rstrip(".")
     strandness = "split" if split_strand else "both"
     output_paths_dict = extract_allc(
         allc_path=allc_path,
+        cmeta_path=cmeta_path,
         output_prefix=output_prefix,
         mc_contexts=mc_contexts,
         strandness=strandness,
         output_format="bed5",
         chrom_size_path=chrom_size_path,
         region=None,
         cov_cutoff=cov_cutoff,
@@ -328,18 +330,19 @@
             )
             bed_df["int_id"] = list(range(0, bed_df.shape[0]))
             bed_df["int_id"].to_hdf(output_dir / f"REGION_ID_{region_name}.hdf", key="data")
             bed_df.iloc[:, :3].to_hdf(output_dir / f"REGION_BED_chrom{bin_size_chr}.hdf", key="data")
 
     with ProcessPoolExecutor(cpu) as executor:
         futures = {}
-        for cell_id, allc_path in allc_series.iteritems():
+        for cell_id, (allc_path, cmeta_path) in allc_series.iterrows():
             future = executor.submit(
                 allc_to_region_count,
                 allc_path=allc_path,
+                cmeta_path=cmeta_path,
                 output_prefix=str(output_dir / cell_id),
                 chrom_size_path=chrom_size_path,
                 mc_contexts=mc_contexts,
                 split_strand=split_strand,
                 region_bed_paths=region_bed_paths,
                 region_bed_names=region_bed_names,
                 bin_sizes=bin_sizes,
```

### Comparing `ALLCools-1.0.8/ALLCools/_bam_to_allc.py` & `allcools-1.1.0/ALLCools/_bam_to_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/_doc.py` & `allcools-1.1.0/ALLCools/_doc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/_extract_allc.py` & `allcools-1.1.0/ALLCools/_extract_allc.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 cur_chrom = cur_line[0]
                 continue
             if prev_line is None:
                 prev_line = cur_line
                 continue
             else:
                 # pos should be continuous, strand should be reverse
-                if int(prev_line[1]) + 1 == int(cur_line[1]) and prev_line[2] != cur_line[2]:
+                if int(prev_line[1]) + 1 == int(cur_line[1]) and prev_line[2] == "+":
                     new_line = prev_line[:4] + [
                         str(int(prev_line[4]) + int(cur_line[4])),
                         str(int(prev_line[5]) + int(cur_line[5])),
                         "1",
                     ]
                     prev_line = None
                 # otherwise, only write and update prev_line
@@ -215,14 +215,15 @@
     strandness_doc=strandness_doc,
     region_doc=region_doc,
     cpu_basic_doc=cpu_basic_doc,
     binarize_doc=binarize_doc,
 )
 def extract_allc(
     allc_path: str,
+    cmeta_path: str,
     output_prefix: str,
     mc_contexts: Union[str, list],
     chrom_size_path: str,
     strandness: str = "both",
     output_format: str = "allc",
     region: str = None,
     cov_cutoff: int = 9999,
@@ -342,15 +343,15 @@
             cpu=cpu,
             chunk_size=parallel_chunk_size,
             tabix=tabix,
         )
 
     # split file first
     # strandness function
-    with open_allc(allc_path, region=region) as allc:
+    with open_allc(allc_path, region=region, cmeta_path=cmeta_path) as allc:
         if strandness == "Split":
             for line in allc:
                 cur_line = line.split("\t")
                 if int(cur_line[5]) > cov_cutoff:
                     continue
                 try:
                     # key is (context, strand)
```

### Comparing `ALLCools-1.0.8/ALLCools/_merge_allc.py` & `allcools-1.1.0/ALLCools/_merge_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/_open.py` & `allcools-1.1.0/ALLCools/_open.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
+
 import codecs
 import gzip
 import os
 import pathlib
 import sys
 import time
 from subprocess import PIPE, Popen, run
@@ -202,15 +203,88 @@
     def readline(self):
         return self._file.readline()
 
     def _raise_if_error(self):
         """
         Raise an exception if the gzip process has exited with an error.
 
-        Raise IOError if process is not running anymore and the
+        Raise OSError if process is not running anymore and the
+        exit code is nonzero.
+        """
+        return_code = self.process.poll()
+        if return_code is not None and return_code != 0:
+            message = self._stderr.read().strip()
+            raise OSError(message)
+
+    def read(self, *args):
+        data = self._file.read(*args)
+        if len(args) == 0 or args[0] <= 0:
+            # wait for process to terminate until we check the exit code
+            self.process.wait()
+        self._raise_if_error()
+        return data
+
+
+class PipedBAllCReader(Closing):
+    def __init__(self, path, cmeta_path=None, region=None, mode="r"):
+        if mode not in ("r"):
+            raise ValueError(f"Mode can only be 'r' for ballc file")
+        if cmeta_path is None:
+            raise NotImplementedError
+        cmeta_path = pathlib.Path(cmeta_path).resolve()
+        if not cmeta_path.exists():
+            raise FileNotFoundError(f"{cmeta_path} does not exist.")
+        cmeta_path = str(cmeta_path)
+
+        if region is None:
+            self.process = Popen(
+                ["ballcools", "query", path, '"*"', "-c", cmeta_path],
+                # stdout=PIPE, stderr=PIPE, encoding="utf8")
+                stdout=PIPE,
+                stderr=PIPE,
+                encoding=None,
+            )
+        else:
+            self.process = Popen(
+                ["ballcools", "query", path] + region.split(" ") + ["-c", cmeta_path],
+                stdout=PIPE,
+                stderr=PIPE,
+                # encoding="utf8",)
+                encoding=None,
+            )
+
+        self.name = path
+        self._file = self.process.stdout
+        self._stderr = self.process.stderr
+        self.closed = False
+        # Give ballcools a little bit of time to report any errors
+        # (such as a non-existing file)
+        time.sleep(0.01)
+        self._raise_if_error()
+
+    def close(self):
+        self.closed = True
+        return_code = self.process.poll()
+        if return_code is None:
+            # still running
+            self.process.terminate()
+        self._raise_if_error()
+
+    def __iter__(self):
+        for line in self._file:
+            yield line.decode("utf-8")
+        self.process.wait()
+        self._raise_if_error()
+
+    def readline(self):
+        return self._file.readline().decode("utf-8")
+
+    def _raise_if_error(self):
+        """
+        Raise OSError if process is not running anymore and the
         exit code is nonzero.
         """
         return_code = self.process.poll()
         if return_code is not None and return_code != 0:
             message = self._stderr.read().strip()
             raise OSError(message)
 
@@ -271,15 +345,15 @@
         self.process.wait()
         self._raise_if_error()
 
     def readline(self):
         return self.file.readline()
 
     def _raise_if_error(self):
-        """Raise IOError if process is not running anymore and the exit code is nonzero."""
+        """Raise OSError if process is not running anymore and the exit code is nonzero."""
         return_code = self.process.poll()
         if return_code is not None and return_code != 0:
             message = self._stderr.read().strip()
             raise OSError(message)
 
     def read(self, *args):
         data = self.file.read(*args)
@@ -378,15 +452,19 @@
     else:
         try:
             return PipedGzipWriter(file_path, mode, compresslevel, threads=threads)
         except OSError:
             return gzip.open(file_path, mode, compresslevel=compresslevel)
 
 
-def open_allc(file_path, mode="r", compresslevel=3, threads=1, region=None):
+def open_ballc(file_path, mode="r", compresslevel=None, threads=None, region=None, cmeta_path=None):
+    return PipedBAllCReader(file_path, cmeta_path=cmeta_path, region=region, mode="r")
+
+
+def open_allc(file_path, mode="r", compresslevel=3, threads=1, region=None, cmeta_path=None):
     """
     Open a .allc file.
 
     A replacement for the "open" function that can also open files that have
     been compressed with gzip, bzip2 or xz. If the file_path is '-', standard
     output (mode 'w') or input (mode 'r') is returned.
 
@@ -418,29 +496,31 @@
 
     if mode in ("r", "w", "a"):
         mode += "t"
     if mode not in ("rt", "rb", "wt", "wb", "at", "ab"):
         raise ValueError(f"mode '{mode}' not supported")
     if compresslevel not in range(1, 10):
         raise ValueError("compresslevel must be between 1 and 9")
-    if region is not None:
+    if (region is not None) and (not file_path.endswith(".ballc")):
         # unzipped file
         if not file_path.endswith("gz"):
             raise ValueError(f"File must be compressed by bgzip to use region query. File path {file_path}")
         # normal gzipped file
         if not has_tabix(file_path):
             raise ValueError(
                 f"Tried inspect {file_path}, " "File is compressed by normal gzip, but region query only apply to bgzip"
             )
 
         if not os.path.exists(file_path + ".tbi"):
             raise FileNotFoundError("region query provided, but .tbi index not found")
 
-    if file_path.endswith("gz"):
+    if file_path.endswith(".gz"):
         return open_gz(file_path, mode, compresslevel, threads, region=region)
+    elif file_path.endswith(".ballc"):
+        return open_ballc(file_path, region=region, cmeta_path=cmeta_path)
     else:
         return open(file_path, mode)
 
 
 def has_tabix(filename):
     tabix_path = filename + ".tbi"
     if os.path.exists(tabix_path):
```

### Comparing `ALLCools-1.0.8/ALLCools/abc/abc_score.py` & `allcools-1.1.0/ALLCools/abc/abc_score.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/api.py` & `allcools-1.1.0/ALLCools/api.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/ClusterMerging.py` & `allcools-1.1.0/ALLCools/clustering/ClusterMerging.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         stop_criterion=None,
         stop_clusters=-1,
         n_cells=200,
         metric="euclidean",
         method="average",
         label_concat_str="::",
     ):
-
         self.data_for_tree = None
         self.cell_to_type = None
         self.gene_mcds = None
 
         self.n_cells = n_cells
         self.metric = metric
         self.method = method
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/ConsensusClustering.py` & `allcools-1.1.0/ALLCools/clustering/ConsensusClustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,22 @@
                 x=x,
                 y=cur_y,
                 frac=self.train_frac,
                 max_train=self.train_max_n,
                 random_state=self.random_state + cur_iter,
                 # every time train-test split got a different random state
             )
-            (clf, score, cluster_map, cmat, r1_cmat, r2_cmat,) = single_supervise_evaluation(
+            (
+                clf,
+                score,
+                cluster_map,
+                cmat,
+                r1_cmat,
+                r2_cmat,
+            ) = single_supervise_evaluation(
                 clf,
                 x_train,
                 y_train,
                 x_test,
                 y_test,
                 r1_norm_step=step,
                 r2_norm_step=step,
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/__init__.py` & `allcools-1.1.0/ALLCools/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/art_of_tsne.py` & `allcools-1.1.0/ALLCools/clustering/art_of_tsne.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/balanced_pca.py` & `allcools-1.1.0/ALLCools/clustering/balanced_pca.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Perform Balanced PCA as well as Reproducible PCA.
 
 A class allow user provide fitted model and just transform MCDS to adata with PCs.
 """
+
 import anndata
 import joblib
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from scipy.stats import ks_2samp
 from sklearn.preprocessing import RobustScaler, StandardScaler
@@ -115,15 +116,17 @@
         adata.obsm[obsm] = pcs[:, :n_components]
         print(f"Changing adata.obsm['X_pca'] from shape {pcs.shape} to {adata.obsm[obsm].shape}")
     return n_components
 
 
 def pc_ks_test(pcs, p_cutoff=0.1, min_pc=4):
     i = 0
-    for i in range(pcs.shape[1] - 1):
+    for i in range(pcs.shape[1]):
+        if i == (pcs.shape[1] - 1):
+            break
         cur_pc = pcs[:, i]
         next_pc = pcs[:, i + 1]
         _, p = ks_2samp(cur_pc, next_pc)
         if p > p_cutoff:
             break
     n_components = min(i + 1, pcs.shape[1])
     min_pc = min(min_pc, pcs.shape[1])
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/chromatin_conformation.py` & `allcools-1.1.0/ALLCools/clustering/chromatin_conformation.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/dmg.py` & `allcools-1.1.0/ALLCools/clustering/dmg.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         if self.verbose:
             print(len(pairs), "pairwise DMGs")
         n_pairs = len(pairs)
 
         with ProcessPoolExecutor(min(n_pairs, self.n_jobs)) as exe:
             step = max(1, n_pairs // 10)
             futures = {}
-            for (cluster_l, cluster_r) in pairs:
+            for cluster_l, cluster_r in pairs:
                 f = exe.submit(
                     _single_pairwise_dmg,
                     cluster_l=cluster_l,
                     cluster_r=cluster_r,
                     top_n=self.top_n,
                     adj_p_cutoff=self.adj_p_cutoff,
                     delta_rate_cutoff=self.delta_rate_cutoff,
@@ -347,20 +347,16 @@
         {
             data_key: pd.DataFrame(adata.uns["rank_genes_groups"][data_key]).stack()
             for data_key in ["names", "pvals_adj"]
         }
     )
     dmg_result = dmg_result[dmg_result.index.get_level_values(1).astype(bool)].reset_index(drop=True)
     # add fold change
-    in_cells_mean = adata.X[
-        adata.obs["groups"].astype(bool),
-    ].mean(axis=0)
-    out_cells_mean = adata.X[
-        ~adata.obs["groups"].astype(bool),
-    ].mean(axis=0)
+    in_cells_mean = adata.X[adata.obs["groups"].astype(bool),].mean(axis=0)
+    out_cells_mean = adata.X[~adata.obs["groups"].astype(bool),].mean(axis=0)
     fc = pd.Series(in_cells_mean / out_cells_mean, index=adata.var_names)
     dmg_result["fc"] = dmg_result["names"].map(fc)
     # filter
     dmg_result = dmg_result[(dmg_result["pvals_adj"] < adj_p_cutoff) & (dmg_result["fc"] < fc_cutoff)].copy()
     dmg_result = dmg_result.set_index("names").drop_duplicates()
 
     # add AUROC and filter again
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/doublets/coverage_doublets.py` & `allcools-1.1.0/ALLCools/clustering/doublets/coverage_doublets.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Reference:
 Thibodeau, Asa, Alper Eroglu, Christopher S. McGinnis, Nathan Lawlor, Djamel Nehar-Belaid, Romy Kursawe,
 Radu Marches, et al. 2021. “AMULET: A Novel Read Count-Based Method for Effective Multiplet Detection from
 Single Nucleus ATAC-Seq Data.” Genome Biology 22 (1): 252.
 
 """
 
-
 import json
 import pathlib
 from collections import defaultdict
 from concurrent.futures import ProcessPoolExecutor, as_completed
 
 import numpy as np
 import pandas as pd
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/doublets/scrublet.py` & `allcools-1.1.0/ALLCools/clustering/doublets/scrublet.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/feature_selection/feature_enrichment.py` & `allcools-1.1.0/ALLCools/clustering/feature_selection/feature_enrichment.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/feature_selection/gene_panel_design.py` & `allcools-1.1.0/ALLCools/clustering/feature_selection/gene_panel_design.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/incremental_pca.py` & `allcools-1.1.0/ALLCools/clustering/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/lsi.py` & `allcools-1.1.0/ALLCools/clustering/lsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sklearn.utils.validation import check_is_fitted
 
 
 def tf_idf(data, scale_factor=100000, idf=None):
     sparse_input = issparse(data)
 
     if idf is None:
-        # add small value in case downsample creates empty feature
+        # add small value in case down sample creates empty feature
         _col_sum = data.sum(axis=0)
         if sparse_input:
             col_sum = _col_sum.A1.astype(np.float32) + 0.00001
         else:
             col_sum = _col_sum.ravel().astype(np.float32) + 0.00001
         idf = np.log(1 + data.shape[0] / col_sum).astype(np.float32)
     else:
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/mcad.py` & `allcools-1.1.0/ALLCools/clustering/mcad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 from pybedtools import BedTool
 
 
-def remove_black_list_region(adata, black_list_path, f=0.2):
+def remove_black_list_region(adata, black_list_path, region_axis=1, f=0.2):
     """
     Remove regions overlap (bedtools intersect -f {f}) with regions in the black_list_path.
 
     Parameters
     ----------
     adata
         AnnData object
     black_list_path
         Path to the black list bed file
+    region_axis
+        Axis of regions. 0 for adata.obs, 1 for adata.var
     f
         Fraction of overlap when calling bedtools intersect
     """
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        feature_bed_df = adata.var[["chrom", "start", "end"]]
+        if region_axis == 1:
+            feature_bed_df = adata.var[["chrom", "start", "end"]]
+        elif region_axis == 0:
+            feature_bed_df = adata.obs[["chrom", "start", "end"]]
+        else:
+            raise ValueError("region_axis should be 0 or 1.")
         feature_bed = BedTool.from_dataframe(feature_bed_df)
         black_list_bed = BedTool(black_list_path)
         black_feature = feature_bed.intersect(black_list_bed, f=f, wa=True)
         try:
             black_feature_index = black_feature.to_dataframe().set_index(["chrom", "start", "end"]).index
             black_feature_id = pd.Index(
                 feature_bed_df.reset_index()
                 .set_index(["chrom", "start", "end"])
                 .loc[black_feature_index][feature_bed_df.index.name]
             )
             print(
-                f"{black_feature_id.size} features removed due to overlapping"
+                f"{black_feature_id.size} regions removed due to overlapping"
                 f" (bedtools intersect -f {f}) with black list regions."
             )
-            adata._inplace_subset_var(~adata.var_names.isin(black_feature_id))
+            if region_axis == 1:
+                adata._inplace_subset_var(~adata.var_names.isin(black_feature_id))
+            else:
+                adata._inplace_subset_obs(~adata.obs_names.isin(black_feature_id))
         except pd.errors.EmptyDataError:
             # no overlap with black list
             pass
     return
 
 
 def remove_chromosomes(adata, exclude_chromosomes=None, include_chromosomes=None, chrom_col="chrom"):
```

### Comparing `ALLCools-1.0.8/ALLCools/clustering/pvclust.py` & `allcools-1.1.0/ALLCools/clustering/pvclust.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/clustering/rutilities.py` & `allcools-1.1.0/ALLCools/clustering/rutilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/base_ds.py` & `allcools-1.1.0/ALLCools/count_matrix/base_ds.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/dataset.py` & `allcools-1.1.0/ALLCools/count_matrix/dataset.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/h5ad.py` & `allcools-1.1.0/ALLCools/count_matrix/h5ad.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/mcad.py` & `allcools-1.1.0/ALLCools/count_matrix/mcad.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/mcds.py` & `allcools-1.1.0/ALLCools/count_matrix/mcds.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,19 +327,25 @@
     """
     if engine not in ["zarr", "netcdf"]:
         raise ValueError(f'engine need to be "zarr" or "netcdf", got {engine}')
     # TODO region bed should have unique id, check before generate mcds
     dtype = parse_dtype(dtype)
 
     if isinstance(allc_table, str):
-        allc_series = pd.read_csv(allc_table, header=None, index_col=0, squeeze=True, sep="\t")
-        if not isinstance(allc_series, pd.Series):
-            raise ValueError("allc_table malformed, should only have 2 columns, 1. file_uid, 2. file_path")
+        allc_series = pd.read_csv(allc_table, header=None, index_col=0, sep="\t")
+        if allc_series.shape[1] == 1:
+            allc_series[2] = ""
+        elif allc_series.shape[1] == 2:
+            pass
+        else:
+            raise ValueError(
+                "allc_table malformed, should have 2 or 3 columns, 1. file_uid, 2. file_path, 3. cmeta_path if ballc format"
+            )
     else:
-        allc_series = allc_table.dropna()
+        allc_series = allc_table[~allc_table[1].isna()]
     if allc_series.index.duplicated().sum() != 0:
         raise ValueError("allc_table file uid have duplicates (1st column)")
 
     rna_series = pd.Series([])
     if rna_table is not None:
         if isinstance(rna_table, str):
             rna_series = pd.read_csv(rna_table, header=None, index_col=0, squeeze=True, sep="\t")
@@ -359,36 +365,36 @@
                 "from the SAME cell/sample that have the SAME cell/sample id. "
                 "If you have to save RNA and mC in different cell/sample ids, "
                 "it would be better to save them in separate files."
             )
         else:
             if n_matched < rna_series.size:
                 print(f"{rna_series.size - n_matched} file_uid in RNA table do not exist in ALLC table")
-            if n_matched < allc_series.size:
+            if n_matched < allc_series.shape[0]:
                 print(f"{allc_series.size - n_matched} file_uid in ALLC table do not exist in RNA table")
 
         # reindex allc and rna series, this may create NaN, will be dropped
         union_index = rna_series.index | allc_series.index
         allc_series = allc_series.reindex(union_index)
         rna_series = rna_series.reindex(union_index)
 
     # if allc files exceed max_per_mcds, save them into chunks
-    if allc_series.size > max_per_mcds:
-        mcds_n_chunk = ceil(allc_series.size / max_per_mcds)
-        chunk_size = ceil(allc_series.size / mcds_n_chunk)
+    if allc_series.shape[0] > max_per_mcds:
+        mcds_n_chunk = ceil(allc_series.shape[0] / max_per_mcds)
+        chunk_size = ceil(allc_series.shape[0] / mcds_n_chunk)
         allc_series_chunks = [
-            allc_series[chunk_start : chunk_start + chunk_size]
-            for chunk_start in range(0, allc_series.size, chunk_size)
+            allc_series.iloc[chunk_start : chunk_start + chunk_size]
+            for chunk_start in range(0, allc_series.shape[0], chunk_size)
         ]
         if rna_table is not None:
             rna_series_chunks = [
                 rna_series[chunk_start : chunk_start + chunk_size]
                 for chunk_start in range(0, rna_series.size, chunk_size)
             ]
-        print(f"Number of file_uids {allc_series.size} > max_per_mcds {max_per_mcds}, ")
+        print(f"Number of file_uids {allc_series.shape[0]} > max_per_mcds {max_per_mcds}, ")
         print(f"will generate MCDS in {len(allc_series_chunks)} chunks.")
 
         # mcds chunks execute sequentially
         for chunk_id, allc_series_chunk in enumerate(allc_series_chunks):
             if rna_table is not None:
                 rna_series_chunk = rna_series_chunks[chunk_id]
             else:
```

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/snap.py` & `allcools-1.1.0/ALLCools/count_matrix/snap.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/count_matrix/zarr.py` & `allcools-1.1.0/ALLCools/count_matrix/zarr.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/dataset/directory_structure.py` & `allcools-1.1.0/ALLCools/dataset/directory_structure.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/dmr/call_dmr.py` & `allcools-1.1.0/ALLCools/dmr/call_dmr.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/dmr/call_dmr_baseds.py` & `allcools-1.1.0/ALLCools/dmr/call_dmr_baseds.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         count_da="data",
         quantile=0.1,
         min_delta=0.2,
         frac_delta_cutoff=0.2,
         frac_delta_quantile=0.05,
         max_dist=250,
         corr_cutoff=0.3,
+        drop_additional_samples=False,
     ):
         self.base_ds = base_ds
         self.cell_groups = cell_groups
         self.dms_ds = dms_ds
         self.chrom = chrom
         self.start = start
         self.end = end
@@ -49,20 +50,26 @@
 
         self.quantile = quantile
         self.min_delta = min_delta
         self.frac_delta_cutoff = frac_delta_cutoff
         self.frac_delta_quantile = frac_delta_quantile
         self.max_dist = max_dist
         self.corr_cutoff = corr_cutoff
-
+        self.drop_additional_samples = drop_additional_samples
         self._all_cpgs = None
         return
 
     def _get_all_cpg(self):
+        if self.drop_additional_samples:
+            use_samples = pd.Series(self.cell_groups).index
+            sample_index = self.base_ds.get_index(self.sample_dim)
+            self.base_ds = self.base_ds.sel({self.sample_dim: sample_index.isin(use_samples)})
+
         all_cpgs = self.base_ds.fetch(self.chrom, self.start, self.end).select_mc_type(self.mcg_pattern)
+
         all_cpgs.coords["group"] = all_cpgs[self.sample_dim].to_pandas().map(self.cell_groups)
         all_cpgs["group_data"] = (
             all_cpgs[self.count_da].groupby("group").sum(dim=self.sample_dim).load(scheduler="sync")
         )
 
         self._all_cpgs = all_cpgs
         return
```

### Comparing `ALLCools-1.0.8/ALLCools/dmr/call_dms.py` & `allcools-1.1.0/ALLCools/dmr/call_dms.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/dmr/call_dms_baseds.py` & `allcools-1.1.0/ALLCools/dmr/call_dms_baseds.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,22 @@
     # noinspection PyUnresolvedReferences
     pos_ds = cg_ds.sel(pos=(~neg_pos).values)
     neg_ds = cg_ds.sel(pos=neg_pos.values)
 
     # modify the pos by -1 so the neg_ds and pos_ds has the same pos,
     # and can be sum together
     neg_ds["pos"] = neg_ds["pos"].to_pandas() - 1
-    cg_ds = pos_ds + neg_ds
+
+    # sum the pos and neg
+    # union the pos and neg index, otherwise if there is only one strand occur in the base_ds,
+    # the other strand will be dropped by sum (xarray take the intersection of index)
+    pos_index = pos_ds.get_index("pos")
+    neg_index = neg_ds.get_index("pos")
+    all_positions = pos_index.union(neg_index)
+    cg_ds = pos_ds.reindex(pos=all_positions, fill_value=0) + neg_ds.reindex(pos=all_positions, fill_value=0)
     return cg_ds
 
 
 def _core_dms_function(count_table, max_row_count, max_total_count, n_permute, min_pvalue, estimate_p=False):
     """Calculate dms p-value and residual for a single CpG count table."""
     count_table = downsample_table(count_table, max_row_count=max_row_count, max_total_count=max_total_count)
     if count_table.sum() == 0:
@@ -45,14 +52,31 @@
 
     residual = calculate_residual(count_table)
     # mc_residual = -c_residual, so only save one column
     residual = residual[:, 1]
     return p_value, residual
 
 
+def add_groups_to_base_ds(base_ds, groups):
+    """Add groups to base_ds.coords"""
+    if isinstance(groups, (str, pathlib.Path)):
+        groups = pd.read_csv(groups, header=None, index_col=0, names=["sample_id", "group"]).squeeze()
+
+    # select samples
+    ds_sample_id = base_ds.get_index("sample_id")
+    use_sample = ds_sample_id.isin(groups.index)
+    if use_sample.sum() != use_sample.size:
+        # noinspection PyUnresolvedReferences
+        base_ds = base_ds.sel(sample_id=use_sample)
+
+    # add group info
+    base_ds.coords["group"] = groups
+    return base_ds
+
+
 def call_dms_worker(
     groups,
     base_ds,
     mcg_pattern,
     n_permute,
     alpha,
     estimate_p,
@@ -67,33 +91,24 @@
 ):
     """
     Worker function for call_dms_from_base_ds.
 
     See call_dms_from_base_ds for parameter description.
     """
     if groups is not None:
-        if isinstance(groups, (str, pathlib.Path)):
-            groups = pd.read_csv(groups, header=None, index_col=0, names=["sample_id", "group"]).squeeze()
-
-        # select samples
-        ds_sample_id = base_ds.get_index("sample_id")
-        use_sample = ds_sample_id.isin(groups.index)
-        if use_sample.sum() != use_sample.size:
-            # noinspection PyUnresolvedReferences
-            base_ds = base_ds.sel(sample_id=use_sample.values)
-
-        # add group info
-        base_ds.coords["group"] = groups
+        base_ds = add_groups_to_base_ds(base_ds, groups)
 
     # select CpG sites
-    cg_base_ds = base_ds.select_mc_type(mcg_pattern)
-
-    if merge_strand:
-        # merge pos and neg strand
-        cg_base_ds = _merge_pos_neg_cpg(cg_base_ds)
+    if mcg_pattern is not None:
+        cg_base_ds = base_ds.select_mc_type(mcg_pattern)
+        if merge_strand:
+            # merge pos and neg strand
+            cg_base_ds = _merge_pos_neg_cpg(cg_base_ds)
+    else:
+        cg_base_ds = base_ds
 
     if groups is not None:
         # group by group and sum base counts
         group_cg_base_ds = cg_base_ds[["data"]].groupby("group").sum(dim="sample_id").load()
     else:
         # if no group, load all data and call DMR across samples, the sample_id is renamed to group
         group_cg_base_ds = cg_base_ds[["data"]].rename({"sample_id": "group"}).load()
@@ -143,28 +158,36 @@
     p_values = pd.Series(p_values).astype("float32")
     p_values.index.name = "pos"
     p_values = p_values.reindex(pos_index)
     assert p_values.isna().sum() == 0, "Some positions are missing p-values."
 
     dms_ds.coords["p-values"] = p_values
 
-    if estimate_p:
-        # FDR correction, only valid for estimate_p
-        from statsmodels.stats.multitest import multipletests
+    n_dms = dms_ds.get_index("pos").size
 
-        _, q, *_ = multipletests(p_values)
-        q = pd.Series(q, index=p_values.index, name="q-values").astype("float32")
-        dms_ds.coords["q-values"] = q
-
-    # filter by p-value
-    if filter_sig:
-        if "q-values" in dms_ds.coords:
-            dms_ds = dms_ds.sel(pos=dms_ds.coords["q-values"] <= alpha)
-        else:
-            dms_ds = dms_ds.sel(pos=dms_ds["p-values"] <= alpha)
+    if n_dms > 0:
+        if estimate_p:
+            # FDR correction, only valid for estimate_p
+            from statsmodels.stats.multitest import multipletests
+
+            _, q, *_ = multipletests(p_values, method="fdr_bh")
+            q = pd.Series(q, index=p_values.index, name="q-values").astype("float32")
+            dms_ds.coords["q-values"] = q
+
+        # filter by p-value
+        if filter_sig:
+            if "q-values" in dms_ds.coords:
+                dms_ds = dms_ds.sel(pos=dms_ds.coords["q-values"] <= alpha)
+            else:
+                dms_ds = dms_ds.sel(pos=dms_ds["p-values"] <= alpha)
+    else:
+        if estimate_p:
+            empty_q = pd.Series([])
+            empty_q.index.name = "pos"
+            dms_ds.coords["q-values"] = empty_q
 
     if output_path is not None:
         dms_ds.to_zarr(output_path, **output_kwargs)
         return None
     else:
         return dms_ds
```

### Comparing `ALLCools-1.0.8/ALLCools/dmr/parse_methylpy.py` & `allcools-1.1.0/ALLCools/dmr/parse_methylpy.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/dmr/rms_test.py` & `allcools-1.1.0/ALLCools/dmr/rms_test.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/gtf/Gtf.py` & `allcools-1.1.0/ALLCools/gtf/Gtf.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/gtf/utilities.py` & `allcools-1.1.0/ALLCools/gtf/utilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/integration/cca.py` & `allcools-1.1.0/ALLCools/integration/cca.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     Returns
     -------
     features_idx : np.array
     """
     # data.shape = (n_cc, total_features)
     n_cc = data.shape[0]
     n_features_per_dim = n_features * 10 // n_cc
+    n_features_per_dim = min(n_features_per_dim, data.shape[1] - 1)
+
     sample_range = np.arange(n_cc)[:, None]
 
     # get idx of n_features_per_dim features with the highest absolute loadings
     data = np.abs(data)
     idx = np.argpartition(-data, n_features_per_dim, axis=1)[:, :n_features_per_dim]
     # idx.shape = (n_cc, n_features_per_dim)
 
@@ -66,15 +68,16 @@
         scale2=scale2,
         max_cc_cell=max_cc_cell,
         random_state=random_state,
     )
 
     # CCA decomposition
     model = TruncatedSVD(n_components=n_components, algorithm=svd_algorithm, random_state=random_state)
-    U = model.fit_transform(tf_data1.dot(tf_data2.T))
+    tf_data2_t = tf_data2.T.copy()
+    U = model.fit_transform(tf_data1.dot(tf_data2_t))
 
     # select dimensions with non-zero singular values
     sel_dim = model.singular_values_ != 0
     print("non zero dims", sel_dim.sum())
 
     V = model.components_[sel_dim].T
     U = U[:, sel_dim] / model.singular_values_[sel_dim]
@@ -198,15 +201,15 @@
     chunk_size=50000,
     svd_algorithm="randomized",
     min_cov_filter=5,
     random_state=0,
 ):
     np.random.seed(random_state)
 
-    # downsample data1 and data2 to run tf_idf and CCA
+    # down sample data1 and data2 to run tf_idf and CCA
     if max_cc_cell < data1.shape[0]:
         sel1 = np.sort(np.random.choice(np.arange(data1.shape[0]), max_cc_cell, False))
         tf_data1 = data1[sel1, :]
     else:
         tf_data1 = data1
     if max_cc_cell < data2.shape[0]:
         sel2 = np.sort(np.random.choice(np.arange(data2.shape[0]), max_cc_cell, False))
@@ -225,22 +228,24 @@
 
     # CCA part
     model = TruncatedSVD(n_components=n_components, algorithm=svd_algorithm, random_state=0)
     tf = tf1.dot(tf2.T)
     U = model.fit_transform(tf)
 
     # select non-zero singular values
-    # transform the whole dataset
+    # transform the whole dataset 2 to get V
     sel_dim = model.singular_values_ != 0
     nnz_singular_values = model.singular_values_[sel_dim]
     nnz_components = model.components_[sel_dim]
     if max_cc_cell > data2.shape[0]:
         V = nnz_components.T
     else:
         # use the safe_sparse_dot to avoid memory error
+        # safe_sparse_dot take both sparse and dense matrix,
+        # for dense matrix, it just uses normal numpy dot product
         V = np.concatenate(
             [
                 safe_sparse_dot(
                     safe_sparse_dot(U.T[sel_dim], tf1),
                     tf_idf(
                         data2[chunk_start : (chunk_start + chunk_size)][:, bin_filter],
                         scale_factor=scale_factor,
@@ -250,14 +255,16 @@
                     ].T,  # [0] is the tf
                 ).T
                 for chunk_start in np.arange(0, data2.shape[0], chunk_size)
             ],
             axis=0,
         )
         V = V / np.square(nnz_singular_values)
+
+    # transform the whole dataset 1 to get U
     if max_cc_cell > data1.shape[0]:
         U = U[:, sel_dim] / nnz_singular_values
     else:
         U = np.concatenate(
             [
                 safe_sparse_dot(
                     tf_idf(
@@ -319,15 +326,15 @@
         return np.concatenate(tf_reduce, axis=0) / self.model.singular_values_
 
 
 class SVD:
     def __init__(
         self,
         n_components=100,
-        algorithm="arpack",
+        algorithm="randomized",
         random_state=0,
     ):
         self.model = TruncatedSVD(n_components=n_components, algorithm=algorithm, random_state=random_state)
 
     def fit(self, data):
         self.model.fit(data)
         return self
```

### Comparing `ALLCools-1.0.8/ALLCools/integration/confusion.py` & `allcools-1.1.0/ALLCools/integration/confusion.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 import igraph as ig
 import leidenalg as la
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 
+def sdi(data):
+    """
+    Calculate the Shannon Diversity Index (SDI) for a categorical data series.
+
+    Higher SDI indicates higher diversity.
+    """
+    if len(data) == 0:
+        return 0
+    counts = pd.Series(data).value_counts()
+    ratio = counts / counts.sum()
+    score = -(np.log(ratio) * ratio).sum()
+    return score
+
+
 def calculate_direct_confusion(*args, **kwargs):
     warn("This function is deprecated. Call calculate_overlap_score instead", DeprecationWarning)
     return calculate_overlap_score(*args, **kwargs)
 
 
 def _get_overlap_score(left_values, right_values):
     score = np.min([left_values, right_values], axis=0).sum()
@@ -93,32 +107,48 @@
     diag_sum = np.diag(group_overlap_score_mean, 0).sum()
     non_diag_sum = group_overlap_score_mean.values.sum() - diag_sum
 
     ratio = diag_sum / non_diag_sum
     return ratio
 
 
-def confusion_matrix_clustering(confusion_matrix, min_value=0, max_value=0.9, seed=0):
+def confusion_matrix_clustering(
+    confusion_matrix, min_value=0.1, max_value=0.9, partition_type=None, resolution=1, seed=0
+):
     """
     Given a confusion matrix, bi-clustering the matrix using Leiden Algorithm.
 
     Parameters
     ----------
     confusion_matrix :
         A confusion matrix. Row is query, column is reference.
     min_value :
         minimum value to be used as an edge weight.
     max_value :
         maximum value to be used as an edge weight. Larger value will be capped to this value.
+    partition_type :
+        The type of partition to be used. See leidenalg documentation for details.
+        If None, use the :class:`~leidenalg.RBConfigurationVertexPartition` partition type.
+    resolution :
+        The resolution parameter to be used. See leidenalg documentation for details.
     seed :
         random seed for Leiden Algorithm.
 
     Returns
     -------
-    query_group, ref_group, ordered confusion_matrix
+    query_group:
+        A series of query cluster integration group.
+    reference_group:
+        A series of reference cluster integration group.
+    confusion_matrix：
+        A confusion matrix ordered by the integration group.
+    g:
+        The Graph object used for leiden clustering and determine integration groups.
+    modularity_score:
+        The modularity score of the graph partition by integration groups.
     """
     # make sure confusion matrix index and columns are unique
     try:
         assert confusion_matrix.index.duplicated().sum() == 0
         assert confusion_matrix.columns.duplicated().sum() == 0
     except AssertionError:
         raise ValueError("Confusion matrix index and columns should be unique")
@@ -138,16 +168,20 @@
     g = nx.Graph()
     for _, (ref, query, weight) in edges.iterrows():
         weight = min(max_value, weight)
         g.add_edge(ref, query, weight=weight)
         # convert to igraph to run leiden
     h = ig.Graph.from_networkx(g)
 
+    if partition_type is None:
+        partition_type = la.RBConfigurationVertexPartition
+
     # leiden clustering
-    partition = la.find_partition(h, la.ModularityVertexPartition, weights="weight", seed=seed)
+    partition = la.find_partition(h, partition_type, weights="weight", seed=seed, resolution_parameter=resolution)
+
     # store output into adata.obs
     groups = np.array(partition.membership)
     idx_to_group = {int(node): g for node, g in zip(g.nodes, groups)}
 
     # map cluster back to original labels
     # -1 means a ref or query cluster is not co-clustered with the other dataset,
     # so the OS is very small and not included in the graph
@@ -155,10 +189,17 @@
     ref_group = pd.Series(ref_idx_map).map(idx_to_group).fillna(-1).astype(int)
 
     # also make an ordered confusion matrix
     confusion_matrix.index = confusion_matrix.index.map({v: k for k, v in query_idx_map.items()})
     confusion_matrix.columns = confusion_matrix.columns.map({v: k for k, v in ref_idx_map.items()})
     confusion_matrix = confusion_matrix.loc[query_group.sort_values().index, ref_group.sort_values().index].copy()
 
-    diag_score = calculate_diagonal_score(confusion_matrix, col_group=ref_group, row_group=query_group)
+    # calculate the graph modularity after partition
+    from collections import defaultdict
+
+    from networkx.algorithms.community import modularity
 
-    return query_group, ref_group, confusion_matrix, diag_score
+    group_nodes = defaultdict(set)
+    for group, node in zip(groups, g.nodes):
+        group_nodes[group].add(node)
+    modularity_score = modularity(g, group_nodes.values())
+    return query_group, ref_group, confusion_matrix, g, modularity_score
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ALLCools-1.0.8/ALLCools/integration/metric.py` & `allcools-1.1.0/ALLCools/integration/metric.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/integration/seurat_class.py` & `allcools-1.1.0/ALLCools/integration/seurat_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,51 +14,14 @@
 from sklearn.preprocessing import OneHotEncoder, normalize
 
 from .cca import cca, lsi_cca
 
 CPU_COUNT = multiprocessing.cpu_count()
 
 
-def top_features_idx(data, n_features):
-    """
-    Select top features with the highest importance in CCs.
-
-    Parameters
-    ----------
-    data
-        data.shape = (n_cc, total_features)
-    n_features
-        number of features to select
-
-    Returns
-    -------
-    features_idx : np.array
-    """
-    # data.shape = (n_cc, total_features)
-    n_cc = data.shape[0]
-    n_features_per_dim = n_features * 10 // n_cc
-    sample_range = np.arange(n_cc)[:, None]
-
-    # get idx of n_features_per_dim features with the highest absolute loadings
-    data = np.abs(data)
-    idx = np.argpartition(-data, n_features_per_dim, axis=1)[:, :n_features_per_dim]
-    # idx.shape = (n_cc, n_features_per_dim)
-
-    # make sure the order of first n_features_per_dim is ordered by loadings
-    idx = idx[sample_range, np.argsort(-data[sample_range, idx], axis=1)]
-
-    for i in range(n_features // n_cc + 1, n_features_per_dim):
-        features_idx = np.unique(idx[:, :i].flatten())
-        if len(features_idx) > n_features:
-            return features_idx
-    else:
-        features_idx = np.unique(idx[:, :n_features_per_dim].flatten())
-        return features_idx
-
-
 def find_neighbor(cc1, cc2, k, random_state=0, n_jobs=-1):
     """
     Find all four way of neighbors for two datasets.
 
     Parameters
     ----------
     cc1
@@ -342,14 +305,17 @@
         chunk_size,
         random_state,
         signorm,
     ):
         """Pairwise anchor between two datasets."""
         adata1 = self.adata_dict[i]
         adata2 = self.adata_dict[j]
+
+        min_sample = min(adata1.shape[0], adata2.shape[0])
+
         if i_sel is not None:
             adata1 = adata1[i_sel, :]
         if j_sel is not None:
             adata2 = adata2[j_sel, :]
 
         if dim_red in ("cca", "pca", "lsi", "lsi-cca"):
             # 1. prepare input matrix for CCA
@@ -389,16 +355,17 @@
                 raise ValueError(f"Dimension reduction method {dim_red} is not supported.")
 
             # 3. normalize CCV per sample/row
             U = normalize(U, axis=1)
             V = normalize(V, axis=1)
 
             # 4. find MNN of U and V to find anchors
-            print("Find Anchors")
-            _k = max(i for i in [k_anchor, k_local, k_score, 50] if i is not None)
+            _k = max(_temp for _temp in [k_anchor, k_local, k_score] if _temp is not None)
+            _k = min(min_sample - 2, _k)
+            print(f"Find Anchors using k={_k}")
             G11, G12, G21, G22, raw_anchors = self._calculate_mutual_knn_and_raw_anchors(
                 i=i, j=j, U=U, V=V, k=_k, k_anchor=k_anchor
             )
 
             # 5. filter anchors by high dimensional neighbors
             if k_filter is not None and high_dim_feature is not None:
                 # compute ccv feature loading
@@ -498,16 +465,16 @@
         adata_list,
         adata_names=None,
         k_local=None,
         key_local="X_pca",
         key_anchor="X",
         dim_red="pca",
         svd_algorithm="randomized",
-        scale1=False,
-        scale2=False,
+        scale1=True,
+        scale2=True,
         scale_list=None,
         k_filter=None,
         n_features=200,
         n_components=None,
         max_cc_cells=50000,
         chunk_size=50000,
         k_anchor=5,
@@ -636,15 +603,15 @@
 
                 # save anchors
                 self.anchor[(i, j)] = anchor_df.copy()
                 print(f"Identified {len(self.anchor[i, j])} anchors between datasets {i} and {j}.")
         return
 
     def find_nearest_anchor(
-        self, data, data_qry, ref, qry, key_correct="X_pca", npc=30, kweight=100, sd=1, random_state=0
+        self, data, data_qry, ref, qry, key_correct="X_pca", npc=30, k_weight=100, sd=1, random_state=0
     ):
         """Find the nearest anchors for each cell in data."""
         print("Initialize")
         cum_ref, cum_qry = [0], [0]
         for xx in ref:
             cum_ref.append(cum_ref[-1] + data[xx].shape[0])
         for xx in qry:
@@ -665,26 +632,29 @@
         score = anchor["score"].values
         anchor = anchor[["x1", "x2"]].values
 
         if key_correct == "X":
             model = PCA(n_components=npc, svd_solver="arpack", random_state=random_state)
             reduce_qry = model.fit_transform(data_qry)
         else:
-            reduce_qry = data_qry
+            reduce_qry = data_qry[:, :npc]
 
-        print("Find nearest anchors")
+        print("Find nearest anchors", end=". ")
         index = pynndescent.NNDescent(
             reduce_qry[anchor[:, 1]],
             metric="euclidean",
-            n_neighbors=kweight,
+            n_neighbors=k_weight,
             random_state=random_state,
             parallel_batch_queries=True,
             n_jobs=self.n_jobs,
         )
-        G, D = index.query(reduce_qry, k=kweight)
+        k_weight = min(k_weight, anchor.shape[0] - 5)
+        k_weight = max(5, k_weight)
+        print("k_weight: ", k_weight, end="\n")
+        G, D = index.query(reduce_qry, k=k_weight)
 
         print("Normalize graph")
         cell_filter = D[:, -1] == 0
         D = (1 - D / D[:, -1][:, None]) * score[G]
         D[cell_filter] = score[G[cell_filter]]
         D = 1 - np.exp(-D * (sd**2) / 4)
         D = D / (np.sum(D, axis=1) + 1e-6)[:, None]
@@ -710,15 +680,15 @@
         anchor, G, D, cum_qry = self.find_nearest_anchor(
             data=data,
             data_qry=data_qry,
             key_correct=key_correct,
             ref=ref,
             qry=qry,
             npc=npc,
-            kweight=k_weight,
+            k_weight=k_weight,
             sd=sd,
             random_state=random_state,
         )
 
         print("Transform data")
         bias = data_ref[anchor[:, 0]] - data_qry[anchor[:, 1]]
         data_prj = np.zeros(data_qry.shape)
@@ -758,15 +728,15 @@
         else:
             # correct dimensionality reduced matrix only
             corrected = [normalize(adata_list[i].obsm[key_correct], axis=1) for i in range(self.n_dataset)]
 
         for xx in self.alignments:
             print(xx)
             corrected = self.transform(
-                data=np.array(corrected),
+                data=np.array(corrected, dtype="object"),
                 ref=xx[0],
                 qry=xx[1],
                 npc=n_components,
                 k_weight=k_weight,
                 sd=sd,
                 random_state=self.random_state,
                 row_normalize=row_normalize,
@@ -777,15 +747,15 @@
     def label_transfer(
         self,
         ref,
         qry,
         categorical_key=None,
         continuous_key=None,
         key_dist="X_pca",
-        kweight=100,
+        k_weight=100,
         npc=30,
         sd=1,
         chunk_size=50000,
         random_state=0,
     ):
         """Transfer labels from query to reference space."""
         adata_list = list(self.adata_dict.values())
@@ -795,15 +765,15 @@
 
         anchor, G, D, cum_qry = self.find_nearest_anchor(
             data=adata_list,
             data_qry=data_qry,
             ref=ref,
             qry=qry,
             npc=npc,
-            kweight=kweight,
+            k_weight=k_weight,
             key_correct=key_dist,
             sd=sd,
             random_state=random_state,
         )
         print("Label transfer")
         label_ref = []
         columns = []
```

### Comparing `ALLCools-1.0.8/ALLCools/jbrowse/__init__.py` & `allcools-1.1.0/ALLCools/jbrowse/__init__.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/mcds/base_ds.py` & `allcools-1.1.0/ALLCools/mcds/base_ds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 import subprocess
 
 import numpy as np
 import pandas as pd
+import pyBigWig
 import xarray as xr
 from numba import njit
 
 from ALLCools.utilities import parse_mc_pattern
 
 
 def _mvalue(mc, cov, alpha=0.1):
@@ -128,15 +129,16 @@
         self.attrs["continuous"] = value
         if not value:
             # remove offset when continuous is False
             self.attrs.pop("offset", None)
 
     @property
     def offset(self):
-        return self.attrs.get("offset", 0)
+        value = self.attrs.get("offset", 0)
+        return int(value)
 
     @offset.setter
     def offset(self, value):
         assert isinstance(value, int), "offset must be an integer."
         self.attrs["offset"] = value
 
     def fetch(self, start=None, end=None):
@@ -152,33 +154,29 @@
         end :
             The end position of region.
 
         Returns
         -------
         BaseDSChrom
         """
-        if start is not None or end is not None:
-            if start is None:
-                start = 0
-            if end is None:
-                end = self.chrom_size
-
-            assert start < end, "start must be less than end."
-
-            if self.continuous:
-                obj = self.sel(pos=slice(start - self.offset, end - self.offset))
-                # copy attrs to avoid changing the original attrs of self
-                obj.attrs = obj.attrs.copy()
-                obj.attrs["offset"] = start
-            else:
-                obj = self.fetch_regions([(start, end)])
-                # attrs will be copied in fetch_regions
-        else:
-            raise ValueError("start and end cannot be both None.")
+        if start is None:
+            start = 0
+        if end is None:
+            end = self.chrom_size
 
+        assert start < end, "start must be less than end."
+
+        if self.continuous:
+            obj = self.sel(pos=slice(start - self.offset, end - self.offset))
+            # copy attrs to avoid changing the original attrs of self
+            obj.attrs = obj.attrs.copy()
+            obj.attrs["offset"] = start
+        else:
+            obj = self.fetch_regions([(start, end)])
+            # attrs will be copied in fetch_regions
         return obj
 
     def fetch_regions(self, regions):
         """
         Select by multiple regions.
 
         Parameters
@@ -201,19 +199,22 @@
 
         assert obj.continuous is False
         assert obj.offset == 0
         return obj
 
     def _fetch_positions(self, positions):
         """Fetch positions only, no prefetch."""
-        positions = np.sort(positions).astype("uint32")
+        if positions.size == 0:
+            obj = self.isel(pos=[])
+        else:
+            positions = np.sort(positions).astype("uint32")
 
-        # always apply offset to positions
-        # if continuous is False, offset will be 0, so no effect
-        obj = self.sel(pos=positions - self.offset)
+            # always apply offset to positions
+            # if continuous is False, offset will be 0, so no effect
+            obj = self.sel(pos=positions - self.offset)
 
         # copy attrs to avoid changing the original attrs of self
         obj.attrs = obj.attrs.copy()
         obj.continuous = False
         obj.coords["pos"] = positions
         return obj
 
@@ -228,15 +229,15 @@
         positions :
             using genome position to select the positions
 
         Returns
         -------
         BaseDSChrom
         """
-        if self.continuous:
+        if self.continuous and len(positions) != 0:
             # if obj is continuous, pre-fetch the min max pos to speed up
             pos_min = min(positions)
             pos_max = max(positions) + 1
             obj = self.fetch(pos_min, pos_max)
             return obj._fetch_positions(positions)
         else:
             return self._fetch_positions(positions)
@@ -438,25 +439,35 @@
             all_idx = self.get_index("pos")
             region_start = all_idx.min() + self.offset if region_start is None else region_start
             region_end = all_idx.max() + self.offset if region_end is None else region_end
 
         if regions is not None:
             if regions.shape[1] == 3:
                 _chrom_sel = regions.iloc[:, 0] == self.chrom
-                regions = regions.iloc[_chrom_sel, 1:].copy()
+                regions = regions.loc[_chrom_sel,].iloc[:, 1:].copy()
             assert regions.shape[1] == 2
             assert regions.shape[0] > 0, "regions must have at least one row."
 
         # get positions
-        pos_idx = self.cb.get_mc_pos(mc_type, offset=self.offset)
-        if regions is not None:
-            region_pos_idx = _regions_to_pos(regions=regions)
-            pos_idx = pos_idx.intersection(region_pos_idx)
-
-        base_ds = self.fetch_positions(positions=pos_idx)
+        if mc_type is not None:
+            pos_idx = self.cb.get_mc_pos(mc_type, offset=self.offset)
+            if regions is not None:
+                region_pos_idx = _regions_to_pos(regions=np.array(regions))
+                pos_idx = pos_idx.intersection(region_pos_idx).astype(int)
+            base_ds = self.fetch_positions(positions=pos_idx)
+        else:
+            # use all positions in the BaseDS (mc_type selection may have been done)
+            base_ds = self
+            pos_idx = base_ds.get_index("pos")
+            if regions is not None:
+                region_pos_idx = _regions_to_pos(regions=np.array(regions))
+                pos_idx = pos_idx.intersection(region_pos_idx).astype(int)
+                base_ds = self.fetch_positions(positions=pos_idx)
+                # update pos_idx
+                pos_idx = base_ds.get_index("pos")
 
         # prepare regions
         if regions is not None:
             bins = regions.iloc[:, 0].tolist() + [regions.iloc[-1, 1]]
             labels = regions.index
             region_name = regions.index.name
         else:
@@ -470,36 +481,38 @@
             if bins[0] > region_start:
                 bins.insert(0, region_start)
 
             labels = []
             for start in bins[:-1]:
                 labels.append(start)
 
-        # border case, no CpG selected
-        if pos_idx.size == 0:
+        if mc_type is not None and len(pos_idx) == 0:
+            # border case, no CpX selected by mc_type
             # create an empty region_ds
             region_ds = base_ds["data"].rename({"pos": "pos_bins"})
             region_ds = region_ds.reindex({"pos_bins": labels}, fill_value=0)
         else:
             region_ds = (
                 base_ds["data"]
                 .groupby_bins(
                     group="pos",
                     bins=bins,
-                    right=True,
+                    # important, include the start position but exclude the end position;
+                    # the same as BED format
+                    right=False,
                     labels=labels,
                     precision=3,
                     include_lowest=True,
                     squeeze=True,
                     restore_coord_dims=False,
                 )
                 .sum(dim="pos")
-                .chunk({"pos_bins": region_chunks})
             )
-
+        if region_chunks is not None:
+            region_ds = region_ds.chunk({"pos_bins": region_chunks})
         if region_name is not None:
             region_ds = region_ds.rename({"pos_bins": region_name})
 
         region_ds = xr.Dataset({"data": region_ds}).fillna(0)
         return region_ds
 
     def call_dms(
@@ -529,14 +542,15 @@
             Samples not occur in the group information will be ignored.
         output_path :
             Path to the output DMS dataset.
             If provided, the result will be saved to disk.
             If not, the result will be returned.
         mcg_pattern :
             Pattern of the methylated cytosine, default is "CGN".
+            If None, use all positions in the BaseDS.
         n_permute :
             Number of permutation to perform.
         alpha :
             Minimum p-value/q-value to consider a site as significant.
         max_row_count :
             Maximum number of base counts for each row (sample) in the DMS input count table.
         max_total_count :
@@ -577,28 +591,29 @@
             filter_sig=filter_sig,
             merge_strand=merge_strand,
             output_path=output_path,
             **output_kwargs,
         )
         return dms_ds
 
-    def dump_sample_bigwig(self, bigwig_path, da_name, sample_dim, sample, value="frac"):
-        import pyBigWig
-
+    def get_sample_mc_values(self, da_name, sample_dim, sample, value):
         da = self[da_name]
-
-        pos = da.get_index("pos")
         mc = da.sel({sample_dim: sample, "count_type": "mc"})
         cov = da.sel({sample_dim: sample, "count_type": "cov"})
         if value == "frac":
             values = _frac(mc=mc, cov=cov).values
         elif value == "mvalue":
             values = _mvalue(mc=mc, cov=cov).values
         else:
             raise ValueError(f"Unknown value: {value}")
+        return values
+
+    def dump_sample_bigwig(self, bigwig_path, da_name, sample_dim, sample, value="frac"):
+        pos = self.get_index("pos")
+        values = self.get_sample_mc_values(da_name=da_name, sample_dim=sample_dim, sample=sample, value=value)
 
         # save to bigwig
         bigwig_path = pathlib.Path(bigwig_path).absolute().resolve()
         # noinspection PyArgumentList
         with pyBigWig.open(str(bigwig_path), "w") as bw:
             bw.addHeader([(self.chrom, self.chrom_size)])
             bw.addEntries(self.chrom, pos.values, values=values, span=1)
@@ -693,27 +708,31 @@
                 merge_cpg_strand=merge_cpg_strand,
             )
             jb.add_track(track_path="/tmp/BaseDS.Positions.bed.gz", name="BaseDS Positions", load="move")
         return jb
 
 
 class BaseDS:
-    def __init__(self, paths, codebook_path=None):
+    def __init__(self, paths, chrom_sizes_path, codebook_path=None):
         """
         A wrapper for one or multiple BaseDS datasets.
 
         Parameters
         ----------
         paths :
             Path to the BaseDS datasets.
+        chrom_sizes_path :
+            Path to the chromosome sizes file.
         codebook_path :
             Path to the codebook file.
         """
         self.paths = self._parse_paths(paths)
         self.codebook_path = codebook_path
+        self.chrom_sizes_path = chrom_sizes_path
+        self.chrom_sizes = pd.read_csv(chrom_sizes_path, sep="\t", header=None, index_col=0).squeeze()
         self.__base_ds_cache = {}
 
     @staticmethod
     def _parse_paths(paths):
         import glob
 
         _paths = []
```

### Comparing `ALLCools-1.0.8/ALLCools/mcds/correlation.py` & `allcools-1.1.0/ALLCools/mcds/correlation.py`

 * *Files 26% similar despite different names*

```diff
@@ -56,14 +56,101 @@
             # if any variable std == 0
             out[idx] = np.nan
         else:
             out[idx] = (a[i] - mu_a[i]) @ (b[j] - mu_b[j]) / k / _sig_a / _sig_b
     return out
 
 
+@njit
+def _corr_all(a, b):
+    """Correlation between all rows in a and b, no nan value"""
+    n, k = a.shape
+    m, k = b.shape
+
+    mu_a = _mean(a)
+    mu_b = _mean(b)
+    sig_a = _std(a)
+    sig_b = _std(b)
+
+    out = np.empty((n, m))
+
+    for i in range(n):
+        for j in range(m):
+            _sig_a = sig_a[i]
+            _sig_b = sig_b[j]
+            if _sig_a == 0 or _sig_b == 0:
+                # if any variable std == 0
+                out[i, j] = np.nan
+            else:
+                out[i, j] = (a[i] - mu_a[i]) @ (b[j] - mu_b[j]) / k / _sig_a / _sig_b
+    return out
+
+
+@njit
+def _corr_row(a, b):
+    """Correlation between each row in a and b, no nan value"""
+    n, k = a.shape
+    m, k = b.shape
+
+    mu_a = _mean(a)
+    mu_b = _mean(b)
+    sig_a = _std(a)
+    sig_b = _std(b)
+
+    out = np.empty((n,))
+
+    for i in range(n):
+        _sig_a = sig_a[i]
+        _sig_b = sig_b[i]
+        if _sig_a == 0 or _sig_b == 0:
+            # if any variable std == 0
+            out[i] = np.nan
+        else:
+            out[i] = (a[i] - mu_a[i]) @ (b[i] - mu_b[i]) / k / _sig_a / _sig_b
+    return out
+
+
+def corr_array(a, b, method="pearson"):
+    """Calculate correlation between two matrix, row by row, return 2D corr values"""
+    if not isinstance(a, np.ndarray):
+        a = a.values
+    if not isinstance(b, np.ndarray):
+        b = b.values
+
+    if method.lower()[0] == "p":
+        pass
+    elif method.lower()[0] == "s":
+        # turn a, b in to rank matrix
+        a = a.argsort(axis=1).argsort(axis=1)
+        b = b.argsort(axis=1).argsort(axis=1)
+    else:
+        raise ValueError("Method can only be pearson or spearman")
+
+    return _corr_all(a, b)
+
+
+def corr_rows(a, b, method="pearson"):
+    """Calculate correlation between the same rows in two matrix, return 1D corr values"""
+    if not isinstance(a, np.ndarray):
+        a = a.values
+    if not isinstance(b, np.ndarray):
+        b = b.values
+
+    if method.lower()[0] == "p":
+        pass
+    elif method.lower()[0] == "s":
+        # turn a, b in to rank matrix
+        a = a.argsort(axis=1).argsort(axis=1)
+        b = b.argsort(axis=1).argsort(axis=1)
+    else:
+        raise ValueError("Method can only be pearson or spearman")
+
+    return _corr_row(a, b)
+
+
 def _corr_preprocess(da, sample_mch, sample_mcg, cpu=1):
     imputer = SimpleImputer(copy=False)
     df = da.to_pandas()
     imputer.fit_transform(df)
     assert df.isna().values.sum() == 0
 
     adata = anndata.AnnData(
@@ -83,15 +170,15 @@
 
     # remove dmr that has 0 std
     # otherwise regress out will fail.
     adata = adata[:, adata.X.std(axis=0) > 0].copy()
 
     if adata.shape[1] > 0:
         # regress out global mCH and mCG
-        # happens on each regions
+        # happens on each region
         sc.pp.regress_out(adata, keys=["sample_mch", "sample_mcg"], n_jobs=cpu)
         sc.pp.scale(adata)
     else:
         print("All features are removed due to 0 std")
     return adata
 
 
@@ -100,14 +187,38 @@
     adata_b,
     max_dist,
     cpu=1,
     method="pearson",
     shuffle_sample=None,
     calculate_n=None,
 ):
+    """
+    Calculate correlation between two anndata, var by var
+
+    Parameters
+    ----------
+    adata_a
+        anndata a
+    adata_b
+        anndata b
+    max_dist
+        max distance between two regions
+    cpu
+        number of cpu to use
+    method
+        correlation method, pearson or spearman
+    shuffle_sample
+        shuffle sample order, for null correlation
+    calculate_n
+        only calculate n regions, for null correlation
+
+    Returns
+    -------
+    adata contains correlation matrix, shape (n_vars_a, n_vars_b)
+    """
     _adata_a = adata_a.copy()
     _adata_b = adata_b.copy()
 
     # trigger njit
     _corr(np.array([[0, 1]]), np.array([[0, 1]]), np.array([0]), np.array([0]))
 
     # this is used when null type is sample
@@ -116,15 +227,15 @@
         np.random.shuffle(obs_names)
         _adata_a.obs_names = obs_names
         _adata_a = _adata_a[_adata_b.obs_names, :]
 
     # create mask
     mask = coo_matrix(np.abs(_adata_a.var["pos"].values[:, None] - _adata_b.var["pos"].values[None, :]) < max_dist)
 
-    # this is used when calculating null, downsample corr call to save time
+    # this is used when calculating null, down sample corr call to save time
     if (calculate_n is not None) and (calculate_n < mask.data.size):
         rand_loc = np.random.choice(range(mask.data.size), size=int(calculate_n), replace=False)
         rand_loc = sorted(rand_loc)
         mask = coo_matrix(
             (mask.data[rand_loc], (mask.row[rand_loc], mask.col[rand_loc])),
             shape=mask.shape,
         )
```

### Comparing `ALLCools-1.0.8/ALLCools/mcds/mcds.py` & `allcools-1.1.0/ALLCools/mcds/mcds.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         if engine is None:
             engine = determine_engine(_final_paths)
 
         if len(_final_paths) == 1:
             ds = xr.open_dataset(
                 _final_paths[0],
                 engine=engine,
-                **kwargs
+                **kwargs,
                 # chunks=chunks  # do not apply chunks parameter here, apply in the end
             )
         else:
             with dask.config.set(**{"array.slicing.split_large_chunks": split_large_chunks}):
                 kwargs["coords"] = coords
                 kwargs["compat"] = compat
                 ds = xr.open_mfdataset(
@@ -406,31 +406,31 @@
             cov_da=da_cov,
             var_dim=var_dim,
             normalize_per_cell=normalize_per_cell,
             clip_norm_value=clip_norm_value,
         )
         return frac
 
-    def add_m_value(self, var_dim=None, da=None, alpha=0.01, normalize_per_cell=True, da_suffix="mvalue"):
+    def add_m_value(self, var_dim=None, da=None, alpha=0.01, da_suffix="mvalue"):
         """
         Add m value data array for certain feature type (var_dim).
 
         M-Value is a transformation of the posterior mC fraction data array to a log ratio scale.
         M = np.log2((frac + alpha) / (1 - frac + alpha)).
 
+        No normalization is applied to M-Value.
+
         Parameters
         ----------
         var_dim :
             Name of the feature type
         da :
             DataArray name. if None, will use f'{var_dim}_da'
         alpha :
             alpha value for the transformation regularization
-        normalize_per_cell :
-            if True, will normalize the mC rate data array per cell
         da_suffix :
             name suffix appended to the calculated mC rate data array
         """
         var_dim = self._verify_dim(var_dim, mode="var")
 
         if da is None:
             if var_dim is None:
@@ -441,17 +441,14 @@
         if var_dim not in self[da].dims:
             raise KeyError(f"{var_dim} is not a dimension of {da}")
 
         frac = self._calculate_frac(var_dim=var_dim, da=da, normalize_per_cell=False, clip_norm_value=None)
 
         m_value = np.log2((frac + alpha) / (1 - frac + alpha))
 
-        if normalize_per_cell:
-            m_value = m_value / m_value.mean(dim=var_dim)
-
         self[da + "_" + da_suffix] = m_value
         return
 
     def add_mc_rate(self, *args, **kwargs):
         """Add mC fraction data array (Deprecated)."""
         warnings.warn(
             'MCDS.add_mc_rate is renamed to MCDS.add_mc_frac, the default suffix also changed from "rate" to "frac"',
@@ -661,15 +658,14 @@
             return name2
         raise KeyError(f"{name1} or {name2} not found in MCDS.")
 
     def calculate_hvf_svr(
         self, mc_type=None, var_dim=None, obs_dim=None, n_top_feature=5000, da_name=None, da_suffix="frac", plot=True
     ):
         """Calculate the highly variable features (hvf) with the Support Vector Regression model."""
-        import plotly.graph_objects as go
         from sklearn.svm import SVR
 
         obs_dim = self._verify_dim(obs_dim, mode="obs")
         var_dim = self._verify_dim(var_dim, mode="var")
 
         if da_name is None:
             da_name = f"{var_dim}_da"
@@ -736,14 +732,21 @@
         print(f"Total Feature Number:     {judge.size}")
         print(
             f"Highly Variable Feature:  {selected_feature_index.size} "
             f"({(selected_feature_index.size / judge.size * 100):.1f}%)"
         )
 
         if plot:
+            try:
+                import plotly.graph_objects as go
+            except ImportError:
+                print("Please install plotly to enable plotting.")
+            plot = False
+
+        if plot:
             if hvf_df.shape[0] > 5000:
                 plot_data = hvf_df.sample(5000)
             else:
                 plot_data = hvf_df
             fig = go.Figure(
                 data=[
                     go.Scatter3d(
```

### Comparing `ALLCools-1.0.8/ALLCools/mcds/region_ds.py` & `allcools-1.1.0/ALLCools/mcds/region_ds.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,14 +377,16 @@
                 chrom_size_path=chrom_size_path,
                 engine=engine,
             )
 
         if use_regions is not None:
             region_ds = region_ds.sel({region_dim: use_regions})
 
+        # TODO: check the chunk issue of RegionDS.open
+        # the open function do not preserve the chunk information from zarr
         if chunks is not None:
             # change object dtype to string
             if obj_to_str:
                 for k in region_ds.coords.keys():
                     if region_ds.coords[k].dtype == "O":
                         region_ds.coords[k] = region_ds.coords[k].astype(str)
```

### Comparing `ALLCools-1.0.8/ALLCools/mcds/utilities.py` & `allcools-1.1.0/ALLCools/mcds/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,18 +463,19 @@
         if v.dtype == "O":
             coord_ds.coords[k] = v.astype(str)
     temp_zarr_path = f"{ds_path}_temp.zarr"
     coord_ds.to_zarr(temp_zarr_path, mode="w")
 
     # move previous coords and zmetadata
     for coord in coord_ds.coords.keys():
-        subprocess.run(["mv", f"{ds_path}/{coord}", f"{temp_zarr_path}/{coord}_backup"], check=True)
+        subprocess.run(["cp", "-r", f"{ds_path}/{coord}", f"{temp_zarr_path}/{coord}_backup"], check=True)
+        subprocess.run(["rm", "-rf", f"{ds_path}/{coord}"], check=True)
     # move new coords
     for coord in coord_ds.coords.keys():
-        subprocess.run(["mv", f"{temp_zarr_path}/{coord}", f"{ds_path}/{coord}"], check=True)
+        subprocess.run(["cp", "-r", f"{temp_zarr_path}/{coord}", f"{ds_path}/{coord}"], check=True)
 
     # zmetadata path
     old_zmetadata_path = f"{ds_path}/.zmetadata"
     new_zmetadata_path = f"{temp_zarr_path}/.zmetadata"
     # load both zmetadata
     with open(old_zmetadata_path) as f:
         zmeta_tmp = json.load(f)
```

### Comparing `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme` & `allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv` & `allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv` & `allcools-1.1.0/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/motif/motifs.py` & `allcools-1.1.0/ALLCools/motif/motifs.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/motif/parse_meme.py` & `allcools-1.1.0/ALLCools/motif/parse_meme.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/motif/snakemake.py` & `allcools-1.1.0/ALLCools/motif/snakemake.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/categorical_scatter.py` & `allcools-1.1.0/ALLCools/plot/categorical_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/color.py` & `allcools-1.1.0/ALLCools/plot/color.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/continuous_scatter.py` & `allcools-1.1.0/ALLCools/plot/continuous_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/contour.py` & `allcools-1.1.0/ALLCools/plot/contour.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/decomposition.py` & `allcools-1.1.0/ALLCools/plot/decomposition.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/dendro.py` & `allcools-1.1.0/ALLCools/plot/dendro.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/genome_track/GtfTrack.py` & `allcools-1.1.0/ALLCools/plot/genome_track/GtfTrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py` & `allcools-1.1.0/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/genome_track/_pygenometrack.py` & `allcools-1.1.0/ALLCools/plot/genome_track/_pygenometrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/qc_plots.py` & `allcools-1.1.0/ALLCools/plot/qc_plots.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/size.py` & `allcools-1.1.0/ALLCools/plot/size.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/sunburst.py` & `allcools-1.1.0/ALLCools/plot/sunburst.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/text_anno_scatter.py` & `allcools-1.1.0/ALLCools/plot/text_anno_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/plot/utilities.py` & `allcools-1.1.0/ALLCools/plot/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,7 +247,25 @@
     elif n < 4000000:
         s = 0.05
     elif n < 5000000:
         s = 0.03
     else:
         s = 0.02
     return s
+
+
+def sync_xylim_width(ax):
+    """Sync x and y axis limit to make them have the same width."""
+    xmin, xmax = ax.get_xlim()
+    ymin, ymax = ax.get_ylim()
+    xdelta = xmax - xmin
+    ydelta = ymax - ymin
+    flank = abs(xdelta - ydelta) / 2
+    if xdelta > ydelta:
+        ymin -= flank
+        ymax += flank
+        ax.set_ylim(ymin, ymax)
+    else:
+        xmin -= flank
+        xmax += flank
+        ax.set_xlim(xmin, xmax)
+    return
```

### Comparing `ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_kmeans.py` & `allcools-1.1.0/ALLCools/pseudo_cell/pseudo_cell_kmeans.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_knn.py` & `allcools-1.1.0/ALLCools/pseudo_cell/pseudo_cell_knn.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
                 pulp = pulp.flatten()
 
                 if (
                     (dist_thresh is None)
                     or ((min_pulp_size is None) and (dists < dist_thresh).all())
                     or ((min_pulp_size is not None) and (dists < dist_thresh).sum() >= min_pulp_size)
                 ):
-
                     if len(set(pulp) - set(unused)) / len(pulp) <= ovlp_tol:
                         kernels.append(kernel)
                         pulps.append(pulp)
                         unused -= set(pulp)
                         changed = True
                         break
             if not changed:
```

### Comparing `ALLCools-1.0.8/ALLCools/reptile/reptile.py` & `allcools-1.1.0/ALLCools/reptile/reptile.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/schema/mcds_schema.py` & `allcools-1.1.0/ALLCools/schema/mcds_schema.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/table_to_allc.py` & `allcools-1.1.0/ALLCools/table_to_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/ALLCools/utilities.py` & `allcools-1.1.0/ALLCools/utilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/LICENSE` & `allcools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.8/pyproject.toml` & `allcools-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     { name = "Hanqing Liu", email = "hanliu@salk.edu" },
     { name = "Jingtian Zhou", email = "jzhou@salk.edu" },
     { name = "Wei Tian", email = "wtian@salk.edu" }
 ]
 urls.Documentation = "https://lhqing.github.io/ALLCools/intro.html"
 urls.Source = "https://github.com/lhqing/ALLCools"
 urls.Home-page = "https://github.com/lhqing/ALLCools"
-version = "1.0.8"
+version = "1.1.0"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 readme = "README.md"
 dependencies = [
     "anndata",
     "numpy",
     'matplotlib',
@@ -40,15 +40,14 @@
     "biopython",
     "dask",
     "numba",
     "imblearn",
     "leidenalg",
     "networkx",
     "opentsne",
-    "plotly",
     "pynndescent",
     "scanpy",
     "scikit-learn",
     "statsmodels",
     "rpy2",
     "tpot",
     "cooler"
```

### Comparing `ALLCools-1.0.8/PKG-INFO` & `allcools-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLCools
-Version: 1.0.8
+Version: 1.1.0
 Summary: Toolkit for single-cell DNA methylome and multiomic data analysis.
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanliu@salk.edu>, Jingtian Zhou <jzhou@salk.edu>, Wei Tian <wtian@salk.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: anndata
 Requires-Dist: numpy
@@ -20,15 +20,14 @@
 Requires-Dist: biopython ; extra == "analysis"
 Requires-Dist: dask ; extra == "analysis"
 Requires-Dist: numba ; extra == "analysis"
 Requires-Dist: imblearn ; extra == "analysis"
 Requires-Dist: leidenalg ; extra == "analysis"
 Requires-Dist: networkx ; extra == "analysis"
 Requires-Dist: opentsne ; extra == "analysis"
-Requires-Dist: plotly ; extra == "analysis"
 Requires-Dist: pynndescent ; extra == "analysis"
 Requires-Dist: scanpy ; extra == "analysis"
 Requires-Dist: scikit-learn ; extra == "analysis"
 Requires-Dist: statsmodels ; extra == "analysis"
 Requires-Dist: rpy2 ; extra == "analysis"
 Requires-Dist: tpot ; extra == "analysis"
 Requires-Dist: cooler ; extra == "analysis"
```

